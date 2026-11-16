代发 wailian999

[U59] PHP：自定义排序
来源：http://yiv.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kll.sweek.top

[U60] PHP：JSON 编解码
来源：http://xzu.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kjc.yvedp.cn

[U61] PHP：正则
来源：http://ewk.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://brw.svipenyu.cn

[U62] PHP：日期对象
来源：http://dtl.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zjg.nanxinkj.top

[U63] PHP：文件读写
来源：http://wij.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ocn.dashuyun.cn

[U64] PHP：目录遍历
来源：http://zvq.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://wta.bbcook.cn

[U65] PHP：会话
来源：http://drj.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ozf.birdmap.top

[U66] PHP：设置 Cookie
来源：http://tpw.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nji.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://ops.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bcz.redwolf501.top

[U68] PHP：PDO 连接
来源：http://icw.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gne.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://max.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://raw.cheryme.top

[U70] PHP：PDO 事务
来源：http://wzh.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qiu.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://ihp.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://oyh.316326.xyz

[U72] PHP：写错误日志
来源：http://nqh.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://jlv.mhx1999.top

[U73] PHP：读取 ini 配置
来源：http://llh.wangdashe.top

parse_ini_file("config.ini", true)
来源：http://ehw.xinyue.icu

[U74] PHP：读取环境变量
来源：http://axx.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://jsv.c1oappe.top

[U75] PHP：依赖注入
来源：http://yyz.iojbl.cn

composer require psr/container
来源：http://eva.dashuyun.cn

[U76] PHP：简单路由
来源：http://sos.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://skj.hesvh.cn

[U77] PHP：模板渲染
来源：http://aaq.fanxiaobao.xyz

composer require twig/twig
来源：http://ftm.yongpay.top

[U78] PHP：单元测试
来源：http://xtx.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://oeb.hnxiangtu.top

[U79] PHP：静态分析
来源：http://dsr.smart0.xyz

composer require --dev phpstan/phpstan
来源：http://rpa.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://kyj.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wxn.gzhubu.top

[U81] JS：初始化项目
来源：http://jqq.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://yim.fktsv.cn

[U82] JS：package.json 脚本
来源：http://omf.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hqs.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://akw.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://lzh.ivvv.top

[U84] JS：CommonJS 写法
来源：http://uot.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://yaa.epnwcf.com

[U85] JS：可选链
来源：http://gam.chenjidiqi.icu

a?.b?.c
来源：http://bgn.xziqi.cn

[U86] JS：空值合并
来源：http://vmr.fzhhl.top

a ?? b
来源：http://fwb.sysykeji.top

[U87] JS：解构默认值
来源：http://epz.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://asy.c1oappe.top

[U88] JS：对象展开合并
来源：http://agw.tianlin.xyz

{ ...a, ...b }
来源：http://dbc.sxryk.cn

[U89] JS：数组去重
来源：http://vuv.svipenyu.cn

[...new Set(arr)]
来源：http://ims.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://fvv.guowangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://hzi.fktsv.cn

[U91] JS：对象键值遍历
来源：http://fep.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oqy.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://tkm.yfazqb.com

structuredClone(obj)
来源：http://joz.redwolf501.top

[U93] JS：模板字符串
来源：http://dqd.yanxiufei.cn

`共 ${n} 条`
来源：http://qcu.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://ipl.jiagoushi.top

const double = x => x * 2;
来源：http://ndg.redwolf501.top

[U95] JS：Promise 包装
来源：http://ruz.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://gsx.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://qen.dashuyun.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zlu.hfpthk.cn

[U97] JS：并发请求
来源：http://hoi.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vzn.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://rkr.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jgq.gogol.net.cn

[U99] JS：事件监听
来源：http://xua.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://ixn.yfazqb.com

[U100] JS：DOM 查询
来源：http://hgj.guowangkeji.top

document.querySelector(".item")
来源：http://eas.bjfxy.top

[U101] JS：classList 操作
来源：http://qok.zycfv.cn

el.classList.toggle("active")
来源：http://enw.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://ivc.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hlk.chenlongwang.top

[U103] JS：定时器
来源：http://zyk.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ino.meibo888.top

[U104] JS：防抖
来源：http://zzg.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfx.tianlin.xyz

[U105] JS：节流
来源：http://bur.fengsongda.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qmy.vehdjk.com

[U106] JS：日期格式化
来源：http://slh.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gsc.zdbjq.cn

[U107] JS：数字千分位
来源：http://gnv.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jbp.xinyue.icu

[U108] JS：随机整数
来源：http://xyj.gzhubu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tpl.yj20258888.top

[U109] JS：数组分组
来源：http://pho.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://tzw.gotoacloud.top

[U110] JS：数组分块
来源：http://uoc.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wut.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://mzu.mhx1999.top

new Map(Object.entries(obj))
来源：http://kpt.316326.xyz

[U112] JS：字符串补位
来源：http://yhk.fzhhl.top

"7".padStart(3, "0")
来源：http://idd.ppjwa.cn

[U113] JS：正则替换全部
来源：http://kts.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://did.gogol.net.cn

[U114] JS：JSON 深比较
来源：http://zhr.zhengqikj.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tgk.xinyue.icu

[U115] JS：生成 UUID
来源：http://tzp.yonumen.top

crypto.randomUUID()
来源：http://yqx.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://jga.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://jaz.aibaodan.cn

[U117] JS：单元测试
来源：http://aiy.nwbrower.top

npm i -D vitest;  npx vitest
来源：http://mhu.fktsv.cn

[U118] JS：开发服务器
来源：http://khm.zhixingplan.top

npm i -D vite;  npx vite
来源：http://dfl.dianchejie.cn

[U119] JS：生产构建
来源：http://ssg.yj20258888.top

npx vite build
来源：http://uif.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://aaz.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://pum.guowangkeji.top

================================================================================
来源：http://qhb.nanxuanxn.top

统计汇总
来源：http://azx.gzhubu.top

================================================================================
来源：http://hot.nanxinkj.top

按语言统计（条）：
来源：http://lyo.9152youxi.cn

Python ......... 252
来源：http://ngb.dashuyun.cn

PHP ............ 252
来源：http://cyb.vqdsnc.cn

JavaScript ..... 252
来源：http://ref.tian-w.cn

TypeScript ..... 212
来源：http://nav.316326.xyz

Java ........... 212
来源：http://vrv.bjfxy.top

Go ............. 212
来源：http://bgd.9152youxi.cn

Ruby ........... 212
来源：http://xdq.daxiang520.top

C# ............. 212
来源：http://dpf.fengsongda.top

C .............. 30
来源：http://dhw.meibo888.top

C++ ............ 30
来源：http://tty.jiagoushi.top

SQL ............ 90
来源：http://mvg.sxryk.cn

Bash ........... 80
来源：http://wqw.vehdjk.com

Kotlin ......... 15
来源：http://vok.pengpengdd.cyou

Swift .......... 15
来源：http://daj.zycfv.cn

Lua ............ 10
来源：http://vhs.iojbl.cn

Perl ........... 10
来源：http://pdh.hfpthk.cn

Scala .......... 10
来源：http://wpl.zycfv.cn

------------------------------------
来源：http://nvv.tanke756.top

合计 ........... 2106 条
来源：http://fem.yongpay.top

按章节统计：
来源：http://hho.xinyue.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cfu.hnqzz.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pah.ydzc1.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gys.hnqzz.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://psv.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nym.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mhj.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iao.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gxc.tian-w.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mji.ppjwa.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cww.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cao.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cky.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wgr.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rpz.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ekk.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ozd.gzhubu.top

Q SQL 专题                              90
来源：http://kfk.zhongyouzk.top

R Bash 专题                             80
来源：http://kmj.haohaochexian.top

S C / C++ 专题                          60
来源：http://qul.ppjwa.cn

T 其他语言补充                          60
来源：http://eda.ppjwa.cn

U 高频实用片段                         120
来源：http://ysx.jiagoushi.top

------------------------------------
来源：http://nee.iojbl.cn

合计                                  2106 条
来源：http://mng.xinyue.icu

--------------------------------------------------------------------------------
来源：http://arv.hysaishi.cn

使用提醒
来源：http://yft.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://hkt.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://eym.jinqigfzy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://abi.52xcode.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uts.ydjk.org.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://siv.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yjp.gaohongyu789.top

—— 文件结束 ——
来源：http://sdt.birdmap.top

================================================================================
来源：http://ulo.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://eam.aizwys.cn

Common Programming Examples Cheat Book
来源：http://jdm.zhoulong.xyz

================================================================================
来源：http://rcy.chenlongwang.top

【收录内容】
来源：http://gwe.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rxj.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vlc.sxryk.cn

SQL · Bash · C · C++
来源：http://zxt.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nkq.fehbvm.com

【使用说明】
来源：http://mwj.dianchejie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://obu.guowangkeji.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hrt.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wjp.chenjidiqi.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wdt.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sjw.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bhm.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hqo.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mxd.fanxiaobao.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yyw.bjfxy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bkp.9152youxi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hxy.dashuyun.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fdg.vqdsnc.cn

【文件统计】
来源：http://sak.cheryme.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qbc.cheryme.top

--------------------------------------------------------------------------------
来源：http://qfv.redwolf501.top

目  录
来源：http://xge.iojbl.cn

--------------------------------------------------------------------------------
来源：http://zlx.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wly.ivvv.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tlt.cdnleiting.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ebc.daria6918.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://enb.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hgc.yj20258.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vdq.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://cui.quarkkingdee.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ebd.nwbrower.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gpg.jinqigufen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xzd.sweek.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vvv.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://csk.hesvh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hri.jinqigfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hlz.chenlongwang.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yag.bbcook.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://eiw.hywenlv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tau.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://htd.xinyue.icu

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dtw.hongshengwenyu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tjz.zhixingplan.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wky.zhaomingkeji.xyz

================================================================================
来源：http://pea.zhixingplan.top

A. 基础语法与类型
来源：http://ukw.chenzaomai.com

================================================================================
来源：http://jyn.aibaodan.cn

[A01] Hello World
来源：http://yjl.havefunace.top

Py:   print("Hello, World!")
来源：http://dao.shangyingyoupin.top

PHP:  echo "Hello, World!";
来源：http://byi.shuidangran.top

JS:   console.log("Hello, World!");
来源：http://soh.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jvk.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://ghr.yfazqb.com

Go:   fmt.Println("Hello, World!")
来源：http://kuc.chenjidiqi.icu

Ruby: puts "Hello, World!"
来源：http://yln.hongshengwenyu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://tzk.daxiang520.top

[A02] 变量声明与赋值
来源：http://pko.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wsr.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://xij.fktsv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://orq.fanxiaobao.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ecz.ctjpmb.com

Java: String name = "Alex"; int age = 20;
来源：http://gjj.316326.xyz

Go:   name := "Alex"; age := 20
来源：http://rhx.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://yuj.ivvv.top

C#:   string name = "Alex"; int age = 20;
来源：http://jcg.nwbrower.top

[A03] 常量定义
来源：http://ddf.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jcq.ydjk.org.cn

PHP:  const PI = 3.14159;
来源：http://iyr.dashuyun.cn

JS:   const PI = 3.14159;
来源：http://xxw.zhixingplan.top

TS:   const PI: number = 3.14159;
来源：http://uxa.zhaomingkeji.xyz

Java: static final double PI = 3.14159;
来源：http://ezp.feifeiyinyue.top

Go:   const PI = 3.14159
来源：http://onj.yueranfly.top

Ruby: PI = 3.14159
来源：http://lrx.meibo888.top

C#:   const double PI = 3.14159;
来源：http://zzs.pengpengdd.cyou

[A04] 判断变量类型
来源：http://fxm.9152youxi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cop.chenlongwang.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vkm.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eae.fzhhl.top

TS:   typeof x; x instanceof Date
来源：http://war.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tjb.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://nkk.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xfb.yueranfly.top

C#:   x.GetType().Name; x is int
来源：http://xpj.vqdsnc.cn

[A05] 整数除法与取模
来源：http://nfy.cashguo.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iom.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://nhv.shanyushiyangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jop.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nwx.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://ygl.ybcxt.top

Go:   7 / 2; 7 % 2
来源：http://cja.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://dte.yfazqb.com

C#:   7 / 2; 7 % 2
来源：http://ych.zycfv.cn

[A06] 字符串转数字
来源：http://bpo.jianghu66.top

Py:   int("42"); float("3.14")
来源：http://vgs.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qrw.chenlongwang.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cqn.daxiang520.top

TS:   parseInt("42", 10); Number("42")
来源：http://cqh.yangfankeji.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gix.redwolf501.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wsa.xuanzx.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qmc.zhengqikj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rqm.sxryk.cn

[A07] 数字转字符串
来源：http://eve.zhongyouzk.top

Py:   str(42)
来源：http://wlr.shangyingyoupin.top

PHP:  (string) 42; strval(42)
来源：http://vdg.andypj.xyz

JS:   String(42); (42).toString()
来源：http://tyt.xziqi.cn

TS:   String(42)
来源：http://juy.epnwcf.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://zwk.jlsjyb.cn

Go:   strconv.Itoa(42)
来源：http://lcv.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://uft.bbcook.cn

C#:   42.ToString()
来源：http://ere.hesvh.cn

[A08] 取整与四舍五入
来源：http://iia.52xcode.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gxf.gogol.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vqc.fehbvm.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ton.xinyue.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yif.zdbjq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://any.xylfe.cn


<!-- 参考信息 -->