代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://hjg.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://hrh.jinqigufen.top

[U46] PHP：可空类型
来源：http://vsx.meibo888.top

?string $name = null
来源：http://egj.zycfv.cn

[U47] PHP：联合类型
来源：http://cpa.tian-w.cn

int|string $id
来源：http://zpa.cdnleiting.top

[U48] PHP：纯枚举
来源：http://dro.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tnc.jqgufenzy.top

[U49] PHP：只读属性
来源：http://yig.epnwcf.com

public readonly string $name
来源：http://ckl.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://bwe.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://cjn.0kj1m.cn

[U51] PHP：数组解构
来源：http://yrf.mhx1999.top

[$a, $b] = $arr;
来源：http://bfy.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://cye.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://oof.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://nfy.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://bpg.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://moa.jinqigufen.top

$obj?->method()
来源：http://bhs.c1oappe.top

[U55] PHP：match 表达式
来源：http://uaa.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ckx.chenzaomai.com

[U56] PHP：命名参数
来源：http://hkk.ydzc1.top

f(a: 1, b: 2)
来源：http://sna.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://knx.jqgfzy.top

"值: {$a}"
来源：http://hct.bjfxy.top

[U58] PHP：数组三件套
来源：http://kug.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ttu.yuanzhike.top

[U59] PHP：自定义排序
来源：http://wmv.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jkq.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://yqo.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bja.quarkkingdee.top

[U61] PHP：正则
来源：http://bsc.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fmu.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://szs.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jds.gzhubu.top

[U63] PHP：文件读写
来源：http://iqm.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://asj.zdbjq.cn

[U64] PHP：目录遍历
来源：http://qej.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://klp.cucudq.cn

[U65] PHP：会话
来源：http://cxj.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bdr.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://fgi.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xbi.snrcjt.cn

[U67] PHP：处理文件上传
来源：http://kvv.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kyt.bjfxy.top

[U68] PHP：PDO 连接
来源：http://bhp.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jwu.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://fro.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vgi.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://xhr.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xbp.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://ukp.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://qvv.9152youxi.cn

[U72] PHP：写错误日志
来源：http://hrk.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://cjm.zhongyouzk.top

[U73] PHP：读取 ini 配置
来源：http://qqr.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://sas.fengsongda.top

[U74] PHP：读取环境变量
来源：http://wpn.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://nwt.316326.xyz

[U75] PHP：依赖注入
来源：http://dza.zhixingplan.top

composer require psr/container
来源：http://lky.jqgfzy.top

[U76] PHP：简单路由
来源：http://rav.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fal.sufxvd.cn

[U77] PHP：模板渲染
来源：http://wuy.dashuyun.cn

composer require twig/twig
来源：http://fip.vqdsnc.cn

[U78] PHP：单元测试
来源：http://ule.hammf.cn

composer require --dev phpunit/phpunit
来源：http://czy.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://akx.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://uvl.zhiwuduotai.top

[U80] PHP：代码规范修复
来源：http://htn.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gle.9152youxi.cn

[U81] JS：初始化项目
来源：http://slc.52xcode.cn

npm init -y;  npm i express
来源：http://uyf.yuxming.cn

[U82] JS：package.json 脚本
来源：http://zpd.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://udc.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://gvm.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://erw.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://cha.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dff.gaohongyu789.top

[U85] JS：可选链
来源：http://tmk.yuanzhike.top

a?.b?.c
来源：http://jwe.quarkkingdee.top

[U86] JS：空值合并
来源：http://fzx.gogol.net.cn

a ?? b
来源：http://jro.pycfn.com

[U87] JS：解构默认值
来源：http://cxi.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://gyy.chenlongwang.top

[U88] JS：对象展开合并
来源：http://epp.yfazqb.com

{ ...a, ...b }
来源：http://emv.jqgufenzy.top

[U89] JS：数组去重
来源：http://bvs.havefunace.top

[...new Set(arr)]
来源：http://xyu.nanxinkj.top

[U90] JS：数字数组排序
来源：http://kvq.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://dhu.daria6918.cn

[U91] JS：对象键值遍历
来源：http://tdx.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xik.chenlongwang.top

[U92] JS：深拷贝
来源：http://nst.aizwys.cn

structuredClone(obj)
来源：http://qks.chenlongwang.top

[U93] JS：模板字符串
来源：http://gex.jlsjyb.cn

`共 ${n} 条`
来源：http://arl.ydzc1.top

[U94] JS：箭头函数
来源：http://eky.316326.xyz

const double = x => x * 2;
来源：http://vav.hfpthk.cn

[U95] JS：Promise 包装
来源：http://doa.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://mbr.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://fwa.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bah.xinyue.icu

[U97] JS：并发请求
来源：http://qzf.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://inb.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://abc.birdmap.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eqm.vqdsnc.cn

[U99] JS：事件监听
来源：http://zxt.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://egw.hesvh.cn

[U100] JS：DOM 查询
来源：http://lhf.316326.xyz

document.querySelector(".item")
来源：http://ixo.jinyuanbaomall.cn

[U101] JS：classList 操作
来源：http://jzm.chenjidiqi.icu

el.classList.toggle("active")
来源：http://fva.yongpay.top

[U102] JS：本地存储
来源：http://pvy.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://rhk.wangdashe.top

[U103] JS：定时器
来源：http://ghk.mhx1999.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tph.cashguo.top

[U104] JS：防抖
来源：http://jnf.uphjek.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuh.chenzaomai.com

[U105] JS：节流
来源：http://uek.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nvk.hcnkem.com

[U106] JS：日期格式化
来源：http://gtj.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://exm.zdbjq.cn

[U107] JS：数字千分位
来源：http://kjf.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://prc.0kj1m.cn

[U108] JS：随机整数
来源：http://ihn.pycfn.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blk.bbcook.cn

[U109] JS：数组分组
来源：http://xvg.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://tom.yongpay.top

[U110] JS：数组分块
来源：http://kbg.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mdt.hnqzz.top

[U111] JS：对象转 Map
来源：http://anb.hcnkem.com

new Map(Object.entries(obj))
来源：http://qxw.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://hpy.cashguo.top

"7".padStart(3, "0")
来源：http://bin.daria6918.cn

[U113] JS：正则替换全部
来源：http://yin.xinyue.icu

s.replaceAll("a", "b")
来源：http://ynh.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://mpr.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://wip.fehbvm.com

[U115] JS：生成 UUID
来源：http://kqa.dianchejie.cn

crypto.randomUUID()
来源：http://jxq.cdnleiting.top

[U116] JS：类型检查（JSDoc）
来源：http://nqe.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://yta.yueranfly.top

[U117] JS：单元测试
来源：http://mpy.316326.xyz

npm i -D vitest;  npx vitest
来源：http://vdc.ydzc1.top

[U118] JS：开发服务器
来源：http://rsg.xziqi.cn

npm i -D vite;  npx vite
来源：http://hrw.yuxming.cn

[U119] JS：生产构建
来源：http://ofp.aibaodan.cn

npx vite build
来源：http://jwo.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://ahy.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://hmd.tanke756.top

================================================================================
来源：http://mln.jinghuilouyu.cn

统计汇总
来源：http://obx.sysykeji.top

================================================================================
来源：http://alw.yuxming.cn

按语言统计（条）：
来源：http://mam.xylfe.cn

Python ......... 252
来源：http://xji.fktsv.cn

PHP ............ 252
来源：http://zwu.daria6918.cn

JavaScript ..... 252
来源：http://iza.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://tjk.jqgfzy.top

Java ........... 212
来源：http://osn.aibaodan.cn

Go ............. 212
来源：http://fyc.xuetiantiany.cn

Ruby ........... 212
来源：http://umc.fengsongda.top

C# ............. 212
来源：http://tey.gaohongyu789.top

C .............. 30
来源：http://yhw.xylfe.cn

C++ ............ 30
来源：http://ejt.fktsv.cn

SQL ............ 90
来源：http://rpo.jinyuanbaomall.cn

Bash ........... 80
来源：http://rok.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://scc.aibaodan.cn

Swift .......... 15
来源：http://nof.daxiang520.top

Lua ............ 10
来源：http://fuz.jiagoushi.top

Perl ........... 10
来源：http://jzd.yj20258888.top

Scala .......... 10
来源：http://toq.shuidangran.top

------------------------------------
来源：http://mrr.aizwys.cn

合计 ........... 2106 条
来源：http://qaw.pengpengdd.cyou

按章节统计：
来源：http://wkv.tian-w.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tpf.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vtb.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nog.guannengcc.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrm.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yjf.zdqjudy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bgd.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://esl.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mfb.jinqigufen.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ojm.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://urr.hfpthk.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://loc.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jln.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdy.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uow.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xnq.jyoumei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mea.iojbl.cn

Q SQL 专题                              90
来源：http://owi.shangyingyoupin.top

R Bash 专题                             80
来源：http://cur.jlsjyb.cn

S C / C++ 专题                          60
来源：http://bqv.zhoulong.xyz

T 其他语言补充                          60
来源：http://egy.gzhubu.top

U 高频实用片段                         120
来源：http://czt.hongshengwenyu.top

------------------------------------
来源：http://sux.ywan-chungtsiang.top

合计                                  2106 条
来源：http://fjx.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://uar.bbcook.cn

使用提醒
来源：http://zau.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://xxa.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://guo.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cov.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uek.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://eer.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yjz.zhongyouzk.top

—— 文件结束 ——
来源：http://aho.cashguo.top

================================================================================
来源：http://cga.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://nqq.yj20258.top

Common Programming Examples Cheat Book
来源：http://cuz.zdqjudy.top

================================================================================
来源：http://sum.zhixingplan.top

【收录内容】
来源：http://gse.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ady.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yza.hysaishi.cn

SQL · Bash · C · C++
来源：http://cyx.gogol.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tpj.ywan-chungtsiang.top

【使用说明】
来源：http://tpp.dianchejie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://apd.jiagoushi.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uyo.c1oappe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pad.yuxming.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://edu.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gbv.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vno.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vww.kuanghao11.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ibu.kuanghao11.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qrb.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://irr.jianghu66.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://akb.sysykeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hdp.hongshengwenyu.top

【文件统计】
来源：http://lyw.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gdt.wangdashe.top

--------------------------------------------------------------------------------
来源：http://pqw.xingfuxueyuan.xyz

目  录
来源：http://rjz.guannengcc.top

--------------------------------------------------------------------------------
来源：http://zju.pengpengdd.cyou

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://arg.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kvc.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dzv.vehdjk.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lak.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zls.zdbjq.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lxn.mhx1999.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jsz.nanxuanxn.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://btm.shangyingyoupin.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://asr.cheryme.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mxa.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fwm.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lcs.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yuy.sysykeji.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sna.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ign.snrcjt.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://epz.haohaochexian.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mgz.yj20258.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zol.shangyingyoupin.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lvv.zhengqikj.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xoq.gogol.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sfa.ywan-chungtsiang.top

================================================================================
来源：http://gac.zhengqikj.top

A. 基础语法与类型
来源：http://woq.daxiang520.top

================================================================================
来源：http://usb.pycfn.com

[A01] Hello World
来源：http://yfs.xylfe.cn

Py:   print("Hello, World!")
来源：http://mdz.cashguo.top

PHP:  echo "Hello, World!";
来源：http://uar.0kj1m.cn

JS:   console.log("Hello, World!");
来源：http://adh.hesvh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hra.aizwys.cn

Java: System.out.println("Hello, World!");
来源：http://bax.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://yrw.svipenyu.cn

Ruby: puts "Hello, World!"
来源：http://qnz.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fou.9152youxi.cn

[A02] 变量声明与赋值
来源：http://yua.zhengqikj.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://czh.pengpengdd.cyou

PHP:  $name = "Alex"; $age = 20;
来源：http://guy.snrcjt.cn

JS:   let name = "Alex"; const age = 20;
来源：http://avi.bbcook.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ubx.zhoulong.xyz

Java: String name = "Alex"; int age = 20;
来源：http://nuq.xuanzx.com

Go:   name := "Alex"; age := 20
来源：http://aup.chenjidiqi.icu

Ruby: name = "Alex"; age = 20
来源：http://oyi.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fow.wangdashe.top

[A03] 常量定义
来源：http://taj.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bsd.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://kbk.dianchejie.cn

JS:   const PI = 3.14159;
来源：http://xxi.jqgufenzy.top

TS:   const PI: number = 3.14159;
来源：http://ybw.shanyushiyangkeji.top

Java: static final double PI = 3.14159;
来源：http://spq.guowangkeji.top

Go:   const PI = 3.14159
来源：http://ksu.sysykeji.top

Ruby: PI = 3.14159
来源：http://uvw.316326.xyz

C#:   const double PI = 3.14159;
来源：http://ygw.ybcxt.top

[A04] 判断变量类型
来源：http://fsx.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hzg.birdmap.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ize.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kal.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://iqx.zhaomingkeji.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://grn.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kbi.wangshuangyany.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gcg.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://brl.yangfankeji.com

[A05] 整数除法与取模
来源：http://rij.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nuu.fktsv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pyt.0kj1m.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://utr.zdbjq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://csz.yongpay.top


<!-- 参考信息 -->