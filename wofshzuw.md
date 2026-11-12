代发 wailian999

[U19] Py：正则替换带回调
来源：http://euj.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bio.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://szs.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://nfr.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://pri.yueranfly.top

@contextlib.contextmanager
来源：http://gez.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://qcy.pengpengdd.cyou

list(zip(*m))
来源：http://aca.shuidangran.top

[U23] Py：分块读取大文件
来源：http://kik.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iim.yj202588.top

[U24] Py：路径操作
来源：http://quy.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://waz.uphjek.com

[U25] Py：CSV 按字典读
来源：http://dod.hesvh.cn

csv.DictReader(f)
来源：http://dnx.hesvh.cn

[U26] Py：并发下载
来源：http://lke.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kav.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://axh.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://wuq.redwolf501.top

[U28] Py：类型别名
来源：http://sza.jyoumei.cn

UserId = int
来源：http://bcl.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://buw.yonumen.top

@property 与 @x.setter 配合
来源：http://pej.zhongyouzk.top

[U30] Py：数据类
来源：http://ygb.tarul.cn

@dataclass(slots=True)
来源：http://zaj.andypj.xyz

[U31] Py：单测
来源：http://ysl.epnwcf.com

python -m pytest -q
来源：http://gkn.nanxinkj.top

[U32] Py：代码格式化
来源：http://dls.mhx1999.top

ruff format . && ruff check --fix .
来源：http://see.sxryk.cn

[U33] Py：打包发布
来源：http://afv.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://zea.cheryme.top

[U34] Py：判断编码
来源：http://qlv.dianchejie.cn

chardet.detect(raw)
来源：http://hxy.hesvh.cn

[U35] Py：发送邮件
来源：http://tks.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qqn.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://gox.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://frn.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://twr.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vfk.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://zlv.meibo888.top

Path(__file__).resolve().parent
来源：http://sog.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://lpf.daxiang520.top

sys.stdout.isatty()
来源：http://pzp.sxryk.cn

[U40] Py：打印到标准错误
来源：http://kro.ctjpmb.com

print("err", file=sys.stderr)
来源：http://pvx.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://qus.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gqu.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://reh.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fge.birdmap.top

[U43] PHP：声明命名空间
来源：http://fwf.yj20258888.top

namespace App\Http;
来源：http://ptq.guannengcc.top

[U44] PHP：开启严格类型
来源：http://bim.guowangkeji.top

declare(strict_types=1);
来源：http://hae.hammf.cn

[U45] PHP：类型声明与返回类型
来源：http://koq.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://lfd.ydzc1.top

[U46] PHP：可空类型
来源：http://kbd.uphjek.com

?string $name = null
来源：http://idd.hysaishi.cn

[U47] PHP：联合类型
来源：http://imh.xuanzx.com

int|string $id
来源：http://mpx.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://pdq.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mqc.wangdashe.top

[U49] PHP：只读属性
来源：http://ehs.ppjwa.cn

public readonly string $name
来源：http://dlm.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://npp.chenlongwang.top

public function __construct(private int $id) {}
来源：http://bfd.cheryme.top

[U51] PHP：数组解构
来源：http://yui.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://tzf.pycfn.com

[U52] PHP：箭头函数
来源：http://wyc.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://uob.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://trh.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://iqx.aibaodan.cn

[U54] PHP：空安全调用
来源：http://ksj.sweek.top

$obj?->method()
来源：http://stq.fktsv.cn

[U55] PHP：match 表达式
来源：http://ksl.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zhy.c1oappe.top

[U56] PHP：命名参数
来源：http://grm.shanyushiyangtech.top

f(a: 1, b: 2)
来源：http://kib.tanke756.top

[U57] PHP：字符串插值
来源：http://yjd.fktsv.cn

"值: {$a}"
来源：http://llb.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://xzd.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sdi.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://coh.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://muw.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://evq.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://etf.dashuyun.cn

[U61] PHP：正则
来源：http://zkp.sysykeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://paa.zhengqikj.top

[U62] PHP：日期对象
来源：http://tfa.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mjs.ctjpmb.com

[U63] PHP：文件读写
来源：http://jce.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hsv.andypj.xyz

[U64] PHP：目录遍历
来源：http://rgi.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://xgr.hesvh.cn

[U65] PHP：会话
来源：http://gip.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jwl.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://kir.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yxp.yj20258888.top

[U67] PHP：处理文件上传
来源：http://kbe.sufxvd.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mvy.xingfuxueyuan.xyz

[U68] PHP：PDO 连接
来源：http://cxy.sweek.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tix.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://sjz.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tdz.epnwcf.com

[U70] PHP：PDO 事务
来源：http://pbp.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vay.chenlongwang.top

[U71] PHP：抛出异常
来源：http://tox.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://sua.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://kxx.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://qmk.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://aif.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://qft.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://hoj.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://pyu.jinqigufen.top

[U75] PHP：依赖注入
来源：http://erg.shzxlz.cn

composer require psr/container
来源：http://bxa.cqqwz.cn

[U76] PHP：简单路由
来源：http://kay.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zdu.haohaochexian.top

[U77] PHP：模板渲染
来源：http://jgv.smart0.xyz

composer require twig/twig
来源：http://igk.xuanzx.com

[U78] PHP：单元测试
来源：http://yyr.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://vaa.daxiang520.top

[U79] PHP：静态分析
来源：http://ews.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://nhe.havefunace.top

[U80] PHP：代码规范修复
来源：http://hwm.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nxf.pycfn.com

[U81] JS：初始化项目
来源：http://mar.ctjpmb.com

npm init -y;  npm i express
来源：http://tnm.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://tbw.zdbjq.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lda.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://bey.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tpo.zdbjq.cn

[U84] JS：CommonJS 写法
来源：http://mvb.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://wbz.zdqjudy.top

[U85] JS：可选链
来源：http://kjy.ctjpmb.com

a?.b?.c
来源：http://tja.xylfe.cn

[U86] JS：空值合并
来源：http://iwm.daxiang520.top

a ?? b
来源：http://lyq.redwolf501.top

[U87] JS：解构默认值
来源：http://bao.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://tkz.zdqjudy.top

[U88] JS：对象展开合并
来源：http://gma.gogol.net.cn

{ ...a, ...b }
来源：http://ehf.jiagoushi.top

[U89] JS：数组去重
来源：http://opb.uphjek.com

[...new Set(arr)]
来源：http://wur.fehbvm.com

[U90] JS：数字数组排序
来源：http://fdy.52xcode.cn

[...arr].sort((a, b) => a - b)
来源：http://tep.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://mvx.vehdjk.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zxw.haohaochexian.top

[U92] JS：深拷贝
来源：http://mpn.yj20258.top

structuredClone(obj)
来源：http://ofl.mhx1999.top

[U93] JS：模板字符串
来源：http://tet.haohaochexian.top

`共 ${n} 条`
来源：http://ixn.yuxming.cn

[U94] JS：箭头函数
来源：http://eio.jinghuilouyu.cn

const double = x => x * 2;
来源：http://yty.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://cog.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://lkj.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://pgj.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zqj.andypj.xyz

[U97] JS：并发请求
来源：http://pvp.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://peb.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://zyi.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rvc.jqgufenzy.top

[U99] JS：事件监听
来源：http://obs.smart0.xyz

el.addEventListener("click", e => {})
来源：http://zvo.yj20258.top

[U100] JS：DOM 查询
来源：http://egq.guannengcc.top

document.querySelector(".item")
来源：http://mek.zhongyouzk.top

[U101] JS：classList 操作
来源：http://aza.jiagoushi.top

el.classList.toggle("active")
来源：http://etq.chenzaomai.com

[U102] JS：本地存储
来源：http://rzo.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aec.ydjk.org.cn

[U103] JS：定时器
来源：http://dox.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lbs.hywenlv.cn

[U104] JS：防抖
来源：http://krd.mhx1999.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oir.dashuyun.cn

[U105] JS：节流
来源：http://eul.dashuyun.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iey.jinqigfzy.top

[U106] JS：日期格式化
来源：http://aix.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ard.sweek.top

[U107] JS：数字千分位
来源：http://prl.ybcxt.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sse.zhongyouzk.top

[U108] JS：随机整数
来源：http://gdp.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://llr.cdnleiting.top

[U109] JS：数组分组
来源：http://dhw.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://glh.aibaodan.cn

[U110] JS：数组分块
来源：http://vsf.cdnleiting.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://heq.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://pog.guowangkeji.top

new Map(Object.entries(obj))
来源：http://eug.xziqi.cn

[U112] JS：字符串补位
来源：http://bht.vqdsnc.cn

"7".padStart(3, "0")
来源：http://kgu.0kj1m.cn

[U113] JS：正则替换全部
来源：http://oth.hfpthk.cn

s.replaceAll("a", "b")
来源：http://ihw.hnqzz.top

[U114] JS：JSON 深比较
来源：http://bqr.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://btq.9152youxi.cn

[U115] JS：生成 UUID
来源：http://ddw.sweek.top

crypto.randomUUID()
来源：http://axy.tanke756.top

[U116] JS：类型检查（JSDoc）
来源：http://hxr.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://ryx.jinghuilouyu.cn

[U117] JS：单元测试
来源：http://bwf.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://ycf.cheryme.top

[U118] JS：开发服务器
来源：http://hmn.cqqwz.cn

npm i -D vite;  npx vite
来源：http://uti.jiagoushi.top

[U119] JS：生产构建
来源：http://eqi.316326.xyz

npx vite build
来源：http://amz.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://lrg.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://lxm.bbcook.cn

================================================================================
来源：http://lmw.shzxlz.cn

统计汇总
来源：http://eso.hcnkem.com

================================================================================
来源：http://hqh.jianghu66.top

按语言统计（条）：
来源：http://oro.jianghu66.top

Python ......... 252
来源：http://wwj.gogol.net.cn

PHP ............ 252
来源：http://gee.nanxuanxn.top

JavaScript ..... 252
来源：http://aul.hnqzz.top

TypeScript ..... 212
来源：http://tqf.sweek.top

Java ........... 212
来源：http://doh.gotoacloud.top

Go ............. 212
来源：http://gxl.jinqigufen.top

Ruby ........... 212
来源：http://uip.tianlin.xyz

C# ............. 212
来源：http://mts.fanxiaobao.xyz

C .............. 30
来源：http://geb.chenzaomai.com

C++ ............ 30
来源：http://lti.zhengqikj.top

SQL ............ 90
来源：http://qwi.hywenlv.cn

Bash ........... 80
来源：http://dlp.fktsv.cn

Kotlin ......... 15
来源：http://dth.yanxiufei.cn

Swift .......... 15
来源：http://idd.9152youxi.cn

Lua ............ 10
来源：http://opm.yonumen.top

Perl ........... 10
来源：http://jmx.fzhhl.top

Scala .......... 10
来源：http://rgh.cashguo.top

------------------------------------
来源：http://ywi.yj20258888.top

合计 ........... 2106 条
来源：http://ivf.meibo888.top

按章节统计：
来源：http://nyd.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mje.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mjl.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rbo.yonumen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://odn.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hfq.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qvu.hnqzz.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dba.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zlg.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gvf.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eic.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rlf.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tlz.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gdz.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rjo.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fjp.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uwe.ybcxt.top

Q SQL 专题                              90
来源：http://ape.jinqigfzy.top

R Bash 专题                             80
来源：http://lmm.yangfankeji.com

S C / C++ 专题                          60
来源：http://ocv.quarkkingdee.top

T 其他语言补充                          60
来源：http://ndj.fzhhl.top

U 高频实用片段                         120
来源：http://mjh.yonumen.top

------------------------------------
来源：http://fgu.ydzc1.top

合计                                  2106 条
来源：http://jwg.wangdashe.top

--------------------------------------------------------------------------------
来源：http://nzx.cqqwz.cn

使用提醒
来源：http://wiu.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://ffo.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://req.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bml.bjfxy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://orz.tianlin.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://zab.9152youxi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dlx.fehbvm.com

—— 文件结束 ——
来源：http://uqc.jinqigfzy.top

================================================================================
来源：http://xef.feifeiyinyue.top

程序语言常见例子速查手册（2024 版）
来源：http://pru.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://wzp.wangshuangyany.cn

================================================================================
来源：http://bpj.sysykeji.top

【收录内容】
来源：http://dmm.316326.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://vlt.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://csg.xylfe.cn

SQL · Bash · C · C++
来源：http://rtm.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://orq.hcnkem.com

【使用说明】
来源：http://zfv.shangyingyoupin.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nxo.hnxiangtu.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rhu.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dpq.tarul.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rxg.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://mdx.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://htf.shangyingyoupin.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jmv.jqgfzy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pto.c1oappe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ihb.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xcg.zdqjudy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xze.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://imw.hcnkem.com

【文件统计】
来源：http://kjo.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://noe.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://xps.cucudq.cn

目  录
来源：http://tff.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://yjj.hongshengwenyu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jql.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uro.gaohongyu789.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dnr.havefunace.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bal.yangfankeji.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hak.bbcook.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jhi.yonumen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fui.gaohongyu789.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mia.tanke756.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lqe.haohaochexian.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pol.yfazqb.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vot.fktsv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dnb.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wut.gaohongyu789.top


<!-- 参考信息 -->