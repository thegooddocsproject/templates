# Requirement writing guide

## Requirement structure

The core structure of most requirements follows the format of:

{Condition}                      | the {subject}    | {compliance} | {verb} {object} | {qualification}
-------------------------------- | ---------------- | ------------ | --------------- | ------------------
After one year of level-2 usage, | the battery-life | MUST         | last 10 hours   | when running {application}.

The elements include:

*   {condition}: Optional criteria explaining when this requirement is
    applicable.
*   {subject}: The entity being defined.
*   {compliance}: One of:
    *   MUST: The requirement must be implemented.
    *   SHOULD: Our organization recommends implementation of the requirement.
    *   MAY: The requirement’s feature may be included or omitted, depending on
        the implementer’s choice.
*   {verb}: The action to be performed by the {subject}.
*   {object}: The entity being acted upon by the subject.
*   {qualification}: Optional qualification for the requirement.

### Use active voice

Use active voice (rather than passive voice) when writing requirements.

**Recommended:**

In active voice, the subject of the sentence is performing the action:

> *   [ ] The {actor} MUST {action} the {target}.
> *   [ ] The display MUST show the time.

**Not recommended:**

In passive voice, the subject of the sentence is being acted upon.

> *   [ ] The {target} MUST be {actioned} by the {actor}.
> *   [ ] The time MUST be shown by the display.

While these two statements are logically the same, with passive voice we can
easily forget to include the {actor} (which introduces ambiguity).

> *   [ ] The {target} MUST be {actioned}.
> *   [ ] The time MUST be shown.

## Singular

Have each requirement state a single capability, characteristic, constraint or
quality factor.

Ensure the requirement stands alone, so that it can be referenced directly from
tests or other requirements. This is a foundational criteria for traceability.
It helps answer questions such as:

> For my device, has every feature been implemented, tested, and verified?

### Avoid combining requirements

Be wary of using conjunction words, such as “and” in requirements. It usually
means you have two requirements in one line.

**Recommended:**

> *   [ ] The control panel MUST display the device location.
> *   [ ] The control panel MUST display the date.

**Not recommended:**

> *   [ ] The control panel MUST display the device location **and** date.

Note: This approach often results in a repetitive list of requirements. That’s
okay. It is more important to have traceable requirements than nice-to-read
text.

Other conjunctions to be wary of include: *and, or, and/or, unless, but,
however, whether, meanwhile, whereas, otherwise*.

Related phrases include: *as well as, on the other hand*.

## Complete

Ensure the requirement sufficiently describes the required capability,
characteristic, constraint or quality factor to meet the entity need, without
needing other information to understand the requirement.

Note: Requirements are regularly presented in a traceability matrix format, such
as `Test A verifies Requirement B`. In this case, the requirement is read on its
own, without seeing prior or subsequent requirements.

### Avoid vague pronouns

Avoid vague pronouns such as *it, this, that* and cross-referencing words such
as *below, above, aforementioned, aforesaid, following, herein, hereafter,
preceding*.

Watch out for run-on requirements, where you need to have read the preceding
requirement to understand this requirement.

**Recommended:**

> *   [ ] The control panel MUST display the device location.
> *   [ ] The control panel MUST display the date.

**Not recommended:**

> *   [ ] The control panel MUST display the device location.
> *   [ ] **It** MUST also display the date.

The resulting language doesn’t flow as well as normal English, but it means that
each requirement can stand on its own.

### Properly reference documents

When referencing external documents, ensure the document and relevant section,
or sections, are uniquely identified.

Requirements often reference an external document, such stating that a component
must comply with a specific standard.

When referring to the document, ensure that you include sufficient information
to easily identify the correct version of the document, such as:

*   The document title.
*   Version number.
*   Release date.
*   URL to source.
*   Relevant section, or sections within the document.

### Describe the extent of compliance with a specification

Be clear about the extent of compliance required from a specification.

To support interoperability between systems, a requirement often states that a
component must comply with a specific standard. The standard typically
represents multiple external requirements (and associated tests).

Often, only a subset of the standard’s requirements are applicable to the
component. This should be stated to avoid testing parts of the standard
unsupported by the component, or to avoid over-testing. This can sometimes be
achieved with a cover-all statement. At other times you need to itemize each
supported specification sub-requirement.

**Recommended:**

> *   [ ] The mapping system MUST publish map features in compliance with the
>     subset of requirements from the
>     [Web Feature Service specification](https://www.ogc.org/standards/wfs),
>     version 2.0.2, which are relevant to read-only requests.
>     *   *Rationale: The mapping system doesn’t support user updates, so it
>         doesn’t need the subset of write requirements from the Web Feature
>         Service specification.*

Tip: Consider how compliance will be tested. Often there is a test suite
associated with the specification which you can reference.

## Unambiguous

### Avoid ambiguous terms

Avoid vague and general terms in requirements. They result in requirements that
are often difficult or even impossible to verify or may allow for multiple
interpretations. The following are types of unbounded or ambiguous terms:

*   Superlatives such as:
    *   *best, most*.
*   Subjective language such as:
    *   *user-friendly, easy to use, cost-effective.*
*   Ambiguous adverbs and adjectives such as:
    *   *almost always, significant, minimal*.
*   Open-ended statements, such as:
    *   *provide support, but not limited to, as a minimum.*
*   Loopholes such as:
    *   *if possible, as appropriate, as applicable*.

### Be clear about the number of options which must be true

If listing multiple options, ensure it is clear whether:

*   All options must be true.
*   One and only one option must be true.
*   One or more options must be true.

**Recommended:**

> *   [ ] The map server MUST be able to publish selected features via one or
>     more of the following formats:
>     *   [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946).
>     *   [Geographic Markup Language (GML)](https://www.ogc.org/standards/gml)
>         version 3.3.
>     *   [KML](https://www.ogc.org/standards/kml) versions 2.2.
>     *   [KML](https://www.ogc.org/standards/kml) versions 2.3.

**Recommended:**

> *   [ ] The map server MUST be able to publish selected features via both
>     [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946) and
>     [Geographic Markup Language (GML)](https://www.ogc.org/standards/gml)
>     version 3.3 formats.

**Not recommended:**

> *   [ ] The map server MUST be able to publish selected features via
>     [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946),
>     [Geographic Markup Language (GML)](https://www.ogc.org/standards/gml)
>     version 3.3, or [KML](https://www.ogc.org/standards/kml) versions 2.2 or
>     2.3.

### Use timeless language

Avoid language that anchors a document to a point in time, such as:

*   *latest, previous, currently, in future, new, old, now, presently, soon*.

Requirements should be written to describe a specific version of a product and
hence shouldn’t refer to future or past conditions.

**Recommended:**

> *   Note - Device releases up to version 5.0 support bluetooth.
> *   Note - For devices released from 6.0 onwards, bluetooth support is
>     deprecated.

**Not recommended:**

> *   Note - The device’s **current** support for bluetooth is being deprecated.

## Verifiable

Ensure the requirement is structured and worded such that its realization can be
proven (verified) to the customer’s satisfaction at the level the requirement
exists. Verifiability is enhanced when the requirement is measurable.

When writing a requirement, ask:

*   How can this requirement be tested and verified?
*   Is such testing and verification realistically achievable with the project’s
    resources?

If you can’t answer that question, then you probably need to change the
requirement.

### Be wary of terms that imply totality

Be wary of terms that imply totality such as:

*   *all, always, never, every*.

Where appropriate, provide explicit tolerances and measurable boundary
conditions.

**Recommended:**

> *   [ ] When power is connected, the battery MUST charge from 3% to 98%
>     capacity within 4 hours.

**Not recommended:**

> *   [ ] When power is connected, the battery MUST fully charge within 4 hours.

### Be careful with the use of “not”

Try to avoid using “not” in requirement statements.

The presence of “not” usually implies “not ever” which cannot be verified in a
finite time.

**Recommended:**

> *   [ ] The system’s availability MUST be greater than or equal to 99.9%.

**Not recommended:**

> *   [ ] The system MUST NOT fail.

## Move extra information out of requirements

It is often valuable to capture supporting information for the requirement.
However, it shouldn’t be included in the requirement statement. Instead it
should be captured in the requirement’s metadata, or in supporting text placed
around the requirement statements.

**Recommended:**

> heading: “Environmental factors”
>
> requirement: “The device must be waterproof to a depth of 10 meters.”
>
> *   rationale: “The device is to be used by people when swimming on the
>     water’s surface.”
> *   text: “Note: Waterproof requirements were introduced in version 2.0 of the
>     device.”

**Not recommended:**

> requirement: “The device must be waterproof to a depth of 10 meters so that
> the device can be used when swimming on the surface. Waterproof requirements
> were introduced in 2022.”
