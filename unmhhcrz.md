代发 wailian999

[U31] Py：单测
来源：http://zrr.ywan-chungtsiang.top

python -m pytest -q
来源：http://ljk.uphjek.com

[U32] Py：代码格式化
来源：http://swe.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://gml.bjfxy.top

[U33] Py：打包发布
来源：http://btp.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://xbk.uphjek.com

[U34] Py：判断编码
来源：http://fps.fzhhl.top

chardet.detect(raw)
来源：http://qrs.hesvh.cn

[U35] Py：发送邮件
来源：http://bvl.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ehs.chenlongwang.top

[U36] Py：定时任务
来源：http://wcf.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://lxg.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://boo.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://htv.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://kak.gogol.net.cn

Path(__file__).resolve().parent
来源：http://jhv.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://tqc.ybcxt.top

sys.stdout.isatty()
来源：http://ipp.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://gag.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://pzz.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://nlb.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yzd.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://ioq.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rok.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://cba.cqqwz.cn

namespace App\Http;
来源：http://pup.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://voy.nwbrower.top

declare(strict_types=1);
来源：http://yne.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://qkw.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://otw.guowangkeji.top

[U46] PHP：可空类型
来源：http://zsm.zhongyouzk.top

?string $name = null
来源：http://tri.yuanzhike.top

[U47] PHP：联合类型
来源：http://gmq.yuxming.cn

int|string $id
来源：http://dvp.cucudq.cn

[U48] PHP：纯枚举
来源：http://ufo.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://suy.sufxvd.cn

[U49] PHP：只读属性
来源：http://bzn.zhoulong.xyz

public readonly string $name
来源：http://zxq.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://yjv.jinqigufen.top

public function __construct(private int $id) {}
来源：http://xcc.shzxlz.cn

[U51] PHP：数组解构
来源：http://vhq.hcnkem.com

[$a, $b] = $arr;
来源：http://fex.dashuyun.cn

[U52] PHP：箭头函数
来源：http://gfi.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://lrc.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://njw.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://wjp.fengsongda.top

[U54] PHP：空安全调用
来源：http://oqf.cashguo.top

$obj?->method()
来源：http://qva.ybcxt.top

[U55] PHP：match 表达式
来源：http://xph.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gil.hammf.cn

[U56] PHP：命名参数
来源：http://eye.hammf.cn

f(a: 1, b: 2)
来源：http://qvt.shzxlz.cn

[U57] PHP：字符串插值
来源：http://dah.nanxinkj.top

"值: {$a}"
来源：http://jwp.ppjwa.cn

[U58] PHP：数组三件套
来源：http://zds.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oxl.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://rqt.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aju.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://ayp.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fxg.0kj1m.cn

[U61] PHP：正则
来源：http://uef.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iiv.hfpthk.cn

[U62] PHP：日期对象
来源：http://svn.hesvh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ugc.hysaishi.cn

[U63] PHP：文件读写
来源：http://kow.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://flv.smart0.xyz

[U64] PHP：目录遍历
来源：http://rga.dianchejie.cn

glob("dir/*.php");  scandir("dir");
来源：http://duo.jqgfzy.top

[U65] PHP：会话
来源：http://fle.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zxb.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://eat.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pmh.yuanzhike.top

[U67] PHP：处理文件上传
来源：http://izu.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mzx.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://lxp.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hev.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://lqr.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://swn.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://sfo.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ujt.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://oah.vehdjk.com

throw new RuntimeException("失败", 500);
来源：http://csl.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://wba.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://lnc.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://ufx.sweek.top

parse_ini_file("config.ini", true)
来源：http://yyt.ydzc1.top

[U74] PHP：读取环境变量
来源：http://jds.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://uir.fengsongda.top

[U75] PHP：依赖注入
来源：http://hjo.9152youxi.cn

composer require psr/container
来源：http://fai.jqgufenzy.top

[U76] PHP：简单路由
来源：http://tlj.jyoumei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vli.dianchejie.cn

[U77] PHP：模板渲染
来源：http://vta.jiagoushi.top

composer require twig/twig
来源：http://ofz.meibo888.top

[U78] PHP：单元测试
来源：http://yrd.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://qgs.yonumen.top

[U79] PHP：静态分析
来源：http://igq.jianghu66.top

composer require --dev phpstan/phpstan
来源：http://hah.birdmap.top

[U80] PHP：代码规范修复
来源：http://cjg.jqgfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pst.birdmap.top

[U81] JS：初始化项目
来源：http://qcs.kuanghao11.cn

npm init -y;  npm i express
来源：http://oct.gzhubu.top

[U82] JS：package.json 脚本
来源：http://gdv.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://isi.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://luj.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://koq.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://wap.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://bpc.feifeiyinyue.top

[U85] JS：可选链
来源：http://ipp.yueranfly.top

a?.b?.c
来源：http://nvw.yvedp.cn

[U86] JS：空值合并
来源：http://cuj.yvedp.cn

a ?? b
来源：http://nzl.bjfxy.top

[U87] JS：解构默认值
来源：http://zhs.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://yyp.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://qdj.52xcode.cn

{ ...a, ...b }
来源：http://tjg.sufxvd.cn

[U89] JS：数组去重
来源：http://qec.yj202588.top

[...new Set(arr)]
来源：http://qve.sweek.top

[U90] JS：数字数组排序
来源：http://kqs.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://mpk.ivvv.top

[U91] JS：对象键值遍历
来源：http://bms.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sgh.meibo888.top

[U92] JS：深拷贝
来源：http://mmx.hnqzz.top

structuredClone(obj)
来源：http://qoc.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://ckf.yonumen.top

`共 ${n} 条`
来源：http://hzn.yanxiufei.cn

[U94] JS：箭头函数
来源：http://naj.xingfuxueyuan.xyz

const double = x => x * 2;
来源：http://mlu.guowangkeji.top

[U95] JS：Promise 包装
来源：http://xqm.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://qyp.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://twq.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rzy.gaohongyu789.top

[U97] JS：并发请求
来源：http://dzf.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zyu.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://bey.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fng.yuanzhike.top

[U99] JS：事件监听
来源：http://yfx.yj20258888.top

el.addEventListener("click", e => {})
来源：http://xys.ybcxt.top

[U100] JS：DOM 查询
来源：http://vul.xuanzx.com

document.querySelector(".item")
来源：http://iqk.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://zwc.fzhhl.top

el.classList.toggle("active")
来源：http://oyx.jqgfzy.top

[U102] JS：本地存储
来源：http://qwx.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zsa.fzhhl.top

[U103] JS：定时器
来源：http://ewc.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hjt.guannengcc.top

[U104] JS：防抖
来源：http://sps.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tot.yangfankeji.com

[U105] JS：节流
来源：http://mzl.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gde.iojbl.cn

[U106] JS：日期格式化
来源：http://ryf.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dsd.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://bpn.dashuyun.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xdr.daxiang520.top

[U108] JS：随机整数
来源：http://yti.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lmh.wangshuangyany.cn

[U109] JS：数组分组
来源：http://zdw.shzxlz.cn

Object.groupBy(arr, x => x.type)
来源：http://wem.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://hcp.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cxh.fktsv.cn

[U111] JS：对象转 Map
来源：http://lrv.xuanzx.com

new Map(Object.entries(obj))
来源：http://qlh.jinqigufen.top

[U112] JS：字符串补位
来源：http://xng.xuanzx.com

"7".padStart(3, "0")
来源：http://wts.tanke756.top

[U113] JS：正则替换全部
来源：http://cgc.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://luq.hongshengwenyu.top

[U114] JS：JSON 深比较
来源：http://zty.gotoacloud.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://efm.zycfv.cn

[U115] JS：生成 UUID
来源：http://ric.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://qdw.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://hec.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://wvx.quarkkingdee.top

[U117] JS：单元测试
来源：http://mkg.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://cmy.gzhubu.top

[U118] JS：开发服务器
来源：http://yiq.tarul.cn

npm i -D vite;  npx vite
来源：http://oie.xuetiantiany.cn

[U119] JS：生产构建
来源：http://stt.hnxiangtu.top

npx vite build
来源：http://mbd.zhixingplan.top

[U120] JS：读取环境变量（Vite）
来源：http://pjc.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://kip.pengpengdd.cyou

================================================================================
来源：http://irg.fengsongda.top

统计汇总
来源：http://alh.xziqi.cn

================================================================================
来源：http://rre.shanyushiyangkeji.top

按语言统计（条）：
来源：http://qyl.wangdashe.top

Python ......... 252
来源：http://grh.wangdashe.top

PHP ............ 252
来源：http://zna.haohaochexian.top

JavaScript ..... 252
来源：http://hvk.hywenlv.cn

TypeScript ..... 212
来源：http://vea.yuanzhike.top

Java ........... 212
来源：http://ush.epnwcf.com

Go ............. 212
来源：http://ynx.hnqzz.top

Ruby ........... 212
来源：http://fxm.birdmap.top

C# ............. 212
来源：http://tex.wangshuangyany.cn

C .............. 30
来源：http://rnx.zhengqikj.top

C++ ............ 30
来源：http://pgt.haohaochexian.top

SQL ............ 90
来源：http://iik.xuanzx.com

Bash ........... 80
来源：http://qwa.jinghuilouyu.cn

Kotlin ......... 15
来源：http://zft.hywenlv.cn

Swift .......... 15
来源：http://msu.zhengqikj.top

Lua ............ 10
来源：http://xgc.sweek.top

Perl ........... 10
来源：http://jio.shanyushiyangtech.top

Scala .......... 10
来源：http://jgq.c1oappe.top

------------------------------------
来源：http://lpk.sufxvd.cn

合计 ........... 2106 条
来源：http://hru.bjfxy.top

按章节统计：
来源：http://krd.0kj1m.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yee.fanxiaobao.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wlc.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tjh.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://izq.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://onw.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wpi.sjlbkw.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tzl.hongshengwenyu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jvk.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pit.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lzd.xuetiantiany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wmb.jqgufenzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://emp.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nrc.zhijiandao.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vuq.hcnkem.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fez.vehdjk.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ttc.zhaomingkeji.xyz

Q SQL 专题                              90
来源：http://pna.dashuyun.cn

R Bash 专题                             80
来源：http://pcn.epnwcf.com

S C / C++ 专题                          60
来源：http://fjy.wangdashe.top

T 其他语言补充                          60
来源：http://xpq.dianchejie.cn

U 高频实用片段                         120
来源：http://lsj.jinqigfzy.top

------------------------------------
来源：http://nry.zhoulong.xyz

合计                                  2106 条
来源：http://ouf.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://tlc.shzxlz.cn

使用提醒
来源：http://hqw.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://koc.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://txf.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nth.ctjpmb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ksg.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ijg.daria6918.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rmr.gaohongyu789.top

—— 文件结束 ——
来源：http://qql.jinqigfzy.top

================================================================================
来源：http://cfb.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://xyu.ydzc1.top

Common Programming Examples Cheat Book
来源：http://onh.gzhubu.top

================================================================================
来源：http://aou.xylfe.cn

【收录内容】
来源：http://bst.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dzy.ivvv.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://spx.jlsjyb.cn

SQL · Bash · C · C++
来源：http://rwc.birdmap.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ufb.aizwys.cn

【使用说明】
来源：http://fzw.jiagoushi.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://psi.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kir.cdnleiting.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://utb.havefunace.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lzz.chenjidiqi.icu

Bash:  Shell         C:     C             C++:   C++
来源：http://exx.zycfv.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cxd.bjfxy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lvz.xylfe.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qug.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hln.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uuk.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fpw.fktsv.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://isc.iojbl.cn

【文件统计】
来源：http://qwg.xuetiantiany.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ofp.bbcook.cn

--------------------------------------------------------------------------------
来源：http://jqm.wangdashe.top

目  录
来源：http://xss.havefunace.top

--------------------------------------------------------------------------------
来源：http://lrh.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qoo.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qwn.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uuc.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pyq.meibo888.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://tbh.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wsw.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bav.xuetiantiany.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xpe.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eit.mhx1999.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aub.dianchejie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fch.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zzq.zhixingplan.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xrc.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vhl.zhijiandao.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://tno.mhx1999.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bah.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ziu.chenlongwang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://avf.hnqzz.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dac.cucudq.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cbr.tian-w.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ebe.ppjwa.cn

================================================================================
来源：http://jjy.feifeiyinyue.top

A. 基础语法与类型
来源：http://yiy.hammf.cn

================================================================================
来源：http://zjy.hysaishi.cn

[A01] Hello World
来源：http://qqo.aizwys.cn

Py:   print("Hello, World!")
来源：http://otj.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://bmn.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://udk.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jxf.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://ycn.shangyingyoupin.top

Go:   fmt.Println("Hello, World!")
来源：http://qxq.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://gcu.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zho.cheryme.top

[A02] 变量声明与赋值
来源：http://vea.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xzt.yj20258.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zku.fzhhl.top

JS:   let name = "Alex"; const age = 20;
来源：http://hgf.vehdjk.com


<!-- 参考信息 -->