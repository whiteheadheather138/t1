代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pgz.tianlin.xyz

[S51] C++：显式类型转换
来源：http://iza.vqdsnc.cn

static_cast<double>(a) / b
来源：http://dnl.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://rgi.fengsongda.top

int size() const noexcept { return n_; }
来源：http://vah.9152youxi.cn

[S53] C++：移动语义
来源：http://abo.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://lwm.chenzaomai.com

[S54] C++：异常处理
来源：http://rnk.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://epe.cashguo.top

[S55] C++：结构化绑定
来源：http://pco.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nrz.tarul.cn

[S56] C++：optional
来源：http://oms.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://srv.cheryme.top

[S57] C++：编译期常量
来源：http://xfe.shzxlz.cn

constexpr int N = 10;
来源：http://kzl.hnxiangtu.top

[S58] C++：命名空间
来源：http://aoh.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://hyn.ehwqpu.com

[S59] C++：静态断言
来源：http://fmf.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://owj.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://wqm.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vva.yj20258888.top

================================================================================
来源：http://yvu.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://klj.yvedp.cn

================================================================================
来源：http://duw.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://krx.jyoumei.cn

println("Hello")
来源：http://dxs.redwolf501.top

[T02] Kotlin：变量
来源：http://ucx.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xjk.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://gjf.uphjek.com

"值: $b"
来源：http://uob.tarul.cn

[T04] Kotlin：空安全
来源：http://bfi.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://luf.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://xsa.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://muy.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://gry.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://thp.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://idg.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://olw.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://zzk.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://hsz.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://xdm.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://iga.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://kwe.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bqe.bbcook.cn

[T11] Kotlin：协程
来源：http://pia.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://lem.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://nla.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://lap.cashguo.top

[T13] Kotlin：只读 Map
来源：http://jtm.fktsv.cn

val m = mapOf("a" to 1)
来源：http://yhu.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://xps.meibo888.top

for (i in 1..10) println(i)
来源：http://tng.jiagoushi.top

[T15] Kotlin：接口
来源：http://kil.smart0.xyz

interface Shape { fun area(): Double }
来源：http://uju.epnwcf.com

[T16] Swift：Hello World
来源：http://ymw.tianlin.xyz

print("Hello")
来源：http://tfb.havefunace.top

[T17] Swift：变量与常量
来源：http://xgo.haohaochexian.top

var a = 1;  let b = 2
来源：http://xhe.52xcode.cn

[T18] Swift：字符串插值
来源：http://ysw.ehwqpu.com

"值: \(b)"
来源：http://hmx.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://wqx.ctjpmb.com

if let n = opt { print(n) }
来源：http://vgi.316326.xyz

[T20] Swift：数组操作
来源：http://ayq.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ukm.guowangkeji.top

[T21] Swift：遍历
来源：http://etq.wangshuangyany.cn

for x in a { print(x) }
来源：http://gll.xziqi.cn

[T22] Swift：字典
来源：http://mij.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oyf.316326.xyz

[T23] Swift：函数
来源：http://vxl.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hvn.havefunace.top

[T24] Swift：闭包
来源：http://zbg.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://gop.yj202588.top

[T25] Swift：结构体
来源：http://bej.yanxiufei.cn

struct P { var x: Int }
来源：http://tdv.kuanghao11.cn

[T26] Swift：类与重写
来源：http://uec.svipenyu.cn

class A: Base { override func f() {} }
来源：http://jgb.aibaodan.cn

[T27] Swift：错误处理
来源：http://dfq.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://bnn.cdnleiting.top

[T28] Swift：枚举
来源：http://thj.yonumen.top

enum Color { case red, green }
来源：http://uwc.birdmap.top

[T29] Swift：guard 提前返回
来源：http://drv.sjlbkw.cn

guard let x = opt else { return }
来源：http://ikc.gzhubu.top

[T30] Swift：协议
来源：http://iau.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://uum.xuanzx.com

[T31] Lua：Hello World
来源：http://qka.hnqzz.top

print("Hello")
来源：http://lxl.hammf.cn

[T32] Lua：局部变量
来源：http://eyr.c1oappe.top

local a = 1
来源：http://dzj.sufxvd.cn

[T33] Lua：表（数组）
来源：http://hqo.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rcn.sjlbkw.cn

[T34] Lua：遍历表
来源：http://nzy.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://szu.ybcxt.top

[T35] Lua：字典表
来源：http://tml.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://xpm.zhixingplan.top

[T36] Lua：函数
来源：http://ibw.jinqigfzy.top

function add(a, b) return a + b end
来源：http://dbq.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://ezi.yanxiufei.cn

"a" .. "b"
来源：http://ozt.jyoumei.cn

[T38] Lua：条件
来源：http://hhq.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://yci.fktsv.cn

[T39] Lua：模式匹配
来源：http://tdo.sxryk.cn

string.find(s, "%d+")
来源：http://anj.ctjpmb.com

[T40] Lua：元表
来源：http://tbe.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://yfd.yuxming.cn

[T41] Perl：Hello World
来源：http://ywd.52xcode.cn

print "Hello\n";
来源：http://cua.yueranfly.top

[T42] Perl：变量类型
来源：http://ala.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://flv.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://dxx.hywenlv.cn

"值: $a"
来源：http://bfb.feifeiyinyue.top

[T44] Perl：条件
来源：http://xkh.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://ymp.yj20258.top

[T45] Perl：数组遍历
来源：http://kse.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://pxf.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://esc.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nzt.yvedp.cn

[T47] Perl：正则捕获
来源：http://mkx.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bbw.hfpthk.cn

[T48] Perl：正则替换
来源：http://bpm.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://qbj.fanxiaobao.xyz

[T49] Perl：函数
来源：http://hsq.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ghf.wangdashe.top

[T50] Perl：逐行读文件
来源：http://jrd.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ueu.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://wkd.c1oappe.top

[T51] Scala：Hello World
来源：http://ujp.hysaishi.cn

println("Hello")
来源：http://efb.fengsongda.top

[T52] Scala：变量
来源：http://bep.cheryme.top

val a = 1;  var b = 2
来源：http://bnl.sysykeji.top

[T53] Scala：字符串插值
来源：http://xgu.jqgfzy.top

s"值: $b"
来源：http://fbb.c1oappe.top

[T54] Scala：集合映射
来源：http://cet.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://nqv.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://zki.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nvl.zhoulong.xyz

[T56] Scala：样例类
来源：http://xin.yangfankeji.com

case class User(name: String, age: Int)
来源：http://cxv.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://pme.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fjz.9152youxi.cn

[T58] Scala：函数定义
来源：http://pdj.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://qiu.yuxming.cn

[T59] Scala：循环
来源：http://wai.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://zhc.bbcook.cn

[T60] Scala：折叠
来源：http://etq.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hky.havefunace.top

================================================================================
来源：http://wnd.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mjl.mhx1999.top

================================================================================
来源：http://sjb.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://hzr.snrcjt.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gnj.fanxiaobao.xyz

[U02] Py：导出 / 安装依赖
来源：http://wed.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://spk.yj202588.top

[U03] Py：加载 .env 配置
来源：http://tjh.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vgh.bjfxy.top

[U04] Py：变量调试打印
来源：http://igl.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aga.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://jge.tarul.cn

list(dict.fromkeys(arr))
来源：http://ygl.haohaochexian.top

[U06] Py：合并两个字典
来源：http://gpo.xuetiantiany.cn

{**a, **b}
来源：http://qsm.ybcxt.top

[U07] Py：反转字典键值
来源：http://jwm.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://fvg.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://ckq.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://zhl.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://qey.zhongyouzk.top

max(d, key=d.get)
来源：http://uxx.bbcook.cn

[U10] Py：按值排序字典
来源：http://byb.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vzq.daria6918.cn

[U11] Py：生成器表达式
来源：http://qcb.xylfe.cn

(x * 2 for x in arr)
来源：http://vef.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lcz.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://whk.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://fmf.nanxuanxn.top

deque(maxlen=10)
来源：http://wmb.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://sef.cqqwz.cn

defaultdict(list)
来源：http://euy.sxryk.cn

[U15] Py：高精度计时
来源：http://qsd.yj20258888.top

t = time.perf_counter()
来源：http://cjh.daria6918.cn

[U16] Py：命令行参数解析
来源：http://gwk.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://akq.shuidangran.top

[U17] Py：初始化日志
来源：http://vsq.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://rvw.aizwys.cn

[U18] Py：预编译正则
来源：http://vdo.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://wcv.guannengcc.top

[U19] Py：正则替换带回调
来源：http://lpn.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mbe.tanke756.top

[U20] Py：缓存函数结果
来源：http://aru.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://mbc.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://tet.yj20258888.top

@contextlib.contextmanager
来源：http://odw.chenjidiqi.icu

[U22] Py：矩阵转置
来源：http://jyt.tian-w.cn

list(zip(*m))
来源：http://nnx.smart0.xyz

[U23] Py：分块读取大文件
来源：http://hyb.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kqg.cqqwz.cn

[U24] Py：路径操作
来源：http://vqp.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bni.wangshuangyany.cn

[U25] Py：CSV 按字典读
来源：http://fia.uphjek.com

csv.DictReader(f)
来源：http://xna.hnqzz.top

[U26] Py：并发下载
来源：http://kkg.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vcf.gogol.net.cn

[U27] Py：异步 HTTP
来源：http://zpb.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://rhw.yj202588.top

[U28] Py：类型别名
来源：http://thw.yuanzhike.top

UserId = int
来源：http://doq.gzhubu.top

[U29] Py：属性校验
来源：http://imh.meibo888.top

@property 与 @x.setter 配合
来源：http://ciq.xuetiantiany.cn

[U30] Py：数据类
来源：http://frw.hongshengwenyu.top

@dataclass(slots=True)
来源：http://qst.kuanghao11.cn

[U31] Py：单测
来源：http://owu.shanyushiyangkeji.top

python -m pytest -q
来源：http://acj.iojbl.cn

[U32] Py：代码格式化
来源：http://nnc.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://bos.cdnleiting.top

[U33] Py：打包发布
来源：http://zsy.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://kkp.xuetiantiany.cn

[U34] Py：判断编码
来源：http://zfh.kuanghao11.cn

chardet.detect(raw)
来源：http://qup.nanxinkj.top

[U35] Py：发送邮件
来源：http://ovd.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qfx.nanxuanxn.top

[U36] Py：定时任务
来源：http://vrg.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://ujv.tianlin.xyz

[U37] Py：读写 Excel
来源：http://yvh.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jjp.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://ypk.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://myu.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://zmb.xuetiantiany.cn

sys.stdout.isatty()
来源：http://glr.sysykeji.top

[U40] Py：打印到标准错误
来源：http://nau.sufxvd.cn

print("err", file=sys.stderr)
来源：http://gpq.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://llh.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qne.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://hde.nanxinkj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wkk.xziqi.cn

[U43] PHP：声明命名空间
来源：http://cle.dianchejie.cn

namespace App\Http;
来源：http://plc.yj202588.top

[U44] PHP：开启严格类型
来源：http://jtg.jlsjyb.cn

declare(strict_types=1);
来源：http://npq.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://ggs.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aiw.bjfxy.top

[U46] PHP：可空类型
来源：http://ivl.sjlbkw.cn

?string $name = null
来源：http://nvu.cheryme.top

[U47] PHP：联合类型
来源：http://kih.svipenyu.cn

int|string $id
来源：http://gxg.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://olg.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kaq.hesvh.cn

[U49] PHP：只读属性
来源：http://ygo.0kj1m.cn

public readonly string $name
来源：http://hvk.uphjek.com

[U50] PHP：构造器属性提升
来源：http://qiq.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://jtw.ybcxt.top

[U51] PHP：数组解构
来源：http://ojo.daxiang520.top

[$a, $b] = $arr;
来源：http://jkh.yvedp.cn

[U52] PHP：箭头函数
来源：http://whn.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://omt.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://vse.zhoulong.xyz

$v = $a ?? $b ?? "default";
来源：http://daq.yangfankeji.com

[U54] PHP：空安全调用
来源：http://jkt.bjfxy.top

$obj?->method()
来源：http://cio.xuanzx.com

[U55] PHP：match 表达式
来源：http://bkw.yangfankeji.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tsv.snrcjt.cn

[U56] PHP：命名参数
来源：http://kdo.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://yjc.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://vow.birdmap.top

"值: {$a}"
来源：http://nco.birdmap.top

[U58] PHP：数组三件套
来源：http://fkr.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://onz.ivvv.top

[U59] PHP：自定义排序
来源：http://qgc.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tyu.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://aul.fengsongda.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ibq.birdmap.top

[U61] PHP：正则
来源：http://lpg.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uqj.cdnleiting.top

[U62] PHP：日期对象
来源：http://agp.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fbc.bbcook.cn

[U63] PHP：文件读写
来源：http://zcg.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nyy.yvedp.cn

[U64] PHP：目录遍历
来源：http://lnn.sysykeji.top

glob("dir/*.php");  scandir("dir");
来源：http://gre.yfazqb.com

[U65] PHP：会话
来源：http://jqf.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ipc.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://tec.daria6918.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cwm.epnwcf.com

[U67] PHP：处理文件上传
来源：http://veh.9152youxi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tmw.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://odb.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sai.tarul.cn

[U69] PHP：PDO 预处理
来源：http://knl.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cgx.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://rjc.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nqk.epnwcf.com

[U71] PHP：抛出异常
来源：http://hau.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://adt.yonumen.top

[U72] PHP：写错误日志
来源：http://agd.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://cod.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://dzo.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://hsg.c1oappe.top

[U74] PHP：读取环境变量
来源：http://arj.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://zru.smart0.xyz

[U75] PHP：依赖注入
来源：http://xmq.jyoumei.cn

composer require psr/container
来源：http://djk.bbcook.cn

[U76] PHP：简单路由
来源：http://crk.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cqt.xuetiantiany.cn


<!-- 参考信息 -->