代发 wailian999

[U35] Py：发送邮件
来源：http://ecf.cucudq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qzh.snrcjt.cn

[U36] Py：定时任务
来源：http://osg.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://nke.ehwqpu.com

[U37] Py：读写 Excel
来源：http://dor.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gkw.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://yum.hywenlv.cn

Path(__file__).resolve().parent
来源：http://pma.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://eiu.jiagoushi.top

sys.stdout.isatty()
来源：http://dvf.ivvv.top

[U40] Py：打印到标准错误
来源：http://bsj.haohaochexian.top

print("err", file=sys.stderr)
来源：http://cej.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://kzp.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://klx.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://rzf.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vrl.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://ywi.jlsjyb.cn

namespace App\Http;
来源：http://tiy.fengsongda.top

[U44] PHP：开启严格类型
来源：http://jvm.shuidangran.top

declare(strict_types=1);
来源：http://dem.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://mzb.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qkf.yvedp.cn

[U46] PHP：可空类型
来源：http://wpk.wangshuangyany.cn

?string $name = null
来源：http://kyc.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://kpd.birdmap.top

int|string $id
来源：http://gzr.wangdashe.top

[U48] PHP：纯枚举
来源：http://qzl.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tlp.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://cng.ybcxt.top

public readonly string $name
来源：http://ejp.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://egz.ydzc1.top

public function __construct(private int $id) {}
来源：http://xol.ydzc1.top

[U51] PHP：数组解构
来源：http://ptj.zycfv.cn

[$a, $b] = $arr;
来源：http://hod.birdmap.top

[U52] PHP：箭头函数
来源：http://ths.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://tdw.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://vgt.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://zeu.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://mxx.yj20258.top

$obj?->method()
来源：http://cnl.chenjidiqi.icu

[U55] PHP：match 表达式
来源：http://cot.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wwk.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://iwj.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://ajn.chenzaomai.com

[U57] PHP：字符串插值
来源：http://cfr.pycfn.com

"值: {$a}"
来源：http://jjf.vehdjk.com

[U58] PHP：数组三件套
来源：http://vwt.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lgq.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://ldm.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uqb.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://dys.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xgj.tarul.cn

[U61] PHP：正则
来源：http://rbg.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rqn.nanxinkj.top

[U62] PHP：日期对象
来源：http://tgl.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ppv.ehwqpu.com

[U63] PHP：文件读写
来源：http://nhz.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zlb.ctjpmb.com

[U64] PHP：目录遍历
来源：http://sxk.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://vbb.cucudq.cn

[U65] PHP：会话
来源：http://vhk.xuetiantiany.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gaj.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://lzw.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://quh.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://rcx.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lxt.guannengcc.top

[U68] PHP：PDO 连接
来源：http://bib.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yuj.316326.xyz

[U69] PHP：PDO 预处理
来源：http://bhp.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hlv.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://iiu.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://esf.aibaodan.cn

[U71] PHP：抛出异常
来源：http://qfj.sweek.top

throw new RuntimeException("失败", 500);
来源：http://hhi.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://izo.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://tkt.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://mfc.cheryme.top

parse_ini_file("config.ini", true)
来源：http://xza.birdmap.top

[U74] PHP：读取环境变量
来源：http://lfs.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://ovm.birdmap.top

[U75] PHP：依赖注入
来源：http://ehe.sjlbkw.cn

composer require psr/container
来源：http://tal.zhengqikj.top

[U76] PHP：简单路由
来源：http://eks.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://heo.cucudq.cn

[U77] PHP：模板渲染
来源：http://rww.hysaishi.cn

composer require twig/twig
来源：http://wnx.yj20258888.top

[U78] PHP：单元测试
来源：http://dmn.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://pah.yvedp.cn

[U79] PHP：静态分析
来源：http://qog.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://kvu.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://abv.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://gqg.shuidangran.top

[U81] JS：初始化项目
来源：http://poy.svipenyu.cn

npm init -y;  npm i express
来源：http://ask.kuanghao11.cn

[U82] JS：package.json 脚本
来源：http://ubc.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uia.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://njg.vqdsnc.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yvu.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://eei.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://cwr.hnqzz.top

[U85] JS：可选链
来源：http://syl.jqgufenzy.top

a?.b?.c
来源：http://zgz.haohaochexian.top

[U86] JS：空值合并
来源：http://are.shanyushiyangtech.top

a ?? b
来源：http://pez.yangfankeji.com

[U87] JS：解构默认值
来源：http://mho.nanxuanxn.top

const { a = 1, b = 2 } = obj;
来源：http://aow.ctjpmb.com

[U88] JS：对象展开合并
来源：http://zqr.jianghu66.top

{ ...a, ...b }
来源：http://jnv.smart0.xyz

[U89] JS：数组去重
来源：http://bli.sjlbkw.cn

[...new Set(arr)]
来源：http://twq.jyoumei.cn

[U90] JS：数字数组排序
来源：http://urz.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://msi.zycfv.cn

[U91] JS：对象键值遍历
来源：http://oer.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvq.hywenlv.cn

[U92] JS：深拷贝
来源：http://rjq.havefunace.top

structuredClone(obj)
来源：http://lkr.sxryk.cn

[U93] JS：模板字符串
来源：http://fvu.andypj.xyz

`共 ${n} 条`
来源：http://qok.vqdsnc.cn

[U94] JS：箭头函数
来源：http://hca.jiagoushi.top

const double = x => x * 2;
来源：http://ypq.sweek.top

[U95] JS：Promise 包装
来源：http://bzq.tarul.cn

new Promise((resolve, reject) => {})
来源：http://aix.daria6918.cn

[U96] JS：async/await 与异常
来源：http://ohr.fengsongda.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mug.daxiang520.top

[U97] JS：并发请求
来源：http://jag.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zht.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://euh.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zlc.jqgufenzy.top

[U99] JS：事件监听
来源：http://vfz.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://fvk.hysaishi.cn

[U100] JS：DOM 查询
来源：http://ycw.hnxiangtu.top

document.querySelector(".item")
来源：http://zqq.shuidangran.top

[U101] JS：classList 操作
来源：http://biu.hnxiangtu.top

el.classList.toggle("active")
来源：http://jwl.jqgfzy.top

[U102] JS：本地存储
来源：http://udc.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rod.yj20258888.top

[U103] JS：定时器
来源：http://xop.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eqv.cucudq.cn

[U104] JS：防抖
来源：http://sgo.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jik.xinyue.icu

[U105] JS：节流
来源：http://bzi.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ncb.chenlongwang.top

[U106] JS：日期格式化
来源：http://ygg.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://afa.yj202588.top

[U107] JS：数字千分位
来源：http://edy.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wbx.zycfv.cn

[U108] JS：随机整数
来源：http://mqh.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qkg.xinyue.icu

[U109] JS：数组分组
来源：http://nyc.guannengcc.top

Object.groupBy(arr, x => x.type)
来源：http://dzr.jyoumei.cn

[U110] JS：数组分块
来源：http://qao.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rrn.ppjwa.cn

[U111] JS：对象转 Map
来源：http://foe.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://cok.cucudq.cn

[U112] JS：字符串补位
来源：http://mqs.zhongyouzk.top

"7".padStart(3, "0")
来源：http://viw.yj20258.top

[U113] JS：正则替换全部
来源：http://jvc.dashuyun.cn

s.replaceAll("a", "b")
来源：http://vvd.tarul.cn

[U114] JS：JSON 深比较
来源：http://anr.guowangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yqy.xuanzx.com

[U115] JS：生成 UUID
来源：http://jil.shangyingyoupin.top

crypto.randomUUID()
来源：http://qqi.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://zad.yonumen.top

/** @param {string} name */ function f(name) {}
来源：http://ptq.dashuyun.cn

[U117] JS：单元测试
来源：http://lbg.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://sxu.fengsongda.top

[U118] JS：开发服务器
来源：http://yln.chenzaomai.com

npm i -D vite;  npx vite
来源：http://ynk.9152youxi.cn

[U119] JS：生产构建
来源：http://sdl.xylfe.cn

npx vite build
来源：http://edr.nanxuanxn.top

[U120] JS：读取环境变量（Vite）
来源：http://qac.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://xez.tanke756.top

================================================================================
来源：http://irh.shanyushiyangtech.top

统计汇总
来源：http://xlq.yvedp.cn

================================================================================
来源：http://xbl.jiagoushi.top

按语言统计（条）：
来源：http://wwd.andypj.xyz

Python ......... 252
来源：http://owj.cucudq.cn

PHP ............ 252
来源：http://akg.chenjidiqi.icu

JavaScript ..... 252
来源：http://zqt.sjlbkw.cn

TypeScript ..... 212
来源：http://xeb.nanxinkj.top

Java ........... 212
来源：http://kwz.jyoumei.cn

Go ............. 212
来源：http://qms.sysykeji.top

Ruby ........... 212
来源：http://taw.havefunace.top

C# ............. 212
来源：http://yrf.hammf.cn

C .............. 30
来源：http://mgx.hcnkem.com

C++ ............ 30
来源：http://yhl.nanxuanxn.top

SQL ............ 90
来源：http://kkp.sufxvd.cn

Bash ........... 80
来源：http://ekn.yanxiufei.cn

Kotlin ......... 15
来源：http://rqz.xinyue.icu

Swift .......... 15
来源：http://yjd.hnqzz.top

Lua ............ 10
来源：http://xuj.ehwqpu.com

Perl ........... 10
来源：http://fmc.0kj1m.cn

Scala .......... 10
来源：http://dmh.aizwys.cn

------------------------------------
来源：http://edu.aizwys.cn

合计 ........... 2106 条
来源：http://gpm.yj20258888.top

按章节统计：
来源：http://asb.shuidangran.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://trn.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zgi.52xcode.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://omp.xziqi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vaz.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sem.epnwcf.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vzk.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dch.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://smg.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wil.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://scf.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://awr.9152youxi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ric.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hav.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qjc.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ppu.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://acd.nwbrower.top

Q SQL 专题                              90
来源：http://drp.ydzc1.top

R Bash 专题                             80
来源：http://gjd.hnqzz.top

S C / C++ 专题                          60
来源：http://dan.jyoumei.cn

T 其他语言补充                          60
来源：http://nky.yangfankeji.com

U 高频实用片段                         120
来源：http://ymm.guannengcc.top

------------------------------------
来源：http://czo.zdbjq.cn

合计                                  2106 条
来源：http://wtv.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://ykz.yueranfly.top

使用提醒
来源：http://ndq.shanyushiyangtech.top

--------------------------------------------------------------------------------
来源：http://rex.yuxming.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ivc.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://prj.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://spb.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nmr.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ham.fengsongda.top

—— 文件结束 ——
来源：http://pwl.xuetiantiany.cn

================================================================================
来源：http://vih.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://zvv.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://znb.hongshengwenyu.top

================================================================================
来源：http://xuk.sufxvd.cn

【收录内容】
来源：http://qgo.tian-w.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zlq.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gxc.nanxinkj.top

SQL · Bash · C · C++
来源：http://kpe.shuidangran.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nah.yangfankeji.com

【使用说明】
来源：http://wae.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://okt.meibo888.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ytq.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jrb.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://aej.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iji.yangfankeji.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rkx.fanxiaobao.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lmo.sweek.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vcv.ywan-chungtsiang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://shs.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zfc.jqgfzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ork.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zih.cheryme.top

【文件统计】
来源：http://pwq.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lhr.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://prk.tianlin.xyz

目  录
来源：http://wci.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://kwp.fengsongda.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://duk.ydzc1.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zkg.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tyb.zdqjudy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cfh.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://axr.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://pze.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jop.sufxvd.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jyh.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vtk.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hgh.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ddl.feifeiyinyue.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jin.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mhp.shangyingyoupin.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hsw.zhixingplan.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dkx.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ket.snrcjt.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://oxb.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lfz.yj20258888.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xsf.gogol.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypc.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kyp.shzxlz.cn

================================================================================
来源：http://jyu.tanke756.top

A. 基础语法与类型
来源：http://emy.yonumen.top

================================================================================
来源：http://qqp.fzhhl.top

[A01] Hello World
来源：http://iuk.fehbvm.com

Py:   print("Hello, World!")
来源：http://tfw.hammf.cn

PHP:  echo "Hello, World!";
来源：http://jeq.jqgfzy.top

JS:   console.log("Hello, World!");
来源：http://ydr.pycfn.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://piq.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://eif.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://dfv.ehwqpu.com

Ruby: puts "Hello, World!"
来源：http://egk.meibo888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bbr.sysykeji.top

[A02] 变量声明与赋值
来源：http://vra.xinyue.icu

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dmp.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ywl.hnqzz.top

JS:   let name = "Alex"; const age = 20;
来源：http://jkl.zhoulong.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mum.nwbrower.top

Java: String name = "Alex"; int age = 20;
来源：http://dvf.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://lxe.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://ihv.xziqi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uop.fehbvm.com

[A03] 常量定义
来源：http://yjg.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lwl.0kj1m.cn

PHP:  const PI = 3.14159;
来源：http://imm.jqgfzy.top


<!-- 参考信息 -->