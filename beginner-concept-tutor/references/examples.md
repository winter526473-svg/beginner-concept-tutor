# Canonical response patterns

These examples demonstrate invariants, not wording to copy. Keep the learner-facing sequence stable while changing the mechanics for the concept type.

## Example 1: Agreement — SLA (Level 1)

### Concept identity

- English: Service Level Agreement (SLA)
- Chinese: 服务级别协议
- Domain: IT service management
- Type: service agreement

### One-sentence grasp

SLA is a measurable service promise agreed between a provider and a customer.

### Why it exists

“The system should be stable” means different things to different people. An SLA turns that vague expectation into agreed targets, measurement rules, responsibilities, and remedies.

### Plain-language explanation

Think of it as a service scorecard agreed before delivery. This analogy helps with measurable promises; unlike an ordinary scorecard, an SLA may also define scope, exclusions, responsibilities, and remedies.

### Precise definition

Within IT service management, an SLA records the services and service targets agreed between a service provider and a customer, together with relevant responsibilities and measurement arrangements. Exact wording and required fields vary by framework and contract.

### Core structure or operation

```text
parties → service scope → metric and target → measurement → responsibility/remedy
```

### Complete example

A cloud provider and customer agree to monthly availability of at least 99.95%, a 15-minute response target for priority-one incidents, a stated measurement method, exclusions for scheduled maintenance, and service credit if the availability target is missed.

### Boundaries and confusions

- SLA: customer ↔ service provider.
- OLA: internal team ↔ internal team, supporting service delivery.
- “Keep it reliable” is not yet an SLA because it lacks an agreed measurable target and context.

### Knowledge map

```text
IT service management
└─ service level management
   ├─ SLA
   ├─ OLA
   └─ supporting supplier agreements
```

### Memory hook

SLA = who promises what service level, how it is measured, and what follows.

### 30-second self-test

Why is “the system must be stable” weaker than “monthly availability ≥ 99.95%”?

## Example 2: Process — DNS resolution (Level 1)

### One-sentence grasp

DNS resolution finds the network address associated with a domain name.

### Why it exists

People remember names such as `example.com`; network communication ultimately needs an address. DNS resolution connects those two representations.

### Plain-language explanation

It resembles asking a directory where a named place is located. This helps explain name-to-address lookup, but DNS is distributed, cached, record-based infrastructure—not one global phone book.

### Precise definition

DNS resolution is the process by which a resolver obtains resource records for a domain name, often including an IP address, by using caches and querying the DNS hierarchy as needed.

### Core structure or operation

```text
application → local/stub resolver → recursive resolver/cache
            → root → TLD → authoritative server → answer
```

Not every request visits every server: cached data may answer earlier.

### Complete example

When a browser requests `www.example.com`, the local resolver asks a recursive resolver. If the answer is absent from cache, that resolver follows referrals through the DNS hierarchy, obtains the relevant record from an authoritative server, caches it for its time-to-live, and returns it.

### Boundaries and confusions

DNS resolution identifies records for a name; it does not itself establish the later HTTP connection or guarantee that the destination is reachable.

### Memory hook

DNS resolution turns a name into the records needed for the next network step.

### 30-second self-test

Why might a DNS lookup finish without querying the root server?

## Example 3: Metric — MTTR (Level 2)

Start by disambiguating: MTTR is used for several “mean time to …” metrics, including repair, recovery, restore, and resolution. Never present one expansion as universal without a governing source.

Then explain the selected variant with its event boundaries, population, time window, unit, and formula. For example, if a course defines it as mean time to repair:

```text
MTTR = total active repair time / number of repaired incidents
```

For repair times of 30, 45, and 75 minutes, MTTR is `(30 + 45 + 75) / 3 = 50 minutes`. Interpret this as an average for that defined population and window—not a guarantee that each repair takes 50 minutes. Contrast it with mean time between failures, and ask the learner which timestamps count under the course's definition.

This example demonstrates why source and measurement boundaries come before arithmetic.

## Example 4: Mathematical concept — variance (Level 1)

Give intuition first: variance measures how spread out values are around their mean. Then define the chosen population or sample formula and its notation. Work a small calculation, such as population data `2, 4, 6`: mean `4`, squared deviations `4, 0, 4`, population variance `8/3`. Explain that variance is in squared units and standard deviation returns to the original unit. Contrast low variance with low mean; neither implies the other.

This example demonstrates that a formula explanation needs assumptions, variable meanings, calculation, unit, and interpretation.

## Anti-patterns

- A catchy analogy replaces the formal definition.
- A source-specific meaning is presented as universal.
- The “example” merely repeats the definition with different nouns.
- Every heading receives equal space despite low relevance.
- A knowledge map invents hierarchy or implies disputed relations as settled.
- The self-test asks trivia that was not central to the explanation.
