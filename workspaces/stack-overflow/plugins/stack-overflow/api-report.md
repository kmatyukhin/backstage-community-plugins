## API Report File for "@backstage-community/plugin-stack-overflow"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
/// <reference types="react" />

import { ApiRef } from '@backstage/core-plugin-api';
import { BackstagePlugin } from '@backstage/core-plugin-api';
import { CardExtensionProps } from '@backstage/plugin-home-react';
import { JSX as JSX_2 } from 'react';
import { default as React_2 } from 'react';
import type { ResultHighlight } from '@backstage/plugin-search-common';
import { SearchResultListItemExtensionProps } from '@backstage/plugin-search-react';

// @public
export const HomePageStackOverflowQuestions: (
  props: CardExtensionProps<StackOverflowQuestionsContentProps>,
) => JSX_2.Element;

// @public (undocumented)
export type StackOverflowApi = {
  listQuestions(options?: {
    requestParams: StackOverflowQuestionsRequestParams;
  }): Promise<StackOverflowQuestion[]>;
};

// @public (undocumented)
export const stackOverflowApiRef: ApiRef<StackOverflowApi>;

// @public
export const StackOverflowIcon: () => React_2.JSX.Element;

// @public
export const stackOverflowPlugin: BackstagePlugin<{}, {}>;

// @public
export type StackOverflowQuestion = {
  title: string;
  link: string;
  owner: Record<string, string>;
  tags: string[];
  answer_count: number;
};

// @public
export type StackOverflowQuestionsContentProps = {
  requestParams: StackOverflowQuestionsRequestParams;
  icon?: React.ReactNode;
};

// @public
export type StackOverflowQuestionsRequestParams = {
  [key: string]: string | string[] | number;
};

// @public
export const StackOverflowSearchResultListItem: (
  props: SearchResultListItemExtensionProps<StackOverflowSearchResultListItemProps>,
) => JSX.Element | null;

// @public
export type StackOverflowSearchResultListItemProps = {
  result?: any;
  icon?: React_2.ReactNode;
  rank?: number;
  highlight?: ResultHighlight;
};
```