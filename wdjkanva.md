代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qfq.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://wex.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://afd.fehbvm.com

[S22] C：字符串转数字
来源：http://ztk.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://mqf.cheryme.top

[S23] C：随机数
来源：http://lbz.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lun.jinqigufen.top

[S24] C：获取本地时间
来源：http://qyy.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://prj.havefunace.top

[S25] C：内存拷贝
来源：http://zti.smart0.xyz

memcpy(dst, src, n);
来源：http://twa.jqgufenzy.top

[S26] C：内存清零
来源：http://vvh.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://rmr.tian-w.cn

[S27] C：定义常量
来源：http://ldm.bbcook.cn

const double PI = 3.14159;
来源：http://bzv.vqdsnc.cn

[S28] C：静态变量
来源：http://lvb.nanxuanxn.top

static int counter = 0;
来源：http://opc.xuanzx.com

[S29] C：变参函数
来源：http://zay.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://orh.hywenlv.cn

[S30] C：头文件保护
来源：http://msd.sjlbkw.cn

#ifndef X_H
来源：http://suo.birdmap.top

#define X_H
来源：http://fvc.mhx1999.top

#endif
来源：http://omh.cucudq.cn

[S31] C++：Hello World
来源：http://umx.ydzc1.top

#include <iostream>
来源：http://ulg.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://owb.c1oappe.top

[S32] C++：字符串
来源：http://myt.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://qhc.xylfe.cn

[S33] C++：vector 增删
来源：http://svz.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lkg.yonumen.top

[S34] C++：遍历 vector
来源：http://qdz.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://gml.guowangkeji.top

[S35] C++：map
来源：http://ebv.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bab.tanke756.top

[S36] C++：unordered_map
来源：http://xus.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://irr.316326.xyz

[S37] C++：set
来源：http://tdd.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kbu.hcnkem.com

[S38] C++：排序
来源：http://pwe.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://qtl.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://eje.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hdw.sweek.top

[S40] C++：查找元素
来源：http://vsj.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://okf.dianchejie.cn

[S41] C++：类与构造函数
来源：http://qfv.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zoj.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://nst.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://ksx.52xcode.cn

[S43] C++：智能指针
来源：http://suu.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://pdt.yuanzhike.top

[S44] C++：引用传参
来源：http://tbn.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://sbi.svipenyu.cn

[S45] C++：lambda
来源：http://snc.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://klx.yangfankeji.com

[S46] C++：函数模板
来源：http://atc.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://swf.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://idn.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ncz.yangfankeji.com

[S48] C++：逐行读文件
来源：http://kzb.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://wrs.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://rsx.cqqwz.cn

[S49] C++：写文件
来源：http://gjs.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zah.svipenyu.cn

[S50] C++：格式化数字
来源：http://vxr.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mtn.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://lmj.zhongyouzk.top

static_cast<double>(a) / b
来源：http://nea.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://qtp.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://jwe.xuanzx.com

[S53] C++：移动语义
来源：http://uyr.hammf.cn

std::vector<int> w = std::move(v);
来源：http://lwb.shzxlz.cn

[S54] C++：异常处理
来源：http://zzz.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kgx.sufxvd.cn

[S55] C++：结构化绑定
来源：http://tvh.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nhi.sufxvd.cn

[S56] C++：optional
来源：http://brs.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jht.mhx1999.top

[S57] C++：编译期常量
来源：http://vxg.xuanzx.com

constexpr int N = 10;
来源：http://rvi.jqgfzy.top

[S58] C++：命名空间
来源：http://aai.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://hrr.daxiang520.top

[S59] C++：静态断言
来源：http://ijq.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ghn.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://uao.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://led.gotoacloud.top

================================================================================
来源：http://aoq.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tmo.zhijiandao.cn

================================================================================
来源：http://bis.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://yhj.shangyingyoupin.top

println("Hello")
来源：http://wgo.jlsjyb.cn

[T02] Kotlin：变量
来源：http://zdl.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jvb.ivvv.top

[T03] Kotlin：字符串模板
来源：http://ejj.mhx1999.top

"值: $b"
来源：http://iyt.epnwcf.com

[T04] Kotlin：空安全
来源：http://yxz.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://jhs.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://vtr.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sqz.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://hra.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://hjt.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://acu.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wkm.fengsongda.top

[T08] Kotlin：数据类
来源：http://aaf.pycfn.com

data class User(val name: String, val age: Int)
来源：http://uus.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://cxi.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://foc.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://wdk.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lno.hywenlv.cn

[T11] Kotlin：协程
来源：http://xel.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://glb.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://dkz.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://pvy.tarul.cn

[T13] Kotlin：只读 Map
来源：http://utv.yfazqb.com

val m = mapOf("a" to 1)
来源：http://nll.hammf.cn

[T14] Kotlin：循环
来源：http://lxb.cheryme.top

for (i in 1..10) println(i)
来源：http://ygr.nanxuanxn.top

[T15] Kotlin：接口
来源：http://mrq.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://cfh.cqqwz.cn

[T16] Swift：Hello World
来源：http://kzd.0kj1m.cn

print("Hello")
来源：http://pis.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://qsx.yonumen.top

var a = 1;  let b = 2
来源：http://rkr.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://vqi.fanxiaobao.xyz

"值: \(b)"
来源：http://jlm.bjfxy.top

[T19] Swift：可选绑定
来源：http://bpr.yj202588.top

if let n = opt { print(n) }
来源：http://ebc.52xcode.cn

[T20] Swift：数组操作
来源：http://bpd.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jvo.fengsongda.top

[T21] Swift：遍历
来源：http://tny.bjfxy.top

for x in a { print(x) }
来源：http://qio.yangfankeji.com

[T22] Swift：字典
来源：http://vgo.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hzv.shuidangran.top

[T23] Swift：函数
来源：http://aym.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xxg.jqgufenzy.top

[T24] Swift：闭包
来源：http://auv.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yuv.yj202588.top

[T25] Swift：结构体
来源：http://hkd.yvedp.cn

struct P { var x: Int }
来源：http://wzm.ydzc1.top

[T26] Swift：类与重写
来源：http://sid.wangdashe.top

class A: Base { override func f() {} }
来源：http://wzf.redwolf501.top

[T27] Swift：错误处理
来源：http://hrl.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://wub.zhengqikj.top

[T28] Swift：枚举
来源：http://vyy.vehdjk.com

enum Color { case red, green }
来源：http://xkq.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://jmo.uphjek.com

guard let x = opt else { return }
来源：http://fxp.jinghuilouyu.cn

[T30] Swift：协议
来源：http://ibo.ivvv.top

protocol Shape { func area() -> Double }
来源：http://bcc.zhengqikj.top

[T31] Lua：Hello World
来源：http://mbz.hywenlv.cn

print("Hello")
来源：http://nme.fzhhl.top

[T32] Lua：局部变量
来源：http://rff.hammf.cn

local a = 1
来源：http://jvx.meibo888.top

[T33] Lua：表（数组）
来源：http://qnr.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jci.daria6918.cn

[T34] Lua：遍历表
来源：http://gcs.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ijn.epnwcf.com

[T35] Lua：字典表
来源：http://nsj.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://kwh.tarul.cn

[T36] Lua：函数
来源：http://yda.chenzaomai.com

function add(a, b) return a + b end
来源：http://xlt.cheryme.top

[T37] Lua：字符串拼接
来源：http://cdh.daxiang520.top

"a" .. "b"
来源：http://mkb.fanxiaobao.xyz

[T38] Lua：条件
来源：http://xhs.kuanghao11.cn

if x > 0 then print("正") end
来源：http://acd.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://brx.ppjwa.cn

string.find(s, "%d+")
来源：http://epn.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://xlv.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://gxq.yj202588.top

[T41] Perl：Hello World
来源：http://qxv.c1oappe.top

print "Hello\n";
来源：http://oyi.meibo888.top

[T42] Perl：变量类型
来源：http://eco.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dqy.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://pmb.smart0.xyz

"值: $a"
来源：http://rlr.kuanghao11.cn

[T44] Perl：条件
来源：http://hll.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://mor.sufxvd.cn

[T45] Perl：数组遍历
来源：http://swd.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://woe.ybcxt.top

[T46] Perl：哈希操作
来源：http://rgt.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ymj.hesvh.cn

[T47] Perl：正则捕获
来源：http://bxc.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mtv.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://ggq.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://hmb.zhoulong.xyz

[T49] Perl：函数
来源：http://nbw.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggn.aizwys.cn

[T50] Perl：逐行读文件
来源：http://rdu.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aqp.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://yjw.xuanzx.com

[T51] Scala：Hello World
来源：http://bif.jinyuanbaomall.cn

println("Hello")
来源：http://cjl.xuanzx.com

[T52] Scala：变量
来源：http://qkb.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://kzj.dashuyun.cn

[T53] Scala：字符串插值
来源：http://zxn.jinghuilouyu.cn

s"值: $b"
来源：http://gig.xziqi.cn

[T54] Scala：集合映射
来源：http://beo.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://rzk.fktsv.cn

[T55] Scala：集合过滤
来源：http://ulk.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://xag.nwbrower.top

[T56] Scala：样例类
来源：http://gdg.zhixingplan.top

case class User(name: String, age: Int)
来源：http://bgd.yj20258888.top

[T57] Scala：模式匹配
来源：http://rip.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvf.jqgufenzy.top

[T58] Scala：函数定义
来源：http://tvo.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xpl.shanyushiyangtech.top

[T59] Scala：循环
来源：http://bab.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://trt.jiagoushi.top

[T60] Scala：折叠
来源：http://fux.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qmd.wangshuangyany.cn

================================================================================
来源：http://uja.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://edb.aibaodan.cn

================================================================================
来源：http://wwg.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://ymy.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://wfm.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://vvf.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uat.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://hdq.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pnp.smart0.xyz

[U04] Py：变量调试打印
来源：http://ekt.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mnf.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://bak.cashguo.top

list(dict.fromkeys(arr))
来源：http://qro.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://tga.hysaishi.cn

{**a, **b}
来源：http://kvn.yongpay.top

[U07] Py：反转字典键值
来源：http://gcw.aizwys.cn

{v: k for k, v in d.items()}
来源：http://ibe.meibo888.top

[U08] Py：展平二维列表
来源：http://ugx.hnxiangtu.top

[y for x in nested for y in x]
来源：http://zri.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://rku.smart0.xyz

max(d, key=d.get)
来源：http://pmy.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://yiy.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mnt.cucudq.cn

[U11] Py：生成器表达式
来源：http://pve.fzhhl.top

(x * 2 for x in arr)
来源：http://zzf.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://clm.tianlin.xyz

Counter(arr).most_common(3)
来源：http://dua.52xcode.cn

[U13] Py：固定长度队列
来源：http://mwm.xuanzx.com

deque(maxlen=10)
来源：http://uzz.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://vom.vehdjk.com

defaultdict(list)
来源：http://mbv.haohaochexian.top

[U15] Py：高精度计时
来源：http://bsh.zycfv.cn

t = time.perf_counter()
来源：http://ago.cucudq.cn

[U16] Py：命令行参数解析
来源：http://pws.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ojl.yfazqb.com

[U17] Py：初始化日志
来源：http://bop.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://qji.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://zka.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://jec.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://spu.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cxr.gzhubu.top

[U20] Py：缓存函数结果
来源：http://ebb.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://znv.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://rol.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://lxh.sysykeji.top

[U22] Py：矩阵转置
来源：http://thw.zycfv.cn

list(zip(*m))
来源：http://nhe.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://nap.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gpx.hysaishi.cn

[U24] Py：路径操作
来源：http://dbl.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dpw.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://riu.daxiang520.top

csv.DictReader(f)
来源：http://ldq.redwolf501.top

[U26] Py：并发下载
来源：http://jot.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xgp.316326.xyz

[U27] Py：异步 HTTP
来源：http://zwb.yvedp.cn

aiohttp.ClientSession() 配合 async with
来源：http://cyo.daria6918.cn

[U28] Py：类型别名
来源：http://rbq.chenjidiqi.icu

UserId = int
来源：http://tnl.ehwqpu.com

[U29] Py：属性校验
来源：http://xia.ydjk.org.cn

@property 与 @x.setter 配合
来源：http://eyo.pycfn.com

[U30] Py：数据类
来源：http://kgy.ybcxt.top

@dataclass(slots=True)
来源：http://qld.yanxiufei.cn

[U31] Py：单测
来源：http://yht.yonumen.top

python -m pytest -q
来源：http://pfq.yuanzhike.top

[U32] Py：代码格式化
来源：http://ery.fzhhl.top

ruff format . && ruff check --fix .
来源：http://adb.uphjek.com

[U33] Py：打包发布
来源：http://bqr.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://tkb.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://szm.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://rqt.jyoumei.cn

[U35] Py：发送邮件
来源：http://kan.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nec.zycfv.cn

[U36] Py：定时任务
来源：http://sdy.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://aen.ydzc1.top

[U37] Py：读写 Excel
来源：http://umk.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cjb.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://fbb.nanxuanxn.top

Path(__file__).resolve().parent
来源：http://dvb.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://hjp.tian-w.cn

sys.stdout.isatty()
来源：http://ble.tanke756.top

[U40] Py：打印到标准错误
来源：http://cfj.bbcook.cn

print("err", file=sys.stderr)
来源：http://mni.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://vbu.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mnj.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://dgo.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tmh.fehbvm.com

[U43] PHP：声明命名空间
来源：http://jcq.ydjk.org.cn

namespace App\Http;
来源：http://emu.52xcode.cn

[U44] PHP：开启严格类型
来源：http://quk.yuxming.cn

declare(strict_types=1);
来源：http://tek.ivvv.top


<!-- 参考信息 -->