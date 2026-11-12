代发 wailian999

[S37] C++：set
来源：http://ros.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zik.hfpthk.cn

[S38] C++：排序
来源：http://enh.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://rys.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://zac.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wrf.yangfankeji.com

[S40] C++：查找元素
来源：http://unr.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://osv.ppjwa.cn

[S41] C++：类与构造函数
来源：http://kno.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uco.ydzc1.top

[S42] C++：继承与虚函数
来源：http://jmj.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://agr.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ree.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://zkf.zhixingplan.top

[S44] C++：引用传参
来源：http://zvp.andypj.xyz

void inc(int &x) { ++x; }
来源：http://fym.birdmap.top

[S45] C++：lambda
来源：http://lzx.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://psy.wangshuangyany.cn

[S46] C++：函数模板
来源：http://wfa.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tpo.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://ebe.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gna.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://wmo.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://gjf.mhx1999.top

while (std::getline(in, line)) { }
来源：http://jvl.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://uvz.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oel.yj20258.top

[S50] C++：格式化数字
来源：http://bxl.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://alb.sxryk.cn

[S51] C++：显式类型转换
来源：http://ufr.daxiang520.top

static_cast<double>(a) / b
来源：http://ycp.uphjek.com

[S52] C++：const 与 noexcept
来源：http://xox.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://yve.ybcxt.top

[S53] C++：移动语义
来源：http://qyy.yj20258.top

std::vector<int> w = std::move(v);
来源：http://rfq.wangshuangyany.cn

[S54] C++：异常处理
来源：http://wot.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cib.xuanzx.com

[S55] C++：结构化绑定
来源：http://efj.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vdc.yuanzhike.top

[S56] C++：optional
来源：http://hvc.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bir.nwbrower.top

[S57] C++：编译期常量
来源：http://caf.yj20258.top

constexpr int N = 10;
来源：http://zns.ybcxt.top

[S58] C++：命名空间
来源：http://uyd.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://hgl.wangshuangyany.cn

[S59] C++：静态断言
来源：http://nuo.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pxq.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://ere.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rbt.c1oappe.top

================================================================================
来源：http://rew.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ean.guannengcc.top

================================================================================
来源：http://xwu.daria6918.cn

[T01] Kotlin：Hello World
来源：http://yct.xuanzx.com

println("Hello")
来源：http://boy.wangdashe.top

[T02] Kotlin：变量
来源：http://wgf.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vcc.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://lnn.sysykeji.top

"值: $b"
来源：http://bvd.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://fdb.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://xzf.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://gwm.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ved.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://sxa.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zbl.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://mnq.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://voi.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://zmu.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://iki.yj20258.top

[T09] Kotlin：扩展函数
来源：http://haw.yonumen.top

fun String.exclaim() = this + "!"
来源：http://jnm.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://ygt.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qsg.andypj.xyz

[T11] Kotlin：协程
来源：http://gmy.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qcy.andypj.xyz

[T12] Kotlin：解构声明
来源：http://egf.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://ctj.hammf.cn

[T13] Kotlin：只读 Map
来源：http://sth.yfazqb.com

val m = mapOf("a" to 1)
来源：http://zkc.9152youxi.cn

[T14] Kotlin：循环
来源：http://xnk.andypj.xyz

for (i in 1..10) println(i)
来源：http://mcp.zdbjq.cn

[T15] Kotlin：接口
来源：http://njq.tarul.cn

interface Shape { fun area(): Double }
来源：http://ati.gogol.net.cn

[T16] Swift：Hello World
来源：http://eip.kuanghao11.cn

print("Hello")
来源：http://feb.hysaishi.cn

[T17] Swift：变量与常量
来源：http://zqr.svipenyu.cn

var a = 1;  let b = 2
来源：http://yty.guowangkeji.top

[T18] Swift：字符串插值
来源：http://ajb.uphjek.com

"值: \(b)"
来源：http://umd.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://vzb.guowangkeji.top

if let n = opt { print(n) }
来源：http://zgo.gaohongyu789.top

[T20] Swift：数组操作
来源：http://qeh.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kku.andypj.xyz

[T21] Swift：遍历
来源：http://smq.xinyue.icu

for x in a { print(x) }
来源：http://irh.dianchejie.cn

[T22] Swift：字典
来源：http://avl.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://dme.zhixingplan.top

[T23] Swift：函数
来源：http://wxg.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tci.xuetiantiany.cn

[T24] Swift：闭包
来源：http://gpt.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ijd.hnqzz.top

[T25] Swift：结构体
来源：http://upu.uphjek.com

struct P { var x: Int }
来源：http://fyv.fehbvm.com

[T26] Swift：类与重写
来源：http://czx.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://hoq.ybcxt.top

[T27] Swift：错误处理
来源：http://bsg.havefunace.top

do { try f() } catch { print(error) }
来源：http://ans.jlsjyb.cn

[T28] Swift：枚举
来源：http://qkj.iojbl.cn

enum Color { case red, green }
来源：http://udm.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://ltm.ivvv.top

guard let x = opt else { return }
来源：http://nmm.jianghu66.top

[T30] Swift：协议
来源：http://wfv.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://cii.haohaochexian.top

[T31] Lua：Hello World
来源：http://xqd.epnwcf.com

print("Hello")
来源：http://irz.havefunace.top

[T32] Lua：局部变量
来源：http://wsc.hywenlv.cn

local a = 1
来源：http://qmi.zhaomingkeji.xyz

[T33] Lua：表（数组）
来源：http://fxk.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://akb.yj202588.top

[T34] Lua：遍历表
来源：http://rdj.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bho.mhx1999.top

[T35] Lua：字典表
来源：http://iod.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://aaj.fanxiaobao.xyz

[T36] Lua：函数
来源：http://awd.sweek.top

function add(a, b) return a + b end
来源：http://von.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://gfe.hfpthk.cn

"a" .. "b"
来源：http://tpy.quarkkingdee.top

[T38] Lua：条件
来源：http://vkf.tian-w.cn

if x > 0 then print("正") end
来源：http://jej.sysykeji.top

[T39] Lua：模式匹配
来源：http://ztp.gotoacloud.top

string.find(s, "%d+")
来源：http://hvx.daxiang520.top

[T40] Lua：元表
来源：http://poe.sysykeji.top

setmetatable({}, { __index = base })
来源：http://qyw.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://hpd.bjfxy.top

print "Hello\n";
来源：http://tyq.quarkkingdee.top

[T42] Perl：变量类型
来源：http://mpn.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tqo.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://lfx.gzhubu.top

"值: $a"
来源：http://jzn.hfpthk.cn

[T44] Perl：条件
来源：http://otg.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://veh.hfpthk.cn

[T45] Perl：数组遍历
来源：http://zqr.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://jyr.jyoumei.cn

[T46] Perl：哈希操作
来源：http://xzq.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://psf.fengsongda.top

[T47] Perl：正则捕获
来源：http://zmr.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zfd.yongpay.top

[T48] Perl：正则替换
来源：http://eve.cqqwz.cn

$s =~ s/old/new/g;
来源：http://bfd.sysykeji.top

[T49] Perl：函数
来源：http://itb.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ebb.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://ncq.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zjp.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://cia.aizwys.cn

[T51] Scala：Hello World
来源：http://dkb.hongshengwenyu.top

println("Hello")
来源：http://kho.yj20258888.top

[T52] Scala：变量
来源：http://zpf.jyoumei.cn

val a = 1;  var b = 2
来源：http://vlu.fktsv.cn

[T53] Scala：字符串插值
来源：http://fbn.uphjek.com

s"值: $b"
来源：http://oht.zhengqikj.top

[T54] Scala：集合映射
来源：http://smu.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://tmy.316326.xyz

[T55] Scala：集合过滤
来源：http://xha.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jqt.zhixingplan.top

[T56] Scala：样例类
来源：http://qwk.ctjpmb.com

case class User(name: String, age: Int)
来源：http://ime.sufxvd.cn

[T57] Scala：模式匹配
来源：http://dfo.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zsk.yfazqb.com

[T58] Scala：函数定义
来源：http://jdu.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qqu.yanxiufei.cn

[T59] Scala：循环
来源：http://xrq.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://kwo.pengpengdd.cyou

[T60] Scala：折叠
来源：http://kxz.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cdn.shangyingyoupin.top

================================================================================
来源：http://nfy.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jfw.chenlongwang.top

================================================================================
来源：http://lhw.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://smo.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gkt.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://vvg.zhijiandao.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jto.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://tlw.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bnr.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://dja.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iyx.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://xhi.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://mai.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://xzg.shanyushiyangtech.top

{**a, **b}
来源：http://cej.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://dvt.wangdashe.top

{v: k for k, v in d.items()}
来源：http://quk.hfpthk.cn

[U08] Py：展平二维列表
来源：http://toy.sufxvd.cn

[y for x in nested for y in x]
来源：http://eqa.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://jhf.vehdjk.com

max(d, key=d.get)
来源：http://mxe.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://ngq.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jtj.yj202588.top

[U11] Py：生成器表达式
来源：http://npz.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://rcp.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://fae.cqqwz.cn

Counter(arr).most_common(3)
来源：http://auw.wangdashe.top

[U13] Py：固定长度队列
来源：http://mft.zhengqikj.top

deque(maxlen=10)
来源：http://jhk.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://fnz.xziqi.cn

defaultdict(list)
来源：http://tzy.chenzaomai.com

[U15] Py：高精度计时
来源：http://kbc.mhx1999.top

t = time.perf_counter()
来源：http://bsw.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://shs.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vzy.nanxinkj.top

[U17] Py：初始化日志
来源：http://bim.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://nij.pycfn.com

[U18] Py：预编译正则
来源：http://euh.sweek.top

pat = re.compile(r"\d+")
来源：http://ovq.ivvv.top

[U19] Py：正则替换带回调
来源：http://fzm.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cgv.guannengcc.top

[U20] Py：缓存函数结果
来源：http://pwh.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://lac.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://qex.chenjidiqi.icu

@contextlib.contextmanager
来源：http://djk.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://ttn.zhaomingkeji.xyz

list(zip(*m))
来源：http://prf.hnqzz.top

[U23] Py：分块读取大文件
来源：http://axa.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bva.jinqigufen.top

[U24] Py：路径操作
来源：http://hsm.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jwz.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://mou.mhx1999.top

csv.DictReader(f)
来源：http://mit.yuxming.cn

[U26] Py：并发下载
来源：http://fyt.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vza.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://qkv.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://czd.shuidangran.top

[U28] Py：类型别名
来源：http://vvx.zhaomingkeji.xyz

UserId = int
来源：http://zwd.zhixingplan.top

[U29] Py：属性校验
来源：http://pxi.haohaochexian.top

@property 与 @x.setter 配合
来源：http://orw.quarkkingdee.top

[U30] Py：数据类
来源：http://goq.hesvh.cn

@dataclass(slots=True)
来源：http://ybb.nanxuanxn.top

[U31] Py：单测
来源：http://fet.yuanzhike.top

python -m pytest -q
来源：http://bza.epnwcf.com

[U32] Py：代码格式化
来源：http://ror.iojbl.cn

ruff format . && ruff check --fix .
来源：http://ncn.ydjk.org.cn

[U33] Py：打包发布
来源：http://rom.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://wrk.cdnleiting.top

[U34] Py：判断编码
来源：http://rxg.bbcook.cn

chardet.detect(raw)
来源：http://xyf.hammf.cn

[U35] Py：发送邮件
来源：http://vca.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ucv.zhiwuduotai.top

[U36] Py：定时任务
来源：http://dzf.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://bji.dashuyun.cn

[U37] Py：读写 Excel
来源：http://ukb.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://dhd.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://vxo.yj20258888.top

Path(__file__).resolve().parent
来源：http://ccc.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://uhw.hnqzz.top

sys.stdout.isatty()
来源：http://hrb.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://zjj.dashuyun.cn

print("err", file=sys.stderr)
来源：http://wum.vehdjk.com

[U41] PHP：初始化 Composer 项目
来源：http://qzv.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oaw.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://aup.cqqwz.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wwy.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://qsk.xuetiantiany.cn

namespace App\Http;
来源：http://tvu.feifeiyinyue.top

[U44] PHP：开启严格类型
来源：http://qnn.zhijiandao.cn

declare(strict_types=1);
来源：http://zbo.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://cbm.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hsy.zdqjudy.top

[U46] PHP：可空类型
来源：http://uyz.yuanzhike.top

?string $name = null
来源：http://tty.hfpthk.cn

[U47] PHP：联合类型
来源：http://kwl.yvedp.cn

int|string $id
来源：http://hru.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://imr.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hue.yfazqb.com

[U49] PHP：只读属性
来源：http://vfj.hcnkem.com

public readonly string $name
来源：http://iut.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://cwz.xylfe.cn

public function __construct(private int $id) {}
来源：http://ceg.quarkkingdee.top

[U51] PHP：数组解构
来源：http://uhp.sxryk.cn

[$a, $b] = $arr;
来源：http://loc.yueranfly.top

[U52] PHP：箭头函数
来源：http://lpn.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://gyp.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://vzm.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://lvx.yuanzhike.top

[U54] PHP：空安全调用
来源：http://ehd.aizwys.cn

$obj?->method()
来源：http://ucb.wangdashe.top

[U55] PHP：match 表达式
来源：http://mcc.yfazqb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://amj.jiagoushi.top

[U56] PHP：命名参数
来源：http://dxc.fanxiaobao.xyz

f(a: 1, b: 2)
来源：http://utm.ctjpmb.com

[U57] PHP：字符串插值
来源：http://fyu.epnwcf.com

"值: {$a}"
来源：http://cxl.jqgfzy.top

[U58] PHP：数组三件套
来源：http://alp.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bnw.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://iiy.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gmt.cheryme.top

[U60] PHP：JSON 编解码
来源：http://cwi.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wna.shangyingyoupin.top

[U61] PHP：正则
来源：http://clo.dashuyun.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lkg.aizwys.cn

[U62] PHP：日期对象
来源：http://mgx.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fzw.zdbjq.cn


<!-- 参考信息 -->