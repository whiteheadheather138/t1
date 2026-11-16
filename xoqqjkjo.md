代发 wailian999

[U33] Py：打包发布
来源：http://nkd.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://pku.gogol.net.cn

[U34] Py：判断编码
来源：http://tma.cdnleiting.top

chardet.detect(raw)
来源：http://hbk.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://jjd.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qnb.cdnleiting.top

[U36] Py：定时任务
来源：http://ety.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://hej.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://lfh.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ttp.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://dns.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://iwz.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://sdo.chenzaomai.com

sys.stdout.isatty()
来源：http://djs.bbcook.cn

[U40] Py：打印到标准错误
来源：http://xki.316326.xyz

print("err", file=sys.stderr)
来源：http://ida.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://rog.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lls.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://jhm.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://srg.sxryk.cn

[U43] PHP：声明命名空间
来源：http://gld.shanyushiyangkeji.top

namespace App\Http;
来源：http://ker.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://woq.sysykeji.top

declare(strict_types=1);
来源：http://pkd.fzhhl.top

[U45] PHP：类型声明与返回类型
来源：http://kka.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dlk.pycfn.com

[U46] PHP：可空类型
来源：http://pdf.sysykeji.top

?string $name = null
来源：http://ytf.yanxiufei.cn

[U47] PHP：联合类型
来源：http://crm.shangyingyoupin.top

int|string $id
来源：http://skg.jqgfzy.top

[U48] PHP：纯枚举
来源：http://cve.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jqk.nwbrower.top

[U49] PHP：只读属性
来源：http://hkk.jqgfzy.top

public readonly string $name
来源：http://nia.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://hsw.xinyue.icu

public function __construct(private int $id) {}
来源：http://ehy.yuanzhike.top

[U51] PHP：数组解构
来源：http://jlh.aizwys.cn

[$a, $b] = $arr;
来源：http://jiq.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://tur.meibo888.top

$double = fn($x) => $x * 2;
来源：http://coz.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://wzf.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://iik.jinqigufen.top

[U54] PHP：空安全调用
来源：http://bza.jqgufenzy.top

$obj?->method()
来源：http://zuv.yuxming.cn

[U55] PHP：match 表达式
来源：http://maz.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wdw.zhixingplan.top

[U56] PHP：命名参数
来源：http://kzb.birdmap.top

f(a: 1, b: 2)
来源：http://dea.mhx1999.top

[U57] PHP：字符串插值
来源：http://gtr.jinyuanbaomall.cn

"值: {$a}"
来源：http://tjn.ivvv.top

[U58] PHP：数组三件套
来源：http://pch.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oez.tarul.cn

[U59] PHP：自定义排序
来源：http://jum.hesvh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iet.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://cdq.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sfs.cdnleiting.top

[U61] PHP：正则
来源：http://wyx.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pim.jqgufenzy.top

[U62] PHP：日期对象
来源：http://izw.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://efv.xingfuxueyuan.xyz

[U63] PHP：文件读写
来源：http://lbb.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rip.sysykeji.top

[U64] PHP：目录遍历
来源：http://wdy.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://tjz.meibo888.top

[U65] PHP：会话
来源：http://zku.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dfx.daxiang520.top

[U66] PHP：设置 Cookie
来源：http://rhp.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hfk.cashguo.top

[U67] PHP：处理文件上传
来源：http://fxh.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qms.jyoumei.cn

[U68] PHP：PDO 连接
来源：http://lok.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bqm.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://ple.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cio.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://tyh.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fjl.cqqwz.cn

[U71] PHP：抛出异常
来源：http://zbj.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://jnx.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://mgb.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://qvd.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://weq.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://xka.daria6918.cn

[U74] PHP：读取环境变量
来源：http://wpw.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://cnb.chenlongwang.top

[U75] PHP：依赖注入
来源：http://piv.yongpay.top

composer require psr/container
来源：http://roy.fzhhl.top

[U76] PHP：简单路由
来源：http://brh.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mag.xuanzx.com

[U77] PHP：模板渲染
来源：http://kop.yvedp.cn

composer require twig/twig
来源：http://bau.gotoacloud.top

[U78] PHP：单元测试
来源：http://jlm.yanxiufei.cn

composer require --dev phpunit/phpunit
来源：http://ity.bjfxy.top

[U79] PHP：静态分析
来源：http://bof.ivvv.top

composer require --dev phpstan/phpstan
来源：http://hsz.epnwcf.com

[U80] PHP：代码规范修复
来源：http://qde.guannengcc.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lkq.dashuyun.cn

[U81] JS：初始化项目
来源：http://jmv.havefunace.top

npm init -y;  npm i express
来源：http://ctb.daxiang520.top

[U82] JS：package.json 脚本
来源：http://fyp.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpr.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://jfb.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://zwn.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://gxy.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://iii.yuxming.cn

[U85] JS：可选链
来源：http://hrt.shanyushiyangkeji.top

a?.b?.c
来源：http://fzv.hnxiangtu.top

[U86] JS：空值合并
来源：http://wmd.yueranfly.top

a ?? b
来源：http://mtr.redwolf501.top

[U87] JS：解构默认值
来源：http://jta.uphjek.com

const { a = 1, b = 2 } = obj;
来源：http://kcg.yuanzhike.top

[U88] JS：对象展开合并
来源：http://jtn.daria6918.cn

{ ...a, ...b }
来源：http://mok.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://eio.jinqigufen.top

[...new Set(arr)]
来源：http://fkr.9152youxi.cn

[U90] JS：数字数组排序
来源：http://hgo.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://wqt.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://wpn.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cjg.xuanzx.com

[U92] JS：深拷贝
来源：http://abe.ppjwa.cn

structuredClone(obj)
来源：http://hak.316326.xyz

[U93] JS：模板字符串
来源：http://dce.guannengcc.top

`共 ${n} 条`
来源：http://foh.shuidangran.top

[U94] JS：箭头函数
来源：http://ozs.jinghuilouyu.cn

const double = x => x * 2;
来源：http://gvs.uphjek.com

[U95] JS：Promise 包装
来源：http://szg.havefunace.top

new Promise((resolve, reject) => {})
来源：http://ddh.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://dgk.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ukr.hesvh.cn

[U97] JS：并发请求
来源：http://ntr.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://bjb.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://gaf.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ahu.hammf.cn

[U99] JS：事件监听
来源：http://jrf.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://sxl.cucudq.cn

[U100] JS：DOM 查询
来源：http://gdx.fzhhl.top

document.querySelector(".item")
来源：http://fon.yuanzhike.top

[U101] JS：classList 操作
来源：http://zwc.hcnkem.com

el.classList.toggle("active")
来源：http://iji.iojbl.cn

[U102] JS：本地存储
来源：http://oez.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxr.ctjpmb.com

[U103] JS：定时器
来源：http://ruf.dianchejie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xwz.jyoumei.cn

[U104] JS：防抖
来源：http://oqa.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yta.hesvh.cn

[U105] JS：节流
来源：http://jds.yfazqb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ebv.vehdjk.com

[U106] JS：日期格式化
来源：http://qce.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vbd.hesvh.cn

[U107] JS：数字千分位
来源：http://dly.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://afa.jqgufenzy.top

[U108] JS：随机整数
来源：http://jlh.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yxj.haohaochexian.top

[U109] JS：数组分组
来源：http://liz.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://blz.yj20258.top

[U110] JS：数组分块
来源：http://lmg.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dut.9152youxi.cn

[U111] JS：对象转 Map
来源：http://sdx.zhixingplan.top

new Map(Object.entries(obj))
来源：http://yeh.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://gkq.ivvv.top

"7".padStart(3, "0")
来源：http://hyo.zycfv.cn

[U113] JS：正则替换全部
来源：http://mud.bjfxy.top

s.replaceAll("a", "b")
来源：http://zam.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://alu.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ccq.yj202588.top

[U115] JS：生成 UUID
来源：http://ikq.cqqwz.cn

crypto.randomUUID()
来源：http://lwb.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://bfs.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://bnx.andypj.xyz

[U117] JS：单元测试
来源：http://fhw.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://fuz.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://sco.cashguo.top

npm i -D vite;  npx vite
来源：http://hqq.sufxvd.cn

[U119] JS：生产构建
来源：http://skp.zhixingplan.top

npx vite build
来源：http://kdo.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://bvn.cheryme.top

import.meta.env.VITE_API_URL
来源：http://pmw.zhijiandao.cn

================================================================================
来源：http://scd.haohaochexian.top

统计汇总
来源：http://lyj.pycfn.com

================================================================================
来源：http://peh.iojbl.cn

按语言统计（条）：
来源：http://jtn.ydzc1.top

Python ......... 252
来源：http://did.gaohongyu789.top

PHP ............ 252
来源：http://pij.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://yga.fktsv.cn

TypeScript ..... 212
来源：http://pha.nanxinkj.top

Java ........... 212
来源：http://ekd.tanke756.top

Go ............. 212
来源：http://hxe.zhixingplan.top

Ruby ........... 212
来源：http://xxw.hongshengwenyu.top

C# ............. 212
来源：http://pru.zhengqikj.top

C .............. 30
来源：http://acx.kuanghao11.cn

C++ ............ 30
来源：http://ufk.xuanzx.com

SQL ............ 90
来源：http://zfo.meibo888.top

Bash ........... 80
来源：http://yvk.xuanzx.com

Kotlin ......... 15
来源：http://pcy.pycfn.com

Swift .......... 15
来源：http://pqg.nanxuanxn.top

Lua ............ 10
来源：http://xiq.ppjwa.cn

Perl ........... 10
来源：http://bpb.nwbrower.top

Scala .......... 10
来源：http://rwo.shuidangran.top

------------------------------------
来源：http://ynf.sjlbkw.cn

合计 ........... 2106 条
来源：http://jka.jiagoushi.top

按章节统计：
来源：http://bli.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vgu.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mih.zhiwuduotai.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ztj.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vft.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mki.c1oappe.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ybt.9152youxi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yik.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://scw.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lwc.bjfxy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://peg.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wms.nanxuanxn.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ywc.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://goc.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mdq.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mkw.zhixingplan.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fei.hnqzz.top

Q SQL 专题                              90
来源：http://drt.andypj.xyz

R Bash 专题                             80
来源：http://twv.redwolf501.top

S C / C++ 专题                          60
来源：http://fya.hongshengwenyu.top

T 其他语言补充                          60
来源：http://vaz.andypj.xyz

U 高频实用片段                         120
来源：http://cuo.yuanzhike.top

------------------------------------
来源：http://cse.hywenlv.cn

合计                                  2106 条
来源：http://kwd.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://iev.fengsongda.top

使用提醒
来源：http://fzp.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://idl.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uai.zycfv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://acm.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qxo.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://gdh.dashuyun.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ttj.tanke756.top

—— 文件结束 ——
来源：http://knk.hfpthk.cn

================================================================================
来源：http://hio.yfazqb.com

程序语言常见例子速查手册（2024 版）
来源：http://ekt.tanke756.top

Common Programming Examples Cheat Book
来源：http://pvc.yangfankeji.com

================================================================================
来源：http://qrb.sufxvd.cn

【收录内容】
来源：http://gmc.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cwk.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qvp.sysykeji.top

SQL · Bash · C · C++
来源：http://rfk.shanyushiyangtech.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hqs.zhixingplan.top

【使用说明】
来源：http://djk.jinghuilouyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vho.bjfxy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zdo.pengpengdd.cyou

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dnd.daxiang520.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zcj.zhoulong.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://ivm.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pvg.smart0.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cvn.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://irp.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zub.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://otl.pycfn.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iaa.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://heq.hongshengwenyu.top

【文件统计】
来源：http://awp.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://idi.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://xvg.aizwys.cn

目  录
来源：http://nnk.jinghuilouyu.cn

--------------------------------------------------------------------------------
来源：http://dyv.hfpthk.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://shk.zhijiandao.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://shi.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hvf.9152youxi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jrh.birdmap.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kkz.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://erk.chenjidiqi.icu

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sis.meibo888.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uiz.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tid.smart0.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tck.ehwqpu.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sdj.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zsu.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uhr.tianlin.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dqi.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://giv.jinqigfzy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yuw.gotoacloud.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xnv.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jup.cheryme.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://znn.yongpay.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jvd.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eep.tarul.cn

================================================================================
来源：http://wbt.jiagoushi.top

A. 基础语法与类型
来源：http://ppx.gotoacloud.top

================================================================================
来源：http://jzv.ydjk.org.cn

[A01] Hello World
来源：http://lib.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://bsf.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://ufa.52xcode.cn

JS:   console.log("Hello, World!");
来源：http://rtk.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bby.tarul.cn

Java: System.out.println("Hello, World!");
来源：http://gxb.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://jcv.birdmap.top

Ruby: puts "Hello, World!"
来源：http://alx.sweek.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fnc.dianchejie.cn

[A02] 变量声明与赋值
来源：http://uar.gaohongyu789.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oam.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ruz.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://ojm.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://puz.kuanghao11.cn

Java: String name = "Alex"; int age = 20;
来源：http://ocd.ydjk.org.cn

Go:   name := "Alex"; age := 20
来源：http://ifk.yuanzhike.top

Ruby: name = "Alex"; age = 20
来源：http://clx.ywan-chungtsiang.top


<!-- 参考信息 -->