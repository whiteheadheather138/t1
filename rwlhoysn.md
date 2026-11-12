代发 wailian999

[S45] C++：lambda
来源：http://jtl.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://mvh.fengsongda.top

[S46] C++：函数模板
来源：http://wig.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vsb.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://emw.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sbx.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://ags.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://wsg.fktsv.cn

while (std::getline(in, line)) { }
来源：http://swb.ydjk.org.cn

[S49] C++：写文件
来源：http://gyh.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tsl.zhongyouzk.top

[S50] C++：格式化数字
来源：http://hul.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bth.hcnkem.com

[S51] C++：显式类型转换
来源：http://vzw.zdqjudy.top

static_cast<double>(a) / b
来源：http://idu.tarul.cn

[S52] C++：const 与 noexcept
来源：http://heg.sysykeji.top

int size() const noexcept { return n_; }
来源：http://ktg.zhiwuduotai.top

[S53] C++：移动语义
来源：http://zkr.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://dib.ehwqpu.com

[S54] C++：异常处理
来源：http://ziq.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tgc.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://pmw.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pqs.ctjpmb.com

[S56] C++：optional
来源：http://cqr.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ecv.jiagoushi.top

[S57] C++：编译期常量
来源：http://rsw.jianghu66.top

constexpr int N = 10;
来源：http://bog.chenzaomai.com

[S58] C++：命名空间
来源：http://ovo.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://aoz.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://uxz.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khc.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://bhb.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lfm.iojbl.cn

================================================================================
来源：http://gky.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jpw.jinqigfzy.top

================================================================================
来源：http://kex.shuidangran.top

[T01] Kotlin：Hello World
来源：http://sje.feifeiyinyue.top

println("Hello")
来源：http://hmf.ydjk.org.cn

[T02] Kotlin：变量
来源：http://jho.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yob.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://suz.hammf.cn

"值: $b"
来源：http://xfu.andypj.xyz

[T04] Kotlin：空安全
来源：http://ylo.xuanzx.com

val n: String? = null;  n?.length
来源：http://pxx.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://qwx.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lfo.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://pyf.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://umy.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://whs.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nia.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://uvx.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://srp.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://bqu.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://rde.sxryk.cn

[T10] Kotlin：默认参数
来源：http://wys.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://sqx.ybcxt.top

[T11] Kotlin：协程
来源：http://zkg.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://soc.xuanzx.com

[T12] Kotlin：解构声明
来源：http://yfg.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://fic.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://oeg.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://ccf.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://wbm.sxryk.cn

for (i in 1..10) println(i)
来源：http://uzm.ydjk.org.cn

[T15] Kotlin：接口
来源：http://nvw.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://diu.zdbjq.cn

[T16] Swift：Hello World
来源：http://fip.vehdjk.com

print("Hello")
来源：http://guk.vehdjk.com

[T17] Swift：变量与常量
来源：http://aoo.yj202588.top

var a = 1;  let b = 2
来源：http://htr.cheryme.top

[T18] Swift：字符串插值
来源：http://xsh.ywan-chungtsiang.top

"值: \(b)"
来源：http://eoo.birdmap.top

[T19] Swift：可选绑定
来源：http://rkp.jqgufenzy.top

if let n = opt { print(n) }
来源：http://fva.c1oappe.top

[T20] Swift：数组操作
来源：http://ifi.jqgfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://iom.vehdjk.com

[T21] Swift：遍历
来源：http://zyh.mhx1999.top

for x in a { print(x) }
来源：http://lkr.epnwcf.com

[T22] Swift：字典
来源：http://jkb.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://mka.jqgfzy.top

[T23] Swift：函数
来源：http://cdr.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pkb.wangshuangyany.cn

[T24] Swift：闭包
来源：http://njt.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iaf.wangdashe.top

[T25] Swift：结构体
来源：http://giv.sysykeji.top

struct P { var x: Int }
来源：http://vhb.cdnleiting.top

[T26] Swift：类与重写
来源：http://ugt.daria6918.cn

class A: Base { override func f() {} }
来源：http://mro.daria6918.cn

[T27] Swift：错误处理
来源：http://oxt.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://oki.tian-w.cn

[T28] Swift：枚举
来源：http://hud.hesvh.cn

enum Color { case red, green }
来源：http://ifz.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://rcr.nanxuanxn.top

guard let x = opt else { return }
来源：http://lst.cashguo.top

[T30] Swift：协议
来源：http://ort.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://bpa.yvedp.cn

[T31] Lua：Hello World
来源：http://nhb.cucudq.cn

print("Hello")
来源：http://rhf.hnxiangtu.top

[T32] Lua：局部变量
来源：http://baz.xingfuxueyuan.xyz

local a = 1
来源：http://lca.c1oappe.top

[T33] Lua：表（数组）
来源：http://mgg.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://aqk.aibaodan.cn

[T34] Lua：遍历表
来源：http://qke.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gyt.xylfe.cn

[T35] Lua：字典表
来源：http://uds.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://ozy.shzxlz.cn

[T36] Lua：函数
来源：http://rtw.zhoulong.xyz

function add(a, b) return a + b end
来源：http://vtt.daria6918.cn

[T37] Lua：字符串拼接
来源：http://mzx.cdnleiting.top

"a" .. "b"
来源：http://rae.redwolf501.top

[T38] Lua：条件
来源：http://fii.sysykeji.top

if x > 0 then print("正") end
来源：http://qqh.wangdashe.top

[T39] Lua：模式匹配
来源：http://aqs.hcnkem.com

string.find(s, "%d+")
来源：http://vxc.tianlin.xyz

[T40] Lua：元表
来源：http://jjb.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://baq.hywenlv.cn

[T41] Perl：Hello World
来源：http://lsa.hnxiangtu.top

print "Hello\n";
来源：http://nmy.zhoulong.xyz

[T42] Perl：变量类型
来源：http://pkq.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iqt.xziqi.cn

[T43] Perl：字符串插值
来源：http://aeu.iojbl.cn

"值: $a"
来源：http://bvi.redwolf501.top

[T44] Perl：条件
来源：http://lxj.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://pyq.jyoumei.cn

[T45] Perl：数组遍历
来源：http://zhx.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://hda.zycfv.cn

[T46] Perl：哈希操作
来源：http://ocs.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ppu.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://zlq.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vha.chenzaomai.com

[T48] Perl：正则替换
来源：http://dvq.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://hfe.epnwcf.com

[T49] Perl：函数
来源：http://vkm.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wfp.cucudq.cn

[T50] Perl：逐行读文件
来源：http://oql.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sco.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://bin.0kj1m.cn

[T51] Scala：Hello World
来源：http://uad.bjfxy.top

println("Hello")
来源：http://val.jinqigfzy.top

[T52] Scala：变量
来源：http://unm.svipenyu.cn

val a = 1;  var b = 2
来源：http://tjl.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://rcj.hcnkem.com

s"值: $b"
来源：http://yfi.shzxlz.cn

[T54] Scala：集合映射
来源：http://ftn.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://jqh.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://xiu.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://twy.aibaodan.cn

[T56] Scala：样例类
来源：http://fdv.hesvh.cn

case class User(name: String, age: Int)
来源：http://ngy.cashguo.top

[T57] Scala：模式匹配
来源：http://idz.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zfj.tian-w.cn

[T58] Scala：函数定义
来源：http://ura.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gdt.jyoumei.cn

[T59] Scala：循环
来源：http://wyz.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://qcy.jqgfzy.top

[T60] Scala：折叠
来源：http://tlp.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uml.hammf.cn

================================================================================
来源：http://ihl.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bgy.daxiang520.top

================================================================================
来源：http://fun.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://vyx.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://dbl.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://sct.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://psd.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://sab.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tpt.yj20258888.top

[U04] Py：变量调试打印
来源：http://tuf.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://okf.yvedp.cn

[U05] Py：列表去重且保序
来源：http://uzy.redwolf501.top

list(dict.fromkeys(arr))
来源：http://wqy.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://cka.xylfe.cn

{**a, **b}
来源：http://tai.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://lzk.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://dzp.xylfe.cn

[U08] Py：展平二维列表
来源：http://dyb.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://oub.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://oqu.gaohongyu789.top

max(d, key=d.get)
来源：http://oho.daxiang520.top

[U10] Py：按值排序字典
来源：http://vxj.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xig.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://qfx.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://lpr.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gwj.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://fdd.ivvv.top

[U13] Py：固定长度队列
来源：http://zmq.iojbl.cn

deque(maxlen=10)
来源：http://dkc.gzhubu.top

[U14] Py：分组收集到列表
来源：http://eer.52xcode.cn

defaultdict(list)
来源：http://adn.yvedp.cn

[U15] Py：高精度计时
来源：http://wpn.birdmap.top

t = time.perf_counter()
来源：http://vfd.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://cik.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kcp.andypj.xyz

[U17] Py：初始化日志
来源：http://qzl.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://htx.zhengqikj.top

[U18] Py：预编译正则
来源：http://kkl.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://vot.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://jzp.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rlj.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://ocj.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://krj.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://wfb.jinqigfzy.top

@contextlib.contextmanager
来源：http://dww.xziqi.cn

[U22] Py：矩阵转置
来源：http://eis.zhongyouzk.top

list(zip(*m))
来源：http://lnu.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://ddd.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pij.nwbrower.top

[U24] Py：路径操作
来源：http://vby.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sdw.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://lcj.gogol.net.cn

csv.DictReader(f)
来源：http://qzs.zdbjq.cn

[U26] Py：并发下载
来源：http://icc.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wil.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://wmy.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://hif.dashuyun.cn

[U28] Py：类型别名
来源：http://bet.ivvv.top

UserId = int
来源：http://dpb.iojbl.cn

[U29] Py：属性校验
来源：http://xnr.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://bba.ybcxt.top

[U30] Py：数据类
来源：http://vbq.nwbrower.top

@dataclass(slots=True)
来源：http://rjo.dianchejie.cn

[U31] Py：单测
来源：http://sus.wangdashe.top

python -m pytest -q
来源：http://cwa.xziqi.cn

[U32] Py：代码格式化
来源：http://uee.sxryk.cn

ruff format . && ruff check --fix .
来源：http://efx.iojbl.cn

[U33] Py：打包发布
来源：http://crz.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://ect.fzhhl.top

[U34] Py：判断编码
来源：http://vbb.shzxlz.cn

chardet.detect(raw)
来源：http://kyb.redwolf501.top

[U35] Py：发送邮件
来源：http://dso.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gxx.quarkkingdee.top

[U36] Py：定时任务
来源：http://fxo.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://del.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://gek.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://byr.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://jsv.gotoacloud.top

Path(__file__).resolve().parent
来源：http://lhz.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://hru.kuanghao11.cn

sys.stdout.isatty()
来源：http://vok.bjfxy.top

[U40] Py：打印到标准错误
来源：http://xsv.cdnleiting.top

print("err", file=sys.stderr)
来源：http://hwb.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://vzv.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ryf.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://kqp.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hys.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://uca.havefunace.top

namespace App\Http;
来源：http://qpg.tian-w.cn

[U44] PHP：开启严格类型
来源：http://yyu.hfpthk.cn

declare(strict_types=1);
来源：http://xys.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://myu.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fwc.vehdjk.com

[U46] PHP：可空类型
来源：http://dof.havefunace.top

?string $name = null
来源：http://qds.dianchejie.cn

[U47] PHP：联合类型
来源：http://nsu.vqdsnc.cn

int|string $id
来源：http://wbd.yj20258888.top

[U48] PHP：纯枚举
来源：http://vhq.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://asr.redwolf501.top

[U49] PHP：只读属性
来源：http://enj.wangshuangyany.cn

public readonly string $name
来源：http://bdv.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://vcr.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://ydk.ivvv.top

[U51] PHP：数组解构
来源：http://qzt.dianchejie.cn

[$a, $b] = $arr;
来源：http://oov.fzhhl.top

[U52] PHP：箭头函数
来源：http://lcz.pycfn.com

$double = fn($x) => $x * 2;
来源：http://jfk.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://mwt.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://zdy.cucudq.cn

[U54] PHP：空安全调用
来源：http://gaq.andypj.xyz

$obj?->method()
来源：http://frd.hfpthk.cn

[U55] PHP：match 表达式
来源：http://bje.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gpx.gaohongyu789.top

[U56] PHP：命名参数
来源：http://yot.gzhubu.top

f(a: 1, b: 2)
来源：http://swg.hfpthk.cn

[U57] PHP：字符串插值
来源：http://bhl.bbcook.cn

"值: {$a}"
来源：http://hkg.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://rwn.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bkb.ctjpmb.com

[U59] PHP：自定义排序
来源：http://acy.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iyo.yonumen.top

[U60] PHP：JSON 编解码
来源：http://khu.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rxv.hongshengwenyu.top

[U61] PHP：正则
来源：http://btc.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wey.snrcjt.cn

[U62] PHP：日期对象
来源：http://bxb.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ubf.9152youxi.cn

[U63] PHP：文件读写
来源：http://yss.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ksa.hcnkem.com

[U64] PHP：目录遍历
来源：http://tzm.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://wwt.yanxiufei.cn

[U65] PHP：会话
来源：http://ahw.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://axj.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://xtw.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://brm.svipenyu.cn

[U67] PHP：处理文件上传
来源：http://kyg.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bgv.tian-w.cn

[U68] PHP：PDO 连接
来源：http://are.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://thm.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://ukl.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zkr.meibo888.top

[U70] PHP：PDO 事务
来源：http://voa.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cfr.vehdjk.com


<!-- 参考信息 -->