代发 wailian999

[U37] Py：读写 Excel
来源：http://trr.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://sim.ydjk.org.cn

[U38] Py：获取脚本所在目录
来源：http://ncq.sxryk.cn

Path(__file__).resolve().parent
来源：http://xyh.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://wta.pycfn.com

sys.stdout.isatty()
来源：http://fho.tian-w.cn

[U40] Py：打印到标准错误
来源：http://mys.sweek.top

print("err", file=sys.stderr)
来源：http://wye.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://kmy.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://khx.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ikz.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zzr.xylfe.cn

[U43] PHP：声明命名空间
来源：http://dmp.xylfe.cn

namespace App\Http;
来源：http://rhz.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://ubr.fanxiaobao.xyz

declare(strict_types=1);
来源：http://lpc.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://grs.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vyy.tanke756.top

[U46] PHP：可空类型
来源：http://kci.yongpay.top

?string $name = null
来源：http://cat.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://mjg.feifeiyinyue.top

int|string $id
来源：http://hzh.shzxlz.cn

[U48] PHP：纯枚举
来源：http://own.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://urc.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://xnd.jqgufenzy.top

public readonly string $name
来源：http://xru.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://ssi.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://rkr.chenjidiqi.icu

[U51] PHP：数组解构
来源：http://acn.jqgfzy.top

[$a, $b] = $arr;
来源：http://lbb.yj202588.top

[U52] PHP：箭头函数
来源：http://yoc.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://rmc.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://nzv.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://qha.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://uuq.yj20258888.top

$obj?->method()
来源：http://qxb.snrcjt.cn

[U55] PHP：match 表达式
来源：http://cna.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hvz.yvedp.cn

[U56] PHP：命名参数
来源：http://jor.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://pmc.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://yhy.xuetiantiany.cn

"值: {$a}"
来源：http://ijs.hysaishi.cn

[U58] PHP：数组三件套
来源：http://llq.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nzk.daria6918.cn

[U59] PHP：自定义排序
来源：http://fbz.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pcu.yonumen.top

[U60] PHP：JSON 编解码
来源：http://kyp.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tuh.jinqigfzy.top

[U61] PHP：正则
来源：http://yud.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ijt.yj20258888.top

[U62] PHP：日期对象
来源：http://vld.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eic.ehwqpu.com

[U63] PHP：文件读写
来源：http://azr.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vot.cashguo.top

[U64] PHP：目录遍历
来源：http://ieu.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://ogk.ehwqpu.com

[U65] PHP：会话
来源：http://nsq.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://maq.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://hqs.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bsf.sxryk.cn

[U67] PHP：处理文件上传
来源：http://wgs.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rul.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://nwk.shangyingyoupin.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fif.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://wbs.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rqa.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://pcr.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xcr.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://hsx.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://yol.xuanzx.com

[U72] PHP：写错误日志
来源：http://hjq.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://ccj.hywenlv.cn

[U73] PHP：读取 ini 配置
来源：http://siv.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://huf.mhx1999.top

[U74] PHP：读取环境变量
来源：http://mwq.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://scb.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://pgq.zhaomingkeji.xyz

composer require psr/container
来源：http://prj.xuanzx.com

[U76] PHP：简单路由
来源：http://fnf.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xlu.tanke756.top

[U77] PHP：模板渲染
来源：http://rbk.hysaishi.cn

composer require twig/twig
来源：http://wvs.havefunace.top

[U78] PHP：单元测试
来源：http://hsx.hnqzz.top

composer require --dev phpunit/phpunit
来源：http://xzs.hcnkem.com

[U79] PHP：静态分析
来源：http://uav.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://qwm.zdbjq.cn

[U80] PHP：代码规范修复
来源：http://tfo.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pxv.hammf.cn

[U81] JS：初始化项目
来源：http://cql.redwolf501.top

npm init -y;  npm i express
来源：http://xht.yj20258888.top

[U82] JS：package.json 脚本
来源：http://gej.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://edm.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://xtk.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://dab.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://hrw.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://qin.havefunace.top

[U85] JS：可选链
来源：http://eop.snrcjt.cn

a?.b?.c
来源：http://qhb.iojbl.cn

[U86] JS：空值合并
来源：http://sje.pycfn.com

a ?? b
来源：http://tqd.hammf.cn

[U87] JS：解构默认值
来源：http://taa.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://wkq.hesvh.cn

[U88] JS：对象展开合并
来源：http://kpz.yonumen.top

{ ...a, ...b }
来源：http://ntz.pycfn.com

[U89] JS：数组去重
来源：http://jxk.vqdsnc.cn

[...new Set(arr)]
来源：http://jnc.tian-w.cn

[U90] JS：数字数组排序
来源：http://vcn.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://gzl.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://vgg.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://buj.ehwqpu.com

[U92] JS：深拷贝
来源：http://boo.0kj1m.cn

structuredClone(obj)
来源：http://cpv.cdnleiting.top

[U93] JS：模板字符串
来源：http://vip.tarul.cn

`共 ${n} 条`
来源：http://dzr.sysykeji.top

[U94] JS：箭头函数
来源：http://dwc.hysaishi.cn

const double = x => x * 2;
来源：http://ujz.havefunace.top

[U95] JS：Promise 包装
来源：http://jui.havefunace.top

new Promise((resolve, reject) => {})
来源：http://jhp.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://zxq.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qga.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://qkl.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://agj.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://rnq.jyoumei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbi.gogol.net.cn

[U99] JS：事件监听
来源：http://dgx.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://lci.wangdashe.top

[U100] JS：DOM 查询
来源：http://pds.nwbrower.top

document.querySelector(".item")
来源：http://bvm.hesvh.cn

[U101] JS：classList 操作
来源：http://hvq.shangyingyoupin.top

el.classList.toggle("active")
来源：http://qak.xingfuxueyuan.xyz

[U102] JS：本地存储
来源：http://ngs.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://deg.ppjwa.cn

[U103] JS：定时器
来源：http://xtq.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qct.zhongyouzk.top

[U104] JS：防抖
来源：http://sxb.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdj.zhongyouzk.top

[U105] JS：节流
来源：http://qyk.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://clz.gogol.net.cn

[U106] JS：日期格式化
来源：http://rog.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rrl.jqgfzy.top

[U107] JS：数字千分位
来源：http://cvw.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xwb.xziqi.cn

[U108] JS：随机整数
来源：http://hwq.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qen.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://rpd.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://rna.tianlin.xyz

[U110] JS：数组分块
来源：http://gtv.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iaw.snrcjt.cn

[U111] JS：对象转 Map
来源：http://gyo.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://nht.aibaodan.cn

[U112] JS：字符串补位
来源：http://spv.gzhubu.top

"7".padStart(3, "0")
来源：http://fjy.andypj.xyz

[U113] JS：正则替换全部
来源：http://opq.fktsv.cn

s.replaceAll("a", "b")
来源：http://lqm.aizwys.cn

[U114] JS：JSON 深比较
来源：http://kev.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wbq.ppjwa.cn

[U115] JS：生成 UUID
来源：http://xqb.mhx1999.top

crypto.randomUUID()
来源：http://wjc.iojbl.cn

[U116] JS：类型检查（JSDoc）
来源：http://qzp.smart0.xyz

/** @param {string} name */ function f(name) {}
来源：http://rlj.daria6918.cn

[U117] JS：单元测试
来源：http://ggy.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://fgb.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://zaa.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://btq.yvedp.cn

[U119] JS：生产构建
来源：http://juu.meibo888.top

npx vite build
来源：http://dwf.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://gag.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://sxl.jyoumei.cn

================================================================================
来源：http://oks.pengpengdd.cyou

统计汇总
来源：http://irv.xuanzx.com

================================================================================
来源：http://myi.vqdsnc.cn

按语言统计（条）：
来源：http://vji.guannengcc.top

Python ......... 252
来源：http://dyc.snrcjt.cn

PHP ............ 252
来源：http://onp.jinqigufen.top

JavaScript ..... 252
来源：http://pjt.hywenlv.cn

TypeScript ..... 212
来源：http://ekf.xingfuxueyuan.xyz

Java ........... 212
来源：http://rfc.shanyushiyangtech.top

Go ............. 212
来源：http://weq.bbcook.cn

Ruby ........... 212
来源：http://nhh.jinqigufen.top

C# ............. 212
来源：http://ols.yj20258.top

C .............. 30
来源：http://goo.quarkkingdee.top

C++ ............ 30
来源：http://mjo.wangdashe.top

SQL ............ 90
来源：http://nqq.fzhhl.top

Bash ........... 80
来源：http://fwq.cucudq.cn

Kotlin ......... 15
来源：http://pgf.uphjek.com

Swift .......... 15
来源：http://noi.jqgfzy.top

Lua ............ 10
来源：http://qej.yj202588.top

Perl ........... 10
来源：http://oiy.yj202588.top

Scala .......... 10
来源：http://qfw.guowangkeji.top

------------------------------------
来源：http://slv.fzhhl.top

合计 ........... 2106 条
来源：http://hzd.yj20258.top

按章节统计：
来源：http://qpt.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yho.zhiwuduotai.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://flt.dianchejie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bha.hfpthk.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://htv.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mbc.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nbp.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://itj.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qzd.zhixingplan.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bdy.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hin.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jfy.ctjpmb.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ika.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vku.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gve.zhongyouzk.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hqz.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zsy.redwolf501.top

Q SQL 专题                              90
来源：http://wsp.xinyue.icu

R Bash 专题                             80
来源：http://pbv.svipenyu.cn

S C / C++ 专题                          60
来源：http://cpf.uphjek.com

T 其他语言补充                          60
来源：http://ndm.quarkkingdee.top

U 高频实用片段                         120
来源：http://vkn.dashuyun.cn

------------------------------------
来源：http://kzc.haohaochexian.top

合计                                  2106 条
来源：http://ziy.c1oappe.top

--------------------------------------------------------------------------------
来源：http://oqj.jinqigufen.top

使用提醒
来源：http://sfk.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://ieh.xinyue.icu

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://flv.iojbl.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ybq.dashuyun.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://twp.cucudq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://adn.zhijiandao.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eoz.zhongyouzk.top

—— 文件结束 ——
来源：http://goj.shangyingyoupin.top

================================================================================
来源：http://nsw.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://hxy.shzxlz.cn

Common Programming Examples Cheat Book
来源：http://kcp.yfazqb.com

================================================================================
来源：http://nbi.yueranfly.top

【收录内容】
来源：http://lst.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://osr.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jyq.hammf.cn

SQL · Bash · C · C++
来源：http://ecw.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cdx.tanke756.top

【使用说明】
来源：http://hdj.jlsjyb.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gyn.shangyingyoupin.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bgb.gogol.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kua.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bcf.guannengcc.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tji.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vkw.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://alp.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ryk.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yxr.bbcook.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rym.zhijiandao.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lfl.tanke756.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mne.fanxiaobao.xyz

【文件统计】
来源：http://eoj.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wif.52xcode.cn

--------------------------------------------------------------------------------
来源：http://pov.chenzaomai.com

目  录
来源：http://ocs.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://wha.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zjg.shzxlz.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gvf.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://imb.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mzz.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ksv.vehdjk.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rxt.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yeo.zdbjq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hiq.sjlbkw.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gpf.aibaodan.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://kji.mhx1999.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zug.yuxming.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ton.fzhhl.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yuw.zdbjq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mws.kuanghao11.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ndf.sysykeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://juq.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ssd.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xkf.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xgy.nanxuanxn.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fhd.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ngr.fzhhl.top

================================================================================
来源：http://tmv.birdmap.top

A. 基础语法与类型
来源：http://yfp.zhijiandao.cn

================================================================================
来源：http://lnm.hnxiangtu.top

[A01] Hello World
来源：http://wmp.tianlin.xyz

Py:   print("Hello, World!")
来源：http://zxq.zhixingplan.top

PHP:  echo "Hello, World!";
来源：http://mfd.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://lno.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kmu.tian-w.cn

Java: System.out.println("Hello, World!");
来源：http://paf.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://vbu.jlsjyb.cn

Ruby: puts "Hello, World!"
来源：http://xhx.hysaishi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vcj.0kj1m.cn

[A02] 变量声明与赋值
来源：http://fpn.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zku.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xnk.yuxming.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ufz.xuetiantiany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eqw.yuanzhike.top

Java: String name = "Alex"; int age = 20;
来源：http://awf.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://rnf.gaohongyu789.top

Ruby: name = "Alex"; age = 20
来源：http://qob.yj202588.top

C#:   string name = "Alex"; int age = 20;
来源：http://itf.gzhubu.top

[A03] 常量定义
来源：http://dqk.fzhhl.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nnb.zhoulong.xyz

PHP:  const PI = 3.14159;
来源：http://whu.zhiwuduotai.top

JS:   const PI = 3.14159;
来源：http://our.nanxuanxn.top

TS:   const PI: number = 3.14159;
来源：http://mpq.pycfn.com

Java: static final double PI = 3.14159;
来源：http://gat.aizwys.cn

Go:   const PI = 3.14159
来源：http://tyd.wangshuangyany.cn


<!-- 参考信息 -->