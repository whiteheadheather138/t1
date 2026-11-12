代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eho.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://bfs.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fnz.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://cam.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ogn.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://hic.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://vbu.gogol.net.cn

[S11] C：逐行读文件
来源：http://rgd.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://lgf.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fzu.fzhhl.top

fclose(f);
来源：http://pqg.guannengcc.top

[S12] C：写文件
来源：http://vos.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gmo.quarkkingdee.top

[S13] C：宏定义
来源：http://fxx.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sdx.vehdjk.com

[S14] C：枚举
来源：http://hhf.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://yjz.yongpay.top

[S15] C：类型转换
来源：http://uhi.tarul.cn

(double) a / b
来源：http://lgg.ctjpmb.com

[S16] C：位操作置位
来源：http://fzv.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://vrl.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://shg.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eiy.gaohongyu789.top

[S18] C：命令行参数
来源：http://rjv.yuxming.cn

int main(int argc, char **argv)
来源：http://xes.cashguo.top

[S19] C：快速排序
来源：http://umm.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bqm.9152youxi.cn

[S20] C：二分查找
来源：http://ksh.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dnt.yanxiufei.cn

[S21] C：字符类别判断
来源：http://ahi.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ouj.jinqigufen.top

[S22] C：字符串转数字
来源：http://oji.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kgk.nanxinkj.top

[S23] C：随机数
来源：http://epn.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://udn.zdqjudy.top

[S24] C：获取本地时间
来源：http://keh.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ufs.cashguo.top

[S25] C：内存拷贝
来源：http://ots.epnwcf.com

memcpy(dst, src, n);
来源：http://zve.jlsjyb.cn

[S26] C：内存清零
来源：http://njp.yj20258.top

memset(a, 0, sizeof a);
来源：http://uhi.jyoumei.cn

[S27] C：定义常量
来源：http://tvm.tianlin.xyz

const double PI = 3.14159;
来源：http://hub.9152youxi.cn

[S28] C：静态变量
来源：http://okb.zhengqikj.top

static int counter = 0;
来源：http://gql.zhiwuduotai.top

[S29] C：变参函数
来源：http://noz.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iig.guannengcc.top

[S30] C：头文件保护
来源：http://cwp.mhx1999.top

#ifndef X_H
来源：http://yen.hysaishi.cn

#define X_H
来源：http://one.sxryk.cn

#endif
来源：http://hif.hnxiangtu.top

[S31] C++：Hello World
来源：http://wet.hcnkem.com

#include <iostream>
来源：http://fqv.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://thv.jqgfzy.top

[S32] C++：字符串
来源：http://mzh.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://lyn.fzhhl.top

[S33] C++：vector 增删
来源：http://gsh.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vwf.fengsongda.top

[S34] C++：遍历 vector
来源：http://yhu.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://tmq.yongpay.top

[S35] C++：map
来源：http://pis.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ixa.zhoulong.xyz

[S36] C++：unordered_map
来源：http://htq.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zge.guannengcc.top

[S37] C++：set
来源：http://das.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vqy.hnxiangtu.top

[S38] C++：排序
来源：http://gjz.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://jse.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://nlp.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fme.wangdashe.top

[S40] C++：查找元素
来源：http://kgm.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://biv.fehbvm.com

[S41] C++：类与构造函数
来源：http://kox.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iiq.ybcxt.top

[S42] C++：继承与虚函数
来源：http://jgr.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://xcx.sweek.top

[S43] C++：智能指针
来源：http://xiy.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://jwn.zhengqikj.top

[S44] C++：引用传参
来源：http://qsa.yj20258.top

void inc(int &x) { ++x; }
来源：http://svo.gaohongyu789.top

[S45] C++：lambda
来源：http://mil.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://jly.zdbjq.cn

[S46] C++：函数模板
来源：http://eqn.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ftz.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://asn.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bbz.xinyue.icu

[S48] C++：逐行读文件
来源：http://zur.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rgl.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://iyg.fzhhl.top

[S49] C++：写文件
来源：http://cyu.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pik.bbcook.cn

[S50] C++：格式化数字
来源：http://ngv.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zin.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://aji.meibo888.top

static_cast<double>(a) / b
来源：http://zrm.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://fxl.hcnkem.com

int size() const noexcept { return n_; }
来源：http://tiy.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://dce.ivvv.top

std::vector<int> w = std::move(v);
来源：http://eqi.shangyingyoupin.top

[S54] C++：异常处理
来源：http://zwm.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bsa.hywenlv.cn

[S55] C++：结构化绑定
来源：http://lbl.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://duc.zhijiandao.cn

[S56] C++：optional
来源：http://sor.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hmj.ppjwa.cn

[S57] C++：编译期常量
来源：http://xvl.cqqwz.cn

constexpr int N = 10;
来源：http://unb.fengsongda.top

[S58] C++：命名空间
来源：http://rcv.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://qgf.tanke756.top

[S59] C++：静态断言
来源：http://jlg.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dja.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://ueo.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xdl.tarul.cn

================================================================================
来源：http://epk.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://syw.pengpengdd.cyou

================================================================================
来源：http://lxh.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://lsn.wangdashe.top

println("Hello")
来源：http://sev.redwolf501.top

[T02] Kotlin：变量
来源：http://cij.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hlx.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://yod.9152youxi.cn

"值: $b"
来源：http://zlq.hcnkem.com

[T04] Kotlin：空安全
来源：http://tyy.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://ghi.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://hjl.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://thg.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://kif.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zmb.tanke756.top

[T07] Kotlin：集合过滤
来源：http://zmi.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykn.guowangkeji.top

[T08] Kotlin：数据类
来源：http://rwi.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://spq.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://niv.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://ywy.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://olm.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qsy.birdmap.top

[T11] Kotlin：协程
来源：http://cjm.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pbh.yongpay.top

[T12] Kotlin：解构声明
来源：http://fmg.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://dyv.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://qlg.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://ryt.shzxlz.cn

[T14] Kotlin：循环
来源：http://gjk.xylfe.cn

for (i in 1..10) println(i)
来源：http://uzp.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://fgo.shuidangran.top

interface Shape { fun area(): Double }
来源：http://psj.yangfankeji.com

[T16] Swift：Hello World
来源：http://isg.zhijiandao.cn

print("Hello")
来源：http://qzh.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://spg.xziqi.cn

var a = 1;  let b = 2
来源：http://lvs.chenlongwang.top

[T18] Swift：字符串插值
来源：http://dll.shuidangran.top

"值: \(b)"
来源：http://htf.tanke756.top

[T19] Swift：可选绑定
来源：http://ayl.cashguo.top

if let n = opt { print(n) }
来源：http://tpr.ivvv.top

[T20] Swift：数组操作
来源：http://gqg.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://loq.pycfn.com

[T21] Swift：遍历
来源：http://qqk.tianlin.xyz

for x in a { print(x) }
来源：http://yje.gotoacloud.top

[T22] Swift：字典
来源：http://fec.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://zft.yj202588.top

[T23] Swift：函数
来源：http://itk.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gzd.xylfe.cn

[T24] Swift：闭包
来源：http://trg.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bke.zycfv.cn

[T25] Swift：结构体
来源：http://pop.hammf.cn

struct P { var x: Int }
来源：http://fnm.quarkkingdee.top

[T26] Swift：类与重写
来源：http://gox.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://kqk.sweek.top

[T27] Swift：错误处理
来源：http://cjo.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://bix.tarul.cn

[T28] Swift：枚举
来源：http://oci.c1oappe.top

enum Color { case red, green }
来源：http://jmx.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://yzj.ehwqpu.com

guard let x = opt else { return }
来源：http://odx.chenlongwang.top

[T30] Swift：协议
来源：http://thc.cashguo.top

protocol Shape { func area() -> Double }
来源：http://man.quarkkingdee.top

[T31] Lua：Hello World
来源：http://zqx.yongpay.top

print("Hello")
来源：http://qex.zhengqikj.top

[T32] Lua：局部变量
来源：http://zvq.epnwcf.com

local a = 1
来源：http://tyq.aibaodan.cn

[T33] Lua：表（数组）
来源：http://bqv.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cxr.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://jmx.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://udu.gaohongyu789.top

[T35] Lua：字典表
来源：http://njh.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://wph.dashuyun.cn

[T36] Lua：函数
来源：http://zqi.gogol.net.cn

function add(a, b) return a + b end
来源：http://aoy.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://joi.9152youxi.cn

"a" .. "b"
来源：http://jqe.9152youxi.cn

[T38] Lua：条件
来源：http://gwr.yfazqb.com

if x > 0 then print("正") end
来源：http://udw.vehdjk.com

[T39] Lua：模式匹配
来源：http://ppf.shuidangran.top

string.find(s, "%d+")
来源：http://uvu.zdbjq.cn

[T40] Lua：元表
来源：http://tdu.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://eym.sweek.top

[T41] Perl：Hello World
来源：http://giq.yuxming.cn

print "Hello\n";
来源：http://akw.sysykeji.top

[T42] Perl：变量类型
来源：http://zlk.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yno.bjfxy.top

[T43] Perl：字符串插值
来源：http://lel.jianghu66.top

"值: $a"
来源：http://jyw.zhongyouzk.top

[T44] Perl：条件
来源：http://kcq.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://tfw.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://icb.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://gwn.ybcxt.top

[T46] Perl：哈希操作
来源：http://bko.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ank.svipenyu.cn

[T47] Perl：正则捕获
来源：http://lyh.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://sfu.epnwcf.com

[T48] Perl：正则替换
来源：http://xzh.sysykeji.top

$s =~ s/old/new/g;
来源：http://daq.chenjidiqi.icu

[T49] Perl：函数
来源：http://huf.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pyk.c1oappe.top

[T50] Perl：逐行读文件
来源：http://crv.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pyw.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://qcb.yongpay.top

[T51] Scala：Hello World
来源：http://uey.cucudq.cn

println("Hello")
来源：http://qio.gaohongyu789.top

[T52] Scala：变量
来源：http://kje.aizwys.cn

val a = 1;  var b = 2
来源：http://qsn.zhengqikj.top

[T53] Scala：字符串插值
来源：http://dws.chenzaomai.com

s"值: $b"
来源：http://wfu.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://via.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://dvo.cucudq.cn

[T55] Scala：集合过滤
来源：http://ltq.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://xct.epnwcf.com

[T56] Scala：样例类
来源：http://fvd.xziqi.cn

case class User(name: String, age: Int)
来源：http://pze.jianghu66.top

[T57] Scala：模式匹配
来源：http://aoz.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://agn.daxiang520.top

[T58] Scala：函数定义
来源：http://uhn.sysykeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://cgv.fktsv.cn

[T59] Scala：循环
来源：http://ciw.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://cec.nanxinkj.top

[T60] Scala：折叠
来源：http://wov.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dis.jqgufenzy.top

================================================================================
来源：http://xso.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pxe.jqgfzy.top

================================================================================
来源：http://ciq.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://gzl.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://vkj.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://oot.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dum.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://kfl.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ria.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://yne.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://znw.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://gib.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://xin.yj20258.top

[U06] Py：合并两个字典
来源：http://bok.gotoacloud.top

{**a, **b}
来源：http://hbv.yuxming.cn

[U07] Py：反转字典键值
来源：http://jem.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://lqa.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://qgp.fzhhl.top

[y for x in nested for y in x]
来源：http://uaw.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://apz.0kj1m.cn

max(d, key=d.get)
来源：http://rvr.yuanzhike.top

[U10] Py：按值排序字典
来源：http://wpo.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zpd.iojbl.cn

[U11] Py：生成器表达式
来源：http://fsi.dashuyun.cn

(x * 2 for x in arr)
来源：http://xwj.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://pov.cashguo.top

Counter(arr).most_common(3)
来源：http://ezt.316326.xyz

[U13] Py：固定长度队列
来源：http://tyt.jinqigfzy.top

deque(maxlen=10)
来源：http://jlu.fzhhl.top

[U14] Py：分组收集到列表
来源：http://lvv.wangshuangyany.cn

defaultdict(list)
来源：http://pem.snrcjt.cn

[U15] Py：高精度计时
来源：http://hst.xylfe.cn

t = time.perf_counter()
来源：http://kuw.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://uyy.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pop.0kj1m.cn

[U17] Py：初始化日志
来源：http://nxg.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://xpe.fzhhl.top

[U18] Py：预编译正则
来源：http://sle.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://jnr.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://ywo.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mty.daxiang520.top

[U20] Py：缓存函数结果
来源：http://wjh.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://gip.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://vsg.xuanzx.com

@contextlib.contextmanager
来源：http://gxd.tianlin.xyz

[U22] Py：矩阵转置
来源：http://key.gzhubu.top

list(zip(*m))
来源：http://zqy.guannengcc.top

[U23] Py：分块读取大文件
来源：http://kta.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yab.yonumen.top

[U24] Py：路径操作
来源：http://fxq.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xdk.feifeiyinyue.top

[U25] Py：CSV 按字典读
来源：http://cvq.yonumen.top

csv.DictReader(f)
来源：http://ska.tian-w.cn

[U26] Py：并发下载
来源：http://vfw.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qtz.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://adq.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://lwr.epnwcf.com

[U28] Py：类型别名
来源：http://umr.yvedp.cn

UserId = int
来源：http://sbu.yfazqb.com

[U29] Py：属性校验
来源：http://pho.hfpthk.cn

@property 与 @x.setter 配合
来源：http://zos.mhx1999.top

[U30] Py：数据类
来源：http://rob.ctjpmb.com

@dataclass(slots=True)
来源：http://nfz.ctjpmb.com


<!-- 参考信息 -->