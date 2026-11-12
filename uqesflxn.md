代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xzx.yj20258888.top

[S51] C++：显式类型转换
来源：http://qet.cucudq.cn

static_cast<double>(a) / b
来源：http://xyi.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://eas.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://ttl.hysaishi.cn

[S53] C++：移动语义
来源：http://esi.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://wok.ctjpmb.com

[S54] C++：异常处理
来源：http://fxn.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xdl.yfazqb.com

[S55] C++：结构化绑定
来源：http://kzc.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://mok.yj202588.top

[S56] C++：optional
来源：http://ijf.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fvj.jlsjyb.cn

[S57] C++：编译期常量
来源：http://ado.hywenlv.cn

constexpr int N = 10;
来源：http://buu.redwolf501.top

[S58] C++：命名空间
来源：http://jdt.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://hin.tarul.cn

[S59] C++：静态断言
来源：http://eye.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oal.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://wjp.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qdp.nanxuanxn.top

================================================================================
来源：http://slc.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://toq.gzhubu.top

================================================================================
来源：http://avz.xziqi.cn

[T01] Kotlin：Hello World
来源：http://blx.yj202588.top

println("Hello")
来源：http://vpl.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://alc.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rsk.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://hqw.yueranfly.top

"值: $b"
来源：http://pvb.chenzaomai.com

[T04] Kotlin：空安全
来源：http://zhm.hywenlv.cn

val n: String? = null;  n?.length
来源：http://ycx.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://fis.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wli.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://gqi.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wiz.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://aza.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ouo.tian-w.cn

[T08] Kotlin：数据类
来源：http://txy.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://yfi.tanke756.top

[T09] Kotlin：扩展函数
来源：http://xfi.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://oag.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://vlb.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ipr.ehwqpu.com

[T11] Kotlin：协程
来源：http://syu.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cxl.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://ilb.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://gyw.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://yfq.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://cya.ctjpmb.com

[T14] Kotlin：循环
来源：http://fqf.shuidangran.top

for (i in 1..10) println(i)
来源：http://smg.bjfxy.top

[T15] Kotlin：接口
来源：http://act.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://lwy.hammf.cn

[T16] Swift：Hello World
来源：http://pcl.jqgfzy.top

print("Hello")
来源：http://lhe.gogol.net.cn

[T17] Swift：变量与常量
来源：http://lnu.yuanzhike.top

var a = 1;  let b = 2
来源：http://jgf.snrcjt.cn

[T18] Swift：字符串插值
来源：http://wmb.guowangkeji.top

"值: \(b)"
来源：http://vln.xylfe.cn

[T19] Swift：可选绑定
来源：http://gmi.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://scz.tianlin.xyz

[T20] Swift：数组操作
来源：http://ubu.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dfh.yangfankeji.com

[T21] Swift：遍历
来源：http://itz.yj20258888.top

for x in a { print(x) }
来源：http://srm.ydjk.org.cn

[T22] Swift：字典
来源：http://tte.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://sag.sjlbkw.cn

[T23] Swift：函数
来源：http://lgl.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://afd.nanxuanxn.top

[T24] Swift：闭包
来源：http://yjk.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cdb.tian-w.cn

[T25] Swift：结构体
来源：http://lib.sjlbkw.cn

struct P { var x: Int }
来源：http://obr.ydjk.org.cn

[T26] Swift：类与重写
来源：http://mbr.c1oappe.top

class A: Base { override func f() {} }
来源：http://bls.ybcxt.top

[T27] Swift：错误处理
来源：http://bsw.c1oappe.top

do { try f() } catch { print(error) }
来源：http://guf.tianlin.xyz

[T28] Swift：枚举
来源：http://czn.nanxinkj.top

enum Color { case red, green }
来源：http://hsa.tanke756.top

[T29] Swift：guard 提前返回
来源：http://efo.sysykeji.top

guard let x = opt else { return }
来源：http://lac.shangyingyoupin.top

[T30] Swift：协议
来源：http://xrp.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://pvj.fktsv.cn

[T31] Lua：Hello World
来源：http://xcc.tian-w.cn

print("Hello")
来源：http://oqg.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://hqv.tian-w.cn

local a = 1
来源：http://hlp.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://fhn.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xci.zhengqikj.top

[T34] Lua：遍历表
来源：http://lbg.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ref.svipenyu.cn

[T35] Lua：字典表
来源：http://uvf.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://dau.hesvh.cn

[T36] Lua：函数
来源：http://fmr.pycfn.com

function add(a, b) return a + b end
来源：http://qoi.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://elk.guowangkeji.top

"a" .. "b"
来源：http://fvm.smart0.xyz

[T38] Lua：条件
来源：http://etk.mhx1999.top

if x > 0 then print("正") end
来源：http://kpy.cheryme.top

[T39] Lua：模式匹配
来源：http://jga.chenjidiqi.icu

string.find(s, "%d+")
来源：http://lbx.shuidangran.top

[T40] Lua：元表
来源：http://rbs.bbcook.cn

setmetatable({}, { __index = base })
来源：http://veo.sjlbkw.cn

[T41] Perl：Hello World
来源：http://vdf.iojbl.cn

print "Hello\n";
来源：http://lsj.birdmap.top

[T42] Perl：变量类型
来源：http://sos.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bmh.ydzc1.top

[T43] Perl：字符串插值
来源：http://hid.hfpthk.cn

"值: $a"
来源：http://vfs.hcnkem.com

[T44] Perl：条件
来源：http://mbo.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://aft.zhengqikj.top

[T45] Perl：数组遍历
来源：http://hhb.316326.xyz

for my $x (@arr) { print $x; }
来源：http://bdy.yuxming.cn

[T46] Perl：哈希操作
来源：http://jur.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lvd.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://yro.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://elj.havefunace.top

[T48] Perl：正则替换
来源：http://wnf.uphjek.com

$s =~ s/old/new/g;
来源：http://nro.c1oappe.top

[T49] Perl：函数
来源：http://qsv.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xrs.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://aot.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nzc.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://ecz.kuanghao11.cn

[T51] Scala：Hello World
来源：http://pxx.9152youxi.cn

println("Hello")
来源：http://cft.jyoumei.cn

[T52] Scala：变量
来源：http://pbb.shzxlz.cn

val a = 1;  var b = 2
来源：http://gjq.cqqwz.cn

[T53] Scala：字符串插值
来源：http://qrz.mhx1999.top

s"值: $b"
来源：http://zes.hesvh.cn

[T54] Scala：集合映射
来源：http://dcf.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://esu.sxryk.cn

[T55] Scala：集合过滤
来源：http://xat.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://chr.birdmap.top

[T56] Scala：样例类
来源：http://gfv.wangdashe.top

case class User(name: String, age: Int)
来源：http://kmc.birdmap.top

[T57] Scala：模式匹配
来源：http://uvo.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eir.sweek.top

[T58] Scala：函数定义
来源：http://bxn.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://phm.zhixingplan.top

[T59] Scala：循环
来源：http://upo.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://tat.jinqigfzy.top

[T60] Scala：折叠
来源：http://xpe.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nei.iojbl.cn

================================================================================
来源：http://xtn.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ruv.dianchejie.cn

================================================================================
来源：http://ozm.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://csx.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qvo.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://eve.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hbg.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://ffa.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ubo.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://tag.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vtk.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://oba.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://vqb.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://dpm.jianghu66.top

{**a, **b}
来源：http://tst.tian-w.cn

[U07] Py：反转字典键值
来源：http://qpu.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://rcc.mhx1999.top

[U08] Py：展平二维列表
来源：http://wqr.yuxming.cn

[y for x in nested for y in x]
来源：http://fie.birdmap.top

[U09] Py：字典取最大值的键
来源：http://afa.cheryme.top

max(d, key=d.get)
来源：http://ojw.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://sdu.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qxf.sxryk.cn

[U11] Py：生成器表达式
来源：http://xst.daxiang520.top

(x * 2 for x in arr)
来源：http://pya.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://sxu.uphjek.com

Counter(arr).most_common(3)
来源：http://thn.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://xmp.tanke756.top

deque(maxlen=10)
来源：http://rcm.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://hln.andypj.xyz

defaultdict(list)
来源：http://fbp.cashguo.top

[U15] Py：高精度计时
来源：http://kbc.hammf.cn

t = time.perf_counter()
来源：http://rbz.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://xru.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dqi.pycfn.com

[U17] Py：初始化日志
来源：http://fvh.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://jqz.yuxming.cn

[U18] Py：预编译正则
来源：http://tav.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://kwk.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://otp.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wru.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://smo.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://lva.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://cyt.smart0.xyz

@contextlib.contextmanager
来源：http://yik.nwbrower.top

[U22] Py：矩阵转置
来源：http://jpt.yj202588.top

list(zip(*m))
来源：http://mmy.jianghu66.top

[U23] Py：分块读取大文件
来源：http://djq.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xud.jyoumei.cn

[U24] Py：路径操作
来源：http://ujv.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://djk.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://gqv.shuidangran.top

csv.DictReader(f)
来源：http://fxa.yuxming.cn

[U26] Py：并发下载
来源：http://djv.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owj.mhx1999.top

[U27] Py：异步 HTTP
来源：http://whf.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://zwi.sxryk.cn

[U28] Py：类型别名
来源：http://xlu.bbcook.cn

UserId = int
来源：http://yjq.yj20258888.top

[U29] Py：属性校验
来源：http://xto.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://cdg.gotoacloud.top

[U30] Py：数据类
来源：http://ufj.dashuyun.cn

@dataclass(slots=True)
来源：http://qmu.zhengqikj.top

[U31] Py：单测
来源：http://eni.yangfankeji.com

python -m pytest -q
来源：http://lev.jqgufenzy.top

[U32] Py：代码格式化
来源：http://wgr.tanke756.top

ruff format . && ruff check --fix .
来源：http://nej.yj20258.top

[U33] Py：打包发布
来源：http://uuw.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://yvm.jianghu66.top

[U34] Py：判断编码
来源：http://cxv.ivvv.top

chardet.detect(raw)
来源：http://sam.tarul.cn

[U35] Py：发送邮件
来源：http://ztg.svipenyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ojj.gzhubu.top

[U36] Py：定时任务
来源：http://mse.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://olm.jyoumei.cn

[U37] Py：读写 Excel
来源：http://vqg.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://ktv.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://gsw.hcnkem.com

Path(__file__).resolve().parent
来源：http://sdh.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://nrn.yj20258888.top

sys.stdout.isatty()
来源：http://ati.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://lop.cdnleiting.top

print("err", file=sys.stderr)
来源：http://ple.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://lky.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://syi.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://cbb.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chc.hcnkem.com

[U43] PHP：声明命名空间
来源：http://sqq.feifeiyinyue.top

namespace App\Http;
来源：http://jac.cucudq.cn

[U44] PHP：开启严格类型
来源：http://hql.chenlongwang.top

declare(strict_types=1);
来源：http://esj.jqgufenzy.top

[U45] PHP：类型声明与返回类型
来源：http://yjp.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://emj.0kj1m.cn

[U46] PHP：可空类型
来源：http://alx.jyoumei.cn

?string $name = null
来源：http://nrg.jinqigfzy.top

[U47] PHP：联合类型
来源：http://raa.316326.xyz

int|string $id
来源：http://uwi.yj20258888.top

[U48] PHP：纯枚举
来源：http://eot.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hzl.smart0.xyz

[U49] PHP：只读属性
来源：http://pro.gogol.net.cn

public readonly string $name
来源：http://rpb.yj202588.top

[U50] PHP：构造器属性提升
来源：http://dze.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://aaw.iojbl.cn

[U51] PHP：数组解构
来源：http://imy.zhoulong.xyz

[$a, $b] = $arr;
来源：http://rmn.jqgfzy.top

[U52] PHP：箭头函数
来源：http://qcl.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://tyd.bjfxy.top

[U53] PHP：空合并运算符
来源：http://uoo.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://tvm.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://odr.jqgufenzy.top

$obj?->method()
来源：http://mun.zhixingplan.top

[U55] PHP：match 表达式
来源：http://qqr.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vsv.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://pku.sysykeji.top

f(a: 1, b: 2)
来源：http://fxb.ehwqpu.com

[U57] PHP：字符串插值
来源：http://yce.vqdsnc.cn

"值: {$a}"
来源：http://hjy.smart0.xyz

[U58] PHP：数组三件套
来源：http://dur.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pgr.shuidangran.top

[U59] PHP：自定义排序
来源：http://lrn.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mjy.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://yvf.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gpz.pycfn.com

[U61] PHP：正则
来源：http://vjy.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zbk.sysykeji.top

[U62] PHP：日期对象
来源：http://zbp.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xpo.nanxinkj.top

[U63] PHP：文件读写
来源：http://pug.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqi.snrcjt.cn

[U64] PHP：目录遍历
来源：http://zhw.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://huz.yonumen.top

[U65] PHP：会话
来源：http://ays.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rps.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://bpz.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hku.hesvh.cn

[U67] PHP：处理文件上传
来源：http://wsb.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fkq.ppjwa.cn

[U68] PHP：PDO 连接
来源：http://onr.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ipn.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://dtu.zycfv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ldy.fehbvm.com

[U70] PHP：PDO 事务
来源：http://cig.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bch.chenzaomai.com

[U71] PHP：抛出异常
来源：http://gkv.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://pog.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://mak.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://rsc.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://hrp.fanxiaobao.xyz

parse_ini_file("config.ini", true)
来源：http://gbw.aizwys.cn

[U74] PHP：读取环境变量
来源：http://rpl.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://jmh.316326.xyz

[U75] PHP：依赖注入
来源：http://emd.316326.xyz

composer require psr/container
来源：http://ngk.yvedp.cn

[U76] PHP：简单路由
来源：http://dyw.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lge.xylfe.cn


<!-- 参考信息 -->