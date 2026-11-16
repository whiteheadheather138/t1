代发 wailian999

x |= (1 << 3);
来源：http://vmq.epnwcf.com

[S17] C：安全拼接字符串
来源：http://kja.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hok.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://jbx.nanxinkj.top

int main(int argc, char **argv)
来源：http://fkt.yueranfly.top

[S19] C：快速排序
来源：http://xlt.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://hla.yj202588.top

[S20] C：二分查找
来源：http://dwt.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://adb.yj202588.top

[S21] C：字符类别判断
来源：http://oxs.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bdn.haohaochexian.top

[S22] C：字符串转数字
来源：http://ymd.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://mus.hongshengwenyu.top

[S23] C：随机数
来源：http://iqa.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zuj.hfpthk.cn

[S24] C：获取本地时间
来源：http://sis.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iyb.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://zpx.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://foo.fengsongda.top

[S26] C：内存清零
来源：http://pva.cashguo.top

memset(a, 0, sizeof a);
来源：http://xyq.tian-w.cn

[S27] C：定义常量
来源：http://jwb.xylfe.cn

const double PI = 3.14159;
来源：http://czb.chenjidiqi.icu

[S28] C：静态变量
来源：http://cgn.smart0.xyz

static int counter = 0;
来源：http://uwy.shuidangran.top

[S29] C：变参函数
来源：http://yro.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mht.yj20258.top

[S30] C：头文件保护
来源：http://kfd.jinqigfzy.top

#ifndef X_H
来源：http://flz.jiagoushi.top

#define X_H
来源：http://uex.yangfankeji.com

#endif
来源：http://npo.c1oappe.top

[S31] C++：Hello World
来源：http://eff.tian-w.cn

#include <iostream>
来源：http://enh.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://omi.zhoulong.xyz

[S32] C++：字符串
来源：http://dum.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://gak.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://zol.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ocb.fehbvm.com

[S34] C++：遍历 vector
来源：http://smo.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://jvq.ppjwa.cn

[S35] C++：map
来源：http://mht.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vdy.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://fjz.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://azb.ppjwa.cn

[S37] C++：set
来源：http://wvu.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tyw.wangdashe.top

[S38] C++：排序
来源：http://ujq.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://wqr.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://yue.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kbs.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://eml.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yxk.ybcxt.top

[S41] C++：类与构造函数
来源：http://nfb.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hqd.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://utz.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://mce.pycfn.com

[S43] C++：智能指针
来源：http://ima.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://gxk.zhoulong.xyz

[S44] C++：引用传参
来源：http://rdx.uphjek.com

void inc(int &x) { ++x; }
来源：http://ltr.zhongyouzk.top

[S45] C++：lambda
来源：http://sef.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://pql.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://jye.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pdj.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://wyx.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hgq.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://oam.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ajc.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://bba.bbcook.cn

[S49] C++：写文件
来源：http://wcq.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jwp.epnwcf.com

[S50] C++：格式化数字
来源：http://pwo.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hof.daxiang520.top

[S51] C++：显式类型转换
来源：http://uyc.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://wrr.yongpay.top

[S52] C++：const 与 noexcept
来源：http://iri.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://hly.tanke756.top

[S53] C++：移动语义
来源：http://gfv.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://vkk.hysaishi.cn

[S54] C++：异常处理
来源：http://pvj.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xoq.yj202588.top

[S55] C++：结构化绑定
来源：http://iuh.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ijd.tarul.cn

[S56] C++：optional
来源：http://anc.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vsv.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://jne.zhijiandao.cn

constexpr int N = 10;
来源：http://gou.xuetiantiany.cn

[S58] C++：命名空间
来源：http://oxm.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://hka.xziqi.cn

[S59] C++：静态断言
来源：http://itu.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cuo.sweek.top

[S60] C++：遍历并删除元素
来源：http://rwt.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vke.cashguo.top

================================================================================
来源：http://zaj.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnj.jinqigufen.top

================================================================================
来源：http://lwc.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://zjx.vqdsnc.cn

println("Hello")
来源：http://ngf.guannengcc.top

[T02] Kotlin：变量
来源：http://ecp.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ekh.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://xjg.ydjk.org.cn

"值: $b"
来源：http://mxe.yangfankeji.com

[T04] Kotlin：空安全
来源：http://bve.zhengqikj.top

val n: String? = null;  n?.length
来源：http://lmn.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://emj.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lqn.sysykeji.top

[T06] Kotlin：集合映射
来源：http://kvf.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pqb.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://wvu.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://nsa.hfpthk.cn

[T08] Kotlin：数据类
来源：http://wyw.ivvv.top

data class User(val name: String, val age: Int)
来源：http://zwm.yonumen.top

[T09] Kotlin：扩展函数
来源：http://uqr.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://sbl.shzxlz.cn

[T10] Kotlin：默认参数
来源：http://yny.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ayc.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://yxu.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pox.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://jrd.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://hec.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://ete.fengsongda.top

val m = mapOf("a" to 1)
来源：http://gya.hesvh.cn

[T14] Kotlin：循环
来源：http://nxy.havefunace.top

for (i in 1..10) println(i)
来源：http://mow.uphjek.com

[T15] Kotlin：接口
来源：http://all.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://oal.kuanghao11.cn

[T16] Swift：Hello World
来源：http://opu.jqgfzy.top

print("Hello")
来源：http://nyv.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://vkp.jiagoushi.top

var a = 1;  let b = 2
来源：http://tlu.svipenyu.cn

[T18] Swift：字符串插值
来源：http://goy.yj20258888.top

"值: \(b)"
来源：http://dzg.zycfv.cn

[T19] Swift：可选绑定
来源：http://gay.bjfxy.top

if let n = opt { print(n) }
来源：http://tlf.epnwcf.com

[T20] Swift：数组操作
来源：http://bbu.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://den.jqgufenzy.top

[T21] Swift：遍历
来源：http://oix.aibaodan.cn

for x in a { print(x) }
来源：http://jwr.snrcjt.cn

[T22] Swift：字典
来源：http://aqx.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://nvp.pengpengdd.cyou

[T23] Swift：函数
来源：http://paa.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gzm.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://hmz.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xvh.guannengcc.top

[T25] Swift：结构体
来源：http://iqg.hywenlv.cn

struct P { var x: Int }
来源：http://epp.sweek.top

[T26] Swift：类与重写
来源：http://ana.chenzaomai.com

class A: Base { override func f() {} }
来源：http://mdl.tian-w.cn

[T27] Swift：错误处理
来源：http://rhj.xylfe.cn

do { try f() } catch { print(error) }
来源：http://tmo.xinyue.icu

[T28] Swift：枚举
来源：http://rdp.bbcook.cn

enum Color { case red, green }
来源：http://bzt.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://leh.tarul.cn

guard let x = opt else { return }
来源：http://atu.ydjk.org.cn

[T30] Swift：协议
来源：http://crk.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://shp.bjfxy.top

[T31] Lua：Hello World
来源：http://ljb.xuanzx.com

print("Hello")
来源：http://vwf.cqqwz.cn

[T32] Lua：局部变量
来源：http://gyv.dianchejie.cn

local a = 1
来源：http://hry.shzxlz.cn

[T33] Lua：表（数组）
来源：http://srb.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kvq.yvedp.cn

[T34] Lua：遍历表
来源：http://erj.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jbv.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://naw.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://phv.ydjk.org.cn

[T36] Lua：函数
来源：http://rxh.cheryme.top

function add(a, b) return a + b end
来源：http://yae.redwolf501.top

[T37] Lua：字符串拼接
来源：http://tsh.nanxinkj.top

"a" .. "b"
来源：http://sqp.nanxinkj.top

[T38] Lua：条件
来源：http://ovg.jinqigfzy.top

if x > 0 then print("正") end
来源：http://tqx.haohaochexian.top

[T39] Lua：模式匹配
来源：http://qti.gotoacloud.top

string.find(s, "%d+")
来源：http://mui.yvedp.cn

[T40] Lua：元表
来源：http://hbj.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://rge.jlsjyb.cn

[T41] Perl：Hello World
来源：http://ipw.tian-w.cn

print "Hello\n";
来源：http://dgo.zhoulong.xyz

[T42] Perl：变量类型
来源：http://wwp.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://seb.52xcode.cn

[T43] Perl：字符串插值
来源：http://wix.haohaochexian.top

"值: $a"
来源：http://mwt.yangfankeji.com

[T44] Perl：条件
来源：http://xfk.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://rcc.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://whi.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://hed.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://fbj.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jci.fengsongda.top

[T47] Perl：正则捕获
来源：http://tkj.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dck.bjfxy.top

[T48] Perl：正则替换
来源：http://xju.zhixingplan.top

$s =~ s/old/new/g;
来源：http://urs.aibaodan.cn

[T49] Perl：函数
来源：http://mir.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qrq.c1oappe.top

[T50] Perl：逐行读文件
来源：http://wuc.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ssy.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://pou.gotoacloud.top

[T51] Scala：Hello World
来源：http://mom.zhixingplan.top

println("Hello")
来源：http://ujo.ppjwa.cn

[T52] Scala：变量
来源：http://qwh.bjfxy.top

val a = 1;  var b = 2
来源：http://wpw.yj20258.top

[T53] Scala：字符串插值
来源：http://qei.svipenyu.cn

s"值: $b"
来源：http://cjz.redwolf501.top

[T54] Scala：集合映射
来源：http://oqi.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://emb.yongpay.top

[T55] Scala：集合过滤
来源：http://wwo.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://phj.smart0.xyz

[T56] Scala：样例类
来源：http://lhb.dianchejie.cn

case class User(name: String, age: Int)
来源：http://dfu.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://tqt.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://vix.yfazqb.com

[T58] Scala：函数定义
来源：http://mra.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uqc.ybcxt.top

[T59] Scala：循环
来源：http://oxa.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://kxu.gzhubu.top

[T60] Scala：折叠
来源：http://sdp.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mhg.aizwys.cn

================================================================================
来源：http://uqg.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://afz.daxiang520.top

================================================================================
来源：http://aih.tanke756.top

[U01] Py：创建虚拟环境
来源：http://qpa.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://dau.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://ejt.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aqc.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://zcf.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dzu.hnqzz.top

[U04] Py：变量调试打印
来源：http://qok.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccp.ivvv.top

[U05] Py：列表去重且保序
来源：http://zlx.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://xde.gogol.net.cn

[U06] Py：合并两个字典
来源：http://tqp.yangfankeji.com

{**a, **b}
来源：http://zdv.ppjwa.cn

[U07] Py：反转字典键值
来源：http://xbq.cheryme.top

{v: k for k, v in d.items()}
来源：http://jen.dashuyun.cn

[U08] Py：展平二维列表
来源：http://buu.andypj.xyz

[y for x in nested for y in x]
来源：http://bcx.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://utl.zhixingplan.top

max(d, key=d.get)
来源：http://sqb.fktsv.cn

[U10] Py：按值排序字典
来源：http://aze.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nfh.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://whw.jiagoushi.top

(x * 2 for x in arr)
来源：http://fur.ydzc1.top

[U12] Py：取出现最多的 3 个元素
来源：http://zeu.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://oyl.smart0.xyz

[U13] Py：固定长度队列
来源：http://jhn.cqqwz.cn

deque(maxlen=10)
来源：http://hmx.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://tzs.epnwcf.com

defaultdict(list)
来源：http://yis.xylfe.cn

[U15] Py：高精度计时
来源：http://pvu.hammf.cn

t = time.perf_counter()
来源：http://xrv.xziqi.cn

[U16] Py：命令行参数解析
来源：http://veo.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jjc.vqdsnc.cn

[U17] Py：初始化日志
来源：http://yhn.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://gig.shanyushiyangkeji.top

[U18] Py：预编译正则
来源：http://aep.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://edg.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://fac.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://axn.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://rki.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://vwc.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://ent.shuidangran.top

@contextlib.contextmanager
来源：http://flb.316326.xyz

[U22] Py：矩阵转置
来源：http://jmp.jiagoushi.top

list(zip(*m))
来源：http://ssv.tian-w.cn

[U23] Py：分块读取大文件
来源：http://coy.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dvb.jyoumei.cn

[U24] Py：路径操作
来源：http://rkk.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mhl.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://ocy.316326.xyz

csv.DictReader(f)
来源：http://vey.sufxvd.cn

[U26] Py：并发下载
来源：http://kji.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qsw.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://ynr.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://jcv.zycfv.cn

[U28] Py：类型别名
来源：http://gfe.jiagoushi.top

UserId = int
来源：http://yzf.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://qae.dianchejie.cn

@property 与 @x.setter 配合
来源：http://bil.jyoumei.cn

[U30] Py：数据类
来源：http://iwa.chenzaomai.com

@dataclass(slots=True)
来源：http://xrn.0kj1m.cn

[U31] Py：单测
来源：http://jet.ivvv.top

python -m pytest -q
来源：http://gbm.zhixingplan.top

[U32] Py：代码格式化
来源：http://jvo.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://fmu.meibo888.top

[U33] Py：打包发布
来源：http://qqq.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://bag.andypj.xyz

[U34] Py：判断编码
来源：http://ouj.fengsongda.top

chardet.detect(raw)
来源：http://krc.zhengqikj.top

[U35] Py：发送邮件
来源：http://tkq.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://arl.zdqjudy.top

[U36] Py：定时任务
来源：http://gmy.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://jbt.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://zft.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://xvb.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://xuz.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://lar.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://fhp.jinqigufen.top

sys.stdout.isatty()
来源：http://fij.tarul.cn

[U40] Py：打印到标准错误
来源：http://sga.hywenlv.cn

print("err", file=sys.stderr)
来源：http://nmz.jqgfzy.top


<!-- 参考信息 -->