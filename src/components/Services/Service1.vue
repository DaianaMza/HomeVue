<script>
import styles from '../../styles'

const { flexCenter, paddingY, } = styles;
export default {
    data() {
        return {
            paddingY, flexCenter,

        };
    },
};
</script>

<template>
    <div>

        <div className="w-full max-w-6xl mx-auto">

            <div className="-mx-3 md:flex items-start">
                <div className="px-3 md:w-1/3">
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO 9001:2015 (Sistemas de
                                    Gestión de la calidad)</h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO/IEC 17025 (Calidad en
                                    laboratorio de ensayo y de calibración)</h6>
                            </div>
                        </div>
                    </div>

                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO 45001:2018 (sistema de
                                    gestión de la seguridad y salud en el trabajo)</h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600"> Norma ISO 39001:2012 E IRAM
                                    3810:2006 (Sistemas de Gestión de la Seguridad Vial)</h6>
                            </div>
                        </div>
                    </div>
                </div>

                <div className="px-3 md:w-1/3">
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO 27001:2013 (Sistema de
                                    Gestión de Seguridad de la Información)</h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">

                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO 14001:2015 (Sistema de
                                    Gestión Ambiental)</h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Protocolo de Bioseguridad </h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600"> HACCP- Análisis de peligros y
                                    puntos críticos de control </h6>
                            </div>
                        </div>
                    </div>

                </div>
                <div className="px-3 md:w-1/3">
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma ISO 50001:2018 (Sistema de
                                    gestión de la Energía).</h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">Norma RSE / SMETA (Responsabilidad
                                    Social Empresarial)</h6>
                            </div>
                        </div>
                    </div>

                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">BPM (Buenas prácticas de
                                    Manufactura) </h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                        <div className="w-full flex mb-4 items-center">
                            <div className="flex-grow pl-3">
                                <h6 className="font-bold text-sm uppercase text-gray-600">ISO 22000 (Sistema de Gestión de
                                    Seguridad Alimentaria) </h6>
                            </div>
                        </div>
                    </div>
                    <div
                        className="w-full mx-auto rounded-lg bg-white border border-gray-200 p-5 text-gray-800 font-light mb-6">
                    <div className="w-full flex mb-4 items-center">
                        <div className="flex-grow pl-3">
                            <h6 className="font-bold text-sm uppercase text-gray-600">BRC (Food Safety) </h6>
                        </div>
                    </div>
                </div>


            </div>


        </div>



    </div>

</div></template>
  

  
<style scoped></style>