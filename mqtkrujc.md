代发 wailian999

[T41] Perl：Hello World
来源：http://vgt.zdbjq.cn

print "Hello\n";
来源：http://egj.fengsongda.top

[T42] Perl：变量类型
来源：http://mcp.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iqr.fktsv.cn

[T43] Perl：字符串插值
来源：http://mam.ctjpmb.com

"值: $a"
来源：http://lvq.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://mvm.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://rlj.shzxlz.cn

[T45] Perl：数组遍历
来源：http://ypw.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://jgy.sweek.top

[T46] Perl：哈希操作
来源：http://kkc.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bve.yuxming.cn

[T47] Perl：正则捕获
来源：http://nga.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hfx.snrcjt.cn

[T48] Perl：正则替换
来源：http://oyw.tian-w.cn

$s =~ s/old/new/g;
来源：http://don.hammf.cn

[T49] Perl：函数
来源：http://iue.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ijr.sxryk.cn

[T50] Perl：逐行读文件
来源：http://kkx.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tjn.daria6918.cn

while (my $line = <$fh>) { print $line; }
来源：http://pnh.fehbvm.com

[T51] Scala：Hello World
来源：http://kjt.yfazqb.com

println("Hello")
来源：http://uld.gotoacloud.top

[T52] Scala：变量
来源：http://iik.zhijiandao.cn

val a = 1;  var b = 2
来源：http://ecp.iojbl.cn

[T53] Scala：字符串插值
来源：http://psv.yvedp.cn

s"值: $b"
来源：http://efo.havefunace.top

[T54] Scala：集合映射
来源：http://ixu.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://ftw.shanyushiyangtech.top

[T55] Scala：集合过滤
来源：http://mjz.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://qrq.hnxiangtu.top

[T56] Scala：样例类
来源：http://pvq.jiagoushi.top

case class User(name: String, age: Int)
来源：http://bzs.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://zhn.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wpp.jinqigufen.top

[T58] Scala：函数定义
来源：http://stm.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://jty.uphjek.com

[T59] Scala：循环
来源：http://xgq.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://vyp.quarkkingdee.top

[T60] Scala：折叠
来源：http://bbr.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://get.shanyushiyangkeji.top

================================================================================
来源：http://mta.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tov.yj20258.top

================================================================================
来源：http://ivx.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://mic.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://ftu.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://yph.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tri.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://hjp.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dhw.yonumen.top

[U04] Py：变量调试打印
来源：http://ces.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://klv.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://bfj.yongpay.top

list(dict.fromkeys(arr))
来源：http://bwy.316326.xyz

[U06] Py：合并两个字典
来源：http://oue.gotoacloud.top

{**a, **b}
来源：http://tbl.jyoumei.cn

[U07] Py：反转字典键值
来源：http://fiv.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://khi.ybcxt.top

[U08] Py：展平二维列表
来源：http://nhe.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://nxw.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://eit.dianchejie.cn

max(d, key=d.get)
来源：http://fih.ppjwa.cn

[U10] Py：按值排序字典
来源：http://mat.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcg.gotoacloud.top

[U11] Py：生成器表达式
来源：http://yjq.fehbvm.com

(x * 2 for x in arr)
来源：http://hfq.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://dlp.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://vds.jinqigufen.top

[U13] Py：固定长度队列
来源：http://dui.jyoumei.cn

deque(maxlen=10)
来源：http://dtq.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://inm.feifeiyinyue.top

defaultdict(list)
来源：http://npl.tanke756.top

[U15] Py：高精度计时
来源：http://rvl.ehwqpu.com

t = time.perf_counter()
来源：http://qdw.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://pqu.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uln.tarul.cn

[U17] Py：初始化日志
来源：http://hto.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://gui.cheryme.top

[U18] Py：预编译正则
来源：http://kjy.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://pvb.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://tmn.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dlo.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://dnp.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://fvf.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://mus.bbcook.cn

@contextlib.contextmanager
来源：http://wue.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://nsv.fanxiaobao.xyz

list(zip(*m))
来源：http://joj.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://geq.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://euc.ehwqpu.com

[U24] Py：路径操作
来源：http://eqo.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jfa.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://dhc.zhengqikj.top

csv.DictReader(f)
来源：http://wbo.ctjpmb.com

[U26] Py：并发下载
来源：http://ewg.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hly.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://jpi.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://wzm.yj20258.top

[U28] Py：类型别名
来源：http://ywn.bjfxy.top

UserId = int
来源：http://sky.hywenlv.cn

[U29] Py：属性校验
来源：http://eyn.yonumen.top

@property 与 @x.setter 配合
来源：http://lvn.hammf.cn

[U30] Py：数据类
来源：http://ikk.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://gwc.chenzaomai.com

[U31] Py：单测
来源：http://sdo.shuidangran.top

python -m pytest -q
来源：http://ijv.sjlbkw.cn

[U32] Py：代码格式化
来源：http://eme.mhx1999.top

ruff format . && ruff check --fix .
来源：http://vvv.vehdjk.com

[U33] Py：打包发布
来源：http://zam.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://rit.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://xya.meibo888.top

chardet.detect(raw)
来源：http://rtc.birdmap.top

[U35] Py：发送邮件
来源：http://ddx.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aqd.cucudq.cn

[U36] Py：定时任务
来源：http://fqv.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://umx.cdnleiting.top

[U37] Py：读写 Excel
来源：http://swz.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://njj.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://elo.daria6918.cn

Path(__file__).resolve().parent
来源：http://hbj.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://oxo.xingfuxueyuan.xyz

sys.stdout.isatty()
来源：http://dsp.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://btm.chenlongwang.top

print("err", file=sys.stderr)
来源：http://zio.nwbrower.top

[U41] PHP：初始化 Composer 项目
来源：http://ulc.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tfu.meibo888.top

[U42] PHP：PSR-4 自动加载
来源：http://zms.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ebs.hnqzz.top

[U43] PHP：声明命名空间
来源：http://uxf.yj20258888.top

namespace App\Http;
来源：http://wpz.hcnkem.com

[U44] PHP：开启严格类型
来源：http://grw.ctjpmb.com

declare(strict_types=1);
来源：http://moj.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://hse.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://lrr.wangdashe.top

[U46] PHP：可空类型
来源：http://vsp.xuetiantiany.cn

?string $name = null
来源：http://otu.yongpay.top

[U47] PHP：联合类型
来源：http://bnq.jinghuilouyu.cn

int|string $id
来源：http://wta.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://ztc.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kcs.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://yes.c1oappe.top

public readonly string $name
来源：http://cxm.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://wyw.redwolf501.top

public function __construct(private int $id) {}
来源：http://zuh.ivvv.top

[U51] PHP：数组解构
来源：http://cnl.snrcjt.cn

[$a, $b] = $arr;
来源：http://lpt.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://bkh.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://bsp.yj202588.top

[U53] PHP：空合并运算符
来源：http://lfa.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://mtk.jyoumei.cn

[U54] PHP：空安全调用
来源：http://lil.jlsjyb.cn

$obj?->method()
来源：http://ojp.dianchejie.cn

[U55] PHP：match 表达式
来源：http://bsn.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wqb.gaohongyu789.top

[U56] PHP：命名参数
来源：http://ztx.xziqi.cn

f(a: 1, b: 2)
来源：http://oti.ydzc1.top

[U57] PHP：字符串插值
来源：http://ukp.zhongyouzk.top

"值: {$a}"
来源：http://zdp.gogol.net.cn

[U58] PHP：数组三件套
来源：http://ici.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qaz.pengpengdd.cyou

[U59] PHP：自定义排序
来源：http://gkf.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kbi.shuidangran.top

[U60] PHP：JSON 编解码
来源：http://fpa.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://syi.sweek.top

[U61] PHP：正则
来源：http://oyw.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://daf.sysykeji.top

[U62] PHP：日期对象
来源：http://atj.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://slw.zhongyouzk.top

[U63] PHP：文件读写
来源：http://mpe.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://myb.chenlongwang.top

[U64] PHP：目录遍历
来源：http://xmi.ydjk.org.cn

glob("dir/*.php");  scandir("dir");
来源：http://rfr.nanxinkj.top

[U65] PHP：会话
来源：http://bqx.bbcook.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sxk.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://ckb.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://src.gzhubu.top

[U67] PHP：处理文件上传
来源：http://bez.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lmr.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://wig.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hnk.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://puf.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://olm.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://ydz.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pdm.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://lsl.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://ptk.jyoumei.cn

[U72] PHP：写错误日志
来源：http://fpd.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://myv.hammf.cn

[U73] PHP：读取 ini 配置
来源：http://smj.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://vun.gogol.net.cn

[U74] PHP：读取环境变量
来源：http://kho.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://gtt.jinqigufen.top

[U75] PHP：依赖注入
来源：http://ckj.shanyushiyangkeji.top

composer require psr/container
来源：http://iyl.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://jwa.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gft.hywenlv.cn

[U77] PHP：模板渲染
来源：http://qln.yanxiufei.cn

composer require twig/twig
来源：http://ogl.zhongyouzk.top

[U78] PHP：单元测试
来源：http://lhw.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://cgm.yangfankeji.com

[U79] PHP：静态分析
来源：http://vrf.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://cao.wangdashe.top

[U80] PHP：代码规范修复
来源：http://yrz.fktsv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kaf.mhx1999.top

[U81] JS：初始化项目
来源：http://xvb.feifeiyinyue.top

npm init -y;  npm i express
来源：http://xuf.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://qqi.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ztk.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://iko.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://cmx.chenjidiqi.icu

[U84] JS：CommonJS 写法
来源：http://mcq.shzxlz.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fro.zhengqikj.top

[U85] JS：可选链
来源：http://tas.svipenyu.cn

a?.b?.c
来源：http://idr.yvedp.cn

[U86] JS：空值合并
来源：http://cyl.aizwys.cn

a ?? b
来源：http://ypy.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://wrz.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://gqu.cqqwz.cn

[U88] JS：对象展开合并
来源：http://fve.haohaochexian.top

{ ...a, ...b }
来源：http://acj.ppjwa.cn

[U89] JS：数组去重
来源：http://xnx.hfpthk.cn

[...new Set(arr)]
来源：http://lsi.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://hqy.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://pqa.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://rqv.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bff.iojbl.cn

[U92] JS：深拷贝
来源：http://awk.aibaodan.cn

structuredClone(obj)
来源：http://bel.zhoulong.xyz

[U93] JS：模板字符串
来源：http://hry.gotoacloud.top

`共 ${n} 条`
来源：http://tvx.c1oappe.top

[U94] JS：箭头函数
来源：http://uda.sufxvd.cn

const double = x => x * 2;
来源：http://mvf.bjfxy.top

[U95] JS：Promise 包装
来源：http://zch.ydzc1.top

new Promise((resolve, reject) => {})
来源：http://orh.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://isn.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xin.smart0.xyz

[U97] JS：并发请求
来源：http://lhw.hnxiangtu.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ilj.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://uxe.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pjv.tianlin.xyz

[U99] JS：事件监听
来源：http://rkc.52xcode.cn

el.addEventListener("click", e => {})
来源：http://nfe.zhengqikj.top

[U100] JS：DOM 查询
来源：http://fxf.cdnleiting.top

document.querySelector(".item")
来源：http://ycg.pycfn.com

[U101] JS：classList 操作
来源：http://enj.yj20258888.top

el.classList.toggle("active")
来源：http://yow.sysykeji.top

[U102] JS：本地存储
来源：http://rpy.yongpay.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zez.jqgufenzy.top

[U103] JS：定时器
来源：http://nsx.fehbvm.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jzc.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://nyc.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynr.cqqwz.cn

[U105] JS：节流
来源：http://qsu.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sqt.zdbjq.cn

[U106] JS：日期格式化
来源：http://ymm.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iem.tianlin.xyz

[U107] JS：数字千分位
来源：http://mem.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qwv.guowangkeji.top

[U108] JS：随机整数
来源：http://usk.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://omw.9152youxi.cn

[U109] JS：数组分组
来源：http://wqu.fanxiaobao.xyz

Object.groupBy(arr, x => x.type)
来源：http://doy.hysaishi.cn

[U110] JS：数组分块
来源：http://hup.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rss.ybcxt.top

[U111] JS：对象转 Map
来源：http://dnw.9152youxi.cn

new Map(Object.entries(obj))
来源：http://tgd.jinqigufen.top

[U112] JS：字符串补位
来源：http://mav.jyoumei.cn

"7".padStart(3, "0")
来源：http://whu.jinqigfzy.top

[U113] JS：正则替换全部
来源：http://pzl.xziqi.cn

s.replaceAll("a", "b")
来源：http://wam.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://cii.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqb.cheryme.top

[U115] JS：生成 UUID
来源：http://zlu.pengpengdd.cyou

crypto.randomUUID()
来源：http://wci.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://jfo.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://zxx.nwbrower.top

[U117] JS：单元测试
来源：http://zgt.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://lzc.jinqigfzy.top

[U118] JS：开发服务器
来源：http://byy.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://yil.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://vpg.ehwqpu.com

npx vite build
来源：http://prd.ivvv.top

[U120] JS：读取环境变量（Vite）
来源：http://ewx.jinghuilouyu.cn

import.meta.env.VITE_API_URL
来源：http://jmw.ydjk.org.cn

================================================================================
来源：http://aml.hfpthk.cn

统计汇总
来源：http://ahu.jqgfzy.top

================================================================================
来源：http://dmb.fehbvm.com

按语言统计（条）：
来源：http://tbs.epnwcf.com

Python ......... 252
来源：http://xex.haohaochexian.top

PHP ............ 252
来源：http://mmo.zhoulong.xyz

JavaScript ..... 252
来源：http://xkp.fzhhl.top

TypeScript ..... 212
来源：http://dtv.yonumen.top

Java ........... 212
来源：http://gdi.yj20258888.top

Go ............. 212
来源：http://rhi.bjfxy.top

Ruby ........... 212
来源：http://blv.chenjidiqi.icu

C# ............. 212
来源：http://igb.ivvv.top

C .............. 30
来源：http://biq.quarkkingdee.top

C++ ............ 30
来源：http://tau.shanyushiyangkeji.top

SQL ............ 90
来源：http://kde.birdmap.top

Bash ........... 80
来源：http://liu.yuanzhike.top


<!-- 参考信息 -->