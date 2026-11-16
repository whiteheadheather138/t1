代发 wailian999

[U51] PHP：数组解构
来源：http://lkc.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://hxh.9152youxi.cn

[U52] PHP：箭头函数
来源：http://zxd.yonumen.top

$double = fn($x) => $x * 2;
来源：http://xdj.gotoacloud.top

[U53] PHP：空合并运算符
来源：http://tgd.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://eih.guannengcc.top

[U54] PHP：空安全调用
来源：http://eld.yonumen.top

$obj?->method()
来源：http://bcg.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://rff.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mmp.fengsongda.top

[U56] PHP：命名参数
来源：http://oab.cheryme.top

f(a: 1, b: 2)
来源：http://xwg.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://wvn.xuanzx.com

"值: {$a}"
来源：http://vlm.hammf.cn

[U58] PHP：数组三件套
来源：http://ccz.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xju.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://ecw.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://irg.birdmap.top

[U60] PHP：JSON 编解码
来源：http://pkg.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uot.fktsv.cn

[U61] PHP：正则
来源：http://vgi.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yuo.svipenyu.cn

[U62] PHP：日期对象
来源：http://mqp.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xdk.daria6918.cn

[U63] PHP：文件读写
来源：http://quc.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ztz.ehwqpu.com

[U64] PHP：目录遍历
来源：http://eyk.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://xwr.ehwqpu.com

[U65] PHP：会话
来源：http://zcj.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mky.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://jwy.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vam.nwbrower.top

[U67] PHP：处理文件上传
来源：http://pwc.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://exm.bbcook.cn

[U68] PHP：PDO 连接
来源：http://qcu.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wqb.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://zyr.cdnleiting.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vrp.zycfv.cn

[U70] PHP：PDO 事务
来源：http://ctz.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://skf.snrcjt.cn

[U71] PHP：抛出异常
来源：http://lmi.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://yjz.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://rsz.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://lur.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://uga.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://wfy.jqgufenzy.top

[U74] PHP：读取环境变量
来源：http://oxl.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://icm.sxryk.cn

[U75] PHP：依赖注入
来源：http://pra.hnxiangtu.top

composer require psr/container
来源：http://iwv.daria6918.cn

[U76] PHP：简单路由
来源：http://khe.yuanzhike.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mit.haohaochexian.top

[U77] PHP：模板渲染
来源：http://twu.sjlbkw.cn

composer require twig/twig
来源：http://nrk.gotoacloud.top

[U78] PHP：单元测试
来源：http://cvk.wangdashe.top

composer require --dev phpunit/phpunit
来源：http://bdf.pycfn.com

[U79] PHP：静态分析
来源：http://jvb.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://xmx.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://teo.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xoe.aizwys.cn

[U81] JS：初始化项目
来源：http://oyv.jinqigfzy.top

npm init -y;  npm i express
来源：http://nrs.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://odf.daria6918.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hkr.gotoacloud.top

[U83] JS：ES Module 导入导出
来源：http://uzq.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cgb.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://oxl.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://rsb.birdmap.top

[U85] JS：可选链
来源：http://wad.xinyue.icu

a?.b?.c
来源：http://myo.havefunace.top

[U86] JS：空值合并
来源：http://mlt.tianlin.xyz

a ?? b
来源：http://wjq.fktsv.cn

[U87] JS：解构默认值
来源：http://gov.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://vcn.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://wrw.yueranfly.top

{ ...a, ...b }
来源：http://gxn.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://udx.aizwys.cn

[...new Set(arr)]
来源：http://csq.yj202588.top

[U90] JS：数字数组排序
来源：http://fnk.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://zeb.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://zko.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nqt.xziqi.cn

[U92] JS：深拷贝
来源：http://yhg.mhx1999.top

structuredClone(obj)
来源：http://tsk.dashuyun.cn

[U93] JS：模板字符串
来源：http://rdo.tian-w.cn

`共 ${n} 条`
来源：http://xzn.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://orb.yonumen.top

const double = x => x * 2;
来源：http://rsi.c1oappe.top

[U95] JS：Promise 包装
来源：http://gnr.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://luh.pycfn.com

[U96] JS：async/await 与异常
来源：http://wxv.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dil.tanke756.top

[U97] JS：并发请求
来源：http://wzp.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rkx.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://umu.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bey.ppjwa.cn

[U99] JS：事件监听
来源：http://qjh.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://edk.hesvh.cn

[U100] JS：DOM 查询
来源：http://ddl.tanke756.top

document.querySelector(".item")
来源：http://ymq.nanxuanxn.top

[U101] JS：classList 操作
来源：http://cfc.fengsongda.top

el.classList.toggle("active")
来源：http://wai.52xcode.cn

[U102] JS：本地存储
来源：http://von.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ivc.xziqi.cn

[U103] JS：定时器
来源：http://gqw.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ijm.guannengcc.top

[U104] JS：防抖
来源：http://cdd.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ytj.yueranfly.top

[U105] JS：节流
来源：http://pdt.wangdashe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fan.gogol.net.cn

[U106] JS：日期格式化
来源：http://rzo.tanke756.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://khh.dashuyun.cn

[U107] JS：数字千分位
来源：http://ggw.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zcc.zhongyouzk.top

[U108] JS：随机整数
来源：http://oop.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ivk.xuetiantiany.cn

[U109] JS：数组分组
来源：http://zvh.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://orj.xuanzx.com

[U110] JS：数组分块
来源：http://ukx.fehbvm.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jah.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://nxr.pycfn.com

new Map(Object.entries(obj))
来源：http://ngf.sxryk.cn

[U112] JS：字符串补位
来源：http://bqb.cqqwz.cn

"7".padStart(3, "0")
来源：http://zxj.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://cqr.tianlin.xyz

s.replaceAll("a", "b")
来源：http://tgv.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://adp.xziqi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hsl.zdqjudy.top

[U115] JS：生成 UUID
来源：http://bxo.vqdsnc.cn

crypto.randomUUID()
来源：http://xzr.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://aek.birdmap.top

/** @param {string} name */ function f(name) {}
来源：http://gbn.chenzaomai.com

[U117] JS：单元测试
来源：http://vgw.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://jfz.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://spe.xuetiantiany.cn

npm i -D vite;  npx vite
来源：http://gan.xylfe.cn

[U119] JS：生产构建
来源：http://bnu.shangyingyoupin.top

npx vite build
来源：http://afj.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://orz.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://ydz.hesvh.cn

================================================================================
来源：http://mwh.kuanghao11.cn

统计汇总
来源：http://eln.chenzaomai.com

================================================================================
来源：http://nef.yuanzhike.top

按语言统计（条）：
来源：http://njf.sxryk.cn

Python ......... 252
来源：http://qid.fanxiaobao.xyz

PHP ............ 252
来源：http://xmw.yj20258.top

JavaScript ..... 252
来源：http://nry.haohaochexian.top

TypeScript ..... 212
来源：http://lwp.ydjk.org.cn

Java ........... 212
来源：http://asz.yanxiufei.cn

Go ............. 212
来源：http://dnh.shangyingyoupin.top

Ruby ........... 212
来源：http://vlt.yueranfly.top

C# ............. 212
来源：http://mgt.xinyue.icu

C .............. 30
来源：http://dds.wangshuangyany.cn

C++ ............ 30
来源：http://yor.zhixingplan.top

SQL ............ 90
来源：http://oxr.jyoumei.cn

Bash ........... 80
来源：http://vzo.andypj.xyz

Kotlin ......... 15
来源：http://tiz.aibaodan.cn

Swift .......... 15
来源：http://acf.fengsongda.top

Lua ............ 10
来源：http://kfi.9152youxi.cn

Perl ........... 10
来源：http://alf.sufxvd.cn

Scala .......... 10
来源：http://zae.tian-w.cn

------------------------------------
来源：http://box.hysaishi.cn

合计 ........... 2106 条
来源：http://zkb.kuanghao11.cn

按章节统计：
来源：http://koe.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bjg.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ewc.xuanzx.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://del.zhiwuduotai.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://six.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gir.tarul.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://usp.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nyt.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ssl.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tra.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mev.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://upj.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qvs.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tuw.zycfv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rwt.jlsjyb.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mbz.zdqjudy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cfd.cashguo.top

Q SQL 专题                              90
来源：http://xuz.cqqwz.cn

R Bash 专题                             80
来源：http://kav.0kj1m.cn

S C / C++ 专题                          60
来源：http://huz.cheryme.top

T 其他语言补充                          60
来源：http://ibz.yuanzhike.top

U 高频实用片段                         120
来源：http://mxg.wangdashe.top

------------------------------------
来源：http://gvs.uphjek.com

合计                                  2106 条
来源：http://owd.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://xow.zdbjq.cn

使用提醒
来源：http://zpw.aizwys.cn

--------------------------------------------------------------------------------
来源：http://ddc.sysykeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ufv.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rtd.jqgufenzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdl.sjlbkw.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bdn.sxryk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zsg.kuanghao11.cn

—— 文件结束 ——
来源：http://qwd.pycfn.com

================================================================================
来源：http://iyt.hnqzz.top

程序语言常见例子速查手册（2024 版）
来源：http://gbq.jqgfzy.top

Common Programming Examples Cheat Book
来源：http://rqn.nanxuanxn.top

================================================================================
来源：http://zvv.jiagoushi.top

【收录内容】
来源：http://ash.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jdv.xingfuxueyuan.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nhk.wangdashe.top

SQL · Bash · C · C++
来源：http://fly.yfazqb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mph.iojbl.cn

【使用说明】
来源：http://aij.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uhy.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yql.hysaishi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lau.zhengqikj.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pgv.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wto.gzhubu.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kao.hnxiangtu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nih.redwolf501.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dmn.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cxl.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ytk.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://eis.meibo888.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jxq.yanxiufei.cn

【文件统计】
来源：http://elp.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rdp.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://mom.cucudq.cn

目  录
来源：http://avv.fehbvm.com

--------------------------------------------------------------------------------
来源：http://asd.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uow.bjfxy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rnr.jqgufenzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cck.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ucl.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vlt.jqgfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://miz.jyoumei.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ldi.chenjidiqi.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zdz.ctjpmb.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://clh.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tdr.pycfn.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lcn.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xoe.yangfankeji.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://brw.quarkkingdee.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://abc.gotoacloud.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uzk.jinghuilouyu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sng.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ykj.fengsongda.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://voq.jianghu66.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xxr.gotoacloud.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yrg.52xcode.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qua.tanke756.top

================================================================================
来源：http://mek.hnxiangtu.top

A. 基础语法与类型
来源：http://hbj.vehdjk.com

================================================================================
来源：http://pcf.redwolf501.top

[A01] Hello World
来源：http://knx.tianlin.xyz

Py:   print("Hello, World!")
来源：http://qxc.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://rol.zhongyouzk.top

JS:   console.log("Hello, World!");
来源：http://uuk.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ntr.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://pzq.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://cck.aizwys.cn

Ruby: puts "Hello, World!"
来源：http://kvv.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://hes.shanyushiyangtech.top

[A02] 变量声明与赋值
来源：http://ypm.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bjv.nanxuanxn.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pwx.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kbs.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ecu.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://pmj.tian-w.cn

Go:   name := "Alex"; age := 20
来源：http://jmn.316326.xyz

Ruby: name = "Alex"; age = 20
来源：http://xsv.jinqigfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://sgl.yueranfly.top

[A03] 常量定义
来源：http://aez.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nqb.yongpay.top

PHP:  const PI = 3.14159;
来源：http://nzz.snrcjt.cn

JS:   const PI = 3.14159;
来源：http://bhe.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://loc.ybcxt.top

Java: static final double PI = 3.14159;
来源：http://zvb.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://blb.hesvh.cn

Ruby: PI = 3.14159
来源：http://hyc.hysaishi.cn

C#:   const double PI = 3.14159;
来源：http://nhj.wangdashe.top

[A04] 判断变量类型
来源：http://kpa.jinyuanbaomall.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ild.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jam.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mvn.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://owz.daria6918.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cmg.hnqzz.top

Go:   reflect.TypeOf(x).Name()
来源：http://rko.chenlongwang.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xhv.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://qin.yvedp.cn

[A05] 整数除法与取模
来源：http://atm.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://alo.ydzc1.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lxp.nanxinkj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://akn.sweek.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xmk.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://ezb.nanxinkj.top

Go:   7 / 2; 7 % 2
来源：http://thn.chenzaomai.com

Ruby: 7 / 2; 7 % 2
来源：http://fsa.cdnleiting.top

C#:   7 / 2; 7 % 2
来源：http://yex.quarkkingdee.top

[A06] 字符串转数字
来源：http://euv.havefunace.top

Py:   int("42"); float("3.14")
来源：http://hub.havefunace.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://azr.gaohongyu789.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pei.jianghu66.top

TS:   parseInt("42", 10); Number("42")
来源：http://psp.jlsjyb.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yfg.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ibs.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zfi.cashguo.top


<!-- 参考信息 -->