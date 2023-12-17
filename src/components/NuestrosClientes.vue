<script>
export default {
    data() {
        return {};
    },
};
</script>

<template>
    <div>
        <section className="bg-blue-light z-depth-1 z-shadow">
            <div className="container mx-auto border-b">
                <div className="text-center pb-6">
                    <h1 className="text-3xl font-semibold mt-6 text-white">Nuestros Clientes:</h1>
                    <p className="mb-4 text-lg font-semibold text-white">
                        Generar una sinergia laboral con nuestros clientes que permita a través de acciones estratégicas
                        sustentables,
                        aumentar su rendimiento competitivo e imagen frente a la sociedad.
                    </p>
                    <div className="slider ">
                        <div className="slide-track">
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-16.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-17.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-18.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-20.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-1.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-2.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-4.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-5.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-6.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-7.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-3.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-8.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-9.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-10.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-11.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-12.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-13.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-14.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-15.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-16.png"
                                    height="100" width="250" alt="" />
                            </div>
                            <div className="slide">
                                <img src="http://www.grupo-kairos.com/default-theme/images/new_clients/cliente-18.png"
                                    height="100" width="250" alt="" />
                            </div>
                        </div>
                    </div>

                </div>

            </div>
        </section>
    </div>
</template>
  

  
<style scoped>
.img {
    padding: 5px;
}

@keyframes scroll {
    0% {
        transform: translateX(0);
    }

    100% {
        transform: translateX(calc(-250px * 7));
    }
}

.slider {
    background: white;
    box-shadow: 0 10px 20px -5px rgba(0, 0, 0, .125);
    height: 100px;
    margin: auto;
    overflow: hidden;
    position: relative;
    width: 960px;
}

.slider::before,
.slider::after {
    background: linear-gradient(to right, rgba(255, 255, 255, 1) 0%, rgba(255, 255, 255, 0) 100%);
    content: "";
    height: 100px;
    position: absolute;
    width: 200px;
    z-index: 2;
}

.slider::after {
    right: 0;
    top: 0;
    transform: rotateZ(180deg);
}

.slider::before {
    left: 0;
    top: 0;
}

.slider .slide-track {
    animation: scroll 40s linear infinite;
    display: flex;
    width: calc(250px * 14);
}

.slider .slide {
    height: 100px;
    width: 250px;
}
</style>