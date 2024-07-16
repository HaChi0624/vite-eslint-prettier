{
    "extends": [
      "next/core-web-vitals",
      "plugin:@typescript-eslint/recommended",
      "eslint:recommended",
      "plugin:react/recommended",
      "plugin:react-hooks/recommended",
      "plugin:storybook/recommended",
      "plugin:import/recommended",
      "plugin:import/typescript",
      "plugin:jsdoc/recommended",
      "prettier",
      "google"
    ],
    "parserOptions": {
      "project": "./tsconfig.json"
    },
    "plugins": ["@emotion"],
    "env": {
      "jest": true
    },
    "rules": {
      // TODO : 開発を進めることで、必要なRuleを決めること。
      "space-before-function-paren": "off",
      "jsdoc/require-returns": "off",
      "jsdoc/check-tag-names": "off",
      "jsdoc/no-undefined-types": "off",
      "jsdoc/check-param-names": "off",
      "jsdoc/require-param-type": "off",
      "jsdoc/valid-types": "off",
      "jsdoc/require-param-description": "off",
      "@typescript-eslint/no-explicit-any": "off",
      // "react/prop-types": "off",
      // "react/react-in-jsx-scope": "off",
      "linebreak-style": 0, // LF, CRLFを全部許容する。
      "require-returns-description": "off",
      "valid-jsdoc": "off",
      "operator-linebreak": "off",
      "no-irregular-whitespace": "off",
      "no-debugger": "warn",
      "indent": 0,
      "max-len": [1, { "code": 120 }],
      "object-curly-spacing": [2, "always"],
      "@typescript-eslint/no-unused-vars": [1, { "args": "after-used", "argsIgnorePattern": "^_" }],
      "no-unused-vars": "off",
      "quote-props": "off",
      "new-cap": "off",
      "comma-dangle": "off"
    },
    "globals": {
      "React": true,
      "JSX": true,
      "jsx": true,
      "google": true,
      "mount": true,
      "mountWithRouter": true,
      "shallow": true,
      "shallowWithRouter": true,
      "context": true,
      "expect": true,
      "jsdom": true,
      "Jest": true
    }
  }