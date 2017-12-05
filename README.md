# changelog-test
just changelog test

## install this tool locally
```
npm install -g conventional-changelog
```

## copy it to package.json
```
"postversion": "conventional-changelog  -i CHANGELOG.md -s -r 0 && git add . && git commit -m \"change log\" && git tag -af $(git describe --abbrev=0 --tags) -m \"$(git describe --abbrev=0 --tags)\" && git push && git push --tags"
```

## You are ready to use npm version
```
npm version patch // minor, major
```