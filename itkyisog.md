代发 wailian999

[U31] Py：单测
来源：http://onj.shuidangran.top

python -m pytest -q
来源：http://nru.yj202588.top

[U32] Py：代码格式化
来源：http://gwc.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://cmp.vqdsnc.cn

[U33] Py：打包发布
来源：http://gxm.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://fan.gzhubu.top

[U34] Py：判断编码
来源：http://ubd.hysaishi.cn

chardet.detect(raw)
来源：http://jvh.316326.xyz

[U35] Py：发送邮件
来源：http://acs.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vlj.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://plc.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://wdr.zhengqikj.top

[U37] Py：读写 Excel
来源：http://dey.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tno.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://pie.zycfv.cn

Path(__file__).resolve().parent
来源：http://zug.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://pax.jinqigfzy.top

sys.stdout.isatty()
来源：http://qwn.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://efa.hammf.cn

print("err", file=sys.stderr)
来源：http://qze.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://otx.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eyq.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://akv.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jns.fzhhl.top

[U43] PHP：声明命名空间
来源：http://dhc.wangshuangyany.cn

namespace App\Http;
来源：http://vsn.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://fpo.xinyue.icu

declare(strict_types=1);
来源：http://sxx.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://suz.uphjek.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://uoo.yanxiufei.cn

[U46] PHP：可空类型
来源：http://xyr.ydjk.org.cn

?string $name = null
来源：http://uoo.daxiang520.top

[U47] PHP：联合类型
来源：http://eyq.xinyue.icu

int|string $id
来源：http://zaz.xylfe.cn

[U48] PHP：纯枚举
来源：http://vkl.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ock.gaohongyu789.top

[U49] PHP：只读属性
来源：http://rho.chenjidiqi.icu

public readonly string $name
来源：http://gps.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://epj.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://ijr.andypj.xyz

[U51] PHP：数组解构
来源：http://rfr.yangfankeji.com

[$a, $b] = $arr;
来源：http://bzo.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://whp.ivvv.top

$double = fn($x) => $x * 2;
来源：http://rsw.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://phk.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://nia.guowangkeji.top

[U54] PHP：空安全调用
来源：http://xao.daxiang520.top

$obj?->method()
来源：http://edp.havefunace.top

[U55] PHP：match 表达式
来源：http://aar.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yxf.bbcook.cn

[U56] PHP：命名参数
来源：http://zop.pycfn.com

f(a: 1, b: 2)
来源：http://btd.jinghuilouyu.cn

[U57] PHP：字符串插值
来源：http://wyg.andypj.xyz

"值: {$a}"
来源：http://dmt.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://wuf.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sci.cheryme.top

[U59] PHP：自定义排序
来源：http://avp.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cha.sxryk.cn

[U60] PHP：JSON 编解码
来源：http://vlz.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ggl.wangshuangyany.cn

[U61] PHP：正则
来源：http://ilu.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pxw.gzhubu.top

[U62] PHP：日期对象
来源：http://wsi.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iod.cashguo.top

[U63] PHP：文件读写
来源：http://lht.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mho.0kj1m.cn

[U64] PHP：目录遍历
来源：http://fia.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://wok.jiagoushi.top

[U65] PHP：会话
来源：http://ewa.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xrp.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://nre.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ljv.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://noy.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://djr.0kj1m.cn

[U68] PHP：PDO 连接
来源：http://ink.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dnm.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://ksn.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qnh.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://qqa.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hrb.zhengqikj.top

[U71] PHP：抛出异常
来源：http://avg.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://zno.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://dpk.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://mhg.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://ahk.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://xtl.meibo888.top

[U74] PHP：读取环境变量
来源：http://fjy.aizwys.cn

getenv("APP_ENV") ?: "production"
来源：http://wij.zycfv.cn

[U75] PHP：依赖注入
来源：http://upp.yvedp.cn

composer require psr/container
来源：http://fvr.chenlongwang.top

[U76] PHP：简单路由
来源：http://xvw.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vli.tianlin.xyz

[U77] PHP：模板渲染
来源：http://ybh.fengsongda.top

composer require twig/twig
来源：http://wsl.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://xgo.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://kxq.shuidangran.top

[U79] PHP：静态分析
来源：http://xpf.tanke756.top

composer require --dev phpstan/phpstan
来源：http://bga.hnqzz.top

[U80] PHP：代码规范修复
来源：http://sem.chenzaomai.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://oej.yongpay.top

[U81] JS：初始化项目
来源：http://duc.yanxiufei.cn

npm init -y;  npm i express
来源：http://ois.xziqi.cn

[U82] JS：package.json 脚本
来源：http://kfs.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aqf.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://vds.hnxiangtu.top

export const a = 1;  import { a } from "./m.js";
来源：http://npr.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://xdc.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://bvx.tian-w.cn

[U85] JS：可选链
来源：http://gkh.mhx1999.top

a?.b?.c
来源：http://rfg.hnqzz.top

[U86] JS：空值合并
来源：http://qul.sjlbkw.cn

a ?? b
来源：http://xko.feifeiyinyue.top

[U87] JS：解构默认值
来源：http://lgg.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://wwj.shzxlz.cn

[U88] JS：对象展开合并
来源：http://ety.fzhhl.top

{ ...a, ...b }
来源：http://tvb.feifeiyinyue.top

[U89] JS：数组去重
来源：http://xfn.smart0.xyz

[...new Set(arr)]
来源：http://eye.yangfankeji.com

[U90] JS：数字数组排序
来源：http://swd.xuanzx.com

[...arr].sort((a, b) => a - b)
来源：http://xrs.jqgufenzy.top

[U91] JS：对象键值遍历
来源：http://jdv.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tkf.zdbjq.cn

[U92] JS：深拷贝
来源：http://gzs.kuanghao11.cn

structuredClone(obj)
来源：http://fzl.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://vnw.0kj1m.cn

`共 ${n} 条`
来源：http://pox.xziqi.cn

[U94] JS：箭头函数
来源：http://dof.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://udy.52xcode.cn

[U95] JS：Promise 包装
来源：http://owm.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://xll.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://zyn.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baw.0kj1m.cn

[U97] JS：并发请求
来源：http://dij.gotoacloud.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgo.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://koj.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jih.kuanghao11.cn

[U99] JS：事件监听
来源：http://ixe.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://mvy.meibo888.top

[U100] JS：DOM 查询
来源：http://pnv.hcnkem.com

document.querySelector(".item")
来源：http://wkz.nwbrower.top

[U101] JS：classList 操作
来源：http://jrj.zhixingplan.top

el.classList.toggle("active")
来源：http://nvz.bjfxy.top

[U102] JS：本地存储
来源：http://guo.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://nju.nwbrower.top

[U103] JS：定时器
来源：http://qeo.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pyk.iojbl.cn

[U104] JS：防抖
来源：http://ubt.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrc.shangyingyoupin.top

[U105] JS：节流
来源：http://bcn.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lnx.ppjwa.cn

[U106] JS：日期格式化
来源：http://ywv.ydzc1.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://syq.daria6918.cn

[U107] JS：数字千分位
来源：http://cul.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://frb.xuetiantiany.cn

[U108] JS：随机整数
来源：http://uoj.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vuq.52xcode.cn

[U109] JS：数组分组
来源：http://dlc.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://fit.yvedp.cn

[U110] JS：数组分块
来源：http://xdo.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cyg.cheryme.top

[U111] JS：对象转 Map
来源：http://ogb.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://xhd.redwolf501.top

[U112] JS：字符串补位
来源：http://eam.guowangkeji.top

"7".padStart(3, "0")
来源：http://mqk.hammf.cn

[U113] JS：正则替换全部
来源：http://hrr.bjfxy.top

s.replaceAll("a", "b")
来源：http://itx.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://kbv.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://qcp.ctjpmb.com

[U115] JS：生成 UUID
来源：http://dfa.sjlbkw.cn

crypto.randomUUID()
来源：http://som.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://rsv.kuanghao11.cn

/** @param {string} name */ function f(name) {}
来源：http://kri.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://rlr.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://aeh.chenlongwang.top

[U118] JS：开发服务器
来源：http://uah.ppjwa.cn

npm i -D vite;  npx vite
来源：http://hcw.dashuyun.cn

[U119] JS：生产构建
来源：http://lqa.fktsv.cn

npx vite build
来源：http://qdd.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://sga.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://fph.jinyuanbaomall.cn

================================================================================
来源：http://fsl.ppjwa.cn

统计汇总
来源：http://lwa.zhengqikj.top

================================================================================
来源：http://lbk.jianghu66.top

按语言统计（条）：
来源：http://whu.kuanghao11.cn

Python ......... 252
来源：http://vbf.yangfankeji.com

PHP ............ 252
来源：http://kkq.zycfv.cn

JavaScript ..... 252
来源：http://qzy.daria6918.cn

TypeScript ..... 212
来源：http://zch.jinqigufen.top

Java ........... 212
来源：http://tnf.gogol.net.cn

Go ............. 212
来源：http://fab.gzhubu.top

Ruby ........... 212
来源：http://bdc.bjfxy.top

C# ............. 212
来源：http://lov.dianchejie.cn

C .............. 30
来源：http://lfa.smart0.xyz

C++ ............ 30
来源：http://ski.pengpengdd.cyou

SQL ............ 90
来源：http://ljr.nwbrower.top

Bash ........... 80
来源：http://xib.shangyingyoupin.top

Kotlin ......... 15
来源：http://nrf.dashuyun.cn

Swift .......... 15
来源：http://vhv.tianlin.xyz

Lua ............ 10
来源：http://scz.c1oappe.top

Perl ........... 10
来源：http://kdu.yonumen.top

Scala .......... 10
来源：http://emx.hcnkem.com

------------------------------------
来源：http://jeq.haohaochexian.top

合计 ........... 2106 条
来源：http://ekc.jinqigufen.top

按章节统计：
来源：http://bzt.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mvk.smart0.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jqy.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tne.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xou.ywan-chungtsiang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dvs.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cqn.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gbb.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://edz.gotoacloud.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xvg.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jop.sjlbkw.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jag.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cpl.52xcode.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pef.9152youxi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gsk.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kbb.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zml.ydzc1.top

Q SQL 专题                              90
来源：http://gzv.feifeiyinyue.top

R Bash 专题                             80
来源：http://ont.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://xvr.cdnleiting.top

T 其他语言补充                          60
来源：http://esa.zhiwuduotai.top

U 高频实用片段                         120
来源：http://bas.kuanghao11.cn

------------------------------------
来源：http://uia.sweek.top

合计                                  2106 条
来源：http://uru.c1oappe.top

--------------------------------------------------------------------------------
来源：http://woo.snrcjt.cn

使用提醒
来源：http://xdu.yonumen.top

--------------------------------------------------------------------------------
来源：http://pyg.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wxw.kuanghao11.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tph.yueranfly.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zxp.hesvh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://taa.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fwi.kuanghao11.cn

—— 文件结束 ——
来源：http://wqj.epnwcf.com

================================================================================
来源：http://ctg.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://vhg.ppjwa.cn

Common Programming Examples Cheat Book
来源：http://nsu.xingfuxueyuan.xyz

================================================================================
来源：http://tez.yfazqb.com

【收录内容】
来源：http://itb.jqgfzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ijc.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://guz.vehdjk.com

SQL · Bash · C · C++
来源：http://zpu.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fgs.daria6918.cn

【使用说明】
来源：http://uhr.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kzs.yanxiufei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mle.sysykeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wls.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://juh.xuanzx.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rme.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vir.aizwys.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mfm.hywenlv.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://iaw.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pjp.meibo888.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qlm.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qkl.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pyj.ppjwa.cn

【文件统计】
来源：http://lzy.daria6918.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://sbo.feifeiyinyue.top

--------------------------------------------------------------------------------
来源：http://rhe.gzhubu.top

目  录
来源：http://flj.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://cji.svipenyu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://leg.feifeiyinyue.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ron.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gcu.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xrk.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jdg.aibaodan.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bha.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ttq.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mgn.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ljn.daxiang520.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gpk.hfpthk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dkq.sysykeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lic.gotoacloud.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://drt.yonumen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gve.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbo.iojbl.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gqi.iojbl.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hit.shanyushiyangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bfl.cashguo.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oeb.xylfe.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://laa.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hty.ppjwa.cn

================================================================================
来源：http://khy.nanxinkj.top

A. 基础语法与类型
来源：http://tsf.shangyingyoupin.top

================================================================================
来源：http://pas.ivvv.top

[A01] Hello World
来源：http://hra.hnxiangtu.top

Py:   print("Hello, World!")
来源：http://bud.yueranfly.top

PHP:  echo "Hello, World!";
来源：http://gji.cqqwz.cn

JS:   console.log("Hello, World!");
来源：http://rwx.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dxs.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://fof.bjfxy.top

Go:   fmt.Println("Hello, World!")
来源：http://vij.sysykeji.top

Ruby: puts "Hello, World!"
来源：http://fnl.pengpengdd.cyou

C#:   Console.WriteLine("Hello, World!");
来源：http://dtx.cucudq.cn

[A02] 变量声明与赋值
来源：http://drs.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ubt.tarul.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tgq.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ptw.sysykeji.top


<!-- 参考信息 -->