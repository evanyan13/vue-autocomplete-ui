<template>
    <div class="autocomplete-ui">
      <CioAutocomplete v-bind="args" />
    </div>
</template>

<script>
import { CioAutocomplete } from '@constructor-io/constructorio-ui-autocomplete';

export default {
    components: {
        CioAutocomplete,
    },
    data() {
        return {
            args: {
                "apiKey": "key_JjeChOYODg7w5dYg",
                "onSubmit": (submitEvent) => console.dir(submitEvent),
                "autocompleteClassName": "cio-autocomplete full-example-autocomplete-styles",
                "placeholder": "What can we help you find?",
                "advancedParameters": {
                    "displaySearchSuggestionImages": true,
                    "displaySearchSuggestionResultCounts": true,
                    "numTermsWithGroupSuggestions": 6
                },
                "sections": [
                    {
                    "indexSectionName": "Search Suggestions",
                    "numResults": 8,
                    "displaySearchTermHighlights": true
                    },
                    {
                    "indexSectionName": "Products",
                    "numResults": 6,
                    "displaySearchTermHighlights": true
                    }
                ],
                "zeroStateSections": [
                    {
                    "podId": "bestsellers",
                    "type": "recommendations",
                    "numResults": 6
                    }
                ]
            }
        }
    }
};
</script>

<style>
</style>