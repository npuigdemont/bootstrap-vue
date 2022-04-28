<template>
    <div class="m-3">
        <h1>
            Formularis
        </h1>

        <form>
            <b-row>
                <b-col md="3">
                     <b-form-input type="text" class="mb-3" v-model="text" :state="comprovar"></b-form-input>
                     <small>Mímim 3 caràcters</small>
                     <p>Text: {{text}}</p>
                </b-col>

                <b-col md="3">
                    <b-form-select class="mb-3" v-model="select" :options="proves"></b-form-select>
                    <p>Selecció: {{select}}</p>
                </b-col>

                 <b-col md="3">
                     <b-form-radio-group class="mb-3" v-model="radio" :options="provesRadio"> </b-form-radio-group>
                     <p>Selecció: {{radio}}</p>
                 </b-col>

                 <b-col md="3">
                     <b-form-checkbox-group class="mb-3" v-model="check" :options="provesRadio"> </b-form-checkbox-group>
                     <p>Selecció: {{check}}</p>
                 </b-col>
            </b-row>
            
        </form>
        
    </div>
</template>

<script>
export default {
    name:'Form',
    data(){
        return {
            text:'',
            check: [],
            radio: null,
            select: null,
            proves: [
                {value: null, text: 'Selecciona una opció'},
                {value: 'opcio 1', text: ' Selecciona una altra opció'},
                {value: 'opcio 2', text: ' Selecciona i una altra opció'},
                {value: 'opcio 3', text: ' I una més'},
            ],
            provesRadio: [
                {value: 'opcio 1', text: ' Selecciona una altra opció'},
                {value: 'opcio 2', text: ' Selecciona i una altra opció'},
                {value: 'opcio 3', text: ' I una més'}
            ]
        }
    },
    computed: {
        comprovar(){
            return this.text.length > 2 ? true : false;
        }
    }
}
</script>