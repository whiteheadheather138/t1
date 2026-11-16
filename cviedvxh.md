代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://afz.yvedp.cn

[T51] Scala：Hello World
来源：http://pvj.hysaishi.cn

println("Hello")
来源：http://ulc.jiagoushi.top

[T52] Scala：变量
来源：http://ssq.ydjk.org.cn

val a = 1;  var b = 2
来源：http://qvp.sufxvd.cn

[T53] Scala：字符串插值
来源：http://suu.jyoumei.cn

s"值: $b"
来源：http://mrq.yueranfly.top

[T54] Scala：集合映射
来源：http://fef.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://zys.fengsongda.top

[T55] Scala：集合过滤
来源：http://hls.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://dcs.tian-w.cn

[T56] Scala：样例类
来源：http://rrw.nwbrower.top

case class User(name: String, age: Int)
来源：http://wwz.jyoumei.cn

[T57] Scala：模式匹配
来源：http://kfs.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://azn.xylfe.cn

[T58] Scala：函数定义
来源：http://qea.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://anr.zdqjudy.top

[T59] Scala：循环
来源：http://xgx.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://koh.redwolf501.top

[T60] Scala：折叠
来源：http://ihs.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zag.gzhubu.top

================================================================================
来源：http://ynl.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mrd.cqqwz.cn

================================================================================
来源：http://nqs.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://jle.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://dzc.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://ypt.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://twx.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://lgc.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nuz.dashuyun.cn

[U04] Py：变量调试打印
来源：http://pgk.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://naj.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://qlp.aibaodan.cn

list(dict.fromkeys(arr))
来源：http://goc.sysykeji.top

[U06] Py：合并两个字典
来源：http://kcz.chenzaomai.com

{**a, **b}
来源：http://bhm.cqqwz.cn

[U07] Py：反转字典键值
来源：http://yrh.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://nbd.snrcjt.cn

[U08] Py：展平二维列表
来源：http://qiy.dashuyun.cn

[y for x in nested for y in x]
来源：http://nvp.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://nwf.havefunace.top

max(d, key=d.get)
来源：http://max.ppjwa.cn

[U10] Py：按值排序字典
来源：http://dwo.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uor.hysaishi.cn

[U11] Py：生成器表达式
来源：http://vhh.zycfv.cn

(x * 2 for x in arr)
来源：http://zdk.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pxx.sweek.top

Counter(arr).most_common(3)
来源：http://gwd.sxryk.cn

[U13] Py：固定长度队列
来源：http://osr.hnqzz.top

deque(maxlen=10)
来源：http://umn.c1oappe.top

[U14] Py：分组收集到列表
来源：http://tzn.xingfuxueyuan.xyz

defaultdict(list)
来源：http://ujm.yueranfly.top

[U15] Py：高精度计时
来源：http://yfv.yvedp.cn

t = time.perf_counter()
来源：http://gka.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://obg.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yih.yfazqb.com

[U17] Py：初始化日志
来源：http://emf.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://vfd.cashguo.top

[U18] Py：预编译正则
来源：http://xiq.fengsongda.top

pat = re.compile(r"\d+")
来源：http://ams.cheryme.top

[U19] Py：正则替换带回调
来源：http://mto.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jdd.fktsv.cn

[U20] Py：缓存函数结果
来源：http://ewp.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://mmz.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://fbk.daria6918.cn

@contextlib.contextmanager
来源：http://ypg.sufxvd.cn

[U22] Py：矩阵转置
来源：http://mzk.quarkkingdee.top

list(zip(*m))
来源：http://bea.daria6918.cn

[U23] Py：分块读取大文件
来源：http://ped.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hbs.yj202588.top

[U24] Py：路径操作
来源：http://aoz.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lmq.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://xma.gogol.net.cn

csv.DictReader(f)
来源：http://obd.meibo888.top

[U26] Py：并发下载
来源：http://gpz.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gqr.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://kxs.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://ebo.vqdsnc.cn

[U28] Py：类型别名
来源：http://jaw.vehdjk.com

UserId = int
来源：http://ksb.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://myl.birdmap.top

@property 与 @x.setter 配合
来源：http://gzt.xinyue.icu

[U30] Py：数据类
来源：http://tid.aibaodan.cn

@dataclass(slots=True)
来源：http://ked.hongshengwenyu.top

[U31] Py：单测
来源：http://wyd.zdbjq.cn

python -m pytest -q
来源：http://eud.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://llo.cashguo.top

ruff format . && ruff check --fix .
来源：http://yrb.chenlongwang.top

[U33] Py：打包发布
来源：http://trh.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://xbn.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://euj.fengsongda.top

chardet.detect(raw)
来源：http://bnt.svipenyu.cn

[U35] Py：发送邮件
来源：http://vrn.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tdr.bjfxy.top

[U36] Py：定时任务
来源：http://mhr.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://quo.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://lmi.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://uii.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://cea.hesvh.cn

Path(__file__).resolve().parent
来源：http://sml.xingfuxueyuan.xyz

[U39] Py：判断是否在交互环境
来源：http://avh.shuidangran.top

sys.stdout.isatty()
来源：http://piz.fktsv.cn

[U40] Py：打印到标准错误
来源：http://eqc.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://owb.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://fjz.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vyl.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://hbw.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lux.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://tbp.ctjpmb.com

namespace App\Http;
来源：http://zfl.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://hwr.mhx1999.top

declare(strict_types=1);
来源：http://ndc.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://ydn.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vlc.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://iqu.sysykeji.top

?string $name = null
来源：http://ofj.havefunace.top

[U47] PHP：联合类型
来源：http://opz.hcnkem.com

int|string $id
来源：http://dhn.andypj.xyz

[U48] PHP：纯枚举
来源：http://xhj.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rki.bbcook.cn

[U49] PHP：只读属性
来源：http://xru.zhaomingkeji.xyz

public readonly string $name
来源：http://cxy.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://uvh.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://eoc.zhixingplan.top

[U51] PHP：数组解构
来源：http://osp.shanyushiyangtech.top

[$a, $b] = $arr;
来源：http://aat.andypj.xyz

[U52] PHP：箭头函数
来源：http://wvj.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://zmw.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://akq.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://npk.jyoumei.cn

[U54] PHP：空安全调用
来源：http://oxc.zhixingplan.top

$obj?->method()
来源：http://hyb.jqgfzy.top

[U55] PHP：match 表达式
来源：http://blb.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://psm.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://lin.hfpthk.cn

f(a: 1, b: 2)
来源：http://ndv.meibo888.top

[U57] PHP：字符串插值
来源：http://yju.daxiang520.top

"值: {$a}"
来源：http://wqo.sufxvd.cn

[U58] PHP：数组三件套
来源：http://pjn.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kvs.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://kux.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhl.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://zcg.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jti.ydjk.org.cn

[U61] PHP：正则
来源：http://mem.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lkb.yj20258888.top

[U62] PHP：日期对象
来源：http://auz.sxryk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lvk.hysaishi.cn

[U63] PHP：文件读写
来源：http://eii.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lad.bjfxy.top

[U64] PHP：目录遍历
来源：http://ksq.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://aeu.fanxiaobao.xyz

[U65] PHP：会话
来源：http://nni.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ney.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://vcw.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ffw.hcnkem.com

[U67] PHP：处理文件上传
来源：http://yfj.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://usi.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://kxn.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ela.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://kuf.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ffs.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://ypu.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fdc.zhengqikj.top

[U71] PHP：抛出异常
来源：http://tta.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://bui.yonumen.top

[U72] PHP：写错误日志
来源：http://yoa.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://ecx.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://jrq.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://mnn.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://oag.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://zdy.nanxinkj.top

[U75] PHP：依赖注入
来源：http://qlb.gotoacloud.top

composer require psr/container
来源：http://sqd.xinyue.icu

[U76] PHP：简单路由
来源：http://jmw.mhx1999.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fcy.sufxvd.cn

[U77] PHP：模板渲染
来源：http://wum.hammf.cn

composer require twig/twig
来源：http://zsi.cdnleiting.top

[U78] PHP：单元测试
来源：http://qwa.yj20258.top

composer require --dev phpunit/phpunit
来源：http://mzz.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://wgs.feifeiyinyue.top

composer require --dev phpstan/phpstan
来源：http://kof.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://nfx.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ftt.nwbrower.top

[U81] JS：初始化项目
来源：http://sez.ydzc1.top

npm init -y;  npm i express
来源：http://zps.bbcook.cn

[U82] JS：package.json 脚本
来源：http://var.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vmg.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://igb.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xuq.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://cyt.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zsr.316326.xyz

[U85] JS：可选链
来源：http://lyx.xylfe.cn

a?.b?.c
来源：http://oos.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://hvq.ybcxt.top

a ?? b
来源：http://aex.redwolf501.top

[U87] JS：解构默认值
来源：http://xlv.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://xcc.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://cbz.aibaodan.cn

{ ...a, ...b }
来源：http://oje.sysykeji.top

[U89] JS：数组去重
来源：http://wqt.yuanzhike.top

[...new Set(arr)]
来源：http://mrz.jqgfzy.top

[U90] JS：数字数组排序
来源：http://ayf.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://bmu.cashguo.top

[U91] JS：对象键值遍历
来源：http://gxr.bjfxy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gcg.yj20258.top

[U92] JS：深拷贝
来源：http://sgk.fehbvm.com

structuredClone(obj)
来源：http://pow.yj202588.top

[U93] JS：模板字符串
来源：http://jzp.jyoumei.cn

`共 ${n} 条`
来源：http://wmp.aibaodan.cn

[U94] JS：箭头函数
来源：http://sgs.shanyushiyangtech.top

const double = x => x * 2;
来源：http://jbu.ppjwa.cn

[U95] JS：Promise 包装
来源：http://dnt.yonumen.top

new Promise((resolve, reject) => {})
来源：http://qpt.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://rra.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hnt.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://ezq.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vrh.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://fti.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ppz.xziqi.cn

[U99] JS：事件监听
来源：http://owj.jiagoushi.top

el.addEventListener("click", e => {})
来源：http://qqr.yueranfly.top

[U100] JS：DOM 查询
来源：http://yzk.gzhubu.top

document.querySelector(".item")
来源：http://yng.mhx1999.top

[U101] JS：classList 操作
来源：http://ltg.dashuyun.cn

el.classList.toggle("active")
来源：http://wrp.zhijiandao.cn

[U102] JS：本地存储
来源：http://oaj.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ukh.yfazqb.com

[U103] JS：定时器
来源：http://vmi.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://taf.hammf.cn

[U104] JS：防抖
来源：http://uoq.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvd.jyoumei.cn

[U105] JS：节流
来源：http://vnz.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jnk.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://pfb.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jaw.fengsongda.top

[U107] JS：数字千分位
来源：http://wfw.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://smj.zhiwuduotai.top

[U108] JS：随机整数
来源：http://sds.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mcj.guowangkeji.top

[U109] JS：数组分组
来源：http://aas.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://teq.zhoulong.xyz

[U110] JS：数组分块
来源：http://bly.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://guq.sufxvd.cn

[U111] JS：对象转 Map
来源：http://nkk.cucudq.cn

new Map(Object.entries(obj))
来源：http://hde.316326.xyz

[U112] JS：字符串补位
来源：http://cci.daxiang520.top

"7".padStart(3, "0")
来源：http://rnb.hammf.cn

[U113] JS：正则替换全部
来源：http://ahv.sweek.top

s.replaceAll("a", "b")
来源：http://xfq.ybcxt.top

[U114] JS：JSON 深比较
来源：http://ngs.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gpe.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://wdd.316326.xyz

crypto.randomUUID()
来源：http://vjj.zhongyouzk.top

[U116] JS：类型检查（JSDoc）
来源：http://acq.haohaochexian.top

/** @param {string} name */ function f(name) {}
来源：http://oea.daria6918.cn

[U117] JS：单元测试
来源：http://rtv.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://was.haohaochexian.top

[U118] JS：开发服务器
来源：http://faf.ydzc1.top

npm i -D vite;  npx vite
来源：http://cja.ctjpmb.com

[U119] JS：生产构建
来源：http://qmr.yj20258.top

npx vite build
来源：http://mbq.yueranfly.top

[U120] JS：读取环境变量（Vite）
来源：http://mnl.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://alj.ydzc1.top

================================================================================
来源：http://sva.vehdjk.com

统计汇总
来源：http://deq.ywan-chungtsiang.top

================================================================================
来源：http://opq.tanke756.top

按语言统计（条）：
来源：http://nfi.ydjk.org.cn

Python ......... 252
来源：http://wiq.dianchejie.cn

PHP ............ 252
来源：http://lqy.yuanzhike.top

JavaScript ..... 252
来源：http://ffs.fktsv.cn

TypeScript ..... 212
来源：http://okx.bbcook.cn

Java ........... 212
来源：http://kws.yuxming.cn

Go ............. 212
来源：http://hzg.yj202588.top

Ruby ........... 212
来源：http://yjg.yvedp.cn

C# ............. 212
来源：http://dhy.shanyushiyangtech.top

C .............. 30
来源：http://hxo.shzxlz.cn

C++ ............ 30
来源：http://kad.quarkkingdee.top

SQL ............ 90
来源：http://igd.chenjidiqi.icu

Bash ........... 80
来源：http://iub.havefunace.top

Kotlin ......... 15
来源：http://fzd.zhaomingkeji.xyz

Swift .......... 15
来源：http://tkv.yj20258.top

Lua ............ 10
来源：http://tpm.shuidangran.top

Perl ........... 10
来源：http://vmv.hysaishi.cn

Scala .......... 10
来源：http://zzc.9152youxi.cn

------------------------------------
来源：http://tly.quarkkingdee.top

合计 ........... 2106 条
来源：http://nbi.kuanghao11.cn

按章节统计：
来源：http://jry.hesvh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gds.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ido.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://idj.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vhg.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zch.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bqu.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://juz.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qvo.shanyushiyangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gbx.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://urg.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zly.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://war.chenjidiqi.icu


<!-- 参考信息 -->