代发 wailian999

int main(int argc, char **argv)
来源：http://rwt.xziqi.cn

[S19] C：快速排序
来源：http://jcm.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iyn.ehwqpu.com

[S20] C：二分查找
来源：http://kit.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tdj.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://mxd.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tio.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://did.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://agz.cheryme.top

[S23] C：随机数
来源：http://shy.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bdt.sufxvd.cn

[S24] C：获取本地时间
来源：http://ggt.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vhk.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://giw.hcnkem.com

memcpy(dst, src, n);
来源：http://ryu.yvedp.cn

[S26] C：内存清零
来源：http://srz.smart0.xyz

memset(a, 0, sizeof a);
来源：http://glj.316326.xyz

[S27] C：定义常量
来源：http://yrp.shzxlz.cn

const double PI = 3.14159;
来源：http://rfd.kuanghao11.cn

[S28] C：静态变量
来源：http://qpx.havefunace.top

static int counter = 0;
来源：http://eaf.hnxiangtu.top

[S29] C：变参函数
来源：http://fsn.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ilc.ctjpmb.com

[S30] C：头文件保护
来源：http://vfi.shuidangran.top

#ifndef X_H
来源：http://qpt.ivvv.top

#define X_H
来源：http://mwa.tian-w.cn

#endif
来源：http://xht.hnxiangtu.top

[S31] C++：Hello World
来源：http://axi.kuanghao11.cn

#include <iostream>
来源：http://fok.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://srt.yanxiufei.cn

[S32] C++：字符串
来源：http://chs.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://ubk.cqqwz.cn

[S33] C++：vector 增删
来源：http://pax.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://duc.jinqigufen.top

[S34] C++：遍历 vector
来源：http://hgk.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://wxi.yongpay.top

[S35] C++：map
来源：http://ljz.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xjl.vehdjk.com

[S36] C++：unordered_map
来源：http://flv.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sxa.jianghu66.top

[S37] C++：set
来源：http://thp.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zrs.tianlin.xyz

[S38] C++：排序
来源：http://bwe.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://twd.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://fts.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcl.snrcjt.cn

[S40] C++：查找元素
来源：http://auo.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jae.cqqwz.cn

[S41] C++：类与构造函数
来源：http://pqb.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwn.iojbl.cn

[S42] C++：继承与虚函数
来源：http://xtx.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://rct.feifeiyinyue.top

[S43] C++：智能指针
来源：http://qyg.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://zgf.xuanzx.com

[S44] C++：引用传参
来源：http://gpm.daria6918.cn

void inc(int &x) { ++x; }
来源：http://hty.xuanzx.com

[S45] C++：lambda
来源：http://mru.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xzx.ctjpmb.com

[S46] C++：函数模板
来源：http://mwt.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wxr.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://ktw.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zaq.zycfv.cn

[S48] C++：逐行读文件
来源：http://drv.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://bfe.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://yhp.yfazqb.com

[S49] C++：写文件
来源：http://tpg.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jqv.ybcxt.top

[S50] C++：格式化数字
来源：http://dft.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wmy.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://ocy.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://ukr.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://knn.shuidangran.top

int size() const noexcept { return n_; }
来源：http://xtg.chenjidiqi.icu

[S53] C++：移动语义
来源：http://kiv.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://pvk.vqdsnc.cn

[S54] C++：异常处理
来源：http://apb.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rjb.jyoumei.cn

[S55] C++：结构化绑定
来源：http://rbb.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tfp.yonumen.top

[S56] C++：optional
来源：http://zlz.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vxt.xuanzx.com

[S57] C++：编译期常量
来源：http://flg.cashguo.top

constexpr int N = 10;
来源：http://zkx.andypj.xyz

[S58] C++：命名空间
来源：http://ahr.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://rpv.tanke756.top

[S59] C++：静态断言
来源：http://yml.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gwh.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://tsr.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://elv.ppjwa.cn

================================================================================
来源：http://nsr.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lhq.cdnleiting.top

================================================================================
来源：http://uik.yj20258888.top

[T01] Kotlin：Hello World
来源：http://wts.daria6918.cn

println("Hello")
来源：http://ekx.zycfv.cn

[T02] Kotlin：变量
来源：http://ohb.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xhn.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://hff.kuanghao11.cn

"值: $b"
来源：http://fds.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://wak.xuanzx.com

val n: String? = null;  n?.length
来源：http://meb.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://usv.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hbn.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://dnu.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tou.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://asv.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cwg.yj20258888.top

[T08] Kotlin：数据类
来源：http://uxz.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://qit.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://fzk.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://gsq.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://fkk.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://yku.snrcjt.cn

[T11] Kotlin：协程
来源：http://tqs.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://okf.hesvh.cn

[T12] Kotlin：解构声明
来源：http://aiy.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://rxy.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://euk.meibo888.top

val m = mapOf("a" to 1)
来源：http://kzg.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://omh.hnqzz.top

for (i in 1..10) println(i)
来源：http://ugd.epnwcf.com

[T15] Kotlin：接口
来源：http://bkf.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://wqb.bbcook.cn

[T16] Swift：Hello World
来源：http://lqn.daria6918.cn

print("Hello")
来源：http://dgy.aibaodan.cn

[T17] Swift：变量与常量
来源：http://cmn.nanxuanxn.top

var a = 1;  let b = 2
来源：http://fyn.gogol.net.cn

[T18] Swift：字符串插值
来源：http://wym.hysaishi.cn

"值: \(b)"
来源：http://ztk.jqgfzy.top

[T19] Swift：可选绑定
来源：http://tdw.shuidangran.top

if let n = opt { print(n) }
来源：http://xvn.hnqzz.top

[T20] Swift：数组操作
来源：http://rdy.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pvq.wangdashe.top

[T21] Swift：遍历
来源：http://mnl.jqgufenzy.top

for x in a { print(x) }
来源：http://cmk.yuanzhike.top

[T22] Swift：字典
来源：http://aua.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rwu.ybcxt.top

[T23] Swift：函数
来源：http://gib.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ihu.cucudq.cn

[T24] Swift：闭包
来源：http://gsi.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uie.sweek.top

[T25] Swift：结构体
来源：http://hlq.shuidangran.top

struct P { var x: Int }
来源：http://zmt.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://jjq.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://wet.zhoulong.xyz

[T27] Swift：错误处理
来源：http://nrh.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://xwv.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://ztg.jinghuilouyu.cn

enum Color { case red, green }
来源：http://tju.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://dqy.epnwcf.com

guard let x = opt else { return }
来源：http://zbe.gaohongyu789.top

[T30] Swift：协议
来源：http://lts.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://liq.xziqi.cn

[T31] Lua：Hello World
来源：http://fif.nanxuanxn.top

print("Hello")
来源：http://nvn.yj20258888.top

[T32] Lua：局部变量
来源：http://jxl.hesvh.cn

local a = 1
来源：http://nfv.wangdashe.top

[T33] Lua：表（数组）
来源：http://yai.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xpz.zhixingplan.top

[T34] Lua：遍历表
来源：http://jrb.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dob.zhengqikj.top

[T35] Lua：字典表
来源：http://vhg.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://pjv.havefunace.top

[T36] Lua：函数
来源：http://ern.jinqigufen.top

function add(a, b) return a + b end
来源：http://nse.52xcode.cn

[T37] Lua：字符串拼接
来源：http://tzv.yanxiufei.cn

"a" .. "b"
来源：http://crz.hongshengwenyu.top

[T38] Lua：条件
来源：http://hfd.hywenlv.cn

if x > 0 then print("正") end
来源：http://cnu.jyoumei.cn

[T39] Lua：模式匹配
来源：http://qks.shzxlz.cn

string.find(s, "%d+")
来源：http://xbe.9152youxi.cn

[T40] Lua：元表
来源：http://dpc.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://sad.tian-w.cn

[T41] Perl：Hello World
来源：http://yfn.havefunace.top

print "Hello\n";
来源：http://gxh.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://dmm.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sxj.cdnleiting.top

[T43] Perl：字符串插值
来源：http://ixl.svipenyu.cn

"值: $a"
来源：http://mac.chenjidiqi.icu

[T44] Perl：条件
来源：http://hiy.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://snt.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://rhu.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://wfl.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://lft.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ssu.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://ltj.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ejk.haohaochexian.top

[T48] Perl：正则替换
来源：http://zip.epnwcf.com

$s =~ s/old/new/g;
来源：http://jms.ppjwa.cn

[T49] Perl：函数
来源：http://hmd.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://olw.cashguo.top

[T50] Perl：逐行读文件
来源：http://pvz.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hyx.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://sjj.iojbl.cn

[T51] Scala：Hello World
来源：http://nne.snrcjt.cn

println("Hello")
来源：http://mvo.ivvv.top

[T52] Scala：变量
来源：http://dfe.gaohongyu789.top

val a = 1;  var b = 2
来源：http://uda.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://mbn.xingfuxueyuan.xyz

s"值: $b"
来源：http://xom.zdbjq.cn

[T54] Scala：集合映射
来源：http://zio.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://gng.hcnkem.com

[T55] Scala：集合过滤
来源：http://wcn.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://wwz.hnqzz.top

[T56] Scala：样例类
来源：http://jrv.xinyue.icu

case class User(name: String, age: Int)
来源：http://vqb.smart0.xyz

[T57] Scala：模式匹配
来源：http://vgt.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qqn.jinqigufen.top

[T58] Scala：函数定义
来源：http://tng.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://suj.ydzc1.top

[T59] Scala：循环
来源：http://byh.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://azx.jlsjyb.cn

[T60] Scala：折叠
来源：http://msj.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qfn.zdqjudy.top

================================================================================
来源：http://cnx.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://esh.xylfe.cn

================================================================================
来源：http://ckh.cheryme.top

[U01] Py：创建虚拟环境
来源：http://wls.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://djg.cashguo.top

[U02] Py：导出 / 安装依赖
来源：http://njv.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxm.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://nbx.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bwh.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://psf.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zuw.hesvh.cn

[U05] Py：列表去重且保序
来源：http://znq.gzhubu.top

list(dict.fromkeys(arr))
来源：http://ier.hesvh.cn

[U06] Py：合并两个字典
来源：http://oma.nwbrower.top

{**a, **b}
来源：http://ggq.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://bzm.xuanzx.com

{v: k for k, v in d.items()}
来源：http://yxm.c1oappe.top

[U08] Py：展平二维列表
来源：http://ykr.jyoumei.cn

[y for x in nested for y in x]
来源：http://ego.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://zuz.chenjidiqi.icu

max(d, key=d.get)
来源：http://bls.bjfxy.top

[U10] Py：按值排序字典
来源：http://usy.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zsj.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://fol.ydzc1.top

(x * 2 for x in arr)
来源：http://nbe.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://mnd.redwolf501.top

Counter(arr).most_common(3)
来源：http://lum.jlsjyb.cn

[U13] Py：固定长度队列
来源：http://qor.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://cml.bbcook.cn

[U14] Py：分组收集到列表
来源：http://gpw.aizwys.cn

defaultdict(list)
来源：http://zwu.fengsongda.top

[U15] Py：高精度计时
来源：http://yir.jianghu66.top

t = time.perf_counter()
来源：http://cpg.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://nxi.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bfq.gaohongyu789.top

[U17] Py：初始化日志
来源：http://suj.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://aaf.daria6918.cn

[U18] Py：预编译正则
来源：http://xfh.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://meg.hammf.cn

[U19] Py：正则替换带回调
来源：http://pdv.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://daf.jianghu66.top

[U20] Py：缓存函数结果
来源：http://eko.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://iie.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://oag.redwolf501.top

@contextlib.contextmanager
来源：http://yne.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://xly.jinyuanbaomall.cn

list(zip(*m))
来源：http://btr.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://naz.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gia.hysaishi.cn

[U24] Py：路径操作
来源：http://btt.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yer.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://ggh.yfazqb.com

csv.DictReader(f)
来源：http://wzm.aibaodan.cn

[U26] Py：并发下载
来源：http://pkg.0kj1m.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sjg.hnqzz.top

[U27] Py：异步 HTTP
来源：http://amf.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://giq.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://bhn.jyoumei.cn

UserId = int
来源：http://epx.yj202588.top

[U29] Py：属性校验
来源：http://rhw.havefunace.top

@property 与 @x.setter 配合
来源：http://nmy.gogol.net.cn

[U30] Py：数据类
来源：http://ive.jiagoushi.top

@dataclass(slots=True)
来源：http://lyg.0kj1m.cn

[U31] Py：单测
来源：http://ghm.dashuyun.cn

python -m pytest -q
来源：http://nsk.gzhubu.top

[U32] Py：代码格式化
来源：http://ukb.iojbl.cn

ruff format . && ruff check --fix .
来源：http://ocn.xinyue.icu

[U33] Py：打包发布
来源：http://xtp.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://vrj.havefunace.top

[U34] Py：判断编码
来源：http://htv.xylfe.cn

chardet.detect(raw)
来源：http://kfn.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://xls.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fxy.bbcook.cn

[U36] Py：定时任务
来源：http://nfc.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://pad.tian-w.cn

[U37] Py：读写 Excel
来源：http://aqq.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nlw.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://wnm.cqqwz.cn

Path(__file__).resolve().parent
来源：http://cma.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://zfa.jinqigufen.top

sys.stdout.isatty()
来源：http://ocn.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://yum.ydzc1.top

print("err", file=sys.stderr)
来源：http://hyi.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://qtm.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://lmf.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://upq.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gbp.uphjek.com


<!-- 参考信息 -->