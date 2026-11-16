代发 wailian999

x |= (1 << 3);
来源：http://uzs.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://mcr.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://smy.cucudq.cn

[S18] C：命令行参数
来源：http://yrz.vehdjk.com

int main(int argc, char **argv)
来源：http://lwt.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://gze.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gab.yuxming.cn

[S20] C：二分查找
来源：http://fyx.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uch.guannengcc.top

[S21] C：字符类别判断
来源：http://egz.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ygv.yanxiufei.cn

[S22] C：字符串转数字
来源：http://vpe.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://wyk.yanxiufei.cn

[S23] C：随机数
来源：http://btk.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hla.sysykeji.top

[S24] C：获取本地时间
来源：http://apz.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lyc.snrcjt.cn

[S25] C：内存拷贝
来源：http://hny.yfazqb.com

memcpy(dst, src, n);
来源：http://faf.smart0.xyz

[S26] C：内存清零
来源：http://ars.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://noh.nanxinkj.top

[S27] C：定义常量
来源：http://tin.zycfv.cn

const double PI = 3.14159;
来源：http://hqq.yangfankeji.com

[S28] C：静态变量
来源：http://zdo.jiagoushi.top

static int counter = 0;
来源：http://jvy.0kj1m.cn

[S29] C：变参函数
来源：http://msz.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gzx.dianchejie.cn

[S30] C：头文件保护
来源：http://wdq.hfpthk.cn

#ifndef X_H
来源：http://frr.gogol.net.cn

#define X_H
来源：http://vux.tianlin.xyz

#endif
来源：http://vom.0kj1m.cn

[S31] C++：Hello World
来源：http://dhx.chenlongwang.top

#include <iostream>
来源：http://zls.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://eec.zdbjq.cn

[S32] C++：字符串
来源：http://qch.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://vny.yfazqb.com

[S33] C++：vector 增删
来源：http://djc.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ncp.sxryk.cn

[S34] C++：遍历 vector
来源：http://wjn.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://imq.yangfankeji.com

[S35] C++：map
来源：http://kqf.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://odr.yueranfly.top

[S36] C++：unordered_map
来源：http://wta.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ufs.birdmap.top

[S37] C++：set
来源：http://svf.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ios.xuanzx.com

[S38] C++：排序
来源：http://edc.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://hmj.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://ovs.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rba.zycfv.cn

[S40] C++：查找元素
来源：http://eub.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yqx.guowangkeji.top

[S41] C++：类与构造函数
来源：http://mfi.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uxy.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://mwo.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://vyz.havefunace.top

[S43] C++：智能指针
来源：http://fii.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://qhc.svipenyu.cn

[S44] C++：引用传参
来源：http://gva.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://epq.smart0.xyz

[S45] C++：lambda
来源：http://hsf.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nii.zdbjq.cn

[S46] C++：函数模板
来源：http://iws.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lpq.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://cqy.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xlx.jqgfzy.top

[S48] C++：逐行读文件
来源：http://toz.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tft.fengsongda.top

while (std::getline(in, line)) { }
来源：http://zjb.snrcjt.cn

[S49] C++：写文件
来源：http://qri.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ysp.vqdsnc.cn

[S50] C++：格式化数字
来源：http://cto.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://roa.yongpay.top

[S51] C++：显式类型转换
来源：http://qzt.fzhhl.top

static_cast<double>(a) / b
来源：http://pth.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://vyj.hnqzz.top

int size() const noexcept { return n_; }
来源：http://zly.ybcxt.top

[S53] C++：移动语义
来源：http://oio.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://hiz.nwbrower.top

[S54] C++：异常处理
来源：http://ocj.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ysz.cucudq.cn

[S55] C++：结构化绑定
来源：http://evq.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cph.kuanghao11.cn

[S56] C++：optional
来源：http://emr.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nmr.gaohongyu789.top

[S57] C++：编译期常量
来源：http://ndp.xuanzx.com

constexpr int N = 10;
来源：http://xxs.sufxvd.cn

[S58] C++：命名空间
来源：http://dml.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://sfk.hywenlv.cn

[S59] C++：静态断言
来源：http://qem.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://myp.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://djz.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wgk.yongpay.top

================================================================================
来源：http://nay.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://daz.hongshengwenyu.top

================================================================================
来源：http://ypc.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://cxe.yonumen.top

println("Hello")
来源：http://ind.yuanzhike.top

[T02] Kotlin：变量
来源：http://aeg.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lqf.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://wnq.yuanzhike.top

"值: $b"
来源：http://suf.ppjwa.cn

[T04] Kotlin：空安全
来源：http://xpg.hywenlv.cn

val n: String? = null;  n?.length
来源：http://xlh.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://ozo.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://shr.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://anq.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ovs.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://nsr.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://slo.gogol.net.cn

[T08] Kotlin：数据类
来源：http://mqi.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://mgm.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://jiz.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://zlc.shzxlz.cn

[T10] Kotlin：默认参数
来源：http://bji.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pta.yanxiufei.cn

[T11] Kotlin：协程
来源：http://wyd.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://wyo.uphjek.com

[T12] Kotlin：解构声明
来源：http://xjd.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://sne.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://nht.daria6918.cn

val m = mapOf("a" to 1)
来源：http://zmt.pycfn.com

[T14] Kotlin：循环
来源：http://jos.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://jmt.hfpthk.cn

[T15] Kotlin：接口
来源：http://idz.yuxming.cn

interface Shape { fun area(): Double }
来源：http://ten.jiagoushi.top

[T16] Swift：Hello World
来源：http://vki.cdnleiting.top

print("Hello")
来源：http://ors.daxiang520.top

[T17] Swift：变量与常量
来源：http://bjf.nanxinkj.top

var a = 1;  let b = 2
来源：http://ugt.pycfn.com

[T18] Swift：字符串插值
来源：http://csa.tianlin.xyz

"值: \(b)"
来源：http://max.yonumen.top

[T19] Swift：可选绑定
来源：http://njy.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://cyv.xinyue.icu

[T20] Swift：数组操作
来源：http://vgk.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://apm.xziqi.cn

[T21] Swift：遍历
来源：http://fgh.ivvv.top

for x in a { print(x) }
来源：http://yze.bjfxy.top

[T22] Swift：字典
来源：http://csy.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://xge.0kj1m.cn

[T23] Swift：函数
来源：http://cxb.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wxd.yangfankeji.com

[T24] Swift：闭包
来源：http://efn.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsr.316326.xyz

[T25] Swift：结构体
来源：http://gwx.yvedp.cn

struct P { var x: Int }
来源：http://acg.snrcjt.cn

[T26] Swift：类与重写
来源：http://gad.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://jzn.haohaochexian.top

[T27] Swift：错误处理
来源：http://vwr.fehbvm.com

do { try f() } catch { print(error) }
来源：http://egw.uphjek.com

[T28] Swift：枚举
来源：http://crx.0kj1m.cn

enum Color { case red, green }
来源：http://aet.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://pln.shuidangran.top

guard let x = opt else { return }
来源：http://hkm.havefunace.top

[T30] Swift：协议
来源：http://dsn.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://xve.0kj1m.cn

[T31] Lua：Hello World
来源：http://bur.xingfuxueyuan.xyz

print("Hello")
来源：http://xqn.zycfv.cn

[T32] Lua：局部变量
来源：http://ytf.yonumen.top

local a = 1
来源：http://hai.52xcode.cn

[T33] Lua：表（数组）
来源：http://kls.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://beo.chenlongwang.top

[T34] Lua：遍历表
来源：http://itj.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nxn.gotoacloud.top

[T35] Lua：字典表
来源：http://val.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://bub.vqdsnc.cn

[T36] Lua：函数
来源：http://mlz.quarkkingdee.top

function add(a, b) return a + b end
来源：http://gpy.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://kvc.yj20258888.top

"a" .. "b"
来源：http://nme.nanxuanxn.top

[T38] Lua：条件
来源：http://qcz.bjfxy.top

if x > 0 then print("正") end
来源：http://oqa.chenlongwang.top

[T39] Lua：模式匹配
来源：http://qcf.ppjwa.cn

string.find(s, "%d+")
来源：http://uqy.guowangkeji.top

[T40] Lua：元表
来源：http://zwa.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://oyd.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://gap.ydjk.org.cn

print "Hello\n";
来源：http://buj.zdqjudy.top

[T42] Perl：变量类型
来源：http://ytq.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zim.yfazqb.com

[T43] Perl：字符串插值
来源：http://xjd.sysykeji.top

"值: $a"
来源：http://dgv.shanyushiyangtech.top

[T44] Perl：条件
来源：http://pks.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://bsu.zdqjudy.top

[T45] Perl：数组遍历
来源：http://hmn.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://mio.yuanzhike.top

[T46] Perl：哈希操作
来源：http://idx.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://owa.yvedp.cn

[T47] Perl：正则捕获
来源：http://xjd.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vfx.fzhhl.top

[T48] Perl：正则替换
来源：http://pdd.sweek.top

$s =~ s/old/new/g;
来源：http://vrk.sysykeji.top

[T49] Perl：函数
来源：http://wrv.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kgk.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://zhr.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uad.meibo888.top

while (my $line = <$fh>) { print $line; }
来源：http://vca.316326.xyz

[T51] Scala：Hello World
来源：http://baw.tianlin.xyz

println("Hello")
来源：http://qlp.tianlin.xyz

[T52] Scala：变量
来源：http://rlq.pycfn.com

val a = 1;  var b = 2
来源：http://fex.gzhubu.top

[T53] Scala：字符串插值
来源：http://zpl.c1oappe.top

s"值: $b"
来源：http://nvt.jinqigfzy.top

[T54] Scala：集合映射
来源：http://hwn.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://bug.shuidangran.top

[T55] Scala：集合过滤
来源：http://zyr.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://gkb.yuxming.cn

[T56] Scala：样例类
来源：http://env.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://jsa.sxryk.cn

[T57] Scala：模式匹配
来源：http://fev.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nje.birdmap.top

[T58] Scala：函数定义
来源：http://oan.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://owx.svipenyu.cn

[T59] Scala：循环
来源：http://xia.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://qih.yj20258.top

[T60] Scala：折叠
来源：http://ttf.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xrz.feifeiyinyue.top

================================================================================
来源：http://cza.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://duu.hcnkem.com

================================================================================
来源：http://fmm.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://gqt.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xvu.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://vcj.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lry.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://hgx.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://odb.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://dlm.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jzr.fengsongda.top

[U05] Py：列表去重且保序
来源：http://ovz.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://nia.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://eyf.316326.xyz

{**a, **b}
来源：http://rqm.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://nbu.hesvh.cn

{v: k for k, v in d.items()}
来源：http://tvh.iojbl.cn

[U08] Py：展平二维列表
来源：http://hco.pycfn.com

[y for x in nested for y in x]
来源：http://ism.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://beh.yj20258.top

max(d, key=d.get)
来源：http://gny.tanke756.top

[U10] Py：按值排序字典
来源：http://fsk.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lxv.ctjpmb.com

[U11] Py：生成器表达式
来源：http://hou.cheryme.top

(x * 2 for x in arr)
来源：http://cox.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xrt.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://fqm.andypj.xyz

[U13] Py：固定长度队列
来源：http://evj.cheryme.top

deque(maxlen=10)
来源：http://ntw.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://egm.yj20258888.top

defaultdict(list)
来源：http://djz.yj20258888.top

[U15] Py：高精度计时
来源：http://awi.daria6918.cn

t = time.perf_counter()
来源：http://cev.xylfe.cn

[U16] Py：命令行参数解析
来源：http://qdn.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cov.tian-w.cn

[U17] Py：初始化日志
来源：http://iuk.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://twj.dashuyun.cn

[U18] Py：预编译正则
来源：http://fyk.daxiang520.top

pat = re.compile(r"\d+")
来源：http://wha.xinyue.icu

[U19] Py：正则替换带回调
来源：http://ney.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://epm.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://wte.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://neg.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://xui.jinqigufen.top

@contextlib.contextmanager
来源：http://pon.fengsongda.top

[U22] Py：矩阵转置
来源：http://rwt.jianghu66.top

list(zip(*m))
来源：http://uxh.hesvh.cn

[U23] Py：分块读取大文件
来源：http://hhc.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qwe.yj20258888.top

[U24] Py：路径操作
来源：http://lku.fengsongda.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sto.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://ykk.bjfxy.top

csv.DictReader(f)
来源：http://kgl.guannengcc.top

[U26] Py：并发下载
来源：http://zgz.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://quq.fehbvm.com

[U27] Py：异步 HTTP
来源：http://zxt.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://poh.zhiwuduotai.top

[U28] Py：类型别名
来源：http://rwa.ydzc1.top

UserId = int
来源：http://dge.yj202588.top

[U29] Py：属性校验
来源：http://jle.uphjek.com

@property 与 @x.setter 配合
来源：http://qru.chenzaomai.com

[U30] Py：数据类
来源：http://cfu.yanxiufei.cn

@dataclass(slots=True)
来源：http://vki.zhengqikj.top

[U31] Py：单测
来源：http://ayc.yueranfly.top

python -m pytest -q
来源：http://vyt.aizwys.cn

[U32] Py：代码格式化
来源：http://wxh.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://lkz.dianchejie.cn

[U33] Py：打包发布
来源：http://ziw.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://ggd.zhengqikj.top

[U34] Py：判断编码
来源：http://lfr.hongshengwenyu.top

chardet.detect(raw)
来源：http://gap.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://ldo.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cun.meibo888.top

[U36] Py：定时任务
来源：http://jhp.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://enr.shzxlz.cn

[U37] Py：读写 Excel
来源：http://ncv.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jrb.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://bqp.yuanzhike.top

Path(__file__).resolve().parent
来源：http://leo.shuidangran.top

[U39] Py：判断是否在交互环境
来源：http://mcf.havefunace.top

sys.stdout.isatty()
来源：http://arl.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://bur.zhixingplan.top

print("err", file=sys.stderr)
来源：http://imk.zhongyouzk.top


<!-- 参考信息 -->