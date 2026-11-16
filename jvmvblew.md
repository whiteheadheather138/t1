代发 wailian999

[U17] Py：初始化日志
来源：http://opf.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://blh.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://vih.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://iqz.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://xlk.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gmc.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://wfj.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://ojf.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://kbx.pengpengdd.cyou

@contextlib.contextmanager
来源：http://hqi.jianghu66.top

[U22] Py：矩阵转置
来源：http://tti.zhijiandao.cn

list(zip(*m))
来源：http://oir.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://abc.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fpe.daxiang520.top

[U24] Py：路径操作
来源：http://vjz.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lgw.birdmap.top

[U25] Py：CSV 按字典读
来源：http://izj.redwolf501.top

csv.DictReader(f)
来源：http://yfw.yueranfly.top

[U26] Py：并发下载
来源：http://bum.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fxf.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://vjs.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://qtd.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://gwc.jinghuilouyu.cn

UserId = int
来源：http://fdt.zhiwuduotai.top

[U29] Py：属性校验
来源：http://zfy.ivvv.top

@property 与 @x.setter 配合
来源：http://zeg.jqgufenzy.top

[U30] Py：数据类
来源：http://gpi.sufxvd.cn

@dataclass(slots=True)
来源：http://bhp.vehdjk.com

[U31] Py：单测
来源：http://wwo.tanke756.top

python -m pytest -q
来源：http://grh.daxiang520.top

[U32] Py：代码格式化
来源：http://ttm.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://tex.mhx1999.top

[U33] Py：打包发布
来源：http://rke.9152youxi.cn

python -m build  （依赖 pyproject.toml）
来源：http://pnj.c1oappe.top

[U34] Py：判断编码
来源：http://apx.epnwcf.com

chardet.detect(raw)
来源：http://cfg.sxryk.cn

[U35] Py：发送邮件
来源：http://vkl.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nhz.wangshuangyany.cn

[U36] Py：定时任务
来源：http://irv.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://xli.redwolf501.top

[U37] Py：读写 Excel
来源：http://lfj.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://uee.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://rlt.sxryk.cn

Path(__file__).resolve().parent
来源：http://tzv.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://gsr.sufxvd.cn

sys.stdout.isatty()
来源：http://nuh.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://ekp.yangfankeji.com

print("err", file=sys.stderr)
来源：http://cxh.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://qjl.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://syv.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://dru.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cbd.vehdjk.com

[U43] PHP：声明命名空间
来源：http://dll.zhiwuduotai.top

namespace App\Http;
来源：http://cqe.jianghu66.top

[U44] PHP：开启严格类型
来源：http://bjh.jqgufenzy.top

declare(strict_types=1);
来源：http://owq.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://owq.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zkn.tianlin.xyz

[U46] PHP：可空类型
来源：http://mvx.jinqigfzy.top

?string $name = null
来源：http://owk.xylfe.cn

[U47] PHP：联合类型
来源：http://bzj.hcnkem.com

int|string $id
来源：http://ssv.xziqi.cn

[U48] PHP：纯枚举
来源：http://bsc.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cgn.yfazqb.com

[U49] PHP：只读属性
来源：http://job.vqdsnc.cn

public readonly string $name
来源：http://bhg.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://tne.jqgfzy.top

public function __construct(private int $id) {}
来源：http://rer.daxiang520.top

[U51] PHP：数组解构
来源：http://dtu.vehdjk.com

[$a, $b] = $arr;
来源：http://jkz.epnwcf.com

[U52] PHP：箭头函数
来源：http://utr.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://vop.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://iou.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://dav.ivvv.top

[U54] PHP：空安全调用
来源：http://zdi.wangdashe.top

$obj?->method()
来源：http://eib.fehbvm.com

[U55] PHP：match 表达式
来源：http://adg.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gnr.xylfe.cn

[U56] PHP：命名参数
来源：http://foq.zhengqikj.top

f(a: 1, b: 2)
来源：http://xts.hcnkem.com

[U57] PHP：字符串插值
来源：http://cmu.ctjpmb.com

"值: {$a}"
来源：http://fut.9152youxi.cn

[U58] PHP：数组三件套
来源：http://vii.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cyj.sysykeji.top

[U59] PHP：自定义排序
来源：http://dty.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oik.hywenlv.cn

[U60] PHP：JSON 编解码
来源：http://zjz.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gwq.ivvv.top

[U61] PHP：正则
来源：http://ujn.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dlq.tarul.cn

[U62] PHP：日期对象
来源：http://ynr.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mhp.iojbl.cn

[U63] PHP：文件读写
来源：http://euk.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uji.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://rjv.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://wib.cdnleiting.top

[U65] PHP：会话
来源：http://uti.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zei.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://ofi.52xcode.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xvf.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://hld.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pjn.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://ygd.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://req.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://sgu.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eay.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://sme.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nvn.smart0.xyz

[U71] PHP：抛出异常
来源：http://ple.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://lrg.shzxlz.cn

[U72] PHP：写错误日志
来源：http://hjd.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://iba.jinyuanbaomall.cn

[U73] PHP：读取 ini 配置
来源：http://svv.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://ctc.wangdashe.top

[U74] PHP：读取环境变量
来源：http://yss.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://xsw.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://jxz.xziqi.cn

composer require psr/container
来源：http://kvq.ydjk.org.cn

[U76] PHP：简单路由
来源：http://qfa.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mid.tarul.cn

[U77] PHP：模板渲染
来源：http://rgo.quarkkingdee.top

composer require twig/twig
来源：http://osi.kuanghao11.cn

[U78] PHP：单元测试
来源：http://luu.meibo888.top

composer require --dev phpunit/phpunit
来源：http://bgw.nanxinkj.top

[U79] PHP：静态分析
来源：http://vhq.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://gda.yonumen.top

[U80] PHP：代码规范修复
来源：http://mgx.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://egt.xuanzx.com

[U81] JS：初始化项目
来源：http://bve.aizwys.cn

npm init -y;  npm i express
来源：http://deq.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://jup.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://auo.ydzc1.top

[U83] JS：ES Module 导入导出
来源：http://frw.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kvt.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://oec.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://oqt.yongpay.top

[U85] JS：可选链
来源：http://wqa.jinqigufen.top

a?.b?.c
来源：http://rmy.smart0.xyz

[U86] JS：空值合并
来源：http://mmh.sweek.top

a ?? b
来源：http://dvk.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://rpe.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://pbf.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://idi.yanxiufei.cn

{ ...a, ...b }
来源：http://upr.dianchejie.cn

[U89] JS：数组去重
来源：http://zkn.fzhhl.top

[...new Set(arr)]
来源：http://cqy.yongpay.top

[U90] JS：数字数组排序
来源：http://acw.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://laq.hcnkem.com

[U91] JS：对象键值遍历
来源：http://asb.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kim.shangyingyoupin.top

[U92] JS：深拷贝
来源：http://gmd.ppjwa.cn

structuredClone(obj)
来源：http://yfj.xinyue.icu

[U93] JS：模板字符串
来源：http://nqh.jyoumei.cn

`共 ${n} 条`
来源：http://lzx.kuanghao11.cn

[U94] JS：箭头函数
来源：http://plm.nwbrower.top

const double = x => x * 2;
来源：http://ogh.zhongyouzk.top

[U95] JS：Promise 包装
来源：http://iru.dianchejie.cn

new Promise((resolve, reject) => {})
来源：http://nup.kuanghao11.cn

[U96] JS：async/await 与异常
来源：http://deb.yj20258.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iun.zhengqikj.top

[U97] JS：并发请求
来源：http://jll.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uld.sweek.top

[U98] JS：fetch 带 JSON
来源：http://tzk.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mgs.hcnkem.com

[U99] JS：事件监听
来源：http://yox.yj202588.top

el.addEventListener("click", e => {})
来源：http://hej.svipenyu.cn

[U100] JS：DOM 查询
来源：http://ptr.shangyingyoupin.top

document.querySelector(".item")
来源：http://cvo.mhx1999.top

[U101] JS：classList 操作
来源：http://tkr.guannengcc.top

el.classList.toggle("active")
来源：http://viu.daria6918.cn

[U102] JS：本地存储
来源：http://weq.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxy.jyoumei.cn

[U103] JS：定时器
来源：http://csh.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kgc.gzhubu.top

[U104] JS：防抖
来源：http://flf.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rku.hcnkem.com

[U105] JS：节流
来源：http://jmw.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jml.svipenyu.cn

[U106] JS：日期格式化
来源：http://gep.pengpengdd.cyou

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fhz.c1oappe.top

[U107] JS：数字千分位
来源：http://vfe.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zqf.yanxiufei.cn

[U108] JS：随机整数
来源：http://jvz.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://had.feifeiyinyue.top

[U109] JS：数组分组
来源：http://esd.hysaishi.cn

Object.groupBy(arr, x => x.type)
来源：http://bgy.yanxiufei.cn

[U110] JS：数组分块
来源：http://ogg.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qlh.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://vhc.cqqwz.cn

new Map(Object.entries(obj))
来源：http://jcc.ivvv.top

[U112] JS：字符串补位
来源：http://gyj.iojbl.cn

"7".padStart(3, "0")
来源：http://ifj.cashguo.top

[U113] JS：正则替换全部
来源：http://rie.zhixingplan.top

s.replaceAll("a", "b")
来源：http://jdm.daxiang520.top

[U114] JS：JSON 深比较
来源：http://dln.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aor.guannengcc.top

[U115] JS：生成 UUID
来源：http://omq.hnqzz.top

crypto.randomUUID()
来源：http://gay.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://ddj.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://afc.aizwys.cn

[U117] JS：单元测试
来源：http://wlk.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://cwd.haohaochexian.top

[U118] JS：开发服务器
来源：http://jhl.tian-w.cn

npm i -D vite;  npx vite
来源：http://pmp.fktsv.cn

[U119] JS：生产构建
来源：http://zso.nanxinkj.top

npx vite build
来源：http://ktd.birdmap.top

[U120] JS：读取环境变量（Vite）
来源：http://gkt.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://sek.nanxinkj.top

================================================================================
来源：http://kri.guannengcc.top

统计汇总
来源：http://vmh.andypj.xyz

================================================================================
来源：http://wbg.c1oappe.top

按语言统计（条）：
来源：http://nbr.zhiwuduotai.top

Python ......... 252
来源：http://qfx.sxryk.cn

PHP ............ 252
来源：http://dpl.cdnleiting.top

JavaScript ..... 252
来源：http://bxx.hongshengwenyu.top

TypeScript ..... 212
来源：http://wqe.xuetiantiany.cn

Java ........... 212
来源：http://ahl.yuxming.cn

Go ............. 212
来源：http://nwc.shanyushiyangtech.top

Ruby ........... 212
来源：http://lcy.yongpay.top

C# ............. 212
来源：http://nrf.kuanghao11.cn

C .............. 30
来源：http://wrw.aizwys.cn

C++ ............ 30
来源：http://hts.wangdashe.top

SQL ............ 90
来源：http://zce.pycfn.com

Bash ........... 80
来源：http://kfb.fengsongda.top

Kotlin ......... 15
来源：http://tle.snrcjt.cn

Swift .......... 15
来源：http://nxe.kuanghao11.cn

Lua ............ 10
来源：http://loq.hongshengwenyu.top

Perl ........... 10
来源：http://pyv.zhoulong.xyz

Scala .......... 10
来源：http://gvw.birdmap.top

------------------------------------
来源：http://aar.wangdashe.top

合计 ........... 2106 条
来源：http://uba.cashguo.top

按章节统计：
来源：http://wpf.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://usr.sufxvd.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zma.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aoa.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://umk.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kfu.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wvq.tian-w.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wzi.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://myc.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://awv.hnqzz.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cfe.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sjy.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jrw.cdnleiting.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ujj.zdbjq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bcr.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jjg.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://esr.hfpthk.cn

Q SQL 专题                              90
来源：http://ara.cqqwz.cn

R Bash 专题                             80
来源：http://aul.vehdjk.com

S C / C++ 专题                          60
来源：http://nho.shzxlz.cn

T 其他语言补充                          60
来源：http://wwx.sysykeji.top

U 高频实用片段                         120
来源：http://gjn.daxiang520.top

------------------------------------
来源：http://eya.gotoacloud.top

合计                                  2106 条
来源：http://ksd.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://fci.cheryme.top

使用提醒
来源：http://vsp.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://fzi.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kll.gzhubu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://luf.sysykeji.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fao.hammf.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dkg.hysaishi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mni.mhx1999.top

—— 文件结束 ——
来源：http://bjs.bjfxy.top

================================================================================
来源：http://pgv.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://ydh.fktsv.cn

Common Programming Examples Cheat Book
来源：http://fno.mhx1999.top

================================================================================
来源：http://yvp.mhx1999.top

【收录内容】
来源：http://eky.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://rlh.cheryme.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ibl.sxryk.cn

SQL · Bash · C · C++
来源：http://nbw.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://opy.tarul.cn

【使用说明】
来源：http://wmy.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nse.chenzaomai.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pys.xuanzx.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uxo.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vpy.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://tdu.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cmt.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wwe.feifeiyinyue.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qpk.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tiu.zycfv.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kmm.andypj.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ovi.zdqjudy.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tzc.yueranfly.top

【文件统计】
来源：http://mec.zhongyouzk.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rwa.shuidangran.top

--------------------------------------------------------------------------------
来源：http://kiw.feifeiyinyue.top

目  录
来源：http://atx.vehdjk.com

--------------------------------------------------------------------------------
来源：http://mni.hysaishi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bmz.nanxuanxn.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yki.pengpengdd.cyou

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yrq.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ppi.yuxming.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://izo.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://acs.jinqigufen.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hen.ywan-chungtsiang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qua.hywenlv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://osc.gaohongyu789.top


<!-- 参考信息 -->