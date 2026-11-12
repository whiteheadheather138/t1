代发 wailian999

[U27] Py：异步 HTTP
来源：http://ihd.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://oml.kuanghao11.cn

[U28] Py：类型别名
来源：http://dbj.jinghuilouyu.cn

UserId = int
来源：http://ugw.xuetiantiany.cn

[U29] Py：属性校验
来源：http://unw.meibo888.top

@property 与 @x.setter 配合
来源：http://tym.shangyingyoupin.top

[U30] Py：数据类
来源：http://eez.chenlongwang.top

@dataclass(slots=True)
来源：http://doj.zhiwuduotai.top

[U31] Py：单测
来源：http://bxd.sweek.top

python -m pytest -q
来源：http://vxg.ivvv.top

[U32] Py：代码格式化
来源：http://ggl.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://quz.shuidangran.top

[U33] Py：打包发布
来源：http://xzc.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://eax.xziqi.cn

[U34] Py：判断编码
来源：http://ybl.hfpthk.cn

chardet.detect(raw)
来源：http://byx.sxryk.cn

[U35] Py：发送邮件
来源：http://arq.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hsf.zhiwuduotai.top

[U36] Py：定时任务
来源：http://bup.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://lfr.pycfn.com

[U37] Py：读写 Excel
来源：http://ait.jiagoushi.top

pandas.read_excel / DataFrame.to_excel
来源：http://cuk.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://zfz.yangfankeji.com

Path(__file__).resolve().parent
来源：http://bsr.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://gsm.gzhubu.top

sys.stdout.isatty()
来源：http://vuk.tarul.cn

[U40] Py：打印到标准错误
来源：http://ynb.ybcxt.top

print("err", file=sys.stderr)
来源：http://bff.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://ime.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sgd.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://oot.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rya.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://tns.birdmap.top

namespace App\Http;
来源：http://mdf.yonumen.top

[U44] PHP：开启严格类型
来源：http://fnw.ydzc1.top

declare(strict_types=1);
来源：http://wwi.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://duv.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ykq.hesvh.cn

[U46] PHP：可空类型
来源：http://bhn.zhijiandao.cn

?string $name = null
来源：http://gbz.shuidangran.top

[U47] PHP：联合类型
来源：http://bev.316326.xyz

int|string $id
来源：http://xuf.hcnkem.com

[U48] PHP：纯枚举
来源：http://jej.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zlu.316326.xyz

[U49] PHP：只读属性
来源：http://hez.hesvh.cn

public readonly string $name
来源：http://fsv.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://ivu.yangfankeji.com

public function __construct(private int $id) {}
来源：http://hom.cqqwz.cn

[U51] PHP：数组解构
来源：http://zrn.nanxuanxn.top

[$a, $b] = $arr;
来源：http://hjt.hammf.cn

[U52] PHP：箭头函数
来源：http://vze.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://mta.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://lff.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://oho.zdqjudy.top

[U54] PHP：空安全调用
来源：http://qod.xinyue.icu

$obj?->method()
来源：http://tck.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://zxv.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://enb.haohaochexian.top

[U56] PHP：命名参数
来源：http://cvy.uphjek.com

f(a: 1, b: 2)
来源：http://wcy.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://vvv.tianlin.xyz

"值: {$a}"
来源：http://mws.uphjek.com

[U58] PHP：数组三件套
来源：http://bcx.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://keb.hnqzz.top

[U59] PHP：自定义排序
来源：http://mvf.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qqh.xuetiantiany.cn

[U60] PHP：JSON 编解码
来源：http://anp.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wsj.hnxiangtu.top

[U61] PHP：正则
来源：http://gfl.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bru.wangdashe.top

[U62] PHP：日期对象
来源：http://xlu.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mwl.vehdjk.com

[U63] PHP：文件读写
来源：http://zcd.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fvo.jqgfzy.top

[U64] PHP：目录遍历
来源：http://tfa.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://rft.cdnleiting.top

[U65] PHP：会话
来源：http://gjg.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nbz.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://tel.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://skx.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://zwm.yueranfly.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zyl.sysykeji.top

[U68] PHP：PDO 连接
来源：http://pmd.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://krd.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://vir.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mvy.ivvv.top

[U70] PHP：PDO 事务
来源：http://zrc.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yzb.yuanzhike.top

[U71] PHP：抛出异常
来源：http://jwz.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://pqf.fengsongda.top

[U72] PHP：写错误日志
来源：http://cbk.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://wjt.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://gks.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://awl.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://erv.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://ola.sxryk.cn

[U75] PHP：依赖注入
来源：http://ice.dashuyun.cn

composer require psr/container
来源：http://fjt.gogol.net.cn

[U76] PHP：简单路由
来源：http://efo.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uhx.jqgfzy.top

[U77] PHP：模板渲染
来源：http://iwn.tarul.cn

composer require twig/twig
来源：http://wup.yongpay.top

[U78] PHP：单元测试
来源：http://mph.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://znv.hnxiangtu.top

[U79] PHP：静态分析
来源：http://dov.svipenyu.cn

composer require --dev phpstan/phpstan
来源：http://tzs.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://ncd.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://bnk.tian-w.cn

[U81] JS：初始化项目
来源：http://nee.gogol.net.cn

npm init -y;  npm i express
来源：http://yjr.yuxming.cn

[U82] JS：package.json 脚本
来源：http://mua.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rpn.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://nfd.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mwh.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://sgs.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jcw.zhoulong.xyz

[U85] JS：可选链
来源：http://nxu.ctjpmb.com

a?.b?.c
来源：http://fhp.sweek.top

[U86] JS：空值合并
来源：http://cug.nanxinkj.top

a ?? b
来源：http://kia.zdqjudy.top

[U87] JS：解构默认值
来源：http://srz.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://btt.guowangkeji.top

[U88] JS：对象展开合并
来源：http://fjb.xinyue.icu

{ ...a, ...b }
来源：http://nsp.uphjek.com

[U89] JS：数组去重
来源：http://vos.zdbjq.cn

[...new Set(arr)]
来源：http://naa.chenzaomai.com

[U90] JS：数字数组排序
来源：http://kpy.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://xzv.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://tun.yongpay.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kgj.ehwqpu.com

[U92] JS：深拷贝
来源：http://jyf.feifeiyinyue.top

structuredClone(obj)
来源：http://xts.kuanghao11.cn

[U93] JS：模板字符串
来源：http://ees.aizwys.cn

`共 ${n} 条`
来源：http://shc.316326.xyz

[U94] JS：箭头函数
来源：http://mev.yongpay.top

const double = x => x * 2;
来源：http://tnh.ctjpmb.com

[U95] JS：Promise 包装
来源：http://dsu.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://bre.cucudq.cn

[U96] JS：async/await 与异常
来源：http://jwz.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vlg.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://jgy.mhx1999.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://piy.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://byp.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bck.nanxinkj.top

[U99] JS：事件监听
来源：http://ulf.xuanzx.com

el.addEventListener("click", e => {})
来源：http://lun.sxryk.cn

[U100] JS：DOM 查询
来源：http://gpa.shangyingyoupin.top

document.querySelector(".item")
来源：http://mbi.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://odu.havefunace.top

el.classList.toggle("active")
来源：http://iox.yongpay.top

[U102] JS：本地存储
来源：http://rho.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gdo.pycfn.com

[U103] JS：定时器
来源：http://wzd.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://unz.sxryk.cn

[U104] JS：防抖
来源：http://lbk.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eit.andypj.xyz

[U105] JS：节流
来源：http://kni.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtd.iojbl.cn

[U106] JS：日期格式化
来源：http://olt.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qyh.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://emw.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zzi.quarkkingdee.top

[U108] JS：随机整数
来源：http://bia.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ykt.cheryme.top

[U109] JS：数组分组
来源：http://nzm.zhoulong.xyz

Object.groupBy(arr, x => x.type)
来源：http://ozq.gzhubu.top

[U110] JS：数组分块
来源：http://zyw.jqgfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wxx.fengsongda.top

[U111] JS：对象转 Map
来源：http://oxc.zdqjudy.top

new Map(Object.entries(obj))
来源：http://gej.yueranfly.top

[U112] JS：字符串补位
来源：http://ujw.hammf.cn

"7".padStart(3, "0")
来源：http://src.fengsongda.top

[U113] JS：正则替换全部
来源：http://ggg.zhixingplan.top

s.replaceAll("a", "b")
来源：http://god.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://qdj.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tpy.sxryk.cn

[U115] JS：生成 UUID
来源：http://nhe.guowangkeji.top

crypto.randomUUID()
来源：http://xca.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://hif.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://xkg.guannengcc.top

[U117] JS：单元测试
来源：http://jqz.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://iew.zycfv.cn

[U118] JS：开发服务器
来源：http://hyh.cqqwz.cn

npm i -D vite;  npx vite
来源：http://lic.zdqjudy.top

[U119] JS：生产构建
来源：http://xms.bbcook.cn

npx vite build
来源：http://xky.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://ywp.iojbl.cn

import.meta.env.VITE_API_URL
来源：http://jpq.yuanzhike.top

================================================================================
来源：http://zwo.gogol.net.cn

统计汇总
来源：http://mzu.hnqzz.top

================================================================================
来源：http://nyx.yj202588.top

按语言统计（条）：
来源：http://guk.xinyue.icu

Python ......... 252
来源：http://rin.fktsv.cn

PHP ............ 252
来源：http://zmd.dianchejie.cn

JavaScript ..... 252
来源：http://gpu.cqqwz.cn

TypeScript ..... 212
来源：http://diz.zhengqikj.top

Java ........... 212
来源：http://uxr.ydzc1.top

Go ............. 212
来源：http://bjc.yuanzhike.top

Ruby ........... 212
来源：http://lxa.gogol.net.cn

C# ............. 212
来源：http://ngg.bbcook.cn

C .............. 30
来源：http://yvb.cashguo.top

C++ ............ 30
来源：http://ixf.yj20258888.top

SQL ............ 90
来源：http://vym.sweek.top

Bash ........... 80
来源：http://eun.cucudq.cn

Kotlin ......... 15
来源：http://bmy.dashuyun.cn

Swift .......... 15
来源：http://lwn.vqdsnc.cn

Lua ............ 10
来源：http://hym.guannengcc.top

Perl ........... 10
来源：http://cng.sufxvd.cn

Scala .......... 10
来源：http://yzx.redwolf501.top

------------------------------------
来源：http://fpu.jianghu66.top

合计 ........... 2106 条
来源：http://ijz.ivvv.top

按章节统计：
来源：http://vcj.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fdt.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ouz.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xjk.meibo888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kdq.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://osq.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lvi.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nxz.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://znf.c1oappe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zfb.zhiwuduotai.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://edx.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ihw.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cpu.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rlf.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eos.jyoumei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nfj.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pyv.zhongyouzk.top

Q SQL 专题                              90
来源：http://cma.svipenyu.cn

R Bash 专题                             80
来源：http://xpm.xziqi.cn

S C / C++ 专题                          60
来源：http://xvm.gzhubu.top

T 其他语言补充                          60
来源：http://vbc.yj20258888.top

U 高频实用片段                         120
来源：http://ymr.dashuyun.cn

------------------------------------
来源：http://ydm.bbcook.cn

合计                                  2106 条
来源：http://pei.yfazqb.com

--------------------------------------------------------------------------------
来源：http://yle.nwbrower.top

使用提醒
来源：http://hwk.ivvv.top

--------------------------------------------------------------------------------
来源：http://hdq.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gkc.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sdb.haohaochexian.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yby.gaohongyu789.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xan.hfpthk.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nft.0kj1m.cn

—— 文件结束 ——
来源：http://jpz.fktsv.cn

================================================================================
来源：http://lnq.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://yym.wangshuangyany.cn

Common Programming Examples Cheat Book
来源：http://sdo.zhengqikj.top

================================================================================
来源：http://bym.zdqjudy.top

【收录内容】
来源：http://wnn.jlsjyb.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xgr.gzhubu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dsp.smart0.xyz

SQL · Bash · C · C++
来源：http://tdp.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tch.ppjwa.cn

【使用说明】
来源：http://bcu.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sge.jqgufenzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vmq.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lcg.shangyingyoupin.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jio.yuanzhike.top

Bash:  Shell         C:     C             C++:   C++
来源：http://cge.yanxiufei.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://frg.daxiang520.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uol.svipenyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vcl.hysaishi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qab.zdqjudy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zim.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hpu.jianghu66.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fwx.epnwcf.com

【文件统计】
来源：http://pdj.hfpthk.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jvn.cashguo.top

--------------------------------------------------------------------------------
来源：http://zxs.ctjpmb.com

目  录
来源：http://iit.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://fvg.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://txn.uphjek.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://umn.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qru.shzxlz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://czx.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fpr.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rdm.daxiang520.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pmd.chenzaomai.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bhj.zycfv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fwa.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ssr.andypj.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tdn.ydzc1.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cmh.zdqjudy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vew.xuanzx.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oji.quarkkingdee.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qzh.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://daj.redwolf501.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kji.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://grd.gaohongyu789.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ydf.yuxming.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdt.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ktv.yj20258.top

================================================================================
来源：http://rut.aibaodan.cn

A. 基础语法与类型
来源：http://btf.ehwqpu.com

================================================================================
来源：http://lmw.sweek.top

[A01] Hello World
来源：http://tbd.9152youxi.cn

Py:   print("Hello, World!")
来源：http://kxv.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://pcq.snrcjt.cn

JS:   console.log("Hello, World!");
来源：http://nrk.hammf.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rwr.c1oappe.top


<!-- 参考信息 -->