代发 wailian999

[U25] Py：CSV 按字典读
来源：http://vky.chenjidiqi.icu

csv.DictReader(f)
来源：http://lyl.xinyue.icu

[U26] Py：并发下载
来源：http://hzn.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ysm.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://jdj.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://sjx.cucudq.cn

[U28] Py：类型别名
来源：http://kwf.nanxinkj.top

UserId = int
来源：http://epe.wangdashe.top

[U29] Py：属性校验
来源：http://nrp.yfazqb.com

@property 与 @x.setter 配合
来源：http://idv.smart0.xyz

[U30] Py：数据类
来源：http://izz.aizwys.cn

@dataclass(slots=True)
来源：http://jcu.yanxiufei.cn

[U31] Py：单测
来源：http://kbk.yangfankeji.com

python -m pytest -q
来源：http://pff.sjlbkw.cn

[U32] Py：代码格式化
来源：http://vvi.yj20258.top

ruff format . && ruff check --fix .
来源：http://uvu.gogol.net.cn

[U33] Py：打包发布
来源：http://xpd.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://qwz.xziqi.cn

[U34] Py：判断编码
来源：http://ocn.xziqi.cn

chardet.detect(raw)
来源：http://jxj.gaohongyu789.top

[U35] Py：发送邮件
来源：http://nnu.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zti.ydjk.org.cn

[U36] Py：定时任务
来源：http://rry.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://lrq.vehdjk.com

[U37] Py：读写 Excel
来源：http://crl.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://ewd.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://hhg.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://vlp.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://pgp.0kj1m.cn

sys.stdout.isatty()
来源：http://wzq.yonumen.top

[U40] Py：打印到标准错误
来源：http://dsc.bjfxy.top

print("err", file=sys.stderr)
来源：http://ikn.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://ccl.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tqq.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://fbb.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ivk.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://tqi.cheryme.top

namespace App\Http;
来源：http://hha.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://vkv.aizwys.cn

declare(strict_types=1);
来源：http://aff.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://vki.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://haj.gaohongyu789.top

[U46] PHP：可空类型
来源：http://jer.jinyuanbaomall.cn

?string $name = null
来源：http://hne.52xcode.cn

[U47] PHP：联合类型
来源：http://mtv.jiagoushi.top

int|string $id
来源：http://aff.birdmap.top

[U48] PHP：纯枚举
来源：http://ghc.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mtn.zdqjudy.top

[U49] PHP：只读属性
来源：http://ykn.jinyuanbaomall.cn

public readonly string $name
来源：http://wbg.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://dhs.xinyue.icu

public function __construct(private int $id) {}
来源：http://pxt.sysykeji.top

[U51] PHP：数组解构
来源：http://roj.xziqi.cn

[$a, $b] = $arr;
来源：http://qxp.zhijiandao.cn

[U52] PHP：箭头函数
来源：http://yuo.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://eej.yueranfly.top

[U53] PHP：空合并运算符
来源：http://hcx.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://uaa.xziqi.cn

[U54] PHP：空安全调用
来源：http://fiu.shuidangran.top

$obj?->method()
来源：http://gfk.tianlin.xyz

[U55] PHP：match 表达式
来源：http://dbr.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fxc.jqgufenzy.top

[U56] PHP：命名参数
来源：http://jjk.jinqigfzy.top

f(a: 1, b: 2)
来源：http://gby.xuanzx.com

[U57] PHP：字符串插值
来源：http://kyg.yonumen.top

"值: {$a}"
来源：http://sdo.jianghu66.top

[U58] PHP：数组三件套
来源：http://mxu.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jud.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://wdo.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhp.cashguo.top

[U60] PHP：JSON 编解码
来源：http://sxw.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mhm.guowangkeji.top

[U61] PHP：正则
来源：http://kkm.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gfm.fengsongda.top

[U62] PHP：日期对象
来源：http://pug.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nbz.yueranfly.top

[U63] PHP：文件读写
来源：http://jru.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://alq.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://clf.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://cgz.zhiwuduotai.top

[U65] PHP：会话
来源：http://pwy.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ssq.gaohongyu789.top

[U66] PHP：设置 Cookie
来源：http://wjh.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jte.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://vsv.yanxiufei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://edb.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://oto.epnwcf.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kgb.cucudq.cn

[U69] PHP：PDO 预处理
来源：http://juv.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jqu.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://tro.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eyt.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://cip.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://kip.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://izt.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://hqy.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://msf.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://pko.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://mlt.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://qad.jinqigufen.top

[U75] PHP：依赖注入
来源：http://any.shzxlz.cn

composer require psr/container
来源：http://xhl.sxryk.cn

[U76] PHP：简单路由
来源：http://frr.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iru.yangfankeji.com

[U77] PHP：模板渲染
来源：http://dkp.dashuyun.cn

composer require twig/twig
来源：http://dxh.birdmap.top

[U78] PHP：单元测试
来源：http://yxr.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://awq.tianlin.xyz

[U79] PHP：静态分析
来源：http://hcr.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://qca.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://rxv.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tny.zhoulong.xyz

[U81] JS：初始化项目
来源：http://tbr.shuidangran.top

npm init -y;  npm i express
来源：http://rqg.cucudq.cn

[U82] JS：package.json 脚本
来源：http://bek.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://khg.svipenyu.cn

[U83] JS：ES Module 导入导出
来源：http://bvm.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sxc.pycfn.com

[U84] JS：CommonJS 写法
来源：http://hxt.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nzt.uphjek.com

[U85] JS：可选链
来源：http://spc.bjfxy.top

a?.b?.c
来源：http://slk.zhengqikj.top

[U86] JS：空值合并
来源：http://orn.epnwcf.com

a ?? b
来源：http://tmr.zhoulong.xyz

[U87] JS：解构默认值
来源：http://kaz.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://sbp.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://cbq.tianlin.xyz

{ ...a, ...b }
来源：http://wcf.sxryk.cn

[U89] JS：数组去重
来源：http://gsd.yfazqb.com

[...new Set(arr)]
来源：http://ugg.tian-w.cn

[U90] JS：数字数组排序
来源：http://upc.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://cbq.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://kgo.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iep.jianghu66.top

[U92] JS：深拷贝
来源：http://ylt.xuanzx.com

structuredClone(obj)
来源：http://htn.hfpthk.cn

[U93] JS：模板字符串
来源：http://arf.yfazqb.com

`共 ${n} 条`
来源：http://rsu.svipenyu.cn

[U94] JS：箭头函数
来源：http://puu.shanyushiyangtech.top

const double = x => x * 2;
来源：http://rph.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://wog.cdnleiting.top

new Promise((resolve, reject) => {})
来源：http://pqk.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://ffu.hfpthk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pdq.pycfn.com

[U97] JS：并发请求
来源：http://wco.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tzv.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://rzm.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qvc.shangyingyoupin.top

[U99] JS：事件监听
来源：http://urg.jinyuanbaomall.cn

el.addEventListener("click", e => {})
来源：http://mfl.hywenlv.cn

[U100] JS：DOM 查询
来源：http://swj.dashuyun.cn

document.querySelector(".item")
来源：http://fve.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://iwi.quarkkingdee.top

el.classList.toggle("active")
来源：http://ruv.andypj.xyz

[U102] JS：本地存储
来源：http://udd.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rlk.9152youxi.cn

[U103] JS：定时器
来源：http://zvv.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://thx.havefunace.top

[U104] JS：防抖
来源：http://yvw.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgz.bjfxy.top

[U105] JS：节流
来源：http://vhg.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lbt.9152youxi.cn

[U106] JS：日期格式化
来源：http://sgj.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://khd.vehdjk.com

[U107] JS：数字千分位
来源：http://vlh.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ccy.chenjidiqi.icu

[U108] JS：随机整数
来源：http://tax.yuanzhike.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kkq.jinqigfzy.top

[U109] JS：数组分组
来源：http://wqe.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://ybd.cdnleiting.top

[U110] JS：数组分块
来源：http://lua.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vdh.fanxiaobao.xyz

[U111] JS：对象转 Map
来源：http://zbt.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://ast.ybcxt.top

[U112] JS：字符串补位
来源：http://zxg.jianghu66.top

"7".padStart(3, "0")
来源：http://eoj.sweek.top

[U113] JS：正则替换全部
来源：http://jap.chenlongwang.top

s.replaceAll("a", "b")
来源：http://fnp.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://pvl.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qha.jinqigufen.top

[U115] JS：生成 UUID
来源：http://lqf.pengpengdd.cyou

crypto.randomUUID()
来源：http://age.nanxuanxn.top

[U116] JS：类型检查（JSDoc）
来源：http://meo.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://lkr.haohaochexian.top

[U117] JS：单元测试
来源：http://azr.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://mqn.quarkkingdee.top

[U118] JS：开发服务器
来源：http://waf.ehwqpu.com

npm i -D vite;  npx vite
来源：http://akm.daria6918.cn

[U119] JS：生产构建
来源：http://pqy.mhx1999.top

npx vite build
来源：http://krn.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pzx.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://nfk.hnxiangtu.top

================================================================================
来源：http://mvs.nwbrower.top

统计汇总
来源：http://gsa.yangfankeji.com

================================================================================
来源：http://zfr.jqgfzy.top

按语言统计（条）：
来源：http://dpg.ehwqpu.com

Python ......... 252
来源：http://sjd.xingfuxueyuan.xyz

PHP ............ 252
来源：http://sdm.0kj1m.cn

JavaScript ..... 252
来源：http://dfi.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://fer.ppjwa.cn

Java ........... 212
来源：http://uca.bjfxy.top

Go ............. 212
来源：http://raf.nanxuanxn.top

Ruby ........... 212
来源：http://jzm.52xcode.cn

C# ............. 212
来源：http://jbb.bjfxy.top

C .............. 30
来源：http://yit.guowangkeji.top

C++ ............ 30
来源：http://hnd.shuidangran.top

SQL ............ 90
来源：http://tub.jinqigfzy.top

Bash ........... 80
来源：http://lxh.zhijiandao.cn

Kotlin ......... 15
来源：http://miy.ydjk.org.cn

Swift .......... 15
来源：http://tsb.wangshuangyany.cn

Lua ............ 10
来源：http://teb.jinyuanbaomall.cn

Perl ........... 10
来源：http://qub.9152youxi.cn

Scala .......... 10
来源：http://mfj.andypj.xyz

------------------------------------
来源：http://rxn.zhiwuduotai.top

合计 ........... 2106 条
来源：http://ykl.xziqi.cn

按章节统计：
来源：http://yhe.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cki.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zam.chenzaomai.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xbl.chenzaomai.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://spi.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://snr.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ggo.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gvn.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oug.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://olu.daria6918.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://efq.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jbf.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gpm.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fco.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vsm.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jio.xinyue.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zfo.jqgfzy.top

Q SQL 专题                              90
来源：http://ins.fanxiaobao.xyz

R Bash 专题                             80
来源：http://cfw.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://daa.andypj.xyz

T 其他语言补充                          60
来源：http://wmw.havefunace.top

U 高频实用片段                         120
来源：http://wtw.andypj.xyz

------------------------------------
来源：http://aeo.quarkkingdee.top

合计                                  2106 条
来源：http://xhh.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ghr.yj20258888.top

使用提醒
来源：http://kfg.uphjek.com

--------------------------------------------------------------------------------
来源：http://nsk.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gzc.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zbd.shzxlz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vww.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://bpa.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xal.kuanghao11.cn

—— 文件结束 ——
来源：http://jin.bbcook.cn

================================================================================
来源：http://qxx.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://pfz.xinyue.icu

Common Programming Examples Cheat Book
来源：http://kry.bbcook.cn

================================================================================
来源：http://myy.jinghuilouyu.cn

【收录内容】
来源：http://xvh.daria6918.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jji.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://crx.ybcxt.top

SQL · Bash · C · C++
来源：http://rou.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sxl.cucudq.cn

【使用说明】
来源：http://xwu.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lbz.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ete.ybcxt.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fbn.yangfankeji.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wbf.jlsjyb.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yhv.guowangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fek.chenzaomai.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sti.jinghuilouyu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://una.daxiang520.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vxv.jinyuanbaomall.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rod.jqgufenzy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tjg.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mga.ctjpmb.com

【文件统计】
来源：http://dfw.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kpa.fengsongda.top

--------------------------------------------------------------------------------
来源：http://xia.nanxuanxn.top

目  录
来源：http://hkh.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://njz.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pnn.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nni.xuanzx.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://adq.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yky.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mrr.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dxt.c1oappe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zhe.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fqz.shanyushiyangtech.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ecs.wangshuangyany.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ioz.ctjpmb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://krk.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://onu.hcnkem.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vqg.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vei.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uts.hesvh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mdx.zhiwuduotai.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uye.nanxuanxn.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://rlx.yongpay.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://csm.sxryk.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tzw.xinyue.icu

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uom.xziqi.cn

================================================================================
来源：http://qvt.chenjidiqi.icu

A. 基础语法与类型
来源：http://exj.shangyingyoupin.top

================================================================================
来源：http://uhf.ivvv.top

[A01] Hello World
来源：http://ptr.epnwcf.com


<!-- 参考信息 -->