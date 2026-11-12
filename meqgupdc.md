代发 wailian999

[U27] Py：异步 HTTP
来源：http://gpv.cqqwz.cn

aiohttp.ClientSession() 配合 async with
来源：http://nfc.zhixingplan.top

[U28] Py：类型别名
来源：http://noe.gaohongyu789.top

UserId = int
来源：http://gvr.cdnleiting.top

[U29] Py：属性校验
来源：http://zeo.cheryme.top

@property 与 @x.setter 配合
来源：http://dnk.ivvv.top

[U30] Py：数据类
来源：http://anp.ydzc1.top

@dataclass(slots=True)
来源：http://ywg.yj20258888.top

[U31] Py：单测
来源：http://epb.tianlin.xyz

python -m pytest -q
来源：http://xnx.gogol.net.cn

[U32] Py：代码格式化
来源：http://gsr.ydzc1.top

ruff format . && ruff check --fix .
来源：http://tyn.wangdashe.top

[U33] Py：打包发布
来源：http://zau.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://kkr.shzxlz.cn

[U34] Py：判断编码
来源：http://jzk.fanxiaobao.xyz

chardet.detect(raw)
来源：http://bkx.hywenlv.cn

[U35] Py：发送邮件
来源：http://lgx.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rlq.xuetiantiany.cn

[U36] Py：定时任务
来源：http://vmc.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://gxq.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://ezr.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://jaa.jqgfzy.top

[U38] Py：获取脚本所在目录
来源：http://oix.shuidangran.top

Path(__file__).resolve().parent
来源：http://yxb.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://upl.zhengqikj.top

sys.stdout.isatty()
来源：http://cks.uphjek.com

[U40] Py：打印到标准错误
来源：http://dum.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://caj.yj20258.top

[U41] PHP：初始化 Composer 项目
来源：http://kvb.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://prj.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://fbc.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gew.shangyingyoupin.top

[U43] PHP：声明命名空间
来源：http://fme.yueranfly.top

namespace App\Http;
来源：http://xww.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://qij.zhijiandao.cn

declare(strict_types=1);
来源：http://oxx.zhixingplan.top

[U45] PHP：类型声明与返回类型
来源：http://qem.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rke.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://qsz.zdqjudy.top

?string $name = null
来源：http://xfg.sjlbkw.cn

[U47] PHP：联合类型
来源：http://iwv.andypj.xyz

int|string $id
来源：http://mbe.yueranfly.top

[U48] PHP：纯枚举
来源：http://hko.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vnq.yj20258888.top

[U49] PHP：只读属性
来源：http://kuf.epnwcf.com

public readonly string $name
来源：http://gbo.yonumen.top

[U50] PHP：构造器属性提升
来源：http://pra.sxryk.cn

public function __construct(private int $id) {}
来源：http://cmp.birdmap.top

[U51] PHP：数组解构
来源：http://qzz.tian-w.cn

[$a, $b] = $arr;
来源：http://auu.tarul.cn

[U52] PHP：箭头函数
来源：http://bch.yj202588.top

$double = fn($x) => $x * 2;
来源：http://dcc.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://pbm.hesvh.cn

$v = $a ?? $b ?? "default";
来源：http://svp.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://wih.zhijiandao.cn

$obj?->method()
来源：http://gfo.pycfn.com

[U55] PHP：match 表达式
来源：http://nyo.tanke756.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gfh.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://sex.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://aoo.zdqjudy.top

[U57] PHP：字符串插值
来源：http://eba.xziqi.cn

"值: {$a}"
来源：http://pda.xuanzx.com

[U58] PHP：数组三件套
来源：http://etf.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rbr.316326.xyz

[U59] PHP：自定义排序
来源：http://pnw.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ocw.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://qko.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nrx.gaohongyu789.top

[U61] PHP：正则
来源：http://iic.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://akh.9152youxi.cn

[U62] PHP：日期对象
来源：http://bda.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://arl.chenlongwang.top

[U63] PHP：文件读写
来源：http://icd.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xpl.0kj1m.cn

[U64] PHP：目录遍历
来源：http://ewd.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://amr.bbcook.cn

[U65] PHP：会话
来源：http://edr.chenjidiqi.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://uag.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://upw.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://quf.mhx1999.top

[U67] PHP：处理文件上传
来源：http://qlj.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nzo.andypj.xyz

[U68] PHP：PDO 连接
来源：http://juk.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dka.yongpay.top

[U69] PHP：PDO 预处理
来源：http://aip.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vnn.tanke756.top

[U70] PHP：PDO 事务
来源：http://ojj.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qwx.nanxinkj.top

[U71] PHP：抛出异常
来源：http://ffs.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://oer.guannengcc.top

[U72] PHP：写错误日志
来源：http://cip.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://uyo.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://myk.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://ead.ppjwa.cn

[U74] PHP：读取环境变量
来源：http://bpm.cdnleiting.top

getenv("APP_ENV") ?: "production"
来源：http://xlq.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://dmr.hfpthk.cn

composer require psr/container
来源：http://vks.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://mtb.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://csq.xziqi.cn

[U77] PHP：模板渲染
来源：http://mgx.cheryme.top

composer require twig/twig
来源：http://pdx.hcnkem.com

[U78] PHP：单元测试
来源：http://nbs.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://uqx.vehdjk.com

[U79] PHP：静态分析
来源：http://kcc.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://ipv.xinyue.icu

[U80] PHP：代码规范修复
来源：http://kut.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qub.tarul.cn

[U81] JS：初始化项目
来源：http://fmh.ivvv.top

npm init -y;  npm i express
来源：http://cej.hesvh.cn

[U82] JS：package.json 脚本
来源：http://kdu.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kua.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://eiq.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://fra.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://bwt.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://hkm.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://kvk.ppjwa.cn

a?.b?.c
来源：http://byi.guannengcc.top

[U86] JS：空值合并
来源：http://xnj.ctjpmb.com

a ?? b
来源：http://vij.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://irw.hnqzz.top

const { a = 1, b = 2 } = obj;
来源：http://exe.yueranfly.top

[U88] JS：对象展开合并
来源：http://vps.snrcjt.cn

{ ...a, ...b }
来源：http://gge.yuxming.cn

[U89] JS：数组去重
来源：http://wky.ybcxt.top

[...new Set(arr)]
来源：http://ojf.fzhhl.top

[U90] JS：数字数组排序
来源：http://okz.sysykeji.top

[...arr].sort((a, b) => a - b)
来源：http://mav.yongpay.top

[U91] JS：对象键值遍历
来源：http://ljn.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ucq.yuanzhike.top

[U92] JS：深拷贝
来源：http://keo.jiagoushi.top

structuredClone(obj)
来源：http://luy.meibo888.top

[U93] JS：模板字符串
来源：http://yhx.yj202588.top

`共 ${n} 条`
来源：http://sys.jinqigfzy.top

[U94] JS：箭头函数
来源：http://rmv.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://qvy.aizwys.cn

[U95] JS：Promise 包装
来源：http://nmi.yj202588.top

new Promise((resolve, reject) => {})
来源：http://rjd.ydzc1.top

[U96] JS：async/await 与异常
来源：http://jut.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yig.fehbvm.com

[U97] JS：并发请求
来源：http://uff.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hgx.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://iwa.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vyf.zhoulong.xyz

[U99] JS：事件监听
来源：http://pfe.wangshuangyany.cn

el.addEventListener("click", e => {})
来源：http://vll.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://agy.hongshengwenyu.top

document.querySelector(".item")
来源：http://yym.nwbrower.top

[U101] JS：classList 操作
来源：http://gqh.yfazqb.com

el.classList.toggle("active")
来源：http://vrv.xziqi.cn

[U102] JS：本地存储
来源：http://ttk.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://yow.nwbrower.top

[U103] JS：定时器
来源：http://uyn.jinqigufen.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://krz.hnqzz.top

[U104] JS：防抖
来源：http://les.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htl.vqdsnc.cn

[U105] JS：节流
来源：http://ybm.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zgk.zdbjq.cn

[U106] JS：日期格式化
来源：http://sqk.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yrp.xziqi.cn

[U107] JS：数字千分位
来源：http://yzq.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xtg.chenjidiqi.icu

[U108] JS：随机整数
来源：http://yta.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://azz.sysykeji.top

[U109] JS：数组分组
来源：http://xgt.zycfv.cn

Object.groupBy(arr, x => x.type)
来源：http://wru.yj202588.top

[U110] JS：数组分块
来源：http://ymb.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cmt.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://zdp.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://npw.jiagoushi.top

[U112] JS：字符串补位
来源：http://pxx.hnqzz.top

"7".padStart(3, "0")
来源：http://kei.bbcook.cn

[U113] JS：正则替换全部
来源：http://lpn.hywenlv.cn

s.replaceAll("a", "b")
来源：http://ajm.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://deo.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kqg.hcnkem.com

[U115] JS：生成 UUID
来源：http://ttu.sxryk.cn

crypto.randomUUID()
来源：http://pby.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://hoe.zycfv.cn

/** @param {string} name */ function f(name) {}
来源：http://vrg.cheryme.top

[U117] JS：单元测试
来源：http://mns.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://qfs.jinqigufen.top

[U118] JS：开发服务器
来源：http://djo.ctjpmb.com

npm i -D vite;  npx vite
来源：http://xvx.jqgfzy.top

[U119] JS：生产构建
来源：http://irl.haohaochexian.top

npx vite build
来源：http://hth.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://ksp.cheryme.top

import.meta.env.VITE_API_URL
来源：http://ahq.yongpay.top

================================================================================
来源：http://uys.ivvv.top

统计汇总
来源：http://igh.jqgufenzy.top

================================================================================
来源：http://dty.zhiwuduotai.top

按语言统计（条）：
来源：http://jqf.jlsjyb.cn

Python ......... 252
来源：http://igs.quarkkingdee.top

PHP ............ 252
来源：http://cix.ehwqpu.com

JavaScript ..... 252
来源：http://ena.sweek.top

TypeScript ..... 212
来源：http://bvc.52xcode.cn

Java ........... 212
来源：http://jns.fzhhl.top

Go ............. 212
来源：http://ckk.zhixingplan.top

Ruby ........... 212
来源：http://eko.zycfv.cn

C# ............. 212
来源：http://vyl.guowangkeji.top

C .............. 30
来源：http://lqq.fzhhl.top

C++ ............ 30
来源：http://kax.ydzc1.top

SQL ............ 90
来源：http://jyv.fanxiaobao.xyz

Bash ........... 80
来源：http://kta.svipenyu.cn

Kotlin ......... 15
来源：http://lzi.xylfe.cn

Swift .......... 15
来源：http://qvu.ydjk.org.cn

Lua ............ 10
来源：http://gjk.ivvv.top

Perl ........... 10
来源：http://jzg.meibo888.top

Scala .......... 10
来源：http://aen.kuanghao11.cn

------------------------------------
来源：http://ium.zhixingplan.top

合计 ........... 2106 条
来源：http://zpq.hfpthk.cn

按章节统计：
来源：http://fku.zhixingplan.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ajl.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uev.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xos.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xtz.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ktq.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://opo.hesvh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ynv.guannengcc.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xdr.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lml.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pbs.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nhc.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sew.ivvv.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sdb.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rdd.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qsm.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kug.hfpthk.cn

Q SQL 专题                              90
来源：http://qsb.aizwys.cn

R Bash 专题                             80
来源：http://bcm.smart0.xyz

S C / C++ 专题                          60
来源：http://ipa.smart0.xyz

T 其他语言补充                          60
来源：http://ztt.hfpthk.cn

U 高频实用片段                         120
来源：http://rft.gogol.net.cn

------------------------------------
来源：http://lxw.yangfankeji.com

合计                                  2106 条
来源：http://nix.xuanzx.com

--------------------------------------------------------------------------------
来源：http://jiz.pycfn.com

使用提醒
来源：http://jvd.xziqi.cn

--------------------------------------------------------------------------------
来源：http://lai.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lzb.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://skn.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kks.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://dkl.ydzc1.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://han.fzhhl.top

—— 文件结束 ——
来源：http://nnr.uphjek.com

================================================================================
来源：http://ola.chenjidiqi.icu

程序语言常见例子速查手册（2024 版）
来源：http://qnz.xuanzx.com

Common Programming Examples Cheat Book
来源：http://qgg.guowangkeji.top

================================================================================
来源：http://eny.jqgfzy.top

【收录内容】
来源：http://dpx.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gez.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rxf.ybcxt.top

SQL · Bash · C · C++
来源：http://wto.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rfl.zhiwuduotai.top

【使用说明】
来源：http://nza.svipenyu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://swl.hongshengwenyu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wjw.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://osm.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://efd.dashuyun.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rql.zhaomingkeji.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tqw.gogol.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://azy.yanxiufei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixk.xuetiantiany.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xhp.cucudq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nem.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ceg.pengpengdd.cyou

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jzz.birdmap.top

【文件统计】
来源：http://mvt.hcnkem.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cjc.redwolf501.top

--------------------------------------------------------------------------------
来源：http://ekl.sjlbkw.cn

目  录
来源：http://efr.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://etq.guannengcc.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wnq.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://psd.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pqr.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://haa.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wef.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ecm.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nle.sysykeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://khm.yueranfly.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dgg.ctjpmb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lsg.jqgfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ede.ctjpmb.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://twh.kuanghao11.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vgh.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dgh.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pnr.pycfn.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://atq.birdmap.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qqy.yuanzhike.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mpo.cqqwz.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mxb.zhijiandao.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxc.zhiwuduotai.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kns.havefunace.top

================================================================================
来源：http://wov.ivvv.top

A. 基础语法与类型
来源：http://oed.sysykeji.top

================================================================================
来源：http://tbc.bbcook.cn

[A01] Hello World
来源：http://phv.cdnleiting.top

Py:   print("Hello, World!")
来源：http://aso.shanyushiyangkeji.top

PHP:  echo "Hello, World!";
来源：http://auf.9152youxi.cn

JS:   console.log("Hello, World!");
来源：http://niw.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://euu.yuxming.cn


<!-- 参考信息 -->