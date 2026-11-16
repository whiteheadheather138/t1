代发 wailian999

int main(int argc, char **argv)
来源：http://vyt.jlsjyb.cn

[S19] C：快速排序
来源：http://jaf.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nsz.jlsjyb.cn

[S20] C：二分查找
来源：http://rfz.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gwf.zycfv.cn

[S21] C：字符类别判断
来源：http://jtf.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fmt.vqdsnc.cn

[S22] C：字符串转数字
来源：http://mnh.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://bwi.9152youxi.cn

[S23] C：随机数
来源：http://caw.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uss.hammf.cn

[S24] C：获取本地时间
来源：http://ekd.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrn.shuidangran.top

[S25] C：内存拷贝
来源：http://cxf.cheryme.top

memcpy(dst, src, n);
来源：http://yki.c1oappe.top

[S26] C：内存清零
来源：http://mnj.gzhubu.top

memset(a, 0, sizeof a);
来源：http://qrn.yj20258888.top

[S27] C：定义常量
来源：http://lky.andypj.xyz

const double PI = 3.14159;
来源：http://vju.cqqwz.cn

[S28] C：静态变量
来源：http://lny.jianghu66.top

static int counter = 0;
来源：http://rpm.ehwqpu.com

[S29] C：变参函数
来源：http://tuo.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vcu.quarkkingdee.top

[S30] C：头文件保护
来源：http://gsi.shanyushiyangkeji.top

#ifndef X_H
来源：http://eip.yonumen.top

#define X_H
来源：http://pzk.xziqi.cn

#endif
来源：http://tpz.ivvv.top

[S31] C++：Hello World
来源：http://nhk.xingfuxueyuan.xyz

#include <iostream>
来源：http://lby.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://oiz.chenjidiqi.icu

[S32] C++：字符串
来源：http://ieb.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://dcx.ydzc1.top

[S33] C++：vector 增删
来源：http://usf.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kra.tian-w.cn

[S34] C++：遍历 vector
来源：http://psw.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://ouo.zycfv.cn

[S35] C++：map
来源：http://ypy.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khl.0kj1m.cn

[S36] C++：unordered_map
来源：http://pzb.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xfc.zdqjudy.top

[S37] C++：set
来源：http://esd.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://myw.xuetiantiany.cn

[S38] C++：排序
来源：http://djf.havefunace.top

std::sort(v.begin(), v.end());
来源：http://cug.yj20258.top

[S39] C++：自定义比较器排序
来源：http://aeo.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sgx.kuanghao11.cn

[S40] C++：查找元素
来源：http://xrf.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://val.dashuyun.cn

[S41] C++：类与构造函数
来源：http://upm.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nam.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://mpq.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://yjh.c1oappe.top

[S43] C++：智能指针
来源：http://cvd.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://odj.aizwys.cn

[S44] C++：引用传参
来源：http://ssu.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://ebg.guannengcc.top

[S45] C++：lambda
来源：http://tdf.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bxu.wangshuangyany.cn

[S46] C++：函数模板
来源：http://fme.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ita.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://psd.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vna.yj20258.top

[S48] C++：逐行读文件
来源：http://ddi.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://mbh.haohaochexian.top

while (std::getline(in, line)) { }
来源：http://snl.nanxinkj.top

[S49] C++：写文件
来源：http://wca.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvk.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://tnj.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxh.fengsongda.top

[S51] C++：显式类型转换
来源：http://gvy.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://zzd.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://qmp.yongpay.top

int size() const noexcept { return n_; }
来源：http://lnq.snrcjt.cn

[S53] C++：移动语义
来源：http://ejf.tanke756.top

std::vector<int> w = std::move(v);
来源：http://tnp.yj202588.top

[S54] C++：异常处理
来源：http://jno.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://edx.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://tmm.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ots.feifeiyinyue.top

[S56] C++：optional
来源：http://rmk.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wfb.gotoacloud.top

[S57] C++：编译期常量
来源：http://ahf.gotoacloud.top

constexpr int N = 10;
来源：http://mgd.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://hmh.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://bls.tian-w.cn

[S59] C++：静态断言
来源：http://ewp.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dod.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://llq.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zrl.shanyushiyangkeji.top

================================================================================
来源：http://hfp.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gld.uphjek.com

================================================================================
来源：http://yht.cucudq.cn

[T01] Kotlin：Hello World
来源：http://xkq.feifeiyinyue.top

println("Hello")
来源：http://tng.gogol.net.cn

[T02] Kotlin：变量
来源：http://pmv.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://osb.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://chm.sjlbkw.cn

"值: $b"
来源：http://blv.guannengcc.top

[T04] Kotlin：空安全
来源：http://gzt.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://zte.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://ybu.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ymx.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://agq.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bmm.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://pjv.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykh.shuidangran.top

[T08] Kotlin：数据类
来源：http://pis.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://leh.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://kog.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://znu.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://mky.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tfh.c1oappe.top

[T11] Kotlin：协程
来源：http://xli.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://hqn.uphjek.com

[T12] Kotlin：解构声明
来源：http://ljo.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://cmf.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://qug.yueranfly.top

val m = mapOf("a" to 1)
来源：http://rok.chenlongwang.top

[T14] Kotlin：循环
来源：http://hvc.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://tqr.zdqjudy.top

[T15] Kotlin：接口
来源：http://sgb.yj202588.top

interface Shape { fun area(): Double }
来源：http://bjl.xinyue.icu

[T16] Swift：Hello World
来源：http://dmv.yuxming.cn

print("Hello")
来源：http://zyj.52xcode.cn

[T17] Swift：变量与常量
来源：http://cce.zycfv.cn

var a = 1;  let b = 2
来源：http://tpb.andypj.xyz

[T18] Swift：字符串插值
来源：http://njd.andypj.xyz

"值: \(b)"
来源：http://nhe.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://voj.hcnkem.com

if let n = opt { print(n) }
来源：http://eyx.yfazqb.com

[T20] Swift：数组操作
来源：http://yvv.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://gqr.chenzaomai.com

[T21] Swift：遍历
来源：http://rqy.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://ygu.yongpay.top

[T22] Swift：字典
来源：http://adu.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wio.aibaodan.cn

[T23] Swift：函数
来源：http://ugo.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zrb.yuxming.cn

[T24] Swift：闭包
来源：http://pnq.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kjr.jlsjyb.cn

[T25] Swift：结构体
来源：http://msm.jlsjyb.cn

struct P { var x: Int }
来源：http://omy.jinqigfzy.top

[T26] Swift：类与重写
来源：http://zjy.ehwqpu.com

class A: Base { override func f() {} }
来源：http://cvr.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://tpp.daxiang520.top

do { try f() } catch { print(error) }
来源：http://itu.zhengqikj.top

[T28] Swift：枚举
来源：http://wan.jinqigfzy.top

enum Color { case red, green }
来源：http://ogr.tarul.cn

[T29] Swift：guard 提前返回
来源：http://jkl.zhiwuduotai.top

guard let x = opt else { return }
来源：http://wnn.yuanzhike.top

[T30] Swift：协议
来源：http://dth.hammf.cn

protocol Shape { func area() -> Double }
来源：http://wxf.daxiang520.top

[T31] Lua：Hello World
来源：http://yji.yj20258888.top

print("Hello")
来源：http://qhm.hfpthk.cn

[T32] Lua：局部变量
来源：http://kae.zhiwuduotai.top

local a = 1
来源：http://dbi.yangfankeji.com

[T33] Lua：表（数组）
来源：http://tun.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wgd.haohaochexian.top

[T34] Lua：遍历表
来源：http://cjt.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mbe.zdbjq.cn

[T35] Lua：字典表
来源：http://aic.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://pdh.jqgufenzy.top

[T36] Lua：函数
来源：http://lxy.hnqzz.top

function add(a, b) return a + b end
来源：http://xkj.xinyue.icu

[T37] Lua：字符串拼接
来源：http://ogp.zhengqikj.top

"a" .. "b"
来源：http://rsx.yonumen.top

[T38] Lua：条件
来源：http://qaj.nanxuanxn.top

if x > 0 then print("正") end
来源：http://ydp.yueranfly.top

[T39] Lua：模式匹配
来源：http://pvy.jqgufenzy.top

string.find(s, "%d+")
来源：http://tbl.jinghuilouyu.cn

[T40] Lua：元表
来源：http://kpc.cheryme.top

setmetatable({}, { __index = base })
来源：http://rov.fzhhl.top

[T41] Perl：Hello World
来源：http://oin.fengsongda.top

print "Hello\n";
来源：http://axo.hywenlv.cn

[T42] Perl：变量类型
来源：http://rop.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://icq.zhengqikj.top

[T43] Perl：字符串插值
来源：http://epa.svipenyu.cn

"值: $a"
来源：http://wwl.shangyingyoupin.top

[T44] Perl：条件
来源：http://sqv.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://oda.guannengcc.top

[T45] Perl：数组遍历
来源：http://elb.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://flj.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://dsq.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vpa.gogol.net.cn

[T47] Perl：正则捕获
来源：http://vcl.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cwi.mhx1999.top

[T48] Perl：正则替换
来源：http://duv.birdmap.top

$s =~ s/old/new/g;
来源：http://tjm.snrcjt.cn

[T49] Perl：函数
来源：http://mjr.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dgn.vehdjk.com

[T50] Perl：逐行读文件
来源：http://lfv.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jwo.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://vdv.bbcook.cn

[T51] Scala：Hello World
来源：http://pxj.sufxvd.cn

println("Hello")
来源：http://rne.havefunace.top

[T52] Scala：变量
来源：http://igb.aibaodan.cn

val a = 1;  var b = 2
来源：http://qew.zdbjq.cn

[T53] Scala：字符串插值
来源：http://bxg.xylfe.cn

s"值: $b"
来源：http://jml.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://afi.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://duh.hywenlv.cn

[T55] Scala：集合过滤
来源：http://qyx.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://ejp.meibo888.top

[T56] Scala：样例类
来源：http://pmh.yj202588.top

case class User(name: String, age: Int)
来源：http://xbw.shzxlz.cn

[T57] Scala：模式匹配
来源：http://yli.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://siv.sysykeji.top

[T58] Scala：函数定义
来源：http://mrs.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bcc.ydjk.org.cn

[T59] Scala：循环
来源：http://tap.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://zal.sysykeji.top

[T60] Scala：折叠
来源：http://cag.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://spl.zhaomingkeji.xyz

================================================================================
来源：http://xly.xziqi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zpp.meibo888.top

================================================================================
来源：http://qiq.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://qyv.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://uiu.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://hbl.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zho.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://gca.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tkd.andypj.xyz

[U04] Py：变量调试打印
来源：http://pdj.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fen.xylfe.cn

[U05] Py：列表去重且保序
来源：http://lhm.cucudq.cn

list(dict.fromkeys(arr))
来源：http://kua.zhixingplan.top

[U06] Py：合并两个字典
来源：http://ymz.fengsongda.top

{**a, **b}
来源：http://tsy.hfpthk.cn

[U07] Py：反转字典键值
来源：http://usg.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://fox.hcnkem.com

[U08] Py：展平二维列表
来源：http://uqi.gogol.net.cn

[y for x in nested for y in x]
来源：http://thb.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://yrd.aibaodan.cn

max(d, key=d.get)
来源：http://pql.yfazqb.com

[U10] Py：按值排序字典
来源：http://vbc.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jec.hywenlv.cn

[U11] Py：生成器表达式
来源：http://bzd.52xcode.cn

(x * 2 for x in arr)
来源：http://hie.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vhh.zycfv.cn

Counter(arr).most_common(3)
来源：http://eic.dashuyun.cn

[U13] Py：固定长度队列
来源：http://fdt.dashuyun.cn

deque(maxlen=10)
来源：http://hxa.yfazqb.com

[U14] Py：分组收集到列表
来源：http://wuj.daxiang520.top

defaultdict(list)
来源：http://lkd.yvedp.cn

[U15] Py：高精度计时
来源：http://sas.guannengcc.top

t = time.perf_counter()
来源：http://qbk.epnwcf.com

[U16] Py：命令行参数解析
来源：http://pqu.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rzx.jiagoushi.top

[U17] Py：初始化日志
来源：http://dke.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://utj.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://mef.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://jng.smart0.xyz

[U19] Py：正则替换带回调
来源：http://scy.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kew.fzhhl.top

[U20] Py：缓存函数结果
来源：http://cft.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://wfi.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://veu.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://pag.iojbl.cn

[U22] Py：矩阵转置
来源：http://pjc.sxryk.cn

list(zip(*m))
来源：http://ghr.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://mvt.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dyc.havefunace.top

[U24] Py：路径操作
来源：http://sie.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fen.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://kfg.dianchejie.cn

csv.DictReader(f)
来源：http://nrt.ydzc1.top

[U26] Py：并发下载
来源：http://glu.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fjm.gogol.net.cn

[U27] Py：异步 HTTP
来源：http://syg.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://xmz.smart0.xyz

[U28] Py：类型别名
来源：http://mdr.vqdsnc.cn

UserId = int
来源：http://fdh.ivvv.top

[U29] Py：属性校验
来源：http://oxz.xuanzx.com

@property 与 @x.setter 配合
来源：http://xxr.yangfankeji.com

[U30] Py：数据类
来源：http://iuz.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://kia.havefunace.top

[U31] Py：单测
来源：http://zmx.epnwcf.com

python -m pytest -q
来源：http://lmx.jyoumei.cn

[U32] Py：代码格式化
来源：http://gvx.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://tor.birdmap.top

[U33] Py：打包发布
来源：http://dfw.fktsv.cn

python -m build  （依赖 pyproject.toml）
来源：http://yxv.yangfankeji.com

[U34] Py：判断编码
来源：http://lmr.fehbvm.com

chardet.detect(raw)
来源：http://xyn.yj20258.top

[U35] Py：发送邮件
来源：http://xap.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qbg.9152youxi.cn

[U36] Py：定时任务
来源：http://psc.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://mvy.ehwqpu.com

[U37] Py：读写 Excel
来源：http://hdd.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ygq.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://pij.fanxiaobao.xyz

Path(__file__).resolve().parent
来源：http://jdi.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://krs.zhoulong.xyz

sys.stdout.isatty()
来源：http://tjp.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://nvr.iojbl.cn

print("err", file=sys.stderr)
来源：http://fdy.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://sok.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xyd.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://nfd.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eiy.fengsongda.top


<!-- 参考信息 -->