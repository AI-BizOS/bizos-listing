# Evidence paths

Read this file when competitor, keyword, review, sales, or traffic evidence affects the Listing decision.

## Source order

Own-product facts are independent of competitor research. Keep a separate record of user-provided facts and any verified own Listing/project data. A competitor claim never becomes an own-product claim.

For external evidence, first inspect the tools **actually available in this session**. If an authorized BizOS MCP tool supports the requested marketplace and competitor/keyword task, use it and inspect the returned status and scope. Do not hard-code an internal endpoint, request credentials, or assume a configured MCP service was successfully queried.

For missing fields or users without BizOS MCP, use available user files, target ASINs, and permitted public browsing. Check the original product page when possible; search result summaries alone support only leads. If no browsing is available, work from supplied material and identify the coverage gap.

## Record each material source

| Field | Meaning |
| --- | --- |
| `mode` | `bizos_mcp`, `user_material`, `public_research`, or `limited` |
| `locator` | Tool result ID, file name/row, ASIN, or URL sufficient to find the evidence again |
| `marketplace` | Site or region that the observation describes |
| `observed_at` | Tool collection time, page access time, or date on supplied material |
| `coverage` | Product count, review count, period, or known limits where available |
| `supports` | The specific claim or comparison that this source supports |
| `status` | Direct observation, source-reported estimate, inference, or unknown |

If a tool exposes only a preview, stale snapshot, or partial sample, say so. Do not fill a missing metric with a guess or relabel a third-party estimate as BizOS first-party observation. Do not state that all competitors were covered when only a few pages were inspected.

## Comparing paths

BizOS MCP may provide richer structured metrics; public pages usually provide visible copy, price, images, rating, and sometimes review samples. This is an expected difference in coverage, not a failure of the portable path. Use the same decision process in both modes, but reduce confidence and omit unsupported metrics when evidence is weaker.
