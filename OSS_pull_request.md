<!--
Thanks for your interest in the project. Bugs filed and PRs submitted are appreciated!

Please make sure that you are familiar with and follow the [Code of Conduct](https://allcontributors.org/docs/en/project/code-of-conduct) for this project.

Also, please make sure you're familiar with and follow the instructions in the
[contributing guidelines](https://github.com/all-contributors/all-contributors/blob/master/CONTRIBUTING.md) (found in the CONTRIBUTING.md file).

If you're new to contributing to open source projects, you might find this free
video course helpful: http://kcd.im/pull-request

Please fill out the information below to expedite the review and (hopefully)
merge of your pull request!
-->
https://github.com/all-contributors/all-contributors/pull/813

**What**: Add support for custom contribution types in the All Contributors specification

This PR adds support for custom contribution types, allowing projects to define their own contribution categories with associated emojis in their `.all-contributorsrc` file.

**Why**: 
- Projects often have unique ways of contributing that don't fit into the standard categories
- Custom contribution types allow projects to better recognize and categorize these unique contributions
- Provides more flexibility while maintaining the structured approach of the All Contributors specification

**How**:
1. Added `customContributions` configuration field in `.all-contributorsrc`:
   ```
   {
     "customContributions": {
       "mentoring": "👨‍🏫",
       "funding": "💵",
       "translation": "🌍"
     }
   }
   ```
2. Updated core specification documentation to include custom types
3. Enhanced bot and CLI documentation with examples and usage instructions
4. Added notes about current CLI limitations

**Checklist**:
- [x] Documentation
  - Updated specification.md
  - Updated bot configuration docs
  - Updated bot usage docs
  - Updated emoji key docs
  - Updated CLI usage docs
- [x] Ready to be merged
- [x] Added myself to contributors table

## Implementation Status

### Core Implementation
- [x] Add `customContributions` field to `.all-contributorsrc` schema
- [x] Update configuration validation to handle custom types
- [x] Add documentation for custom types
- [x] Test basic functionality with CLI
- [ ] Add emoji validation for custom types
- [ ] Update contributor recognition logic to handle custom types

### Documentation
- [x] Update specification.md with custom types
- [x] Add examples for custom types in bot docs
- [x] Document CLI limitations
- [x] Update emoji key documentation
- [x] Add configuration examples

### Testing
- [x] Manual testing of basic functionality
- [x] Tested CLI with single custom type
- [x] Verified README updates
- [ ] Unit tests for custom type handling
- [ ] Integration tests
- [ ] Test coverage for new features

### Technical Implementation Details
- [x] Basic configuration changes
  - Added `customContributions` field
  - Updated documentation
  - Added examples
- [ ] Advanced validation
  - Emoji validation
  - Type name validation
  - Input sanitization
- [ ] Performance considerations
  - Type caching
  - Merge optimization
- [ ] Error handling
  - Invalid type errors
  - User-friendly messages

## Detailed Changes

### Feature Overview
- Support for custom contribution types in the All Contributors bot
- Ability to define custom types with associated emojis in `.all-contributorsrc`
- Full documentation and examples for both bot and CLI usage

### Changes Made
- Added `customContributions` configuration field in `.all-contributorsrc`
- Updated specification to include custom contribution types
- Added documentation for custom types in bot configuration
- Added usage examples in bot documentation
- Updated emoji key documentation
- Documented CLI limitations with multiple custom types

### Testing Done
- Successfully tested adding a contributor with custom type "mentoring"
- Verified correct updates in both `.all-contributorsrc` and README.md
- Tested using the CLI locally
- Documented current CLI limitation with multiple custom types

### Notes
- The CLI currently has a limitation where only one custom contribution type can be added at a time
- Multiple custom contributions need to be added one at a time or using the bot instead 