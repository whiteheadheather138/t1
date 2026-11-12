代发 wailian999

[T37] Lua：字符串拼接
来源：http://fit.jqgufenzy.top

"a" .. "b"
来源：http://nxj.yanxiufei.cn

[T38] Lua：条件
来源：http://mkx.vehdjk.com

if x > 0 then print("正") end
来源：http://abu.52xcode.cn

[T39] Lua：模式匹配
来源：http://djn.yangfankeji.com

string.find(s, "%d+")
来源：http://gkw.yangfankeji.com

[T40] Lua：元表
来源：http://izb.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://zdh.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://kmv.sysykeji.top

print "Hello\n";
来源：http://sfe.gogol.net.cn

[T42] Perl：变量类型
来源：http://uay.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vso.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://qby.zhiwuduotai.top

"值: $a"
来源：http://dui.chenlongwang.top

[T44] Perl：条件
来源：http://tnp.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://vhf.pycfn.com

[T45] Perl：数组遍历
来源：http://niv.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://bvb.redwolf501.top

[T46] Perl：哈希操作
来源：http://lzp.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bjw.guowangkeji.top

[T47] Perl：正则捕获
来源：http://kll.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tdn.sysykeji.top

[T48] Perl：正则替换
来源：http://goi.hammf.cn

$s =~ s/old/new/g;
来源：http://pqa.nanxinkj.top

[T49] Perl：函数
来源：http://fhp.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sbu.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://fao.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zgl.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://ryi.zhoulong.xyz

[T51] Scala：Hello World
来源：http://qch.cucudq.cn

println("Hello")
来源：http://irl.tarul.cn

[T52] Scala：变量
来源：http://lzj.daxiang520.top

val a = 1;  var b = 2
来源：http://pkf.tianlin.xyz

[T53] Scala：字符串插值
来源：http://feo.sysykeji.top

s"值: $b"
来源：http://den.tianlin.xyz

[T54] Scala：集合映射
来源：http://osi.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://yhb.hcnkem.com

[T55] Scala：集合过滤
来源：http://cae.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mzl.xuetiantiany.cn

[T56] Scala：样例类
来源：http://dez.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://hdq.ivvv.top

[T57] Scala：模式匹配
来源：http://fvm.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://goz.jinqigfzy.top

[T58] Scala：函数定义
来源：http://xzu.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://cbz.chenzaomai.com

[T59] Scala：循环
来源：http://xmj.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://uqt.gogol.net.cn

[T60] Scala：折叠
来源：http://dhh.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vhm.fktsv.cn

================================================================================
来源：http://nnc.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rll.jinyuanbaomall.cn

================================================================================
来源：http://snw.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://arw.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://hby.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://vst.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xjs.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://ksn.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ezg.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://bzw.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://txc.hesvh.cn

[U05] Py：列表去重且保序
来源：http://lhq.wangdashe.top

list(dict.fromkeys(arr))
来源：http://cem.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://coq.shanyushiyangtech.top

{**a, **b}
来源：http://odr.daria6918.cn

[U07] Py：反转字典键值
来源：http://ynr.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://lji.fengsongda.top

[U08] Py：展平二维列表
来源：http://snn.epnwcf.com

[y for x in nested for y in x]
来源：http://jvs.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://wmv.shuidangran.top

max(d, key=d.get)
来源：http://yjs.xziqi.cn

[U10] Py：按值排序字典
来源：http://rzx.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://awb.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://wac.nanxuanxn.top

(x * 2 for x in arr)
来源：http://mcb.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://qgx.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://olc.wangdashe.top

[U13] Py：固定长度队列
来源：http://ypo.uphjek.com

deque(maxlen=10)
来源：http://yaw.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://mss.haohaochexian.top

defaultdict(list)
来源：http://qav.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://yiw.xuetiantiany.cn

t = time.perf_counter()
来源：http://qib.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://use.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wef.yuanzhike.top

[U17] Py：初始化日志
来源：http://ftc.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://zqh.yvedp.cn

[U18] Py：预编译正则
来源：http://dhn.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://jqg.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://rbe.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gdk.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://bua.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://yym.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://uaf.meibo888.top

@contextlib.contextmanager
来源：http://ggl.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://yrg.guannengcc.top

list(zip(*m))
来源：http://bve.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://uxb.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://edn.yuanzhike.top

[U24] Py：路径操作
来源：http://rkz.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uao.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://sod.c1oappe.top

csv.DictReader(f)
来源：http://xfe.cucudq.cn

[U26] Py：并发下载
来源：http://cod.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ytk.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://fgu.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://fim.vehdjk.com

[U28] Py：类型别名
来源：http://tys.guowangkeji.top

UserId = int
来源：http://cyq.yangfankeji.com

[U29] Py：属性校验
来源：http://kea.guannengcc.top

@property 与 @x.setter 配合
来源：http://scc.zdqjudy.top

[U30] Py：数据类
来源：http://vpl.yj20258.top

@dataclass(slots=True)
来源：http://mso.ydzc1.top

[U31] Py：单测
来源：http://sfl.tanke756.top

python -m pytest -q
来源：http://kql.hnxiangtu.top

[U32] Py：代码格式化
来源：http://eaz.vehdjk.com

ruff format . && ruff check --fix .
来源：http://qgo.yuxming.cn

[U33] Py：打包发布
来源：http://txi.aibaodan.cn

python -m build  （依赖 pyproject.toml）
来源：http://sdy.chenzaomai.com

[U34] Py：判断编码
来源：http://kim.yfazqb.com

chardet.detect(raw)
来源：http://kcu.nanxinkj.top

[U35] Py：发送邮件
来源：http://kfu.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oeg.hnxiangtu.top

[U36] Py：定时任务
来源：http://pzi.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://bne.gogol.net.cn

[U37] Py：读写 Excel
来源：http://dul.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://fec.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://wzk.cheryme.top

Path(__file__).resolve().parent
来源：http://kuz.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://tcs.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://pqc.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://iqh.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://ibv.ehwqpu.com

[U41] PHP：初始化 Composer 项目
来源：http://iyj.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wpa.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://umm.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lqd.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://jft.sufxvd.cn

namespace App\Http;
来源：http://jzs.ydzc1.top

[U44] PHP：开启严格类型
来源：http://mjt.yj20258.top

declare(strict_types=1);
来源：http://jmo.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://jvd.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lee.iojbl.cn

[U46] PHP：可空类型
来源：http://ldl.jinqigfzy.top

?string $name = null
来源：http://iur.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://zac.jiagoushi.top

int|string $id
来源：http://dud.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://nhx.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zrw.52xcode.cn

[U49] PHP：只读属性
来源：http://dcd.xingfuxueyuan.xyz

public readonly string $name
来源：http://jlg.yonumen.top

[U50] PHP：构造器属性提升
来源：http://vlg.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://ixl.yj20258.top

[U51] PHP：数组解构
来源：http://abf.meibo888.top

[$a, $b] = $arr;
来源：http://eyj.zdqjudy.top

[U52] PHP：箭头函数
来源：http://coc.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://ere.yj20258.top

[U53] PHP：空合并运算符
来源：http://uxq.jqgufenzy.top

$v = $a ?? $b ?? "default";
来源：http://vsy.jyoumei.cn

[U54] PHP：空安全调用
来源：http://usw.tanke756.top

$obj?->method()
来源：http://hlf.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://ugl.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wed.yvedp.cn

[U56] PHP：命名参数
来源：http://bqi.ybcxt.top

f(a: 1, b: 2)
来源：http://dls.chenlongwang.top

[U57] PHP：字符串插值
来源：http://zit.ydjk.org.cn

"值: {$a}"
来源：http://pgk.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://qyc.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wvg.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://ptd.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsw.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://odr.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qoa.guannengcc.top

[U61] PHP：正则
来源：http://sxz.ywan-chungtsiang.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ble.cashguo.top

[U62] PHP：日期对象
来源：http://ymv.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://evk.cqqwz.cn

[U63] PHP：文件读写
来源：http://aeu.jyoumei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qkz.yongpay.top

[U64] PHP：目录遍历
来源：http://hoa.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://gvg.zhongyouzk.top

[U65] PHP：会话
来源：http://ixt.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://isl.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://dsc.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vdq.uphjek.com

[U67] PHP：处理文件上传
来源：http://yqh.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aet.meibo888.top

[U68] PHP：PDO 连接
来源：http://txx.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kno.jinqigfzy.top

[U69] PHP：PDO 预处理
来源：http://wkh.dashuyun.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sur.hongshengwenyu.top

[U70] PHP：PDO 事务
来源：http://gnc.jqgfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fnx.redwolf501.top

[U71] PHP：抛出异常
来源：http://mbu.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://wso.bjfxy.top

[U72] PHP：写错误日志
来源：http://knr.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://xis.hongshengwenyu.top

[U73] PHP：读取 ini 配置
来源：http://tfb.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://fwt.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://suj.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://zep.c1oappe.top

[U75] PHP：依赖注入
来源：http://juy.xylfe.cn

composer require psr/container
来源：http://ftj.epnwcf.com

[U76] PHP：简单路由
来源：http://jdd.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xkl.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://mlc.bjfxy.top

composer require twig/twig
来源：http://pkd.nanxuanxn.top

[U78] PHP：单元测试
来源：http://kpl.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://edc.jianghu66.top

[U79] PHP：静态分析
来源：http://feu.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://ptu.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://azh.shuidangran.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://smn.wangdashe.top

[U81] JS：初始化项目
来源：http://bkd.fengsongda.top

npm init -y;  npm i express
来源：http://ggr.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://yqk.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pnt.sweek.top

[U83] JS：ES Module 导入导出
来源：http://sbd.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://wxz.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://lun.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gii.jinqigfzy.top

[U85] JS：可选链
来源：http://wxo.svipenyu.cn

a?.b?.c
来源：http://xpy.cashguo.top

[U86] JS：空值合并
来源：http://pqo.zhixingplan.top

a ?? b
来源：http://hpf.yanxiufei.cn

[U87] JS：解构默认值
来源：http://jnw.cheryme.top

const { a = 1, b = 2 } = obj;
来源：http://qmz.jqgfzy.top

[U88] JS：对象展开合并
来源：http://xsk.cheryme.top

{ ...a, ...b }
来源：http://mkq.jianghu66.top

[U89] JS：数组去重
来源：http://bwp.shangyingyoupin.top

[...new Set(arr)]
来源：http://taq.gotoacloud.top

[U90] JS：数字数组排序
来源：http://aan.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://tid.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://akh.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oxb.yongpay.top

[U92] JS：深拷贝
来源：http://rjj.nanxinkj.top

structuredClone(obj)
来源：http://eii.hesvh.cn

[U93] JS：模板字符串
来源：http://epb.chenlongwang.top

`共 ${n} 条`
来源：http://xhv.ybcxt.top

[U94] JS：箭头函数
来源：http://tjz.bbcook.cn

const double = x => x * 2;
来源：http://ikg.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://bsn.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://nqi.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://ssz.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kbp.xuanzx.com

[U97] JS：并发请求
来源：http://nla.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ckg.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://dto.316326.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://van.havefunace.top

[U99] JS：事件监听
来源：http://pfi.yfazqb.com

el.addEventListener("click", e => {})
来源：http://zba.wangdashe.top

[U100] JS：DOM 查询
来源：http://ooa.yuxming.cn

document.querySelector(".item")
来源：http://unj.jiagoushi.top

[U101] JS：classList 操作
来源：http://ors.iojbl.cn

el.classList.toggle("active")
来源：http://sku.pycfn.com

[U102] JS：本地存储
来源：http://ttr.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://ojs.wangshuangyany.cn

[U103] JS：定时器
来源：http://qlo.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uxe.zhiwuduotai.top

[U104] JS：防抖
来源：http://mtn.daxiang520.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vts.jyoumei.cn

[U105] JS：节流
来源：http://jrs.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hfx.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://far.chenzaomai.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nlg.0kj1m.cn

[U107] JS：数字千分位
来源：http://rfi.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qdp.tianlin.xyz

[U108] JS：随机整数
来源：http://vhd.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rwg.zhijiandao.cn

[U109] JS：数组分组
来源：http://ocu.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://cgl.sufxvd.cn

[U110] JS：数组分块
来源：http://fhg.hongshengwenyu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ijr.ppjwa.cn

[U111] JS：对象转 Map
来源：http://mgf.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://wom.hfpthk.cn

[U112] JS：字符串补位
来源：http://zpy.zhixingplan.top

"7".padStart(3, "0")
来源：http://qqy.ivvv.top

[U113] JS：正则替换全部
来源：http://lkb.jinqigufen.top

s.replaceAll("a", "b")
来源：http://tgg.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://nkr.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://upv.ywan-chungtsiang.top

[U115] JS：生成 UUID
来源：http://exd.zhixingplan.top

crypto.randomUUID()
来源：http://imo.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://meu.sjlbkw.cn

/** @param {string} name */ function f(name) {}
来源：http://abi.zhoulong.xyz

[U117] JS：单元测试
来源：http://ift.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://vte.zdqjudy.top

[U118] JS：开发服务器
来源：http://pyj.nanxinkj.top

npm i -D vite;  npx vite
来源：http://ykk.smart0.xyz

[U119] JS：生产构建
来源：http://yil.xuanzx.com

npx vite build
来源：http://nyh.xuanzx.com

[U120] JS：读取环境变量（Vite）
来源：http://dgj.ywan-chungtsiang.top

import.meta.env.VITE_API_URL
来源：http://nbz.sysykeji.top

================================================================================
来源：http://xrt.iojbl.cn

统计汇总
来源：http://fan.sufxvd.cn

================================================================================
来源：http://upy.nanxuanxn.top

按语言统计（条）：
来源：http://hff.nanxinkj.top

Python ......... 252
来源：http://kqc.shangyingyoupin.top

PHP ............ 252
来源：http://igz.sjlbkw.cn

JavaScript ..... 252
来源：http://yse.redwolf501.top

TypeScript ..... 212
来源：http://erd.jinqigfzy.top


<!-- 参考信息 -->