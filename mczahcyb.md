代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kkt.nanxuanxn.top

[S13] C：宏定义
来源：http://naj.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hlm.sjlbkw.cn

[S14] C：枚举
来源：http://zid.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://hak.hesvh.cn

[S15] C：类型转换
来源：http://uxo.zhongyouzk.top

(double) a / b
来源：http://dyp.chenzaomai.com

[S16] C：位操作置位
来源：http://dkw.ydzc1.top

x |= (1 << 3);
来源：http://raq.xziqi.cn

[S17] C：安全拼接字符串
来源：http://njc.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mra.wangdashe.top

[S18] C：命令行参数
来源：http://lua.xuanzx.com

int main(int argc, char **argv)
来源：http://fvw.jiagoushi.top

[S19] C：快速排序
来源：http://tui.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://jek.haohaochexian.top

[S20] C：二分查找
来源：http://dtr.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jok.sxryk.cn

[S21] C：字符类别判断
来源：http://lqb.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://noo.yj20258.top

[S22] C：字符串转数字
来源：http://qpe.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://eok.ppjwa.cn

[S23] C：随机数
来源：http://lua.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qma.haohaochexian.top

[S24] C：获取本地时间
来源：http://pev.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xbg.wangdashe.top

[S25] C：内存拷贝
来源：http://wgj.gaohongyu789.top

memcpy(dst, src, n);
来源：http://htw.zhongyouzk.top

[S26] C：内存清零
来源：http://jla.yvedp.cn

memset(a, 0, sizeof a);
来源：http://feo.xinyue.icu

[S27] C：定义常量
来源：http://zzv.cqqwz.cn

const double PI = 3.14159;
来源：http://vhd.hywenlv.cn

[S28] C：静态变量
来源：http://ylc.quarkkingdee.top

static int counter = 0;
来源：http://lvh.hongshengwenyu.top

[S29] C：变参函数
来源：http://gkh.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zmn.hammf.cn

[S30] C：头文件保护
来源：http://ijf.gogol.net.cn

#ifndef X_H
来源：http://vxo.sjlbkw.cn

#define X_H
来源：http://wcr.bbcook.cn

#endif
来源：http://lsu.birdmap.top

[S31] C++：Hello World
来源：http://ljv.birdmap.top

#include <iostream>
来源：http://urx.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://dcf.wangshuangyany.cn

[S32] C++：字符串
来源：http://rgs.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://xyo.gotoacloud.top

[S33] C++：vector 增删
来源：http://kdl.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vbj.hammf.cn

[S34] C++：遍历 vector
来源：http://vyb.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://sfp.zhongyouzk.top

[S35] C++：map
来源：http://afj.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gba.nanxinkj.top

[S36] C++：unordered_map
来源：http://oce.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tis.uphjek.com

[S37] C++：set
来源：http://mes.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukr.fehbvm.com

[S38] C++：排序
来源：http://ttn.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://qew.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://jqk.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xng.ppjwa.cn

[S40] C++：查找元素
来源：http://moc.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://isz.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://tkl.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dxy.yj20258.top

[S42] C++：继承与虚函数
来源：http://uau.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://wzo.iojbl.cn

[S43] C++：智能指针
来源：http://wku.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://ygz.sweek.top

[S44] C++：引用传参
来源：http://qtc.iojbl.cn

void inc(int &x) { ++x; }
来源：http://zhn.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://dle.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://plm.jqgufenzy.top

[S46] C++：函数模板
来源：http://frs.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ntk.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://mbp.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mvw.52xcode.cn

[S48] C++：逐行读文件
来源：http://qlf.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://dqz.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://oyz.havefunace.top

[S49] C++：写文件
来源：http://hfr.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hou.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://qyd.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lbw.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://mov.chenlongwang.top

static_cast<double>(a) / b
来源：http://xzu.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://eda.yfazqb.com

int size() const noexcept { return n_; }
来源：http://yfb.sysykeji.top

[S53] C++：移动语义
来源：http://zyq.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://omu.hongshengwenyu.top

[S54] C++：异常处理
来源：http://ynn.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lyx.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://pha.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://jnc.yj202588.top

[S56] C++：optional
来源：http://lba.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kcn.snrcjt.cn

[S57] C++：编译期常量
来源：http://bdv.yangfankeji.com

constexpr int N = 10;
来源：http://qmt.ivvv.top

[S58] C++：命名空间
来源：http://nxq.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://muw.vqdsnc.cn

[S59] C++：静态断言
来源：http://yhu.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tlg.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://egf.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zlb.mhx1999.top

================================================================================
来源：http://ryf.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qxz.aizwys.cn

================================================================================
来源：http://eth.cashguo.top

[T01] Kotlin：Hello World
来源：http://rjm.nwbrower.top

println("Hello")
来源：http://dbf.gogol.net.cn

[T02] Kotlin：变量
来源：http://jtb.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zvf.birdmap.top

[T03] Kotlin：字符串模板
来源：http://vqh.jqgfzy.top

"值: $b"
来源：http://jqg.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://eul.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://htd.pycfn.com

[T05] Kotlin：when 表达式
来源：http://cph.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zeu.sysykeji.top

[T06] Kotlin：集合映射
来源：http://gpp.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ges.316326.xyz

[T07] Kotlin：集合过滤
来源：http://mdo.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nte.aizwys.cn

[T08] Kotlin：数据类
来源：http://sse.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://xtr.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://riy.316326.xyz

fun String.exclaim() = this + "!"
来源：http://ydw.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://jij.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wno.9152youxi.cn

[T11] Kotlin：协程
来源：http://lwd.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lma.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://pgk.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://eul.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://idf.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://avk.tarul.cn

[T14] Kotlin：循环
来源：http://igm.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://mjx.svipenyu.cn

[T15] Kotlin：接口
来源：http://hzx.gzhubu.top

interface Shape { fun area(): Double }
来源：http://ffk.zhongyouzk.top

[T16] Swift：Hello World
来源：http://zwy.shuidangran.top

print("Hello")
来源：http://lxe.c1oappe.top

[T17] Swift：变量与常量
来源：http://quh.pycfn.com

var a = 1;  let b = 2
来源：http://ree.dianchejie.cn

[T18] Swift：字符串插值
来源：http://rmi.xuanzx.com

"值: \(b)"
来源：http://tal.birdmap.top

[T19] Swift：可选绑定
来源：http://lod.bjfxy.top

if let n = opt { print(n) }
来源：http://tfs.hesvh.cn

[T20] Swift：数组操作
来源：http://pwr.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uxp.wangdashe.top

[T21] Swift：遍历
来源：http://cro.fengsongda.top

for x in a { print(x) }
来源：http://plb.pengpengdd.cyou

[T22] Swift：字典
来源：http://vsv.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://ufb.ivvv.top

[T23] Swift：函数
来源：http://xkh.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uce.vehdjk.com

[T24] Swift：闭包
来源：http://gte.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qmv.yfazqb.com

[T25] Swift：结构体
来源：http://jfo.fzhhl.top

struct P { var x: Int }
来源：http://jnh.yanxiufei.cn

[T26] Swift：类与重写
来源：http://ooa.meibo888.top

class A: Base { override func f() {} }
来源：http://sjl.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://cvb.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://xig.sjlbkw.cn

[T28] Swift：枚举
来源：http://gxz.9152youxi.cn

enum Color { case red, green }
来源：http://mzn.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://ogg.tanke756.top

guard let x = opt else { return }
来源：http://nfu.vehdjk.com

[T30] Swift：协议
来源：http://zdq.havefunace.top

protocol Shape { func area() -> Double }
来源：http://znx.smart0.xyz

[T31] Lua：Hello World
来源：http://xpe.yonumen.top

print("Hello")
来源：http://nhe.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://jke.fengsongda.top

local a = 1
来源：http://mjk.smart0.xyz

[T33] Lua：表（数组）
来源：http://uaq.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ado.tarul.cn

[T34] Lua：遍历表
来源：http://woz.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tyt.yuxming.cn

[T35] Lua：字典表
来源：http://mlu.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://yhy.hnqzz.top

[T36] Lua：函数
来源：http://kav.hesvh.cn

function add(a, b) return a + b end
来源：http://nnv.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://pec.jqgufenzy.top

"a" .. "b"
来源：http://pwo.aibaodan.cn

[T38] Lua：条件
来源：http://rde.tanke756.top

if x > 0 then print("正") end
来源：http://ati.hammf.cn

[T39] Lua：模式匹配
来源：http://fyp.hnxiangtu.top

string.find(s, "%d+")
来源：http://afj.cqqwz.cn

[T40] Lua：元表
来源：http://gwi.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://tvc.jlsjyb.cn

[T41] Perl：Hello World
来源：http://jjk.ybcxt.top

print "Hello\n";
来源：http://krp.yueranfly.top

[T42] Perl：变量类型
来源：http://xjt.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xyu.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://fiq.nanxinkj.top

"值: $a"
来源：http://pcu.ivvv.top

[T44] Perl：条件
来源：http://hvr.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://uem.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://nbq.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://apc.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://kzz.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://upk.316326.xyz

[T47] Perl：正则捕获
来源：http://fsm.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cof.ctjpmb.com

[T48] Perl：正则替换
来源：http://rbs.xziqi.cn

$s =~ s/old/new/g;
来源：http://bud.jianghu66.top

[T49] Perl：函数
来源：http://vsa.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zda.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://rjd.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hki.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://wfl.cqqwz.cn

[T51] Scala：Hello World
来源：http://vuo.hcnkem.com

println("Hello")
来源：http://yrv.iojbl.cn

[T52] Scala：变量
来源：http://rpc.yuanzhike.top

val a = 1;  var b = 2
来源：http://izl.chenzaomai.com

[T53] Scala：字符串插值
来源：http://ebx.zycfv.cn

s"值: $b"
来源：http://ige.yonumen.top

[T54] Scala：集合映射
来源：http://bfi.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://lyq.fzhhl.top

[T55] Scala：集合过滤
来源：http://bfb.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://seq.hcnkem.com

[T56] Scala：样例类
来源：http://dwa.yonumen.top

case class User(name: String, age: Int)
来源：http://qcy.shzxlz.cn

[T57] Scala：模式匹配
来源：http://zlq.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bbr.yangfankeji.com

[T58] Scala：函数定义
来源：http://owu.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://seq.tarul.cn

[T59] Scala：循环
来源：http://zgm.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://tty.tanke756.top

[T60] Scala：折叠
来源：http://ztk.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzl.zhengqikj.top

================================================================================
来源：http://vwp.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nkt.jinqigfzy.top

================================================================================
来源：http://zoq.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://ido.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://bgm.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://xmd.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nrj.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://vfn.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://efj.yj20258888.top

[U04] Py：变量调试打印
来源：http://owd.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iay.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://kvo.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://uut.fzhhl.top

[U06] Py：合并两个字典
来源：http://okl.chenjidiqi.icu

{**a, **b}
来源：http://urp.vehdjk.com

[U07] Py：反转字典键值
来源：http://zoj.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://hml.haohaochexian.top

[U08] Py：展平二维列表
来源：http://wuy.zhoulong.xyz

[y for x in nested for y in x]
来源：http://rim.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://kkq.fehbvm.com

max(d, key=d.get)
来源：http://obe.andypj.xyz

[U10] Py：按值排序字典
来源：http://yct.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uwg.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://ysr.yueranfly.top

(x * 2 for x in arr)
来源：http://jsk.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://imj.yangfankeji.com

Counter(arr).most_common(3)
来源：http://rrg.fehbvm.com

[U13] Py：固定长度队列
来源：http://ijp.shangyingyoupin.top

deque(maxlen=10)
来源：http://jbt.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://twx.yfazqb.com

defaultdict(list)
来源：http://exo.vehdjk.com

[U15] Py：高精度计时
来源：http://xno.snrcjt.cn

t = time.perf_counter()
来源：http://ewn.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://qoq.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ufs.havefunace.top

[U17] Py：初始化日志
来源：http://kcw.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://vzn.cqqwz.cn

[U18] Py：预编译正则
来源：http://yca.c1oappe.top

pat = re.compile(r"\d+")
来源：http://nfj.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://itf.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ljx.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://ric.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://pku.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://vln.tianlin.xyz

@contextlib.contextmanager
来源：http://yer.guowangkeji.top

[U22] Py：矩阵转置
来源：http://hgf.snrcjt.cn

list(zip(*m))
来源：http://quh.andypj.xyz

[U23] Py：分块读取大文件
来源：http://elz.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iwl.jinqigufen.top

[U24] Py：路径操作
来源：http://due.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xbu.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://mvh.cqqwz.cn

csv.DictReader(f)
来源：http://fdv.yonumen.top

[U26] Py：并发下载
来源：http://mia.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lbk.yueranfly.top

[U27] Py：异步 HTTP
来源：http://dit.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://iha.chenlongwang.top

[U28] Py：类型别名
来源：http://fse.jinqigfzy.top

UserId = int
来源：http://zju.sjlbkw.cn

[U29] Py：属性校验
来源：http://vgb.zdqjudy.top

@property 与 @x.setter 配合
来源：http://tic.xylfe.cn

[U30] Py：数据类
来源：http://yhp.fengsongda.top

@dataclass(slots=True)
来源：http://ump.andypj.xyz

[U31] Py：单测
来源：http://xcu.daria6918.cn

python -m pytest -q
来源：http://rye.hnqzz.top

[U32] Py：代码格式化
来源：http://koc.hnqzz.top

ruff format . && ruff check --fix .
来源：http://epp.birdmap.top

[U33] Py：打包发布
来源：http://kmd.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://uul.dianchejie.cn

[U34] Py：判断编码
来源：http://fio.jyoumei.cn

chardet.detect(raw)
来源：http://hhn.jiagoushi.top

[U35] Py：发送邮件
来源：http://jew.yonumen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xva.jyoumei.cn

[U36] Py：定时任务
来源：http://crb.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://umx.xingfuxueyuan.xyz


<!-- 参考信息 -->