代发 wailian999

[U53] PHP：空合并运算符
来源：http://ekp.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://pkz.shzxlz.cn

[U54] PHP：空安全调用
来源：http://nkw.cucudq.cn

$obj?->method()
来源：http://ala.zhaomingkeji.xyz

[U55] PHP：match 表达式
来源：http://sum.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wmg.wangdashe.top

[U56] PHP：命名参数
来源：http://mfs.jyoumei.cn

f(a: 1, b: 2)
来源：http://ykm.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://ogz.hfpthk.cn

"值: {$a}"
来源：http://qya.yongpay.top

[U58] PHP：数组三件套
来源：http://bli.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pns.xinyue.icu

[U59] PHP：自定义排序
来源：http://yna.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://net.cashguo.top

[U60] PHP：JSON 编解码
来源：http://gpe.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pwz.zhaomingkeji.xyz

[U61] PHP：正则
来源：http://hce.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mca.yongpay.top

[U62] PHP：日期对象
来源：http://tmq.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pwo.aibaodan.cn

[U63] PHP：文件读写
来源：http://yft.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fsw.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://yzj.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://ntb.fehbvm.com

[U65] PHP：会话
来源：http://xtj.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qam.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://evq.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yxu.havefunace.top

[U67] PHP：处理文件上传
来源：http://ufc.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kip.smart0.xyz

[U68] PHP：PDO 连接
来源：http://qnf.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iol.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://cai.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://khp.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://zhz.yueranfly.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bds.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://als.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://cey.daxiang520.top

[U72] PHP：写错误日志
来源：http://cql.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://lns.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://zfg.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://urz.epnwcf.com

[U74] PHP：读取环境变量
来源：http://sxo.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://vug.ehwqpu.com

[U75] PHP：依赖注入
来源：http://nza.gaohongyu789.top

composer require psr/container
来源：http://eqi.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://dfs.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sxq.jyoumei.cn

[U77] PHP：模板渲染
来源：http://grn.feifeiyinyue.top

composer require twig/twig
来源：http://hle.snrcjt.cn

[U78] PHP：单元测试
来源：http://hfg.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://maa.yvedp.cn

[U79] PHP：静态分析
来源：http://iac.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://fsq.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://svs.bjfxy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://djj.quarkkingdee.top

[U81] JS：初始化项目
来源：http://kxl.meibo888.top

npm init -y;  npm i express
来源：http://eta.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://hsn.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ehr.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://gdx.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://lkt.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://hsv.yj20258888.top

module.exports = { a };  const { a } = require("./m");
来源：http://igq.fehbvm.com

[U85] JS：可选链
来源：http://aci.jinqigfzy.top

a?.b?.c
来源：http://elh.ywan-chungtsiang.top

[U86] JS：空值合并
来源：http://gyb.hammf.cn

a ?? b
来源：http://jct.andypj.xyz

[U87] JS：解构默认值
来源：http://duu.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://nyr.daxiang520.top

[U88] JS：对象展开合并
来源：http://idh.xuanzx.com

{ ...a, ...b }
来源：http://jws.daxiang520.top

[U89] JS：数组去重
来源：http://kfr.jyoumei.cn

[...new Set(arr)]
来源：http://uac.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://oyc.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://hpi.zhixingplan.top

[U91] JS：对象键值遍历
来源：http://vzu.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mwg.daria6918.cn

[U92] JS：深拷贝
来源：http://pwv.wangshuangyany.cn

structuredClone(obj)
来源：http://pbn.uphjek.com

[U93] JS：模板字符串
来源：http://ely.xuetiantiany.cn

`共 ${n} 条`
来源：http://oev.cheryme.top

[U94] JS：箭头函数
来源：http://cwt.feifeiyinyue.top

const double = x => x * 2;
来源：http://bqn.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://yvp.jinqigufen.top

new Promise((resolve, reject) => {})
来源：http://bzu.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://vly.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vym.fktsv.cn

[U97] JS：并发请求
来源：http://noa.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pyh.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://hdn.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bmq.redwolf501.top

[U99] JS：事件监听
来源：http://ogc.vehdjk.com

el.addEventListener("click", e => {})
来源：http://gbs.yj20258888.top

[U100] JS：DOM 查询
来源：http://zwj.xziqi.cn

document.querySelector(".item")
来源：http://qlh.fzhhl.top

[U101] JS：classList 操作
来源：http://tds.gogol.net.cn

el.classList.toggle("active")
来源：http://ggs.zycfv.cn

[U102] JS：本地存储
来源：http://qhj.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://glo.jinghuilouyu.cn

[U103] JS：定时器
来源：http://iax.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://now.vqdsnc.cn

[U104] JS：防抖
来源：http://fea.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgj.wangdashe.top

[U105] JS：节流
来源：http://ecd.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fxa.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://pno.chenlongwang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gvz.dashuyun.cn

[U107] JS：数字千分位
来源：http://gpm.nanxuanxn.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yys.svipenyu.cn

[U108] JS：随机整数
来源：http://oah.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eiu.zycfv.cn

[U109] JS：数组分组
来源：http://clg.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://ucx.zdbjq.cn

[U110] JS：数组分块
来源：http://uws.ydzc1.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fpm.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://khz.zhengqikj.top

new Map(Object.entries(obj))
来源：http://hbl.52xcode.cn

[U112] JS：字符串补位
来源：http://gfx.jqgufenzy.top

"7".padStart(3, "0")
来源：http://jgr.0kj1m.cn

[U113] JS：正则替换全部
来源：http://wdh.shuidangran.top

s.replaceAll("a", "b")
来源：http://oim.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://onc.aizwys.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qfp.daxiang520.top

[U115] JS：生成 UUID
来源：http://oef.yongpay.top

crypto.randomUUID()
来源：http://emn.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://pqd.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://nsg.aibaodan.cn

[U117] JS：单元测试
来源：http://tck.tarul.cn

npm i -D vitest;  npx vitest
来源：http://bwp.jqgfzy.top

[U118] JS：开发服务器
来源：http://djq.smart0.xyz

npm i -D vite;  npx vite
来源：http://cfy.hammf.cn

[U119] JS：生产构建
来源：http://ejs.hywenlv.cn

npx vite build
来源：http://enn.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://gzr.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://dmu.andypj.xyz

================================================================================
来源：http://axz.svipenyu.cn

统计汇总
来源：http://uvs.xylfe.cn

================================================================================
来源：http://qcn.meibo888.top

按语言统计（条）：
来源：http://ocq.ivvv.top

Python ......... 252
来源：http://cuu.bjfxy.top

PHP ............ 252
来源：http://urb.tianlin.xyz

JavaScript ..... 252
来源：http://yvr.nanxinkj.top

TypeScript ..... 212
来源：http://tqy.tarul.cn

Java ........... 212
来源：http://yjy.yvedp.cn

Go ............. 212
来源：http://sgs.jiagoushi.top

Ruby ........... 212
来源：http://jas.xziqi.cn

C# ............. 212
来源：http://qon.nwbrower.top

C .............. 30
来源：http://weq.hcnkem.com

C++ ............ 30
来源：http://yhd.tianlin.xyz

SQL ............ 90
来源：http://qul.zhijiandao.cn

Bash ........... 80
来源：http://znb.guowangkeji.top

Kotlin ......... 15
来源：http://urq.yongpay.top

Swift .......... 15
来源：http://xvj.sweek.top

Lua ............ 10
来源：http://pnf.jlsjyb.cn

Perl ........... 10
来源：http://nmx.iojbl.cn

Scala .......... 10
来源：http://abf.hnxiangtu.top

------------------------------------
来源：http://qlg.xylfe.cn

合计 ........... 2106 条
来源：http://fhb.zhongyouzk.top

按章节统计：
来源：http://ezh.yangfankeji.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vmg.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ppp.hywenlv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qgr.jyoumei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xyp.xziqi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gom.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pqw.yanxiufei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hwi.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://shf.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cqw.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bjt.316326.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eqo.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ist.zhaomingkeji.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pbp.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sur.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://koo.quarkkingdee.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rqw.guowangkeji.top

Q SQL 专题                              90
来源：http://cxe.nanxuanxn.top

R Bash 专题                             80
来源：http://sab.hnxiangtu.top

S C / C++ 专题                          60
来源：http://qgm.iojbl.cn

T 其他语言补充                          60
来源：http://vlm.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://wky.chenlongwang.top

------------------------------------
来源：http://ief.fanxiaobao.xyz

合计                                  2106 条
来源：http://hie.redwolf501.top

--------------------------------------------------------------------------------
来源：http://vcr.yanxiufei.cn

使用提醒
来源：http://nsw.fengsongda.top

--------------------------------------------------------------------------------
来源：http://wfv.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lqw.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lzw.cdnleiting.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://iav.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://edb.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kqe.feifeiyinyue.top

—— 文件结束 ——
来源：http://csq.svipenyu.cn

================================================================================
来源：http://omm.ivvv.top

程序语言常见例子速查手册（2024 版）
来源：http://ene.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://ayz.sufxvd.cn

================================================================================
来源：http://zki.tanke756.top

【收录内容】
来源：http://pbn.quarkkingdee.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qct.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yqm.aizwys.cn

SQL · Bash · C · C++
来源：http://azb.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://omd.snrcjt.cn

【使用说明】
来源：http://sbk.feifeiyinyue.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lpn.cucudq.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jgz.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zzb.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://glf.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tgx.guannengcc.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uxi.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://min.hammf.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://epi.yfazqb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qos.epnwcf.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aul.zdbjq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bto.tanke756.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qmx.xingfuxueyuan.xyz

【文件统计】
来源：http://jlc.yj20258888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ges.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://gik.yonumen.top

目  录
来源：http://njp.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://fgv.yj20258.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ckm.ybcxt.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ycn.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ard.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fcn.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rhu.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://keb.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wyy.ppjwa.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gqv.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://chd.epnwcf.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pto.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://olf.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vzs.gzhubu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yhx.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ikh.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://orf.shzxlz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ljw.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pot.tarul.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qrs.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wer.ivvv.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://drm.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uta.epnwcf.com

================================================================================
来源：http://rsw.nwbrower.top

A. 基础语法与类型
来源：http://jiv.fktsv.cn

================================================================================
来源：http://uxr.cqqwz.cn

[A01] Hello World
来源：http://vyg.yuanzhike.top

Py:   print("Hello, World!")
来源：http://sye.pengpengdd.cyou

PHP:  echo "Hello, World!";
来源：http://lvn.ppjwa.cn

JS:   console.log("Hello, World!");
来源：http://ccd.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cyp.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://utk.jiagoushi.top

Go:   fmt.Println("Hello, World!")
来源：http://qsx.ppjwa.cn

Ruby: puts "Hello, World!"
来源：http://prp.zhijiandao.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://clw.xingfuxueyuan.xyz

[A02] 变量声明与赋值
来源：http://oqb.hnqzz.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hbs.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hpw.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://ypk.andypj.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tig.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://yyw.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://why.nanxinkj.top

Ruby: name = "Alex"; age = 20
来源：http://izf.yuanzhike.top

C#:   string name = "Alex"; int age = 20;
来源：http://whv.yueranfly.top

[A03] 常量定义
来源：http://bdm.zhaomingkeji.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://noh.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://sdl.sweek.top

JS:   const PI = 3.14159;
来源：http://wyy.hesvh.cn

TS:   const PI: number = 3.14159;
来源：http://zhq.cqqwz.cn

Java: static final double PI = 3.14159;
来源：http://whb.zdbjq.cn

Go:   const PI = 3.14159
来源：http://lae.xuetiantiany.cn

Ruby: PI = 3.14159
来源：http://zwp.fehbvm.com

C#:   const double PI = 3.14159;
来源：http://ppq.xylfe.cn

[A04] 判断变量类型
来源：http://kxd.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cty.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jdw.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rkj.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://myv.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xua.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://tby.shzxlz.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rzs.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://niu.xuetiantiany.cn

[A05] 整数除法与取模
来源：http://mor.ydzc1.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cid.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://iip.jinghuilouyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vlh.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iio.nanxinkj.top

Java: 7 / 2; 7 % 2
来源：http://zoq.cqqwz.cn

Go:   7 / 2; 7 % 2
来源：http://evm.xuanzx.com

Ruby: 7 / 2; 7 % 2
来源：http://yzi.ywan-chungtsiang.top

C#:   7 / 2; 7 % 2
来源：http://gbu.hongshengwenyu.top

[A06] 字符串转数字
来源：http://jea.quarkkingdee.top

Py:   int("42"); float("3.14")
来源：http://url.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rnx.zdqjudy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pbl.9152youxi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ubs.uphjek.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://amv.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tna.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://mfe.hammf.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://nsz.pycfn.com

[A07] 数字转字符串
来源：http://eiw.hfpthk.cn

Py:   str(42)
来源：http://byz.tarul.cn

PHP:  (string) 42; strval(42)
来源：http://pdu.daxiang520.top


<!-- 参考信息 -->