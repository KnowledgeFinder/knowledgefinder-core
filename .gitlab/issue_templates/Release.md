

## Check list:

* [ ] Create milestone with [release number](https://github.com/KnowledgeFinder/knowledgefinder-core/wiki/Release-Number-Management)
* [ ] Create release branches (with name release-{release_number}) in all project repositories concerned
* [ ] Test release and fix it,  if necessary (redo after fix)
  * [ ] Run unit tests
  * [ ] Run build scripts
  * [ ] Run integration test
* [ ] Finalize release notes
* [ ] Merge release branch into master
* [ ] Tag release in master
* [ ] Merge release branch into development
* [ ] Delete release branch
* [ ] Publish (optional - only necessary for KnowledgeFinder code updates)
  * [ ] code on [github](https://github.com/KnowledgeFinder)
  * [ ] release notes on [webpage](https://knowledgefinder.github.io/)
* [ ] Deploy (optional)
* [ ] Close milestone