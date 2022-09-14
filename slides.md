---
theme: ./theme
lineNumbers: false
class: text-center
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
drawings:
  persist: false
css: windicss
title: Artemis
layout: intro
---

# Artemis

## Explanation and exploration

<!--
You've heard the word thrown around and may not know what it is and what it entailed, so this is an attempt to dive into it
-->

---
layout: presenter
presenterImage: /greg-bt.jpeg
---

# Who am I?

Gregory Waxman, Staff Engineer @  <fancy-link href="https://intellimize.com">Intellimize</fancy-link>

<v-clicks>

* 15+ years doing JavaScript
* Frameworks used:
  * Homegrown contraptions
  * Angular
  * Built my own, <a href="https://github.com/Akkuma/Rome">Rome</a> + Papa
  * React (on & off since 2013)
    * MobX
    * Redux
  * Backbone
  * Elm

</v-clicks>

---
layout: center
---

 # Who made this happen?

<v-clicks>

<div class="flex gap-4 items-center">Justin Helmer <Pic imgclass="object-top" src="/justin.jpeg"/></div>
<div class="flex flex-row-reverse gap-4 items-center">Kevin Dam <Pic imgclass="object-top" src="/kevin.jpeg"/></div>
<div class="flex gap-4 items-center">Joe Parisi <Pic src="https://ca.slack-edge.com/T4FPS3JHK-U038NE6N12Q-3fea1f73032f-512"/></div>
<div class="flex flex-row-reverse gap-4 items-center">Anuj Pant <Pic imgstyle="object-position: 0 -4px" src="/anuj.jpeg"/></div>
<div class="flex gap-4 items-center">Chris Swasey <Pic imgstyle="object-position: 6px 0px" src="https://ca.slack-edge.com/T4FPS3JHK-U02TKLT0RK9-c8a09f43611a-512"/></div>
<div class="flex flex-row-reverse gap-4 items-center">Geng Li <Pic imgstyle="object-position: -2px -4px" src="/geng.jpeg"/></div>

</v-clicks>

---
layout: new-section
---

# So what is Artemis?

<div class="flex justify-center gap-2">
<img class="w-screen-sm" src="https://pbs.twimg.com/media/Eigm9joU0AALQxF.jpg:large" />
</div>

<!--
The goddess of the hunt, the wilderness, wild animals, nature, vegetation, childbirth, care of children, and chastity
-->

---
layout: new-section
---

# So what is Artemis?

<div class="flex justify-center">
<img class="w-400px" src="https://www.monkeyuser.com/assets/images/2022/245-small-delights.png" alt="Small Delights" title="I’m not a great programmer; I’m just a good programmer with great habits. ― Martin Fowler">
</div>

<!--
The act of unraveling everything
-->

---
layout: center
title: A lot
---

<div class="text-8xl">It is a lot</div>

---

# History of the World, Part 3

dv2 aka dashboard had grown long in the tooth.

There was a need to amp up development.
<style>
@keyframes strike{
  0%   { width : 0; }
  100% { width: 48ch; }
}
.strike {
  position: relative;
}
.strike.slidev-vclick-prior::after {
  content: ' ';
  position: absolute;
  background: red;
  top: 50%;
  left: 0;
  width: 0;
  translate: transform3d(-50%, 0, 0);
  height: 2px;
  animation-name: strike;
  animation-duration: 1s;
  animation-timing-function: linear;
  animation-iteration-count: 1;
  animation-fill-mode: forwards; 
  animation-delay: 1s;
}
</style>

<p v-click class="strike">The war against the hybrid zombie robots was about to commence.</p>


<v-clicks>

- Latest & greatest
- Faster & better dev experience
- Build upon previous lessons
- More unified dev patterns
- Improved customer experience 

</v-clicks>

<!--
Latest & greatest 
- Lots of outdated dependencies & tools
  - Including node

Faster & better dev experience
- Webpack 4 doesn't hold a candle to Webpack 5 or vite
  - Hot Module Reload, supplanted by Fast Refresh
    - Dev can work without full page refreshes in many cases

Build upon previous lessons
- Artemis went hand in hand with Apollo, which was to redevelop the customer experience
- Redevelopment of both functionality & design offered an opportunity to get our moonshot to land

More unified dev patterns
- I can't directly speak to this from my limited time in dv2
- Supposedly an evolution of ideas in various places, but never unified

Improved customer xp
- Speed is a feature and if you don't build for it you won't get it
-->

---
layout: center
class: text-center
---

# Sounds good, right?

<img class="w-500px" src="https://i.imgur.com/6ADLV4r.gif" />

---

# Rome wasn't built in a day

<p v-click>It was built in 2 weeks</p>

<v-click>

- Rapid PoC
- Rapid porting
- Rapid ideation
- Lots of conversations & calls
- Rapid rapid

</v-click>

<!--
Speedrunning competition 
-->
---
layout: new-section
---

# Tech stack

<div class="flex justify-center"><img style="clip-path: inset(0 0 20% 0)" class="w-100" src="https://i.kym-cdn.com/photos/images/newsfeed/001/513/012/625.jpg" /></div>
---

# Latest & Greatest

<div class="flex justify-between">

- Vite
- Valtio
- React (didn't change)
- Vitest
- Visx
- Windicss
- New directory structure

<div class="overflow-scroll h-400px max-w-1/2 flex-1">
```json
 "dependencies": {
    "@amcharts/amcharts4": "^4.10.25",
    "@auth0/auth0-spa-js": "1.16.1",
    "@dnd-kit/core": "^6.0.5",
    "@dnd-kit/sortable": "^7.0.1",
    "@dnd-kit/utilities": "^3.2.0",
    "@fortawesome/fontawesome-svg-core": "^6.1.1",
    "@fortawesome/free-regular-svg-icons": "^6.1.1",
    "@fortawesome/free-solid-svg-icons": "^6.1.1",
    "@fortawesome/pro-duotone-svg-icons": "^6.1.1",
    "@fortawesome/pro-light-svg-icons": "^6.1.1",
    "@fortawesome/pro-regular-svg-icons": "^6.1.1",
    "@fortawesome/pro-solid-svg-icons": "^6.1.1",
    "@fortawesome/pro-thin-svg-icons": "^6.1.1",
    "@fortawesome/react-fontawesome": "^0.1.18",
    "@intellimize/customer": "^4.8.3",
    "@intellimize/fe-shared": "^2.17.0",
    "@intellimize/dash-shared": "^2.0.0",
    "@intellimize/logger": "^3.2.2",
    "@intellimize/optional": "^1.2.0",
    "@tanstack/react-query": "^4.2.1",
    "@tippyjs/react": "^4.2.6",
    "@visx/annotation": "^2.10.0",
    "@visx/axis": "^2.10.0",
    "@visx/group": "^2.10.0",
    "@visx/mock-data": "^2.1.2",
    "@visx/responsive": "^2.10.0",
    "@visx/scale": "^2.2.2",
    "@visx/shape": "^2.10.0",
    "@visx/tooltip": "^2.10.0",
    "@visx/xychart": "^2.10.0",
    "ace-builds": "1.4.14",
    "brace": "^0.11.1",
    "clsx": "^1.1.1",
    "date-fns": "^2.28.0",
    "date-fns-tz": "^1.3.1",
    "draft-js": "^0.11.7",
    "draft-js-export-html": "^1.4.1",
    "foundation-sites": "^6.7.4",
    "history": "^5.3.0",
    "jsdom": "^20.0.0",
    "lodash-es": "^4.17.21",
    "query-string": "^7.1.1",
    "react": "^17.0.2",
    "react-ace": "^9.5.0",
    "react-calendar": "^3.7.0",
    "react-dom": "^17.0.2",
    "react-error-boundary": "^3.1.4",
    "react-router-dom": "^6.2.2",
    "react-split": "^2.0.14",
    "react-spring": "^9.4.5",
    "react-time-picker": "^4.5.0",
    "react-toggle": "^4.1.2",
    "react-window": "^1.8.7",
    "use-constant": "^1.1.0",
    "valtio": "^1.5.0"
  },
  "devDependencies": {
    "@fortawesome/fontawesome-common-types": "^6.1.1",
    "@honkhonk/vite-plugin-svgr": "^1.1.0",
    "@nabla/vite-plugin-eslint": "^1.4.0",
    "@originjs/vite-plugin-commonjs": "^1.0.3",
    "@testing-library/react": "^12.1.4",
    "@testing-library/user-event": "^14.2.0",
    "@tsconfig/recommended": "^1.0.1",
    "@types/auth0": "^2.34.14",
    "@types/chrome": "0.0.158",
    "@types/debug": "^4.1.7",
    "@types/draft-js": "^0.11.9",
    "@types/lodash-es": "^4.17.6",
    "@types/node-fetch": "^2.6.2",
    "@types/react": "^17.0.33",
    "@types/react-calendar": "^3.5.0",
    "@types/react-dom": "^17.0.10",
    "@types/react-fontawesome": "^1.6.5",
    "@types/react-time-picker": "^4.0.2",
    "@types/react-toggle": "^4.0.3",
    "@types/react-window": "^1.8.5",
    "@types/ws": "^8.5.3",
    "@typescript-eslint/eslint-plugin": "^5.16.0",
    "@typescript-eslint/parser": "^5.27.1",
    "@unocss/reset": "^0.30.8",
    "@vitejs/plugin-react": "^1.0.7",
    "cypress": "^10.2.0",
    "dotenv": "^16.0.1",
    "eslint": "^8.17.0",
    "eslint-config-airbnb": "^19.0.4",
    "eslint-config-prettier": "^8.5.0",
    "eslint-import-resolver-alias": "^1.1.2",
    "eslint-plugin-chai-friendly": "^0.7.2",
    "eslint-plugin-cypress": "^2.12.1",
    "eslint-plugin-import": "^2.26.0",
    "eslint-plugin-jsx-a11y": "^6.5.1",
    "eslint-plugin-prettier": "^4.0.0",
    "eslint-plugin-react": "^7.29.4",
    "eslint-plugin-react-hooks": "^4.3.0",
    "eslint-plugin-testing-library": "^5.1.0",
    "happy-dom": "^5.0.0",
    "lint-staged": "^12.3.7",
    "mongodb": "^4.6.0",
    "msw": "^0.42.1",
    "prettier": "^2.6.1",
    "sass": "^1.49.9",
    "ts-toolbelt": "^9.6.0",
    "type-fest": "^2.19.0",
    "typescript": "^4.7.3",
    "unocss": "^0.30.8",
    "vite": "^2.8.0",
    "vite-esbuild-typescript-checker": "^0.0.1-alpha.9",
    "vite-plugin-environment": "^1.1.0",
    "vite-plugin-windicss": "^1.8.3",
    "vite-tsconfig-paths": "^3.4.1",
    "vitest": "^0.23.1",
    "windicss": "^3.5.1"
  }
```
</div>
</div>

<!--
Feel free to peruse all those dependencies, but the generally largest changes have been called out
-->

---
layout: center
class: text-center
---

# That's it?
<img class="w-screen-sm" src="https://i.kym-cdn.com/entries/icons/original/000/018/489/nick-young-confused-face-300x256-nqlyaa.jpg" />

<p v-click>Sort of</p>

---

# Mini dive into each

<v-clicks>

- Vite "Next Generation Frontend Tooling"
  - A replacement for Webpack 
- Valtio "Proxy state made simple"
  - A state management library
- Vitest "A Vite-native unit test framework"
  - A test runner built on top of vite
- Visx "a collection of expressive, low-level visualization primitives for React"
  - A low level library that allows you to build your own charting library/components
- Windicss "Next generation utility-first CSS framework"
  - CSS library that uses utility classes for styling purposes
- Flattened out directories for less nesting
  - Easier to find and easier to group related functionality

</v-clicks>

<!--
### Vite

- Easier and simpler to config
- Learnt from the lessons of webpack and skypack
- Built on the backs of rollup & esbuild

### Valtio

- A completely different paradigm for how to interact with state
- Built as a vanilla js library with integration points for React
- "New wave" of libraries written first as vanilla offering greater flexibility
  - https://faultlore.com/blah/c-isnt-a-language/
- You mutate state and only subscribers interested in that portion of state will get notified

### Vitest

- Avoids configuration hell that anyone who has worked with Jest can attest to
- Jest is dead
- We're already using Vite

### Visx

- Chosen because it is one of the lighter weight charting libraries out there
- Not forced into any pre-packaged charting solutions requiring putting squares into circles

### Windicss

- No separate stylesheets needed (styling lives alongside components)
- Outputs a css stylesheet
- Fast dev cycles

### Flat

- Pages contain their page specific components
- Pages can create modules for code separation and reduce file bloat

-->

---
layout: new-section
---

# Show me the money

<img style="clip-path: inset(20% 0 25% 0)" class="relative bottom-100px" v-click src="/ribs.jpeg" />

---
layout: text-window
---

# Old school

This is just one example of how we used to do things.

- Containers were separated out from pages
- Routing information was passed into components

::window::

```ts {all|3-7|8}
const ExperienceReportPageContainer: FunctionComponent<
  RouteComponentProps<{ experienceId: string; campaignId: string }>
> = ({
  match: {
    params: { experienceId, campaignId },
  },
}) => {
  const { account } = useContext(AccountContext);

  let experience: Experience | undefined;

  account.getCampaign(campaignId).ifPresent((campaign) => {
    campaign.getExperience(experienceId).ifPresent((exp) => {
      experience = exp;
    });
  });

  return experience ? <ExperienceReportPage account={account} experience={experience} /> : <ErrorPage type="404" />;
};

export default ExperienceReportPageContainer;
```

<!-- 
### Container

- Containers are components that hold business logic so that other components can be as close to pure as possible
  - Purity in this case is very similar to the functional concepts of same input -> same output

### Context

- We had redux mixed with Context

-->

---
layout: text-window
---

# Old school part 2

- Deeply integrated into React
- Using context with React's state

::window::

```ts {all|160-178} {maxHeight: '450px'}
export interface AccountContextStore {
  account: Customer;
  attributeDefinitions: AttributeDefinitions;
  isAuthorized: (permission: Permission) => boolean;
  fetchAccount(): Promise<Customer | void>;
  fetchAndUpdateAccount(): Promise<Customer | void>;
  isFeatureAuthorizedForUser: (feature: FeatureFlagKeys) => boolean;
  isFeatureAuthorizedForCustomer: (featureFlag: FeatureFlagKeys) => boolean;
  isFeatureAuthorized: (featureFlag: FeatureFlagKeys) => boolean;
}

// eslint-disable-next-line @typescript-eslint/ban-ts-comment
// @ts-ignore
export const AccountContext: Context<AccountContextStore> = React.createContext<AccountContextStore>();

export const AccountProvider: FunctionComponent = ({ children }) => {
  const builder = useRef(new CustomerBuilder());
  const accountList = useContext(AccountListContext);
  const { getTokenSilently, isAuthenticated, user, logout } = useAuth0();
  const [account, setAccount] = useState<Customer>();
  const [error, setError] = useState(false);
  const [customerFeatureFlags, setCustomerFeatureFlags] = useState<string[]>();
  const isAuthorized = useCallback(
    (permission) => {
      const accountId = account ? account.getId() : undefined;
      return auth.isAuthorized(user, permission, accountId);
    },
    [user, account]
  );

  // This method is checking whether a feature is accessible by an user.
  const isFeatureAuthorizedForUser = useCallback(
    (featureKey: FeatureFlagKeys): boolean => {
      if (user.authorization.globalFeatures[featureKey]) {
        return true;
      }
      if (account) {
        const featureMetaData = user.authorization.customers[account.getId()];
        return featureMetaData && featureMetaData.features ? !!featureMetaData.features[featureKey] : false;
      }
      return false;
    },
    [account, user.authorization.customers, user.authorization.globalFeatures]
  );

  // This method is checking whether a feature is accessible by a customer.
  const isFeatureAuthorizedForCustomer = useCallback(
    (featureFlag: FeatureFlagKeys): boolean => {
      if (featureFlag) {
        // If customerFeatureFlags is populated, show feature if the feature flag is presented
        if (customerFeatureFlags && customerFeatureFlags.length !== 0) {
          return customerFeatureFlags.includes(featureFlag);
        } // If customerFeatureFlags is unavailable, return false.
        return false;
      }

      return false;
    },
    [customerFeatureFlags]
  );

  // This method checks whether a feature is accessible from both customer & user level.
  const isFeatureAuthorized = (featureFlag: FeatureFlagKeys) => {
    return isFeatureAuthorizedForUser(featureFlag) || isFeatureAuthorizedForCustomer(featureFlag);
  };

  const {
    match: {
      params: { accountId: accountIdParam },
    },
  } = useReactRouter<{ accountId: string }>();

  const prevAccountIdParam = usePrevious(accountIdParam);
  const accountVersion = useRef<number | undefined>();
  const accountId = useRef<string | undefined>();
  const loading = useRef(false);

  const fetchAccount = useCallback(async (): Promise<Customer | undefined> => {
    return capturePromiseErrors(async (): Promise<Customer | undefined> => {
      if (!loading.current) {
        loading.current = true;
        const token = await getTokenSilently();

        const response = await fetch(`/api/v2/customers/${accountIdParam}`, {
          headers: {
            Authorization: `Bearer ${token}`,
          },
        });

        loading.current = false;
        let json;
        try {
          if (response.ok) {
            json = builder.current.build(await response.json());
          } else {
            throw new Error(`${response.status}: ${response.statusText}`);
          }
        } catch (e) {
          setError(true);
        }
        return json;
      }

      return undefined;
    });
  }, [accountIdParam, getTokenSilently]);

  // We use accountId and accountVersion as refs to track whether or not to update the account object whenever
  // fetchAndUpdateAccount is called. This is in place of checking the actual account object so that the fetchAndUpdateAccount dependency won't
  // change every time account is updated. This prevents double account calls in consumers that
  // call fetchAndUpdateAccount in a useEffect hook whenever self-serve changes are made.
  const fetchAndUpdateAccount = useCallback(async (): Promise<Customer | void> => {
    const newAccount = await fetchAccount();
    if (newAccount) {
      // only update the account if:
      // 1) this is the first render in which case accountId === undefined
      // 2) the account version in memory has a different version from the latest fetched newAccount
      // eslint-disable-next-line no-underscore-dangle
      if (!accountId.current || accountVersion.current !== newAccount.getVersion()) {
        setAccount(newAccount);
        accountVersion.current = newAccount.getVersion();
        accountId.current = newAccount.getId();
      } else {
        return undefined;
      }
    }
    return newAccount;
  }, [accountId, fetchAccount]);

  const fetchAppFeatureFlags = useCallback(async (): Promise<string[]> => {
    return capturePromiseErrors(async (): Promise<string[]> => {
      if (!loading.current && !!accountId.current) {
        loading.current = true;
        const token = await getTokenSilently();
        const response = await fetch(`/api/v2/feature-flags/${accountId.current}`, {
          headers: {
            Authorization: `Bearer ${token}`,
          },
        });

        loading.current = false;
        let json;
        try {
          if (response.ok) {
            json = await response.json();
            setCustomerFeatureFlags(json);
          } else {
            setCustomerFeatureFlags([]);
            throw new Error(`${response.status}: ${response.statusText}`);
          }
        } catch {
          setCustomerFeatureFlags([]);
        }
        return json;
      }

      return [];
    });
  }, [getTokenSilently]);

  useEffect(() => {
    // trigger hook on first load (prevAccountIdParam === undefined), or when accountId changes (user changes accounts)
    const isFirstMount = prevAccountIdParam === undefined;
    const isSwitchingAccounts = !isFirstMount && prevAccountIdParam !== accountIdParam;
    if (isAuthenticated && (isFirstMount || isSwitchingAccounts)) {
      if (!loading.current) {
        // Load feature flags after the real account object is acquired successfully.
        fetchAndUpdateAccount().then(fetchAppFeatureFlags);
      }
      // only set account, version, and id to undefined when switching accounts (prevents flash of content for when a forced refetch of account occurs
      if (isSwitchingAccounts) {
        accountVersion.current = undefined;
        accountId.current = undefined;
        setAccount(undefined);
        setCustomerFeatureFlags(undefined);
      }
    }
  }, [accountIdParam, fetchAndUpdateAccount, isAuthenticated, prevAccountIdParam, fetchAppFeatureFlags]);

  // Only set the customer domain value if it changes
  const customerDomainValue = account ? `${account.getId()}: ${account.getName()}` : undefined;
  useEffect(() => {
    if (customerDomainValue) {
      setGADomain(GADomains.CUSTOMER, customerDomainValue);
    }
  }, [customerDomainValue]);

  // If the logged in user does not have access to the current account context, redirect to the base page.
  // To prevent infinite loop in the case where a user no longer has access to a customer that is set as their default in localStorage, clear the default ID
  if (!accountList.find((acc) => acc.id === accountIdParam)) {
    clearDefaultAccountId(accountIdParam);
    return <Redirect to="/" />;
  }

  if (error) {
    logout();
  }

  // Between account transitions and while fetching the new account, the previous account id will not match the account id URL param so render null
  // to prevent the component tree for the previous account from briefly rendering
  // Also check whether customerFeatureFlags is populated before rendering children because they can largely depend on whether the shape of feature flags
  // either on successful/failed retrival. (undefined means the API call hasn't finished yet)
  if (account && accountIdParam === account.getId() && customerFeatureFlags !== undefined) {
    const store: AccountContextStore = {
      account,
      attributeDefinitions: builder.current.getAttributeDefinitions(),
      isAuthorized,
      isFeatureAuthorizedForUser,
      fetchAccount,
      fetchAndUpdateAccount,
      isFeatureAuthorizedForCustomer,
      isFeatureAuthorized,
    };

    return <AccountContext.Provider value={store}>{children}</AccountContext.Provider>;
  }

  return null;
};
```

---
layout: text-window
---

# Old school part 3

- Lots of useState
- Lots of useCallback
- No memoization of components

::window::

```ts {all|105-130} {maxHeight: '450px'}
// take VariationChange (CustomCodeChange or AttributeChange) and returns string
const getVarChangeString = (change: VariationChange) => {
  if (change instanceof CustomCodeChange) {
    return [change.getCss().orElse(''), change.getCode().orElse('')];
  }

  // if not CustomCodeChange, then field is an AttributeChange
  if (change instanceof AttributeChange) {
    const selector = change.getSelector();
    const attributes = Object.values(change.getAttributes()).map((attribute) => {
      if (typeof attribute === 'string') {
        return attribute;
      }
      return JSON.stringify(attribute);
    });
    return [selector, ...attributes];
  }

  return [];
};

// takes all properties we search in a string and concatenate into a single string for easy search
const generateSearchStringArray = (variation: Variation): string[] => {
  const varName = variation.getName();
  const varCode = variation.getCode().orElse('');
  const varCss = variation.getCss().orElse('');
  const redirectUrl = variation.getRedirect().orElse('');
  const varChanges = variation.getChanges().flatMap(getVarChangeString);
  return [varName, varCode, varCss, redirectUrl, ...varChanges];
};

// returns default set of selected status based on state of variations in list
// if list includes variation in "approving" state, show "launch ready" as default status
// if no live or draft variations, then also display paused variations
// if no live, draft or paused variations, then also display archived variations
const getDefaultSelectedStatus = (
  hasApproving: boolean,
  variationsByState: VariationCountByState
): VariationStatusSet => {
  const defaultStatus = new Set([VariationStatusEnum.LIVE, VariationStatusEnum.DRAFT]);
  // show "Launch" as option only if experience include a variation in "approving" status
  if (hasApproving) {
    defaultStatus.add(VariationStatusEnum.APPROVING);
  }

  // get count of variations in different state
  const countLiveVariations = variationsByState.live || 0;
  const countDraftVariations = variationsByState.draft || 0;
  const countPausedVariations = variationsByState.paused || 0;
  // if experience does not have any live or draft variation, then display paused variations
  if (countLiveVariations + countDraftVariations === 0) {
    defaultStatus.add(VariationStatusEnum.PAUSED);
  }
  // if experience does not have any live, draft, or paused variations, then also display archived variations
  if (countLiveVariations + countDraftVariations + countPausedVariations === 0) {
    defaultStatus.add(VariationStatusEnum.ARCHIVED);
  }
  return defaultStatus;
};

// default performance stat data for variations that do not have data in user-journey API
const DEFAULT_PERFORMANCE_STATS: PerformanceComparisonStats = {
  performance: {
    scopeSum: 0,
    valuePerScope: 0,
    valueSum: 0,
    conversionSum: 0,
    conversionsPerScope: 0.0,
  },
};

export interface VariationPerformanceStatsContainerProps {
  experience: Experience;
}

const getIsColumnInView = (
  columnsInView: VariationColumnsInViewSet,
  isGoalSet: boolean,
  scope: VariationScope
): boolean => {
  const conversionColsByScope =
    scope === VariationScope.global ? COLUMNS_GLOBAL_GOAL_CONVERSION_METRIC : COLUMNS_LOCAL_GOAL;
  const valueColsByScope =
    scope === VariationScope.global ? COLUMNS_GLOBAL_GOAL_VALUE_METRIC : COLUMNS_LOCAL_GOAL_VALUE_METRIC;
  return (
    isGoalSet &&
    [...columnsInView].some((columnKey) => conversionColsByScope.has(columnKey) || valueColsByScope.has(columnKey))
  );
};

const getConfidenceValue = (comparisonStats: ComparisonStats) => {
  // Use valueSignificance instead of conversionSignificance for value based campaigns (valueSignificance will only exist if the metricType === 'value')
  let confidenceLocal;
  if ('valueSignificance' in comparisonStats) {
    confidenceLocal = comparisonStats.valueSignificance;
  } else if ('conversionSignificance' in comparisonStats) {
    confidenceLocal = comparisonStats.conversionSignificance;
  }
  return confidenceLocal;
};

const VariationPerformanceStatsContainer: FunctionComponent<VariationPerformanceStatsContainerProps> = ({
  experience,
}) => {
  const [localVariationStatsById, setLocalVariationStatsById] = useState<SplitUserJourneyStats | undefined>();
  const [globalVariationStatsById, setGlobalVariationStatsById] = useState<SplitUserJourneyStats | undefined>();
  const hasLocalStatsData = localVariationStatsById !== undefined;
  const hasGlobalStatsData = globalVariationStatsById !== undefined;
  const [statsError, setStatsError] = useState<Error>();
  const abortableFetchProps = useAbortable();
  const { account } = useContext(AccountContext);
  const globalGoals = account.getMetrics().filter((m) => m.isGoal());
  const isGlobalGoalSet = !!globalGoals && globalGoals.length > 0;
  const localGoals = experience
    .getCampaign()
    .getMetrics()
    .filter((m) => m.isGoal());
  const isLocalGoalSet = !!localGoals && localGoals.length > 0;
  const [searchTerm, setSearchTerm] = useState('');
  const variationScope: VariationScope = isGlobalGoalSet ? VariationScope.global : VariationScope.local;
  const [currentTab, setCurrentTab] = useState<VariationSelectionTabs>(
    variationScope === VariationScope.global ? VariationSelectionTabs.SITE_WIDE : VariationSelectionTabs.ON_PAGE
  );
  const [metricAttrs, setMetricAttrs] = useState<IntervalMetricAttrs>();

  const attrs = useExperienceReportAttrs(experience);
  const { start, end, rangeType } = attrs;
  const apiRange = { start: new Date(start), end: new Date(end) };
  const setAttrs = useSetAttrs<ExperienceReportPageAttrs>();
  const handleSetDateRange = useCallback<IntervalSelectorDropdownProps['setInterval']>(
    (dateRange, metricAttrs, rangeType) => {
      setAttrs({ start: dateRange.start.toISOString(), end: dateRange.end.toISOString(), rangeType });
      setMetricAttrs(metricAttrs);
    },
    [setAttrs]
  );

  const fetchFilterValues = useFetchUserJourneyFilterValues({
    start,
    end,
    accountId: account.getId(),
    experienceId: experience.getId(),
  });
  const handleSetFilterAttrs = useCallback<FilterProviderProps['handleSetFilterAttr']>(
    (filters) => {
      setAttrs({ filters });
    },
    [setAttrs]
  );
  const dimensionListState = useDimensionListState(`/api/v2/customers/${account.getId()}/user-journey/filters`);

  const { metricType: globalMetricType, metricScope: globalMetricScope } = getMetricMeasurement(account.getMetrics());
  const { metricType: localMetricType, metricScope: localMetricScope } = getMetricMeasurement(localGoals);

  // get selected columns from URL/use default values if not in URL
  const { selectedColumns } = useAttrs<VariationTableColumnKeyAttrs>({
    selectedColumns: [...(COLUMNS_BY_SCOPE_AND_TAB[variationScope][currentTab] || [])],
  });
  // generate VariationColumnsInViewSet from array of columns in URL params
  const columnsInView: VariationColumnsInViewSet = useMemo(
    () => new Set([...REQUIRED_COLUMNS, ...selectedColumns]),
    [selectedColumns]
  );

  // setter function to update selected columns in URL
  const updateSelectedColumns = useSetAttrs<VariationTableColumnKeyAttrs>();
  // calls the setter function with correctly formatted object
  const setColumnsInView = useCallback(
    (columnsInView: VariationColumnsInViewSet) => updateSelectedColumns({ selectedColumns: [...columnsInView] }),
    [updateSelectedColumns]
  );

  const updateTab = useCallback(
    (tab: VariationSelectionTabs): void => {
      setColumnsInView(COLUMNS_BY_SCOPE_AND_TAB[variationScope][tab] || new Set(REQUIRED_COLUMNS));
      setCurrentTab(tab);
    },
    [setColumnsInView, variationScope]
  );

  const isGlobalColumnsInView = getIsColumnInView(columnsInView, isGlobalGoalSet, VariationScope.global);
  const isLocalColumnsInView = getIsColumnInView(columnsInView, isLocalGoalSet, VariationScope.local);

  /**
   * geng - TODOs:
   * 1. Column selector (Done)
   * 2. Goal selector
   * 3. Once #1 is in place, conditionally render visible columns and column selector options based on whether
   * customer has global goals.
   * 4. Align on what to display when metrics type === value
   */
  const [variationPerformanceStatsRowPropsById, hasVariationInApprovingState, variationsByState] = useMemo(() => {
    const rowPropsById: VariationColumnPropsById = {};
    const globalStatsById = globalVariationStatsById || {};
    const localStatsById = localVariationStatsById || {};
    let hasVariationInApprovingState = false;
    const numVariationByState: VariationCountByState = {};

    experience.getRealVariations().forEach((variation) => {
      const variationId = variation.getId();
      const variationState = variation.getState();
      const isNoChange = util.isNoChange(variation);

      // track variations by state
      numVariationByState[variationState] = 1 + (numVariationByState[variationState] || 0);
      if (variation.getState() === VariationStatusEnum.APPROVING) {
        hasVariationInApprovingState = true;
      }

      rowPropsById[variationId] = {
        [VariationTableColumnKey.NAME]: variation.getName(),
        [VariationTableColumnKey.STATE]: variationState,
        // concatenated string of everything that we search in a variation
        [VariationTableColumnKey.SEARCH_STRING_ARRAY]: generateSearchStringArray(variation),
      };

      const globalStats = globalStatsById[variationId] || DEFAULT_PERFORMANCE_STATS;

      rowPropsById[variationId][VariationTableColumnKey.SCOPE_SUM] = globalStats.performance.scopeSum;
      rowPropsById[variationId][VariationTableColumnKey.CONVERSION_RATE_GLOBAL] =
        'conversionsPerScope' in globalStats.performance ? globalStats.performance.conversionsPerScope : undefined;
      rowPropsById[variationId][VariationTableColumnKey.VALUE_SUM_GLOBAL] =
        'valueSum' in globalStats.performance ? globalStats.performance.valueSum : 0;
      rowPropsById[variationId][VariationTableColumnKey.CONVERSION_SUM_GLOBAL] =
        'conversionSum' in globalStats.performance ? globalStats.performance.conversionSum : undefined;
      rowPropsById[variationId][VariationTableColumnKey.VALUE_PER_SCOPE_GLOBAL] =
        'valuePerScope' in globalStats.performance ? globalStats.performance.valuePerScope : undefined;
      rowPropsById[variationId][VariationTableColumnKey.VALUE_PER_CONVERSION_GLOBAL] =
        'valueSum' in globalStats.performance &&
        'conversionSum' in globalStats.performance &&
        globalStats.performance.conversionSum !== undefined &&
        globalStats.performance.conversionSum !== 0
          ? globalStats.performance.valueSum / globalStats.performance.conversionSum
          : 0;

      if (globalStats.comparison && !isNoChange) {
        rowPropsById[variationId][VariationTableColumnKey.CONVERSION_COMPARISON_GLOBAL] =
          'conversionPercentage' in globalStats.comparison ? globalStats.comparison.conversionPercentage : undefined;
        rowPropsById[variationId][VariationTableColumnKey.CONVERSION_STRENGTH_GLOBAL] =
          'conversionStrengthDirection' in globalStats.comparison
            ? globalStats.comparison.conversionStrengthDirection
            : undefined;
        rowPropsById[variationId][VariationTableColumnKey.VALUE_COMPARISON_GLOBAL] =
          'valueSignificance' in globalStats.comparison ? globalStats.comparison.valuePercentage : undefined;
        rowPropsById[variationId][VariationTableColumnKey.VALUE_STRENGTH_GLOBAL] =
          'valueStrengthDirection' in globalStats.comparison
            ? globalStats.comparison.valueStrengthDirection
            : undefined;
        rowPropsById[variationId][VariationTableColumnKey.CONFIDENCE_GLOBAL] = getConfidenceValue(
          globalStats.comparison
        );
      }

      const localStats = localStatsById[variationId] || DEFAULT_PERFORMANCE_STATS;

      rowPropsById[variationId].conversionRateLocal =
        'conversionsPerScope' in localStats.performance ? localStats.performance.conversionsPerScope : undefined;
      rowPropsById[variationId].valueSumLocal =
        'valueSum' in localStats.performance ? localStats.performance.valueSum : 0;
      rowPropsById[variationId].conversionSumLocal =
        'conversionSum' in localStats.performance ? localStats.performance.conversionSum : undefined;
      rowPropsById[variationId].valuePerScopeLocal =
        'valuePerScope' in localStats.performance ? localStats.performance.valuePerScope : undefined;
      if (localStats.comparison && !isNoChange) {
        rowPropsById[variationId].conversionComparisonLocal =
          'conversionPercentage' in localStats.comparison ? localStats.comparison.conversionPercentage : undefined;
        rowPropsById[variationId][VariationTableColumnKey.CONVERSION_STRENGTH_LOCAL] =
          'conversionStrengthDirection' in localStats.comparison
            ? localStats.comparison.conversionStrengthDirection
            : undefined;
        rowPropsById[variationId][VariationTableColumnKey.VALUE_COMPARISON_LOCAL] =
          'valueSignificance' in localStats.comparison ? localStats.comparison.valuePercentage : undefined;
        rowPropsById[variationId][VariationTableColumnKey.VALUE_STRENGTH_LOCAL] =
          'valueStrengthDirection' in localStats.comparison ? localStats.comparison.valueStrengthDirection : undefined;
        rowPropsById[variationId][VariationTableColumnKey.VALUE_PER_CONVERSION_LOCAL] =
          'valueSum' in localStats.performance &&
          'conversionSum' in localStats.performance &&
          localStats.performance.conversionSum !== undefined &&
          localStats.performance.conversionSum !== 0
            ? localStats.performance.valueSum / localStats.performance.conversionSum
            : 0;
        rowPropsById[variationId][VariationTableColumnKey.CONFIDENCE_LOCAL] = getConfidenceValue(localStats.comparison);
      }

      // if scope_sum is 0 at this stage, this means that global stats did not have data so was defaulted to 0. in this case, we check local stats
      if (rowPropsById[variationId][VariationTableColumnKey.SCOPE_SUM] === 0) {
        rowPropsById[variationId][VariationTableColumnKey.SCOPE_SUM] = localStats.performance.scopeSum;
      }
    });

    return [rowPropsById, hasVariationInApprovingState, numVariationByState];
  }, [globalVariationStatsById, localVariationStatsById, experience]);

  const [selectedStatus, setSelectedStatus] = useState<VariationStatusSet>(
    getDefaultSelectedStatus(hasVariationInApprovingState, variationsByState)
  );

  const filterMetricScope = hasGlobalStatsData ? globalMetricScope : localMetricScope;

  return (
    <ExpVarStateProvider>
      <PreviewProvider>
        <VariationPerformanceStatsController
          setLocalStats={setLocalVariationStatsById}
          setGlobalStats={setGlobalVariationStatsById}
          setFetchStatsError={setStatsError}
          experience={experience}
          metricAttrs={metricAttrs}
          isGlobalStatsColumnInView={isGlobalColumnsInView}
          isLocalStatsColumnInView={isLocalColumnsInView}
          {...abortableFetchProps}
          {...attrs}
        >
          <VariationPerformanceStatsSettings
            experience={experience}
            campaign={experience.getCampaign()}
            setInterval={handleSetDateRange}
            selectedInterval={apiRange}
            rangeType={rangeType}
            metricScope={filterMetricScope}
            fetchFilterValues={fetchFilterValues}
            handleSetFilterAttr={handleSetFilterAttrs}
            dimensionList={dimensionListState}
          />
          <VariationPerformanceStatsTable
            error={statsError}
            variationColumnPropsById={variationPerformanceStatsRowPropsById}
            includesApprovingStatus={hasVariationInApprovingState}
            columnsInView={columnsInView}
            experience={experience}
            selectedStatus={selectedStatus}
            setSelectedStatus={setSelectedStatus}
            setColumnsInView={setColumnsInView}
            searchTerm={searchTerm}
            setSearchTerm={setSearchTerm}
            currentTab={currentTab}
            setCurrentTab={updateTab}
            variationScope={variationScope}
            hasLocalData={hasLocalStatsData}
            hasGlobalData={hasGlobalStatsData}
            variationCountByState={variationsByState}
            localMetricType={localMetricType}
            globalMetricType={globalMetricType}
          />
        </VariationPerformanceStatsController>
      </PreviewProvider>
    </ExpVarStateProvider>
  );
};

export default VariationPerformanceStatsContainer;
```
<!--
### Mixing paradigms

- React context, react state, redux, and even redux saga were all being used
- Not optimized for renders as react's primitives are just that, primitive
-->
---
layout: text-window
reverse: true
---

# New school

Everything can live side-by-side

More unified state management

Less reliance on direct React usage

::window::

```ts {all|1|375|2-16} {maxHeight: '450px'}
export const CcVariationsTableController = ({ experience, experienceUIModel }: WithExperienceProps): ReactElement => {
  const {
    goals: { selectedGoal },
    globalGoals: { goals: globalGoals },
    localGoals: { goals: localGoals },
    expState: { isExperienceLive },
    reportFilters,
    customerAttributes: { vertical },
  } = useReportSnap();
  const appliedFilters = reportFilters.appliedFilters as FiltersState; // TODO: More generic fix for snapshot types and nested readonly? https://github.com/pmndrs/valtio/issues/327
  const { setColumnsAction, setFilterAction } = useReportActions();
  const { dimensionListState } = useDimensionListSnap();
  const {
    variationDataTable,
    columns: { columnsInView },
  } = useExperienceReportSnap();
  const {
    hasGlobalStatsData: hasGlobalData,
    hasLocalStatsData: hasLocalData,
    rowPropsById,
    hasVariationInApprovingState,
    numVariationByState: variationsByState,
  } = variationDataTable as BuildStatsTableData;
  const [search, setSearch] = useState('');
  const [selectedStatus, setSelectedStatus] = useState<VariationStatusSet>(
    getDefaultSelectedStatus(hasVariationInApprovingState, variationsByState)
  );
  const hasUpdateStatePermission = useUser().hasPermission('update:variation-state');
  const { customer, isSavingCustomer } = useCustomerSnap();
  const { updateVariationStates } = useCustomerActions();
  const [apiError, setApiError] = useState<string>();
  const variations = Object.values(experienceUIModel.variations);
  const availableBatchActions = hasUpdateStatePermission ? getAvailableBatchActions(variations) : [];

  const selectionOptions = {
    disabled: false,
  };

  const { metricScope, metricType: localMetricType } = getMetricMeasurement(localGoals);
  const { metricType: globalMetricType } = getMetricMeasurement(customer.metrics);

  const columns: TableColumn<FormattedVariationStats>[] = [
    {
      key: 'name',
      label: 'Name',
      width: 2,
      render: (item) => <VariationPreviewTableCell label={item.name} urlDetail={item.preview} />,
    },
    {
      key: 'globalConfidenceRate',
      label: 'Confidence Rate',
      shortLabel: 'Confidence',
      group: 'Sitewide Goal',
      width: 1,
      optional: true,
      isLoading: (item) => !item.hasGlobalData,
      scope: VariationScope.global,
      render: (item) => (
        <StatSigCellContent
          confidence={item.globalConfidenceRate}
          confidenceFormatted={item.globalConfidenceRateFormatted}
        />
      ),
    },
    {
      key: 'globalConversionRate',
      label: 'Conversion Rate',
      shortLabel: 'CVR',
      group: 'Sitewide Goal',
      width: 1.25,
      render: (item) => (
        <ConversionRateCell
          conversionRate={item.globalConversionRate}
          confidence={item.globalConfidenceRate}
          comparison={item.globalComparisonRate}
        />
      ),
      optional: true,
      isLoading: (item) => !item.hasGlobalData,
      scope: VariationScope.global,
    },
    {
      key: 'globalConversions',
      label: 'Conversions',
      shortLabel: 'Total',
      group: 'Sitewide Goal',
      width: 1,
      renderKey: 'globalConversionsFormatted',
      optional: true,
      isLoading: (item) => !item.hasGlobalData,
      scope: VariationScope.global,
    },
  ];

  if (globalMetricType === 'value') {
    columns.push(
      {
        key: 'valueSumGlobal',
        label: 'Total Sales',
        group: 'Sitewide Goal',
        width: 1,
        renderKey: 'valueSumGlobalFormatted',
        optional: true,
        isLoading: (item) => !item.hasGlobalData,
        scope: VariationScope.global,
      },
      {
        key: 'valuePerConversionGlobal',
        label: vertical === 'ecommerce' ? 'Average order value' : 'Average conversion value',
        group: 'Sitewide Goal',
        width: 1,
        renderKey: 'valuePerConversionGlobalFormatted',
        optional: true,
        isLoading: (item) => !item.hasGlobalData,
        scope: VariationScope.global,
      },
      {
        key: 'valuePerScopeGlobal',
        label: 'Average session value',
        group: 'Sitewide Goal',
        width: 1,
        renderKey: 'valuePerScopeGlobalFormatted',
        optional: true,
        isLoading: (item) => !item.hasGlobalData,
        scope: VariationScope.global,
      }
    );
  }

  columns.push(
    {
      key: 'localConfidenceRate',
      label: 'Confidence',
      shortLabel: 'Confidence',
      group: 'On-page Goal',
      width: 1,
      optional: true,
      isLoading: (item) => !item.hasLocalData,
      scope: VariationScope.local,
      render: (item) => (
        <StatSigCellContent
          confidence={item.localConfidenceRate}
          confidenceFormatted={item.localConfidenceRateFormatted}
        />
      ),
    },
    {
      key: 'localConversionRate',
      label: 'Conversion Rate',
      shortLabel: 'CVR',
      group: 'On-page Goal',
      width: 1.25,
      optional: true,
      isLoading: (item) => !item.hasLocalData,
      scope: VariationScope.local,
      render: (item) => (
        <ConversionRateCell
          conversionRate={item.localConversionRate}
          confidence={item.localConfidenceRate}
          comparison={item.localComparisonRate}
        />
      ),
    },
    {
      key: 'localConversions',
      label: 'Conversions',
      shortLabel: 'Total',
      group: 'On-page Goal',
      width: 1,
      renderKey: 'localConversionsFormatted',
      optional: true,
      isLoading: (item) => !item.hasLocalData,
      scope: VariationScope.local,
    }
  );

  if (localMetricType === 'value') {
    columns.push(
      {
        key: 'valueSumLocal',
        label: 'Total Value',
        group: 'On-page Goal',
        width: 1,
        renderKey: 'valueSumLocalFormatted',
        optional: true,
        isLoading: (item) => !item.hasLocalData,
        scope: VariationScope.local,
      },
      {
        key: 'valuePerConversionLocal',
        label: 'Average conversion value',
        group: 'On-page Goal',
        width: 1,
        renderKey: 'valuePerConversionLocalFormatted',
        optional: true,
        isLoading: (item) => !item.hasLocalData,
        scope: VariationScope.local,
      },
      {
        key: 'valuePerScopeLocal',
        label: 'Average session value',
        group: 'On-page Goal',
        width: 1,
        renderKey: 'valuePerScopeLocalFormatted',
        optional: true,
        isLoading: (item) => !item.hasLocalData,
        scope: VariationScope.local,
      }
    );
  }

  columns.push(
    {
      key: 'sessions',
      label: 'Sessions',
      width: 1,
      renderKey: 'sessionsFormatted',
    },
    {
      key: 'users',
      label: 'Users',
      width: 1,
      renderKey: 'usersFormatted',
      optional: true,
    },
    {
      key: 'state',
      label: 'Status',
      width: 1,
      render: (item) => (
        <div m="l-4">
          <StatusIndicator state={item.state} variationId={item.id} experience={item.experience} />
        </div>
      ),
    }
  );

  const items = Object.keys(rowPropsById).map((variationId) =>
    formatVariationStats(rowPropsById[variationId], variationId, experience, hasGlobalData, hasLocalData)
  );

  const searchFilteredItems = search === '' ? items : items.filter((item) => isRowMatchingSearchTerm(item, search));

  const filteredItems = searchFilteredItems.filter((item) => selectedStatus.has(item.state as VariationStatusEnum));

  const filteredColumns = columns.filter((column) => {
    if (globalGoals.length === 0 && column.scope === VariationScope.global) {
      return false;
    }
    if (localGoals.length === 0 && column.scope === VariationScope.local) {
      return false;
    }
    return true;
  });

  const [sortItems, sortColumns] = useTableSort(
    filteredItems,
    filteredColumns,
    selectedGoal === 'global' ? 'globalConversionRate' : 'localConversionRate',
    SortOrder.Descending
  );

  const [selectionItems, selectionColumns, resetSelection] = useTableSelection(
    sortItems,
    sortColumns,
    undefined,
    selectionOptions
  );

  const onRunBatchAction = (batchAction: BatchInfo) => {
    setApiError(undefined);
    updateVariationStates({ experience, variationStates: batchAction.body }).then((res) => {
      if ('error' in res) {
        setApiError(res.error.message);
      } else {
        resetSelection();
      }
    });
  };

  const actionItems = selectionItems.map((item) => {
    const availableActions = availableBatchActions.filter((action) => !!action.body[item.id]);
    const actions: TableAction[] = availableActions.map((batchInfo) => ({
      label: ActionTextForSelectedVariation[batchInfo.action],
      buttonVariant: 'primary',
      fn: (selectedKeys) =>
        onRunBatchAction({
          ...batchInfo,
          body: selectedKeys.reduce(
            (currentBody, currentKey) => ({
              ...currentBody,
              ...(batchInfo.body[currentKey] ? { [currentKey]: batchInfo.state } : {}),
            }),
            {}
          ),
        }),
      disabled: isSavingCustomer,
      requireSelection: true,
    }));

    return {
      ...item,
      actions,
    };
  });

  const [finalItems, actionColumns] = useTableActions(actionItems, selectionColumns);

  const [finalColumns] = useTableToggleColumns(actionColumns, [...columnsInView.values()]);

  const filterIcon = appliedFilters.count > 0 ? fasFaFilter : falFaFilter;
  const filterTrigger = (
    <Button variant="secondary" className="ml-4">
      <FontAwesomeIcon icon={filterIcon} className="mr-2" />
      Filters
    </Button>
  );

  return (
    <ExpVarStateProvider>
      <PreviewProvider>
        <VarStateCallout experience={experience} />
        {apiError && (
          <div p="y-8px x-6" text="red">
            {apiError}
          </div>
        )}
        <CcVariationsTableView>
          <TableSearchField value={search} onChange={setSearch} />
          {globalGoals.length > 1 ? (
            <div className="ml-4">
              <GoalsDropdown />
            </div>
          ) : null}
          {isExperienceLive ? (
            <FiltersDropdown
              dimensionList={dimensionListState}
              metricScope={metricScope}
              handleSetFilterAttr={setFilterAction}
              trigger={filterTrigger}
            />
          ) : null}
          <OptionsList
            options={getStatusSelectOptions(hasVariationInApprovingState, variationsByState)}
            selected={selectedStatus}
            setSelected={setSelectedStatus}
            disabledOptions={REQUIRED_STATUS_OPTIONS}
          />
          {/* TODO: Remove overridden type */}
          <ColumnDropdown
            allColumns={sortColumns}
            selectedColumns={finalColumns}
            setColumnsAction={setColumnsAction as (selectedOptions: Set<keyof FormattedVariationStats>) => void}
          />
          <StatusLabel selectedStatus={selectedStatus} setSelectedStatus={setSelectedStatus} />
          <Table className="inCard" items={finalItems} columns={finalColumns} rowComponent={TableStatsRow} />
        </CcVariationsTableView>
      </PreviewProvider>
    </ExpVarStateProvider>
  );
};

interface CcVariationsTableViewProps {
  children: [
    ReactElement,
    ReactElement | null,
    ReactElement | null,
    ReactElement,
    ReactElement,
    ReactElement,
    ReactElement
  ];
}

const CcVariationsTableView = ({
  children: [SearchField, GoalsDropdown, FilterDropdown, StatusToggles, Options, Label, Table],
}: CcVariationsTableViewProps): ReactElement => (
  <div>
    <div p="y-8px x-6" flex="~">
      {SearchField}
      {GoalsDropdown}
      {FilterDropdown}
      <Dropdown
        trigger={
          <Button variant="secondary" className="ml-4">
            <FontAwesomeIcon icon={faCheck} className="mr-2" />
            Status
          </Button>
        }
        addContentPadding
        placement="bottom"
      >
        {StatusToggles}
      </Dropdown>
      <Dropdown
        trigger={
          <Button variant="secondary" className="ml-4">
            <FontAwesomeIcon icon={faLineColumns} className="mr-2" />
            Columns
          </Button>
        }
        addContentPadding
        placement="bottom"
      >
        {Options}
      </Dropdown>
    </div>
    <div p="x-6">{Label}</div>
    {Table}
  </div>
);

const CcVariationsTable = withExperience(withDimensionList(CcVariationsTableController));
export default CcVariationsTable;
```

<!--
### Side-by-side

- Easier and faster to dev without jumping between files

### State management

- Easier and faster to understand where to look for state, how to manipulate it, and how to read it

### Less React

- React's tools like `useEffect` are easy to misuse unintentionally
- Less React makes it harder to screw up React
-->

---
layout: new-section
---

# Meet Ralpio

<img class="w-screen-sm m-x-auto" src="https://i.ytimg.com/vi/fm9H0X3tHfU/maxresdefault.jpg" />

---

# Ralphio is Valtio's cousin

<v-clicks>

- Builds on top of Valtio, so sort of a framework
- Based on lessons learnt from the initial Apollo VE, ABP, RBP effort
- Desire to standardize DX
- Remove as many footguns as possible
- Improve capabilities
- Fix major issues

</v-clicks>

---
layout: text-window
---

# Prior to Ralphio

- Lots of derives based on other states
- Custom solution(s) for caching combined with lots of derives
- Stores looked different depending on who wrote it
- Stores behaved different depending on caching

::window::

```ts {all|2-5|85-113} {maxHeight: '450px'}
const createRbpStore = (stores: Stores, initialExperience: RbpExperience): RbpStore => {
  const authStore = stores.get(StoreName.AUTH);
  const { getAuthToken } = authStore.actions;
  const customerStore = stores.get(StoreName.CUSTOMER);
  const reportStore = stores.get(StoreName.REPORT);
  const localResponseCache: Record<string, SplitUserJourneyStats | undefined> = {};
  const globalResponseCache: Record<string, SplitUserJourneyStats | undefined> = {};
  const userResponseCache: Record<string, SplitUserJourneyStats | undefined> = {};
  const chartResponseCache: Record<string, SplitUserJourneyStats | undefined> = {};

  // @TODO: Temporary workaround to have the table update when variations states change
  const experienceState = derive({
    experience: async (get) => {
      const customer = await get(customerStore.state).customer;
      return customer
        .getExperience(initialExperience.getId())
        .map<RbpExperience>((exp) => (isRbpExperience(exp) ? exp : initialExperience))
        .orElse(initialExperience);
    },
  });

  const variationDataViz = derive({
    chart: async (get) => {
      const [authToken, user, customer, reportUrlAttrs, localGoals] = await Promise.all([
        getAuthToken(),
        get(authStore.state).user,
        get(customerStore.state).customer,
        get(reportStore.state.intervalAndFilters).reportUrlAttrs,
        get(reportStore.state.localGoals).goals,
      ]);
      const experience = await get(experienceState).experience;
      const userId = user.getId();
      const { metricAttrs } = get(reportStore.state).metrics;

      const cacheKey = JSON.stringify(reportUrlAttrs) + (metricAttrs ? JSON.stringify(metricAttrs) : '{}');
      const localEventFilters = localGoals.map((goal) => metricToEventFilter(goal));

      const localPerfStats =
        chartResponseCache[cacheKey] ||
        (await generatePerfStats(
          authToken,
          userId,
          customer,
          experience,
          undefined,
          reportUrlAttrs,
          VariationScope.local,
          localEventFilters,
          metricAttrs,
          undefined,
          VariationSelectionTabs.ON_PAGE
        ));

      chartResponseCache[cacheKey] = localPerfStats;

      return buildChartData(localPerfStats, experience);
    },
  });

  const variationDataTable = derive({
    table: async (get) => {
      const [authToken, user, reportUrlAttrs, globalGoals, localGoals, selectedGoals] = await Promise.all([
        getAuthToken(),
        get(authStore.state).user,
        get(reportStore.state.intervalAndFilters).reportUrlAttrs,
        get(reportStore.state.globalGoals).goals,
        get(reportStore.state.localGoals).goals,
        get(reportStore.state.globalGoals).selected,
      ]);
      const experience = await get(experienceState).experience;
      const customer = experience.getCampaign().getCustomer();
      const userId = user.getId();
      const { metricAttrs } = get(reportStore.state).metrics;

      const selectedGlobalEventFilters = [...selectedGoals].map((goalId) => {
        const [goal] = globalGoals.filter((goal) => goal.getId() === goalId); // will return an array with single item
        return metricToEventFilter(goal);
      });
      const localEventFilters = localGoals.map((goal) => metricToEventFilter(goal));

      const cacheKey =
        JSON.stringify(reportUrlAttrs) +
        (metricAttrs ? JSON.stringify(metricAttrs) : '{}') +
        JSON.stringify(selectedGlobalEventFilters);

      const [localPerfStats, globalPerfStats, userStats] = await Promise.all([
        localResponseCache[cacheKey] ||
          generatePerfStats(
            authToken,
            userId,
            customer,
            experience,
            undefined,
            reportUrlAttrs,
            VariationScope.local,
            localEventFilters,
            metricAttrs,
            undefined,
            VariationSelectionTabs.ON_PAGE
          ),
        globalResponseCache[cacheKey] ||
          generatePerfStats(
            authToken,
            userId,
            customer,
            experience,
            undefined,
            reportUrlAttrs,
            VariationScope.global,
            selectedGlobalEventFilters,
            metricAttrs,
            undefined,
            VariationSelectionTabs.SITE_WIDE
          ),
        userResponseCache[cacheKey] ||
          generatePerfStats(
            authToken,
            userId,
            customer,
            experience,
            [VariationTableColumnKey.USER_SUM],
            reportUrlAttrs,
            VariationScope.global,
            selectedGlobalEventFilters,
            metricAttrs,
            'user'
          ),
      ]);

      localResponseCache[cacheKey] = localPerfStats;
      globalResponseCache[cacheKey] = globalPerfStats;
      userResponseCache[cacheKey] = userStats;

      return {
        localStats: buildTableData(localPerfStats, experience),
        globalStats: buildTableData(globalPerfStats, experience),
        userStats: buildUserColumnData(userStats, experience),
        hasVariationInApprovingState: detectVariationInApprovingState(experience),
        variationsByState: getVariationsByState(experience),
      };
    },
  });

  const columns = derive({
    columnsInView: (get) => {
      const { selectedColumns } = get(reportStore.state).columns;
      const columnsNotNull = selectedColumns || [];

      return columnsNotNull;
    },
  });

  return proxy<RbpStore>({
    variationDataViz,
    variationDataTable,
    columns,
  });
};

export { createRbpStore };
```
---
layout: text-window
reverse: true
---

# Ralpio

State is well defined!

No manual deriving behavior required!

No manual caching required!

::window::

```ts {all|5-41|45-51|115-125} {maxHeight: '450px'}
const createRbpStore = (experienceUIModel: ExperienceUIModel, sc: StoreCreator<RbpState>): RbpStore => {
  const experience = getExperienceFromUIModel(experienceUIModel) as RbpExperience;
  const staticTableData = getVariationReportTableData(experience);

  const state = {
    stats: {
      variationsDetail: staticTableData,
      localPerfStats: undefined,
      globalPerfStats: undefined,
      userStats: undefined,
    },
    variationDataViz: {
      chartData: [{ label: '', usage: 0, sessions: 0, conversions: 0, cvr: 0 }],
      totalPersonalizedPercentage: 0,
      localGoal: '',
      avgCvr: {
        personalizedAvgCvr: 0,
        everyoneElseCvr: 0,
      },
      highlights: {
        mostSessions: null,
        mostConversions: null,
      },
      hasEveryoneElse: false,
      hideChart: false,
    },
    variationDataTable: {
      localStats: {},
      hasLocalStatsData: false,
      globalStats: {},
      hasGlobalStatsData: false,
      userStats: {},
      hasUserStatsData: false,
      hasVariationInApprovingState: false,
      variationsByState: {},
    },
    columns: {
      columnsInView: proxySet([]),
    },
    error: undefined,
  };

  const createdStore = sc({
    state,
    subscriptions: [
      sc.sub(
        sc.fromStores({
          auth: ['user'],
          customer: ['customer.metrics'],
          report: ['intervalAndFilters', 'localGoals', 'metrics.metricAttrs'],
          self: ['columns.columnsInView'],
        }),
        async ({ state, vals, tx }) => {
          const {
            auth: [userState],
            customer: [metrics],
            report: [{ reportUrlAttrs: urlState }, { goals }, metricAttrs],
            self: [columnsInView],
          } = vals;

          const [user, reportUrlAttrs, localGoals] = await Promise.all([userState, urlState, goals]);
          const userId = user.getId();

          const localEventFilters = localGoals.map((goal) => metricToEventFilter(goal));

          state.stats.localPerfStats = undefined;

          const localPerfStats = await generatePerfStats(
            tx,
            userId,
            metrics,
            experience,
            [...columnsInView.values()] as VariationTableColumnKey[],
            reportUrlAttrs,
            VariationScope.local,
            localEventFilters,
            metricAttrs,
            undefined,
            VariationSelectionTabs.ON_PAGE,
            true // force local stats to be fetched as RBP uses it for chart
          );

          state.stats.localPerfStats = localPerfStats;
        }
      ),
      sc.sub(
        sc.fromStores({
          auth: ['user'],
          customer: ['customer.metrics'],
          report: ['intervalAndFilters', 'globalGoals', 'metrics.metricAttrs'],
          self: ['columns.columnsInView'],
        }),
        async ({ state, vals, tx }) => {
          const {
            auth: [userState],
            customer: [metrics],
            report: [{ reportUrlAttrs: urlState }, { goals, selected }, metricAttrs],
            self: [columnsInView],
          } = vals;

          const [user, reportUrlAttrs, globalGoals, selectedGoals] = await Promise.all([
            userState,
            urlState,
            goals,
            selected,
          ]);
          const userId = user.getId();

          const selectedGlobalEventFilters = [...selectedGoals].map((goalId) => {
            const [goal] = globalGoals.filter((goal) => goal.id === goalId);
            return metricToEventFilter(goal);
          });

          state.stats.globalPerfStats = undefined;

          const globalPerfStats = await generatePerfStats(
            tx,
            userId,
            metrics,
            experience,
            [...columnsInView.values()] as VariationTableColumnKey[],
            reportUrlAttrs,
            VariationScope.global,
            selectedGlobalEventFilters,
            metricAttrs
          );

          state.stats.globalPerfStats = globalPerfStats;
        }
      ),
      sc.sub(
        sc.fromStores({
          auth: ['user'],
          customer: ['customer.metrics'],
          report: ['intervalAndFilters', 'globalGoals', 'metrics.metricAttrs'],
        }),
        async ({ state, vals, tx }) => {
          const {
            auth: [userState],
            customer: [metrics],
            report: [{ reportUrlAttrs: urlState }, { goals, selected }, metricAttrs],
          } = vals;

          const [user, reportUrlAttrs, globalGoals, selectedGoals] = await Promise.all([
            userState,
            urlState,
            goals,
            selected,
          ]);
          const userId = user.getId();

          const selectedGlobalEventFilters = [...selectedGoals].map((goalId) => {
            const [goal] = globalGoals.filter((goal) => goal.id === goalId);
            return metricToEventFilter(goal);
          });

          state.stats.userStats = undefined;

          const userStats = await generatePerfStats(
            tx,
            userId,
            metrics,
            experience,
            [VariationTableColumnKey.USER_SUM],
            reportUrlAttrs,
            VariationScope.global,
            selectedGlobalEventFilters,
            metricAttrs,
            'user'
          );

          state.stats.userStats = userStats;
        }
      ),
      sc.sub(
        sc.fromStores({
          self: ['stats.globalPerfStats', 'stats.localPerfStats', 'stats.userStats'],
          variation: ['variations'],
        }),
        ({ state, vals }) => {
          const {
            self: [globalPerfStats, localPerfStats, userStats],
            variation: [variations],
          } = vals;

          state.variationDataTable = {
            localStats: buildTableData(localPerfStats, experience, variations),
            hasLocalStatsData: localPerfStats !== undefined,
            globalStats: buildTableData(globalPerfStats, experience, variations),
            hasGlobalStatsData: globalPerfStats !== undefined,
            userStats: buildUserColumnData(userStats, experience),
            hasUserStatsData: userStats !== undefined,
            hasVariationInApprovingState: detectVariationInApprovingState(experience),
            variationsByState: getVariationsByState(experience),
          };
        }
      ),
      sc.sub(
        sc.fromStores({
          self: ['stats'],
        }),
        ({ state, vals }) => {
          const {
            self: [{ localPerfStats }],
          } = vals;

          if (localPerfStats !== undefined) {
            state.variationDataViz = buildChartData(localPerfStats, experience);
          }
        }
      ),
      sc.sub(
        sc.fromStores({
          customer: ['customer'],
          report: ['columns.selectedColumns', 'goals.selectedGoal', 'localGoals.goals', 'customerAttributes.vertical'],
        }),
        async ({ state, vals }) => {
          const {
            customer: [customer],
            report: [selectedColumns, selectedGoal, localGoals, vertical],
          } = vals;

          const [selectedGoalVal, verticalVal] = await Promise.all([selectedGoal, vertical]);

          const selectedColumnsArray = [...selectedColumns.values()] as (keyof FormattedVariationStats)[];

          const { metricType: localMetricType } = getMetricMeasurement(localGoals);
          const { metricType: globalMetricType } = getMetricMeasurement(customer.metrics);

          const localColumns: Extract<keyof FormattedVariationStats, string>[] =
            localMetricType === 'value' && verticalVal === 'ecommerce'
              ? ['priority', 'localConversionRate', 'valueSumLocal', 'valuePerConversionLocal', 'sessions']
              : ['priority', 'sessions', 'localConversionRate', 'localConversions'];
          const globalColumns: Extract<keyof FormattedVariationStats, string>[] =
            globalMetricType === 'value' && verticalVal === 'ecommerce'
              ? ['priority', 'globalConversionRate', 'valueSumGlobal', 'valuePerConversionGlobal', 'sessions']
              : ['priority', 'sessions', 'globalConversionRate', 'globalConversions'];

          const initialColumns: Extract<keyof FormattedVariationStats, string>[] =
            selectedGoalVal === VariationScope.local ? localColumns : globalColumns;
          const initialPlusSelected: Extract<keyof FormattedVariationStats, string>[] =
            selectedColumnsArray.length > 0 ? selectedColumnsArray : initialColumns;

          if (isEqual([...state.columns.columnsInView.values()], initialPlusSelected)) return;

          state.columns.columnsInView.clear();
          initialPlusSelected.forEach((column) => state.columns.columnsInView.add(column));
        }
      ),
    ],
  });

  return createdStore;
};

export { createRbpStore };
```
---
layout: text-window
reverse: true
---

# Ralpio

No query parameter footguns!

::window::

```ts
sc.sub(sc.fromStores({ queryParams: ['start', 'end', 'rangeType', 'filters'] }), ({ state, vals }) => {
  const {
    queryParams: [start, end, rangeType, filters],
  } = vals;

  state.intervalAndFilters.reportUrlAttrs = getUrlAttrs(experiencePassedIn, { start, end, rangeType, filters });
}),
```

---
layout: text-window
reverse: true
---

# Ralpio

Normalized access to everything you desire!

::window::

```ts {all|1}
saveNewCampaignExperience: async ({ state, tx }, { body, page, updateCustomer }) => {
  const res = await saveNewCampaignExperience({
    tx,
    customer: { id: state.customer.id, schemaVersion: state.customer.schemaVersion },
    page: { id: page.getId(), name: page.getName() },
    experiencesBody: body,
    campaignNames: state.customerClass.getCampaigns().map((_) => _.getName()),
    eventNames: Object.values(state.customer.events).map((_) => _.name),
  });

  if ('item' in res) {
    const campaignId = res.item.getCampaign().getId();
    const experienceId = res.item.getId();
    state.customer.experiences[experienceId] = createExperienceUIModel({
      customerJson: res.customerJson,
      campaignId,
      experienceId,
    });
  }

  return handleCustomerRes(state, res, updateCustomer);
},
```
---
layout: center
---

# Ralphio's core

```ts {all} { maxHeight: '450px' }
// Not exposed from Valtio
type Cleanup = () => void;

export interface DefaultState extends Record<string, unknown> {
  error?: unknown;
  loading?: Record<string, Promise<unknown>> | Promise<unknown>;
}

export type Actions = Record<string, (...args: any[]) => any>;

export interface StoreData<T, A = unknown> {
  stores: Stores;
  state: T;
  tx: Tx;
  actions: A;
}

interface CreateStoreData {
  tx: TxStateWrapper; // A Tx that will closure around the store's state for updating loading/error states
  stores: Stores; // All external stores that should largely be for subscription use transparently and a few edge cases
}

type CreateStoreArgs = CreateStoreData;

export type AreActions<A /* , T extends DefaultState */> = {
  [K in keyof A]: A[K] extends (...args: unknown[]) => unknown
    ? A[K]
    : /* Parameters<A[K]>['length'] extends 0
      ? A[K]
      : Parameters<A[K]>[0] extends Action<T>
      ? A[K]
      : 'Actions are expected to look like (data: StoreData<T>, ...args: unknown[]) => void' */
      'Actions should be functions';
};

export type StoreActions<T extends DefaultState, A> = {
  [K in keyof A]: A[K] extends (...a: infer U) => infer R ? (data: StoreData<T, A>, ...a: U) => R : never;
};

const EmptyObj = {} as const;
// Data used for creating a store
export interface StoreCreation<T extends DefaultState, A extends Actions = never> {
  state: T; // Initial state of the store
  onInit?: (data: StoreData<T>) => void; // If any sort of state needs to be created/computed after initializing
  subscriptions?: (({ stores, state, tx, actions }: StoreData<T, A>) => Cleanup)[]; // Any subscriptions to the internal store state, external state, or both
  actions?: StoreActions<T, A>; // Non-proxied Fns
}

// Obj returned when we create a store
export interface BaseStore<T extends DefaultState> {
  state: T;
  unsub: () => void;
}

export interface StoreWithActions<T extends DefaultState, A extends Actions> extends BaseStore<T> {
  actions: A;
}

export type UnwrapState<S extends Store> = S extends Store<infer State, Actions>
  ? State
  : S extends BaseStore<infer State>
  ? State
  : never;
export type UnwrapActions<S extends Store> = S extends Store<any, infer A> ? A : never;

export type Store<
  T extends DefaultState = Record<string, unknown>,
  A extends Actions = typeof EmptyObj
> = keyof A extends never ? BaseStore<T> : StoreWithActions<T, A>;

// Fn that is used for creating a store with common helper functions for store creation
export type StoreCreator<T extends DefaultState, A extends Actions = never> = {
  (config: StoreCreation<T, A>): Store<T, A>;
  sub: <S extends Subs<T>>(
    subs: S,
    cb: SubCb<T, S>,
    cleanup?: () => void
  ) => ({ state, tx }: { state: T; tx: Tx }) => Cleanup;
  fromStores: typeof fromStores;
};

export const createStore = <T extends DefaultState, A extends Actions>({
  tx: ogTx,
  stores,
}: CreateStoreArgs): StoreCreator<T, A> => {
  const storeCreator = ({ state: initialState, onInit, subscriptions = [], actions }: StoreCreation<T, A>) => {
    const state = proxy(initialState);
    const tx = ogTx(state);

    const baseStoreData = { stores, state, tx };
    const wrappedActions = actions
      ? Object.entries<StoreActions<T, A>[keyof A]>(actions).reduce<any>((acc, [key, val]) => {
          acc[key] = (...args: any[]) => val({ ...baseStoreData, actions: wrappedActions }, ...args);
          return acc;
        }, {})
      : {};
    wrappedActions.clearAllErrors = () => {
      state.error = undefined;
    };

    const storeData = { ...baseStoreData, actions: wrappedActions };
    onInit?.(storeData);
    const unsubscribes = subscriptions.map((sub) => sub(storeData));

    const unsub = () => {
      unsubscribes.forEach((unsubscribe) => unsubscribe());
    };
    const store = {
      state,
      actions: wrappedActions,
      unsub,
    };

    return store;
  };

  storeCreator.sub = sub<T>(stores);
  storeCreator.fromStores = fromStores;

  return storeCreator;
};

export interface SubCbData<T extends DefaultState, X extends Subs<T>> {
  state: T;
  tx: Tx;
  vals: SubVals<T, X>;
}

export type SubCb<T extends DefaultState, X extends Subs<T>> = (subCbData: SubCbData<T, X>) => void;

type Join<K, P> = K extends string | number
  ? P extends string | number
    ? `${K}${'' extends P ? '' : '.'}${P}`
    : never
  : never;

type Prop<T, K extends keyof T, D = false> = K extends string | number
  ? /* customerClass is a proxy so this is kind of bad 
    K extends `${infer C}Class`
    ? never
    : */
    D extends true
    ? `${K}` | Join<K, Paths<T[K], T>>
    : `${K}`
  : never;

type Paths<T, PrevType = never> = T extends object
  ? {
      [K in keyof T]-?: Prop<
        T,
        K,
        T extends PrevType & Record<string, unknown>
          ? false
          : T[K] extends Array<unknown> | Readonly<Array<unknown>> | Promise<unknown>
          ? false
          : true
      >;
    }[keyof T]
  : '';

export type StoreNames = CamelCase<`${StoreName}`>;
type StoresWithState = keyof StoreTypeCamelCaseMap;
type StoresWithoutState = keyof NonStandardStoreTypesCamelCaseMap;
type AllExposedStoreNames = StoresWithState | StoresWithoutState;

type StoreType<K extends AllExposedStoreNames> = K extends StoresWithState
  ? StoreTypeCamelCaseMap[K]['state']
  : K extends StoresWithoutState
  ? NonStandardStoreTypesCamelCaseMap[K]
  : never;

type ExternalSubs = {
  readonly [K in AllExposedStoreNames]?: readonly Paths<StoreType<K>>[];
};

type Subs<T> = ExternalSubs & { self?: Paths<T>[] };

type Gets<BaseType, T> = T extends readonly [infer Head, ...infer Tail] | [infer Head, ...infer Tail]
  ? Head extends string
    ? [Get<BaseType, Head>, ...Gets<BaseType, Tail>]
    : []
  : T extends Array<any> | Readonly<Array<any>>
  ? T
  : never;

type SubVals<Self, X extends Subs<Self>> = {
  [K in AllExposedStoreNames | 'self' as X[K] extends Array<any> | Readonly<Array<any>> ? K : never]: K extends 'self'
    ? Gets<Self, X[K]>
    : K extends AllExposedStoreNames
    ? Gets<StoreType<K>, X[K]>
    : never; // T[K] extends readonly [infer Head, ...infer Tail] ? K extends string ? Head extends string ? [Get<Nested[K], Head>, ...Gets<Tail, Nested[K]>] : K : T[K] : T[K]
};

export const fromStores = <T>(store: F.Narrow<T>): F.Narrow<T> => store;

export const sub =
  <T extends DefaultState>(stores: Stores) =>
  <S extends Subs<T>>(subs: S, cb: SubCb<T, S>, cleanup?: () => void) =>
  ({ state, tx }: { state: T; tx: Tx }): (() => void) => {
    const cleanups: Cleanup[] = [];

    let qpDerived: Record<string, string>;
    if (subs.queryParams) {
      qpDerived = createQpDerive(stores.get('QUERY_PARAMS' as StoreName), subs.queryParams);
      cleanups.push(() => underive(qpDerived));
    }

    const subsEntries = Object.entries(subs as unknown as Record<string, string[]>);
    const txEntries = Object.entries(tx);

    const stop = watch(
      (get) => {
        const retrievedVals = subsEntries.reduce<Record<string, unknown[]>>((acc, [key, vals]: [string, string[]]) => {
          // 'self' is a special key that we use so we can subscribe to our own state changes
          const store = key === 'self' ? { state } : stores.get(snakeCase(key).toUpperCase() as StoreName);

          // queryParams is a special case in that the real store is problematic for consumers
          const storeState = key === 'queryParams' ? qpDerived : (store as { state: unknown }).state;

          // Take all of the props, get their values and assign it as an array under the store name
          acc[key] = vals.reduce<unknown[]>((acc, val) => {
            const propSplit = val.split('.');

            const storeVal = _get(storeState, val);
            // If the value is an object we can just get it directly for any changes on it
            if (typeof storeVal === 'object' && getVersion(storeVal)) {
              acc.push(get(storeVal));
              return acc;
            }

            // The value is a primitive, so we want to watch the parent for optimal tracking
            const subState = propSplit.length > 1 ? _get(storeState, propSplit.slice(0, -1).join('.')) : storeState;
            acc.push(get(subState)[propSplit.at(-1) as string]);
            return acc;
          }, []);

          return acc;
        }, {});

        const abort = new AbortController();

        const abortableTx = txEntries.reduce<Tx>((acc, [key, fn]) => {
          acc[key as keyof Tx] = <T>(url: string, opts?: TxFetchOpts<T>) =>
            fn(url, { fetch: { abortController: abort, ...opts?.fetch }, tx: opts?.tx });
          return acc;
        }, {} as Tx);

        const run = async () => {
          try {
            await cb({ state, tx: abortableTx, vals: retrievedVals });
          } catch (e) {
            // TODO: log?
            if (import.meta.env.DEV) {
              // eslint-disable-next-line no-console
              console.error(`Watch for ${JSON.stringify(subs)} failed`, e);
            }
          }
        };

        run();

        return () => {
          // TODO: Understand what store subscription is causing API requests to be aborted
          // till then, comment out the code
          // abort.abort();
          cleanup?.();
        };
      },
      { sync: false }
    );

    cleanups.push(stop);
    return () => cleanups.forEach((cleanup) => cleanup());
  };

type QPGet = (prox: QueryParamsStore) => Record<string, string>;
// Creates a derived proxy as to prevent query params we aren't paying attention to from causing downstream watch/derive from firing
const createQpDerive = (qpStore: QueryParamsStore, props: readonly string[]) => {
  const qpSubState = props.reduce<Record<string, (get: QPGet) => string>>((acc, prop) => {
    acc[prop] = (get) => get(qpStore)[prop];
    return acc;
  }, {});

  return derive<Record<string, string>, Record<string, string>>(qpSubState);
};
```
---
layout: center
---

# Non-Quiz Quiz

What is a dashboard?

What is an application? 

---

# The Future

<vi-clicks>

- Optimistic updates
- Ability to work toward "realtime multiplayer experience"
- Improved types with Opaque types
- Simpler functions

</vi-clicks>

<!--
### Optimistic updates

- Improved UX

### Multiplayer

- Sumologic already mentioned running into this issue
- Data conflicts aren't the norm

### Improved types

- Our UI Models can be typed as we need them
- Our functions can guarantee the correct id is used

### Simpler functions

- If you work on strings then you don't need an entire class to guarantee the right string
-->
