<template>

    <thead>
    <tr>
        <th v-for="key in $parent.gridColumns"
            @click="$parent.sortBy(key)"
            v-bind:class="{active: $parent.sortKey == key}">

            {{ key }}

            <span class="arrow"

                  v-bind:class="$parent.sortOrder > 0 ? 'asc' : 'dsc'">

                                </span>

        </th>

        <th>Actions</th>

    </tr>
    </thead>

</template>