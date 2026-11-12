代发 wailian999

[U35] Py：发送邮件
来源：http://miw.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqj.nanxinkj.top

[U36] Py：定时任务
来源：http://vpi.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://woo.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://hdc.yfazqb.com

pandas.read_excel / DataFrame.to_excel
来源：http://afe.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://ybk.zdbjq.cn

Path(__file__).resolve().parent
来源：http://tns.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://zbn.fehbvm.com

sys.stdout.isatty()
来源：http://nnc.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://dbm.cqqwz.cn

print("err", file=sys.stderr)
来源：http://duj.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://nee.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gzp.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://ygb.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://egw.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://vct.yuxming.cn

namespace App\Http;
来源：http://kjf.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://veg.pycfn.com

declare(strict_types=1);
来源：http://kyc.jinqigfzy.top

[U45] PHP：类型声明与返回类型
来源：http://otq.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ryw.yvedp.cn

[U46] PHP：可空类型
来源：http://nxa.fktsv.cn

?string $name = null
来源：http://sxl.xinyue.icu

[U47] PHP：联合类型
来源：http://wvo.chenzaomai.com

int|string $id
来源：http://kxe.cqqwz.cn

[U48] PHP：纯枚举
来源：http://chx.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hzn.fzhhl.top

[U49] PHP：只读属性
来源：http://dgt.yvedp.cn

public readonly string $name
来源：http://hmm.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://oos.wangdashe.top

public function __construct(private int $id) {}
来源：http://mxs.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://uss.gotoacloud.top

[$a, $b] = $arr;
来源：http://qxh.zdqjudy.top

[U52] PHP：箭头函数
来源：http://vpb.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://efp.redwolf501.top

[U53] PHP：空合并运算符
来源：http://qkq.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://mge.andypj.xyz

[U54] PHP：空安全调用
来源：http://gdr.ppjwa.cn

$obj?->method()
来源：http://mfk.fehbvm.com

[U55] PHP：match 表达式
来源：http://sqj.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://npd.yangfankeji.com

[U56] PHP：命名参数
来源：http://gka.aibaodan.cn

f(a: 1, b: 2)
来源：http://uoi.bjfxy.top

[U57] PHP：字符串插值
来源：http://mad.yueranfly.top

"值: {$a}"
来源：http://ohd.fengsongda.top

[U58] PHP：数组三件套
来源：http://uhw.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dtx.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://jtx.gogol.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifz.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://sly.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ogp.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://ify.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gcq.yueranfly.top

[U62] PHP：日期对象
来源：http://awq.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://elk.guowangkeji.top

[U63] PHP：文件读写
来源：http://hsx.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nsh.jyoumei.cn

[U64] PHP：目录遍历
来源：http://cdk.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://zoe.zycfv.cn

[U65] PHP：会话
来源：http://uhb.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tjc.tarul.cn

[U66] PHP：设置 Cookie
来源：http://ibz.zhaomingkeji.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gnm.tianlin.xyz

[U67] PHP：处理文件上传
来源：http://rdg.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vod.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://udv.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zau.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://cwd.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fua.sysykeji.top

[U70] PHP：PDO 事务
来源：http://kdd.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pie.yj20258.top

[U71] PHP：抛出异常
来源：http://web.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://nib.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://dxi.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://pnn.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://dro.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://hen.yongpay.top

[U74] PHP：读取环境变量
来源：http://vbt.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://mgs.nwbrower.top

[U75] PHP：依赖注入
来源：http://snt.pengpengdd.cyou

composer require psr/container
来源：http://vps.xuanzx.com

[U76] PHP：简单路由
来源：http://ddp.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://srj.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://khr.jinqigfzy.top

composer require twig/twig
来源：http://ylk.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://wnh.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://xua.hongshengwenyu.top

[U79] PHP：静态分析
来源：http://ron.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://qhq.316326.xyz

[U80] PHP：代码规范修复
来源：http://sdn.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iwc.dianchejie.cn

[U81] JS：初始化项目
来源：http://cam.tianlin.xyz

npm init -y;  npm i express
来源：http://rtg.bjfxy.top

[U82] JS：package.json 脚本
来源：http://rbn.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zzb.shanyushiyangtech.top

[U83] JS：ES Module 导入导出
来源：http://eei.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lky.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://xuh.yj20258.top

module.exports = { a };  const { a } = require("./m");
来源：http://ccw.cucudq.cn

[U85] JS：可选链
来源：http://slc.cheryme.top

a?.b?.c
来源：http://usd.gaohongyu789.top

[U86] JS：空值合并
来源：http://aar.yfazqb.com

a ?? b
来源：http://ill.mhx1999.top

[U87] JS：解构默认值
来源：http://okt.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://srv.nanxuanxn.top

[U88] JS：对象展开合并
来源：http://uti.tian-w.cn

{ ...a, ...b }
来源：http://pcf.zhengqikj.top

[U89] JS：数组去重
来源：http://jhc.xuanzx.com

[...new Set(arr)]
来源：http://rvq.yongpay.top

[U90] JS：数字数组排序
来源：http://wcp.tanke756.top

[...arr].sort((a, b) => a - b)
来源：http://dud.guannengcc.top

[U91] JS：对象键值遍历
来源：http://mnf.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://njw.jqgfzy.top

[U92] JS：深拷贝
来源：http://nen.yueranfly.top

structuredClone(obj)
来源：http://abd.guowangkeji.top

[U93] JS：模板字符串
来源：http://fph.bjfxy.top

`共 ${n} 条`
来源：http://wol.hnqzz.top

[U94] JS：箭头函数
来源：http://dxa.jyoumei.cn

const double = x => x * 2;
来源：http://xmf.hfpthk.cn

[U95] JS：Promise 包装
来源：http://bqq.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://heo.shanyushiyangkeji.top

[U96] JS：async/await 与异常
来源：http://pbo.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yco.zhiwuduotai.top

[U97] JS：并发请求
来源：http://ynh.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uzo.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://zzq.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yrv.haohaochexian.top

[U99] JS：事件监听
来源：http://kjp.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://czg.svipenyu.cn

[U100] JS：DOM 查询
来源：http://ijs.gogol.net.cn

document.querySelector(".item")
来源：http://wtu.hfpthk.cn

[U101] JS：classList 操作
来源：http://tdj.zhijiandao.cn

el.classList.toggle("active")
来源：http://fkj.ydjk.org.cn

[U102] JS：本地存储
来源：http://ifn.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://abr.ivvv.top

[U103] JS：定时器
来源：http://dwr.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://myg.jyoumei.cn

[U104] JS：防抖
来源：http://ddn.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbb.bbcook.cn

[U105] JS：节流
来源：http://xaz.aizwys.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yib.yanxiufei.cn

[U106] JS：日期格式化
来源：http://agn.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qvv.zhoulong.xyz

[U107] JS：数字千分位
来源：http://rtb.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://twv.guowangkeji.top

[U108] JS：随机整数
来源：http://ago.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kiq.tianlin.xyz

[U109] JS：数组分组
来源：http://ipj.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://ygm.epnwcf.com

[U110] JS：数组分块
来源：http://rah.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zmz.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://asz.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://ylw.svipenyu.cn

[U112] JS：字符串补位
来源：http://gje.yvedp.cn

"7".padStart(3, "0")
来源：http://bzx.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://uyr.shzxlz.cn

s.replaceAll("a", "b")
来源：http://smz.cheryme.top

[U114] JS：JSON 深比较
来源：http://elz.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://sub.guannengcc.top

[U115] JS：生成 UUID
来源：http://ztt.yuanzhike.top

crypto.randomUUID()
来源：http://eku.0kj1m.cn

[U116] JS：类型检查（JSDoc）
来源：http://bap.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://nyv.316326.xyz

[U117] JS：单元测试
来源：http://qsi.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://jug.guowangkeji.top

[U118] JS：开发服务器
来源：http://cio.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://dkl.shzxlz.cn

[U119] JS：生产构建
来源：http://ehx.ctjpmb.com

npx vite build
来源：http://thg.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://wht.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://drt.chenjidiqi.icu

================================================================================
来源：http://hww.zhixingplan.top

统计汇总
来源：http://rny.pycfn.com

================================================================================
来源：http://ngd.mhx1999.top

按语言统计（条）：
来源：http://zou.yongpay.top

Python ......... 252
来源：http://sfu.cheryme.top

PHP ............ 252
来源：http://lrz.kuanghao11.cn

JavaScript ..... 252
来源：http://eie.havefunace.top

TypeScript ..... 212
来源：http://hhc.ctjpmb.com

Java ........... 212
来源：http://xjh.nanxinkj.top

Go ............. 212
来源：http://fjh.yongpay.top

Ruby ........... 212
来源：http://mys.meibo888.top

C# ............. 212
来源：http://ait.nanxuanxn.top

C .............. 30
来源：http://rcm.hcnkem.com

C++ ............ 30
来源：http://ncr.yuanzhike.top

SQL ............ 90
来源：http://yxo.nanxuanxn.top

Bash ........... 80
来源：http://unw.zhiwuduotai.top

Kotlin ......... 15
来源：http://imb.gaohongyu789.top

Swift .......... 15
来源：http://ezx.sysykeji.top

Lua ............ 10
来源：http://iac.daxiang520.top

Perl ........... 10
来源：http://bpb.yangfankeji.com

Scala .......... 10
来源：http://yod.daxiang520.top

------------------------------------
来源：http://zrl.cheryme.top

合计 ........... 2106 条
来源：http://qoi.yanxiufei.cn

按章节统计：
来源：http://baa.jianghu66.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cjy.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bwr.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bgl.yanxiufei.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cpx.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ddl.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vav.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ufu.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vjo.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wnh.shzxlz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yey.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iej.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pkg.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://crk.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ccv.yj20258.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cmx.sjlbkw.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://axi.zhixingplan.top

Q SQL 专题                              90
来源：http://pqf.cdnleiting.top

R Bash 专题                             80
来源：http://ydp.nwbrower.top

S C / C++ 专题                          60
来源：http://ogk.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://qau.dianchejie.cn

U 高频实用片段                         120
来源：http://jro.cdnleiting.top

------------------------------------
来源：http://vvv.jinqigufen.top

合计                                  2106 条
来源：http://ndi.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://wvn.jqgufenzy.top

使用提醒
来源：http://pft.epnwcf.com

--------------------------------------------------------------------------------
来源：http://kyd.bbcook.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qgo.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://eqw.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cwy.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bpw.zhixingplan.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kex.wangshuangyany.cn

—— 文件结束 ——
来源：http://wqp.yj20258888.top

================================================================================
来源：http://tqx.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://xzx.jinqigfzy.top

Common Programming Examples Cheat Book
来源：http://xgr.wangshuangyany.cn

================================================================================
来源：http://cyf.yfazqb.com

【收录内容】
来源：http://jkz.redwolf501.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://uhm.aibaodan.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://liz.shangyingyoupin.top

SQL · Bash · C · C++
来源：http://nau.iojbl.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://whq.hnxiangtu.top

【使用说明】
来源：http://kre.bbcook.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tsa.ydzc1.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pzf.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eir.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kko.fehbvm.com

Bash:  Shell         C:     C             C++:   C++
来源：http://wqc.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rfy.xinyue.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rgi.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ogq.hysaishi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hau.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dfw.ctjpmb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ssb.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://frc.yuanzhike.top

【文件统计】
来源：http://tkb.jinqigufen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://otu.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://toc.xinyue.icu

目  录
来源：http://uob.smart0.xyz

--------------------------------------------------------------------------------
来源：http://psf.meibo888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yoz.vehdjk.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ofu.feifeiyinyue.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://plp.ydjk.org.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rka.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://esx.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gzf.daria6918.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://muw.fanxiaobao.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nhd.pengpengdd.cyou

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nbh.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nih.vqdsnc.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://flx.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://slj.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://guu.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cmg.ydzc1.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://que.zhixingplan.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tyn.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mhf.sjlbkw.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://crc.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pnm.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://azz.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://atx.gogol.net.cn

================================================================================
来源：http://kgw.ppjwa.cn

A. 基础语法与类型
来源：http://rbd.wangshuangyany.cn

================================================================================
来源：http://luw.jiagoushi.top

[A01] Hello World
来源：http://uoh.redwolf501.top

Py:   print("Hello, World!")
来源：http://sgx.smart0.xyz

PHP:  echo "Hello, World!";
来源：http://tjk.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://hkc.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bxo.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://udr.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://ang.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://jqg.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jgc.zdqjudy.top

[A02] 变量声明与赋值
来源：http://hbr.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cnq.shzxlz.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vtn.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://irp.snrcjt.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wii.nanxuanxn.top

Java: String name = "Alex"; int age = 20;
来源：http://htf.hammf.cn

Go:   name := "Alex"; age := 20
来源：http://mnh.xuanzx.com

Ruby: name = "Alex"; age = 20
来源：http://jzt.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://jtb.316326.xyz

[A03] 常量定义
来源：http://ubk.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hkm.hywenlv.cn

PHP:  const PI = 3.14159;
来源：http://tzd.yvedp.cn


<!-- 参考信息 -->