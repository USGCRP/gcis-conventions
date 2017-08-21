# Universally Unique Identifier

## Definition

A universally unique identifier (UUID) is a 128-bit number used to identify
information in computer systems. The term globally unique identifier (GUID) is
also used.

When generated according to the standard methods, UUIDs are for practical
purposes unique, without depending for their uniqueness on a central
registration authority or coordination between the parties generating them,
unlike most other numbering schemes. While the probability that a UUID will be
duplicated is not zero, it is so close to zero as to be negligible.

Thus, anyone can create a UUID and use it to identify something with near
certainty that the identifier does not duplicate one that has already been, or
will be, created to identify something else. Information labeled with UUIDs by
independent parties can therefore be later combined into a single database, or
transmitted on the same channel, without needing to resolve conflicts between
identifiers.

Adoption of UUIDs and GUIDs is widespread, with many computing platforms
providing support for generating them, and for parsing their textual
representation.

[Read More at Wikipedia](https://en.wikipedia.org/wiki/UUID) (Source:
[Wikipedia](https://en.wikipedia.org),
[CC-BY-SA](https://en.wikipedia.org/wiki/CC-BY-SA)

## GCIS Usage

GCIS UUIDs are generated via the Perl module
[UUID::Tiny](https://metacpan.org/pod/UUID::Tiny) implementation.
