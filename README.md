# ARC-Tracker
Contains documentation and public issue tracker for the [ARC Toolkit extension](https://www.paciellogroup.com/toolkit/).
<ul>
  <li><a href="https://www.paciellogroup.com/arc-toolkit-the-service-terms-of-service/">ARC Toolkit Terms of use</a>
  <li><a href="https://www.paciellogroup.com/arc-toolkit-the-service-terms-of-service/">Download ARC Toolkit</a> from the Google Chrome store.
  <li>Download the <a href="https://www.paciellogroup.com/wp-content/uploads/2019/05/ARC-Toolkit-Quickstart-Guide-Accessible_Final.pdf">ARC Toolkit Quickstart Guide (PDF)</a> to get started.

## Reporting issues

If you find an issue with the ARC Toolkit, please [file an issue](https://github.com/ThePacielloGroup/ARC-Tracker/issues) with the following information:
* Concise title that summarises the issue;
* Brief description of the issue;
* ARC Toolkit version;
* Name and version of the OS and browser;
* Expected result
* Actual result
* Test case that demonstrates the issue - provide linked test case codepen/JSbin etc.
<h2>The rules</h2>
The following is the documentation on the assertions that form the ARC rule set in the ARC extension. This documentation is a work in progress, but I hope will provide you with a clear understanding of what the ARC extension currently tests.
<table><caption>ARC rules</caption>
<thead>
<tr>
<th>AAP ID</th>
<th>Assertion</th>
<th>Category</th>
<th>WCAG 2.0 Criteria</th>
</tr>
</thead>
<tbody>
<tr>
<td>269</td>
<td><strong>activeSvgMissingAriaLabel</strong>

active <code>SVG</code> missing aria-label</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>270</td>
<td><strong>altAttributeOnSvgElement</strong>

The <code>SVG</code> image uses the <code>alt</code> attribute to provide a text alternative. This is an invalid method of providing a text alternative for <code>SVG</code> images.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>271</td>
<td><strong>altTextIsallWhitespace</strong>

<code>&lt;img&gt;</code> elements must provide an <code>alt</code> attribute value in order to convey the meaning of the image to screen reader users.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>272</td>
<td><strong>altTextIsallWhitespaceInput</strong>

The <code>input</code> (type=image") has no programmatic label."</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>273</td>
<td><strong>ariaExpandedOnInvalidRole</strong>

The <code>aria-expanded</code> attribute is incorrectly used. The <code>aria-expanded</code> attribute is to be set on the item/element which controls the expansion and collapse of another item. It does not get set on the item which is expanded or collapsed. The state is not accurately conveyed to screen readers.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>274</td>
<td><strong>ARIAHiddenUsedOnFocusable</strong>

An element that receives keyboard focus has <code>aria-hidden="true"</code> set on it. Nothing is announced by screen readers when the element receives keyboard focus. Sceen reader users will not know what the element is."</td>
<td>Error</td>
<td>2.1.1 Keyboard (A)</td>
</tr>
<tr>
<td>275</td>
<td><strong>ariaLabelledbyOnNonInteractiveElement</strong>

<code>aria-labelledby</code> is used on an element which does not reliably convey this attribute</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>276</td>
<td><strong>ariaLabelOnNonInteractiveElement</strong>

<code>aria-label</code> is used on an element which does not reliably convey this attribute</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>277</td>
<td><strong>badAriaAttribute</strong>

An element uses an invalid ARIA attribute. No information about the attribute is available to assistive technology.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>278</td>
<td><strong>badAriaRole</strong>

An element uses an invalid ARIA role. No information about the role (the type of element) is available to assistive technology.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>279</td>
<td><strong>badLongdesc</strong>

The <code>longdesc</code> attribute value contains a space or is empty. The <code>longdesc</code> attribute value must be null or contain spaces.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td></td>
<td><strong>duplicateForAndId</strong>

The <code>id</code> attributes used on the page must be unique. Some screen readers and browsers will be confused by duplicate ids.</td>
<td>Error</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>281</td>
<td><strong>duplicateLabelsUsed</strong>

Form labels are duplicated. This makes it more difficult for all users to understand and complete forms unless the structure provides adequate differentiation and context for labels.</td>
<td>Error</td>
<td>2.4.6 Headings and Labels (AA)</td>
</tr>
<tr>
<td>282</td>
<td><strong>emptyAltInput</strong>

empty <code>alt</code>&lt; /td&gt;</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>283</td>
<td><strong>emptyAltWithTitle</strong>

The image has an empty <code>alt</code> attribute but has a <code>title</code> or <code>aria-label</code> attribute.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>284</td>
<td><strong>emptyAltWtihARIALabel</strong>

The image has an empty <code>alt</code> attribute but has a <code>title</code> or <code>aria-label</code> attribute.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>285</td>
<td><strong>emptyFrameTitle</strong>

<code>title</code> is empty - add text describing the purpose of the frame to the <code>title</code> attribute or use the word 'empty' to indicate no user content</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>286</td>
<td><strong>emptyLabelText</strong>

The labeling method used for the form field is an empty string. Screen readers will not announce the form field label.</td>
<td>Error</td>
<td>2.4.6 Headings and Labels (AA)</td>
</tr>
<tr>
<td>287</td>
<td><strong>emptyLangOnHTML</strong>

language attribute is empty</td>
<td>Error</td>
<td>3.1.1 Language of Page (A)</td>
</tr>
<tr>
<td>288</td>
<td><strong>hotSpotWithEmptyAlt</strong>

The image <code>map</code> and image <code>map</code> hot spots have empty <code>alt</code> attributes. Image maps and hotspots should have an <code>alt</code> attribute set with alternative text that describes the function of the image <code>map</code> (what the image does and/or where the link goes) so screen reader users will understand the image <code>map</code> links.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>289</td>
<td><strong>hotSpotWithNoAlt</strong>

The image <code>map</code> and image <code>map</code> hot spots are missing <code>alt</code> attributes. Image maps and hotspots should have alternative text that describes the function of the image <code>map</code> (what the image does and/or where the link goes) so screen reader users will understand the image <code>map</code> links.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>290</td>
<td><strong>iframeNoTitle</strong>

The <code>iframe</code> is missing the <code>title</code> attribute. The <code>iframe</code> purpose is not communicated clearly to screen reader users.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>291</td>
<td><strong>imgWithAriaDescribedBy</strong>

The image has a null <code>alt</code> attribute or no <code>alt</code> attribute and uses the <code>aria-describedby</code> attribute. The meaning of the image may not be available to some assistive technology.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>292</td>
<td><strong>inputNoAccessibleName</strong>

The form control has no visible label text. Users will not understand the purpose of the control or what type of <code>input</code> is expected.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>293</td>
<td><strong>inputNoAccessibleNameUseAlt</strong>

The button uses an image that has no text alternative. The button name and/or function will not be available to users of assistive technology.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td></td>
<td><strong>InsufficientNormalTextContrast</strong> Insufficient color contrast between foreground text and the background</td>
<td>Error</td>
<td>1.4.3 Contrast (Minimum) (AA)</td>
</tr>
<tr>
<td>294</td>
<td><strong>invalidARIALabelledbyID</strong>

invalid <code>aria-labelledby</code> id</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>295</td>
<td><strong>invalidAttrOnRadioButton</strong>

The <code>aria-invalid</code> attribute is set on a radio button.</td>
<td>Error</td>
<td>3.3.3 Error Suggestion (AA)</td>
</tr>
<tr>
<td>296</td>
<td><strong>invalidTitleChars</strong>

The HTML <code>&lt;title&gt;</code> element contains special characters, such as '~' or '^'. The page <code>title</code> may be confusing to users of assistive technology.</td>
<td>Error</td>
<td>2.4.2 Page <code>title</code> d (A)</td>
</tr>
<tr>
<td>297</td>
<td><strong>labelHiddenWithAriaHidden</strong>

A form control uses a <code>&lt;label&gt;</code> element but the <code>&lt;label&gt;</code> is hidden from assistive technology by using aria-hidden=true". The form control label will not be announced by screen readers."</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>298</td>
<td><strong>labelHiddenWithDisplayNone</strong>

A form control uses a <code>&lt;label&gt;</code> element but the <code>&lt;label&gt;</code> is hidden from assistive technology by using display:none. The form control label will not be announced by screen readers.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>299</td>
<td><strong>labelHiddenWithVisibilityHidden</strong>

A form control uses a <code>&lt;label&gt;</code> element but the <code>&lt;label&gt;</code> is hidden from assistive technology by using visibility:hidden. The form control label will not be announced by screen readers.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>300</td>
<td><strong>labelParentHiddenWithAriaHidden</strong>

A form control uses a <code>&lt;label&gt;</code> element but the <code>&lt;label&gt;</code> is hidden from assistive technology by using aria-hidden=true" on the parent element that contains the <code>&lt;label&gt;</code>. The form control label will not be announced by screen readers."</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>301</td>
<td><strong>labelParentHiddenWithDisplayNone</strong>

A form control uses a <code>&lt;label&gt;</code> element but the <code>&lt;label&gt;</code> is hidden from assistive technology by using display:none that is set on the parent element that contains the <code>&lt;label&gt;</code>. The form control label will not be announced by screen readers.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>302</td>
<td><strong>langNotDefinedOnHTML</strong>

The page does not specify the default language. Screen readers may not read the content with the correct pronunciation.</td>
<td>Error</td>
<td>3.1.1 Language of Page (A)</td>
</tr>
<tr>
<td>303</td>
<td><strong>legendEmpty</strong>

The <code>&lt;legend&gt;</code> element has no text. The programmatic grouping information is not available to assistive technology.</td>
<td>Error</td>
<td>3.3.2 Labels or Instructions (A)</td>
</tr>
<tr>
<td>304</td>
<td><strong>listItemHasNoListParent</strong>

List items (<code>&lt;li&gt;</code>) do not have the required <code>&lt;ul&gt;</code> or <code>&lt;ol&gt;</code> parent element.</td>
<td>Error</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>305</td>
<td><strong>longdescWithEmptyAlt</strong>

An image that uses <code>longdesc</code> has an empty <code>alt</code> attribute.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>306</td>
<td><strong>longdescWithNoAlt</strong>

An image that uses <code>longdesc</code> has no <code>alt</code> attribute and text alternative.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>307</td>
<td><strong>missingLinkAltAttribute</strong>

The link/button purpose cannot be determined from the link text and the page context. Screen reader users may not know the purpose of the link.</td>
<td>Error</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>308</td>
<td><strong>missingTableHeaders</strong>

missing column and row headers</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>309</td>
<td><strong>multipleFormLabelsUsed</strong>

There are multiple <code>&lt;label&gt;</code> elements that reference the same form field. Screen readers may not be able to correctly associate labels and form fields.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>310</td>
<td><strong>multipleLegendElements</strong>

The <code>&lt;fieldset&gt;</code> element contains more than one <code>&lt;legend&gt;</code> element.</td>
<td>Error</td>
<td>3.3.2 Labels or Instructions (A)</td>
</tr>
<tr>
<td>311</td>
<td><strong>multipleMainLandmarks</strong>

The page contains more than one main ARIA landmark or HTML5 <code>&lt;main&gt;</code> element.</td>
<td>Error</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>312</td>
<td><strong>noAlt</strong>

<code>&lt;img&gt;</code> elements must provide an <code>alt</code> attribute in order to convey the meaning of the image to screen reader users</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>313</td>
<td><strong>noAriaLevelOnRoleHeading</strong>

Headings defined with the ARIA role='heading' do not have the aria-level attribute set on them to indicate the heading level. Some screen readers may interpret the heading level incorrectly.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>314</td>
<td><strong>noButtonText</strong>

The button has no programmatic name. The purpose of the button will not be available to users of assistive technology.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>315</td>
<td><strong>noBypassAvailable</strong>

No method is provided to bypass blocks of content.</td>
<td>Error</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>316</td>
<td><strong>noDoctype</strong>

The HTML <code>&lt;doctype&gt;</code> element is missing. Assistive technology relies on the <code>&lt;doctype&gt;</code> element to interpret the page so AT users can perceive and interact with page content.</td>
<td>Error</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>317</td>
<td><strong>noH1</strong>

There is no h1 heading on the page. Each page should have an h1 heading at the start of the main page content. The heading text should describe the main page content and be the same as the page <code>title</code> .</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>318</td>
<td><strong>noHeadingsOnPage</strong>

The headings on the page do not use the relevant h1 to h6 elements to indicate page structure.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>319</td>
<td><strong>noHeadingText</strong>

There are empty headings on the page. Screen reader users may find the page structure confusing, inaccurate, or hard to navigate.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>320</td>
<td><strong>noImageRole</strong>

missing role = 'img' on <code>SVG</code> element</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>321</td>
<td><strong>noLinkText</strong>

The link/button purpose cannot be determined from the link text and the page context. Screen reader users may not know the purpose of the link.</td>
<td>Error</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>322</td>
<td><strong>noModalTitle</strong>

the modal does not have a <code>title</code></td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>323</td>
<td><strong>nonActiveElementInTabOrder</strong>

An element that is focusable with the keyboard but has no role.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>324</td>
<td><strong>nonLayoutTableHasNestedTable</strong>

Tables that are used for layout should not contain HTML table markup such as <code>&lt;th&gt;</code>, summary, and <code>&lt;caption&gt;</code>.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>325</td>
<td><strong>noTitleSVG</strong>

no <code>title</code> for the SVG</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>326</td>
<td><strong>nullValueOnInput</strong>

value attribute is empty - value attribute must either be non-empty or unspecifed for <code>&lt;input&gt;</code> elements with type = 'submit' or 'reset'</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>327</td>
<td><strong>pageHasAutoRefresh</strong>

The page has content that is automatically refreshed or updated. Users with cognitive or reading disabilities, low vision, or motor-control disabilities may be unable to access the content.</td>
<td>Error</td>
<td>2.2.1 Timing Adjustable (A)</td>
</tr>
<tr>
<td>328</td>
<td><strong>pageHasDelayedRedirect</strong>

The page uses a delayed redirect. Some users of assistive technology may not have enough time to interact with elements on the page before the redirect occurs.</td>
<td>Error</td>
<td>2.2.1 Timing Adjustable (A)</td>
</tr>
<tr>
<td>329</td>
<td><strong>pageTitleHasUntitled</strong>

The HTML <code>&lt;title&gt;</code> element contains placeholder text, such as 'untitled' or the file name. Page <code>title</code> s provide AT users with orientation information when the page initially loads.</td>
<td>Error</td>
<td>2.4.2 Page <code>title</code> d (A)</td>
</tr>
<tr>
<td>330</td>
<td><strong>pageTitleIsEmpty</strong>

The HTML <code>&lt;title&gt;</code> element is missing. Page <code>title</code> s provide AT users with orientation information when the page initially loads.</td>
<td>Error</td>
<td>2.4.2 Page <code>title</code> d (A)</td>
</tr>
<tr>
<td>331</td>
<td><strong>placeholderUsedForLabel</strong>

Placeholder text is used to provide the form label in form fields. This information disappears when the form field receives keyboard focus or when <code>input</code> is entered, so it is not communicated to screen reader users.</td>
<td>Error</td>
<td>2.4.6 Headings and Labels (AA)</td>
</tr>
<tr>
<td>332</td>
<td><strong>pseudoContent</strong>

pseudo content found - ensure text alternative is provided when appropriate</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>333</td>
<td><strong>requiredAttrOnRadioButton</strong>

The aria-required attribute or HTML required attribute is used on a radio button.</td>
<td>Error</td>
<td>3.3.2 Labels or Instructions (A)</td>
</tr>
<tr>
<td>334</td>
<td><strong>requiredNotSemanticallyDefined</strong>

the '*' character was detected in the label, indicating a required field, but the field is not semantically defined as being required</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>335</td>
<td><strong>rolePresentationOnTableWithDataElements</strong>

A table defined as a semantically nuetral table contains pertinent semantic table markup.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>336</td>
<td><strong>svgMissingAriaLabelledby</strong>

verify <code>&lt;svg&gt;</code> label</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>337</td>
<td><strong>tabindexGreaterThanZero</strong>

Elements are in the incorrect tab order. This limits the ability of keyboard and screen reader users to access page content in a logical order.</td>
<td>Error</td>
<td>2.4.3 Focus Order (A)</td>
</tr>
<tr>
<td>338</td>
<td><strong>tableCellHaScope</strong>

Table data cells defined as <code>&lt;td&gt;</code> elements use the scope attribute.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>339</td>
<td><strong>tableHeaderMissingScope</strong>

The data table header cells have no scope attributes defined. Some screen readers may not interpret the relationship between the headers and data cells.</td>
<td>Error</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>340</td>
<td><strong>targetLinkDoesNotExist</strong>

The skip link is provided but the target of the href does not exist. This makes page navigation more difficult for screen reader and keyboard users.</td>
<td>Error</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>341</td>
<td><strong>targetNotFocusable</strong>

An in-page or skip link is provided but the target is not focuable. This makes page navigation more difficult for screen reader and keyboard users.</td>
<td>Error</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td></td>
<td><strong>textWithBackgroundImage</strong>
Unable to determine contrast of text on a background image or css generated background</td>
<td>Warning</td>
<td>1.4.3 Contrast (Minimum) (AA)</td>
</tr>
<tr>
<td>342</td>
<td><strong>usingAbstractRole</strong>

An element uses an ARIA composite role.</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>343</td>
<td><strong>visibleLabelWithHiddenInput</strong>

form element with visible label has a hidden <code>input</code></td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>344</td>
<td><strong>visibleModalSiblings</strong>

content behind the modal can be read by screen readers</td>
<td>Error</td>
<td>1.3.2 Meaningful Sequence (A)</td>
</tr>
<tr>
<td>345</td>
<td><strong>zoomingDisabled</strong>

The page text cannot be resized on mobile due to viewport settings. Low-vision users who rely on being able to increase size by at least 200% may not be able to access all content.</td>
<td>Error</td>
<td>1.4.4 Resize text (AA)</td>
</tr>
<tr>
<td>346</td>
<td><strong>1x1ImageAltText</strong>

Images used for visual layout or spacing have alt-text. Images that convey no information should have no text in the <code>alt</code> attribute.</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>347</td>
<td><strong>accessKeyUsed</strong>

accessKeysUsed</td>
<td>Alert</td>
<td>2.1.1 Keyboard (A)</td>
</tr>
<tr>
<td>348</td>
<td><strong>applicationFoundInbody</strong>

The ARIA role=application" is set on the page <code>&lt;body&gt;</code> tag. This may complicate how screen reader users can interact with page content."</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>349</td>
<td><strong>ariaExpandedOnInvalidRole</strong>

The <code>aria-expanded</code> attribute is incorrectly used. The <code>aria-expanded</code> attribute is to be set on the item/element which controls the expansion and collapse of another item. It does not get set on the item which is expanded or collapsed. The state is not accurately conveyed to screen readers.</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>350</td>
<td><strong>ARIAHiddenUsed</strong>

Be sure that it is appropriate to hide this item from screen reader users.</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>351</td>
<td><strong>ARIAHiddenUsedOnFocusable</strong>

An element that receives keyboard focus has aria-hidden=true" set on it. Nothing is announced by screen readers when the element receives keyboard focus. Sceen reader users will not know what the element is."</td>
<td>Alert</td>
<td>2.1.1 Keyboard (A)</td>
</tr>
<tr>
<td>352</td>
<td><strong>ARIAHiddenUsedOnParentOfFocusable</strong>

aria-hidden='true' set on an element that contains focusable children</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>353</td>
<td><strong>ariaLabelOnInputImage</strong>

aria-label or <code>aria-labelledby</code> found on an image button without an <code>alt</code> attribute</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>354</td>
<td><strong>ariaLevelOnHeading</strong>

The aria-level attribute is set on a native HTML heading. This can complicate how some screen reader identify the heading level.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>355</td>
<td><strong>badLongdestTarget</strong>

bad <code>longdesc</code> target</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>356</td>
<td><strong>checkIfLinkTextNeeded</strong>

no link text</td>
<td>Alert</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>357</td>
<td><strong>dlUsed</strong>

Definition list markup is used. Some screen readers will announce this as an unordered list. None of the semantic relationships will be conveyed to screen readers.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>358</td>
<td><strong>duplicateHeaders</strong>

Heading text is duplicated. Screen reader users may find the page structure confusing, inaccurate, or hard to navigate unless the structure provides adequate differentiation between the duplicate headings.</td>
<td>Alert</td>
<td>2.4.6 Headings and Labels (AA)</td>
</tr>
<tr>
<td>359</td>
<td><strong>emptyList</strong>

A list is present that contains no list items (<code>&lt;li&gt;</code>). Screen reader users may find the content structure confusing or difficult to navigate.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>360</td>
<td><strong>emptyListItem</strong>

Empty list items (<code>&lt;li&gt;</code>) are present, which may be announced by screen readers. Screen reader users may find the content structure confusing or difficult to navigate.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>361</td>
<td><strong>framesetHasTitle</strong>

Has <code>title</code> - Remove <code>title</code> from frameset. <code>title</code> attribute should be on frame elements</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>362</td>
<td><strong>h1InHeader</strong>

An h1 heading is present in the page header/banner. This makes it more difficult for screen reader users to quickly locate the main page content.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>363</td>
<td><strong>headingLevelMismatch</strong>

The aria-level value does not match the HTML heading level.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>364</td>
<td><strong>headingLevelSkipped</strong>

Heading levels are skipped or used out of order. Some screen reader users may find the page structure confusing, inaccurate or hard to navigate.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>365</td>
<td><strong>imgWithPresentationRole</strong>

<code>&lt;img&gt;</code> has role of either 'presentation' or 'none'</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>366</td>
<td><strong>inputTypeIsEmail</strong>

A form field uses <code>input</code> type=email". HTML5 form field validation is not fully supported for all assistive technology and browser combinations."</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>367</td>
<td><strong>labelTextVisibleTextMismatch</strong>

The calculated name for the element does not match the visible text presented on the screen.</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>368</td>
<td><strong>legendNotFirstChild</strong>

<code>&lt;legend&gt;</code> is not the first child of the <code>&lt;fieldset&gt;</code></td>
<td>Alert</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>369</td>
<td><strong>lineBreakUsed</strong>

line break used</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>370</td>
<td><strong>linkTextContainsClick</strong>

A link uses text of Click". This type of text is not necessary to include in a link. Screen reader users know that the link must be "clicked" to be activated."</td>
<td>Alert</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>371</td>
<td><strong>linkTextMayNotBeDescriptive</strong>

The purpose of the link may not be known to screen reader users.</td>
<td>Alert</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>372</td>
<td><strong>missingBypassMethods</strong>

missing methods to bypass blocks of content.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>373</td>
<td><strong>missingHREF</strong>

The link anchor has no href attribute</td>
<td>Alert</td>
<td>2.1.1 Keyboard (A)</td>
</tr>
<tr>
<td>374</td>
<td><strong>multipleFooterLandmarks</strong>

There are multiple ARIA contentinfo landmarks or HTML5 footer elements used on the page.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>375</td>
<td><strong>multipleH1</strong>

There are multiple <code>&lt;h1&gt;</code> heading elements on the page. Screen reader users may not be able to navigate easily to the main content of the page.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>376</td>
<td><strong>multipleHeaderLandmarks</strong>

There are multiple ARIA banner landmarks or HTML5 header elements used on the page.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>377</td>
<td><strong>multipleLabellingTechniquesUsed</strong>

Multiple labeling techniques are used for a form control. Assistive technology may not provide correct information about the form control.</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>378</td>
<td><strong>nestedListNotNestedCorrectly</strong>

An incorrectly nested list is present.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>379</td>
<td><strong>nestingFormLabelMissingId</strong>

The checkbox/radio button form fields with visible text labels are associated with the text label by wrapping the label around the form field. Some screen readers may not be able to correctly associate text labels and form fields where nesting is the only way the label is associated with the form field (this is a screen reader/browser bug).</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>380</td>
<td><strong>noLegend</strong>

A <code>&lt;fieldset&gt;</code> is defined that has no <code>&lt;legend&gt;</code>. The grouping information for the form fields will not be available to screen reader users.</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>381</td>
<td><strong>noMainLandmark</strong>

The page does not contain a main ARIA landmark or HTML5 <code>&lt;main&gt;</code> element.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>382</td>
<td><strong>noNavLandmark</strong>

The page navigation is not defined with an ARIA landmark or HTML5 <code>&lt;nav&gt;</code> element. Screen reader users are not able to easily navigate back to the page navigation.</td>
<td>Alert</td>
<td>2.4.1 Bypass Blocks (A)</td>
</tr>
<tr>
<td>383</td>
<td><strong>nonDescriptiveLinkText</strong>

A link uses text of Click Here" or "Here". The purpose of the link may not be known to screen reader users."</td>
<td>Alert</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>384</td>
<td><strong>nonLayoutTableHasNestedTable</strong>

Tables that are used for layout should not contain HTML table markup such as <code>&lt;th&gt;</code>, summary, and <code>&lt;caption&gt;</code>.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>385</td>
<td><strong>nonListItemChildOfList</strong>

An element other than <code>&lt;li&gt;</code> is used as the first child element of a list. Some assistive technology may not imaprt correct list semantics to users.</td>
<td>Alert</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>386</td>
<td><strong>onlyOneListItem</strong>

A list is present that has only one list item. The information conveyed to screen reader users may be misleading or confusing.</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>387</td>
<td><strong>orphanedLabelNoMatchingIDAttribute</strong>

orphaned form label - no matching <code>id</code> attribute</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>388</td>
<td><strong>placeholderDoesNotMatchLabel</strong>

Placeholder text is used in a form that does not match the visual label text. This may cause confusion for screen reader users.</td>
<td>Alert</td>
<td>2.4.6 Headings and Labels (AA)</td>
</tr>
<tr>
<td>389</td>
<td><strong>possibleHTMLInTitle</strong>

The HTML <code>&lt;title&gt;</code> element contains HTML markup. The markup will be read by screen readers when the page loads, which will be confusing for screen reader users and will not adequately describe the purpose of the page.</td>
<td>Alert</td>
<td>2.4.2 Page <code>title</code> d (A)</td>
</tr>
<tr>
<td>390</td>
<td><strong>problematicLinkText</strong>

The image alt-text contains the image type or identifies the image as a graphic element (icon, jpeg, thumbnail, etc.). Images are already identified by assistive technology as graphic elements. Providing this additional information causes redundancy and increases the auditory load of the page for screen reader users.</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>391</td>
<td><strong>requiredIsIndicatedByHTML5Attribute</strong>

A form control other than <code>input</code> type=radio" uses the HTML required attribute."</td>
<td>Alert</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>392</td>
<td><strong>SVGFocusable</strong>

SVG elements are accessible with the keyboard when using Internet Explorer. When used in an active element, the element will have two tabs stops. One for the active element and one for the SVG.</td>
<td>Alert</td>
<td>2.1.1 Keyboard (A)</td>
</tr>
<tr>
<td>393</td>
<td><strong>titleOnLink</strong>

The link text and the <code>title</code> attribute contain the same text. Screen readers may read this text twice.</td>
<td>Alert</td>
<td>2.4.4 Link Purpose (In Context) (A)</td>
</tr>
<tr>
<td>394</td>
<td><strong>unknownTablePurpose</strong>

Table purpose is not known</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>395</td>
<td><strong>verifyDefaultBrowserText</strong>

No default button text specified - Verify the browser supplied text is appropriate</td>
<td>Alert</td>
<td>3.3.2 Labels or Instructions (A)</td>
</tr>
<tr>
<td>396</td>
<td><strong>titleOnNonActiveElement</strong>

An inactive element is present that has a <code>title</code> attribute set on it</td>
<td>Alert</td>
<td>3.3.2 Labels or Instructions (A)</td>
</tr>
<tr>
<td>397</td>
<td><strong>boldUsed</strong>

the text is formatted as bold text - if the bold text conveys meaning, add visually hidden text describing the meaning, or use a more appropriate element such as a heading</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>398</td>
<td><strong>doesNotUsePUA</strong>

character is not in the Private Use Area</td>
<td>Alert</td>
<td>4.1.1 Parsing (A)</td>
</tr>
<tr>
<td>399</td>
<td><strong>invalidARIADescribedbyID</strong>

invalid <code>aria-describedby</code> <code>id</code> - ensure that the <code>id</code> values refer to a valid element</td>
<td>Error</td>
<td>4.1.2 Name, Role, Value (A)</td>
</tr>
<tr>
<td>400</td>
<td><strong>italicUsed</strong>

the text is formatted as italic text - if the italic text conveys meaning, add visually hidden text describing the meaning</td>
<td>Alert</td>
<td>1.3.1 Info and Relationships (A)</td>
</tr>
<tr>
<td>401</td>
<td><strong>nonPUAContentInSameTextElement</strong>

pseudo content found on text element, not in Private Use Area - add the pseudo content to its own span with aria-hidden='true'. Also, add a text alternative when appropriate</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>402</td>
<td><strong>nonPUAContentOnActiveElement</strong>

pseudo content is not hidden - add an <code>aria-label</code> to the clickable item to override the link text, or use a character in the Private Use Area</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>403</td>
<td><strong>nonPUAContentOnNonActiveElement</strong>

pseudo content found, not in Private Use Area - either add aria-hidden to the pseudo content or use content from the Private Use Area. Also, add a text alternative when appropriate</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>404</td>
<td><strong>periodPseudoContent</strong>

pseudo content found on text element, not in Private Use Area - If the '.' character is used for formatting, use ' ' (space) instead. Otherwise, add the pseudo content to its own span with aria-hidden='true'. Also, add a text alternative when appropriate.</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>405</td>
<td><strong>pseudoContentActiveNotHidden</strong>

pseudo content is not hidden - add an <code>aria-label</code> to the clickable item to override the link text, or put the pseudo content on a child span with aria-hidden='true' and use a character in the Private Use Area</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>406</td>
<td><strong>pseudoContentCheckForAlternativeText</strong>

pseudo content found - ensure text alternative is provided when appropriate</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>407</td>
<td><strong>pseudoContentNonActiveNotHidden</strong>

pseudo content is not hidden - put the pseudo content on a child span with aria-hidden='true'</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>408</td>
<td><strong>pseudoContentUsingURL</strong>

an image was inserted with the CSS content property. This will be read as 'image' by some screen readers</td>
<td>Error</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>409</td>
<td><strong>specialCharactersUsed</strong>

a non-alphanumeric character is used - remove the character, make it a background image, or use aria-hidden='true'</td>
<td>Alert</td>
<td>1.1.1 Non-text Content (A)</td>
</tr>
<tr>
<td>410</td>
<td><strong>strikeThroughUsed</strong>

the text is formatted as strikethrough text - if the strikethrough text contains meaning, add visually hidden text describing the meaning</td>
<td>Alert</td>
<td>1.3.3 Sensory Characteristics (A)</td>
</tr>
<tr>
<td>411</td>
<td><strong>underlineUsed</strong>

the text is formatted as underline text - if the underline text conveys meaning, add visually hidden text describing the meaning</td>
<td>Alert</td>
<td>1.3.3 Sensory Characteristics (A)</td>
</tr>
</tbody>
</table>
