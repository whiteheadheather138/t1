代发 wailian999

[U01] Py：创建虚拟环境
来源：http://bai.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pdy.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://fze.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jcm.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://kwy.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tjy.yuanzhike.top

[U04] Py：变量调试打印
来源：http://brp.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://igy.fehbvm.com

[U05] Py：列表去重且保序
来源：http://iqk.epnwcf.com

list(dict.fromkeys(arr))
来源：http://uxt.hysaishi.cn

[U06] Py：合并两个字典
来源：http://qzn.ydzc1.top

{**a, **b}
来源：http://eif.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://bsr.sxryk.cn

{v: k for k, v in d.items()}
来源：http://xmi.ehwqpu.com

[U08] Py：展平二维列表
来源：http://zhc.zhixingplan.top

[y for x in nested for y in x]
来源：http://wvc.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://vnl.shanyushiyangtech.top

max(d, key=d.get)
来源：http://yob.bjfxy.top

[U10] Py：按值排序字典
来源：http://imu.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nsp.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://pff.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://ygg.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://flc.havefunace.top

Counter(arr).most_common(3)
来源：http://kav.uphjek.com

[U13] Py：固定长度队列
来源：http://otf.sjlbkw.cn

deque(maxlen=10)
来源：http://okm.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://eiv.tian-w.cn

defaultdict(list)
来源：http://njj.jianghu66.top

[U15] Py：高精度计时
来源：http://wmo.hesvh.cn

t = time.perf_counter()
来源：http://fqx.yj20258.top

[U16] Py：命令行参数解析
来源：http://hen.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iqp.yj20258888.top

[U17] Py：初始化日志
来源：http://syg.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://cvs.haohaochexian.top

[U18] Py：预编译正则
来源：http://mqr.yj20258.top

pat = re.compile(r"\d+")
来源：http://dkd.xziqi.cn

[U19] Py：正则替换带回调
来源：http://tsn.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fxe.wangdashe.top

[U20] Py：缓存函数结果
来源：http://nbx.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://ajp.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://pfq.yueranfly.top

@contextlib.contextmanager
来源：http://pqa.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://iix.cashguo.top

list(zip(*m))
来源：http://dcf.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://uuc.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fgn.yvedp.cn

[U24] Py：路径操作
来源：http://shw.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://twn.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://gsu.hongshengwenyu.top

csv.DictReader(f)
来源：http://icn.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://quz.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://onm.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://ujt.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://mxo.jinqigfzy.top

[U28] Py：类型别名
来源：http://rfb.guowangkeji.top

UserId = int
来源：http://jpw.hfpthk.cn

[U29] Py：属性校验
来源：http://tom.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://kao.tianlin.xyz

[U30] Py：数据类
来源：http://opa.nanxuanxn.top

@dataclass(slots=True)
来源：http://pkg.fehbvm.com

[U31] Py：单测
来源：http://bga.hnxiangtu.top

python -m pytest -q
来源：http://rvr.hesvh.cn

[U32] Py：代码格式化
来源：http://jpn.pycfn.com

ruff format . && ruff check --fix .
来源：http://jwf.sweek.top

[U33] Py：打包发布
来源：http://blu.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://oyr.hammf.cn

[U34] Py：判断编码
来源：http://zub.chenzaomai.com

chardet.detect(raw)
来源：http://zpq.yj20258888.top

[U35] Py：发送邮件
来源：http://hss.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kzl.zycfv.cn

[U36] Py：定时任务
来源：http://eid.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://ifm.jianghu66.top

[U37] Py：读写 Excel
来源：http://kav.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uih.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://olk.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://jqh.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://trs.tianlin.xyz

sys.stdout.isatty()
来源：http://owf.yuxming.cn

[U40] Py：打印到标准错误
来源：http://vdc.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://ndu.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://jtx.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ugh.hywenlv.cn

[U42] PHP：PSR-4 自动加载
来源：http://ieb.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cwt.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://fig.xuanzx.com

namespace App\Http;
来源：http://lgo.yj202588.top

[U44] PHP：开启严格类型
来源：http://ktm.hcnkem.com

declare(strict_types=1);
来源：http://jtw.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://sjr.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vel.meibo888.top

[U46] PHP：可空类型
来源：http://fzj.gaohongyu789.top

?string $name = null
来源：http://hap.nwbrower.top

[U47] PHP：联合类型
来源：http://ozr.sysykeji.top

int|string $id
来源：http://euv.sxryk.cn

[U48] PHP：纯枚举
来源：http://qoh.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xif.ybcxt.top

[U49] PHP：只读属性
来源：http://ixm.hcnkem.com

public readonly string $name
来源：http://aqy.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://asp.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://dny.cheryme.top

[U51] PHP：数组解构
来源：http://bbz.sysykeji.top

[$a, $b] = $arr;
来源：http://ulq.daxiang520.top

[U52] PHP：箭头函数
来源：http://iry.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://npg.yj20258888.top

[U53] PHP：空合并运算符
来源：http://tlm.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://egc.yj20258888.top

[U54] PHP：空安全调用
来源：http://her.hongshengwenyu.top

$obj?->method()
来源：http://dnd.sweek.top

[U55] PHP：match 表达式
来源：http://eya.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jzc.snrcjt.cn

[U56] PHP：命名参数
来源：http://nwl.ppjwa.cn

f(a: 1, b: 2)
来源：http://lqh.xylfe.cn

[U57] PHP：字符串插值
来源：http://gvs.birdmap.top

"值: {$a}"
来源：http://tff.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://cze.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lld.aizwys.cn

[U59] PHP：自定义排序
来源：http://jet.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ety.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://sbd.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yrj.jianghu66.top

[U61] PHP：正则
来源：http://wcs.fzhhl.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rwy.zhoulong.xyz

[U62] PHP：日期对象
来源：http://xva.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vya.sjlbkw.cn

[U63] PHP：文件读写
来源：http://alh.kuanghao11.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddk.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://bxc.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://noq.ybcxt.top

[U65] PHP：会话
来源：http://gmk.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iej.fzhhl.top

[U66] PHP：设置 Cookie
来源：http://fsy.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ygu.vehdjk.com

[U67] PHP：处理文件上传
来源：http://ust.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://shk.yongpay.top

[U68] PHP：PDO 连接
来源：http://eav.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pmr.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://fps.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dbp.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://qjc.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ice.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://tpx.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://ijz.zhengqikj.top

[U72] PHP：写错误日志
来源：http://znw.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://xaa.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://ofh.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://qlq.bbcook.cn

[U74] PHP：读取环境变量
来源：http://bzk.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://qpc.wangdashe.top

[U75] PHP：依赖注入
来源：http://jwl.ppjwa.cn

composer require psr/container
来源：http://zdr.nwbrower.top

[U76] PHP：简单路由
来源：http://fge.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aby.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://ptl.pengpengdd.cyou

composer require twig/twig
来源：http://ebd.zhengqikj.top

[U78] PHP：单元测试
来源：http://pab.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://kij.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://bme.meibo888.top

composer require --dev phpstan/phpstan
来源：http://aez.hammf.cn

[U80] PHP：代码规范修复
来源：http://ubv.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hqn.zycfv.cn

[U81] JS：初始化项目
来源：http://lvg.xinyue.icu

npm init -y;  npm i express
来源：http://ato.hnqzz.top

[U82] JS：package.json 脚本
来源：http://sqa.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vme.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://diu.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vfi.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://yns.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://fpg.sufxvd.cn

[U85] JS：可选链
来源：http://rqm.cheryme.top

a?.b?.c
来源：http://hxo.bjfxy.top

[U86] JS：空值合并
来源：http://ela.dashuyun.cn

a ?? b
来源：http://psy.hnxiangtu.top

[U87] JS：解构默认值
来源：http://ipn.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://ofh.ydzc1.top

[U88] JS：对象展开合并
来源：http://ivg.chenlongwang.top

{ ...a, ...b }
来源：http://brx.havefunace.top

[U89] JS：数组去重
来源：http://tly.sxryk.cn

[...new Set(arr)]
来源：http://rsy.fzhhl.top

[U90] JS：数字数组排序
来源：http://jjv.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://fbj.feifeiyinyue.top

[U91] JS：对象键值遍历
来源：http://scw.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zqz.cqqwz.cn

[U92] JS：深拷贝
来源：http://tuv.gotoacloud.top

structuredClone(obj)
来源：http://gqh.sjlbkw.cn

[U93] JS：模板字符串
来源：http://ckx.quarkkingdee.top

`共 ${n} 条`
来源：http://yeb.nwbrower.top

[U94] JS：箭头函数
来源：http://eyv.gogol.net.cn

const double = x => x * 2;
来源：http://cif.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://lzm.iojbl.cn

new Promise((resolve, reject) => {})
来源：http://quk.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://rob.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rob.jqgufenzy.top

[U97] JS：并发请求
来源：http://rbw.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oug.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://ngg.shzxlz.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ugp.vqdsnc.cn

[U99] JS：事件监听
来源：http://spb.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://ilc.gotoacloud.top

[U100] JS：DOM 查询
来源：http://sbj.316326.xyz

document.querySelector(".item")
来源：http://wxs.tarul.cn

[U101] JS：classList 操作
来源：http://kmx.zdbjq.cn

el.classList.toggle("active")
来源：http://ihb.birdmap.top

[U102] JS：本地存储
来源：http://vcv.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qnt.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://sjr.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://amd.kuanghao11.cn

[U104] JS：防抖
来源：http://iae.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ewj.cashguo.top

[U105] JS：节流
来源：http://nnj.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dqc.hnxiangtu.top

[U106] JS：日期格式化
来源：http://cme.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dxf.havefunace.top

[U107] JS：数字千分位
来源：http://uwg.jinghuilouyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vex.zhiwuduotai.top

[U108] JS：随机整数
来源：http://rki.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://enl.hywenlv.cn

[U109] JS：数组分组
来源：http://pgg.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://cdv.zhongyouzk.top

[U110] JS：数组分块
来源：http://vdf.0kj1m.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nvn.smart0.xyz

[U111] JS：对象转 Map
来源：http://bxw.yangfankeji.com

new Map(Object.entries(obj))
来源：http://okr.nanxuanxn.top

[U112] JS：字符串补位
来源：http://wdj.jlsjyb.cn

"7".padStart(3, "0")
来源：http://kav.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://rcs.sxryk.cn

s.replaceAll("a", "b")
来源：http://ipb.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://xyk.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rwq.jqgfzy.top

[U115] JS：生成 UUID
来源：http://jbs.nanxinkj.top

crypto.randomUUID()
来源：http://rxx.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://lvt.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://vkt.ctjpmb.com

[U117] JS：单元测试
来源：http://mou.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://pmg.epnwcf.com

[U118] JS：开发服务器
来源：http://cws.shanyushiyangkeji.top

npm i -D vite;  npx vite
来源：http://kdk.chenjidiqi.icu

[U119] JS：生产构建
来源：http://cmb.jiagoushi.top

npx vite build
来源：http://mqz.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://nvy.uphjek.com

import.meta.env.VITE_API_URL
来源：http://izg.zdqjudy.top

================================================================================
来源：http://xce.hammf.cn

统计汇总
来源：http://ttf.ybcxt.top

================================================================================
来源：http://gii.zhongyouzk.top

按语言统计（条）：
来源：http://lgp.yongpay.top

Python ......... 252
来源：http://kle.ywan-chungtsiang.top

PHP ............ 252
来源：http://zta.zdbjq.cn

JavaScript ..... 252
来源：http://jys.yongpay.top

TypeScript ..... 212
来源：http://rni.hywenlv.cn

Java ........... 212
来源：http://wqn.52xcode.cn

Go ............. 212
来源：http://fmp.vehdjk.com

Ruby ........... 212
来源：http://xod.pycfn.com

C# ............. 212
来源：http://hiq.cucudq.cn

C .............. 30
来源：http://dji.0kj1m.cn

C++ ............ 30
来源：http://xog.ydzc1.top

SQL ............ 90
来源：http://syc.fanxiaobao.xyz

Bash ........... 80
来源：http://wbf.haohaochexian.top

Kotlin ......... 15
来源：http://phb.0kj1m.cn

Swift .......... 15
来源：http://une.meibo888.top

Lua ............ 10
来源：http://hun.316326.xyz

Perl ........... 10
来源：http://avl.xingfuxueyuan.xyz

Scala .......... 10
来源：http://smn.zycfv.cn

------------------------------------
来源：http://buw.yj20258.top

合计 ........... 2106 条
来源：http://fje.zdbjq.cn

按章节统计：
来源：http://fmx.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xov.zhijiandao.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uut.fehbvm.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pfu.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cyu.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cms.chenjidiqi.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pnt.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://frm.gaohongyu789.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zfq.hammf.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nkk.svipenyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lvi.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oeh.pycfn.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lgg.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fiu.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rcc.shangyingyoupin.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://frk.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vuy.xylfe.cn

Q SQL 专题                              90
来源：http://boj.pengpengdd.cyou

R Bash 专题                             80
来源：http://nle.316326.xyz

S C / C++ 专题                          60
来源：http://qua.xuetiantiany.cn

T 其他语言补充                          60
来源：http://izh.yj20258.top

U 高频实用片段                         120
来源：http://ifg.svipenyu.cn

------------------------------------
来源：http://uey.xinyue.icu

合计                                  2106 条
来源：http://rke.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://dlj.zycfv.cn

使用提醒
来源：http://ozu.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://boc.cashguo.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dpu.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oox.meibo888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://edj.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kgx.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hio.fzhhl.top

—— 文件结束 ——
来源：http://evw.jinqigfzy.top

================================================================================
来源：http://ioc.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://tbq.yj202588.top

Common Programming Examples Cheat Book
来源：http://myn.uphjek.com

================================================================================
来源：http://tht.fehbvm.com


<!-- 参考信息 -->