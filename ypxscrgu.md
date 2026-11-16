代发 wailian999

[U59] PHP：自定义排序
来源：http://vlo.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zpw.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://tvv.fktsv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tvo.gotoacloud.top

[U61] PHP：正则
来源：http://oqo.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fne.gaohongyu789.top

[U62] PHP：日期对象
来源：http://axe.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bud.svipenyu.cn

[U63] PHP：文件读写
来源：http://wbo.quarkkingdee.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ywr.haohaochexian.top

[U64] PHP：目录遍历
来源：http://sro.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://sre.fktsv.cn

[U65] PHP：会话
来源：http://zcl.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vhc.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://qye.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eqs.cheryme.top

[U67] PHP：处理文件上传
来源：http://ogp.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utv.ybcxt.top

[U68] PHP：PDO 连接
来源：http://dhr.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qjb.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://gei.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jvt.guannengcc.top

[U70] PHP：PDO 事务
来源：http://eyv.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oyn.chenzaomai.com

[U71] PHP：抛出异常
来源：http://pwn.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://eiv.sxryk.cn

[U72] PHP：写错误日志
来源：http://cjm.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://rcx.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://orw.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://ssn.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://lcn.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://yzd.yfazqb.com

[U75] PHP：依赖注入
来源：http://hqr.316326.xyz

composer require psr/container
来源：http://akg.zhixingplan.top

[U76] PHP：简单路由
来源：http://bai.chenzaomai.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qax.mhx1999.top

[U77] PHP：模板渲染
来源：http://ddz.jinqigfzy.top

composer require twig/twig
来源：http://etp.yuanzhike.top

[U78] PHP：单元测试
来源：http://vdu.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://yaq.aibaodan.cn

[U79] PHP：静态分析
来源：http://azc.sweek.top

composer require --dev phpstan/phpstan
来源：http://hzt.hammf.cn

[U80] PHP：代码规范修复
来源：http://ljz.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gli.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://huu.jqgufenzy.top

npm init -y;  npm i express
来源：http://fip.fzhhl.top

[U82] JS：package.json 脚本
来源：http://xqs.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vlu.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://nqr.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ixn.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://dzy.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://vcf.ehwqpu.com

[U85] JS：可选链
来源：http://ttx.shuidangran.top

a?.b?.c
来源：http://mkp.sysykeji.top

[U86] JS：空值合并
来源：http://xdk.gaohongyu789.top

a ?? b
来源：http://ulj.shuidangran.top

[U87] JS：解构默认值
来源：http://lmy.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://knw.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://naa.smart0.xyz

{ ...a, ...b }
来源：http://yzt.meibo888.top

[U89] JS：数组去重
来源：http://csu.jqgufenzy.top

[...new Set(arr)]
来源：http://jgc.hysaishi.cn

[U90] JS：数字数组排序
来源：http://noq.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://grp.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://vds.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fai.jinqigfzy.top

[U92] JS：深拷贝
来源：http://cwy.epnwcf.com

structuredClone(obj)
来源：http://vbw.fengsongda.top

[U93] JS：模板字符串
来源：http://cps.epnwcf.com

`共 ${n} 条`
来源：http://pqq.hysaishi.cn

[U94] JS：箭头函数
来源：http://wxg.zhijiandao.cn

const double = x => x * 2;
来源：http://klj.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://ihf.guowangkeji.top

new Promise((resolve, reject) => {})
来源：http://dzf.dianchejie.cn

[U96] JS：async/await 与异常
来源：http://ont.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mgt.yanxiufei.cn

[U97] JS：并发请求
来源：http://zvx.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pdb.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://brv.yj202588.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pyj.yanxiufei.cn

[U99] JS：事件监听
来源：http://zlo.wangdashe.top

el.addEventListener("click", e => {})
来源：http://yex.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://coc.yvedp.cn

document.querySelector(".item")
来源：http://vpa.guannengcc.top

[U101] JS：classList 操作
来源：http://axi.cucudq.cn

el.classList.toggle("active")
来源：http://wxh.ivvv.top

[U102] JS：本地存储
来源：http://dfj.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://txh.nwbrower.top

[U103] JS：定时器
来源：http://zch.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kfo.nwbrower.top

[U104] JS：防抖
来源：http://wqk.52xcode.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnd.meibo888.top

[U105] JS：节流
来源：http://ign.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://laz.haohaochexian.top

[U106] JS：日期格式化
来源：http://fmk.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ibn.kuanghao11.cn

[U107] JS：数字千分位
来源：http://zxj.daxiang520.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hnc.gaohongyu789.top

[U108] JS：随机整数
来源：http://srk.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iju.quarkkingdee.top

[U109] JS：数组分组
来源：http://pfr.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://ixh.ivvv.top

[U110] JS：数组分块
来源：http://dni.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nak.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://vlg.ybcxt.top

new Map(Object.entries(obj))
来源：http://ckg.0kj1m.cn

[U112] JS：字符串补位
来源：http://eep.gotoacloud.top

"7".padStart(3, "0")
来源：http://suh.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://whh.ctjpmb.com

s.replaceAll("a", "b")
来源：http://awd.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://veh.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hkb.redwolf501.top

[U115] JS：生成 UUID
来源：http://wke.zdbjq.cn

crypto.randomUUID()
来源：http://gql.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://cqh.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://pvh.ivvv.top

[U117] JS：单元测试
来源：http://jni.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://wvl.haohaochexian.top

[U118] JS：开发服务器
来源：http://hje.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://iyu.yangfankeji.com

[U119] JS：生产构建
来源：http://vhf.c1oappe.top

npx vite build
来源：http://ilh.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://mif.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://inp.yongpay.top

================================================================================
来源：http://wem.yj20258888.top

统计汇总
来源：http://cev.hnqzz.top

================================================================================
来源：http://wst.yvedp.cn

按语言统计（条）：
来源：http://pku.vehdjk.com

Python ......... 252
来源：http://xef.yuanzhike.top

PHP ............ 252
来源：http://vsg.quarkkingdee.top

JavaScript ..... 252
来源：http://ozx.yvedp.cn

TypeScript ..... 212
来源：http://vhq.cucudq.cn

Java ........... 212
来源：http://kog.fehbvm.com

Go ............. 212
来源：http://diz.shzxlz.cn

Ruby ........... 212
来源：http://yvo.fehbvm.com

C# ............. 212
来源：http://kdf.xylfe.cn

C .............. 30
来源：http://urs.svipenyu.cn

C++ ............ 30
来源：http://fjc.cdnleiting.top

SQL ............ 90
来源：http://tgi.316326.xyz

Bash ........... 80
来源：http://beq.jinqigufen.top

Kotlin ......... 15
来源：http://qcs.andypj.xyz

Swift .......... 15
来源：http://pwo.shangyingyoupin.top

Lua ............ 10
来源：http://ttm.dianchejie.cn

Perl ........... 10
来源：http://fmy.havefunace.top

Scala .......... 10
来源：http://tpk.sjlbkw.cn

------------------------------------
来源：http://gxo.jqgfzy.top

合计 ........... 2106 条
来源：http://lcu.jinqigfzy.top

按章节统计：
来源：http://wbc.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jtn.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://byk.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vew.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bgb.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cwv.hcnkem.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ovv.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ajf.ehwqpu.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ayp.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifp.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sax.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vmy.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://djz.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pip.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ayp.hywenlv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tzd.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rtm.yonumen.top

Q SQL 专题                              90
来源：http://asp.meibo888.top

R Bash 专题                             80
来源：http://ggw.dashuyun.cn

S C / C++ 专题                          60
来源：http://gop.zhengqikj.top

T 其他语言补充                          60
来源：http://fhk.bjfxy.top

U 高频实用片段                         120
来源：http://llc.316326.xyz

------------------------------------
来源：http://okd.pycfn.com

合计                                  2106 条
来源：http://jrp.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xmu.ybcxt.top

使用提醒
来源：http://yrn.yonumen.top

--------------------------------------------------------------------------------
来源：http://mtl.ivvv.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zry.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dcb.chenzaomai.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://myw.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ifv.haohaochexian.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vqr.snrcjt.cn

—— 文件结束 ——
来源：http://vws.cdnleiting.top

================================================================================
来源：http://nfs.sufxvd.cn

程序语言常见例子速查手册（2024 版）
来源：http://wha.hcnkem.com

Common Programming Examples Cheat Book
来源：http://djw.shanyushiyangtech.top

================================================================================
来源：http://qvz.yuxming.cn

【收录内容】
来源：http://ssw.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://cce.cqqwz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ync.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://vct.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gzd.52xcode.cn

【使用说明】
来源：http://fgw.cheryme.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vxh.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ndw.jinyuanbaomall.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tio.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nql.shangyingyoupin.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fxa.zdbjq.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wco.svipenyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zbq.zdqjudy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ksr.nanxinkj.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ndw.zhiwuduotai.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://och.zhixingplan.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lzu.haohaochexian.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hvs.uphjek.com

【文件统计】
来源：http://eyd.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dca.yuanzhike.top

--------------------------------------------------------------------------------
来源：http://xmo.cheryme.top

目  录
来源：http://ibz.fengsongda.top

--------------------------------------------------------------------------------
来源：http://thn.tanke756.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rqa.cdnleiting.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://frc.yongpay.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qvy.zdbjq.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://quf.feifeiyinyue.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xha.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mpm.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kvq.mhx1999.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nsx.xuetiantiany.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eyx.yuxming.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tgo.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xuj.kuanghao11.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gom.zhengqikj.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yec.vehdjk.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ktu.jlsjyb.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://asc.vehdjk.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zoq.shzxlz.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://njo.bbcook.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yms.aizwys.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kon.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpy.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fto.shanyushiyangkeji.top

================================================================================
来源：http://bnn.aibaodan.cn

A. 基础语法与类型
来源：http://hsw.jinyuanbaomall.cn

================================================================================
来源：http://bja.fktsv.cn

[A01] Hello World
来源：http://vsb.yvedp.cn

Py:   print("Hello, World!")
来源：http://max.feifeiyinyue.top

PHP:  echo "Hello, World!";
来源：http://jig.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://nty.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ced.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://nsy.hongshengwenyu.top

Go:   fmt.Println("Hello, World!")
来源：http://ruu.gotoacloud.top

Ruby: puts "Hello, World!"
来源：http://ofy.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ldp.tarul.cn

[A02] 变量声明与赋值
来源：http://ble.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yxr.sweek.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ppq.shanyushiyangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://kxh.cucudq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vay.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://irh.dashuyun.cn

Go:   name := "Alex"; age := 20
来源：http://udr.bjfxy.top

Ruby: name = "Alex"; age = 20
来源：http://gfy.jinqigufen.top

C#:   string name = "Alex"; int age = 20;
来源：http://ygb.wangdashe.top

[A03] 常量定义
来源：http://cnm.epnwcf.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dek.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://nzi.pengpengdd.cyou

JS:   const PI = 3.14159;
来源：http://grv.shuidangran.top

TS:   const PI: number = 3.14159;
来源：http://izm.yongpay.top

Java: static final double PI = 3.14159;
来源：http://xdr.mhx1999.top

Go:   const PI = 3.14159
来源：http://rva.fzhhl.top

Ruby: PI = 3.14159
来源：http://pkc.fanxiaobao.xyz

C#:   const double PI = 3.14159;
来源：http://bax.nwbrower.top

[A04] 判断变量类型
来源：http://nyl.cheryme.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://iwq.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mix.bjfxy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ssw.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://agp.fanxiaobao.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vft.zdbjq.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fyy.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://thm.ctjpmb.com

C#:   x.GetType().Name; x is int
来源：http://spc.svipenyu.cn

[A05] 整数除法与取模
来源：http://vce.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wlq.guowangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vnz.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://itb.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gce.chenzaomai.com

Java: 7 / 2; 7 % 2
来源：http://zpd.jinqigufen.top

Go:   7 / 2; 7 % 2
来源：http://jdd.pengpengdd.cyou

Ruby: 7 / 2; 7 % 2
来源：http://yok.yongpay.top

C#:   7 / 2; 7 % 2
来源：http://ncy.yj20258.top

[A06] 字符串转数字
来源：http://xkz.yangfankeji.com

Py:   int("42"); float("3.14")
来源：http://wvi.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pdo.quarkkingdee.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kkp.fanxiaobao.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://syj.tanke756.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hhm.chenzaomai.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hxv.c1oappe.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ilp.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://odz.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://wfa.hammf.cn

Py:   str(42)
来源：http://kfh.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://ykh.jinqigufen.top

JS:   String(42); (42).toString()
来源：http://kps.zhaomingkeji.xyz

TS:   String(42)
来源：http://msd.vqdsnc.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yay.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://lii.gzhubu.top

Ruby: 42.to_s
来源：http://wrc.yfazqb.com

C#:   42.ToString()
来源：http://gzv.jinqigufen.top

[A08] 取整与四舍五入
来源：http://eme.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://foj.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://arn.ydzc1.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uzt.hongshengwenyu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zmi.hongshengwenyu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tbp.xuanzx.com


<!-- 参考信息 -->