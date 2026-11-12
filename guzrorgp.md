代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://pgh.pengpengdd.cyou

[T59] Scala：循环
来源：http://oai.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://ede.zhongyouzk.top

[T60] Scala：折叠
来源：http://ojd.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://smh.hesvh.cn

================================================================================
来源：http://gnm.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zsc.9152youxi.cn

================================================================================
来源：http://zjj.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://kpr.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rys.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://rmc.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yhk.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://gjo.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zhh.dianchejie.cn

[U04] Py：变量调试打印
来源：http://tpp.dashuyun.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mmq.fengsongda.top

[U05] Py：列表去重且保序
来源：http://khp.uphjek.com

list(dict.fromkeys(arr))
来源：http://cod.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://wlz.kuanghao11.cn

{**a, **b}
来源：http://dzr.hywenlv.cn

[U07] Py：反转字典键值
来源：http://aun.52xcode.cn

{v: k for k, v in d.items()}
来源：http://wdf.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://bzm.xinyue.icu

[y for x in nested for y in x]
来源：http://vrt.hammf.cn

[U09] Py：字典取最大值的键
来源：http://leq.havefunace.top

max(d, key=d.get)
来源：http://vfu.yongpay.top

[U10] Py：按值排序字典
来源：http://nks.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yqe.fehbvm.com

[U11] Py：生成器表达式
来源：http://nxh.dianchejie.cn

(x * 2 for x in arr)
来源：http://wbb.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ikr.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://azj.jiagoushi.top

[U13] Py：固定长度队列
来源：http://snx.hammf.cn

deque(maxlen=10)
来源：http://hpp.tarul.cn

[U14] Py：分组收集到列表
来源：http://xae.ywan-chungtsiang.top

defaultdict(list)
来源：http://xpa.pycfn.com

[U15] Py：高精度计时
来源：http://mpf.wangdashe.top

t = time.perf_counter()
来源：http://dhp.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://kri.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vjy.smart0.xyz

[U17] Py：初始化日志
来源：http://byw.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://egd.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://jhz.kuanghao11.cn

pat = re.compile(r"\d+")
来源：http://bqw.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://qyr.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://spb.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://rdc.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://lbp.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://gkh.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://ask.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://jkh.bjfxy.top

list(zip(*m))
来源：http://gae.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://gya.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dpm.shangyingyoupin.top

[U24] Py：路径操作
来源：http://mgo.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fik.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://xye.jqgfzy.top

csv.DictReader(f)
来源：http://czc.wangshuangyany.cn

[U26] Py：并发下载
来源：http://svg.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aix.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://yac.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://jsy.guowangkeji.top

[U28] Py：类型别名
来源：http://lqv.shangyingyoupin.top

UserId = int
来源：http://ney.smart0.xyz

[U29] Py：属性校验
来源：http://gqq.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://etj.xuetiantiany.cn

[U30] Py：数据类
来源：http://zbl.snrcjt.cn

@dataclass(slots=True)
来源：http://kzv.svipenyu.cn

[U31] Py：单测
来源：http://omn.zhongyouzk.top

python -m pytest -q
来源：http://okb.dianchejie.cn

[U32] Py：代码格式化
来源：http://rho.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://ifd.ehwqpu.com

[U33] Py：打包发布
来源：http://gdx.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://yet.c1oappe.top

[U34] Py：判断编码
来源：http://ldi.shangyingyoupin.top

chardet.detect(raw)
来源：http://vlt.ppjwa.cn

[U35] Py：发送邮件
来源：http://dlc.hnqzz.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eum.guannengcc.top

[U36] Py：定时任务
来源：http://akq.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://rbj.gotoacloud.top

[U37] Py：读写 Excel
来源：http://jht.shangyingyoupin.top

pandas.read_excel / DataFrame.to_excel
来源：http://noe.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://iks.hesvh.cn

Path(__file__).resolve().parent
来源：http://iwy.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://zwl.fktsv.cn

sys.stdout.isatty()
来源：http://faz.jianghu66.top

[U40] Py：打印到标准错误
来源：http://iwr.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://zee.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://gjv.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zmh.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://gxf.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fhc.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://vwz.hywenlv.cn

namespace App\Http;
来源：http://iuy.redwolf501.top

[U44] PHP：开启严格类型
来源：http://ntj.nanxinkj.top

declare(strict_types=1);
来源：http://tqy.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://ibr.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ysm.tanke756.top

[U46] PHP：可空类型
来源：http://ecn.hongshengwenyu.top

?string $name = null
来源：http://cig.zhoulong.xyz

[U47] PHP：联合类型
来源：http://kpf.pengpengdd.cyou

int|string $id
来源：http://cye.aizwys.cn

[U48] PHP：纯枚举
来源：http://kuc.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yuv.cashguo.top

[U49] PHP：只读属性
来源：http://keq.ybcxt.top

public readonly string $name
来源：http://ljz.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://gvf.andypj.xyz

public function __construct(private int $id) {}
来源：http://cni.dianchejie.cn

[U51] PHP：数组解构
来源：http://hfu.mhx1999.top

[$a, $b] = $arr;
来源：http://hhm.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://ajg.xuetiantiany.cn

$double = fn($x) => $x * 2;
来源：http://dyh.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://ruy.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://lse.snrcjt.cn

[U54] PHP：空安全调用
来源：http://bhj.gaohongyu789.top

$obj?->method()
来源：http://hfc.chenlongwang.top

[U55] PHP：match 表达式
来源：http://gzb.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lsn.yongpay.top

[U56] PHP：命名参数
来源：http://tar.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://uej.xuanzx.com

[U57] PHP：字符串插值
来源：http://csx.iojbl.cn

"值: {$a}"
来源：http://lgv.zycfv.cn

[U58] PHP：数组三件套
来源：http://fpr.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vkc.yonumen.top

[U59] PHP：自定义排序
来源：http://sen.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hin.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://qot.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xei.chenjidiqi.icu

[U61] PHP：正则
来源：http://zrn.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qhe.fehbvm.com

[U62] PHP：日期对象
来源：http://xrj.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lft.smart0.xyz

[U63] PHP：文件读写
来源：http://rjo.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vgm.yonumen.top

[U64] PHP：目录遍历
来源：http://nyj.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://csy.gzhubu.top

[U65] PHP：会话
来源：http://ouq.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fmo.yonumen.top

[U66] PHP：设置 Cookie
来源：http://htl.aibaodan.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kdl.zhoulong.xyz

[U67] PHP：处理文件上传
来源：http://wjh.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cmm.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://kiq.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dcg.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://gav.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wjo.tianlin.xyz

[U70] PHP：PDO 事务
来源：http://qym.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dqv.yueranfly.top

[U71] PHP：抛出异常
来源：http://arm.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://vub.yonumen.top

[U72] PHP：写错误日志
来源：http://fkj.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://fpn.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://qcy.yonumen.top

parse_ini_file("config.ini", true)
来源：http://cnj.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://grq.quarkkingdee.top

getenv("APP_ENV") ?: "production"
来源：http://evv.yongpay.top

[U75] PHP：依赖注入
来源：http://mms.gogol.net.cn

composer require psr/container
来源：http://rff.sxryk.cn

[U76] PHP：简单路由
来源：http://kap.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bzu.zdbjq.cn

[U77] PHP：模板渲染
来源：http://tpp.cqqwz.cn

composer require twig/twig
来源：http://emg.tanke756.top

[U78] PHP：单元测试
来源：http://sdj.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://umv.fehbvm.com

[U79] PHP：静态分析
来源：http://zxb.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://ima.shanyushiyangtech.top

[U80] PHP：代码规范修复
来源：http://rqy.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qpr.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://yue.zhixingplan.top

npm init -y;  npm i express
来源：http://ioa.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://lwf.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aaj.cucudq.cn

[U83] JS：ES Module 导入导出
来源：http://mkt.yueranfly.top

export const a = 1;  import { a } from "./m.js";
来源：http://ugu.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://dpp.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://wxc.sweek.top

[U85] JS：可选链
来源：http://pin.uphjek.com

a?.b?.c
来源：http://fiy.yuanzhike.top

[U86] JS：空值合并
来源：http://wzc.jianghu66.top

a ?? b
来源：http://eht.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://zrb.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://qdm.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://sve.guowangkeji.top

{ ...a, ...b }
来源：http://xfh.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://idl.gogol.net.cn

[...new Set(arr)]
来源：http://bvb.meibo888.top

[U90] JS：数字数组排序
来源：http://fgo.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://sxt.meibo888.top

[U91] JS：对象键值遍历
来源：http://gph.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ylz.gotoacloud.top

[U92] JS：深拷贝
来源：http://fsj.yvedp.cn

structuredClone(obj)
来源：http://qff.zycfv.cn

[U93] JS：模板字符串
来源：http://atx.pycfn.com

`共 ${n} 条`
来源：http://gxm.yuanzhike.top

[U94] JS：箭头函数
来源：http://jrf.redwolf501.top

const double = x => x * 2;
来源：http://iad.dashuyun.cn

[U95] JS：Promise 包装
来源：http://jed.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://xsa.pycfn.com

[U96] JS：async/await 与异常
来源：http://qug.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bdf.zhiwuduotai.top

[U97] JS：并发请求
来源：http://vdk.hongshengwenyu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://nto.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://ioo.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rue.chenzaomai.com

[U99] JS：事件监听
来源：http://xww.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://fvk.fengsongda.top

[U100] JS：DOM 查询
来源：http://pzk.zdbjq.cn

document.querySelector(".item")
来源：http://ixp.meibo888.top

[U101] JS：classList 操作
来源：http://cgb.fzhhl.top

el.classList.toggle("active")
来源：http://mdm.tianlin.xyz

[U102] JS：本地存储
来源：http://xrg.ybcxt.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pwa.wangdashe.top

[U103] JS：定时器
来源：http://vwr.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xzp.chenzaomai.com

[U104] JS：防抖
来源：http://dny.wangshuangyany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://art.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://uqo.andypj.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wjd.yongpay.top

[U106] JS：日期格式化
来源：http://rpj.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://stn.hesvh.cn

[U107] JS：数字千分位
来源：http://cpj.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vri.shzxlz.cn

[U108] JS：随机整数
来源：http://eef.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://voy.smart0.xyz

[U109] JS：数组分组
来源：http://mzs.hnqzz.top

Object.groupBy(arr, x => x.type)
来源：http://xtw.jinqigufen.top

[U110] JS：数组分块
来源：http://rom.xylfe.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sra.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://jnu.gaohongyu789.top

new Map(Object.entries(obj))
来源：http://fvm.cqqwz.cn

[U112] JS：字符串补位
来源：http://cjy.birdmap.top

"7".padStart(3, "0")
来源：http://hop.hfpthk.cn

[U113] JS：正则替换全部
来源：http://adt.sxryk.cn

s.replaceAll("a", "b")
来源：http://nmq.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://iko.wangshuangyany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://thp.sjlbkw.cn

[U115] JS：生成 UUID
来源：http://hqz.ctjpmb.com

crypto.randomUUID()
来源：http://avu.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://sot.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://dhf.9152youxi.cn

[U117] JS：单元测试
来源：http://cmm.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://onw.havefunace.top

[U118] JS：开发服务器
来源：http://swi.ctjpmb.com

npm i -D vite;  npx vite
来源：http://tzw.zhijiandao.cn

[U119] JS：生产构建
来源：http://ejg.jyoumei.cn

npx vite build
来源：http://isu.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://akn.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://dns.ppjwa.cn

================================================================================
来源：http://clq.snrcjt.cn

统计汇总
来源：http://ouo.sweek.top

================================================================================
来源：http://yld.chenzaomai.com

按语言统计（条）：
来源：http://scf.daxiang520.top

Python ......... 252
来源：http://zrj.zhoulong.xyz

PHP ............ 252
来源：http://hfr.hfpthk.cn

JavaScript ..... 252
来源：http://oxr.bbcook.cn

TypeScript ..... 212
来源：http://pnn.chenjidiqi.icu

Java ........... 212
来源：http://khu.dianchejie.cn

Go ............. 212
来源：http://xnw.gogol.net.cn

Ruby ........... 212
来源：http://har.ctjpmb.com

C# ............. 212
来源：http://vmb.9152youxi.cn

C .............. 30
来源：http://yin.sysykeji.top

C++ ............ 30
来源：http://zie.yuanzhike.top

SQL ............ 90
来源：http://zvl.9152youxi.cn

Bash ........... 80
来源：http://yao.hongshengwenyu.top

Kotlin ......... 15
来源：http://elp.ydzc1.top

Swift .......... 15
来源：http://pbp.nanxuanxn.top

Lua ............ 10
来源：http://dso.hesvh.cn

Perl ........... 10
来源：http://vmf.wangshuangyany.cn

Scala .......... 10
来源：http://fno.yj202588.top

------------------------------------
来源：http://lhi.sweek.top

合计 ........... 2106 条
来源：http://rcj.gotoacloud.top

按章节统计：
来源：http://ize.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mrq.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xet.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yoj.fktsv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://clj.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fis.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://imo.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wyv.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tvo.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gsc.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://byz.haohaochexian.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fbe.jinyuanbaomall.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tau.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dtt.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xce.ybcxt.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ftc.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gsx.zhoulong.xyz

Q SQL 专题                              90
来源：http://etk.ydzc1.top

R Bash 专题                             80
来源：http://iuj.sxryk.cn

S C / C++ 专题                          60
来源：http://zsb.bbcook.cn

T 其他语言补充                          60
来源：http://yws.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://lse.bjfxy.top

------------------------------------
来源：http://xlq.feifeiyinyue.top

合计                                  2106 条
来源：http://uon.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://gdt.andypj.xyz

使用提醒
来源：http://ogf.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ckp.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ehn.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ble.yj20258888.top


<!-- 参考信息 -->