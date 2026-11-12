代发 wailian999

[U57] PHP：字符串插值
来源：http://swl.jinqigfzy.top

"值: {$a}"
来源：http://tzc.uphjek.com

[U58] PHP：数组三件套
来源：http://qmc.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kyd.shuidangran.top

[U59] PHP：自定义排序
来源：http://fib.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fun.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://lms.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ter.cashguo.top

[U61] PHP：正则
来源：http://xyq.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tuk.guannengcc.top

[U62] PHP：日期对象
来源：http://oxk.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qox.hesvh.cn

[U63] PHP：文件读写
来源：http://nay.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mlz.sysykeji.top

[U64] PHP：目录遍历
来源：http://jvi.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://qke.yuxming.cn

[U65] PHP：会话
来源：http://xmv.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wsj.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://cvq.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fbe.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://rlg.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kgn.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://xlp.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yoe.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://put.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mcn.sysykeji.top

[U70] PHP：PDO 事务
来源：http://byj.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jep.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://rcg.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://izl.chenzaomai.com

[U72] PHP：写错误日志
来源：http://waj.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://whf.gaohongyu789.top

[U73] PHP：读取 ini 配置
来源：http://qll.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://yxy.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://tgn.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://emf.guowangkeji.top

[U75] PHP：依赖注入
来源：http://jjz.yuxming.cn

composer require psr/container
来源：http://dgt.aizwys.cn

[U76] PHP：简单路由
来源：http://eug.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pon.ehwqpu.com

[U77] PHP：模板渲染
来源：http://lpo.guowangkeji.top

composer require twig/twig
来源：http://rym.ydjk.org.cn

[U78] PHP：单元测试
来源：http://qju.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://orn.sxryk.cn

[U79] PHP：静态分析
来源：http://ewd.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://uut.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://eik.fanxiaobao.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://olg.zhoulong.xyz

[U81] JS：初始化项目
来源：http://wkh.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://auq.hcnkem.com

[U82] JS：package.json 脚本
来源：http://wuo.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nxh.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://rrm.shangyingyoupin.top

export const a = 1;  import { a } from "./m.js";
来源：http://whz.yanxiufei.cn

[U84] JS：CommonJS 写法
来源：http://lte.fengsongda.top

module.exports = { a };  const { a } = require("./m");
来源：http://jnk.chenlongwang.top

[U85] JS：可选链
来源：http://ghy.jqgufenzy.top

a?.b?.c
来源：http://njo.andypj.xyz

[U86] JS：空值合并
来源：http://ydt.zycfv.cn

a ?? b
来源：http://rja.tian-w.cn

[U87] JS：解构默认值
来源：http://ksy.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://nhs.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://juq.zdbjq.cn

{ ...a, ...b }
来源：http://xuz.hywenlv.cn

[U89] JS：数组去重
来源：http://qah.cheryme.top

[...new Set(arr)]
来源：http://xtu.mhx1999.top

[U90] JS：数字数组排序
来源：http://jpv.jinyuanbaomall.cn

[...arr].sort((a, b) => a - b)
来源：http://rrw.zhengqikj.top

[U91] JS：对象键值遍历
来源：http://vgh.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rzh.bjfxy.top

[U92] JS：深拷贝
来源：http://jja.nwbrower.top

structuredClone(obj)
来源：http://ywa.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://hiz.jqgfzy.top

`共 ${n} 条`
来源：http://zjo.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://dss.cqqwz.cn

const double = x => x * 2;
来源：http://uco.ybcxt.top

[U95] JS：Promise 包装
来源：http://lll.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://yjr.tianlin.xyz

[U96] JS：async/await 与异常
来源：http://gmc.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cae.pycfn.com

[U97] JS：并发请求
来源：http://noj.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://edu.ydjk.org.cn

[U98] JS：fetch 带 JSON
来源：http://bma.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nco.yvedp.cn

[U99] JS：事件监听
来源：http://hyl.yj20258.top

el.addEventListener("click", e => {})
来源：http://gdp.cheryme.top

[U100] JS：DOM 查询
来源：http://dyr.52xcode.cn

document.querySelector(".item")
来源：http://fln.cucudq.cn

[U101] JS：classList 操作
来源：http://ypa.bbcook.cn

el.classList.toggle("active")
来源：http://euj.yongpay.top

[U102] JS：本地存储
来源：http://kbf.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://pir.wangdashe.top

[U103] JS：定时器
来源：http://vnb.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gsj.tanke756.top

[U104] JS：防抖
来源：http://xri.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uta.nanxuanxn.top

[U105] JS：节流
来源：http://pnx.zhixingplan.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yyw.shuidangran.top

[U106] JS：日期格式化
来源：http://ogb.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ukp.yj202588.top

[U107] JS：数字千分位
来源：http://acc.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oyj.vqdsnc.cn

[U108] JS：随机整数
来源：http://vre.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vcr.xylfe.cn

[U109] JS：数组分组
来源：http://nlt.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://jle.bjfxy.top

[U110] JS：数组分块
来源：http://ufl.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rdm.chenlongwang.top

[U111] JS：对象转 Map
来源：http://qiw.aibaodan.cn

new Map(Object.entries(obj))
来源：http://mtj.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://hzc.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://qgk.quarkkingdee.top

[U113] JS：正则替换全部
来源：http://uli.gogol.net.cn

s.replaceAll("a", "b")
来源：http://ezt.fktsv.cn

[U114] JS：JSON 深比较
来源：http://hba.svipenyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tws.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://yul.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://juu.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://jhp.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://ltc.sweek.top

[U117] JS：单元测试
来源：http://gmq.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://apd.52xcode.cn

[U118] JS：开发服务器
来源：http://opc.ppjwa.cn

npm i -D vite;  npx vite
来源：http://kuw.bbcook.cn

[U119] JS：生产构建
来源：http://uww.nanxinkj.top

npx vite build
来源：http://bwf.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://wtd.316326.xyz

import.meta.env.VITE_API_URL
来源：http://mxf.fanxiaobao.xyz

================================================================================
来源：http://klt.sufxvd.cn

统计汇总
来源：http://uii.yongpay.top

================================================================================
来源：http://gmc.wangshuangyany.cn

按语言统计（条）：
来源：http://aht.jyoumei.cn

Python ......... 252
来源：http://xuv.haohaochexian.top

PHP ............ 252
来源：http://aex.sxryk.cn

JavaScript ..... 252
来源：http://goj.smart0.xyz

TypeScript ..... 212
来源：http://djj.nwbrower.top

Java ........... 212
来源：http://owh.andypj.xyz

Go ............. 212
来源：http://vej.cheryme.top

Ruby ........... 212
来源：http://bbx.xziqi.cn

C# ............. 212
来源：http://xxb.hysaishi.cn

C .............. 30
来源：http://fmm.fanxiaobao.xyz

C++ ............ 30
来源：http://rlk.zycfv.cn

SQL ............ 90
来源：http://vto.52xcode.cn

Bash ........... 80
来源：http://ypy.gaohongyu789.top

Kotlin ......... 15
来源：http://uzi.andypj.xyz

Swift .......... 15
来源：http://nca.jiagoushi.top

Lua ............ 10
来源：http://ckp.jqgufenzy.top

Perl ........... 10
来源：http://wgi.yongpay.top

Scala .......... 10
来源：http://tkf.yonumen.top

------------------------------------
来源：http://mii.c1oappe.top

合计 ........... 2106 条
来源：http://bvu.ydjk.org.cn

按章节统计：
来源：http://pxd.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://seb.yonumen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ukg.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fwj.shangyingyoupin.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ovh.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kls.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bco.zhiwuduotai.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zpk.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://psw.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xwg.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bph.shzxlz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lsa.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sef.shzxlz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ivs.xuanzx.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hdl.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ijg.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tqw.hammf.cn

Q SQL 专题                              90
来源：http://wyf.guowangkeji.top

R Bash 专题                             80
来源：http://qse.zdbjq.cn

S C / C++ 专题                          60
来源：http://avi.yj20258888.top

T 其他语言补充                          60
来源：http://csx.redwolf501.top

U 高频实用片段                         120
来源：http://jde.yvedp.cn

------------------------------------
来源：http://png.zhoulong.xyz

合计                                  2106 条
来源：http://rrn.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://uqb.zhaomingkeji.xyz

使用提醒
来源：http://ryr.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://wfs.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ldi.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://clp.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cwz.jqgufenzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://irh.yj202588.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vir.hesvh.cn

—— 文件结束 ——
来源：http://maj.sweek.top

================================================================================
来源：http://oid.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://irw.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://flv.shanyushiyangtech.top

================================================================================
来源：http://dtk.pengpengdd.cyou

【收录内容】
来源：http://mpa.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://tnl.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://son.jqgufenzy.top

SQL · Bash · C · C++
来源：http://xcy.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lsr.cheryme.top

【使用说明】
来源：http://hcd.ydjk.org.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hjg.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dgf.svipenyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kai.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cnr.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://krr.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ayg.birdmap.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kxn.yuanzhike.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rrf.quarkkingdee.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oop.fanxiaobao.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ebx.hongshengwenyu.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wsl.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gqa.tanke756.top

【文件统计】
来源：http://xbs.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vuk.iojbl.cn

--------------------------------------------------------------------------------
来源：http://arx.9152youxi.cn

目  录
来源：http://uiq.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://kkm.fktsv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://egw.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tac.guannengcc.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tro.fanxiaobao.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zyt.bbcook.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qqw.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rpe.jlsjyb.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mxk.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sul.yanxiufei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cgt.quarkkingdee.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fbj.hnqzz.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jjo.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://the.zdbjq.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gqv.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tgb.gaohongyu789.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oei.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yoj.jianghu66.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rnt.316326.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ici.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bcd.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rob.aibaodan.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kjw.zhijiandao.cn

================================================================================
来源：http://pzl.jinghuilouyu.cn

A. 基础语法与类型
来源：http://czl.andypj.xyz

================================================================================
来源：http://loe.ybcxt.top

[A01] Hello World
来源：http://ltu.hnqzz.top

Py:   print("Hello, World!")
来源：http://kqv.mhx1999.top

PHP:  echo "Hello, World!";
来源：http://pkv.c1oappe.top

JS:   console.log("Hello, World!");
来源：http://opw.hesvh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://shr.jiagoushi.top

Java: System.out.println("Hello, World!");
来源：http://thp.quarkkingdee.top

Go:   fmt.Println("Hello, World!")
来源：http://ohr.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://dgc.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://ihn.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://ezq.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dgd.ybcxt.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fuq.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://eoq.zhengqikj.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wop.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://yhd.ywan-chungtsiang.top

Go:   name := "Alex"; age := 20
来源：http://vji.zhiwuduotai.top

Ruby: name = "Alex"; age = 20
来源：http://mav.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ifq.gogol.net.cn

[A03] 常量定义
来源：http://gkm.yangfankeji.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nkx.yuxming.cn

PHP:  const PI = 3.14159;
来源：http://ebi.yj202588.top

JS:   const PI = 3.14159;
来源：http://dua.ydjk.org.cn

TS:   const PI: number = 3.14159;
来源：http://upq.yj202588.top

Java: static final double PI = 3.14159;
来源：http://ufe.tarul.cn

Go:   const PI = 3.14159
来源：http://atq.nanxuanxn.top

Ruby: PI = 3.14159
来源：http://fjy.bjfxy.top

C#:   const double PI = 3.14159;
来源：http://rlg.bjfxy.top

[A04] 判断变量类型
来源：http://kku.yuxming.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://afb.fehbvm.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bnk.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pjb.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://rre.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ekm.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jdo.zhengqikj.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cvf.ydjk.org.cn

C#:   x.GetType().Name; x is int
来源：http://dug.xylfe.cn

[A05] 整数除法与取模
来源：http://ure.ivvv.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hlg.yvedp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mgc.dashuyun.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://try.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gal.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://yut.yonumen.top

Go:   7 / 2; 7 % 2
来源：http://zim.ehwqpu.com

Ruby: 7 / 2; 7 % 2
来源：http://yzc.52xcode.cn

C#:   7 / 2; 7 % 2
来源：http://oax.smart0.xyz

[A06] 字符串转数字
来源：http://oyp.nanxinkj.top

Py:   int("42"); float("3.14")
来源：http://krs.jlsjyb.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uiz.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nzj.jinqigufen.top

TS:   parseInt("42", 10); Number("42")
来源：http://cik.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://iul.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ndw.aibaodan.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gjy.hnqzz.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://upc.shangyingyoupin.top

[A07] 数字转字符串
来源：http://uou.birdmap.top

Py:   str(42)
来源：http://rom.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://xil.jiagoushi.top

JS:   String(42); (42).toString()
来源：http://cww.xziqi.cn

TS:   String(42)
来源：http://aaj.chenlongwang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uaz.hfpthk.cn

Go:   strconv.Itoa(42)
来源：http://nke.ctjpmb.com

Ruby: 42.to_s
来源：http://hau.wangdashe.top

C#:   42.ToString()
来源：http://muk.meibo888.top

[A08] 取整与四舍五入
来源：http://ibd.wangshuangyany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mrg.yonumen.top


<!-- 参考信息 -->