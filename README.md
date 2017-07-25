# DiverseHeterogeneousAdapter

[ ![Download](https://api.bintray.com/packages/khang-nt/maven/DiverseHeterogeneousAdapter/images/download.svg) ](https://bintray.com/khang-nt/maven/DiverseHeterogeneousAdapter/_latestVersion)

DiverseHeterogeneousAdapter is a fork version of _marverenic/HeterogeneousAdapter_, you can find the description here:   https://github.com/marverenic/HeterogeneousAdapter
> HeterogeneousAdapter is an implementation of `RecyclerView.Adapter` designed for easily creating lists with different views for different types of data. In a regular RecyclerView Adapter, you would have to override `getItemViewType()`, `onCreateViewHolder()`, and `onBindViewHolder()` manually to deal with combined data sets. For lists that have one or two data types this is no big deal, but when several different data types need to be displayed in a single list, `onBindViewHolder` can become a tangled mess to figure out the correct indices for data in a particular collection, in particular if the list has something like headers that disappear when their corresponding section is empty.
>
> `HeterogeneousAdapter` completely removes the need to override these methods. This is done by separating
the data into Sections. Each Section behaves very much like a regular RecyclerView adapter, but _**each
Section can only have one view type. Sections cannot be interwoven with each other**_.
Heterogeneous Adapter also includes an EmptyState interface.

DiverseHeterogeneousAdapter reimplement `HeterogeneousAdapter` in order to make it more flexible in some certain cases.
The data is also separated into Sections, but each Section can have more than one view type and can share the view type with other sections.

## Gradle Installation
```
dependencies {
    compile 'org.khangnt.diverseheterogeneousadapter:lib:0.1'
}
```

## Example
Example code is available at [sample](sample).

## License
DiverseHeterogeneousAdapter is distributed under an Apache 2.0 License.