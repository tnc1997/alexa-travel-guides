## API Report File for "@alexa-travel-guides/services"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { Attraction } from '@alexa-travel-guides/entities';
import { IAttractionRepository } from '@alexa-travel-guides/repositories';
import { IRepository } from '@alexa-travel-guides/repositories';
import { IRestaurantRepository } from '@alexa-travel-guides/repositories';
import { ISpecification } from '@alexa-travel-guides/specifications';
import { Restaurant } from '@alexa-travel-guides/entities';

// @public (undocumented)
export class AttractionService extends Service<Attraction> implements IAttractionService {
    constructor(attractionRepository: IAttractionRepository);
}

// @public (undocumented)
export interface IAttractionService extends IService<Attraction> {
}

// @public (undocumented)
export interface IRestaurantService extends IService<Restaurant> {
}

// @public (undocumented)
export interface IService<T> {
    // (undocumented)
    get(): Promise<T[]>;
    // (undocumented)
    get(specification: ISpecification<T>): Promise<T[]>;
}

// @public (undocumented)
export class RestaurantService extends Service<Restaurant> implements IRestaurantService {
    constructor(restaurantRepository: IRestaurantRepository);
}

// @public (undocumented)
export abstract class Service<T> implements IService<T> {
    protected constructor(repository: IRepository<T>);
    // (undocumented)
    get(): Promise<T[]>;
    // (undocumented)
    get(specification: ISpecification<T>): Promise<T[]>;
    }


// (No @packageDocumentation comment for this package)

```
