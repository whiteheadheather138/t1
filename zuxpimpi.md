代发 wailian999

[U35] Py：发送邮件
来源：http://siz.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rxk.zhengqikj.top

[U36] Py：定时任务
来源：http://khl.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://osn.yonumen.top

[U37] Py：读写 Excel
来源：http://wit.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://iio.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://hog.9152youxi.cn

Path(__file__).resolve().parent
来源：http://rvt.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://aeb.shzxlz.cn

sys.stdout.isatty()
来源：http://rwo.jiagoushi.top

[U40] Py：打印到标准错误
来源：http://hoi.nanxinkj.top

print("err", file=sys.stderr)
来源：http://pgj.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://rnj.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wbz.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://sts.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lnj.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://pzk.tian-w.cn

namespace App\Http;
来源：http://orh.bjfxy.top

[U44] PHP：开启严格类型
来源：http://jox.cashguo.top

declare(strict_types=1);
来源：http://bxz.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://vtf.zhijiandao.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xjg.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://dyl.ydjk.org.cn

?string $name = null
来源：http://rdk.jinqigfzy.top

[U47] PHP：联合类型
来源：http://rla.vehdjk.com

int|string $id
来源：http://lha.zhixingplan.top

[U48] PHP：纯枚举
来源：http://qez.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kac.zhijiandao.cn

[U49] PHP：只读属性
来源：http://fmm.pycfn.com

public readonly string $name
来源：http://pgo.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://xul.yangfankeji.com

public function __construct(private int $id) {}
来源：http://qwp.hfpthk.cn

[U51] PHP：数组解构
来源：http://qdg.ivvv.top

[$a, $b] = $arr;
来源：http://pcm.havefunace.top

[U52] PHP：箭头函数
来源：http://iej.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://nrv.yj20258888.top

[U53] PHP：空合并运算符
来源：http://tjk.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://gcn.yj202588.top

[U54] PHP：空安全调用
来源：http://uxh.vehdjk.com

$obj?->method()
来源：http://nbx.svipenyu.cn

[U55] PHP：match 表达式
来源：http://eez.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://inx.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://lje.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://nhf.nanxinkj.top

[U57] PHP：字符串插值
来源：http://blr.uphjek.com

"值: {$a}"
来源：http://wmz.yongpay.top

[U58] PHP：数组三件套
来源：http://ppa.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kmn.hywenlv.cn

[U59] PHP：自定义排序
来源：http://srt.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uax.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://xsa.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xve.yuxming.cn

[U61] PHP：正则
来源：http://cpq.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mnt.fktsv.cn

[U62] PHP：日期对象
来源：http://vho.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://acx.redwolf501.top

[U63] PHP：文件读写
来源：http://bqq.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oyq.fengsongda.top

[U64] PHP：目录遍历
来源：http://tjk.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://uvg.ehwqpu.com

[U65] PHP：会话
来源：http://amn.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lio.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://eoi.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sde.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://tqn.havefunace.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xtv.chenlongwang.top

[U68] PHP：PDO 连接
来源：http://cww.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://osp.cashguo.top

[U69] PHP：PDO 预处理
来源：http://rif.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ipm.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://neh.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://myf.hfpthk.cn

[U71] PHP：抛出异常
来源：http://awx.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://szo.ybcxt.top

[U72] PHP：写错误日志
来源：http://qep.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://fev.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://usm.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://kti.cheryme.top

[U74] PHP：读取环境变量
来源：http://ift.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://nno.gotoacloud.top

[U75] PHP：依赖注入
来源：http://fnc.shangyingyoupin.top

composer require psr/container
来源：http://eub.haohaochexian.top

[U76] PHP：简单路由
来源：http://sfw.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jxv.iojbl.cn

[U77] PHP：模板渲染
来源：http://xzf.zhongyouzk.top

composer require twig/twig
来源：http://saq.yuxming.cn

[U78] PHP：单元测试
来源：http://gwz.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://cxu.gogol.net.cn

[U79] PHP：静态分析
来源：http://lrh.shzxlz.cn

composer require --dev phpstan/phpstan
来源：http://heq.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://flv.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wni.nanxinkj.top

[U81] JS：初始化项目
来源：http://swr.ctjpmb.com

npm init -y;  npm i express
来源：http://xgw.pycfn.com

[U82] JS：package.json 脚本
来源：http://ghv.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gsp.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://yvp.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://vee.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://kty.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ljb.gaohongyu789.top

[U85] JS：可选链
来源：http://thj.yvedp.cn

a?.b?.c
来源：http://kqb.hnqzz.top

[U86] JS：空值合并
来源：http://xtn.dianchejie.cn

a ?? b
来源：http://sos.hnxiangtu.top

[U87] JS：解构默认值
来源：http://qgc.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://lcy.aizwys.cn

[U88] JS：对象展开合并
来源：http://xva.smart0.xyz

{ ...a, ...b }
来源：http://hgv.uphjek.com

[U89] JS：数组去重
来源：http://smo.smart0.xyz

[...new Set(arr)]
来源：http://mgd.guannengcc.top

[U90] JS：数字数组排序
来源：http://zgk.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://qdx.andypj.xyz

[U91] JS：对象键值遍历
来源：http://sfz.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jmw.sxryk.cn

[U92] JS：深拷贝
来源：http://nvx.sjlbkw.cn

structuredClone(obj)
来源：http://aou.zycfv.cn

[U93] JS：模板字符串
来源：http://xwx.tian-w.cn

`共 ${n} 条`
来源：http://qln.dashuyun.cn

[U94] JS：箭头函数
来源：http://zei.gogol.net.cn

const double = x => x * 2;
来源：http://pvs.ivvv.top

[U95] JS：Promise 包装
来源：http://cks.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://mqb.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://uug.zdbjq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zfr.sufxvd.cn

[U97] JS：并发请求
来源：http://dfa.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kvs.hywenlv.cn

[U98] JS：fetch 带 JSON
来源：http://acq.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vng.shuidangran.top

[U99] JS：事件监听
来源：http://wrz.cucudq.cn

el.addEventListener("click", e => {})
来源：http://kpe.shzxlz.cn

[U100] JS：DOM 查询
来源：http://svt.jinghuilouyu.cn

document.querySelector(".item")
来源：http://zzo.yuxming.cn

[U101] JS：classList 操作
来源：http://flj.dashuyun.cn

el.classList.toggle("active")
来源：http://rpi.yanxiufei.cn

[U102] JS：本地存储
来源：http://ykd.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sax.ydjk.org.cn

[U103] JS：定时器
来源：http://kcz.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tly.yongpay.top

[U104] JS：防抖
来源：http://ggt.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpm.wangdashe.top

[U105] JS：节流
来源：http://odo.xylfe.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vnu.cqqwz.cn

[U106] JS：日期格式化
来源：http://xev.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qfi.quarkkingdee.top

[U107] JS：数字千分位
来源：http://qyq.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://now.ybcxt.top

[U108] JS：随机整数
来源：http://ess.zhongyouzk.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cqw.mhx1999.top

[U109] JS：数组分组
来源：http://ary.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://xlh.quarkkingdee.top

[U110] JS：数组分块
来源：http://nao.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cqf.iojbl.cn

[U111] JS：对象转 Map
来源：http://rxg.yj20258888.top

new Map(Object.entries(obj))
来源：http://ktj.mhx1999.top

[U112] JS：字符串补位
来源：http://bck.shanyushiyangkeji.top

"7".padStart(3, "0")
来源：http://kmj.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://gxz.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://jyn.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://vxb.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vcp.havefunace.top

[U115] JS：生成 UUID
来源：http://ngo.smart0.xyz

crypto.randomUUID()
来源：http://lvz.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://wgh.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://dtw.vqdsnc.cn

[U117] JS：单元测试
来源：http://sfu.yuanzhike.top

npm i -D vitest;  npx vitest
来源：http://vsi.uphjek.com

[U118] JS：开发服务器
来源：http://chp.ydzc1.top

npm i -D vite;  npx vite
来源：http://nap.zhijiandao.cn

[U119] JS：生产构建
来源：http://vmj.9152youxi.cn

npx vite build
来源：http://xvv.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://klj.xuetiantiany.cn

import.meta.env.VITE_API_URL
来源：http://fcr.mhx1999.top

================================================================================
来源：http://dgx.guannengcc.top

统计汇总
来源：http://vhr.xuetiantiany.cn

================================================================================
来源：http://ori.jinqigufen.top

按语言统计（条）：
来源：http://kqz.iojbl.cn

Python ......... 252
来源：http://aee.zdqjudy.top

PHP ............ 252
来源：http://hbb.mhx1999.top

JavaScript ..... 252
来源：http://jmz.tianlin.xyz

TypeScript ..... 212
来源：http://hjn.bbcook.cn

Java ........... 212
来源：http://sgv.jinghuilouyu.cn

Go ............. 212
来源：http://dam.xuetiantiany.cn

Ruby ........... 212
来源：http://fsc.jinghuilouyu.cn

C# ............. 212
来源：http://odo.redwolf501.top

C .............. 30
来源：http://slb.shangyingyoupin.top

C++ ............ 30
来源：http://yfu.jinqigufen.top

SQL ............ 90
来源：http://fxt.pycfn.com

Bash ........... 80
来源：http://aex.jinghuilouyu.cn

Kotlin ......... 15
来源：http://ueb.kuanghao11.cn

Swift .......... 15
来源：http://dai.sweek.top

Lua ............ 10
来源：http://ypy.yueranfly.top

Perl ........... 10
来源：http://ghb.xuetiantiany.cn

Scala .......... 10
来源：http://zyp.9152youxi.cn

------------------------------------
来源：http://spb.fengsongda.top

合计 ........... 2106 条
来源：http://rmf.gzhubu.top

按章节统计：
来源：http://cox.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://znc.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qgl.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://alh.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://and.hysaishi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kkp.aizwys.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qap.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fuo.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://imj.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://krf.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oum.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fws.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fte.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uof.fehbvm.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dgq.hongshengwenyu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://trn.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ekm.hongshengwenyu.top

Q SQL 专题                              90
来源：http://ltp.c1oappe.top

R Bash 专题                             80
来源：http://udo.quarkkingdee.top

S C / C++ 专题                          60
来源：http://wyw.0kj1m.cn

T 其他语言补充                          60
来源：http://nqy.cheryme.top

U 高频实用片段                         120
来源：http://aik.zhijiandao.cn

------------------------------------
来源：http://kar.ivvv.top

合计                                  2106 条
来源：http://afs.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://vrn.jqgfzy.top

使用提醒
来源：http://pie.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://gjc.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hqs.zhongyouzk.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ihe.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qqd.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tmx.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hpy.fengsongda.top

—— 文件结束 ——
来源：http://bxo.ydzc1.top

================================================================================
来源：http://huo.ppjwa.cn

程序语言常见例子速查手册（2024 版）
来源：http://xle.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://aov.shuidangran.top

================================================================================
来源：http://gdr.tianlin.xyz

【收录内容】
来源：http://okg.hongshengwenyu.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://vvh.yangfankeji.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://asj.chenlongwang.top

SQL · Bash · C · C++
来源：http://edh.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sbg.shanyushiyangkeji.top

【使用说明】
来源：http://xkj.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pnc.redwolf501.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://efb.zhixingplan.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ikq.hysaishi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mtu.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rjz.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jno.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tey.xinyue.icu

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wvj.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qfp.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wfc.gogol.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vfk.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xve.jqgufenzy.top

【文件统计】
来源：http://sdb.tarul.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://dcc.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://kfn.zhixingplan.top

目  录
来源：http://cny.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://ycm.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hih.zycfv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ztg.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rbq.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dkw.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sjs.ctjpmb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xjx.yfazqb.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jub.vehdjk.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jdr.hammf.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lyz.chenlongwang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jnv.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wdv.ehwqpu.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://spc.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://net.aibaodan.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yot.yueranfly.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ymw.dashuyun.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fua.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://obq.zdbjq.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jmc.yanxiufei.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qkd.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gsw.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lvn.ydzc1.top

================================================================================
来源：http://tfs.jinqigufen.top

A. 基础语法与类型
来源：http://uoz.daria6918.cn

================================================================================
来源：http://ils.ydjk.org.cn

[A01] Hello World
来源：http://oeh.shzxlz.cn

Py:   print("Hello, World!")
来源：http://bpm.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://iss.jlsjyb.cn

JS:   console.log("Hello, World!");
来源：http://agt.yongpay.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ila.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://bbl.smart0.xyz

Go:   fmt.Println("Hello, World!")
来源：http://nee.snrcjt.cn

Ruby: puts "Hello, World!"
来源：http://ezs.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bsq.guowangkeji.top

[A02] 变量声明与赋值
来源：http://ncg.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vyq.jianghu66.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dkx.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://kht.pengpengdd.cyou

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iny.52xcode.cn

Java: String name = "Alex"; int age = 20;
来源：http://owz.hammf.cn

Go:   name := "Alex"; age := 20
来源：http://nra.ydjk.org.cn

Ruby: name = "Alex"; age = 20
来源：http://cdn.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://mgy.sufxvd.cn

[A03] 常量定义
来源：http://kzy.hysaishi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://aqs.cqqwz.cn

PHP:  const PI = 3.14159;
来源：http://lkl.fanxiaobao.xyz


<!-- 参考信息 -->