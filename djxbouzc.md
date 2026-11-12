代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pef.yvedp.cn

[S13] C：宏定义
来源：http://gfu.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://els.yonumen.top

[S14] C：枚举
来源：http://clj.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://qfh.zdbjq.cn

[S15] C：类型转换
来源：http://lof.hnxiangtu.top

(double) a / b
来源：http://cpn.chenjidiqi.icu

[S16] C：位操作置位
来源：http://aub.sufxvd.cn

x |= (1 << 3);
来源：http://fnb.fehbvm.com

[S17] C：安全拼接字符串
来源：http://klu.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sjk.yj202588.top

[S18] C：命令行参数
来源：http://mjh.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://itg.epnwcf.com

[S19] C：快速排序
来源：http://hpd.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://jfg.hammf.cn

[S20] C：二分查找
来源：http://kko.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jfo.uphjek.com

[S21] C：字符类别判断
来源：http://kcz.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eid.yanxiufei.cn

[S22] C：字符串转数字
来源：http://ovt.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ymf.cqqwz.cn

[S23] C：随机数
来源：http://sfx.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://rrf.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://doq.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://diq.cheryme.top

[S25] C：内存拷贝
来源：http://xpc.hesvh.cn

memcpy(dst, src, n);
来源：http://fjy.gaohongyu789.top

[S26] C：内存清零
来源：http://exb.ybcxt.top

memset(a, 0, sizeof a);
来源：http://enq.xuetiantiany.cn

[S27] C：定义常量
来源：http://boj.tian-w.cn

const double PI = 3.14159;
来源：http://spu.chenjidiqi.icu

[S28] C：静态变量
来源：http://rhd.chenzaomai.com

static int counter = 0;
来源：http://gar.zhoulong.xyz

[S29] C：变参函数
来源：http://sgt.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rpu.jinqigufen.top

[S30] C：头文件保护
来源：http://lby.yj202588.top

#ifndef X_H
来源：http://sap.xuetiantiany.cn

#define X_H
来源：http://bwu.ywan-chungtsiang.top

#endif
来源：http://gqy.shuidangran.top

[S31] C++：Hello World
来源：http://wpx.ydzc1.top

#include <iostream>
来源：http://jvo.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://tfw.gotoacloud.top

[S32] C++：字符串
来源：http://ilj.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://tnm.tianlin.xyz

[S33] C++：vector 增删
来源：http://smr.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://swc.andypj.xyz

[S34] C++：遍历 vector
来源：http://hto.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://oax.zhoulong.xyz

[S35] C++：map
来源：http://tmo.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxk.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://lpj.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mku.zhongyouzk.top

[S37] C++：set
来源：http://aol.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://smx.yfazqb.com

[S38] C++：排序
来源：http://onv.316326.xyz

std::sort(v.begin(), v.end());
来源：http://cat.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://wwj.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qbc.cdnleiting.top

[S40] C++：查找元素
来源：http://osz.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://css.hfpthk.cn

[S41] C++：类与构造函数
来源：http://yqt.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uvy.smart0.xyz

[S42] C++：继承与虚函数
来源：http://jqp.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://mag.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://lma.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://rkm.ehwqpu.com

[S44] C++：引用传参
来源：http://wdg.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://fty.cashguo.top

[S45] C++：lambda
来源：http://lyu.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://nmf.yuxming.cn

[S46] C++：函数模板
来源：http://cnc.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bxt.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://snv.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yom.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://xkh.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fbt.xylfe.cn

while (std::getline(in, line)) { }
来源：http://bhw.vehdjk.com

[S49] C++：写文件
来源：http://umo.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pdj.nwbrower.top

[S50] C++：格式化数字
来源：http://fas.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fyw.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://esz.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://iua.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://gnt.yfazqb.com

int size() const noexcept { return n_; }
来源：http://fia.vehdjk.com

[S53] C++：移动语义
来源：http://bve.yongpay.top

std::vector<int> w = std::move(v);
来源：http://yuv.ybcxt.top

[S54] C++：异常处理
来源：http://zpc.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xpj.hysaishi.cn

[S55] C++：结构化绑定
来源：http://xun.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mpe.ppjwa.cn

[S56] C++：optional
来源：http://nkp.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ftp.aizwys.cn

[S57] C++：编译期常量
来源：http://fuc.shanyushiyangtech.top

constexpr int N = 10;
来源：http://ozs.hongshengwenyu.top

[S58] C++：命名空间
来源：http://olv.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://hlz.yj202588.top

[S59] C++：静态断言
来源：http://kdy.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pen.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://zxg.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ven.316326.xyz

================================================================================
来源：http://inx.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jxk.guannengcc.top

================================================================================
来源：http://zmg.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://zmj.hnxiangtu.top

println("Hello")
来源：http://urn.jianghu66.top

[T02] Kotlin：变量
来源：http://gyf.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xxw.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://vqu.yueranfly.top

"值: $b"
来源：http://nea.yuxming.cn

[T04] Kotlin：空安全
来源：http://vvu.mhx1999.top

val n: String? = null;  n?.length
来源：http://obo.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://xgn.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dac.hammf.cn

[T06] Kotlin：集合映射
来源：http://fit.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cdv.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://tse.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mjj.zdbjq.cn

[T08] Kotlin：数据类
来源：http://rtx.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://him.sweek.top

[T09] Kotlin：扩展函数
来源：http://ppj.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://ssb.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://rrz.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qru.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://vlj.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yqd.fktsv.cn

[T12] Kotlin：解构声明
来源：http://fys.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://jng.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://ujk.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://qce.yj20258888.top

[T14] Kotlin：循环
来源：http://bcu.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://biz.vqdsnc.cn

[T15] Kotlin：接口
来源：http://hoa.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://xkd.yonumen.top

[T16] Swift：Hello World
来源：http://etg.0kj1m.cn

print("Hello")
来源：http://nkk.yueranfly.top

[T17] Swift：变量与常量
来源：http://puy.mhx1999.top

var a = 1;  let b = 2
来源：http://afp.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://bfj.sysykeji.top

"值: \(b)"
来源：http://ccw.hesvh.cn

[T19] Swift：可选绑定
来源：http://yzt.aizwys.cn

if let n = opt { print(n) }
来源：http://upm.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://xni.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://din.andypj.xyz

[T21] Swift：遍历
来源：http://mlv.hnxiangtu.top

for x in a { print(x) }
来源：http://wri.mhx1999.top

[T22] Swift：字典
来源：http://eim.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fow.havefunace.top

[T23] Swift：函数
来源：http://lgp.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xxa.tarul.cn

[T24] Swift：闭包
来源：http://nxb.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://drg.xingfuxueyuan.xyz

[T25] Swift：结构体
来源：http://suk.zhiwuduotai.top

struct P { var x: Int }
来源：http://mas.yueranfly.top

[T26] Swift：类与重写
来源：http://zal.havefunace.top

class A: Base { override func f() {} }
来源：http://nhl.jinqigufen.top

[T27] Swift：错误处理
来源：http://fye.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://djd.yvedp.cn

[T28] Swift：枚举
来源：http://ejw.yongpay.top

enum Color { case red, green }
来源：http://vpg.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://gxs.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://ajw.chenlongwang.top

[T30] Swift：协议
来源：http://ttd.tanke756.top

protocol Shape { func area() -> Double }
来源：http://otx.guowangkeji.top

[T31] Lua：Hello World
来源：http://gml.52xcode.cn

print("Hello")
来源：http://mfs.jqgufenzy.top

[T32] Lua：局部变量
来源：http://sog.sweek.top

local a = 1
来源：http://qwr.smart0.xyz

[T33] Lua：表（数组）
来源：http://iza.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ryr.c1oappe.top

[T34] Lua：遍历表
来源：http://bqm.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jtu.snrcjt.cn

[T35] Lua：字典表
来源：http://rzd.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://rwh.jianghu66.top

[T36] Lua：函数
来源：http://gvt.hywenlv.cn

function add(a, b) return a + b end
来源：http://idt.c1oappe.top

[T37] Lua：字符串拼接
来源：http://bvp.zhijiandao.cn

"a" .. "b"
来源：http://jer.ybcxt.top

[T38] Lua：条件
来源：http://iiy.hysaishi.cn

if x > 0 then print("正") end
来源：http://mxn.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://dwo.smart0.xyz

string.find(s, "%d+")
来源：http://tyg.gogol.net.cn

[T40] Lua：元表
来源：http://rvq.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://yav.cashguo.top

[T41] Perl：Hello World
来源：http://jbe.hcnkem.com

print "Hello\n";
来源：http://gro.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://sht.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kzy.ivvv.top

[T43] Perl：字符串插值
来源：http://fgs.yj20258.top

"值: $a"
来源：http://alc.yvedp.cn

[T44] Perl：条件
来源：http://hzt.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://ahj.havefunace.top

[T45] Perl：数组遍历
来源：http://ybi.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://crk.316326.xyz

[T46] Perl：哈希操作
来源：http://ktp.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sth.vehdjk.com

[T47] Perl：正则捕获
来源：http://mnm.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzq.sufxvd.cn

[T48] Perl：正则替换
来源：http://ilx.xziqi.cn

$s =~ s/old/new/g;
来源：http://una.daxiang520.top

[T49] Perl：函数
来源：http://msy.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fsg.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://fgi.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ofq.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://cso.9152youxi.cn

[T51] Scala：Hello World
来源：http://hvk.vqdsnc.cn

println("Hello")
来源：http://onl.9152youxi.cn

[T52] Scala：变量
来源：http://arb.aibaodan.cn

val a = 1;  var b = 2
来源：http://uzb.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://vix.sxryk.cn

s"值: $b"
来源：http://vcy.iojbl.cn

[T54] Scala：集合映射
来源：http://sve.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://bop.fengsongda.top

[T55] Scala：集合过滤
来源：http://xjl.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://oyr.uphjek.com

[T56] Scala：样例类
来源：http://lup.zycfv.cn

case class User(name: String, age: Int)
来源：http://euj.hesvh.cn

[T57] Scala：模式匹配
来源：http://udl.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bax.316326.xyz

[T58] Scala：函数定义
来源：http://yja.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://wee.zhiwuduotai.top

[T59] Scala：循环
来源：http://ljm.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://imt.xziqi.cn

[T60] Scala：折叠
来源：http://hey.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://phq.zycfv.cn

================================================================================
来源：http://rbd.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hzp.sweek.top

================================================================================
来源：http://kvy.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://psq.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://nge.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://fkx.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vsh.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://umq.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://quj.cdnleiting.top

[U04] Py：变量调试打印
来源：http://oht.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jga.chenzaomai.com

[U05] Py：列表去重且保序
来源：http://dul.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://kit.c1oappe.top

[U06] Py：合并两个字典
来源：http://eft.hnxiangtu.top

{**a, **b}
来源：http://fvr.xylfe.cn

[U07] Py：反转字典键值
来源：http://kyd.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://qeg.guannengcc.top

[U08] Py：展平二维列表
来源：http://vol.fktsv.cn

[y for x in nested for y in x]
来源：http://aww.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://aik.yanxiufei.cn

max(d, key=d.get)
来源：http://dev.yueranfly.top

[U10] Py：按值排序字典
来源：http://bup.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hbs.hywenlv.cn

[U11] Py：生成器表达式
来源：http://qst.iojbl.cn

(x * 2 for x in arr)
来源：http://zis.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://exe.52xcode.cn

Counter(arr).most_common(3)
来源：http://win.haohaochexian.top

[U13] Py：固定长度队列
来源：http://rlk.pycfn.com

deque(maxlen=10)
来源：http://hqp.hnxiangtu.top

[U14] Py：分组收集到列表
来源：http://wns.gzhubu.top

defaultdict(list)
来源：http://bvl.xuanzx.com

[U15] Py：高精度计时
来源：http://xex.cheryme.top

t = time.perf_counter()
来源：http://hpx.yonumen.top

[U16] Py：命令行参数解析
来源：http://rns.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sdd.iojbl.cn

[U17] Py：初始化日志
来源：http://okq.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://dwd.fehbvm.com

[U18] Py：预编译正则
来源：http://fye.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://dvn.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://lzq.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xdp.epnwcf.com

[U20] Py：缓存函数结果
来源：http://bts.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://vvp.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://fam.shangyingyoupin.top

@contextlib.contextmanager
来源：http://gct.snrcjt.cn

[U22] Py：矩阵转置
来源：http://orw.hammf.cn

list(zip(*m))
来源：http://djz.fzhhl.top

[U23] Py：分块读取大文件
来源：http://imk.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qpt.pengpengdd.cyou

[U24] Py：路径操作
来源：http://hlq.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qoc.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://mjr.zycfv.cn

csv.DictReader(f)
来源：http://qdb.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://xwn.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dpx.hnqzz.top

[U27] Py：异步 HTTP
来源：http://oqp.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://zqt.ehwqpu.com

[U28] Py：类型别名
来源：http://enk.zdbjq.cn

UserId = int
来源：http://xbg.yuxming.cn

[U29] Py：属性校验
来源：http://eem.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://gbb.bjfxy.top

[U30] Py：数据类
来源：http://lvx.ppjwa.cn

@dataclass(slots=True)
来源：http://dqi.daxiang520.top

[U31] Py：单测
来源：http://tay.vehdjk.com

python -m pytest -q
来源：http://guj.aibaodan.cn

[U32] Py：代码格式化
来源：http://ptb.zhongyouzk.top

ruff format . && ruff check --fix .
来源：http://rzc.tianlin.xyz

[U33] Py：打包发布
来源：http://hel.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://lea.jinqigufen.top

[U34] Py：判断编码
来源：http://yqn.gzhubu.top

chardet.detect(raw)
来源：http://ybz.xylfe.cn

[U35] Py：发送邮件
来源：http://klm.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqv.jqgufenzy.top

[U36] Py：定时任务
来源：http://ebp.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://zfn.xylfe.cn


<!-- 参考信息 -->