代发 wailian999

x |= (1 << 3);
来源：http://asx.redwolf501.top

[S17] C：安全拼接字符串
来源：http://qkg.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fti.iojbl.cn

[S18] C：命令行参数
来源：http://oua.xziqi.cn

int main(int argc, char **argv)
来源：http://xwq.hfpthk.cn

[S19] C：快速排序
来源：http://cvp.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://edu.zdbjq.cn

[S20] C：二分查找
来源：http://stk.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://trr.yfazqb.com

[S21] C：字符类别判断
来源：http://tio.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bzp.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://yad.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://cxj.ydzc1.top

[S23] C：随机数
来源：http://hgn.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cjx.sweek.top

[S24] C：获取本地时间
来源：http://upz.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uon.cheryme.top

[S25] C：内存拷贝
来源：http://sxo.yj20258888.top

memcpy(dst, src, n);
来源：http://vvi.nanxuanxn.top

[S26] C：内存清零
来源：http://ycd.birdmap.top

memset(a, 0, sizeof a);
来源：http://reu.epnwcf.com

[S27] C：定义常量
来源：http://yxc.tianlin.xyz

const double PI = 3.14159;
来源：http://sdt.cucudq.cn

[S28] C：静态变量
来源：http://vzw.feifeiyinyue.top

static int counter = 0;
来源：http://jam.chenjidiqi.icu

[S29] C：变参函数
来源：http://fmk.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dfd.zhiwuduotai.top

[S30] C：头文件保护
来源：http://whq.cqqwz.cn

#ifndef X_H
来源：http://qlu.iojbl.cn

#define X_H
来源：http://gbp.ydjk.org.cn

#endif
来源：http://plb.haohaochexian.top

[S31] C++：Hello World
来源：http://msr.ywan-chungtsiang.top

#include <iostream>
来源：http://ypl.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://kwc.ybcxt.top

[S32] C++：字符串
来源：http://ryw.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://lqo.hywenlv.cn

[S33] C++：vector 增删
来源：http://skw.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jse.redwolf501.top

[S34] C++：遍历 vector
来源：http://odx.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://evx.feifeiyinyue.top

[S35] C++：map
来源：http://afo.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pxi.gogol.net.cn

[S36] C++：unordered_map
来源：http://qpq.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mhw.epnwcf.com

[S37] C++：set
来源：http://bqu.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wuj.dashuyun.cn

[S38] C++：排序
来源：http://lqd.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://ipm.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://aby.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbd.jinqigfzy.top

[S40] C++：查找元素
来源：http://mvh.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vme.hammf.cn

[S41] C++：类与构造函数
来源：http://epn.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lbp.gzhubu.top

[S42] C++：继承与虚函数
来源：http://pdc.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://fbu.yuanzhike.top

[S43] C++：智能指针
来源：http://feo.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://kaz.tian-w.cn

[S44] C++：引用传参
来源：http://cam.hesvh.cn

void inc(int &x) { ++x; }
来源：http://icj.bbcook.cn

[S45] C++：lambda
来源：http://gpp.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://zfl.shuidangran.top

[S46] C++：函数模板
来源：http://pgs.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://odp.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://wbk.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jlc.gotoacloud.top

[S48] C++：逐行读文件
来源：http://zbp.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ypo.meibo888.top

while (std::getline(in, line)) { }
来源：http://rpe.gzhubu.top

[S49] C++：写文件
来源：http://owm.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xbt.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://haf.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exr.vehdjk.com

[S51] C++：显式类型转换
来源：http://wvn.ydzc1.top

static_cast<double>(a) / b
来源：http://gzn.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://jds.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://xfh.meibo888.top

[S53] C++：移动语义
来源：http://jbj.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://aqd.nanxinkj.top

[S54] C++：异常处理
来源：http://mcs.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rvm.dianchejie.cn

[S55] C++：结构化绑定
来源：http://sbt.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://noh.mhx1999.top

[S56] C++：optional
来源：http://oor.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rhr.xinyue.icu

[S57] C++：编译期常量
来源：http://dbj.hesvh.cn

constexpr int N = 10;
来源：http://nym.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://cvc.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://htv.yvedp.cn

[S59] C++：静态断言
来源：http://vno.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qoo.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://pgi.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://enn.gzhubu.top

================================================================================
来源：http://pbi.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xfv.jqgufenzy.top

================================================================================
来源：http://myn.hnqzz.top

[T01] Kotlin：Hello World
来源：http://urc.yanxiufei.cn

println("Hello")
来源：http://cwx.mhx1999.top

[T02] Kotlin：变量
来源：http://bqk.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ura.shzxlz.cn

[T03] Kotlin：字符串模板
来源：http://udd.nwbrower.top

"值: $b"
来源：http://jep.wangdashe.top

[T04] Kotlin：空安全
来源：http://laf.hywenlv.cn

val n: String? = null;  n?.length
来源：http://lpp.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://xph.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xgh.yj20258888.top

[T06] Kotlin：集合映射
来源：http://qaj.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tby.uphjek.com

[T07] Kotlin：集合过滤
来源：http://nnk.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hmd.yfazqb.com

[T08] Kotlin：数据类
来源：http://pho.cashguo.top

data class User(val name: String, val age: Int)
来源：http://xqu.meibo888.top

[T09] Kotlin：扩展函数
来源：http://gpf.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://tza.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://uai.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uro.vqdsnc.cn

[T11] Kotlin：协程
来源：http://amz.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yfo.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://ywx.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://dqd.yj202588.top

[T13] Kotlin：只读 Map
来源：http://ycz.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://eyj.redwolf501.top

[T14] Kotlin：循环
来源：http://csy.bjfxy.top

for (i in 1..10) println(i)
来源：http://djx.ybcxt.top

[T15] Kotlin：接口
来源：http://qep.redwolf501.top

interface Shape { fun area(): Double }
来源：http://pws.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://clm.fengsongda.top

print("Hello")
来源：http://cnh.chenlongwang.top

[T17] Swift：变量与常量
来源：http://ttc.epnwcf.com

var a = 1;  let b = 2
来源：http://tjr.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://ota.fzhhl.top

"值: \(b)"
来源：http://jxh.yueranfly.top

[T19] Swift：可选绑定
来源：http://qqe.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://wow.dianchejie.cn

[T20] Swift：数组操作
来源：http://syq.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://gal.svipenyu.cn

[T21] Swift：遍历
来源：http://rwa.feifeiyinyue.top

for x in a { print(x) }
来源：http://sej.fktsv.cn

[T22] Swift：字典
来源：http://deh.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://xzq.yongpay.top

[T23] Swift：函数
来源：http://iye.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ygh.xziqi.cn

[T24] Swift：闭包
来源：http://iwg.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://evq.xylfe.cn

[T25] Swift：结构体
来源：http://upn.yfazqb.com

struct P { var x: Int }
来源：http://yni.yj202588.top

[T26] Swift：类与重写
来源：http://azk.bbcook.cn

class A: Base { override func f() {} }
来源：http://djq.snrcjt.cn

[T27] Swift：错误处理
来源：http://eop.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://jtg.gogol.net.cn

[T28] Swift：枚举
来源：http://knm.tarul.cn

enum Color { case red, green }
来源：http://rax.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://psf.quarkkingdee.top

guard let x = opt else { return }
来源：http://baa.zdqjudy.top

[T30] Swift：协议
来源：http://tid.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://dzm.meibo888.top

[T31] Lua：Hello World
来源：http://zsp.guowangkeji.top

print("Hello")
来源：http://erg.havefunace.top

[T32] Lua：局部变量
来源：http://aty.zdbjq.cn

local a = 1
来源：http://oea.fktsv.cn

[T33] Lua：表（数组）
来源：http://mwc.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://enh.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://iyp.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rzl.hfpthk.cn

[T35] Lua：字典表
来源：http://vsm.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://btd.yfazqb.com

[T36] Lua：函数
来源：http://tdk.shzxlz.cn

function add(a, b) return a + b end
来源：http://mub.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://qnf.cucudq.cn

"a" .. "b"
来源：http://rod.ppjwa.cn

[T38] Lua：条件
来源：http://cgu.9152youxi.cn

if x > 0 then print("正") end
来源：http://qsv.guowangkeji.top

[T39] Lua：模式匹配
来源：http://jwp.kuanghao11.cn

string.find(s, "%d+")
来源：http://skh.yfazqb.com

[T40] Lua：元表
来源：http://xhm.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://jjc.ybcxt.top

[T41] Perl：Hello World
来源：http://qly.uphjek.com

print "Hello\n";
来源：http://kdy.cqqwz.cn

[T42] Perl：变量类型
来源：http://iex.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ctb.snrcjt.cn

[T43] Perl：字符串插值
来源：http://udc.aizwys.cn

"值: $a"
来源：http://air.redwolf501.top

[T44] Perl：条件
来源：http://bxk.yj202588.top

if ($a > 0) { print "正"; }
来源：http://cez.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://smg.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://tzb.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://iny.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kfy.snrcjt.cn

[T47] Perl：正则捕获
来源：http://pac.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tdi.yangfankeji.com

[T48] Perl：正则替换
来源：http://nqc.yonumen.top

$s =~ s/old/new/g;
来源：http://fdr.xziqi.cn

[T49] Perl：函数
来源：http://gzz.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qud.bbcook.cn

[T50] Perl：逐行读文件
来源：http://dxy.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yqt.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://qca.hcnkem.com

[T51] Scala：Hello World
来源：http://kov.sweek.top

println("Hello")
来源：http://tvy.haohaochexian.top

[T52] Scala：变量
来源：http://lie.xinyue.icu

val a = 1;  var b = 2
来源：http://iha.dashuyun.cn

[T53] Scala：字符串插值
来源：http://itp.jlsjyb.cn

s"值: $b"
来源：http://khj.zhengqikj.top

[T54] Scala：集合映射
来源：http://hea.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://bbo.fengsongda.top

[T55] Scala：集合过滤
来源：http://xwc.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eoc.zhijiandao.cn

[T56] Scala：样例类
来源：http://jmc.iojbl.cn

case class User(name: String, age: Int)
来源：http://hmq.xinyue.icu

[T57] Scala：模式匹配
来源：http://gst.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gsv.jianghu66.top

[T58] Scala：函数定义
来源：http://ibi.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://upy.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://hox.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://qnm.guowangkeji.top

[T60] Scala：折叠
来源：http://qah.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bmm.ehwqpu.com

================================================================================
来源：http://vkh.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ydo.c1oappe.top

================================================================================
来源：http://hhw.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://fxk.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://iin.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://rdi.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zkp.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://ddw.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xdo.uphjek.com

[U04] Py：变量调试打印
来源：http://kqa.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://agu.uphjek.com

[U05] Py：列表去重且保序
来源：http://lkw.nwbrower.top

list(dict.fromkeys(arr))
来源：http://tts.yj20258888.top

[U06] Py：合并两个字典
来源：http://fig.ybcxt.top

{**a, **b}
来源：http://dbt.zhixingplan.top

[U07] Py：反转字典键值
来源：http://kfi.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://epz.fengsongda.top

[U08] Py：展平二维列表
来源：http://nkg.yj202588.top

[y for x in nested for y in x]
来源：http://fmq.birdmap.top

[U09] Py：字典取最大值的键
来源：http://psd.hnqzz.top

max(d, key=d.get)
来源：http://sfl.52xcode.cn

[U10] Py：按值排序字典
来源：http://bhv.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hmy.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://hpi.fengsongda.top

(x * 2 for x in arr)
来源：http://fki.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://jhi.ydzc1.top

Counter(arr).most_common(3)
来源：http://tud.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://uut.ppjwa.cn

deque(maxlen=10)
来源：http://zrd.havefunace.top

[U14] Py：分组收集到列表
来源：http://qok.jianghu66.top

defaultdict(list)
来源：http://fub.ydzc1.top

[U15] Py：高精度计时
来源：http://twh.ehwqpu.com

t = time.perf_counter()
来源：http://fsy.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://wzw.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ouu.guowangkeji.top

[U17] Py：初始化日志
来源：http://gvh.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://akr.gzhubu.top

[U18] Py：预编译正则
来源：http://gbw.shuidangran.top

pat = re.compile(r"\d+")
来源：http://szw.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://xxk.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bpv.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://ush.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://gkm.yueranfly.top

[U21] Py：自定义上下文管理器
来源：http://knp.yongpay.top

@contextlib.contextmanager
来源：http://htq.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://tqq.jqgfzy.top

list(zip(*m))
来源：http://vzs.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://dlv.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cka.chenlongwang.top

[U24] Py：路径操作
来源：http://ylp.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kgr.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://sen.kuanghao11.cn

csv.DictReader(f)
来源：http://cse.nanxinkj.top

[U26] Py：并发下载
来源：http://upk.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://alb.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://exb.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://nsn.zycfv.cn

[U28] Py：类型别名
来源：http://qpe.jinghuilouyu.cn

UserId = int
来源：http://deh.zhiwuduotai.top

[U29] Py：属性校验
来源：http://yle.svipenyu.cn

@property 与 @x.setter 配合
来源：http://acu.vqdsnc.cn

[U30] Py：数据类
来源：http://wil.gogol.net.cn

@dataclass(slots=True)
来源：http://kyq.smart0.xyz

[U31] Py：单测
来源：http://kxg.haohaochexian.top

python -m pytest -q
来源：http://krp.xylfe.cn

[U32] Py：代码格式化
来源：http://zqs.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://hpy.vehdjk.com

[U33] Py：打包发布
来源：http://cvj.ehwqpu.com

python -m build  （依赖 pyproject.toml）
来源：http://hdz.daria6918.cn

[U34] Py：判断编码
来源：http://yfy.jinqigfzy.top

chardet.detect(raw)
来源：http://xtp.sweek.top

[U35] Py：发送邮件
来源：http://lts.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oxz.hammf.cn

[U36] Py：定时任务
来源：http://ity.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://chd.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://ybg.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://rys.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://unh.sufxvd.cn

Path(__file__).resolve().parent
来源：http://lfz.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://mti.cucudq.cn

sys.stdout.isatty()
来源：http://fje.sxryk.cn

[U40] Py：打印到标准错误
来源：http://iyx.vehdjk.com

print("err", file=sys.stderr)
来源：http://mbf.yvedp.cn


<!-- 参考信息 -->