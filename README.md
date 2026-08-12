Input channel width is the encompassed width, thus
 * OFDM is 22-190 MHz
 * OFDMA is 6.4-95 MHz with 25 kHz spacing, or 10-95 MHz with 50 kHz spacing

The following overhead is accounted for:
 * Cyclic prefix
 * Pilots
 * Complementary pilots
 * PLC
 * NCP message blocks
 * Codewords
   - Assuming no shortened OFDM codewords
   - Follows CableLabs' algorithm for OFDMA codewords
 * MAC header
   - EH: Baseline privacy, upstream + downstream
   - EH: Packet sequencing, downstream
 * Segment header
 * MAP overhead
   - Profile A is assumed to be 256-QAM
   - Overhead for a single channel's data grants (this script's OFDMA)
 * Ethernet header
 * IPv4 header
 * TCP header

Mixed modulation/exclusion zone can be defined.

The MER threshold is displayed (average MER),
based on some common threshold values.
