## API Report File for "@alexa-travel-guides/specifications"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { Attraction } from '@alexa-travel-guides/entities';
import { Restaurant } from '@alexa-travel-guides/entities';

// @public (undocumented)
export class AttractionNameSpecification extends Specification<Attraction> {
    constructor(name: string);
}

// @public (undocumented)
export interface ISpecification<T> {
    // (undocumented)
    isSatisfiedBy(entity: T): boolean;
}

// @public (undocumented)
export class RestaurantMealsSpecification extends Specification<Restaurant> {
    constructor(meal: string);
}

// @public (undocumented)
export abstract class Specification<T> implements ISpecification<T> {
    protected constructor(predicate: (entity: T) => boolean);
    // (undocumented)
    isSatisfiedBy(entity: T): boolean;
    // (undocumented)
    protected predicate: (entity: T) => boolean;
}


// (No @packageDocumentation comment for this package)

```
