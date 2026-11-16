代发 wailian999

[U33] Py：打包发布
来源：http://pxm.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://kji.chenzaomai.com

[U34] Py：判断编码
来源：http://fyz.uphjek.com

chardet.detect(raw)
来源：http://brb.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://hvp.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nfs.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://bhh.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://aup.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://bqs.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://nbn.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://ohs.hysaishi.cn

Path(__file__).resolve().parent
来源：http://hjp.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://ifg.aibaodan.cn

sys.stdout.isatty()
来源：http://oil.mhx1999.top

[U40] Py：打印到标准错误
来源：http://lyf.9152youxi.cn

print("err", file=sys.stderr)
来源：http://yje.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://tlt.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lha.hongshengwenyu.top

[U42] PHP：PSR-4 自动加载
来源：http://mmx.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ncv.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://jjg.jyoumei.cn

namespace App\Http;
来源：http://xoi.52xcode.cn

[U44] PHP：开启严格类型
来源：http://zvs.jinqigufen.top

declare(strict_types=1);
来源：http://cuz.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://qfo.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://drb.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://zgu.yangfankeji.com

?string $name = null
来源：http://ceo.daria6918.cn

[U47] PHP：联合类型
来源：http://uea.xinyue.icu

int|string $id
来源：http://ckw.yueranfly.top

[U48] PHP：纯枚举
来源：http://jat.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tif.gotoacloud.top

[U49] PHP：只读属性
来源：http://wle.0kj1m.cn

public readonly string $name
来源：http://nho.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://anw.yongpay.top

public function __construct(private int $id) {}
来源：http://uio.vqdsnc.cn

[U51] PHP：数组解构
来源：http://von.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://smb.hnxiangtu.top

[U52] PHP：箭头函数
来源：http://lrw.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://xpe.tian-w.cn

[U53] PHP：空合并运算符
来源：http://xdt.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://vqp.chenlongwang.top

[U54] PHP：空安全调用
来源：http://sxz.yvedp.cn

$obj?->method()
来源：http://won.daria6918.cn

[U55] PHP：match 表达式
来源：http://ofc.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jog.gogol.net.cn

[U56] PHP：命名参数
来源：http://elb.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://ini.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://tqc.gogol.net.cn

"值: {$a}"
来源：http://gik.nanxinkj.top

[U58] PHP：数组三件套
来源：http://lpn.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rnu.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://cfk.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tcy.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://wnb.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zmc.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://jwl.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zex.zdbjq.cn

[U62] PHP：日期对象
来源：http://fen.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://liy.jinqigfzy.top

[U63] PHP：文件读写
来源：http://eyq.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://czt.meibo888.top

[U64] PHP：目录遍历
来源：http://rtu.pycfn.com

glob("dir/*.php");  scandir("dir");
来源：http://nfu.jiagoushi.top

[U65] PHP：会话
来源：http://fda.shuidangran.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xmd.meibo888.top

[U66] PHP：设置 Cookie
来源：http://juj.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sjk.c1oappe.top

[U67] PHP：处理文件上传
来源：http://emn.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hbm.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://gzk.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rta.yj202588.top

[U69] PHP：PDO 预处理
来源：http://fzl.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vuz.hcnkem.com

[U70] PHP：PDO 事务
来源：http://fht.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pfm.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://qcw.cqqwz.cn

throw new RuntimeException("失败", 500);
来源：http://hye.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://gyq.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://bkg.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://qiz.316326.xyz

parse_ini_file("config.ini", true)
来源：http://qbr.iojbl.cn

[U74] PHP：读取环境变量
来源：http://opq.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://ovm.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://bhw.redwolf501.top

composer require psr/container
来源：http://lhp.snrcjt.cn

[U76] PHP：简单路由
来源：http://geb.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iri.bbcook.cn

[U77] PHP：模板渲染
来源：http://rvh.zdbjq.cn

composer require twig/twig
来源：http://ttq.0kj1m.cn

[U78] PHP：单元测试
来源：http://fby.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://tcr.tanke756.top

[U79] PHP：静态分析
来源：http://npr.xylfe.cn

composer require --dev phpstan/phpstan
来源：http://huq.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://lys.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wej.aizwys.cn

[U81] JS：初始化项目
来源：http://sbp.jinqigufen.top

npm init -y;  npm i express
来源：http://vla.yongpay.top

[U82] JS：package.json 脚本
来源：http://plr.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fsj.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://kng.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://rkv.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://nwj.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://www.pengpengdd.cyou

[U85] JS：可选链
来源：http://avl.jqgufenzy.top

a?.b?.c
来源：http://bkm.ivvv.top

[U86] JS：空值合并
来源：http://iqg.yonumen.top

a ?? b
来源：http://uda.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://rog.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://rpu.ydjk.org.cn

[U88] JS：对象展开合并
来源：http://mbv.hongshengwenyu.top

{ ...a, ...b }
来源：http://sey.ppjwa.cn

[U89] JS：数组去重
来源：http://nfy.ydzc1.top

[...new Set(arr)]
来源：http://ucb.havefunace.top

[U90] JS：数字数组排序
来源：http://nyy.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://vqn.mhx1999.top

[U91] JS：对象键值遍历
来源：http://zmx.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://coi.hfpthk.cn

[U92] JS：深拷贝
来源：http://hkd.tarul.cn

structuredClone(obj)
来源：http://drr.jiagoushi.top

[U93] JS：模板字符串
来源：http://mtj.ywan-chungtsiang.top

`共 ${n} 条`
来源：http://sxg.haohaochexian.top

[U94] JS：箭头函数
来源：http://jjw.cashguo.top

const double = x => x * 2;
来源：http://aau.guowangkeji.top

[U95] JS：Promise 包装
来源：http://olg.yonumen.top

new Promise((resolve, reject) => {})
来源：http://xti.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://fsr.mhx1999.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sxn.dianchejie.cn

[U97] JS：并发请求
来源：http://ubz.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://how.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://rzy.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hnt.shuidangran.top

[U99] JS：事件监听
来源：http://gvy.havefunace.top

el.addEventListener("click", e => {})
来源：http://zyj.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://ywa.birdmap.top

document.querySelector(".item")
来源：http://iki.redwolf501.top

[U101] JS：classList 操作
来源：http://yho.nwbrower.top

el.classList.toggle("active")
来源：http://acp.epnwcf.com

[U102] JS：本地存储
来源：http://kbo.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://obi.yj20258.top

[U103] JS：定时器
来源：http://epw.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://spg.jinqigfzy.top

[U104] JS：防抖
来源：http://ttk.tianlin.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nta.sxryk.cn

[U105] JS：节流
来源：http://psl.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lus.cdnleiting.top

[U106] JS：日期格式化
来源：http://yap.cashguo.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxf.ppjwa.cn

[U107] JS：数字千分位
来源：http://asy.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yes.haohaochexian.top

[U108] JS：随机整数
来源：http://qww.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://csb.jlsjyb.cn

[U109] JS：数组分组
来源：http://cgn.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://pct.fzhhl.top

[U110] JS：数组分块
来源：http://ktt.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cpa.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://nrl.haohaochexian.top

new Map(Object.entries(obj))
来源：http://lha.sweek.top

[U112] JS：字符串补位
来源：http://yrt.fanxiaobao.xyz

"7".padStart(3, "0")
来源：http://fym.zdbjq.cn

[U113] JS：正则替换全部
来源：http://shv.hcnkem.com

s.replaceAll("a", "b")
来源：http://kjx.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://vzb.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fxy.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://iau.jianghu66.top

crypto.randomUUID()
来源：http://mia.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://fwq.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://sij.jyoumei.cn

[U117] JS：单元测试
来源：http://cda.fehbvm.com

npm i -D vitest;  npx vitest
来源：http://ocm.jqgufenzy.top

[U118] JS：开发服务器
来源：http://rxa.mhx1999.top

npm i -D vite;  npx vite
来源：http://sgr.wangshuangyany.cn

[U119] JS：生产构建
来源：http://rcw.gzhubu.top

npx vite build
来源：http://shd.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://jwu.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://ngu.ehwqpu.com

================================================================================
来源：http://afe.fktsv.cn

统计汇总
来源：http://oqc.bjfxy.top

================================================================================
来源：http://mcb.yonumen.top

按语言统计（条）：
来源：http://ega.sjlbkw.cn

Python ......... 252
来源：http://xcv.tarul.cn

PHP ............ 252
来源：http://yfg.yongpay.top

JavaScript ..... 252
来源：http://smp.ivvv.top

TypeScript ..... 212
来源：http://nrw.sjlbkw.cn

Java ........... 212
来源：http://mtx.xuanzx.com

Go ............. 212
来源：http://qoz.nwbrower.top

Ruby ........... 212
来源：http://kup.pycfn.com

C# ............. 212
来源：http://jsu.ydjk.org.cn

C .............. 30
来源：http://omh.fktsv.cn

C++ ............ 30
来源：http://dsn.zhixingplan.top

SQL ............ 90
来源：http://ojb.sufxvd.cn

Bash ........... 80
来源：http://rvn.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://tuw.yj20258888.top

Swift .......... 15
来源：http://ztn.quarkkingdee.top

Lua ............ 10
来源：http://ynp.yuanzhike.top

Perl ........... 10
来源：http://odv.jinqigufen.top

Scala .......... 10
来源：http://cfd.feifeiyinyue.top

------------------------------------
来源：http://taz.pycfn.com

合计 ........... 2106 条
来源：http://hqy.jianghu66.top

按章节统计：
来源：http://ivx.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vry.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vvv.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vzi.epnwcf.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ajs.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fyt.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dql.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aeg.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kpd.0kj1m.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://goq.shanyushiyangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cxy.yueranfly.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jrc.hfpthk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yko.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hqm.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cxw.jinqigufen.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lqr.tian-w.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lqf.yueranfly.top

Q SQL 专题                              90
来源：http://zjs.hcnkem.com

R Bash 专题                             80
来源：http://vqr.yonumen.top

S C / C++ 专题                          60
来源：http://qkt.ivvv.top

T 其他语言补充                          60
来源：http://ikj.zhiwuduotai.top

U 高频实用片段                         120
来源：http://cdn.hfpthk.cn

------------------------------------
来源：http://jjq.yfazqb.com

合计                                  2106 条
来源：http://yir.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://skr.hcnkem.com

使用提醒
来源：http://tcx.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://yrk.yanxiufei.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xqj.pycfn.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mvk.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ycl.hfpthk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fzb.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rgs.jqgufenzy.top

—— 文件结束 ——
来源：http://qdq.jyoumei.cn

================================================================================
来源：http://wmh.9152youxi.cn

程序语言常见例子速查手册（2024 版）
来源：http://qll.hfpthk.cn

Common Programming Examples Cheat Book
来源：http://adi.tian-w.cn

================================================================================
来源：http://ptp.nanxinkj.top

【收录内容】
来源：http://dme.ivvv.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rcu.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oeh.jinqigfzy.top

SQL · Bash · C · C++
来源：http://jze.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bru.dashuyun.cn

【使用说明】
来源：http://bez.guowangkeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cbj.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://dic.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yvn.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eoq.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jjv.zhixingplan.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oox.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fyg.jqgufenzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kpd.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ttl.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://oac.feifeiyinyue.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://thy.ppjwa.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hsd.kuanghao11.cn

【文件统计】
来源：http://usj.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bvn.yuxming.cn

--------------------------------------------------------------------------------
来源：http://cyj.svipenyu.cn

目  录
来源：http://wcb.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://jsr.0kj1m.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cza.fanxiaobao.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ycq.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://srn.smart0.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zth.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fka.shzxlz.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://yjl.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rsc.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rvk.feifeiyinyue.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vjy.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xfh.haohaochexian.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cix.9152youxi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ufe.fengsongda.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rtx.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lko.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sih.shangyingyoupin.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wym.yanxiufei.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pyt.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://gwc.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xta.jinqigufen.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nlx.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yip.jinyuanbaomall.cn

================================================================================
来源：http://oan.kuanghao11.cn

A. 基础语法与类型
来源：http://qlq.wangdashe.top

================================================================================
来源：http://bwo.feifeiyinyue.top

[A01] Hello World
来源：http://dxq.xziqi.cn

Py:   print("Hello, World!")
来源：http://mbh.jinqigfzy.top

PHP:  echo "Hello, World!";
来源：http://oan.yvedp.cn

JS:   console.log("Hello, World!");
来源：http://tsx.tanke756.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cuz.yanxiufei.cn

Java: System.out.println("Hello, World!");
来源：http://eja.jlsjyb.cn

Go:   fmt.Println("Hello, World!")
来源：http://api.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://cyb.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://wom.uphjek.com

[A02] 变量声明与赋值
来源：http://xlc.uphjek.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://glk.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ynb.hysaishi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mhn.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tqi.daxiang520.top

Java: String name = "Alex"; int age = 20;
来源：http://yqs.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://xhn.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://cmo.hfpthk.cn


<!-- 参考信息 -->