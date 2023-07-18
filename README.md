## Installation

```
npm install cosmos -g
```

or

```
git clone https://github.com/magicalcosmos/cosmos.git
cd cosmos && npm install
npm link
```

## Usage

Open your terminal and type `cosmos -h` , you'll see the help infomation below:

```
Usage: cosmos <command>

Options:
  -V, --version  output the version number
  -h, --help     output usage information

Commands:
  add            add a new template
  delete         delete a template
  list           List the templateList
  init           init a project
```

## cosmos add

This command would help you to add a new template to the `templates.json`, which will be used by `cosmos` to init projects.

```
$ cosmos add
? 请输入模板名称 admin
? 请输入模板地址 https://github.com/Michael-lzg/vue-ant-template.git

√ Add a template successfully!

The latest templateList is:

┌─────────────────────┬─────────────────────────────────────────────────────────────────────────┐
│ name                │ url                                                                     │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ vue-cli4-vant       │ https://github.com/Michael-lzg/vue-cli4-vant.git                        │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ base-angular-16     │ https://github.com/magicalcosmos/Base-Angular-16.git                    │
└─────────────────────┴─────────────────────────────────────────────────────────────────────────┘
```

## cosmos delete

To delete a template, you could use this command:

```
$ cosmos delete
? 请输入要删除的模板名称 admin
? 请输入要删除的模板名称 admin

√ Deleted successfully!

The latest templateList is:

┌─────────────────────┬─────────────────────────────────────────────────────────────────────────┐
│ name                │ url                                                                     │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ vue-cli4-vant       │ https://github.com/Michael-lzg/vue-cli4-vant.git                        │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ base-angular-16     │ https://github.com/magicalcosmos/Base-Angular-16.git                    │
└─────────────────────┴─────────────────────────────────────────────────────────────────────────┘
```

## cosmos list

This command will shows you the templates list.

```
$ cosmos list
┌─────────────────────┬─────────────────────────────────────────────────────────────────────────┐
│ name                │ url                                                                     │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ vue-cli4-vant       │ https://github.com/Michael-lzg/vue-cli4-vant.git                        │
├─────────────────────┼─────────────────────────────────────────────────────────────────────────┤
│ base-angular-16     │ https://github.com/magicalcosmos/Base-Angular-16.git                    │
└─────────────────────┴─────────────────────────────────────────────────────────────────────────┘
```

## cosmos init 

You can init a templates use this command

```
cosmos init vue-cli4-vant project
```
