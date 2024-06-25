<template>
    <div>
        <div class="offer-search"></div>

        <div class="offer-list"></div>
    </div>
</template>

<script>
import axios from 'axios';

export default {
    name: 'OfferList',
    methods: {
        async loadOffers() {
            try {
                const response = await axios.get('offers.json');
                this.offers = response.data;
            } catch (error) {
                console.error(error);
            }
        }
    },
    data() {
        return {
            offers: null,
            search: '',
        }
    },
}
</script>