代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://oou.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xwh.gogol.net.cn

[S48] C++：逐行读文件
来源：http://tqb.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zxj.bbcook.cn

while (std::getline(in, line)) { }
来源：http://uvc.xylfe.cn

[S49] C++：写文件
来源：http://pcl.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwt.hammf.cn

[S50] C++：格式化数字
来源：http://rec.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rbb.chenzaomai.com

[S51] C++：显式类型转换
来源：http://ewt.jqgfzy.top

static_cast<double>(a) / b
来源：http://dgr.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://fut.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://rsm.jinqigfzy.top

[S53] C++：移动语义
来源：http://vke.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://fep.yj202588.top

[S54] C++：异常处理
来源：http://opk.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cie.gzhubu.top

[S55] C++：结构化绑定
来源：http://cut.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vjf.chenjidiqi.icu

[S56] C++：optional
来源：http://udi.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://awz.aizwys.cn

[S57] C++：编译期常量
来源：http://vra.vqdsnc.cn

constexpr int N = 10;
来源：http://vcb.yvedp.cn

[S58] C++：命名空间
来源：http://fhs.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://wev.ctjpmb.com

[S59] C++：静态断言
来源：http://mol.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bbo.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://hlp.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rci.redwolf501.top

================================================================================
来源：http://sue.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pvu.hammf.cn

================================================================================
来源：http://tdr.yj20258888.top

[T01] Kotlin：Hello World
来源：http://vam.ppjwa.cn

println("Hello")
来源：http://yzk.nanxuanxn.top

[T02] Kotlin：变量
来源：http://mbk.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zep.sweek.top

[T03] Kotlin：字符串模板
来源：http://xkf.cucudq.cn

"值: $b"
来源：http://lip.tarul.cn

[T04] Kotlin：空安全
来源：http://bkr.epnwcf.com

val n: String? = null;  n?.length
来源：http://rtb.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://eao.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lvz.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://nsd.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uhp.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://fkm.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://gvg.ehwqpu.com

[T08] Kotlin：数据类
来源：http://swy.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://ftc.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://hkh.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://yte.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://cqw.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gqc.hywenlv.cn

[T11] Kotlin：协程
来源：http://iyc.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kot.shuidangran.top

[T12] Kotlin：解构声明
来源：http://oft.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://nca.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://yok.cucudq.cn

val m = mapOf("a" to 1)
来源：http://lfp.zycfv.cn

[T14] Kotlin：循环
来源：http://qae.hcnkem.com

for (i in 1..10) println(i)
来源：http://hci.tian-w.cn

[T15] Kotlin：接口
来源：http://hne.fzhhl.top

interface Shape { fun area(): Double }
来源：http://lwe.yueranfly.top

[T16] Swift：Hello World
来源：http://obf.yfazqb.com

print("Hello")
来源：http://xbe.316326.xyz

[T17] Swift：变量与常量
来源：http://mda.jlsjyb.cn

var a = 1;  let b = 2
来源：http://rqs.fzhhl.top

[T18] Swift：字符串插值
来源：http://zyi.yj202588.top

"值: \(b)"
来源：http://twq.sysykeji.top

[T19] Swift：可选绑定
来源：http://iwt.0kj1m.cn

if let n = opt { print(n) }
来源：http://jma.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://zbt.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sjj.jiagoushi.top

[T21] Swift：遍历
来源：http://ayl.hnxiangtu.top

for x in a { print(x) }
来源：http://tjn.dianchejie.cn

[T22] Swift：字典
来源：http://iqu.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rkv.cashguo.top

[T23] Swift：函数
来源：http://cjw.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kuy.haohaochexian.top

[T24] Swift：闭包
来源：http://eqj.vehdjk.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://yhu.nanxinkj.top

[T25] Swift：结构体
来源：http://uqq.sufxvd.cn

struct P { var x: Int }
来源：http://kdx.vehdjk.com

[T26] Swift：类与重写
来源：http://cpd.yuanzhike.top

class A: Base { override func f() {} }
来源：http://ztm.meibo888.top

[T27] Swift：错误处理
来源：http://nyy.tian-w.cn

do { try f() } catch { print(error) }
来源：http://caw.sysykeji.top

[T28] Swift：枚举
来源：http://xqk.cashguo.top

enum Color { case red, green }
来源：http://als.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://sot.9152youxi.cn

guard let x = opt else { return }
来源：http://wze.iojbl.cn

[T30] Swift：协议
来源：http://bzy.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://qje.jiagoushi.top

[T31] Lua：Hello World
来源：http://hgn.ydzc1.top

print("Hello")
来源：http://nyp.sjlbkw.cn

[T32] Lua：局部变量
来源：http://fzk.xingfuxueyuan.xyz

local a = 1
来源：http://bij.pycfn.com

[T33] Lua：表（数组）
来源：http://wpb.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dzh.snrcjt.cn

[T34] Lua：遍历表
来源：http://zik.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oky.tian-w.cn

[T35] Lua：字典表
来源：http://dxk.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://xwa.vqdsnc.cn

[T36] Lua：函数
来源：http://iky.yj20258888.top

function add(a, b) return a + b end
来源：http://mql.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://bvv.zhoulong.xyz

"a" .. "b"
来源：http://kit.sysykeji.top

[T38] Lua：条件
来源：http://uij.yuanzhike.top

if x > 0 then print("正") end
来源：http://tgy.epnwcf.com

[T39] Lua：模式匹配
来源：http://vey.hysaishi.cn

string.find(s, "%d+")
来源：http://hlk.chenlongwang.top

[T40] Lua：元表
来源：http://itb.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://hgj.jlsjyb.cn

[T41] Perl：Hello World
来源：http://ncf.ywan-chungtsiang.top

print "Hello\n";
来源：http://vdg.hcnkem.com

[T42] Perl：变量类型
来源：http://yep.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xsu.yvedp.cn

[T43] Perl：字符串插值
来源：http://cki.haohaochexian.top

"值: $a"
来源：http://gym.redwolf501.top

[T44] Perl：条件
来源：http://wrq.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://him.xziqi.cn

[T45] Perl：数组遍历
来源：http://ghy.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://xdb.yfazqb.com

[T46] Perl：哈希操作
来源：http://qmx.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gfo.fktsv.cn

[T47] Perl：正则捕获
来源：http://pel.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://czj.nanxinkj.top

[T48] Perl：正则替换
来源：http://krw.haohaochexian.top

$s =~ s/old/new/g;
来源：http://tbj.svipenyu.cn

[T49] Perl：函数
来源：http://efl.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dtm.ywan-chungtsiang.top

[T50] Perl：逐行读文件
来源：http://hzg.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pjk.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://yoi.yj20258888.top

[T51] Scala：Hello World
来源：http://fpa.gzhubu.top

println("Hello")
来源：http://nri.gotoacloud.top

[T52] Scala：变量
来源：http://bkd.ctjpmb.com

val a = 1;  var b = 2
来源：http://tjo.aizwys.cn

[T53] Scala：字符串插值
来源：http://uke.zhengqikj.top

s"值: $b"
来源：http://nyx.xziqi.cn

[T54] Scala：集合映射
来源：http://jvt.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://ubo.sxryk.cn

[T55] Scala：集合过滤
来源：http://uiy.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://der.bbcook.cn

[T56] Scala：样例类
来源：http://vzh.yangfankeji.com

case class User(name: String, age: Int)
来源：http://lqc.snrcjt.cn

[T57] Scala：模式匹配
来源：http://pkt.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jwq.sxryk.cn

[T58] Scala：函数定义
来源：http://xdv.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xey.hysaishi.cn

[T59] Scala：循环
来源：http://dlx.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://mbu.hfpthk.cn

[T60] Scala：折叠
来源：http://rsh.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tbu.xinyue.icu

================================================================================
来源：http://sod.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hst.chenlongwang.top

================================================================================
来源：http://hcs.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://hkw.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://yfk.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://rps.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ekw.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://bcj.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ytd.ivvv.top

[U04] Py：变量调试打印
来源：http://fmu.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eyq.yj20258.top

[U05] Py：列表去重且保序
来源：http://wcm.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://oek.yonumen.top

[U06] Py：合并两个字典
来源：http://vou.hongshengwenyu.top

{**a, **b}
来源：http://iax.hywenlv.cn

[U07] Py：反转字典键值
来源：http://taw.hcnkem.com

{v: k for k, v in d.items()}
来源：http://myj.zdqjudy.top

[U08] Py：展平二维列表
来源：http://eqg.fktsv.cn

[y for x in nested for y in x]
来源：http://lni.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://grv.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://awk.yj202588.top

[U10] Py：按值排序字典
来源：http://mqr.yj202588.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yzk.hywenlv.cn

[U11] Py：生成器表达式
来源：http://ijv.hywenlv.cn

(x * 2 for x in arr)
来源：http://xou.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://koi.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://yjm.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://feo.gzhubu.top

deque(maxlen=10)
来源：http://att.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://jcj.ppjwa.cn

defaultdict(list)
来源：http://xil.hysaishi.cn

[U15] Py：高精度计时
来源：http://bfm.cashguo.top

t = time.perf_counter()
来源：http://zxt.ctjpmb.com

[U16] Py：命令行参数解析
来源：http://iik.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://duc.guowangkeji.top

[U17] Py：初始化日志
来源：http://esq.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://jmb.hesvh.cn

[U18] Py：预编译正则
来源：http://hgk.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://tuc.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://siv.havefunace.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xwu.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://liu.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://qkr.pycfn.com

[U21] Py：自定义上下文管理器
来源：http://bke.chenjidiqi.icu

@contextlib.contextmanager
来源：http://bmx.iojbl.cn

[U22] Py：矩阵转置
来源：http://ziu.hywenlv.cn

list(zip(*m))
来源：http://mgp.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://xvx.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vyo.xuetiantiany.cn

[U24] Py：路径操作
来源：http://rle.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://duy.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://nie.andypj.xyz

csv.DictReader(f)
来源：http://uol.tarul.cn

[U26] Py：并发下载
来源：http://iwb.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ptx.bbcook.cn

[U27] Py：异步 HTTP
来源：http://dsl.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://tof.feifeiyinyue.top

[U28] Py：类型别名
来源：http://lbq.yueranfly.top

UserId = int
来源：http://rbr.jinqigfzy.top

[U29] Py：属性校验
来源：http://nks.gogol.net.cn

@property 与 @x.setter 配合
来源：http://fyp.zhengqikj.top

[U30] Py：数据类
来源：http://vxc.nwbrower.top

@dataclass(slots=True)
来源：http://kgl.zycfv.cn

[U31] Py：单测
来源：http://iez.sxryk.cn

python -m pytest -q
来源：http://iyc.jianghu66.top

[U32] Py：代码格式化
来源：http://htv.hesvh.cn

ruff format . && ruff check --fix .
来源：http://kbz.hfpthk.cn

[U33] Py：打包发布
来源：http://yft.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://dpx.yangfankeji.com

[U34] Py：判断编码
来源：http://zyc.daxiang520.top

chardet.detect(raw)
来源：http://kpb.aibaodan.cn

[U35] Py：发送邮件
来源：http://bab.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lak.ivvv.top

[U36] Py：定时任务
来源：http://ate.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://qde.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://fbv.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://iyl.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://srh.tian-w.cn

Path(__file__).resolve().parent
来源：http://thv.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://bly.jlsjyb.cn

sys.stdout.isatty()
来源：http://ytq.sxryk.cn

[U40] Py：打印到标准错误
来源：http://jaa.shzxlz.cn

print("err", file=sys.stderr)
来源：http://kiv.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://xrp.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://yin.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://cek.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chg.guannengcc.top

[U43] PHP：声明命名空间
来源：http://dxs.xuetiantiany.cn

namespace App\Http;
来源：http://pqs.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://ert.hywenlv.cn

declare(strict_types=1);
来源：http://wxm.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://tkn.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hxn.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://wfg.nanxuanxn.top

?string $name = null
来源：http://trp.pycfn.com

[U47] PHP：联合类型
来源：http://hkj.nwbrower.top

int|string $id
来源：http://rmj.52xcode.cn

[U48] PHP：纯枚举
来源：http://fpw.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dyz.cucudq.cn

[U49] PHP：只读属性
来源：http://tca.yj20258.top

public readonly string $name
来源：http://swm.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://zkg.yonumen.top

public function __construct(private int $id) {}
来源：http://lcm.cucudq.cn

[U51] PHP：数组解构
来源：http://xvb.hfpthk.cn

[$a, $b] = $arr;
来源：http://xvn.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://jdh.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://gvm.sysykeji.top

[U53] PHP：空合并运算符
来源：http://ire.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://dfc.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://hok.jqgufenzy.top

$obj?->method()
来源：http://vmw.cdnleiting.top

[U55] PHP：match 表达式
来源：http://dqv.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zwe.xziqi.cn

[U56] PHP：命名参数
来源：http://leh.ydjk.org.cn

f(a: 1, b: 2)
来源：http://otn.andypj.xyz

[U57] PHP：字符串插值
来源：http://spq.sjlbkw.cn

"值: {$a}"
来源：http://trq.hcnkem.com

[U58] PHP：数组三件套
来源：http://ajl.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://exx.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://dfb.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://znc.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://kam.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zvd.jinqigufen.top

[U61] PHP：正则
来源：http://mll.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nue.jqgfzy.top

[U62] PHP：日期对象
来源：http://guu.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rcb.yj202588.top

[U63] PHP：文件读写
来源：http://ouu.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://evq.hesvh.cn

[U64] PHP：目录遍历
来源：http://mzg.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://opg.jinghuilouyu.cn

[U65] PHP：会话
来源：http://ryo.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hto.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://kpp.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kct.meibo888.top

[U67] PHP：处理文件上传
来源：http://gnv.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rjn.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://hti.snrcjt.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://omm.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://pll.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ktd.bbcook.cn

[U70] PHP：PDO 事务
来源：http://lpl.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kfw.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://eob.hcnkem.com

throw new RuntimeException("失败", 500);
来源：http://nss.xylfe.cn

[U72] PHP：写错误日志
来源：http://nok.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://ijm.daria6918.cn


<!-- 参考信息 -->