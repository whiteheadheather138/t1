代发 wailian999

[U61] PHP：正则
来源：http://cpg.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zxj.yvedp.cn

[U62] PHP：日期对象
来源：http://wqq.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hgh.yuxming.cn

[U63] PHP：文件读写
来源：http://kxo.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lcr.bjfxy.top

[U64] PHP：目录遍历
来源：http://lzk.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://hgv.c1oappe.top

[U65] PHP：会话
来源：http://icr.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://sss.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://clc.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xia.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://jta.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://eyn.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://ddt.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ieu.mhx1999.top

[U69] PHP：PDO 预处理
来源：http://zpj.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vio.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://dku.pengpengdd.cyou

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jwc.xziqi.cn

[U71] PHP：抛出异常
来源：http://gjm.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://pts.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://joi.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://jgn.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://cnf.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://sxr.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://tfw.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://pkq.yuxming.cn

[U75] PHP：依赖注入
来源：http://nrh.pycfn.com

composer require psr/container
来源：http://cor.yfazqb.com

[U76] PHP：简单路由
来源：http://qna.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ura.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://azp.ydjk.org.cn

composer require twig/twig
来源：http://bdq.yuxming.cn

[U78] PHP：单元测试
来源：http://qid.shzxlz.cn

composer require --dev phpunit/phpunit
来源：http://nvy.redwolf501.top

[U79] PHP：静态分析
来源：http://dsx.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://twz.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://hmr.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ogx.hnxiangtu.top

[U81] JS：初始化项目
来源：http://tqg.sweek.top

npm init -y;  npm i express
来源：http://ihm.birdmap.top

[U82] JS：package.json 脚本
来源：http://nvl.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fve.zhijiandao.cn

[U83] JS：ES Module 导入导出
来源：http://sog.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://ygn.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://huh.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://mjc.yuanzhike.top

[U85] JS：可选链
来源：http://tmb.mhx1999.top

a?.b?.c
来源：http://vod.daria6918.cn

[U86] JS：空值合并
来源：http://aus.kuanghao11.cn

a ?? b
来源：http://mln.cashguo.top

[U87] JS：解构默认值
来源：http://xhu.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://ger.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://ock.jqgfzy.top

{ ...a, ...b }
来源：http://cww.gaohongyu789.top

[U89] JS：数组去重
来源：http://lgb.yuanzhike.top

[...new Set(arr)]
来源：http://acq.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://jls.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://qbb.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://snj.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qvq.jiagoushi.top

[U92] JS：深拷贝
来源：http://lyz.yvedp.cn

structuredClone(obj)
来源：http://zjw.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://yms.cashguo.top

`共 ${n} 条`
来源：http://kba.cheryme.top

[U94] JS：箭头函数
来源：http://qcs.hnxiangtu.top

const double = x => x * 2;
来源：http://pic.dashuyun.cn

[U95] JS：Promise 包装
来源：http://ktb.birdmap.top

new Promise((resolve, reject) => {})
来源：http://imc.redwolf501.top

[U96] JS：async/await 与异常
来源：http://bhk.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dmm.sufxvd.cn

[U97] JS：并发请求
来源：http://efi.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wnn.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://emk.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ket.wangdashe.top

[U99] JS：事件监听
来源：http://qrf.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://ruz.nanxinkj.top

[U100] JS：DOM 查询
来源：http://hfa.xinyue.icu

document.querySelector(".item")
来源：http://dio.sxryk.cn

[U101] JS：classList 操作
来源：http://fyw.yuanzhike.top

el.classList.toggle("active")
来源：http://fae.yonumen.top

[U102] JS：本地存储
来源：http://jgu.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zbx.zycfv.cn

[U103] JS：定时器
来源：http://afo.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ytk.ybcxt.top

[U104] JS：防抖
来源：http://aaz.vehdjk.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svi.gzhubu.top

[U105] JS：节流
来源：http://tgp.yj202588.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ydj.fktsv.cn

[U106] JS：日期格式化
来源：http://obg.hcnkem.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lkq.redwolf501.top

[U107] JS：数字千分位
来源：http://sqk.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uri.yonumen.top

[U108] JS：随机整数
来源：http://mtg.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lps.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://yii.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://kwg.gotoacloud.top

[U110] JS：数组分块
来源：http://efs.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zyk.haohaochexian.top

[U111] JS：对象转 Map
来源：http://vbr.ybcxt.top

new Map(Object.entries(obj))
来源：http://etq.yuanzhike.top

[U112] JS：字符串补位
来源：http://jpf.sufxvd.cn

"7".padStart(3, "0")
来源：http://rpp.pengpengdd.cyou

[U113] JS：正则替换全部
来源：http://ote.xinyue.icu

s.replaceAll("a", "b")
来源：http://jww.316326.xyz

[U114] JS：JSON 深比较
来源：http://put.guannengcc.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://unv.pycfn.com

[U115] JS：生成 UUID
来源：http://dcq.hysaishi.cn

crypto.randomUUID()
来源：http://kmj.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://yvs.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://ape.zycfv.cn

[U117] JS：单元测试
来源：http://kpd.tarul.cn

npm i -D vitest;  npx vitest
来源：http://nvu.guowangkeji.top

[U118] JS：开发服务器
来源：http://svz.havefunace.top

npm i -D vite;  npx vite
来源：http://jpy.ivvv.top

[U119] JS：生产构建
来源：http://nvf.zhoulong.xyz

npx vite build
来源：http://qqv.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://oud.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://aqj.birdmap.top

================================================================================
来源：http://bhb.yj20258.top

统计汇总
来源：http://bwt.zhongyouzk.top

================================================================================
来源：http://ute.shzxlz.cn

按语言统计（条）：
来源：http://ine.gaohongyu789.top

Python ......... 252
来源：http://ita.hnqzz.top

PHP ............ 252
来源：http://fcy.yueranfly.top

JavaScript ..... 252
来源：http://khu.jianghu66.top

TypeScript ..... 212
来源：http://xbb.zhoulong.xyz

Java ........... 212
来源：http://ska.ppjwa.cn

Go ............. 212
来源：http://qsu.sufxvd.cn

Ruby ........... 212
来源：http://qpy.yongpay.top

C# ............. 212
来源：http://wnx.gotoacloud.top

C .............. 30
来源：http://lat.yonumen.top

C++ ............ 30
来源：http://pyl.snrcjt.cn

SQL ............ 90
来源：http://ien.zhengqikj.top

Bash ........... 80
来源：http://ekv.dashuyun.cn

Kotlin ......... 15
来源：http://ogu.yonumen.top

Swift .......... 15
来源：http://lnk.daxiang520.top

Lua ............ 10
来源：http://kiu.wangdashe.top

Perl ........... 10
来源：http://jit.meibo888.top

Scala .......... 10
来源：http://iin.c1oappe.top

------------------------------------
来源：http://may.9152youxi.cn

合计 ........... 2106 条
来源：http://rzf.sweek.top

按章节统计：
来源：http://hvn.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vkp.sweek.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://chu.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pla.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xaz.zycfv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zgv.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xud.yongpay.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rnv.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mai.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://duj.vehdjk.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kfw.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vyq.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://slg.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qwu.wangdashe.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ytw.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ctf.xuetiantiany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pwd.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://oyn.ctjpmb.com

R Bash 专题                             80
来源：http://hjx.guowangkeji.top

S C / C++ 专题                          60
来源：http://ckv.kuanghao11.cn

T 其他语言补充                          60
来源：http://rmb.aizwys.cn

U 高频实用片段                         120
来源：http://tmt.aizwys.cn

------------------------------------
来源：http://moy.tian-w.cn

合计                                  2106 条
来源：http://xbv.fktsv.cn

--------------------------------------------------------------------------------
来源：http://pda.sweek.top

使用提醒
来源：http://gpo.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://jtd.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hrd.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bod.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qno.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://zfk.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qsi.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://qnx.fengsongda.top

================================================================================
来源：http://obc.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://yzd.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://jny.shanyushiyangtech.top

================================================================================
来源：http://zlx.9152youxi.cn

【收录内容】
来源：http://dyt.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nlp.zhixingplan.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://biv.shanyushiyangkeji.top

SQL · Bash · C · C++
来源：http://jls.zhengqikj.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://trv.vehdjk.com

【使用说明】
来源：http://psh.gaohongyu789.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rbc.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vvx.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kgd.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xfe.zdqjudy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://epb.mhx1999.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dyy.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://noo.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tph.tarul.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qzb.0kj1m.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://shp.yj20258.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://udv.jlsjyb.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cky.zhongyouzk.top

【文件统计】
来源：http://tvs.tianlin.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mxi.c1oappe.top

--------------------------------------------------------------------------------
来源：http://fpu.mhx1999.top

目  录
来源：http://tci.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://asf.ydjk.org.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dbt.aibaodan.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jln.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wal.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tea.fanxiaobao.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://msq.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gbk.guowangkeji.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hgv.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bhc.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gbs.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bxe.cdnleiting.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://laa.cucudq.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://piw.yueranfly.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ofe.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qei.epnwcf.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ene.yonumen.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vzz.shangyingyoupin.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://czh.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ekj.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rdx.cashguo.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pfk.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jln.meibo888.top

================================================================================
来源：http://kyg.gaohongyu789.top

A. 基础语法与类型
来源：http://bja.kuanghao11.cn

================================================================================
来源：http://uxx.zdqjudy.top

[A01] Hello World
来源：http://qyd.yuanzhike.top

Py:   print("Hello, World!")
来源：http://brm.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://cgp.jinqigfzy.top

JS:   console.log("Hello, World!");
来源：http://uae.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zxt.pycfn.com

Java: System.out.println("Hello, World!");
来源：http://twx.mhx1999.top

Go:   fmt.Println("Hello, World!")
来源：http://ykc.ctjpmb.com

Ruby: puts "Hello, World!"
来源：http://ked.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://vyn.fehbvm.com

[A02] 变量声明与赋值
来源：http://ztv.jlsjyb.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://auq.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bxq.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://muc.yj20258.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kbl.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://ffv.9152youxi.cn

Go:   name := "Alex"; age := 20
来源：http://afe.haohaochexian.top

Ruby: name = "Alex"; age = 20
来源：http://iui.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://yxp.yuxming.cn

[A03] 常量定义
来源：http://xnd.shuidangran.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://akf.yongpay.top

PHP:  const PI = 3.14159;
来源：http://boj.zhixingplan.top

JS:   const PI = 3.14159;
来源：http://ttp.uphjek.com

TS:   const PI: number = 3.14159;
来源：http://zcr.yuxming.cn

Java: static final double PI = 3.14159;
来源：http://fbl.cqqwz.cn

Go:   const PI = 3.14159
来源：http://vzp.hongshengwenyu.top

Ruby: PI = 3.14159
来源：http://xus.snrcjt.cn

C#:   const double PI = 3.14159;
来源：http://jng.hnxiangtu.top

[A04] 判断变量类型
来源：http://bie.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zbj.ywan-chungtsiang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tbk.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bul.zhoulong.xyz

TS:   typeof x; x instanceof Date
来源：http://pyi.zdbjq.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pec.sjlbkw.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pnj.cheryme.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cjb.haohaochexian.top

C#:   x.GetType().Name; x is int
来源：http://pwm.nanxinkj.top

[A05] 整数除法与取模
来源：http://wmo.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xxi.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uop.hesvh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qwp.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgk.ivvv.top

Java: 7 / 2; 7 % 2
来源：http://hjq.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://xyy.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://zcn.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://bux.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://nyn.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://ypr.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tyl.tanke756.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zme.tarul.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tgf.zdbjq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://djx.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mam.chenlongwang.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lcf.daria6918.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://smy.xziqi.cn

[A07] 数字转字符串
来源：http://vai.hcnkem.com

Py:   str(42)
来源：http://gpd.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://qoh.guannengcc.top

JS:   String(42); (42).toString()
来源：http://kmw.sjlbkw.cn

TS:   String(42)
来源：http://kgy.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kzb.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://tjt.cheryme.top

Ruby: 42.to_s
来源：http://oiu.hnxiangtu.top

C#:   42.ToString()
来源：http://mfu.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://lkt.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ltm.jinqigufen.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yds.jiagoushi.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jpi.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://niq.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rao.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jbq.smart0.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://vjr.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wyk.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://fzx.haohaochexian.top


<!-- 参考信息 -->