<script>
export default {
    name: "SezioneRegistrazione"

}

</script>

<template>
    <div class="cont">
        <div class="box-registrazione">
            <div>
                <span> send a message</span>
                <h2>Get in <span>touch</span></h2>
                <p>We will respond to youre message soon as possible</p>
                <div class="row">
                    <div class="col">
                        <input type="text" class="form-control" placeholder=" Name" aria-label="">
                        <input type="text" class="form-control" placeholder="Email" aria-label="">
                    </div>
                    <div class="col">
                        <input type="text" class="form-control" placeholder="Phone" aria-label="">
                        <input type="text" class="form-control" placeholder="More info" aria-label="">
                    </div>
                    <div class="input-group pt-1">
                        <textarea class="form-control" aria-label="With textarea" placeholder="Inserisci testo"></textarea>
                    </div>
                </div>
            </div>
        </div>

        <div class="box-contatti">
            <div class="text">
                <h3>Examole Inc.</h3>
                <p>Lorem iosum dolor sit, consectetur adipiscing elit</p>
                <p>Lorem iosum dolor sit, consectetur adipiscing elit</p>
            </div>
            <div class="contatti d-flex ">
                <span><i class="fa-solid fa-phone"></i> +1 (305) 1223-3456</span>
                <span><i class="fa-solid fa-envelope"></i> Hello@example.com</span>
                <span><i class="fa-solid fa-location-dot"></i> Main Avenue, 987</span>
                <a href="">view map</a>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.cont {
    display: flex;
    width: 70%;
    margin: 0 auto;
    padding: 50px 0;

    .box-registrazione {
        width: 60%;
        // display: flex;
        // justify-content: flex-end;

        div {
            span {
                color: #00A6A6;
            }

            h2 {
                span {
                    color: #058283;
                    background-color: #DAECED;
                }
            }

            .row {
                .col {
                    input {
                        margin: 8px 0;
                    }
                }

                .input-group {
                    height: 140px;
                }
            }
        }

    }

    .box-contatti {
        width: 40%;
        padding: 20px 0 20px 35px;

        .contatti {
            display: flex;
            flex-direction: column;

            span {
                padding-top: 15px;

                i {
                    padding: 10px 10px;
                    background-color: #00A6A6;
                    border-radius: 50%;
                }
            }
        }

    }
}
</style>