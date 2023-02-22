<template>
    <ClientOnly>
        <div class=" w-[42rem] m-auto mt-10 p-8 border rounded-2xl bg-slate-200 ">
            <h1 class="font-semibold text-blue-600"># Task Brief</h1>
            <p>This is a Vue.js code that creates a form with two dropdown menus, where the first dropdown contains a list
                of main categories, and the second dropdown shows subcategories based on the main category selected. Once
                the user selects a subcategory, the form will dynamically generate a set of properties based on the
                subcategory selected.</p>
            <p>The properties consist of a label for each property and an input field (either a dropdown or text field),
                depending on whether the property has predefined options or not. The user can either select an option from
                the dropdown or enter their own value in the text field.</p>
            <p>When the user clicks the "Submit" button, the form will display a table showing the selected values for each
                category and property.</p>
            <h1 class="font-semibold  text-blue-600 mt-10"># Unit Testing Scenarios</h1>
            <p> 1- Test that the main categories are correctly fetched from the API and mapped to an array of names:
            <ul>
                <li class="mt-3"> a) Set up a mock API response with a list of categories and their names.</li>
                <li class="mt-2"> b) Invoke the <span class="text-orange-600">resMap()</span> <span
                        class="text-red-500">function</span> with the mock
                    response.
                </li>
                <li class="mt-2"> c) Assert that the resulting <span class="text-green-600">mainCats[]</span> <span
                        class="text-blue-800">array</span> matches the expected array of category names.
                </li>
            </ul>
            </p>
            <p> 2- Test that the subcategories are correctly fetched and mapped to an array of names and IDs when a main
                category is selected:
            <ul>
                <li class="mt-3"> a) Set up a mock API response with a list of subcategories and their names and IDs for a
                    given main category.</li>
                <li class="mt-2"> b) Set the <span class="text-pink-600">selectedMain</span> value to the corresponding
                    category name.</li>
                <li class="mt-2"> c) Invoke the <span class="text-orange-600">findSubs()</span> <span
                        class="text-red-500">function.</span></li>
                <li class="mt-2"> d) Assert that the resulting <span class="text-green-600">subCats[]</span> and <span
                        class="text-green-600">subCatsIds[]</span> <span class="text-blue-800">arrays</span> match the
                    expected arrays of
                    subcategory names and IDs.</li>
            </ul>
            </p>
            <p> 3- Test that the properties are correctly fetched and mapped to an array of names and options when a
                subcategory is selected:
            <ul>
                <li class="mt-3"> a) Set up a mock API response with a list of properties and their names and options for a
                    given subcategory.</li>
                <li class="mt-2"> b) Set the <span class="text-pink-600">selectedSub</span> value to the corresponding
                    subcategory name.</li>
                <li class="mt-2"> c) Invoke the <span class="text-orange-600">findProps()</span> <span
                        class="text-red-500">function.</span></li>
                <li class="mt-2"> d) Assert that the resulting <span class="text-green-600">resProps[]</span> and <span
                        class="text-green-600">namesProps[]</span> <span class="text-blue-800">arrays</span> match the
                    expected arrays of
                    properties and their names, and that the optProps array contains the expected options for each property.
                </li>
            </ul>
            </p>
        </div>
        <div class="h-20"></div>
    </ClientOnly>
</template>

<script setup>


useHead({
    title: "Testing"
})

</script>