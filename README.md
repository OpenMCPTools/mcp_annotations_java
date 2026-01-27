# MCP Java Annotations

Currently, in the MCP [python sdk](https://github.com/modelcontextprotocol/python-sdk), and the [typescript](https://github.com/modelcontextprotocol/typescript-sdk) sdk, decorators are defined in the sdk to allow mcp server and client developers to use
any tools, as the decorators themselves are available in the freely available and open source sdks and defined by the [MCP protocol schema](https://github.com/modelcontextprotocol/modelcontextprotocol/tree/main/schema).

Currently (1/2026), the [Java MCP SDK](https://github.com/modelcontextprotocol/java-sdk) does not have annotation classes defined in the SDK itself.  Rather, several server-side frameworks have defined annotation classes appropriate for each framework.  For example, the Spring AI project has [mcp-annotations](https://github.com/scottslewis/mcp-annotations).  These annotation classes are in the [org.springaicommunity.mcp.annotation package](https://github.com/scottslewis/mcp-annotations/tree/main/mcp-annotations/src/main/java/org/springaicommunity/mcp/annotation).  There is an issue to include these [annotations in the current MCP SDK](https://github.com/spring-ai-community/mcp-annotations/issues/10) but unclear whether this will be done or include community-desired annotations (e.g. [meta-support](https://github.com/modelcontextprotocol/java-sdk/issues/344)).

Duplicating annotation classes for each framework is a waste of technical effort, and very inconvenient for mcp server and client developers, as they are forced to choose an MCP server implementation framework (e.g. Spring AI community) in order to define the meta-data for their MCP Primitives:  [Tools, Resources, and Prompts](https://modelcontextprotocol.io/specification/2025-11-25/server). It would be better for the entire MCP dev community if these annotation classes were part of an open, community-driven, framework-independent project and team.

The goal of this repo is to serve as a dev-community-managed, public, multi-framework, 'standardized' set of MCP schema/spec-compliant annotation classes. Further, the goal is to have participation/contribution/review from as many tools builders, framework builders, and dev community contributors.  This so that everyone can build on an open, spec-compliant, framework-agnostic, interoperabile, and well-maintained minimal package of classes.  

Interested developers are encouraged to join the project and/or contribute code, docs, public discussion and reviews, build infrastructure, or other ways.

The license will be open source, and dictated by the conventions selected by the MCP project/org.
