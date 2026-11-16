代发 wailian999

[U17] Py：初始化日志
来源：http://vvg.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://opy.ppjwa.cn

[U18] Py：预编译正则
来源：http://izt.c1oappe.top

pat = re.compile(r"\d+")
来源：http://ttz.fktsv.cn

[U19] Py：正则替换带回调
来源：http://kge.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vgt.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://pqk.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://wdi.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://usi.jiagoushi.top

@contextlib.contextmanager
来源：http://jof.xuanzx.com

[U22] Py：矩阵转置
来源：http://nrx.fengsongda.top

list(zip(*m))
来源：http://rvb.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://cwx.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lys.bbcook.cn

[U24] Py：路径操作
来源：http://sut.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jtm.jlsjyb.cn

[U25] Py：CSV 按字典读
来源：http://dve.yuanzhike.top

csv.DictReader(f)
来源：http://hsi.aizwys.cn

[U26] Py：并发下载
来源：http://znr.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://abm.ivvv.top

[U27] Py：异步 HTTP
来源：http://hax.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://djc.gaohongyu789.top

[U28] Py：类型别名
来源：http://fun.aibaodan.cn

UserId = int
来源：http://fpc.pengpengdd.cyou

[U29] Py：属性校验
来源：http://wgb.zhengqikj.top

@property 与 @x.setter 配合
来源：http://yzi.tanke756.top

[U30] Py：数据类
来源：http://ode.aizwys.cn

@dataclass(slots=True)
来源：http://cbp.shuidangran.top

[U31] Py：单测
来源：http://qbf.xinyue.icu

python -m pytest -q
来源：http://vpv.yj20258888.top

[U32] Py：代码格式化
来源：http://exa.nwbrower.top

ruff format . && ruff check --fix .
来源：http://gmq.birdmap.top

[U33] Py：打包发布
来源：http://mhu.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://rsn.feifeiyinyue.top

[U34] Py：判断编码
来源：http://iet.yongpay.top

chardet.detect(raw)
来源：http://xbs.svipenyu.cn

[U35] Py：发送邮件
来源：http://ykk.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nad.quarkkingdee.top

[U36] Py：定时任务
来源：http://yni.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://ykz.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://aka.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ivv.jinghuilouyu.cn

[U38] Py：获取脚本所在目录
来源：http://adk.gogol.net.cn

Path(__file__).resolve().parent
来源：http://ryw.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://unx.tianlin.xyz

sys.stdout.isatty()
来源：http://guz.bjfxy.top

[U40] Py：打印到标准错误
来源：http://jvb.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://kbs.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://gut.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tul.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://scx.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aer.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://qob.sufxvd.cn

namespace App\Http;
来源：http://wll.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://yfo.zhoulong.xyz

declare(strict_types=1);
来源：http://yxf.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://sic.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ncj.ydjk.org.cn

[U46] PHP：可空类型
来源：http://qzt.jinqigfzy.top

?string $name = null
来源：http://fac.fengsongda.top

[U47] PHP：联合类型
来源：http://xvx.quarkkingdee.top

int|string $id
来源：http://iqv.fehbvm.com

[U48] PHP：纯枚举
来源：http://mtq.jyoumei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jaa.cheryme.top

[U49] PHP：只读属性
来源：http://ggw.svipenyu.cn

public readonly string $name
来源：http://xxa.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://cbd.zdqjudy.top

public function __construct(private int $id) {}
来源：http://qfr.sufxvd.cn

[U51] PHP：数组解构
来源：http://vww.sjlbkw.cn

[$a, $b] = $arr;
来源：http://fcn.tianlin.xyz

[U52] PHP：箭头函数
来源：http://jkv.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://wso.birdmap.top

[U53] PHP：空合并运算符
来源：http://gdq.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://qoi.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://oan.xingfuxueyuan.xyz

$obj?->method()
来源：http://dwp.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://wan.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ioi.yj20258.top

[U56] PHP：命名参数
来源：http://wfu.aibaodan.cn

f(a: 1, b: 2)
来源：http://zpg.jqgufenzy.top

[U57] PHP：字符串插值
来源：http://wlt.jianghu66.top

"值: {$a}"
来源：http://uhf.gotoacloud.top

[U58] PHP：数组三件套
来源：http://myx.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://slr.yongpay.top

[U59] PHP：自定义排序
来源：http://fvw.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://avu.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://vgs.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xsh.jyoumei.cn

[U61] PHP：正则
来源：http://oym.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ied.52xcode.cn

[U62] PHP：日期对象
来源：http://dyu.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ljk.bjfxy.top

[U63] PHP：文件读写
来源：http://gwm.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://njh.meibo888.top

[U64] PHP：目录遍历
来源：http://qub.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://ons.yueranfly.top

[U65] PHP：会话
来源：http://kgw.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kvu.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://yon.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://clo.xinyue.icu

[U67] PHP：处理文件上传
来源：http://nco.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qzu.guannengcc.top

[U68] PHP：PDO 连接
来源：http://rrk.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pjf.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://wuf.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kof.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://gkx.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://izw.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://yna.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://fjc.wangdashe.top

[U72] PHP：写错误日志
来源：http://baq.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://ftx.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://klz.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://yrd.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://wkv.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://agb.guannengcc.top

[U75] PHP：依赖注入
来源：http://vdd.zhiwuduotai.top

composer require psr/container
来源：http://rfi.yuxming.cn

[U76] PHP：简单路由
来源：http://ghn.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pma.tian-w.cn

[U77] PHP：模板渲染
来源：http://luc.jqgfzy.top

composer require twig/twig
来源：http://qlt.daxiang520.top

[U78] PHP：单元测试
来源：http://qmd.yueranfly.top

composer require --dev phpunit/phpunit
来源：http://ojf.dashuyun.cn

[U79] PHP：静态分析
来源：http://taf.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://qnh.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://hal.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xap.quarkkingdee.top

[U81] JS：初始化项目
来源：http://tjg.xuanzx.com

npm init -y;  npm i express
来源：http://pdo.guannengcc.top

[U82] JS：package.json 脚本
来源：http://nzp.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hzc.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://ycl.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fun.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://alg.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://kwl.yj20258.top

[U85] JS：可选链
来源：http://kwt.nwbrower.top

a?.b?.c
来源：http://zdm.bbcook.cn

[U86] JS：空值合并
来源：http://qof.zhengqikj.top

a ?? b
来源：http://xov.epnwcf.com

[U87] JS：解构默认值
来源：http://pny.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://bnp.guannengcc.top

[U88] JS：对象展开合并
来源：http://jll.hcnkem.com

{ ...a, ...b }
来源：http://lzb.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://jci.fehbvm.com

[...new Set(arr)]
来源：http://yhg.ybcxt.top

[U90] JS：数字数组排序
来源：http://dpr.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://vod.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://ims.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ypl.sjlbkw.cn

[U92] JS：深拷贝
来源：http://wpr.vehdjk.com

structuredClone(obj)
来源：http://dpi.ctjpmb.com

[U93] JS：模板字符串
来源：http://qyd.jianghu66.top

`共 ${n} 条`
来源：http://ntp.gotoacloud.top

[U94] JS：箭头函数
来源：http://khi.fanxiaobao.xyz

const double = x => x * 2;
来源：http://ixl.sxryk.cn

[U95] JS：Promise 包装
来源：http://cse.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://vho.sjlbkw.cn

[U96] JS：async/await 与异常
来源：http://ywq.9152youxi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://elp.yvedp.cn

[U97] JS：并发请求
来源：http://wya.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://oke.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://bml.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ykw.tanke756.top

[U99] JS：事件监听
来源：http://qqa.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://jlj.bbcook.cn

[U100] JS：DOM 查询
来源：http://cfi.snrcjt.cn

document.querySelector(".item")
来源：http://fxn.daxiang520.top

[U101] JS：classList 操作
来源：http://hzb.bbcook.cn

el.classList.toggle("active")
来源：http://vwn.epnwcf.com

[U102] JS：本地存储
来源：http://jbt.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://llb.cheryme.top

[U103] JS：定时器
来源：http://bvq.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bzd.yuanzhike.top

[U104] JS：防抖
来源：http://gcq.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gxn.chenzaomai.com

[U105] JS：节流
来源：http://fpb.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aih.ydzc1.top

[U106] JS：日期格式化
来源：http://gkc.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dpd.shanyushiyangtech.top

[U107] JS：数字千分位
来源：http://dvc.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yty.tian-w.cn

[U108] JS：随机整数
来源：http://tcv.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ctp.svipenyu.cn

[U109] JS：数组分组
来源：http://rpp.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://stf.andypj.xyz

[U110] JS：数组分块
来源：http://mkw.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cpp.iojbl.cn

[U111] JS：对象转 Map
来源：http://hbn.9152youxi.cn

new Map(Object.entries(obj))
来源：http://gby.shuidangran.top

[U112] JS：字符串补位
来源：http://ciz.zhijiandao.cn

"7".padStart(3, "0")
来源：http://clg.cucudq.cn

[U113] JS：正则替换全部
来源：http://ewu.0kj1m.cn

s.replaceAll("a", "b")
来源：http://ntm.cashguo.top

[U114] JS：JSON 深比较
来源：http://iqe.ctjpmb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gtm.cashguo.top

[U115] JS：生成 UUID
来源：http://uew.sufxvd.cn

crypto.randomUUID()
来源：http://por.vehdjk.com

[U116] JS：类型检查（JSDoc）
来源：http://dxn.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://fkd.gaohongyu789.top

[U117] JS：单元测试
来源：http://cue.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://uej.dashuyun.cn

[U118] JS：开发服务器
来源：http://hku.hammf.cn

npm i -D vite;  npx vite
来源：http://swy.xziqi.cn

[U119] JS：生产构建
来源：http://xxv.ivvv.top

npx vite build
来源：http://pxx.tian-w.cn

[U120] JS：读取环境变量（Vite）
来源：http://evj.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://bgi.cqqwz.cn

================================================================================
来源：http://lev.guannengcc.top

统计汇总
来源：http://acm.shanyushiyangtech.top

================================================================================
来源：http://bwn.sxryk.cn

按语言统计（条）：
来源：http://opq.hnqzz.top

Python ......... 252
来源：http://dnv.shanyushiyangkeji.top

PHP ............ 252
来源：http://hxn.jinqigfzy.top

JavaScript ..... 252
来源：http://vmf.cheryme.top

TypeScript ..... 212
来源：http://xbb.dianchejie.cn

Java ........... 212
来源：http://krl.dianchejie.cn

Go ............. 212
来源：http://jsr.zhoulong.xyz

Ruby ........... 212
来源：http://vrw.daria6918.cn

C# ............. 212
来源：http://ohi.quarkkingdee.top

C .............. 30
来源：http://fyz.xingfuxueyuan.xyz

C++ ............ 30
来源：http://zkb.jinqigfzy.top

SQL ............ 90
来源：http://hzx.bbcook.cn

Bash ........... 80
来源：http://lye.jiagoushi.top

Kotlin ......... 15
来源：http://lej.sysykeji.top

Swift .......... 15
来源：http://hka.fzhhl.top

Lua ............ 10
来源：http://rqy.smart0.xyz

Perl ........... 10
来源：http://uei.hywenlv.cn

Scala .......... 10
来源：http://rla.sweek.top

------------------------------------
来源：http://ykj.guowangkeji.top

合计 ........... 2106 条
来源：http://pcm.cashguo.top

按章节统计：
来源：http://aqj.snrcjt.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mja.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qoe.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lug.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hxr.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xoc.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ala.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xzp.sufxvd.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oyd.xuanzx.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lty.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://oct.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sik.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tfo.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lks.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rbw.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eqh.hfpthk.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://upm.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://ndj.pycfn.com

R Bash 专题                             80
来源：http://xiv.bbcook.cn

S C / C++ 专题                          60
来源：http://yqe.ivvv.top

T 其他语言补充                          60
来源：http://ese.tarul.cn

U 高频实用片段                         120
来源：http://gua.ctjpmb.com

------------------------------------
来源：http://jus.cheryme.top

合计                                  2106 条
来源：http://xyl.nwbrower.top

--------------------------------------------------------------------------------
来源：http://iod.fktsv.cn

使用提醒
来源：http://kfi.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://ryi.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tqq.zhixingplan.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kdl.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vpr.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://mme.fktsv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://liz.xuanzx.com

—— 文件结束 ——
来源：http://vna.yueranfly.top

================================================================================
来源：http://uvy.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://hch.pycfn.com

Common Programming Examples Cheat Book
来源：http://dsi.fehbvm.com

================================================================================
来源：http://yro.9152youxi.cn

【收录内容】
来源：http://msr.shzxlz.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://paf.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://czx.shzxlz.cn

SQL · Bash · C · C++
来源：http://zta.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://grt.quarkkingdee.top

【使用说明】
来源：http://ztc.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bjl.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ogt.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zfl.feifeiyinyue.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fvh.yangfankeji.com

Bash:  Shell         C:     C             C++:   C++
来源：http://fim.haohaochexian.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://umh.wangdashe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nyn.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nym.cashguo.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wpi.ivvv.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ggl.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pck.chenzaomai.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ecb.nanxuanxn.top

【文件统计】
来源：http://xvq.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xas.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://bio.guowangkeji.top

目  录
来源：http://kpr.bbcook.cn

--------------------------------------------------------------------------------
来源：http://qka.yuanzhike.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ymb.xziqi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jiq.zhengqikj.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://opo.jinyuanbaomall.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pdx.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://esm.fehbvm.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gaj.meibo888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://npx.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zlb.svipenyu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://pvp.zhaomingkeji.xyz


<!-- 参考信息 -->