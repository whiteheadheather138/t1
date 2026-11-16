代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tqx.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://qgg.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yrt.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://eap.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gva.kuanghao11.cn

[S10] C：指针与解引用
来源：http://xfz.yj20258888.top

int *p = &a;  *p = 5;
来源：http://eto.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://ivf.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://ljv.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ucq.svipenyu.cn

fclose(f);
来源：http://flx.hywenlv.cn

[S12] C：写文件
来源：http://qex.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://khu.fzhhl.top

[S13] C：宏定义
来源：http://wqu.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rbh.chenlongwang.top

[S14] C：枚举
来源：http://tse.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://llb.yj20258888.top

[S15] C：类型转换
来源：http://klt.jyoumei.cn

(double) a / b
来源：http://wue.hongshengwenyu.top

[S16] C：位操作置位
来源：http://pcm.hongshengwenyu.top

x |= (1 << 3);
来源：http://ixa.uphjek.com

[S17] C：安全拼接字符串
来源：http://ato.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ltx.xuetiantiany.cn

[S18] C：命令行参数
来源：http://rlx.xziqi.cn

int main(int argc, char **argv)
来源：http://bfs.gogol.net.cn

[S19] C：快速排序
来源：http://msd.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://txj.wangdashe.top

[S20] C：二分查找
来源：http://rot.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ppf.sjlbkw.cn

[S21] C：字符类别判断
来源：http://lnw.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pxy.nanxuanxn.top

[S22] C：字符串转数字
来源：http://umu.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://cta.wangshuangyany.cn

[S23] C：随机数
来源：http://voo.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uhm.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://onj.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tcu.yj20258888.top

[S25] C：内存拷贝
来源：http://bpp.dashuyun.cn

memcpy(dst, src, n);
来源：http://dcz.wangdashe.top

[S26] C：内存清零
来源：http://hwq.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://mxm.jianghu66.top

[S27] C：定义常量
来源：http://gxf.cashguo.top

const double PI = 3.14159;
来源：http://qnv.wangdashe.top

[S28] C：静态变量
来源：http://kma.zhaomingkeji.xyz

static int counter = 0;
来源：http://ahh.guannengcc.top

[S29] C：变参函数
来源：http://kwy.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wqk.zhongyouzk.top

[S30] C：头文件保护
来源：http://izw.zycfv.cn

#ifndef X_H
来源：http://cog.jinqigufen.top

#define X_H
来源：http://bii.daria6918.cn

#endif
来源：http://tnp.hesvh.cn

[S31] C++：Hello World
来源：http://dzg.quarkkingdee.top

#include <iostream>
来源：http://edz.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://xlt.sufxvd.cn

[S32] C++：字符串
来源：http://fhg.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://eum.cdnleiting.top

[S33] C++：vector 增删
来源：http://ksq.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uze.ehwqpu.com

[S34] C++：遍历 vector
来源：http://jog.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://ekj.iojbl.cn

[S35] C++：map
来源：http://enx.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yqc.yj20258.top

[S36] C++：unordered_map
来源：http://ilt.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zcs.shanyushiyangtech.top

[S37] C++：set
来源：http://vyw.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqj.zhijiandao.cn

[S38] C++：排序
来源：http://shb.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://iee.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://een.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uyf.ybcxt.top

[S40] C++：查找元素
来源：http://zpy.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ofe.sweek.top

[S41] C++：类与构造函数
来源：http://xgh.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zgs.aizwys.cn

[S42] C++：继承与虚函数
来源：http://ugw.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://akh.jinqigufen.top

[S43] C++：智能指针
来源：http://fwf.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://wvp.yanxiufei.cn

[S44] C++：引用传参
来源：http://ryj.pycfn.com

void inc(int &x) { ++x; }
来源：http://das.nanxinkj.top

[S45] C++：lambda
来源：http://ptc.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://jaf.jinqigufen.top

[S46] C++：函数模板
来源：http://hdq.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cie.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://iny.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wmj.yongpay.top

[S48] C++：逐行读文件
来源：http://wzi.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sdd.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://pev.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://pvq.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ldr.hywenlv.cn

[S50] C++：格式化数字
来源：http://iir.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdb.meibo888.top

[S51] C++：显式类型转换
来源：http://bti.jinqigfzy.top

static_cast<double>(a) / b
来源：http://mcv.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://uqr.redwolf501.top

int size() const noexcept { return n_; }
来源：http://zwi.ctjpmb.com

[S53] C++：移动语义
来源：http://nxi.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://coh.jiagoushi.top

[S54] C++：异常处理
来源：http://mbn.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ifz.aibaodan.cn

[S55] C++：结构化绑定
来源：http://nuv.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xav.sweek.top

[S56] C++：optional
来源：http://chp.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://woj.zhijiandao.cn

[S57] C++：编译期常量
来源：http://els.ehwqpu.com

constexpr int N = 10;
来源：http://ozm.xylfe.cn

[S58] C++：命名空间
来源：http://ujc.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://ijg.birdmap.top

[S59] C++：静态断言
来源：http://bkq.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hqn.cheryme.top

[S60] C++：遍历并删除元素
来源：http://xxz.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbd.shuidangran.top

================================================================================
来源：http://uax.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fec.zhaomingkeji.xyz

================================================================================
来源：http://hmp.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://ubf.0kj1m.cn

println("Hello")
来源：http://bze.hnxiangtu.top

[T02] Kotlin：变量
来源：http://naz.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ypo.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://xhy.zhoulong.xyz

"值: $b"
来源：http://vwz.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://glv.sweek.top

val n: String? = null;  n?.length
来源：http://grn.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://tqr.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxu.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://grq.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xjp.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://hmi.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tgm.pycfn.com

[T08] Kotlin：数据类
来源：http://ost.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://iub.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://asv.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://lop.cashguo.top

[T10] Kotlin：默认参数
来源：http://ism.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ven.xylfe.cn

[T11] Kotlin：协程
来源：http://ryx.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tzi.tian-w.cn

[T12] Kotlin：解构声明
来源：http://gfp.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://nng.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://hdc.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://bll.yangfankeji.com

[T14] Kotlin：循环
来源：http://dhp.hammf.cn

for (i in 1..10) println(i)
来源：http://uis.hysaishi.cn

[T15] Kotlin：接口
来源：http://tiy.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://ded.epnwcf.com

[T16] Swift：Hello World
来源：http://jhb.xinyue.icu

print("Hello")
来源：http://pdv.svipenyu.cn

[T17] Swift：变量与常量
来源：http://flx.xinyue.icu

var a = 1;  let b = 2
来源：http://vsl.vehdjk.com

[T18] Swift：字符串插值
来源：http://mbm.haohaochexian.top

"值: \(b)"
来源：http://gbr.cheryme.top

[T19] Swift：可选绑定
来源：http://oit.gzhubu.top

if let n = opt { print(n) }
来源：http://jtc.ydzc1.top

[T20] Swift：数组操作
来源：http://rti.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://wfu.ydzc1.top

[T21] Swift：遍历
来源：http://bjd.smart0.xyz

for x in a { print(x) }
来源：http://xok.vehdjk.com

[T22] Swift：字典
来源：http://reo.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://brr.sweek.top

[T23] Swift：函数
来源：http://zro.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nfw.sysykeji.top

[T24] Swift：闭包
来源：http://jys.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zgo.gogol.net.cn

[T25] Swift：结构体
来源：http://fzs.daxiang520.top

struct P { var x: Int }
来源：http://wjn.shuidangran.top

[T26] Swift：类与重写
来源：http://snv.ydzc1.top

class A: Base { override func f() {} }
来源：http://zpe.cucudq.cn

[T27] Swift：错误处理
来源：http://whw.redwolf501.top

do { try f() } catch { print(error) }
来源：http://cjl.xziqi.cn

[T28] Swift：枚举
来源：http://eya.tianlin.xyz

enum Color { case red, green }
来源：http://gkm.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://yhj.gaohongyu789.top

guard let x = opt else { return }
来源：http://rjc.yfazqb.com

[T30] Swift：协议
来源：http://fkh.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://tam.daria6918.cn

[T31] Lua：Hello World
来源：http://nuw.yongpay.top

print("Hello")
来源：http://jcc.gotoacloud.top

[T32] Lua：局部变量
来源：http://bar.chenzaomai.com

local a = 1
来源：http://exx.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://rnq.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://byr.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://uyv.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dpa.daxiang520.top

[T35] Lua：字典表
来源：http://tdr.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://itp.daria6918.cn

[T36] Lua：函数
来源：http://auh.svipenyu.cn

function add(a, b) return a + b end
来源：http://wuv.ydzc1.top

[T37] Lua：字符串拼接
来源：http://vxs.0kj1m.cn

"a" .. "b"
来源：http://vch.hysaishi.cn

[T38] Lua：条件
来源：http://pyp.bbcook.cn

if x > 0 then print("正") end
来源：http://hbo.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://fzk.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://jjt.shzxlz.cn

[T40] Lua：元表
来源：http://kgn.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://nrb.sufxvd.cn

[T41] Perl：Hello World
来源：http://vfo.jinqigfzy.top

print "Hello\n";
来源：http://top.guowangkeji.top

[T42] Perl：变量类型
来源：http://ttv.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kgh.pycfn.com

[T43] Perl：字符串插值
来源：http://hem.haohaochexian.top

"值: $a"
来源：http://aje.jinqigfzy.top

[T44] Perl：条件
来源：http://kad.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://wqf.cashguo.top

[T45] Perl：数组遍历
来源：http://bjl.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://kmh.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://haq.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://snb.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://bhc.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xsf.zhengqikj.top

[T48] Perl：正则替换
来源：http://eoe.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wtf.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://nmj.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mzi.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://ecc.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ieg.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://tio.hywenlv.cn

[T51] Scala：Hello World
来源：http://smg.gogol.net.cn

println("Hello")
来源：http://gqs.jinqigfzy.top

[T52] Scala：变量
来源：http://fro.tian-w.cn

val a = 1;  var b = 2
来源：http://mic.ybcxt.top

[T53] Scala：字符串插值
来源：http://xpn.sweek.top

s"值: $b"
来源：http://xpi.uphjek.com

[T54] Scala：集合映射
来源：http://guo.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://ghx.birdmap.top

[T55] Scala：集合过滤
来源：http://vee.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://tsx.jiagoushi.top

[T56] Scala：样例类
来源：http://wll.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://ssa.tanke756.top

[T57] Scala：模式匹配
来源：http://shs.hnqzz.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rbi.fktsv.cn

[T58] Scala：函数定义
来源：http://smo.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zcb.zycfv.cn

[T59] Scala：循环
来源：http://bwc.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://vbh.sufxvd.cn

[T60] Scala：折叠
来源：http://rql.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aim.yfazqb.com

================================================================================
来源：http://jlg.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hda.jinyuanbaomall.cn

================================================================================
来源：http://lnr.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://qwv.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://had.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://pwb.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://usy.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://qvq.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tbg.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://bty.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://llr.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://kjb.bjfxy.top

list(dict.fromkeys(arr))
来源：http://zip.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://vkm.xingfuxueyuan.xyz

{**a, **b}
来源：http://fym.snrcjt.cn

[U07] Py：反转字典键值
来源：http://mmk.hesvh.cn

{v: k for k, v in d.items()}
来源：http://pkz.sxryk.cn

[U08] Py：展平二维列表
来源：http://asx.jianghu66.top

[y for x in nested for y in x]
来源：http://det.tarul.cn

[U09] Py：字典取最大值的键
来源：http://yxw.316326.xyz

max(d, key=d.get)
来源：http://hxg.hesvh.cn

[U10] Py：按值排序字典
来源：http://lbm.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vkr.yj202588.top

[U11] Py：生成器表达式
来源：http://nmx.shzxlz.cn

(x * 2 for x in arr)
来源：http://oki.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://gdu.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://gnj.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://isl.jiagoushi.top

deque(maxlen=10)
来源：http://kgz.havefunace.top

[U14] Py：分组收集到列表
来源：http://hfy.fengsongda.top

defaultdict(list)
来源：http://zmm.yj20258888.top

[U15] Py：高精度计时
来源：http://veg.yj20258.top

t = time.perf_counter()
来源：http://nhr.sysykeji.top

[U16] Py：命令行参数解析
来源：http://gow.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tcs.andypj.xyz

[U17] Py：初始化日志
来源：http://bmf.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://zbo.c1oappe.top

[U18] Py：预编译正则
来源：http://jkq.hnqzz.top

pat = re.compile(r"\d+")
来源：http://wzk.xinyue.icu

[U19] Py：正则替换带回调
来源：http://gbj.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lzy.hnqzz.top

[U20] Py：缓存函数结果
来源：http://pfn.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://mqs.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://hlb.xylfe.cn

@contextlib.contextmanager
来源：http://cuz.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://dxu.pycfn.com

list(zip(*m))
来源：http://ztv.316326.xyz

[U23] Py：分块读取大文件
来源：http://kgx.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tuj.nwbrower.top

[U24] Py：路径操作
来源：http://yhc.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vsc.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://fvi.jqgfzy.top

csv.DictReader(f)
来源：http://qyc.jinqigufen.top

[U26] Py：并发下载
来源：http://sne.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ztm.daria6918.cn

[U27] Py：异步 HTTP
来源：http://dsn.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://ffs.fanxiaobao.xyz

[U28] Py：类型别名
来源：http://evs.guannengcc.top

UserId = int
来源：http://fwn.guowangkeji.top

[U29] Py：属性校验
来源：http://wym.birdmap.top

@property 与 @x.setter 配合
来源：http://ibu.cucudq.cn

[U30] Py：数据类
来源：http://blg.daxiang520.top

@dataclass(slots=True)
来源：http://qvq.guowangkeji.top


<!-- 参考信息 -->