<template>
    <HeroRow text-alignment="center">
        <b-h level="2">Key Benefits</b-h>
        <b-p text-color="secondary">
            Discover why over 100,000 users love our platform
        </b-p>
    </HeroRow>

    <Row gutter="x-3" columns="1 md-2">
        <Col>
            <Card class="hover-translate shadow-sm bg-transparent">
                <Background 
                    img-src="/unsplash/image/480x220/dlxmedia-hu-U-W8FKeC6Mo-unsplash.jpg"
                    overlay="true"
                    overlay-color="white"
                    rounded
                >
                    <CardBody>
                        <CardTitle class="text-dark">Design Tools</CardTitle>
                        <CardText class="text-dark">
                            Access to advanced design techniques
                        </CardText>
                    </CardBody>
                    <CardFooter>
                        <CardLink to="/">
                            Browse tools
                            <BIcon class="ms-1" small icon="bi:chevron-right" />
                        </CardLink>
                    </CardFooter>
                </Background>
            </Card>
        </Col>

        <Col padding="y-3">
            <Row>
                <Col col="md-6">
                    <BIcon icon="bi:graph-up" class="text-primary fs-2" />
                    <b-h level="4">Interactive Dashboards</b-h>
                    <b-p text-color="secondary">
                        Visualize your ideas and turn them into beautiful designs.
                    </b-p>
                </Col>

                <Col col="md-6">
                    <BIcon icon="bi:bar-chart-fill" class="text-primary fs-2" />
                    <b-h level="4">Management Center</b-h>
                    <b-p text-color="secondary">
                        Organize and map out your projects efficiently.
                    </b-p>
                </Col>

                <Col col="md-6">
                    <BIcon icon="bi:lightbulb-fill" class="text-primary fs-2" />
                    <b-h level="4">Data Insights</b-h>
                    <b-p text-color="secondary">
                        Gain deep insights into your data with our analytics engine.
                    </b-p>
                </Col>

                <Col col="md-6">
                    <BIcon icon="bi:lightning-charge-fill" class="text-primary fs-2" />
                    <b-h level="4">Custom Analytics</b-h>
                    <b-p text-color="secondary">
                        Generate custom reports tailored to your business needs.
                    </b-p>
                </Col>
            </Row>
        </Col>
    </Row>
</template>
