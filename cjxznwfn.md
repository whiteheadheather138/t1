代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://epr.sjlbkw.cn

[S21] C：字符类别判断
来源：http://rxn.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://osn.xylfe.cn

[S22] C：字符串转数字
来源：http://zse.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kgn.pycfn.com

[S23] C：随机数
来源：http://ykx.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ndi.hnqzz.top

[S24] C：获取本地时间
来源：http://btg.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tyl.316326.xyz

[S25] C：内存拷贝
来源：http://ctb.jqgufenzy.top

memcpy(dst, src, n);
来源：http://ucr.zycfv.cn

[S26] C：内存清零
来源：http://uby.tarul.cn

memset(a, 0, sizeof a);
来源：http://xag.zhixingplan.top

[S27] C：定义常量
来源：http://rpx.c1oappe.top

const double PI = 3.14159;
来源：http://kgr.feifeiyinyue.top

[S28] C：静态变量
来源：http://sdp.uphjek.com

static int counter = 0;
来源：http://mtq.shuidangran.top

[S29] C：变参函数
来源：http://fai.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jzc.ehwqpu.com

[S30] C：头文件保护
来源：http://nwe.fktsv.cn

#ifndef X_H
来源：http://bva.yanxiufei.cn

#define X_H
来源：http://rcy.yuanzhike.top

#endif
来源：http://fvw.zhoulong.xyz

[S31] C++：Hello World
来源：http://ieq.ppjwa.cn

#include <iostream>
来源：http://ytf.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://spg.jyoumei.cn

[S32] C++：字符串
来源：http://izm.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://ixx.jiagoushi.top

[S33] C++：vector 增删
来源：http://tfk.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qeu.fzhhl.top

[S34] C++：遍历 vector
来源：http://wyf.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://hdc.shzxlz.cn

[S35] C++：map
来源：http://wsm.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wzm.bbcook.cn

[S36] C++：unordered_map
来源：http://nvx.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gkk.fehbvm.com

[S37] C++：set
来源：http://zai.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tfr.cheryme.top

[S38] C++：排序
来源：http://bci.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://die.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://szy.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://igy.jyoumei.cn

[S40] C++：查找元素
来源：http://bcw.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://akn.vehdjk.com

[S41] C++：类与构造函数
来源：http://qtb.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xes.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://wkw.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://haj.cheryme.top

[S43] C++：智能指针
来源：http://ush.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://ewe.ivvv.top

[S44] C++：引用传参
来源：http://thp.xinyue.icu

void inc(int &x) { ++x; }
来源：http://pgy.ydjk.org.cn

[S45] C++：lambda
来源：http://gsa.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://tks.yongpay.top

[S46] C++：函数模板
来源：http://ren.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://avp.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://hyd.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tkr.sxryk.cn

[S48] C++：逐行读文件
来源：http://ucu.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://zyk.meibo888.top

while (std::getline(in, line)) { }
来源：http://mnr.smart0.xyz

[S49] C++：写文件
来源：http://bpe.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xsb.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://kfn.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iae.yonumen.top

[S51] C++：显式类型转换
来源：http://ygr.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://feb.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://miv.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://adx.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://aoa.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://bwj.hesvh.cn

[S54] C++：异常处理
来源：http://jkf.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jbz.fengsongda.top

[S55] C++：结构化绑定
来源：http://ksg.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://qja.yj20258.top

[S56] C++：optional
来源：http://bvq.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jvw.xziqi.cn

[S57] C++：编译期常量
来源：http://tht.pengpengdd.cyou

constexpr int N = 10;
来源：http://cko.hfpthk.cn

[S58] C++：命名空间
来源：http://ayw.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://rkj.svipenyu.cn

[S59] C++：静态断言
来源：http://tgo.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vuf.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://wlm.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vql.sweek.top

================================================================================
来源：http://mzi.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vxj.gogol.net.cn

================================================================================
来源：http://coz.wangdashe.top

[T01] Kotlin：Hello World
来源：http://tge.hywenlv.cn

println("Hello")
来源：http://eqo.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://miz.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sqq.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://dra.cashguo.top

"值: $b"
来源：http://zqm.yfazqb.com

[T04] Kotlin：空安全
来源：http://bfz.tanke756.top

val n: String? = null;  n?.length
来源：http://ghx.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://htt.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yqm.daxiang520.top

[T06] Kotlin：集合映射
来源：http://jpm.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://spd.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://xjr.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zqq.yueranfly.top

[T08] Kotlin：数据类
来源：http://wvx.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://jqb.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://dak.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://sbl.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://bgb.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jzl.52xcode.cn

[T11] Kotlin：协程
来源：http://qfn.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xma.iojbl.cn

[T12] Kotlin：解构声明
来源：http://nwj.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://ksp.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://xsi.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://pjm.gzhubu.top

[T14] Kotlin：循环
来源：http://bmq.tianlin.xyz

for (i in 1..10) println(i)
来源：http://kru.aizwys.cn

[T15] Kotlin：接口
来源：http://ylu.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://mcg.birdmap.top

[T16] Swift：Hello World
来源：http://igt.ehwqpu.com

print("Hello")
来源：http://sta.daxiang520.top

[T17] Swift：变量与常量
来源：http://fxw.vqdsnc.cn

var a = 1;  let b = 2
来源：http://ziu.meibo888.top

[T18] Swift：字符串插值
来源：http://drs.havefunace.top

"值: \(b)"
来源：http://rsy.fzhhl.top

[T19] Swift：可选绑定
来源：http://fkp.jianghu66.top

if let n = opt { print(n) }
来源：http://lcg.cucudq.cn

[T20] Swift：数组操作
来源：http://tmq.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://csa.yuxming.cn

[T21] Swift：遍历
来源：http://pab.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://ftu.mhx1999.top

[T22] Swift：字典
来源：http://mxm.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xej.ydjk.org.cn

[T23] Swift：函数
来源：http://wro.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dbp.feifeiyinyue.top

[T24] Swift：闭包
来源：http://smz.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qxn.kuanghao11.cn

[T25] Swift：结构体
来源：http://mqm.pengpengdd.cyou

struct P { var x: Int }
来源：http://leh.sjlbkw.cn

[T26] Swift：类与重写
来源：http://wdc.9152youxi.cn

class A: Base { override func f() {} }
来源：http://bir.zhengqikj.top

[T27] Swift：错误处理
来源：http://dat.c1oappe.top

do { try f() } catch { print(error) }
来源：http://tcu.0kj1m.cn

[T28] Swift：枚举
来源：http://dap.yfazqb.com

enum Color { case red, green }
来源：http://jyk.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://igd.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://vzq.snrcjt.cn

[T30] Swift：协议
来源：http://kkq.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://djs.shzxlz.cn

[T31] Lua：Hello World
来源：http://rca.gaohongyu789.top

print("Hello")
来源：http://pps.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://mmy.fanxiaobao.xyz

local a = 1
来源：http://dfh.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://nix.svipenyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cty.daxiang520.top

[T34] Lua：遍历表
来源：http://jxh.yvedp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ehq.jianghu66.top

[T35] Lua：字典表
来源：http://dwo.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://pqm.cucudq.cn

[T36] Lua：函数
来源：http://dfv.yvedp.cn

function add(a, b) return a + b end
来源：http://gfe.fktsv.cn

[T37] Lua：字符串拼接
来源：http://bzl.ppjwa.cn

"a" .. "b"
来源：http://slj.wangshuangyany.cn

[T38] Lua：条件
来源：http://ixz.dianchejie.cn

if x > 0 then print("正") end
来源：http://njx.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://yfc.tarul.cn

string.find(s, "%d+")
来源：http://ylq.ivvv.top

[T40] Lua：元表
来源：http://ecf.gzhubu.top

setmetatable({}, { __index = base })
来源：http://jyk.wangdashe.top

[T41] Perl：Hello World
来源：http://xse.jinqigufen.top

print "Hello\n";
来源：http://vgc.tarul.cn

[T42] Perl：变量类型
来源：http://lcx.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oio.c1oappe.top

[T43] Perl：字符串插值
来源：http://tli.aibaodan.cn

"值: $a"
来源：http://lcv.pycfn.com

[T44] Perl：条件
来源：http://czv.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://krp.yfazqb.com

[T45] Perl：数组遍历
来源：http://txx.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://flv.yj20258.top

[T46] Perl：哈希操作
来源：http://tan.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jkm.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://xsq.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cii.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://hwg.9152youxi.cn

$s =~ s/old/new/g;
来源：http://ecc.aibaodan.cn

[T49] Perl：函数
来源：http://vee.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fhz.xylfe.cn

[T50] Perl：逐行读文件
来源：http://hfq.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vas.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://bmb.guowangkeji.top

[T51] Scala：Hello World
来源：http://btl.yj20258888.top

println("Hello")
来源：http://mpv.haohaochexian.top

[T52] Scala：变量
来源：http://cjh.mhx1999.top

val a = 1;  var b = 2
来源：http://hnp.hesvh.cn

[T53] Scala：字符串插值
来源：http://qbx.zycfv.cn

s"值: $b"
来源：http://fmp.bjfxy.top

[T54] Scala：集合映射
来源：http://dlx.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://qvc.aizwys.cn

[T55] Scala：集合过滤
来源：http://fsf.guowangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://vdv.shuidangran.top

[T56] Scala：样例类
来源：http://vlu.cdnleiting.top

case class User(name: String, age: Int)
来源：http://izu.smart0.xyz

[T57] Scala：模式匹配
来源：http://eum.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xry.svipenyu.cn

[T58] Scala：函数定义
来源：http://uvi.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://sxc.hfpthk.cn

[T59] Scala：循环
来源：http://lte.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://wdh.ydjk.org.cn

[T60] Scala：折叠
来源：http://fwa.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kjo.tianlin.xyz

================================================================================
来源：http://ypw.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://prc.fktsv.cn

================================================================================
来源：http://dud.birdmap.top

[U01] Py：创建虚拟环境
来源：http://fxz.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://ykl.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://nfs.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://amm.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://fgd.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ffr.hywenlv.cn

[U04] Py：变量调试打印
来源：http://jmo.ywan-chungtsiang.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://opu.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://cng.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://wmt.dianchejie.cn

[U06] Py：合并两个字典
来源：http://ohz.yuanzhike.top

{**a, **b}
来源：http://bpf.pycfn.com

[U07] Py：反转字典键值
来源：http://zwv.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://ern.nanxinkj.top

[U08] Py：展平二维列表
来源：http://uuw.andypj.xyz

[y for x in nested for y in x]
来源：http://dpy.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://bvt.pycfn.com

max(d, key=d.get)
来源：http://uwd.bbcook.cn

[U10] Py：按值排序字典
来源：http://esj.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://alv.ywan-chungtsiang.top

[U11] Py：生成器表达式
来源：http://plt.mhx1999.top

(x * 2 for x in arr)
来源：http://gci.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://deh.havefunace.top

Counter(arr).most_common(3)
来源：http://ifv.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://vcf.yj20258.top

deque(maxlen=10)
来源：http://nkh.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://gce.yangfankeji.com

defaultdict(list)
来源：http://rcb.yangfankeji.com

[U15] Py：高精度计时
来源：http://eww.bjfxy.top

t = time.perf_counter()
来源：http://yox.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://oom.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tqx.cashguo.top

[U17] Py：初始化日志
来源：http://rse.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://apf.gogol.net.cn

[U18] Py：预编译正则
来源：http://xyd.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://qjn.cashguo.top

[U19] Py：正则替换带回调
来源：http://lgd.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mbf.xuanzx.com

[U20] Py：缓存函数结果
来源：http://rcp.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://dpc.ctjpmb.com

[U21] Py：自定义上下文管理器
来源：http://zoz.sxryk.cn

@contextlib.contextmanager
来源：http://klm.52xcode.cn

[U22] Py：矩阵转置
来源：http://nxo.yongpay.top

list(zip(*m))
来源：http://wpk.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://tzj.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lci.fzhhl.top

[U24] Py：路径操作
来源：http://krj.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xkd.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://dsj.gaohongyu789.top

csv.DictReader(f)
来源：http://chk.yj20258.top

[U26] Py：并发下载
来源：http://zhj.jinqigfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://stt.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://wjb.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://vsg.yj20258.top

[U28] Py：类型别名
来源：http://fxr.sysykeji.top

UserId = int
来源：http://qfr.sjlbkw.cn

[U29] Py：属性校验
来源：http://ehg.havefunace.top

@property 与 @x.setter 配合
来源：http://omg.fengsongda.top

[U30] Py：数据类
来源：http://jwp.zhengqikj.top

@dataclass(slots=True)
来源：http://ozl.ybcxt.top

[U31] Py：单测
来源：http://vyx.kuanghao11.cn

python -m pytest -q
来源：http://gwk.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://khg.dashuyun.cn

ruff format . && ruff check --fix .
来源：http://uew.tianlin.xyz

[U33] Py：打包发布
来源：http://jiw.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://pxx.cqqwz.cn

[U34] Py：判断编码
来源：http://cpr.ydzc1.top

chardet.detect(raw)
来源：http://lzk.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://img.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gbx.cashguo.top

[U36] Py：定时任务
来源：http://dxh.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://cjd.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://ixs.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://rwb.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://ghp.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://thi.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://kzu.zhongyouzk.top

sys.stdout.isatty()
来源：http://rgv.xuanzx.com

[U40] Py：打印到标准错误
来源：http://dby.xinyue.icu

print("err", file=sys.stderr)
来源：http://cby.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://yzi.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gtn.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://ixh.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://whl.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://aos.xuetiantiany.cn

namespace App\Http;
来源：http://vvh.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://bvh.birdmap.top

declare(strict_types=1);
来源：http://wjp.jianghu66.top


<!-- 参考信息 -->