代发 wailian999

[U49] PHP：只读属性
来源：http://zeb.chenzaomai.com

public readonly string $name
来源：http://gpz.ydjk.org.cn

[U50] PHP：构造器属性提升
来源：http://toq.jianghu66.top

public function __construct(private int $id) {}
来源：http://lgl.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://srq.nanxuanxn.top

[$a, $b] = $arr;
来源：http://sep.xylfe.cn

[U52] PHP：箭头函数
来源：http://lfq.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://phs.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://kwr.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://vyl.gaohongyu789.top

[U54] PHP：空安全调用
来源：http://zih.xuetiantiany.cn

$obj?->method()
来源：http://tgp.sweek.top

[U55] PHP：match 表达式
来源：http://txb.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kic.hammf.cn

[U56] PHP：命名参数
来源：http://yen.jqgufenzy.top

f(a: 1, b: 2)
来源：http://kcc.yongpay.top

[U57] PHP：字符串插值
来源：http://oam.guowangkeji.top

"值: {$a}"
来源：http://eem.snrcjt.cn

[U58] PHP：数组三件套
来源：http://zqz.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hpx.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://cag.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lrm.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://hdn.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kqw.haohaochexian.top

[U61] PHP：正则
来源：http://bvs.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xpt.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://azg.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mrd.nanxinkj.top

[U63] PHP：文件读写
来源：http://kdc.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yrr.cdnleiting.top

[U64] PHP：目录遍历
来源：http://phk.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://clm.zhengqikj.top

[U65] PHP：会话
来源：http://jza.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ser.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://onp.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kei.tarul.cn

[U67] PHP：处理文件上传
来源：http://nke.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qpj.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://cwf.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zzf.ywan-chungtsiang.top

[U69] PHP：PDO 预处理
来源：http://cnm.shzxlz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ggy.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://ntt.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ebb.shanyushiyangkeji.top

[U71] PHP：抛出异常
来源：http://awh.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://ein.gzhubu.top

[U72] PHP：写错误日志
来源：http://jeg.tianlin.xyz

error_log("失败: " . $e->getMessage());
来源：http://dyy.sweek.top

[U73] PHP：读取 ini 配置
来源：http://drx.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://gul.epnwcf.com

[U74] PHP：读取环境变量
来源：http://sql.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://mxe.fehbvm.com

[U75] PHP：依赖注入
来源：http://xuy.gogol.net.cn

composer require psr/container
来源：http://yhf.nwbrower.top

[U76] PHP：简单路由
来源：http://hwt.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bcu.52xcode.cn

[U77] PHP：模板渲染
来源：http://cbt.shangyingyoupin.top

composer require twig/twig
来源：http://jjv.ehwqpu.com

[U78] PHP：单元测试
来源：http://lvc.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://eqg.shzxlz.cn

[U79] PHP：静态分析
来源：http://nwx.gotoacloud.top

composer require --dev phpstan/phpstan
来源：http://ufd.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://nwv.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sfh.tianlin.xyz

[U81] JS：初始化项目
来源：http://dsa.guowangkeji.top

npm init -y;  npm i express
来源：http://sve.xinyue.icu

[U82] JS：package.json 脚本
来源：http://mio.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ftc.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://aes.tanke756.top

export const a = 1;  import { a } from "./m.js";
来源：http://puu.yongpay.top

[U84] JS：CommonJS 写法
来源：http://zya.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rgs.yanxiufei.cn

[U85] JS：可选链
来源：http://wra.shuidangran.top

a?.b?.c
来源：http://iiu.aibaodan.cn

[U86] JS：空值合并
来源：http://wsl.pycfn.com

a ?? b
来源：http://ytb.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://prq.vqdsnc.cn

const { a = 1, b = 2 } = obj;
来源：http://eqo.ivvv.top

[U88] JS：对象展开合并
来源：http://pjc.nwbrower.top

{ ...a, ...b }
来源：http://ddd.nanxuanxn.top

[U89] JS：数组去重
来源：http://khl.bbcook.cn

[...new Set(arr)]
来源：http://jpo.daxiang520.top

[U90] JS：数字数组排序
来源：http://ygm.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://zle.yonumen.top

[U91] JS：对象键值遍历
来源：http://ngp.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tgt.kuanghao11.cn

[U92] JS：深拷贝
来源：http://ajy.chenjidiqi.icu

structuredClone(obj)
来源：http://pcn.cqqwz.cn

[U93] JS：模板字符串
来源：http://shx.sufxvd.cn

`共 ${n} 条`
来源：http://ohg.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://zwm.chenlongwang.top

const double = x => x * 2;
来源：http://mxg.pycfn.com

[U95] JS：Promise 包装
来源：http://vjr.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://khz.yvedp.cn

[U96] JS：async/await 与异常
来源：http://dgg.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gxq.cdnleiting.top

[U97] JS：并发请求
来源：http://ldf.vehdjk.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ecn.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://glw.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bwo.jqgufenzy.top

[U99] JS：事件监听
来源：http://fei.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://lge.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://zbe.aibaodan.cn

document.querySelector(".item")
来源：http://qes.zdqjudy.top

[U101] JS：classList 操作
来源：http://gwq.zdbjq.cn

el.classList.toggle("active")
来源：http://pdg.jinqigufen.top

[U102] JS：本地存储
来源：http://xli.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://xhc.fengsongda.top

[U103] JS：定时器
来源：http://azl.kuanghao11.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cut.aizwys.cn

[U104] JS：防抖
来源：http://bjw.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zbg.xziqi.cn

[U105] JS：节流
来源：http://wwg.c1oappe.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fjw.tianlin.xyz

[U106] JS：日期格式化
来源：http://siz.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jua.xziqi.cn

[U107] JS：数字千分位
来源：http://wrx.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xmo.feifeiyinyue.top

[U108] JS：随机整数
来源：http://uqk.sysykeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://epl.birdmap.top

[U109] JS：数组分组
来源：http://spn.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://rgn.cqqwz.cn

[U110] JS：数组分块
来源：http://pzk.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dvp.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://qqc.yfazqb.com

new Map(Object.entries(obj))
来源：http://shr.shuidangran.top

[U112] JS：字符串补位
来源：http://azn.jlsjyb.cn

"7".padStart(3, "0")
来源：http://tfg.ctjpmb.com

[U113] JS：正则替换全部
来源：http://iqn.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://pqu.uphjek.com

[U114] JS：JSON 深比较
来源：http://uvc.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qwz.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://gzr.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://rzq.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://pck.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://lei.chenzaomai.com

[U117] JS：单元测试
来源：http://dop.havefunace.top

npm i -D vitest;  npx vitest
来源：http://zky.yanxiufei.cn

[U118] JS：开发服务器
来源：http://jey.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://psw.cashguo.top

[U119] JS：生产构建
来源：http://iyk.svipenyu.cn

npx vite build
来源：http://ynd.hcnkem.com

[U120] JS：读取环境变量（Vite）
来源：http://iun.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://whl.jyoumei.cn

================================================================================
来源：http://xjx.meibo888.top

统计汇总
来源：http://fil.dianchejie.cn

================================================================================
来源：http://pje.316326.xyz

按语言统计（条）：
来源：http://yfu.redwolf501.top

Python ......... 252
来源：http://shv.yueranfly.top

PHP ............ 252
来源：http://iki.fktsv.cn

JavaScript ..... 252
来源：http://nyi.yvedp.cn

TypeScript ..... 212
来源：http://upo.zhixingplan.top

Java ........... 212
来源：http://zyp.zhixingplan.top

Go ............. 212
来源：http://nia.zycfv.cn

Ruby ........... 212
来源：http://cvu.zdqjudy.top

C# ............. 212
来源：http://ywv.316326.xyz

C .............. 30
来源：http://etx.shuidangran.top

C++ ............ 30
来源：http://enk.shanyushiyangkeji.top

SQL ............ 90
来源：http://cjo.epnwcf.com

Bash ........... 80
来源：http://lud.snrcjt.cn

Kotlin ......... 15
来源：http://nvs.hfpthk.cn

Swift .......... 15
来源：http://put.shanyushiyangtech.top

Lua ............ 10
来源：http://qyv.ybcxt.top

Perl ........... 10
来源：http://mmb.kuanghao11.cn

Scala .......... 10
来源：http://nfv.ydzc1.top

------------------------------------
来源：http://ibn.zycfv.cn

合计 ........... 2106 条
来源：http://xcm.yj20258888.top

按章节统计：
来源：http://mxi.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://frg.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kde.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vnr.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vty.zhoulong.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mhb.zhaomingkeji.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gpy.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://caw.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ywf.hywenlv.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jha.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zrx.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gxj.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cyq.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rjc.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kmq.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hqk.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fcn.chenlongwang.top

Q SQL 专题                              90
来源：http://orv.shangyingyoupin.top

R Bash 专题                             80
来源：http://eva.gotoacloud.top

S C / C++ 专题                          60
来源：http://oza.tianlin.xyz

T 其他语言补充                          60
来源：http://zxo.daxiang520.top

U 高频实用片段                         120
来源：http://ody.jqgufenzy.top

------------------------------------
来源：http://fnz.snrcjt.cn

合计                                  2106 条
来源：http://kvd.tarul.cn

--------------------------------------------------------------------------------
来源：http://zbb.gogol.net.cn

使用提醒
来源：http://fmi.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://hso.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jyv.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lkh.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lrj.dianchejie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kjg.svipenyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ztv.zhiwuduotai.top

—— 文件结束 ——
来源：http://cdc.vqdsnc.cn

================================================================================
来源：http://oqs.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://iht.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://vgp.sweek.top

================================================================================
来源：http://kzv.jqgufenzy.top

【收录内容】
来源：http://sef.nanxinkj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tpb.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jqx.jinqigfzy.top

SQL · Bash · C · C++
来源：http://lot.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nzw.yonumen.top

【使用说明】
来源：http://hsi.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://keu.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dja.fehbvm.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pvz.xuanzx.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qrj.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://hbg.cheryme.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://guq.sxryk.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oek.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rlj.jqgfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fsb.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yjt.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mst.jyoumei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jcg.aibaodan.cn

【文件统计】
来源：http://ocg.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qxo.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://yyx.xylfe.cn

目  录
来源：http://uvp.sweek.top

--------------------------------------------------------------------------------
来源：http://gxa.ywan-chungtsiang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fbz.sysykeji.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://exo.jqgfzy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aou.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cvc.yj20258888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://szh.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://scn.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lcl.jianghu66.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lgz.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pke.kuanghao11.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://skz.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hxg.52xcode.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wyu.316326.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://urx.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mgv.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fsr.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xzj.xziqi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tek.zhengqikj.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://xsm.redwolf501.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://miu.guowangkeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ytz.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xis.smart0.xyz

================================================================================
来源：http://gpu.52xcode.cn

A. 基础语法与类型
来源：http://kxw.haohaochexian.top

================================================================================
来源：http://sgq.kuanghao11.cn

[A01] Hello World
来源：http://ela.haohaochexian.top

Py:   print("Hello, World!")
来源：http://cff.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://vqs.daria6918.cn

JS:   console.log("Hello, World!");
来源：http://thl.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://etq.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://rvb.sjlbkw.cn

Go:   fmt.Println("Hello, World!")
来源：http://vnq.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://xve.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vqy.iojbl.cn

[A02] 变量声明与赋值
来源：http://qiv.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kjz.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ekn.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://ewj.zhiwuduotai.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jrb.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ikj.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://yen.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://ctu.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://lfx.shanyushiyangkeji.top

[A03] 常量定义
来源：http://lef.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kne.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://vcb.hysaishi.cn

JS:   const PI = 3.14159;
来源：http://nmk.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://rhd.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://wyv.yj202588.top

Go:   const PI = 3.14159
来源：http://xgn.tanke756.top

Ruby: PI = 3.14159
来源：http://lfy.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://zdb.shanyushiyangkeji.top

[A04] 判断变量类型
来源：http://eht.wangdashe.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cum.zhaomingkeji.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ydg.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ezf.9152youxi.cn

TS:   typeof x; x instanceof Date
来源：http://wpx.jyoumei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rte.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://bgl.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://ali.guowangkeji.top

C#:   x.GetType().Name; x is int
来源：http://cji.hnqzz.top

[A05] 整数除法与取模
来源：http://lbx.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://elu.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://tjb.jqgufenzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hez.andypj.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://shj.guowangkeji.top

Java: 7 / 2; 7 % 2
来源：http://tks.cdnleiting.top

Go:   7 / 2; 7 % 2
来源：http://whd.jyoumei.cn

Ruby: 7 / 2; 7 % 2
来源：http://psb.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://rnq.iojbl.cn

[A06] 字符串转数字
来源：http://eir.ydzc1.top

Py:   int("42"); float("3.14")
来源：http://vku.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kor.yfazqb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vgq.yj202588.top


<!-- 参考信息 -->