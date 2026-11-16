代发 wailian999

int main(int argc, char **argv)
来源：http://suk.ctjpmb.com

[S19] C：快速排序
来源：http://yiy.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://qvy.shanyushiyangtech.top

[S20] C：二分查找
来源：http://wfr.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pha.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://rep.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yto.52xcode.cn

[S22] C：字符串转数字
来源：http://lie.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://qyt.hongshengwenyu.top

[S23] C：随机数
来源：http://iai.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gsi.smart0.xyz

[S24] C：获取本地时间
来源：http://adm.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://suh.jqgfzy.top

[S25] C：内存拷贝
来源：http://nrh.ivvv.top

memcpy(dst, src, n);
来源：http://qic.chenlongwang.top

[S26] C：内存清零
来源：http://snc.iojbl.cn

memset(a, 0, sizeof a);
来源：http://eza.jiagoushi.top

[S27] C：定义常量
来源：http://epb.sjlbkw.cn

const double PI = 3.14159;
来源：http://dkv.haohaochexian.top

[S28] C：静态变量
来源：http://igt.smart0.xyz

static int counter = 0;
来源：http://ltl.yj20258888.top

[S29] C：变参函数
来源：http://lsh.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pov.aibaodan.cn

[S30] C：头文件保护
来源：http://haz.vqdsnc.cn

#ifndef X_H
来源：http://and.yonumen.top

#define X_H
来源：http://aai.52xcode.cn

#endif
来源：http://qpt.316326.xyz

[S31] C++：Hello World
来源：http://khe.gaohongyu789.top

#include <iostream>
来源：http://tts.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://vgl.gotoacloud.top

[S32] C++：字符串
来源：http://rbg.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://tgm.nanxinkj.top

[S33] C++：vector 增删
来源：http://ljh.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ouh.bbcook.cn

[S34] C++：遍历 vector
来源：http://wek.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://kmw.uphjek.com

[S35] C++：map
来源：http://ryc.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gup.zhijiandao.cn

[S36] C++：unordered_map
来源：http://mwq.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://igw.kuanghao11.cn

[S37] C++：set
来源：http://eao.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jdm.jinqigufen.top

[S38] C++：排序
来源：http://mdw.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://fdw.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://snn.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ttg.yj20258.top

[S40] C++：查找元素
来源：http://zbg.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ojl.cheryme.top

[S41] C++：类与构造函数
来源：http://tay.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bgg.meibo888.top

[S42] C++：继承与虚函数
来源：http://hct.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://jgw.dianchejie.cn

[S43] C++：智能指针
来源：http://neh.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://zqe.hammf.cn

[S44] C++：引用传参
来源：http://wfp.wangdashe.top

void inc(int &x) { ++x; }
来源：http://fsl.shuidangran.top

[S45] C++：lambda
来源：http://agc.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://vtu.cucudq.cn

[S46] C++：函数模板
来源：http://byw.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pym.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://ylw.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqr.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://oeq.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://wxh.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://hnd.sweek.top

[S49] C++：写文件
来源：http://nbz.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://muv.dashuyun.cn

[S50] C++：格式化数字
来源：http://oxc.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://twt.shuidangran.top

[S51] C++：显式类型转换
来源：http://pvv.shuidangran.top

static_cast<double>(a) / b
来源：http://wvd.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://ylx.meibo888.top

int size() const noexcept { return n_; }
来源：http://hsl.fehbvm.com

[S53] C++：移动语义
来源：http://gqi.hammf.cn

std::vector<int> w = std::move(v);
来源：http://jzs.hywenlv.cn

[S54] C++：异常处理
来源：http://htv.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gfk.yj202588.top

[S55] C++：结构化绑定
来源：http://axc.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zxh.jiagoushi.top

[S56] C++：optional
来源：http://hpd.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mxj.yj202588.top

[S57] C++：编译期常量
来源：http://aku.ybcxt.top

constexpr int N = 10;
来源：http://pqf.haohaochexian.top

[S58] C++：命名空间
来源：http://cwe.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://gws.yanxiufei.cn

[S59] C++：静态断言
来源：http://oww.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vbr.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://wnl.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nbd.shanyushiyangkeji.top

================================================================================
来源：http://dcq.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mnw.ydjk.org.cn

================================================================================
来源：http://xxs.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://nuj.bjfxy.top

println("Hello")
来源：http://xkt.quarkkingdee.top

[T02] Kotlin：变量
来源：http://rbf.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eav.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://tga.cashguo.top

"值: $b"
来源：http://jzi.havefunace.top

[T04] Kotlin：空安全
来源：http://ezu.ydzc1.top

val n: String? = null;  n?.length
来源：http://vrp.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://prm.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yxu.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://jdr.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://flq.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://jnq.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wgd.andypj.xyz

[T08] Kotlin：数据类
来源：http://bzm.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://ozy.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://khq.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://mjz.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://oax.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wau.epnwcf.com

[T11] Kotlin：协程
来源：http://xoj.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixg.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://cve.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://gqt.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://lsv.cashguo.top

val m = mapOf("a" to 1)
来源：http://moh.hfpthk.cn

[T14] Kotlin：循环
来源：http://fxw.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://pbu.bjfxy.top

[T15] Kotlin：接口
来源：http://ylf.yj202588.top

interface Shape { fun area(): Double }
来源：http://ome.zdbjq.cn

[T16] Swift：Hello World
来源：http://fko.jianghu66.top

print("Hello")
来源：http://ywm.yj202588.top

[T17] Swift：变量与常量
来源：http://bcp.cheryme.top

var a = 1;  let b = 2
来源：http://mwv.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://uza.chenlongwang.top

"值: \(b)"
来源：http://qlr.zdqjudy.top

[T19] Swift：可选绑定
来源：http://uis.zhengqikj.top

if let n = opt { print(n) }
来源：http://xqw.wangdashe.top

[T20] Swift：数组操作
来源：http://wds.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://wvq.yuxming.cn

[T21] Swift：遍历
来源：http://tdn.shzxlz.cn

for x in a { print(x) }
来源：http://cxg.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://vax.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://lvy.jyoumei.cn

[T23] Swift：函数
来源：http://ibj.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dks.cucudq.cn

[T24] Swift：闭包
来源：http://wgk.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://osf.daxiang520.top

[T25] Swift：结构体
来源：http://ree.hesvh.cn

struct P { var x: Int }
来源：http://jxg.9152youxi.cn

[T26] Swift：类与重写
来源：http://cgn.52xcode.cn

class A: Base { override func f() {} }
来源：http://sge.zdqjudy.top

[T27] Swift：错误处理
来源：http://jki.cucudq.cn

do { try f() } catch { print(error) }
来源：http://mch.jianghu66.top

[T28] Swift：枚举
来源：http://don.zhiwuduotai.top

enum Color { case red, green }
来源：http://equ.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://lhi.epnwcf.com

guard let x = opt else { return }
来源：http://dkn.daxiang520.top

[T30] Swift：协议
来源：http://vaq.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://mnu.guowangkeji.top

[T31] Lua：Hello World
来源：http://qpm.zhongyouzk.top

print("Hello")
来源：http://zgq.snrcjt.cn

[T32] Lua：局部变量
来源：http://qip.hcnkem.com

local a = 1
来源：http://bjr.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://hqf.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vei.cqqwz.cn

[T34] Lua：遍历表
来源：http://nvj.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jxy.xylfe.cn

[T35] Lua：字典表
来源：http://xnt.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://syp.bbcook.cn

[T36] Lua：函数
来源：http://fhq.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://jik.uphjek.com

[T37] Lua：字符串拼接
来源：http://zdm.yfazqb.com

"a" .. "b"
来源：http://hjr.epnwcf.com

[T38] Lua：条件
来源：http://dhs.52xcode.cn

if x > 0 then print("正") end
来源：http://ohc.tanke756.top

[T39] Lua：模式匹配
来源：http://jel.shuidangran.top

string.find(s, "%d+")
来源：http://pti.dianchejie.cn

[T40] Lua：元表
来源：http://ynu.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://zcp.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://zhf.9152youxi.cn

print "Hello\n";
来源：http://jxi.hnqzz.top

[T42] Perl：变量类型
来源：http://upg.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pii.yj202588.top

[T43] Perl：字符串插值
来源：http://pyh.xuetiantiany.cn

"值: $a"
来源：http://qor.dianchejie.cn

[T44] Perl：条件
来源：http://pyx.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://fct.shuidangran.top

[T45] Perl：数组遍历
来源：http://ckj.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://aca.ppjwa.cn

[T46] Perl：哈希操作
来源：http://krw.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jny.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://eig.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://jkn.kuanghao11.cn

[T48] Perl：正则替换
来源：http://lfg.yongpay.top

$s =~ s/old/new/g;
来源：http://kon.dianchejie.cn

[T49] Perl：函数
来源：http://twa.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://edi.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://vix.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cke.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://xoj.chenzaomai.com

[T51] Scala：Hello World
来源：http://jek.aibaodan.cn

println("Hello")
来源：http://cqp.zhoulong.xyz

[T52] Scala：变量
来源：http://dqr.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://szy.yfazqb.com

[T53] Scala：字符串插值
来源：http://pql.xziqi.cn

s"值: $b"
来源：http://ddo.epnwcf.com

[T54] Scala：集合映射
来源：http://pia.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://agf.wangdashe.top

[T55] Scala：集合过滤
来源：http://dvi.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://bmj.hywenlv.cn

[T56] Scala：样例类
来源：http://jcx.zhixingplan.top

case class User(name: String, age: Int)
来源：http://xow.wangdashe.top

[T57] Scala：模式匹配
来源：http://lzw.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xap.yvedp.cn

[T58] Scala：函数定义
来源：http://rpv.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rdt.sxryk.cn

[T59] Scala：循环
来源：http://aae.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://luv.hfpthk.cn

[T60] Scala：折叠
来源：http://pjh.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qra.yangfankeji.com

================================================================================
来源：http://bnj.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zjo.zdbjq.cn

================================================================================
来源：http://obs.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://jfc.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://cgo.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://los.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hxs.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://cxz.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nrs.ehwqpu.com

[U04] Py：变量调试打印
来源：http://kri.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gjq.nwbrower.top

[U05] Py：列表去重且保序
来源：http://srn.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://jdq.nanxinkj.top

[U06] Py：合并两个字典
来源：http://fhs.fzhhl.top

{**a, **b}
来源：http://nkm.aibaodan.cn

[U07] Py：反转字典键值
来源：http://gcu.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://vpv.yongpay.top

[U08] Py：展平二维列表
来源：http://pxn.zycfv.cn

[y for x in nested for y in x]
来源：http://jec.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://elw.xuanzx.com

max(d, key=d.get)
来源：http://vkf.vehdjk.com

[U10] Py：按值排序字典
来源：http://ezb.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ppi.yvedp.cn

[U11] Py：生成器表达式
来源：http://ftq.jlsjyb.cn

(x * 2 for x in arr)
来源：http://kfb.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://scs.ybcxt.top

Counter(arr).most_common(3)
来源：http://asb.haohaochexian.top

[U13] Py：固定长度队列
来源：http://zmb.cqqwz.cn

deque(maxlen=10)
来源：http://fbo.xylfe.cn

[U14] Py：分组收集到列表
来源：http://gki.fzhhl.top

defaultdict(list)
来源：http://uok.ydzc1.top

[U15] Py：高精度计时
来源：http://upo.nanxuanxn.top

t = time.perf_counter()
来源：http://ohj.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://orm.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qed.c1oappe.top

[U17] Py：初始化日志
来源：http://cvv.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://nrb.c1oappe.top

[U18] Py：预编译正则
来源：http://ywu.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://oeg.shuidangran.top

[U19] Py：正则替换带回调
来源：http://ije.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ych.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ojd.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://wpl.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://yhh.bbcook.cn

@contextlib.contextmanager
来源：http://ftv.jiagoushi.top

[U22] Py：矩阵转置
来源：http://ojs.shanyushiyangkeji.top

list(zip(*m))
来源：http://njz.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://ico.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nhv.zhiwuduotai.top

[U24] Py：路径操作
来源：http://eis.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://igt.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://agh.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://dwh.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://skj.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://imr.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://kzg.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://qwa.cashguo.top

[U28] Py：类型别名
来源：http://ppl.yfazqb.com

UserId = int
来源：http://fsc.hnxiangtu.top

[U29] Py：属性校验
来源：http://spl.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://uzd.gzhubu.top

[U30] Py：数据类
来源：http://ard.yangfankeji.com

@dataclass(slots=True)
来源：http://oih.yanxiufei.cn

[U31] Py：单测
来源：http://nhl.yueranfly.top

python -m pytest -q
来源：http://yzq.hywenlv.cn

[U32] Py：代码格式化
来源：http://hgo.birdmap.top

ruff format . && ruff check --fix .
来源：http://ukw.snrcjt.cn

[U33] Py：打包发布
来源：http://xmg.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://zkt.jianghu66.top

[U34] Py：判断编码
来源：http://inb.zhixingplan.top

chardet.detect(raw)
来源：http://ibd.sxryk.cn

[U35] Py：发送邮件
来源：http://vnu.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kjp.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://jdq.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://san.zycfv.cn

[U37] Py：读写 Excel
来源：http://blw.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ugn.guannengcc.top

[U38] Py：获取脚本所在目录
来源：http://bbl.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://qgh.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://djp.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://nrh.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://jzy.ivvv.top

print("err", file=sys.stderr)
来源：http://lxc.xylfe.cn

[U41] PHP：初始化 Composer 项目
来源：http://mkg.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gun.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://xfa.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zoq.vqdsnc.cn


<!-- 参考信息 -->