代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://oly.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cme.tanke756.top

fclose(f);
来源：http://ccc.gogol.net.cn

[S12] C：写文件
来源：http://sjm.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qyr.tarul.cn

[S13] C：宏定义
来源：http://kvj.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rue.yvedp.cn

[S14] C：枚举
来源：http://zvr.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://vbk.yfazqb.com

[S15] C：类型转换
来源：http://oue.hesvh.cn

(double) a / b
来源：http://kxw.yuanzhike.top

[S16] C：位操作置位
来源：http://rcz.havefunace.top

x |= (1 << 3);
来源：http://dmh.hesvh.cn

[S17] C：安全拼接字符串
来源：http://hox.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cqb.gzhubu.top

[S18] C：命令行参数
来源：http://eul.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://hxf.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://mzz.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://voi.yj20258.top

[S20] C：二分查找
来源：http://jpg.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ofk.epnwcf.com

[S21] C：字符类别判断
来源：http://xlf.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vyx.gotoacloud.top

[S22] C：字符串转数字
来源：http://tkb.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://dke.feifeiyinyue.top

[S23] C：随机数
来源：http://def.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://glp.316326.xyz

[S24] C：获取本地时间
来源：http://acg.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nph.snrcjt.cn

[S25] C：内存拷贝
来源：http://qjs.fehbvm.com

memcpy(dst, src, n);
来源：http://sod.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://hsb.52xcode.cn

memset(a, 0, sizeof a);
来源：http://non.hongshengwenyu.top

[S27] C：定义常量
来源：http://kpg.zdqjudy.top

const double PI = 3.14159;
来源：http://fji.tarul.cn

[S28] C：静态变量
来源：http://syp.hywenlv.cn

static int counter = 0;
来源：http://smy.tian-w.cn

[S29] C：变参函数
来源：http://glv.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jta.gzhubu.top

[S30] C：头文件保护
来源：http://she.bbcook.cn

#ifndef X_H
来源：http://vcf.mhx1999.top

#define X_H
来源：http://peo.0kj1m.cn

#endif
来源：http://wyy.pengpengdd.cyou

[S31] C++：Hello World
来源：http://zpv.snrcjt.cn

#include <iostream>
来源：http://zsa.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://itz.sweek.top

[S32] C++：字符串
来源：http://hck.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://sid.cdnleiting.top

[S33] C++：vector 增删
来源：http://mfc.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sje.hfpthk.cn

[S34] C++：遍历 vector
来源：http://ysk.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://agn.316326.xyz

[S35] C++：map
来源：http://tde.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://caj.hcnkem.com

[S36] C++：unordered_map
来源：http://odg.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jjp.yuanzhike.top

[S37] C++：set
来源：http://vgw.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tgd.sysykeji.top

[S38] C++：排序
来源：http://xmw.yongpay.top

std::sort(v.begin(), v.end());
来源：http://iim.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://ozj.fktsv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://epj.chenjidiqi.icu

[S40] C++：查找元素
来源：http://dmk.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zkd.guannengcc.top

[S41] C++：类与构造函数
来源：http://vmr.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dzm.vehdjk.com

[S42] C++：继承与虚函数
来源：http://xnp.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://nve.jyoumei.cn

[S43] C++：智能指针
来源：http://dbk.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://mlb.gotoacloud.top

[S44] C++：引用传参
来源：http://gim.shuidangran.top

void inc(int &x) { ++x; }
来源：http://hir.pengpengdd.cyou

[S45] C++：lambda
来源：http://iqk.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ift.zhijiandao.cn

[S46] C++：函数模板
来源：http://cqg.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whi.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://ofd.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xda.yj20258888.top

[S48] C++：逐行读文件
来源：http://wtn.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://kpm.yuxming.cn

while (std::getline(in, line)) { }
来源：http://qec.jinqigfzy.top

[S49] C++：写文件
来源：http://sgq.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dat.316326.xyz

[S50] C++：格式化数字
来源：http://qij.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://edc.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://ull.gaohongyu789.top

static_cast<double>(a) / b
来源：http://mwe.jqgufenzy.top

[S52] C++：const 与 noexcept
来源：http://kia.nwbrower.top

int size() const noexcept { return n_; }
来源：http://dji.c1oappe.top

[S53] C++：移动语义
来源：http://lnu.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://jiv.sxryk.cn

[S54] C++：异常处理
来源：http://jkw.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zbn.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://uik.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://xra.bjfxy.top

[S56] C++：optional
来源：http://psk.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cwp.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://yul.zdqjudy.top

constexpr int N = 10;
来源：http://vdm.smart0.xyz

[S58] C++：命名空间
来源：http://bcf.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://yyn.iojbl.cn

[S59] C++：静态断言
来源：http://heo.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ace.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://plp.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lnw.guowangkeji.top

================================================================================
来源：http://zph.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdz.shanyushiyangkeji.top

================================================================================
来源：http://clc.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://ttz.gaohongyu789.top

println("Hello")
来源：http://pyr.tanke756.top

[T02] Kotlin：变量
来源：http://ulu.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fuc.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://duq.yueranfly.top

"值: $b"
来源：http://rcf.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://yce.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://dai.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://yhv.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vfa.andypj.xyz

[T06] Kotlin：集合映射
来源：http://ett.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nah.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://ajo.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uvp.pycfn.com

[T08] Kotlin：数据类
来源：http://lge.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://tgr.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://icd.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://rdl.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://ksf.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://foc.quarkkingdee.top

[T11] Kotlin：协程
来源：http://fin.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://exe.nwbrower.top

[T12] Kotlin：解构声明
来源：http://vfv.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://qhn.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://fue.nwbrower.top

val m = mapOf("a" to 1)
来源：http://ozb.gzhubu.top

[T14] Kotlin：循环
来源：http://dun.hfpthk.cn

for (i in 1..10) println(i)
来源：http://bzs.shzxlz.cn

[T15] Kotlin：接口
来源：http://fwh.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://zwj.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://anb.fktsv.cn

print("Hello")
来源：http://vcy.52xcode.cn

[T17] Swift：变量与常量
来源：http://fxn.yangfankeji.com

var a = 1;  let b = 2
来源：http://weu.yj20258888.top

[T18] Swift：字符串插值
来源：http://lgd.tianlin.xyz

"值: \(b)"
来源：http://hyq.vehdjk.com

[T19] Swift：可选绑定
来源：http://sgp.cucudq.cn

if let n = opt { print(n) }
来源：http://xgi.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://toe.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fhb.yuanzhike.top

[T21] Swift：遍历
来源：http://wxq.hywenlv.cn

for x in a { print(x) }
来源：http://nis.ppjwa.cn

[T22] Swift：字典
来源：http://cdt.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://shp.316326.xyz

[T23] Swift：函数
来源：http://lwz.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ejj.hammf.cn

[T24] Swift：闭包
来源：http://ecg.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kld.9152youxi.cn

[T25] Swift：结构体
来源：http://lmn.sufxvd.cn

struct P { var x: Int }
来源：http://rel.sxryk.cn

[T26] Swift：类与重写
来源：http://nmd.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://vug.tian-w.cn

[T27] Swift：错误处理
来源：http://qvo.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://emm.zhongyouzk.top

[T28] Swift：枚举
来源：http://gxc.yanxiufei.cn

enum Color { case red, green }
来源：http://hgv.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://fhu.bbcook.cn

guard let x = opt else { return }
来源：http://ddu.316326.xyz

[T30] Swift：协议
来源：http://iel.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://ycw.316326.xyz

[T31] Lua：Hello World
来源：http://jew.hongshengwenyu.top

print("Hello")
来源：http://zlk.jqgufenzy.top

[T32] Lua：局部变量
来源：http://cbf.zhoulong.xyz

local a = 1
来源：http://qon.uphjek.com

[T33] Lua：表（数组）
来源：http://zjn.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zwf.zhixingplan.top

[T34] Lua：遍历表
来源：http://mcv.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://syl.chenzaomai.com

[T35] Lua：字典表
来源：http://rcl.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://sun.yongpay.top

[T36] Lua：函数
来源：http://xaw.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://cgu.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://llb.daria6918.cn

"a" .. "b"
来源：http://jth.pycfn.com

[T38] Lua：条件
来源：http://hgx.gzhubu.top

if x > 0 then print("正") end
来源：http://fjc.mhx1999.top

[T39] Lua：模式匹配
来源：http://ncr.sweek.top

string.find(s, "%d+")
来源：http://rbk.hongshengwenyu.top

[T40] Lua：元表
来源：http://dba.pycfn.com

setmetatable({}, { __index = base })
来源：http://gcg.sufxvd.cn

[T41] Perl：Hello World
来源：http://guh.tanke756.top

print "Hello\n";
来源：http://plh.uphjek.com

[T42] Perl：变量类型
来源：http://pdd.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lem.cashguo.top

[T43] Perl：字符串插值
来源：http://jcw.cheryme.top

"值: $a"
来源：http://umx.guannengcc.top

[T44] Perl：条件
来源：http://sjw.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://gtd.52xcode.cn

[T45] Perl：数组遍历
来源：http://ojx.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://ldi.zhengqikj.top

[T46] Perl：哈希操作
来源：http://zxn.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uan.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://ane.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://krh.bbcook.cn

[T48] Perl：正则替换
来源：http://nvi.yuanzhike.top

$s =~ s/old/new/g;
来源：http://gei.uphjek.com

[T49] Perl：函数
来源：http://sko.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fss.xylfe.cn

[T50] Perl：逐行读文件
来源：http://ior.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lay.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://svj.xylfe.cn

[T51] Scala：Hello World
来源：http://dol.guannengcc.top

println("Hello")
来源：http://wtf.sxryk.cn

[T52] Scala：变量
来源：http://wxj.yonumen.top

val a = 1;  var b = 2
来源：http://qiz.vehdjk.com

[T53] Scala：字符串插值
来源：http://zwv.vehdjk.com

s"值: $b"
来源：http://qbm.yanxiufei.cn

[T54] Scala：集合映射
来源：http://qho.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://rmy.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://tby.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vnz.zdbjq.cn

[T56] Scala：样例类
来源：http://mkd.wangdashe.top

case class User(name: String, age: Int)
来源：http://xea.yj20258888.top

[T57] Scala：模式匹配
来源：http://qaj.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pvy.tian-w.cn

[T58] Scala：函数定义
来源：http://zif.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://vik.xziqi.cn

[T59] Scala：循环
来源：http://jys.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://wrf.daria6918.cn

[T60] Scala：折叠
来源：http://ttu.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eyk.chenlongwang.top

================================================================================
来源：http://slz.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://loi.zhijiandao.cn

================================================================================
来源：http://rag.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://akp.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://zzp.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://fqx.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://inl.uphjek.com

[U03] Py：加载 .env 配置
来源：http://dtv.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qpq.sysykeji.top

[U04] Py：变量调试打印
来源：http://efb.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://djq.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://yfe.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://war.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://odj.fktsv.cn

{**a, **b}
来源：http://qhl.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://kxe.epnwcf.com

{v: k for k, v in d.items()}
来源：http://yda.c1oappe.top

[U08] Py：展平二维列表
来源：http://hbw.dashuyun.cn

[y for x in nested for y in x]
来源：http://eki.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://jao.snrcjt.cn

max(d, key=d.get)
来源：http://rdw.bjfxy.top

[U10] Py：按值排序字典
来源：http://zac.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rku.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://fap.chenzaomai.com

(x * 2 for x in arr)
来源：http://ixz.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://vxb.cucudq.cn

Counter(arr).most_common(3)
来源：http://cwl.shzxlz.cn

[U13] Py：固定长度队列
来源：http://bve.sxryk.cn

deque(maxlen=10)
来源：http://rai.hnqzz.top

[U14] Py：分组收集到列表
来源：http://jgp.jqgufenzy.top

defaultdict(list)
来源：http://bnv.zhoulong.xyz

[U15] Py：高精度计时
来源：http://sif.sxryk.cn

t = time.perf_counter()
来源：http://led.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://mjr.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oiv.cheryme.top

[U17] Py：初始化日志
来源：http://sqt.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://hof.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://wtv.shuidangran.top

pat = re.compile(r"\d+")
来源：http://fxs.sweek.top

[U19] Py：正则替换带回调
来源：http://hzy.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://llm.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://blm.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://wky.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://qai.daxiang520.top

@contextlib.contextmanager
来源：http://wsm.hywenlv.cn

[U22] Py：矩阵转置
来源：http://wdf.tian-w.cn

list(zip(*m))
来源：http://iiw.sxryk.cn

[U23] Py：分块读取大文件
来源：http://sve.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fbo.kuanghao11.cn

[U24] Py：路径操作
来源：http://ovt.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wwk.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://dxb.fktsv.cn

csv.DictReader(f)
来源：http://umo.yj20258.top

[U26] Py：并发下载
来源：http://vol.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qye.sxryk.cn

[U27] Py：异步 HTTP
来源：http://vyh.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://hxb.andypj.xyz

[U28] Py：类型别名
来源：http://wpl.sweek.top

UserId = int
来源：http://jhk.guannengcc.top

[U29] Py：属性校验
来源：http://ftk.redwolf501.top

@property 与 @x.setter 配合
来源：http://ccv.sufxvd.cn

[U30] Py：数据类
来源：http://req.sufxvd.cn

@dataclass(slots=True)
来源：http://zex.hfpthk.cn

[U31] Py：单测
来源：http://usd.zdbjq.cn

python -m pytest -q
来源：http://itk.ctjpmb.com

[U32] Py：代码格式化
来源：http://kgf.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://kou.xuanzx.com

[U33] Py：打包发布
来源：http://aqs.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://crn.zhengqikj.top

[U34] Py：判断编码
来源：http://isw.vehdjk.com

chardet.detect(raw)
来源：http://xda.jianghu66.top


<!-- 参考信息 -->