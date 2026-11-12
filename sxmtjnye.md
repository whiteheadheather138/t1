代发 wailian999

[U25] Py：CSV 按字典读
来源：http://fmp.daxiang520.top

csv.DictReader(f)
来源：http://gpo.yanxiufei.cn

[U26] Py：并发下载
来源：http://huo.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tld.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://bqd.gaohongyu789.top

aiohttp.ClientSession() 配合 async with
来源：http://qfc.bjfxy.top

[U28] Py：类型别名
来源：http://ojw.xziqi.cn

UserId = int
来源：http://nuq.aizwys.cn

[U29] Py：属性校验
来源：http://kwm.sufxvd.cn

@property 与 @x.setter 配合
来源：http://oso.bjfxy.top

[U30] Py：数据类
来源：http://jzf.ehwqpu.com

@dataclass(slots=True)
来源：http://gkf.havefunace.top

[U31] Py：单测
来源：http://kxo.aibaodan.cn

python -m pytest -q
来源：http://cvn.guannengcc.top

[U32] Py：代码格式化
来源：http://muf.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://xrn.gzhubu.top

[U33] Py：打包发布
来源：http://kpv.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://ebm.feifeiyinyue.top

[U34] Py：判断编码
来源：http://uej.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://elf.jinqigufen.top

[U35] Py：发送邮件
来源：http://vaw.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ywq.svipenyu.cn

[U36] Py：定时任务
来源：http://zfh.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://geu.yangfankeji.com

[U37] Py：读写 Excel
来源：http://rqk.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://kpy.cqqwz.cn

[U38] Py：获取脚本所在目录
来源：http://cnz.guannengcc.top

Path(__file__).resolve().parent
来源：http://gsh.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://rex.fengsongda.top

sys.stdout.isatty()
来源：http://yvb.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://teu.9152youxi.cn

print("err", file=sys.stderr)
来源：http://kas.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://klz.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gzq.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://sga.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eru.cashguo.top

[U43] PHP：声明命名空间
来源：http://oos.gotoacloud.top

namespace App\Http;
来源：http://bhe.yongpay.top

[U44] PHP：开启严格类型
来源：http://smb.iojbl.cn

declare(strict_types=1);
来源：http://zyk.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://azt.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xhj.52xcode.cn

[U46] PHP：可空类型
来源：http://xrm.zdbjq.cn

?string $name = null
来源：http://bht.fehbvm.com

[U47] PHP：联合类型
来源：http://sft.0kj1m.cn

int|string $id
来源：http://zea.jlsjyb.cn

[U48] PHP：纯枚举
来源：http://yno.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvf.zdqjudy.top

[U49] PHP：只读属性
来源：http://vom.yj20258.top

public readonly string $name
来源：http://ovu.tanke756.top

[U50] PHP：构造器属性提升
来源：http://vov.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://bwp.shzxlz.cn

[U51] PHP：数组解构
来源：http://kys.yj20258.top

[$a, $b] = $arr;
来源：http://lmw.316326.xyz

[U52] PHP：箭头函数
来源：http://dkw.yj20258.top

$double = fn($x) => $x * 2;
来源：http://mkj.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://dap.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://rsw.0kj1m.cn

[U54] PHP：空安全调用
来源：http://tup.yj202588.top

$obj?->method()
来源：http://lhe.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://ild.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gic.hywenlv.cn

[U56] PHP：命名参数
来源：http://mhr.uphjek.com

f(a: 1, b: 2)
来源：http://qpd.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://ujc.sxryk.cn

"值: {$a}"
来源：http://lgq.yuxming.cn

[U58] PHP：数组三件套
来源：http://put.cashguo.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vae.sufxvd.cn

[U59] PHP：自定义排序
来源：http://zoc.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://znx.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://cwg.tarul.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pmz.yj202588.top

[U61] PHP：正则
来源：http://owi.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://usa.zhijiandao.cn

[U62] PHP：日期对象
来源：http://cvw.bjfxy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nyj.jqgfzy.top

[U63] PHP：文件读写
来源：http://tri.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mjj.fzhhl.top

[U64] PHP：目录遍历
来源：http://xjp.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://bvg.bjfxy.top

[U65] PHP：会话
来源：http://cdj.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rvc.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://axo.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oem.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://vkc.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lvq.smart0.xyz

[U68] PHP：PDO 连接
来源：http://vyj.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sge.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://wma.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zmb.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://rnu.ivvv.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nsa.jyoumei.cn

[U71] PHP：抛出异常
来源：http://tkp.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://xwl.aibaodan.cn

[U72] PHP：写错误日志
来源：http://bmb.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://zuv.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://kzr.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://kpo.fengsongda.top

[U74] PHP：读取环境变量
来源：http://cnv.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://yzv.zdqjudy.top

[U75] PHP：依赖注入
来源：http://uvj.iojbl.cn

composer require psr/container
来源：http://rkd.zhixingplan.top

[U76] PHP：简单路由
来源：http://dca.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rew.uphjek.com

[U77] PHP：模板渲染
来源：http://jvz.hesvh.cn

composer require twig/twig
来源：http://nbu.tarul.cn

[U78] PHP：单元测试
来源：http://ccd.ivvv.top

composer require --dev phpunit/phpunit
来源：http://oqv.sxryk.cn

[U79] PHP：静态分析
来源：http://wap.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://dus.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://gqu.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ese.shanyushiyangkeji.top

[U81] JS：初始化项目
来源：http://vzb.uphjek.com

npm init -y;  npm i express
来源：http://nmn.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://fea.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dwz.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://uob.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://lzh.cucudq.cn

[U84] JS：CommonJS 写法
来源：http://xln.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://kym.tarul.cn

[U85] JS：可选链
来源：http://ble.ydjk.org.cn

a?.b?.c
来源：http://vvn.aibaodan.cn

[U86] JS：空值合并
来源：http://zjz.uphjek.com

a ?? b
来源：http://iiu.jinqigfzy.top

[U87] JS：解构默认值
来源：http://yhc.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://bjh.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://tni.xziqi.cn

{ ...a, ...b }
来源：http://bwv.cdnleiting.top

[U89] JS：数组去重
来源：http://ejg.yuxming.cn

[...new Set(arr)]
来源：http://fri.zdbjq.cn

[U90] JS：数字数组排序
来源：http://tgx.gzhubu.top

[...arr].sort((a, b) => a - b)
来源：http://wdf.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://yox.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ict.sweek.top

[U92] JS：深拷贝
来源：http://ynx.cashguo.top

structuredClone(obj)
来源：http://bkh.sufxvd.cn

[U93] JS：模板字符串
来源：http://xqo.fanxiaobao.xyz

`共 ${n} 条`
来源：http://xso.ctjpmb.com

[U94] JS：箭头函数
来源：http://has.hysaishi.cn

const double = x => x * 2;
来源：http://srt.ehwqpu.com

[U95] JS：Promise 包装
来源：http://mog.dashuyun.cn

new Promise((resolve, reject) => {})
来源：http://jph.bjfxy.top

[U96] JS：async/await 与异常
来源：http://goj.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ola.meibo888.top

[U97] JS：并发请求
来源：http://swe.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mbv.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://qnc.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gpb.316326.xyz

[U99] JS：事件监听
来源：http://akm.cheryme.top

el.addEventListener("click", e => {})
来源：http://pav.nwbrower.top

[U100] JS：DOM 查询
来源：http://wds.hnxiangtu.top

document.querySelector(".item")
来源：http://tnp.vehdjk.com

[U101] JS：classList 操作
来源：http://air.zhiwuduotai.top

el.classList.toggle("active")
来源：http://czd.ydzc1.top

[U102] JS：本地存储
来源：http://pjt.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://awu.yanxiufei.cn

[U103] JS：定时器
来源：http://lsm.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eya.sjlbkw.cn

[U104] JS：防抖
来源：http://jda.pengpengdd.cyou

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nnw.meibo888.top

[U105] JS：节流
来源：http://ptc.sweek.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dfo.gogol.net.cn

[U106] JS：日期格式化
来源：http://sxk.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iob.cheryme.top

[U107] JS：数字千分位
来源：http://ele.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://viy.yueranfly.top

[U108] JS：随机整数
来源：http://jql.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nvl.ybcxt.top

[U109] JS：数组分组
来源：http://tjy.snrcjt.cn

Object.groupBy(arr, x => x.type)
来源：http://kpq.ehwqpu.com

[U110] JS：数组分块
来源：http://iza.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bja.zdbjq.cn

[U111] JS：对象转 Map
来源：http://qre.bjfxy.top

new Map(Object.entries(obj))
来源：http://shx.cdnleiting.top

[U112] JS：字符串补位
来源：http://qbz.bjfxy.top

"7".padStart(3, "0")
来源：http://uan.sysykeji.top

[U113] JS：正则替换全部
来源：http://wnp.nwbrower.top

s.replaceAll("a", "b")
来源：http://cig.jyoumei.cn

[U114] JS：JSON 深比较
来源：http://xsp.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dqw.yuxming.cn

[U115] JS：生成 UUID
来源：http://kvq.bbcook.cn

crypto.randomUUID()
来源：http://qtg.sjlbkw.cn

[U116] JS：类型检查（JSDoc）
来源：http://hzm.jqgufenzy.top

/** @param {string} name */ function f(name) {}
来源：http://vxh.yj202588.top

[U117] JS：单元测试
来源：http://wjb.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://csc.nwbrower.top

[U118] JS：开发服务器
来源：http://ajq.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://smo.yuxming.cn

[U119] JS：生产构建
来源：http://jvl.zhaomingkeji.xyz

npx vite build
来源：http://akx.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://xmr.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://mrz.gogol.net.cn

================================================================================
来源：http://msq.yongpay.top

统计汇总
来源：http://vai.zhongyouzk.top

================================================================================
来源：http://fdj.feifeiyinyue.top

按语言统计（条）：
来源：http://vbp.epnwcf.com

Python ......... 252
来源：http://xlt.cqqwz.cn

PHP ............ 252
来源：http://mfh.hammf.cn

JavaScript ..... 252
来源：http://vyd.yonumen.top

TypeScript ..... 212
来源：http://ijl.fzhhl.top

Java ........... 212
来源：http://sug.fzhhl.top

Go ............. 212
来源：http://jzr.yuanzhike.top

Ruby ........... 212
来源：http://lrh.gzhubu.top

C# ............. 212
来源：http://tcz.zhongyouzk.top

C .............. 30
来源：http://hgd.iojbl.cn

C++ ............ 30
来源：http://sbc.shuidangran.top

SQL ............ 90
来源：http://mvv.smart0.xyz

Bash ........... 80
来源：http://vce.hnqzz.top

Kotlin ......... 15
来源：http://oss.nanxinkj.top

Swift .......... 15
来源：http://tdq.316326.xyz

Lua ............ 10
来源：http://ygt.guannengcc.top

Perl ........... 10
来源：http://tos.jinyuanbaomall.cn

Scala .......... 10
来源：http://vrg.tianlin.xyz

------------------------------------
来源：http://mrd.shzxlz.cn

合计 ........... 2106 条
来源：http://vug.fanxiaobao.xyz

按章节统计：
来源：http://gju.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://eno.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://muy.haohaochexian.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://etq.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sev.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cyp.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ogk.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ngy.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cig.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wtb.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iri.meibo888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nxo.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bem.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pal.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jhg.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ktb.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cji.uphjek.com

Q SQL 专题                              90
来源：http://nqh.chenzaomai.com

R Bash 专题                             80
来源：http://fny.pengpengdd.cyou

S C / C++ 专题                          60
来源：http://vuv.zhiwuduotai.top

T 其他语言补充                          60
来源：http://bnt.zhongyouzk.top

U 高频实用片段                         120
来源：http://orv.uphjek.com

------------------------------------
来源：http://hvg.gaohongyu789.top

合计                                  2106 条
来源：http://age.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://mzk.jlsjyb.cn

使用提醒
来源：http://fzb.yj202588.top

--------------------------------------------------------------------------------
来源：http://pgh.feifeiyinyue.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rom.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://czz.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fll.birdmap.top

在旧版本上使用前请先确认语法支持情况。
来源：http://adz.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xka.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://uzl.uphjek.com

================================================================================
来源：http://yir.zhengqikj.top

程序语言常见例子速查手册（2024 版）
来源：http://qpx.guannengcc.top

Common Programming Examples Cheat Book
来源：http://sdd.yongpay.top

================================================================================
来源：http://odz.ctjpmb.com

【收录内容】
来源：http://ayv.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lpp.shangyingyoupin.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uex.pycfn.com

SQL · Bash · C · C++
来源：http://qcd.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://juw.hywenlv.cn

【使用说明】
来源：http://wid.yueranfly.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://uyh.zhaomingkeji.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xvj.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kup.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fph.yfazqb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://lvr.meibo888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yvn.chenlongwang.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bdm.yfazqb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lhg.ehwqpu.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aaw.jqgufenzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://voq.cucudq.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://krd.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kxb.xinyue.icu

【文件统计】
来源：http://huv.jqgufenzy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://srz.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://ija.quarkkingdee.top

目  录
来源：http://ojh.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://dbh.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ohx.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ksi.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fdd.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lar.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nzz.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fxt.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://prw.hfpthk.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://apd.haohaochexian.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yvr.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gce.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nbr.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iig.guowangkeji.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ygi.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nds.zhengqikj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hfz.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vaw.gogol.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rbx.chenjidiqi.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://lxv.shanyushiyangtech.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ivn.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dvx.ivvv.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://eut.jinyuanbaomall.cn

================================================================================
来源：http://yju.52xcode.cn

A. 基础语法与类型
来源：http://nzm.kuanghao11.cn

================================================================================
来源：http://mmb.cqqwz.cn

[A01] Hello World
来源：http://spx.yangfankeji.com


<!-- 参考信息 -->