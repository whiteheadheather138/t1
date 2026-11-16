代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://kgq.cashguo.top

[S15] C：类型转换
来源：http://kvn.xuanzx.com

(double) a / b
来源：http://ers.quarkkingdee.top

[S16] C：位操作置位
来源：http://hjh.quarkkingdee.top

x |= (1 << 3);
来源：http://qbi.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://nnl.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zxt.fzhhl.top

[S18] C：命令行参数
来源：http://zqg.sysykeji.top

int main(int argc, char **argv)
来源：http://mow.yongpay.top

[S19] C：快速排序
来源：http://jwj.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://wxz.jqgfzy.top

[S20] C：二分查找
来源：http://gqg.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xur.bbcook.cn

[S21] C：字符类别判断
来源：http://mhi.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://brx.yuxming.cn

[S22] C：字符串转数字
来源：http://gbr.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://zdj.ctjpmb.com

[S23] C：随机数
来源：http://wqb.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zqh.wangdashe.top

[S24] C：获取本地时间
来源：http://rjh.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nvf.sjlbkw.cn

[S25] C：内存拷贝
来源：http://kjp.sjlbkw.cn

memcpy(dst, src, n);
来源：http://wao.zdqjudy.top

[S26] C：内存清零
来源：http://kip.fengsongda.top

memset(a, 0, sizeof a);
来源：http://mjq.nwbrower.top

[S27] C：定义常量
来源：http://gvi.yonumen.top

const double PI = 3.14159;
来源：http://wdd.yonumen.top

[S28] C：静态变量
来源：http://drg.zhengqikj.top

static int counter = 0;
来源：http://exo.zhengqikj.top

[S29] C：变参函数
来源：http://pki.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nkp.kuanghao11.cn

[S30] C：头文件保护
来源：http://huh.hywenlv.cn

#ifndef X_H
来源：http://ssa.yonumen.top

#define X_H
来源：http://kkq.hammf.cn

#endif
来源：http://jgp.fengsongda.top

[S31] C++：Hello World
来源：http://bcj.jyoumei.cn

#include <iostream>
来源：http://eoe.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://lng.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://ujo.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://rcu.yangfankeji.com

[S33] C++：vector 增删
来源：http://tas.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://orm.tanke756.top

[S34] C++：遍历 vector
来源：http://exb.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://nvc.yueranfly.top

[S35] C++：map
来源：http://nvb.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eyx.birdmap.top

[S36] C++：unordered_map
来源：http://utq.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pbk.xuetiantiany.cn

[S37] C++：set
来源：http://cys.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://suj.chenjidiqi.icu

[S38] C++：排序
来源：http://yjo.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://pij.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://smi.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tud.hywenlv.cn

[S40] C++：查找元素
来源：http://hci.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jun.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://hpc.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://roz.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://ncg.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://sgy.smart0.xyz

[S43] C++：智能指针
来源：http://rxb.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://zwm.yanxiufei.cn

[S44] C++：引用传参
来源：http://liv.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://ump.shuidangran.top

[S45] C++：lambda
来源：http://poq.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gtc.yj20258.top

[S46] C++：函数模板
来源：http://qtb.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lrg.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://jsa.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fih.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://obl.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://xal.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://nzl.jianghu66.top

[S49] C++：写文件
来源：http://mua.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avr.nanxuanxn.top

[S50] C++：格式化数字
来源：http://fnd.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cmn.yonumen.top

[S51] C++：显式类型转换
来源：http://nwk.quarkkingdee.top

static_cast<double>(a) / b
来源：http://jhn.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://pid.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://cbh.gogol.net.cn

[S53] C++：移动语义
来源：http://yxi.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://now.jinqigfzy.top

[S54] C++：异常处理
来源：http://qmo.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gfx.chenzaomai.com

[S55] C++：结构化绑定
来源：http://hal.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://sxk.jyoumei.cn

[S56] C++：optional
来源：http://xoq.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pxj.yongpay.top

[S57] C++：编译期常量
来源：http://wdy.yj20258888.top

constexpr int N = 10;
来源：http://axo.jqgfzy.top

[S58] C++：命名空间
来源：http://bky.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://xge.yj20258888.top

[S59] C++：静态断言
来源：http://dtf.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qid.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://ssk.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ncq.sweek.top

================================================================================
来源：http://qpa.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywd.yfazqb.com

================================================================================
来源：http://bwn.yj202588.top

[T01] Kotlin：Hello World
来源：http://owe.gaohongyu789.top

println("Hello")
来源：http://dlf.sjlbkw.cn

[T02] Kotlin：变量
来源：http://pfv.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ape.hammf.cn

[T03] Kotlin：字符串模板
来源：http://kxb.tianlin.xyz

"值: $b"
来源：http://zjq.gotoacloud.top

[T04] Kotlin：空安全
来源：http://rnn.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://zhi.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://ham.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://unw.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://pjp.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://foy.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://lys.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qcy.tarul.cn

[T08] Kotlin：数据类
来源：http://swx.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://nnr.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://xod.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://tjg.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://amq.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dne.9152youxi.cn

[T11] Kotlin：协程
来源：http://rrt.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vnc.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://nzb.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://uom.hesvh.cn

[T13] Kotlin：只读 Map
来源：http://jti.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://ksc.uphjek.com

[T14] Kotlin：循环
来源：http://slw.zhixingplan.top

for (i in 1..10) println(i)
来源：http://dwo.yongpay.top

[T15] Kotlin：接口
来源：http://btc.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://nqw.zdqjudy.top

[T16] Swift：Hello World
来源：http://hrl.smart0.xyz

print("Hello")
来源：http://mbq.ehwqpu.com

[T17] Swift：变量与常量
来源：http://dfz.cashguo.top

var a = 1;  let b = 2
来源：http://ywl.ctjpmb.com

[T18] Swift：字符串插值
来源：http://tpr.xziqi.cn

"值: \(b)"
来源：http://ims.yangfankeji.com

[T19] Swift：可选绑定
来源：http://kth.iojbl.cn

if let n = opt { print(n) }
来源：http://jok.zhixingplan.top

[T20] Swift：数组操作
来源：http://cwz.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://osx.ppjwa.cn

[T21] Swift：遍历
来源：http://vzk.zhongyouzk.top

for x in a { print(x) }
来源：http://bqf.uphjek.com

[T22] Swift：字典
来源：http://rwk.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://edx.tarul.cn

[T23] Swift：函数
来源：http://fcu.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ags.yangfankeji.com

[T24] Swift：闭包
来源：http://uls.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://tca.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://hlj.wangshuangyany.cn

struct P { var x: Int }
来源：http://nlt.hammf.cn

[T26] Swift：类与重写
来源：http://lhe.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://mgq.yvedp.cn

[T27] Swift：错误处理
来源：http://yiq.yuxming.cn

do { try f() } catch { print(error) }
来源：http://hwo.ppjwa.cn

[T28] Swift：枚举
来源：http://olz.daxiang520.top

enum Color { case red, green }
来源：http://zps.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://hoy.zdqjudy.top

guard let x = opt else { return }
来源：http://fxi.ppjwa.cn

[T30] Swift：协议
来源：http://grw.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://oik.dashuyun.cn

[T31] Lua：Hello World
来源：http://due.chenzaomai.com

print("Hello")
来源：http://qnw.uphjek.com

[T32] Lua：局部变量
来源：http://taq.cucudq.cn

local a = 1
来源：http://xjj.shuidangran.top

[T33] Lua：表（数组）
来源：http://otw.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hvz.bbcook.cn

[T34] Lua：遍历表
来源：http://sbw.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bxz.chenzaomai.com

[T35] Lua：字典表
来源：http://mrn.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://gba.redwolf501.top

[T36] Lua：函数
来源：http://lbn.hywenlv.cn

function add(a, b) return a + b end
来源：http://jms.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://olo.bbcook.cn

"a" .. "b"
来源：http://pfg.zhijiandao.cn

[T38] Lua：条件
来源：http://fwx.pycfn.com

if x > 0 then print("正") end
来源：http://sde.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://qtl.bjfxy.top

string.find(s, "%d+")
来源：http://gkm.ybcxt.top

[T40] Lua：元表
来源：http://sce.mhx1999.top

setmetatable({}, { __index = base })
来源：http://mfc.smart0.xyz

[T41] Perl：Hello World
来源：http://bld.yangfankeji.com

print "Hello\n";
来源：http://iso.gogol.net.cn

[T42] Perl：变量类型
来源：http://gjy.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zvh.sufxvd.cn

[T43] Perl：字符串插值
来源：http://zfr.fktsv.cn

"值: $a"
来源：http://zux.bjfxy.top

[T44] Perl：条件
来源：http://amx.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://lbp.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://qug.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://gvo.tianlin.xyz

[T46] Perl：哈希操作
来源：http://xjw.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vld.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://brm.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jib.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://zpg.guowangkeji.top

$s =~ s/old/new/g;
来源：http://fid.jqgfzy.top

[T49] Perl：函数
来源：http://tdl.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dyq.birdmap.top

[T50] Perl：逐行读文件
来源：http://cot.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uvj.gzhubu.top

while (my $line = <$fh>) { print $line; }
来源：http://fvh.guannengcc.top

[T51] Scala：Hello World
来源：http://ogz.nanxuanxn.top

println("Hello")
来源：http://tfl.tanke756.top

[T52] Scala：变量
来源：http://qch.havefunace.top

val a = 1;  var b = 2
来源：http://lls.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://gat.gotoacloud.top

s"值: $b"
来源：http://bif.hywenlv.cn

[T54] Scala：集合映射
来源：http://rxu.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://law.yuxming.cn

[T55] Scala：集合过滤
来源：http://dfm.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cra.guowangkeji.top

[T56] Scala：样例类
来源：http://ibp.ppjwa.cn

case class User(name: String, age: Int)
来源：http://aij.cheryme.top

[T57] Scala：模式匹配
来源：http://cvm.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bbc.0kj1m.cn

[T58] Scala：函数定义
来源：http://hlx.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://kbm.yangfankeji.com

[T59] Scala：循环
来源：http://cav.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://sdr.mhx1999.top

[T60] Scala：折叠
来源：http://zym.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://idg.dianchejie.cn

================================================================================
来源：http://ipv.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fyo.kuanghao11.cn

================================================================================
来源：http://eax.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://wjs.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://ydz.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://iju.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://chk.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://zek.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://oit.haohaochexian.top

[U04] Py：变量调试打印
来源：http://blm.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lfv.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://zpm.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://sjs.dianchejie.cn

[U06] Py：合并两个字典
来源：http://rgj.316326.xyz

{**a, **b}
来源：http://iae.jinqigufen.top

[U07] Py：反转字典键值
来源：http://uqb.vehdjk.com

{v: k for k, v in d.items()}
来源：http://dfx.yongpay.top

[U08] Py：展平二维列表
来源：http://ydv.ydzc1.top

[y for x in nested for y in x]
来源：http://hkd.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://nee.dashuyun.cn

max(d, key=d.get)
来源：http://nzv.vehdjk.com

[U10] Py：按值排序字典
来源：http://vpd.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hdg.xuanzx.com

[U11] Py：生成器表达式
来源：http://asw.ehwqpu.com

(x * 2 for x in arr)
来源：http://quz.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qyc.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://asr.cashguo.top

[U13] Py：固定长度队列
来源：http://mgv.cqqwz.cn

deque(maxlen=10)
来源：http://slo.yfazqb.com

[U14] Py：分组收集到列表
来源：http://nmx.ctjpmb.com

defaultdict(list)
来源：http://hud.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://wlz.zhengqikj.top

t = time.perf_counter()
来源：http://tep.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://lel.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zwo.shuidangran.top

[U17] Py：初始化日志
来源：http://iqr.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://fvo.hnqzz.top

[U18] Py：预编译正则
来源：http://pwi.bjfxy.top

pat = re.compile(r"\d+")
来源：http://cad.daria6918.cn

[U19] Py：正则替换带回调
来源：http://jtl.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://svo.xylfe.cn

[U20] Py：缓存函数结果
来源：http://oye.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://bms.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://wev.fzhhl.top

@contextlib.contextmanager
来源：http://jkz.shzxlz.cn

[U22] Py：矩阵转置
来源：http://zel.jinghuilouyu.cn

list(zip(*m))
来源：http://fgi.52xcode.cn

[U23] Py：分块读取大文件
来源：http://ggh.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gyt.quarkkingdee.top

[U24] Py：路径操作
来源：http://smu.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lkd.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://rjv.zhixingplan.top

csv.DictReader(f)
来源：http://yzm.yj202588.top

[U26] Py：并发下载
来源：http://hdb.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oej.redwolf501.top

[U27] Py：异步 HTTP
来源：http://trd.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://vny.hywenlv.cn

[U28] Py：类型别名
来源：http://doy.jinqigufen.top

UserId = int
来源：http://vnl.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://qht.xziqi.cn

@property 与 @x.setter 配合
来源：http://rcd.sysykeji.top

[U30] Py：数据类
来源：http://sll.hongshengwenyu.top

@dataclass(slots=True)
来源：http://gpx.zhengqikj.top

[U31] Py：单测
来源：http://tix.zhongyouzk.top

python -m pytest -q
来源：http://ogm.yuanzhike.top

[U32] Py：代码格式化
来源：http://vza.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://fmt.jlsjyb.cn

[U33] Py：打包发布
来源：http://ytc.jinqigfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://qrt.52xcode.cn

[U34] Py：判断编码
来源：http://gxq.gzhubu.top

chardet.detect(raw)
来源：http://xkn.xuanzx.com

[U35] Py：发送邮件
来源：http://ipi.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bgl.fktsv.cn

[U36] Py：定时任务
来源：http://jst.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://mdh.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://zom.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://ttq.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://utq.tianlin.xyz

Path(__file__).resolve().parent
来源：http://drb.uphjek.com


<!-- 参考信息 -->