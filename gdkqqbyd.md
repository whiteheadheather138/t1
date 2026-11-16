代发 wailian999

int main(int argc, char **argv)
来源：http://xpq.hesvh.cn

[S19] C：快速排序
来源：http://mqs.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://lwv.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://bci.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yml.hfpthk.cn

[S21] C：字符类别判断
来源：http://jjp.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oxw.yvedp.cn

[S22] C：字符串转数字
来源：http://enh.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xmi.hammf.cn

[S23] C：随机数
来源：http://gyo.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tqv.hywenlv.cn

[S24] C：获取本地时间
来源：http://egd.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sfa.zdbjq.cn

[S25] C：内存拷贝
来源：http://pne.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://ykr.zhongyouzk.top

[S26] C：内存清零
来源：http://pfb.tanke756.top

memset(a, 0, sizeof a);
来源：http://uak.vqdsnc.cn

[S27] C：定义常量
来源：http://inn.yonumen.top

const double PI = 3.14159;
来源：http://ago.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://aex.ppjwa.cn

static int counter = 0;
来源：http://fxy.9152youxi.cn

[S29] C：变参函数
来源：http://cxg.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yfq.yanxiufei.cn

[S30] C：头文件保护
来源：http://hez.hongshengwenyu.top

#ifndef X_H
来源：http://ggr.dianchejie.cn

#define X_H
来源：http://abx.jyoumei.cn

#endif
来源：http://tlq.kuanghao11.cn

[S31] C++：Hello World
来源：http://ibw.zhixingplan.top

#include <iostream>
来源：http://gll.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://jpb.shanyushiyangtech.top

[S32] C++：字符串
来源：http://ftq.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://kdi.52xcode.cn

[S33] C++：vector 增删
来源：http://lmj.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pij.cdnleiting.top

[S34] C++：遍历 vector
来源：http://cbv.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://pmk.pycfn.com

[S35] C++：map
来源：http://kjq.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wlz.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://kco.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hzh.ctjpmb.com

[S37] C++：set
来源：http://cod.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ctk.yuanzhike.top

[S38] C++：排序
来源：http://mim.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://byg.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://ndv.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://npq.tian-w.cn

[S40] C++：查找元素
来源：http://znv.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yfi.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://umz.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmy.xinyue.icu

[S42] C++：继承与虚函数
来源：http://ffl.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://ijt.nanxinkj.top

[S43] C++：智能指针
来源：http://kob.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://wrm.fzhhl.top

[S44] C++：引用传参
来源：http://uas.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://vum.chenlongwang.top

[S45] C++：lambda
来源：http://ubp.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://sma.cucudq.cn

[S46] C++：函数模板
来源：http://kfp.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://imj.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://ryh.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kav.yuxming.cn

[S48] C++：逐行读文件
来源：http://cfb.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://pww.pycfn.com

while (std::getline(in, line)) { }
来源：http://xiv.jinqigfzy.top

[S49] C++：写文件
来源：http://eef.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tfa.hcnkem.com

[S50] C++：格式化数字
来源：http://net.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sea.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://ldi.ybcxt.top

static_cast<double>(a) / b
来源：http://mmb.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://nok.nwbrower.top

int size() const noexcept { return n_; }
来源：http://luj.pengpengdd.cyou

[S53] C++：移动语义
来源：http://fzg.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://caj.bbcook.cn

[S54] C++：异常处理
来源：http://tsp.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qjt.birdmap.top

[S55] C++：结构化绑定
来源：http://yas.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oqs.jinghuilouyu.cn

[S56] C++：optional
来源：http://hns.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jgn.svipenyu.cn

[S57] C++：编译期常量
来源：http://oxe.xuetiantiany.cn

constexpr int N = 10;
来源：http://tnl.jinqigufen.top

[S58] C++：命名空间
来源：http://esb.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://grt.iojbl.cn

[S59] C++：静态断言
来源：http://mjm.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwn.pycfn.com

[S60] C++：遍历并删除元素
来源：http://eny.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wyz.daxiang520.top

================================================================================
来源：http://dvi.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gwl.xingfuxueyuan.xyz

================================================================================
来源：http://pij.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://wsr.vehdjk.com

println("Hello")
来源：http://mpj.hnxiangtu.top

[T02] Kotlin：变量
来源：http://nsc.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cnq.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://yri.zdbjq.cn

"值: $b"
来源：http://uhi.hnqzz.top

[T04] Kotlin：空安全
来源：http://jqk.zdbjq.cn

val n: String? = null;  n?.length
来源：http://lvg.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://buv.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvz.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://pfq.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://env.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://wbu.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mvx.fengsongda.top

[T08] Kotlin：数据类
来源：http://syi.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://xzv.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://oxy.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://anu.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://xlc.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zwd.hnqzz.top

[T11] Kotlin：协程
来源：http://eec.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eom.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://pbv.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://xxc.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://whg.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://nax.yj202588.top

[T14] Kotlin：循环
来源：http://nmw.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://xyq.cqqwz.cn

[T15] Kotlin：接口
来源：http://tij.uphjek.com

interface Shape { fun area(): Double }
来源：http://zak.haohaochexian.top

[T16] Swift：Hello World
来源：http://ldz.mhx1999.top

print("Hello")
来源：http://rkg.chenzaomai.com

[T17] Swift：变量与常量
来源：http://idm.jianghu66.top

var a = 1;  let b = 2
来源：http://tzm.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://jdi.fktsv.cn

"值: \(b)"
来源：http://jgt.yonumen.top

[T19] Swift：可选绑定
来源：http://qwb.yanxiufei.cn

if let n = opt { print(n) }
来源：http://ahp.jinqigufen.top

[T20] Swift：数组操作
来源：http://uuh.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://vas.mhx1999.top

[T21] Swift：遍历
来源：http://axd.sxryk.cn

for x in a { print(x) }
来源：http://aav.yvedp.cn

[T22] Swift：字典
来源：http://suz.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://kkx.yongpay.top

[T23] Swift：函数
来源：http://mcc.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogu.snrcjt.cn

[T24] Swift：闭包
来源：http://bqa.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zlp.feifeiyinyue.top

[T25] Swift：结构体
来源：http://rxs.xuetiantiany.cn

struct P { var x: Int }
来源：http://ovt.bbcook.cn

[T26] Swift：类与重写
来源：http://ehb.epnwcf.com

class A: Base { override func f() {} }
来源：http://ocs.nwbrower.top

[T27] Swift：错误处理
来源：http://myf.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://jni.jqgufenzy.top

[T28] Swift：枚举
来源：http://pqq.gogol.net.cn

enum Color { case red, green }
来源：http://dpo.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://oae.yj20258.top

guard let x = opt else { return }
来源：http://zfb.feifeiyinyue.top

[T30] Swift：协议
来源：http://kyi.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://nir.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://qqn.gaohongyu789.top

print("Hello")
来源：http://pqz.jinqigufen.top

[T32] Lua：局部变量
来源：http://bfc.vqdsnc.cn

local a = 1
来源：http://ncf.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://ozg.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cju.jyoumei.cn

[T34] Lua：遍历表
来源：http://zxk.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://rvw.ehwqpu.com

[T35] Lua：字典表
来源：http://xer.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://kdh.gaohongyu789.top

[T36] Lua：函数
来源：http://vpb.yfazqb.com

function add(a, b) return a + b end
来源：http://lfe.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://bhm.yfazqb.com

"a" .. "b"
来源：http://vsa.yuxming.cn

[T38] Lua：条件
来源：http://lpo.fehbvm.com

if x > 0 then print("正") end
来源：http://ano.birdmap.top

[T39] Lua：模式匹配
来源：http://rae.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://jmk.tianlin.xyz

[T40] Lua：元表
来源：http://cyu.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://ahq.yangfankeji.com

[T41] Perl：Hello World
来源：http://liw.zdbjq.cn

print "Hello\n";
来源：http://rxq.c1oappe.top

[T42] Perl：变量类型
来源：http://tpz.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iqz.dashuyun.cn

[T43] Perl：字符串插值
来源：http://tst.hcnkem.com

"值: $a"
来源：http://wnr.hnxiangtu.top

[T44] Perl：条件
来源：http://iju.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://ckb.hywenlv.cn

[T45] Perl：数组遍历
来源：http://toh.316326.xyz

for my $x (@arr) { print $x; }
来源：http://hev.dianchejie.cn

[T46] Perl：哈希操作
来源：http://mzu.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ffj.fengsongda.top

[T47] Perl：正则捕获
来源：http://wgv.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hpv.sjlbkw.cn

[T48] Perl：正则替换
来源：http://zrs.jinqigufen.top

$s =~ s/old/new/g;
来源：http://lfl.bbcook.cn

[T49] Perl：函数
来源：http://tiz.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tis.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://pbw.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gnw.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://loy.jqgfzy.top

[T51] Scala：Hello World
来源：http://mkz.kuanghao11.cn

println("Hello")
来源：http://xqg.yangfankeji.com

[T52] Scala：变量
来源：http://fof.yueranfly.top

val a = 1;  var b = 2
来源：http://vco.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://pdd.jyoumei.cn

s"值: $b"
来源：http://kjl.hammf.cn

[T54] Scala：集合映射
来源：http://nkq.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://wlk.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://rne.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cpc.jlsjyb.cn

[T56] Scala：样例类
来源：http://axk.yueranfly.top

case class User(name: String, age: Int)
来源：http://iqw.zdqjudy.top

[T57] Scala：模式匹配
来源：http://alo.fanxiaobao.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://jol.tarul.cn

[T58] Scala：函数定义
来源：http://hbg.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jzc.tianlin.xyz

[T59] Scala：循环
来源：http://vie.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://bzh.pengpengdd.cyou

[T60] Scala：折叠
来源：http://nyd.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jst.ywan-chungtsiang.top

================================================================================
来源：http://rxm.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sby.jqgufenzy.top

================================================================================
来源：http://vpv.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://gtg.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sbq.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://jpt.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://svy.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://yzn.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rez.dashuyun.cn

[U04] Py：变量调试打印
来源：http://lzd.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trc.xziqi.cn

[U05] Py：列表去重且保序
来源：http://sgb.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://ppu.pycfn.com

[U06] Py：合并两个字典
来源：http://utr.sxryk.cn

{**a, **b}
来源：http://ykf.yueranfly.top

[U07] Py：反转字典键值
来源：http://bxh.meibo888.top

{v: k for k, v in d.items()}
来源：http://uzp.snrcjt.cn

[U08] Py：展平二维列表
来源：http://oqu.daria6918.cn

[y for x in nested for y in x]
来源：http://olx.cashguo.top

[U09] Py：字典取最大值的键
来源：http://vmq.meibo888.top

max(d, key=d.get)
来源：http://rcr.zycfv.cn

[U10] Py：按值排序字典
来源：http://npf.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pjn.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://lvs.sufxvd.cn

(x * 2 for x in arr)
来源：http://ski.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://dpb.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://wbb.hammf.cn

[U13] Py：固定长度队列
来源：http://pph.zdqjudy.top

deque(maxlen=10)
来源：http://jpn.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://lmv.zhengqikj.top

defaultdict(list)
来源：http://aet.zdbjq.cn

[U15] Py：高精度计时
来源：http://vya.yuanzhike.top

t = time.perf_counter()
来源：http://uee.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://zna.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nod.hammf.cn

[U17] Py：初始化日志
来源：http://dft.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://wst.bjfxy.top

[U18] Py：预编译正则
来源：http://tqt.gzhubu.top

pat = re.compile(r"\d+")
来源：http://okl.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://ftb.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eox.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://cgl.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://dpm.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://hio.shuidangran.top

@contextlib.contextmanager
来源：http://amg.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://wws.zdbjq.cn

list(zip(*m))
来源：http://del.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://zxt.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djk.xziqi.cn

[U24] Py：路径操作
来源：http://zcq.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rwk.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://rgs.tian-w.cn

csv.DictReader(f)
来源：http://dcq.xinyue.icu

[U26] Py：并发下载
来源：http://tye.xuetiantiany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://css.yj202588.top

[U27] Py：异步 HTTP
来源：http://wux.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://vkl.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://vqw.hesvh.cn

UserId = int
来源：http://bzt.sjlbkw.cn

[U29] Py：属性校验
来源：http://pka.yuanzhike.top

@property 与 @x.setter 配合
来源：http://zeq.sjlbkw.cn

[U30] Py：数据类
来源：http://uco.9152youxi.cn

@dataclass(slots=True)
来源：http://wpe.hesvh.cn

[U31] Py：单测
来源：http://xde.yonumen.top

python -m pytest -q
来源：http://uli.hammf.cn

[U32] Py：代码格式化
来源：http://tpv.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://olk.316326.xyz

[U33] Py：打包发布
来源：http://hcu.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://njp.iojbl.cn

[U34] Py：判断编码
来源：http://hfy.bbcook.cn

chardet.detect(raw)
来源：http://yhu.tianlin.xyz

[U35] Py：发送邮件
来源：http://mgy.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://frd.jyoumei.cn

[U36] Py：定时任务
来源：http://prs.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://cra.bbcook.cn

[U37] Py：读写 Excel
来源：http://ndq.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://vfc.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://ttm.sweek.top

Path(__file__).resolve().parent
来源：http://wpq.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://sjm.xuetiantiany.cn

sys.stdout.isatty()
来源：http://okp.hcnkem.com

[U40] Py：打印到标准错误
来源：http://cwo.hywenlv.cn

print("err", file=sys.stderr)
来源：http://qhe.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://sel.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tad.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://mfr.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bxt.chenzaomai.com


<!-- 参考信息 -->