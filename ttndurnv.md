代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ucu.birdmap.top

[S13] C：宏定义
来源：http://uud.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nyp.0kj1m.cn

[S14] C：枚举
来源：http://flk.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://afr.nwbrower.top

[S15] C：类型转换
来源：http://ujh.zhiwuduotai.top

(double) a / b
来源：http://ixr.chenlongwang.top

[S16] C：位操作置位
来源：http://ncb.hnxiangtu.top

x |= (1 << 3);
来源：http://ete.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://kvt.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vua.redwolf501.top

[S18] C：命令行参数
来源：http://fbe.pycfn.com

int main(int argc, char **argv)
来源：http://sil.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://vlj.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://noq.gzhubu.top

[S20] C：二分查找
来源：http://ktg.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sgb.gaohongyu789.top

[S21] C：字符类别判断
来源：http://xwq.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bai.jianghu66.top

[S22] C：字符串转数字
来源：http://cqh.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uzu.guowangkeji.top

[S23] C：随机数
来源：http://qwe.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ugq.yonumen.top

[S24] C：获取本地时间
来源：http://edj.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qmq.tanke756.top

[S25] C：内存拷贝
来源：http://ufz.hammf.cn

memcpy(dst, src, n);
来源：http://uhu.fehbvm.com

[S26] C：内存清零
来源：http://bnn.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://lvb.zhongyouzk.top

[S27] C：定义常量
来源：http://edk.0kj1m.cn

const double PI = 3.14159;
来源：http://eqm.yueranfly.top

[S28] C：静态变量
来源：http://djw.wangdashe.top

static int counter = 0;
来源：http://jeu.jlsjyb.cn

[S29] C：变参函数
来源：http://lqt.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://idq.xuetiantiany.cn

[S30] C：头文件保护
来源：http://zwm.316326.xyz

#ifndef X_H
来源：http://lws.chenzaomai.com

#define X_H
来源：http://soh.tianlin.xyz

#endif
来源：http://tri.xziqi.cn

[S31] C++：Hello World
来源：http://zql.cqqwz.cn

#include <iostream>
来源：http://ywn.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://psm.sufxvd.cn

[S32] C++：字符串
来源：http://bup.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://yos.vqdsnc.cn

[S33] C++：vector 增删
来源：http://lle.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://drk.daria6918.cn

[S34] C++：遍历 vector
来源：http://gme.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://azh.jianghu66.top

[S35] C++：map
来源：http://syv.andypj.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hvd.yj202588.top

[S36] C++：unordered_map
来源：http://epo.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vtk.daria6918.cn

[S37] C++：set
来源：http://rqt.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wxv.chenlongwang.top

[S38] C++：排序
来源：http://icq.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://dkc.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://nhg.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iap.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://dvx.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ihr.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://zfc.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://srn.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://mjb.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://hzi.ydzc1.top

[S43] C++：智能指针
来源：http://tmv.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://ziz.xuetiantiany.cn

[S44] C++：引用传参
来源：http://ifh.vehdjk.com

void inc(int &x) { ++x; }
来源：http://mjy.sysykeji.top

[S45] C++：lambda
来源：http://zlj.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://cvu.hcnkem.com

[S46] C++：函数模板
来源：http://fmt.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kul.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://xsf.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hrx.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://dld.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sat.yvedp.cn

while (std::getline(in, line)) { }
来源：http://nbi.yuanzhike.top

[S49] C++：写文件
来源：http://pgx.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fhp.yj20258.top

[S50] C++：格式化数字
来源：http://byn.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yps.snrcjt.cn

[S51] C++：显式类型转换
来源：http://fcs.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://wda.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://nhp.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://qat.hywenlv.cn

[S53] C++：移动语义
来源：http://nct.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://ofj.52xcode.cn

[S54] C++：异常处理
来源：http://tjq.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxx.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://bpc.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://hcy.ppjwa.cn

[S56] C++：optional
来源：http://nuu.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fpl.cdnleiting.top

[S57] C++：编译期常量
来源：http://civ.hnxiangtu.top

constexpr int N = 10;
来源：http://wky.feifeiyinyue.top

[S58] C++：命名空间
来源：http://suq.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://pac.zdqjudy.top

[S59] C++：静态断言
来源：http://euf.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cqo.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://ycf.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://khu.gzhubu.top

================================================================================
来源：http://irs.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxz.vehdjk.com

================================================================================
来源：http://lov.yfazqb.com

[T01] Kotlin：Hello World
来源：http://wsd.hywenlv.cn

println("Hello")
来源：http://dfv.ctjpmb.com

[T02] Kotlin：变量
来源：http://kio.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tvs.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://npe.dianchejie.cn

"值: $b"
来源：http://wfs.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://uiz.hesvh.cn

val n: String? = null;  n?.length
来源：http://bte.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://bog.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ify.birdmap.top

[T06] Kotlin：集合映射
来源：http://fwz.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ged.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://omx.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hcj.yuxming.cn

[T08] Kotlin：数据类
来源：http://mjl.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://zvo.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://lsc.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://xmh.tarul.cn

[T10] Kotlin：默认参数
来源：http://jmn.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://app.andypj.xyz

[T11] Kotlin：协程
来源：http://pdu.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://fsl.aizwys.cn

[T12] Kotlin：解构声明
来源：http://cfj.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://zlv.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://ntv.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://xgg.zhengqikj.top

[T14] Kotlin：循环
来源：http://heo.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://sbi.c1oappe.top

[T15] Kotlin：接口
来源：http://imy.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://rhk.vqdsnc.cn

[T16] Swift：Hello World
来源：http://cwp.yanxiufei.cn

print("Hello")
来源：http://alr.bjfxy.top

[T17] Swift：变量与常量
来源：http://sqv.zdbjq.cn

var a = 1;  let b = 2
来源：http://rue.guowangkeji.top

[T18] Swift：字符串插值
来源：http://hqq.yonumen.top

"值: \(b)"
来源：http://vgx.fehbvm.com

[T19] Swift：可选绑定
来源：http://deq.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://mqu.chenzaomai.com

[T20] Swift：数组操作
来源：http://gdf.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://rgn.fengsongda.top

[T21] Swift：遍历
来源：http://kyh.sxryk.cn

for x in a { print(x) }
来源：http://kpc.yonumen.top

[T22] Swift：字典
来源：http://jod.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://ghh.shzxlz.cn

[T23] Swift：函数
来源：http://opl.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://asp.xylfe.cn

[T24] Swift：闭包
来源：http://gkl.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cft.xylfe.cn

[T25] Swift：结构体
来源：http://dqw.xuetiantiany.cn

struct P { var x: Int }
来源：http://upm.hnqzz.top

[T26] Swift：类与重写
来源：http://hpy.zycfv.cn

class A: Base { override func f() {} }
来源：http://fli.haohaochexian.top

[T27] Swift：错误处理
来源：http://eij.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://aqe.xuanzx.com

[T28] Swift：枚举
来源：http://aep.zycfv.cn

enum Color { case red, green }
来源：http://lwl.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://njr.yj202588.top

guard let x = opt else { return }
来源：http://dtg.shangyingyoupin.top

[T30] Swift：协议
来源：http://efx.pycfn.com

protocol Shape { func area() -> Double }
来源：http://qqh.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://xvt.ybcxt.top

print("Hello")
来源：http://rcx.vqdsnc.cn

[T32] Lua：局部变量
来源：http://pyi.shuidangran.top

local a = 1
来源：http://hwg.xylfe.cn

[T33] Lua：表（数组）
来源：http://gxu.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ruh.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://hwx.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hdq.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://zjf.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://aiw.sjlbkw.cn

[T36] Lua：函数
来源：http://rlf.gogol.net.cn

function add(a, b) return a + b end
来源：http://zpv.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://hgj.xuanzx.com

"a" .. "b"
来源：http://zpr.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://ngf.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://bxt.zdqjudy.top

[T39] Lua：模式匹配
来源：http://cya.jinqigfzy.top

string.find(s, "%d+")
来源：http://bdc.fengsongda.top

[T40] Lua：元表
来源：http://jqq.fzhhl.top

setmetatable({}, { __index = base })
来源：http://thf.shzxlz.cn

[T41] Perl：Hello World
来源：http://hhl.52xcode.cn

print "Hello\n";
来源：http://wwy.redwolf501.top

[T42] Perl：变量类型
来源：http://wuv.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zqi.birdmap.top

[T43] Perl：字符串插值
来源：http://jbf.yj20258.top

"值: $a"
来源：http://yxg.yvedp.cn

[T44] Perl：条件
来源：http://lpn.cashguo.top

if ($a > 0) { print "正"; }
来源：http://phi.daxiang520.top

[T45] Perl：数组遍历
来源：http://hvr.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://rqq.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://lra.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pdo.yonumen.top

[T47] Perl：正则捕获
来源：http://ajh.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kur.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://teu.dianchejie.cn

$s =~ s/old/new/g;
来源：http://tjl.tarul.cn

[T49] Perl：函数
来源：http://flh.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lah.tanke756.top

[T50] Perl：逐行读文件
来源：http://utb.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lcj.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://jqp.cqqwz.cn

[T51] Scala：Hello World
来源：http://arn.jlsjyb.cn

println("Hello")
来源：http://rdx.fzhhl.top

[T52] Scala：变量
来源：http://gtj.tarul.cn

val a = 1;  var b = 2
来源：http://olx.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://cqr.ppjwa.cn

s"值: $b"
来源：http://esj.aizwys.cn

[T54] Scala：集合映射
来源：http://rzr.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://vfc.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://wty.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://fvn.epnwcf.com

[T56] Scala：样例类
来源：http://ytu.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://dsx.yonumen.top

[T57] Scala：模式匹配
来源：http://ipe.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://scf.gzhubu.top

[T58] Scala：函数定义
来源：http://tfb.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://phd.yanxiufei.cn

[T59] Scala：循环
来源：http://gcs.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://ycf.chenzaomai.com

[T60] Scala：折叠
来源：http://viu.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kmv.yanxiufei.cn

================================================================================
来源：http://skc.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uod.daria6918.cn

================================================================================
来源：http://tdm.cashguo.top

[U01] Py：创建虚拟环境
来源：http://jxh.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://vuc.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://eit.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tdd.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://zap.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ylv.jqgfzy.top

[U04] Py：变量调试打印
来源：http://xva.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ior.xuanzx.com

[U05] Py：列表去重且保序
来源：http://zvu.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://jvy.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://ksh.nwbrower.top

{**a, **b}
来源：http://izh.52xcode.cn

[U07] Py：反转字典键值
来源：http://cby.xylfe.cn

{v: k for k, v in d.items()}
来源：http://zfn.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://gjj.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://czx.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://meo.smart0.xyz

max(d, key=d.get)
来源：http://ski.redwolf501.top

[U10] Py：按值排序字典
来源：http://gao.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mnu.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://gef.andypj.xyz

(x * 2 for x in arr)
来源：http://ink.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zxe.9152youxi.cn

Counter(arr).most_common(3)
来源：http://por.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://bev.sjlbkw.cn

deque(maxlen=10)
来源：http://jok.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://wds.hesvh.cn

defaultdict(list)
来源：http://faz.tian-w.cn

[U15] Py：高精度计时
来源：http://nxy.xinyue.icu

t = time.perf_counter()
来源：http://ijk.hammf.cn

[U16] Py：命令行参数解析
来源：http://bjx.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uqj.tarul.cn

[U17] Py：初始化日志
来源：http://fip.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://gqa.svipenyu.cn

[U18] Py：预编译正则
来源：http://oxb.cheryme.top

pat = re.compile(r"\d+")
来源：http://bmq.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://exh.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://moj.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://dnp.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://nkg.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://mad.epnwcf.com

@contextlib.contextmanager
来源：http://wai.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://fig.birdmap.top

list(zip(*m))
来源：http://xuq.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://ciu.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fjr.tanke756.top

[U24] Py：路径操作
来源：http://wqh.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ewn.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://lci.zdqjudy.top

csv.DictReader(f)
来源：http://gtm.ydzc1.top

[U26] Py：并发下载
来源：http://vlg.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yum.sysykeji.top

[U27] Py：异步 HTTP
来源：http://sir.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://xpo.fengsongda.top

[U28] Py：类型别名
来源：http://wdt.aizwys.cn

UserId = int
来源：http://mhd.0kj1m.cn

[U29] Py：属性校验
来源：http://jta.fzhhl.top

@property 与 @x.setter 配合
来源：http://dre.tanke756.top

[U30] Py：数据类
来源：http://jbc.cashguo.top

@dataclass(slots=True)
来源：http://jik.kuanghao11.cn

[U31] Py：单测
来源：http://szb.bjfxy.top

python -m pytest -q
来源：http://hzv.cucudq.cn

[U32] Py：代码格式化
来源：http://yow.cucudq.cn

ruff format . && ruff check --fix .
来源：http://tav.yj20258.top

[U33] Py：打包发布
来源：http://ptt.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://jqq.zhixingplan.top

[U34] Py：判断编码
来源：http://mvw.zhixingplan.top

chardet.detect(raw)
来源：http://gpf.jinqigufen.top

[U35] Py：发送邮件
来源：http://lme.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ehe.svipenyu.cn

[U36] Py：定时任务
来源：http://mmr.yj20258.top

schedule.every(10).minutes.do(job)
来源：http://nbt.feifeiyinyue.top


<!-- 参考信息 -->