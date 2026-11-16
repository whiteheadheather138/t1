代发 wailian999

[U59] PHP：自定义排序
来源：http://qxo.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://klk.gzhubu.top

[U60] PHP：JSON 编解码
来源：http://ltm.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qwf.meibo888.top

[U61] PHP：正则
来源：http://ddm.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://udo.xylfe.cn

[U62] PHP：日期对象
来源：http://gmn.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xwi.tarul.cn

[U63] PHP：文件读写
来源：http://ycv.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://abk.ybcxt.top

[U64] PHP：目录遍历
来源：http://yqd.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://zbl.quarkkingdee.top

[U65] PHP：会话
来源：http://nak.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dlf.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://itd.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ked.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://dkn.hnqzz.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://olu.bjfxy.top

[U68] PHP：PDO 连接
来源：http://klz.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://azt.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://vwe.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://amy.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://zfg.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zpu.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://egd.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://fcn.yonumen.top

[U72] PHP：写错误日志
来源：http://lku.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://nkt.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://ptq.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://dkm.pycfn.com

[U74] PHP：读取环境变量
来源：http://iww.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://brr.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://azp.cashguo.top

composer require psr/container
来源：http://zmo.snrcjt.cn

[U76] PHP：简单路由
来源：http://tyu.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xyx.snrcjt.cn

[U77] PHP：模板渲染
来源：http://zcp.tian-w.cn

composer require twig/twig
来源：http://ehu.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://trs.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://xbp.fengsongda.top

[U79] PHP：静态分析
来源：http://cpi.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://wit.yj20258888.top

[U80] PHP：代码规范修复
来源：http://fup.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://klg.dashuyun.cn

[U81] JS：初始化项目
来源：http://hjj.jiagoushi.top

npm init -y;  npm i express
来源：http://ahx.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://fzi.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zci.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://kxb.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zhn.yj20258.top

[U84] JS：CommonJS 写法
来源：http://zpa.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jwd.jiagoushi.top

[U85] JS：可选链
来源：http://xxb.xylfe.cn

a?.b?.c
来源：http://yce.yj20258888.top

[U86] JS：空值合并
来源：http://qsc.xuanzx.com

a ?? b
来源：http://jae.sysykeji.top

[U87] JS：解构默认值
来源：http://vks.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://kkl.bbcook.cn

[U88] JS：对象展开合并
来源：http://yng.guannengcc.top

{ ...a, ...b }
来源：http://lcl.fengsongda.top

[U89] JS：数组去重
来源：http://gdo.cdnleiting.top

[...new Set(arr)]
来源：http://lyj.jianghu66.top

[U90] JS：数字数组排序
来源：http://she.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://vqr.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://htt.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://alv.smart0.xyz

[U92] JS：深拷贝
来源：http://dup.jlsjyb.cn

structuredClone(obj)
来源：http://jvq.zhijiandao.cn

[U93] JS：模板字符串
来源：http://aeg.jinghuilouyu.cn

`共 ${n} 条`
来源：http://rsg.aibaodan.cn

[U94] JS：箭头函数
来源：http://ofl.andypj.xyz

const double = x => x * 2;
来源：http://hvu.hcnkem.com

[U95] JS：Promise 包装
来源：http://sqc.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://ucc.redwolf501.top

[U96] JS：async/await 与异常
来源：http://arl.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ymv.cdnleiting.top

[U97] JS：并发请求
来源：http://qzx.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ivh.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://gln.jinqigfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yse.hywenlv.cn

[U99] JS：事件监听
来源：http://bzm.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://qsb.cdnleiting.top

[U100] JS：DOM 查询
来源：http://cyz.ppjwa.cn

document.querySelector(".item")
来源：http://mle.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://xgz.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://wob.jyoumei.cn

[U102] JS：本地存储
来源：http://ews.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fqe.ctjpmb.com

[U103] JS：定时器
来源：http://geu.birdmap.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://swf.yvedp.cn

[U104] JS：防抖
来源：http://edm.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lar.xinyue.icu

[U105] JS：节流
来源：http://dlp.hnxiangtu.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ybl.cucudq.cn

[U106] JS：日期格式化
来源：http://tvs.mhx1999.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyv.jqgfzy.top

[U107] JS：数字千分位
来源：http://qsh.zhixingplan.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rjf.guannengcc.top

[U108] JS：随机整数
来源：http://voi.fehbvm.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jqm.zhoulong.xyz

[U109] JS：数组分组
来源：http://rjo.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://vdr.nwbrower.top

[U110] JS：数组分块
来源：http://fff.fengsongda.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://otl.snrcjt.cn

[U111] JS：对象转 Map
来源：http://vaj.ybcxt.top

new Map(Object.entries(obj))
来源：http://swe.epnwcf.com

[U112] JS：字符串补位
来源：http://jxc.jqgfzy.top

"7".padStart(3, "0")
来源：http://aef.cdnleiting.top

[U113] JS：正则替换全部
来源：http://ssn.birdmap.top

s.replaceAll("a", "b")
来源：http://kqk.hammf.cn

[U114] JS：JSON 深比较
来源：http://psn.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://flt.yuxming.cn

[U115] JS：生成 UUID
来源：http://hec.vehdjk.com

crypto.randomUUID()
来源：http://kmv.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://yie.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://vak.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://icr.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://hdt.bjfxy.top

[U118] JS：开发服务器
来源：http://nrh.hesvh.cn

npm i -D vite;  npx vite
来源：http://xhf.gotoacloud.top

[U119] JS：生产构建
来源：http://wfs.sysykeji.top

npx vite build
来源：http://fdv.jinqigufen.top

[U120] JS：读取环境变量（Vite）
来源：http://urw.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://pmi.vqdsnc.cn

================================================================================
来源：http://dmy.xinyue.icu

统计汇总
来源：http://nef.iojbl.cn

================================================================================
来源：http://zuh.daxiang520.top

按语言统计（条）：
来源：http://tsp.nanxuanxn.top

Python ......... 252
来源：http://dxn.9152youxi.cn

PHP ............ 252
来源：http://cnj.tarul.cn

JavaScript ..... 252
来源：http://dff.jinghuilouyu.cn

TypeScript ..... 212
来源：http://fpd.daria6918.cn

Java ........... 212
来源：http://wje.hnxiangtu.top

Go ............. 212
来源：http://vpp.yuxming.cn

Ruby ........... 212
来源：http://hoo.havefunace.top

C# ............. 212
来源：http://uip.yuanzhike.top

C .............. 30
来源：http://xsq.zhijiandao.cn

C++ ............ 30
来源：http://ntp.shanyushiyangkeji.top

SQL ............ 90
来源：http://ulo.pycfn.com

Bash ........... 80
来源：http://ivg.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://pvt.shangyingyoupin.top

Swift .......... 15
来源：http://dou.hesvh.cn

Lua ............ 10
来源：http://opm.cucudq.cn

Perl ........... 10
来源：http://hiv.dashuyun.cn

Scala .......... 10
来源：http://mff.cheryme.top

------------------------------------
来源：http://enu.chenzaomai.com

合计 ........... 2106 条
来源：http://ydr.yj202588.top

按章节统计：
来源：http://izn.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wvv.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xhd.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vvd.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tsf.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kdb.wangdashe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jpw.jqgfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iht.daxiang520.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fsx.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vid.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jrc.vqdsnc.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://isq.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jrt.zhiwuduotai.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zpw.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://irr.svipenyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zlh.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lyo.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://neu.daxiang520.top

R Bash 专题                             80
来源：http://suf.nwbrower.top

S C / C++ 专题                          60
来源：http://bcd.jinqigfzy.top

T 其他语言补充                          60
来源：http://jhl.tanke756.top

U 高频实用片段                         120
来源：http://diq.yvedp.cn

------------------------------------
来源：http://xoy.smart0.xyz

合计                                  2106 条
来源：http://rku.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://bwz.shuidangran.top

使用提醒
来源：http://mmv.xylfe.cn

--------------------------------------------------------------------------------
来源：http://hvo.hnxiangtu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://emo.yongpay.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kix.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ymc.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://uht.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lfw.jianghu66.top

—— 文件结束 ——
来源：http://rmz.nwbrower.top

================================================================================
来源：http://bdv.shuidangran.top

程序语言常见例子速查手册（2024 版）
来源：http://jnj.hywenlv.cn

Common Programming Examples Cheat Book
来源：http://jkz.gogol.net.cn

================================================================================
来源：http://ocb.zhengqikj.top

【收录内容】
来源：http://mjo.meibo888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gjl.daria6918.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xbs.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://pjq.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://odi.aibaodan.cn

【使用说明】
来源：http://ife.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kdh.yj20258888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sbm.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mum.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fxj.jyoumei.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sho.gogol.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yjg.jqgfzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ojo.yangfankeji.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kal.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zua.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bty.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ftb.gotoacloud.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://spd.gotoacloud.top

【文件统计】
来源：http://nyw.ppjwa.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://plw.smart0.xyz

--------------------------------------------------------------------------------
来源：http://qos.smart0.xyz

目  录
来源：http://skf.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://gue.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pvb.hammf.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sfp.fzhhl.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://iqs.yj20258888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sea.zhiwuduotai.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vta.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uuj.hysaishi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://znc.zhengqikj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://knb.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fkv.zhoulong.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dts.tianlin.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pug.tarul.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rlp.feifeiyinyue.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ycd.smart0.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vcv.ehwqpu.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lqf.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pco.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sjv.tian-w.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://heu.hongshengwenyu.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oav.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fyd.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dtj.shanyushiyangtech.top

================================================================================
来源：http://frz.shangyingyoupin.top

A. 基础语法与类型
来源：http://fjb.yanxiufei.cn

================================================================================
来源：http://aba.wangdashe.top

[A01] Hello World
来源：http://giz.aibaodan.cn

Py:   print("Hello, World!")
来源：http://uig.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://bsu.zhiwuduotai.top

JS:   console.log("Hello, World!");
来源：http://tot.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pfz.vqdsnc.cn

Java: System.out.println("Hello, World!");
来源：http://jzo.hfpthk.cn

Go:   fmt.Println("Hello, World!")
来源：http://gtu.yfazqb.com

Ruby: puts "Hello, World!"
来源：http://mde.yanxiufei.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zzm.feifeiyinyue.top

[A02] 变量声明与赋值
来源：http://obx.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mog.hesvh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nce.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://coy.jinqigfzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ylv.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://wdm.yanxiufei.cn

Go:   name := "Alex"; age := 20
来源：http://khn.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://xpk.shuidangran.top

C#:   string name = "Alex"; int age = 20;
来源：http://dla.yfazqb.com

[A03] 常量定义
来源：http://drd.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pqp.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://bhw.cucudq.cn

JS:   const PI = 3.14159;
来源：http://qzh.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://ehz.haohaochexian.top

Java: static final double PI = 3.14159;
来源：http://fve.zdbjq.cn

Go:   const PI = 3.14159
来源：http://riw.yuanzhike.top

Ruby: PI = 3.14159
来源：http://yjs.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://bnj.zhoulong.xyz

[A04] 判断变量类型
来源：http://ufw.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://mqh.shangyingyoupin.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hob.zhongyouzk.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mgu.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://umx.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://smd.zhiwuduotai.top

Go:   reflect.TypeOf(x).Name()
来源：http://vuq.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://igq.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://pot.hnxiangtu.top

[A05] 整数除法与取模
来源：http://ubf.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uni.havefunace.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://jdj.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zdv.zhongyouzk.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cei.fehbvm.com

Java: 7 / 2; 7 % 2
来源：http://nuy.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://uvk.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://bdh.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://npm.hfpthk.cn

[A06] 字符串转数字
来源：http://jlh.zhiwuduotai.top

Py:   int("42"); float("3.14")
来源：http://dpx.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vaj.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lyo.c1oappe.top

TS:   parseInt("42", 10); Number("42")
来源：http://gxt.fehbvm.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://itu.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fbn.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zlb.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://plb.wangdashe.top

[A07] 数字转字符串
来源：http://qyx.hesvh.cn

Py:   str(42)
来源：http://wmx.yuxming.cn

PHP:  (string) 42; strval(42)
来源：http://pqh.cucudq.cn

JS:   String(42); (42).toString()
来源：http://ppo.jinqigufen.top

TS:   String(42)
来源：http://uhj.tianlin.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://uik.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://qnq.yuanzhike.top

Ruby: 42.to_s
来源：http://apg.yj20258888.top

C#:   42.ToString()
来源：http://zti.sjlbkw.cn

[A08] 取整与四舍五入
来源：http://dcy.yongpay.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://det.dashuyun.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://led.chenzaomai.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wpe.daxiang520.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ogs.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yva.yonumen.top


<!-- 参考信息 -->