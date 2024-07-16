module.exports = {
    root: true,
    extends: [
      'eslint:recommended',
      'plugin:react/recommended',
      'plugin:@typescript-eslint/recommended',
      // 'plugin:@typescript-eslint/eslint-recommended',
      'plugin:prettier/recommended',
      'prettier',
      // 'prettier/@typescript-eslint',
      'plugin:@next/next/recommended'
    ],
    plugins: [
      '@typescript-eslint',
      'react'
      // 'simple-import-sort'
    ],
    parser: '@typescript-eslint/parser',
    parserOptions: {
      sourceType: 'module',
      ecmaFeatures: {
        jsx: true
      }
    },
    env: {
      browser: true,
      node: true,
      es6: true
    },
    settings: {
      react: {
        version: 'detect'
      }
    },
  
    rules: {
      eqeqeq: 'error',
      // 'simple-import-sort/imports': 'error',
      'react/react-in-jsx-scope': 'off',
      '@typescript-eslint/explicit-module-boundary-types': 'off',
      '@next/next/link-passhref': 'off',
      'react/display-name': 'off',
      // '@typescript-eslint/no-unused-vars': [
      //   'error',
      //   { varsIgnorePattern: '^_', argsIgnorePattern: '^_' }
      // ]
      'react/no-unknown-property': 'off',
      '@typescript-eslint/no-unused-vars': 'off',
      '@typescript-eslint/no-explicit-any': 'warn',
      'prettier/prettier': 'warn',
      'react/no-deprecated': 'warn',
      '@typescript-eslint/no-empty-function': 'off',
      'no-unused-vars': 'off',
  
      'no-restricted-syntax': [
        'error',
        'TSEnumDeclaration',
        'TSInterfaceDeclaration',
        'ForInStatement',
        'LabeledStatement',
        'WithStatement',
        "VariableDeclaration[kind='let']"
      ]
    },
  
    overrides: [
      {
        files: ['*.js'],
        rules: {
          '@typescript-eslint/no-var-requires': ['off']
          // 'react/display-name': ['off'],
          // 'react/display-name': false
        }
      }
    ]
  }
  