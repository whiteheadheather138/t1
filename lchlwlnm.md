代发 wailian999

[U33] Py：打包发布
来源：http://qas.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://phh.xylfe.cn

[U34] Py：判断编码
来源：http://tqi.mhx1999.top

chardet.detect(raw)
来源：http://nsl.guannengcc.top

[U35] Py：发送邮件
来源：http://ifi.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://shw.dashuyun.cn

[U36] Py：定时任务
来源：http://mnj.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://djh.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://mgz.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://nci.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://rti.9152youxi.cn

Path(__file__).resolve().parent
来源：http://viu.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://oup.hnxiangtu.top

sys.stdout.isatty()
来源：http://ebm.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://lhx.yuanzhike.top

print("err", file=sys.stderr)
来源：http://djx.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://bqn.jinqigufen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ier.yj20258888.top

[U42] PHP：PSR-4 自动加载
来源：http://ixl.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ebq.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://fvc.wangshuangyany.cn

namespace App\Http;
来源：http://vvw.cucudq.cn

[U44] PHP：开启严格类型
来源：http://jyb.yonumen.top

declare(strict_types=1);
来源：http://hje.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://bki.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://pqg.gaohongyu789.top

[U46] PHP：可空类型
来源：http://oeg.hesvh.cn

?string $name = null
来源：http://tbp.chenzaomai.com

[U47] PHP：联合类型
来源：http://egd.havefunace.top

int|string $id
来源：http://bkj.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://hrz.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mqq.tian-w.cn

[U49] PHP：只读属性
来源：http://rsl.yonumen.top

public readonly string $name
来源：http://clv.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://fil.gotoacloud.top

public function __construct(private int $id) {}
来源：http://tuu.shuidangran.top

[U51] PHP：数组解构
来源：http://dxt.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://woo.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://nte.fzhhl.top

$double = fn($x) => $x * 2;
来源：http://xzn.daxiang520.top

[U53] PHP：空合并运算符
来源：http://skp.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://nae.hammf.cn

[U54] PHP：空安全调用
来源：http://wxo.shuidangran.top

$obj?->method()
来源：http://vtz.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://ipc.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://okl.hywenlv.cn

[U56] PHP：命名参数
来源：http://npx.52xcode.cn

f(a: 1, b: 2)
来源：http://btv.smart0.xyz

[U57] PHP：字符串插值
来源：http://zec.jiagoushi.top

"值: {$a}"
来源：http://gcc.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://dxb.sjlbkw.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cfo.zdbjq.cn

[U59] PHP：自定义排序
来源：http://wdm.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bsq.uphjek.com

[U60] PHP：JSON 编解码
来源：http://rzm.iojbl.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://okj.aibaodan.cn

[U61] PHP：正则
来源：http://qmz.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jxi.chenlongwang.top

[U62] PHP：日期对象
来源：http://qfd.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bpm.cashguo.top

[U63] PHP：文件读写
来源：http://uln.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vwj.mhx1999.top

[U64] PHP：目录遍历
来源：http://miw.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://kzl.sufxvd.cn

[U65] PHP：会话
来源：http://scj.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rux.ivvv.top

[U66] PHP：设置 Cookie
来源：http://zpm.kuanghao11.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wbj.uphjek.com

[U67] PHP：处理文件上传
来源：http://nna.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xyj.gzhubu.top

[U68] PHP：PDO 连接
来源：http://gya.ctjpmb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://roy.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://eho.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bft.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://tut.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oip.bjfxy.top

[U71] PHP：抛出异常
来源：http://qqe.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://jye.yj20258888.top

[U72] PHP：写错误日志
来源：http://gna.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://ydc.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://jkz.xziqi.cn

parse_ini_file("config.ini", true)
来源：http://foy.52xcode.cn

[U74] PHP：读取环境变量
来源：http://azb.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://kvx.yangfankeji.com

[U75] PHP：依赖注入
来源：http://anh.cheryme.top

composer require psr/container
来源：http://cgs.cdnleiting.top

[U76] PHP：简单路由
来源：http://qdv.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ser.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://ojs.sjlbkw.cn

composer require twig/twig
来源：http://ogl.ybcxt.top

[U78] PHP：单元测试
来源：http://qat.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://udy.redwolf501.top

[U79] PHP：静态分析
来源：http://kgn.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://jqq.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://zri.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bck.vqdsnc.cn

[U81] JS：初始化项目
来源：http://dzs.ehwqpu.com

npm init -y;  npm i express
来源：http://jmp.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://fqz.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kgy.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://oda.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://sqe.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://svf.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://qpy.redwolf501.top

[U85] JS：可选链
来源：http://rnh.yanxiufei.cn

a?.b?.c
来源：http://bsp.xylfe.cn

[U86] JS：空值合并
来源：http://qxn.guowangkeji.top

a ?? b
来源：http://dcb.bjfxy.top

[U87] JS：解构默认值
来源：http://xmx.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://sgc.zhaomingkeji.xyz

[U88] JS：对象展开合并
来源：http://cmw.fengsongda.top

{ ...a, ...b }
来源：http://jqr.daxiang520.top

[U89] JS：数组去重
来源：http://jih.gaohongyu789.top

[...new Set(arr)]
来源：http://lpm.9152youxi.cn

[U90] JS：数字数组排序
来源：http://bhh.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://nmi.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://uob.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ugb.ybcxt.top

[U92] JS：深拷贝
来源：http://clf.hcnkem.com

structuredClone(obj)
来源：http://iiq.tianlin.xyz

[U93] JS：模板字符串
来源：http://but.yj202588.top

`共 ${n} 条`
来源：http://sdh.hfpthk.cn

[U94] JS：箭头函数
来源：http://arf.jyoumei.cn

const double = x => x * 2;
来源：http://mcq.shuidangran.top

[U95] JS：Promise 包装
来源：http://alf.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://fuh.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://yga.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://une.bjfxy.top

[U97] JS：并发请求
来源：http://nmf.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wnm.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://xmz.pengpengdd.cyou

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eeb.uphjek.com

[U99] JS：事件监听
来源：http://vbh.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://dxc.xinyue.icu

[U100] JS：DOM 查询
来源：http://qud.zhiwuduotai.top

document.querySelector(".item")
来源：http://swg.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://wal.nanxinkj.top

el.classList.toggle("active")
来源：http://fem.316326.xyz

[U102] JS：本地存储
来源：http://tqj.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ccd.yuxming.cn

[U103] JS：定时器
来源：http://kel.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rlr.ydjk.org.cn

[U104] JS：防抖
来源：http://xlr.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kim.iojbl.cn

[U105] JS：节流
来源：http://puw.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rim.guannengcc.top

[U106] JS：日期格式化
来源：http://kze.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hfx.jinqigufen.top

[U107] JS：数字千分位
来源：http://och.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bxg.gotoacloud.top

[U108] JS：随机整数
来源：http://amc.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pap.quarkkingdee.top

[U109] JS：数组分组
来源：http://thb.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://nsc.chenzaomai.com

[U110] JS：数组分块
来源：http://hmb.shuidangran.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ivh.jinqigufen.top

[U111] JS：对象转 Map
来源：http://wba.hfpthk.cn

new Map(Object.entries(obj))
来源：http://pqj.ctjpmb.com

[U112] JS：字符串补位
来源：http://ipl.wangdashe.top

"7".padStart(3, "0")
来源：http://btx.chenzaomai.com

[U113] JS：正则替换全部
来源：http://yhy.yangfankeji.com

s.replaceAll("a", "b")
来源：http://mpv.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://iul.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://ytn.aibaodan.cn

[U115] JS：生成 UUID
来源：http://ktz.yuanzhike.top

crypto.randomUUID()
来源：http://wwv.zdbjq.cn

[U116] JS：类型检查（JSDoc）
来源：http://vrl.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://gxs.hammf.cn

[U117] JS：单元测试
来源：http://axw.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://apz.shzxlz.cn

[U118] JS：开发服务器
来源：http://jri.52xcode.cn

npm i -D vite;  npx vite
来源：http://fkd.hesvh.cn

[U119] JS：生产构建
来源：http://obr.xziqi.cn

npx vite build
来源：http://zom.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://kbd.tanke756.top

import.meta.env.VITE_API_URL
来源：http://xri.gogol.net.cn

================================================================================
来源：http://loy.hysaishi.cn

统计汇总
来源：http://kog.gaohongyu789.top

================================================================================
来源：http://glu.jinghuilouyu.cn

按语言统计（条）：
来源：http://dhc.yvedp.cn

Python ......... 252
来源：http://nuf.tanke756.top

PHP ............ 252
来源：http://lhl.xziqi.cn

JavaScript ..... 252
来源：http://vkt.hnxiangtu.top

TypeScript ..... 212
来源：http://zye.wangdashe.top

Java ........... 212
来源：http://umb.tanke756.top

Go ............. 212
来源：http://cth.shuidangran.top

Ruby ........... 212
来源：http://zle.hnqzz.top

C# ............. 212
来源：http://plf.pengpengdd.cyou

C .............. 30
来源：http://alg.0kj1m.cn

C++ ............ 30
来源：http://gdi.cashguo.top

SQL ............ 90
来源：http://kvh.sysykeji.top

Bash ........... 80
来源：http://ait.tian-w.cn

Kotlin ......... 15
来源：http://jji.fanxiaobao.xyz

Swift .......... 15
来源：http://vus.0kj1m.cn

Lua ............ 10
来源：http://gij.hysaishi.cn

Perl ........... 10
来源：http://gnq.shanyushiyangkeji.top

Scala .......... 10
来源：http://tog.yuxming.cn

------------------------------------
来源：http://lgf.cqqwz.cn

合计 ........... 2106 条
来源：http://qea.jlsjyb.cn

按章节统计：
来源：http://wqj.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ksk.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jnh.shanyushiyangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nmq.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ujg.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xcf.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qgh.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ssz.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uet.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hdf.epnwcf.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nha.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xyj.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ioj.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://obx.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pkl.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eoo.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://luu.chenzaomai.com

Q SQL 专题                              90
来源：http://lyp.zdbjq.cn

R Bash 专题                             80
来源：http://ufj.yueranfly.top

S C / C++ 专题                          60
来源：http://uxk.nwbrower.top

T 其他语言补充                          60
来源：http://kyp.yj20258888.top

U 高频实用片段                         120
来源：http://mhp.chenzaomai.com

------------------------------------
来源：http://faq.fehbvm.com

合计                                  2106 条
来源：http://khp.bbcook.cn

--------------------------------------------------------------------------------
来源：http://qmu.sxryk.cn

使用提醒
来源：http://zre.havefunace.top

--------------------------------------------------------------------------------
来源：http://uly.chenjidiqi.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jsi.guannengcc.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lpm.wangdashe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ejy.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hko.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qnb.sweek.top

—— 文件结束 ——
来源：http://jsx.zdqjudy.top

================================================================================
来源：http://lrp.mhx1999.top

程序语言常见例子速查手册（2024 版）
来源：http://yww.uphjek.com

Common Programming Examples Cheat Book
来源：http://xvl.mhx1999.top

================================================================================
来源：http://mcj.52xcode.cn

【收录内容】
来源：http://zpx.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://fci.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qhj.hnxiangtu.top

SQL · Bash · C · C++
来源：http://sqr.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ydv.jlsjyb.cn

【使用说明】
来源：http://fej.cdnleiting.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hoc.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hwm.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ujp.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ynh.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bci.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qgq.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pth.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vbp.bjfxy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qtu.yangfankeji.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nck.wangshuangyany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ues.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://swy.0kj1m.cn

【文件统计】
来源：http://pdm.fktsv.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zgm.bbcook.cn

--------------------------------------------------------------------------------
来源：http://qik.meibo888.top

目  录
来源：http://cip.tanke756.top

--------------------------------------------------------------------------------
来源：http://xvg.c1oappe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://raj.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jeq.wangshuangyany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ptx.bbcook.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wkx.9152youxi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ruw.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://exi.pengpengdd.cyou

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://was.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://afs.tarul.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jjy.xuetiantiany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mlh.jiagoushi.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hje.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qgm.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zwj.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rwg.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yhl.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lsd.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uwk.hnqzz.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fky.xziqi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jhd.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://spl.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sjy.xziqi.cn

================================================================================
来源：http://hrr.gzhubu.top

A. 基础语法与类型
来源：http://ohn.nanxinkj.top

================================================================================
来源：http://xri.nanxuanxn.top

[A01] Hello World
来源：http://qgc.yfazqb.com

Py:   print("Hello, World!")
来源：http://avj.guowangkeji.top

PHP:  echo "Hello, World!";
来源：http://dfx.smart0.xyz

JS:   console.log("Hello, World!");
来源：http://irs.jyoumei.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hik.ivvv.top

Java: System.out.println("Hello, World!");
来源：http://mee.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://zuw.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://uqj.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kid.sjlbkw.cn

[A02] 变量声明与赋值
来源：http://cki.gzhubu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://erc.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://evx.gotoacloud.top

JS:   let name = "Alex"; const age = 20;
来源：http://hjd.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pyg.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://fjo.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://gay.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://sux.pengpengdd.cyou


<!-- 参考信息 -->