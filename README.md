# use replaces

``` js
const plugins = [[
    'import-replaces',
    {
        exclude: 'node_modules',//忽略
        ignore: [
            '@/common/service/modules/index'// 忽略全匹配路径
        ],
        importReplace: [{//替换
            key: '@/common/utils',
            value: 'sss/common/utils'
        }, {
            key: '@/common/service',
            value: 'sss/common/service'
        }
    ]
    }
]]