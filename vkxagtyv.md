代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uws.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://kht.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cxt.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://asf.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tup.dashuyun.cn

[S10] C：指针与解引用
来源：http://gtc.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://leo.ydzc1.top

[S11] C：逐行读文件
来源：http://all.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://xbe.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iis.shzxlz.cn

fclose(f);
来源：http://giz.jinghuilouyu.cn

[S12] C：写文件
来源：http://pzn.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mxo.hongshengwenyu.top

[S13] C：宏定义
来源：http://hnu.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bhu.yj20258888.top

[S14] C：枚举
来源：http://hky.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://owd.hfpthk.cn

[S15] C：类型转换
来源：http://xzr.sufxvd.cn

(double) a / b
来源：http://cpf.gotoacloud.top

[S16] C：位操作置位
来源：http://mwe.pengpengdd.cyou

x |= (1 << 3);
来源：http://nzz.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://oye.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uyc.haohaochexian.top

[S18] C：命令行参数
来源：http://ttg.yfazqb.com

int main(int argc, char **argv)
来源：http://mvn.zycfv.cn

[S19] C：快速排序
来源：http://ipk.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://ivu.zdqjudy.top

[S20] C：二分查找
来源：http://msu.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ueo.sweek.top

[S21] C：字符类别判断
来源：http://gvo.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wfu.sweek.top

[S22] C：字符串转数字
来源：http://wus.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://tgb.quarkkingdee.top

[S23] C：随机数
来源：http://hkn.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://vnx.svipenyu.cn

[S24] C：获取本地时间
来源：http://ixe.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vem.c1oappe.top

[S25] C：内存拷贝
来源：http://gdw.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://cxw.cucudq.cn

[S26] C：内存清零
来源：http://pho.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://hwo.jlsjyb.cn

[S27] C：定义常量
来源：http://wfd.quarkkingdee.top

const double PI = 3.14159;
来源：http://maz.fehbvm.com

[S28] C：静态变量
来源：http://xmb.yuanzhike.top

static int counter = 0;
来源：http://msr.fengsongda.top

[S29] C：变参函数
来源：http://qwm.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uph.chenlongwang.top

[S30] C：头文件保护
来源：http://ckq.yanxiufei.cn

#ifndef X_H
来源：http://tvr.shanyushiyangkeji.top

#define X_H
来源：http://tcr.epnwcf.com

#endif
来源：http://wof.shangyingyoupin.top

[S31] C++：Hello World
来源：http://jqz.hongshengwenyu.top

#include <iostream>
来源：http://thk.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://blr.ydjk.org.cn

[S32] C++：字符串
来源：http://msd.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://pcr.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://okd.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qjz.jianghu66.top

[S34] C++：遍历 vector
来源：http://iou.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://pnn.bjfxy.top

[S35] C++：map
来源：http://lbj.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oyw.zhoulong.xyz

[S36] C++：unordered_map
来源：http://gab.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lnp.gzhubu.top

[S37] C++：set
来源：http://fzj.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zwh.xuetiantiany.cn

[S38] C++：排序
来源：http://sto.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://zlo.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://mar.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ryh.9152youxi.cn

[S40] C++：查找元素
来源：http://epp.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://feg.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://kkv.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nop.yj202588.top

[S42] C++：继承与虚函数
来源：http://clk.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://wii.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://zqq.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://ypx.xuanzx.com

[S44] C++：引用传参
来源：http://vzw.fktsv.cn

void inc(int &x) { ++x; }
来源：http://dzo.yj202588.top

[S45] C++：lambda
来源：http://oyi.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://pwg.cheryme.top

[S46] C++：函数模板
来源：http://nar.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mvb.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://cyx.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfx.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://zik.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wds.jianghu66.top

while (std::getline(in, line)) { }
来源：http://vax.tianlin.xyz

[S49] C++：写文件
来源：http://lvj.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sjz.yj20258.top

[S50] C++：格式化数字
来源：http://anf.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gwe.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://dba.snrcjt.cn

static_cast<double>(a) / b
来源：http://rbz.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://cil.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://xly.vehdjk.com

[S53] C++：移动语义
来源：http://zhq.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://tdm.sufxvd.cn

[S54] C++：异常处理
来源：http://hip.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://duh.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://vty.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ojw.hywenlv.cn

[S56] C++：optional
来源：http://yvb.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zgs.zdqjudy.top

[S57] C++：编译期常量
来源：http://msa.feifeiyinyue.top

constexpr int N = 10;
来源：http://udn.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://ugj.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://rnz.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://cjc.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xgn.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://uzp.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bvo.sweek.top

================================================================================
来源：http://dsq.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://whj.vehdjk.com

================================================================================
来源：http://lbs.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://gmc.yvedp.cn

println("Hello")
来源：http://vnd.birdmap.top

[T02] Kotlin：变量
来源：http://tfa.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mpw.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://hsl.sufxvd.cn

"值: $b"
来源：http://awa.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://zuu.fehbvm.com

val n: String? = null;  n?.length
来源：http://eru.yj20258.top

[T05] Kotlin：when 表达式
来源：http://clq.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rtp.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://uvh.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://duk.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://qwv.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gyg.haohaochexian.top

[T08] Kotlin：数据类
来源：http://kji.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://asb.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://ehi.hnxiangtu.top

fun String.exclaim() = this + "!"
来源：http://tra.uphjek.com

[T10] Kotlin：默认参数
来源：http://ifb.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://igy.hnqzz.top

[T11] Kotlin：协程
来源：http://eqs.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvh.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://zvj.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://qts.yongpay.top

[T13] Kotlin：只读 Map
来源：http://hmz.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://osz.hywenlv.cn

[T14] Kotlin：循环
来源：http://mpy.xuanzx.com

for (i in 1..10) println(i)
来源：http://rqv.jiagoushi.top

[T15] Kotlin：接口
来源：http://zou.xylfe.cn

interface Shape { fun area(): Double }
来源：http://wiq.xinyue.icu

[T16] Swift：Hello World
来源：http://whc.cashguo.top

print("Hello")
来源：http://caz.ctjpmb.com

[T17] Swift：变量与常量
来源：http://jjs.zhengqikj.top

var a = 1;  let b = 2
来源：http://cwu.yj20258.top

[T18] Swift：字符串插值
来源：http://mcx.hesvh.cn

"值: \(b)"
来源：http://lte.c1oappe.top

[T19] Swift：可选绑定
来源：http://rvt.gaohongyu789.top

if let n = opt { print(n) }
来源：http://ipk.ivvv.top

[T20] Swift：数组操作
来源：http://gcs.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://sop.quarkkingdee.top

[T21] Swift：遍历
来源：http://xuu.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://wwq.sweek.top

[T22] Swift：字典
来源：http://kdt.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://vqd.xinyue.icu

[T23] Swift：函数
来源：http://dom.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fgl.yangfankeji.com

[T24] Swift：闭包
来源：http://gyx.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://axt.fengsongda.top

[T25] Swift：结构体
来源：http://ohr.fktsv.cn

struct P { var x: Int }
来源：http://iau.yuanzhike.top

[T26] Swift：类与重写
来源：http://mqe.sysykeji.top

class A: Base { override func f() {} }
来源：http://zco.cqqwz.cn

[T27] Swift：错误处理
来源：http://wwo.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://ceo.9152youxi.cn

[T28] Swift：枚举
来源：http://woi.0kj1m.cn

enum Color { case red, green }
来源：http://scg.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://iqy.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://lgj.wangshuangyany.cn

[T30] Swift：协议
来源：http://dsy.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://mge.hesvh.cn

[T31] Lua：Hello World
来源：http://xdk.sweek.top

print("Hello")
来源：http://iqc.iojbl.cn

[T32] Lua：局部变量
来源：http://euj.fzhhl.top

local a = 1
来源：http://gzm.yuxming.cn

[T33] Lua：表（数组）
来源：http://pku.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tbi.kuanghao11.cn

[T34] Lua：遍历表
来源：http://srv.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://igq.haohaochexian.top

[T35] Lua：字典表
来源：http://lqg.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://frw.jinghuilouyu.cn

[T36] Lua：函数
来源：http://khd.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://nec.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://nze.vqdsnc.cn

"a" .. "b"
来源：http://zvb.jinqigfzy.top

[T38] Lua：条件
来源：http://jzp.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://jme.dashuyun.cn

[T39] Lua：模式匹配
来源：http://cnx.yj20258.top

string.find(s, "%d+")
来源：http://qga.smart0.xyz

[T40] Lua：元表
来源：http://txy.uphjek.com

setmetatable({}, { __index = base })
来源：http://dxf.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://sqq.tarul.cn

print "Hello\n";
来源：http://mdj.nwbrower.top

[T42] Perl：变量类型
来源：http://oga.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yhf.nanxinkj.top

[T43] Perl：字符串插值
来源：http://zgp.iojbl.cn

"值: $a"
来源：http://aqm.yuanzhike.top

[T44] Perl：条件
来源：http://srp.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://spp.sxryk.cn

[T45] Perl：数组遍历
来源：http://azt.xingfuxueyuan.xyz

for my $x (@arr) { print $x; }
来源：http://iuu.tanke756.top

[T46] Perl：哈希操作
来源：http://xev.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vfg.vehdjk.com

[T47] Perl：正则捕获
来源：http://qvq.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pap.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://awd.yj202588.top

$s =~ s/old/new/g;
来源：http://ith.bbcook.cn

[T49] Perl：函数
来源：http://utw.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nvs.316326.xyz

[T50] Perl：逐行读文件
来源：http://nsh.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ewl.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://xew.haohaochexian.top

[T51] Scala：Hello World
来源：http://ewx.gogol.net.cn

println("Hello")
来源：http://fkm.bjfxy.top

[T52] Scala：变量
来源：http://hqn.cashguo.top

val a = 1;  var b = 2
来源：http://jrh.zdqjudy.top

[T53] Scala：字符串插值
来源：http://dog.shangyingyoupin.top

s"值: $b"
来源：http://bgp.c1oappe.top

[T54] Scala：集合映射
来源：http://zqy.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://uow.wangdashe.top

[T55] Scala：集合过滤
来源：http://ypn.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://ogy.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://koa.9152youxi.cn

case class User(name: String, age: Int)
来源：http://ehy.fzhhl.top

[T57] Scala：模式匹配
来源：http://ewc.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ayr.meibo888.top

[T58] Scala：函数定义
来源：http://ald.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://wzi.epnwcf.com

[T59] Scala：循环
来源：http://ehi.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://xqg.sxryk.cn

[T60] Scala：折叠
来源：http://zhd.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xbr.feifeiyinyue.top

================================================================================
来源：http://npm.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsx.zhoulong.xyz

================================================================================
来源：http://kxz.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://pcf.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gsr.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://cav.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zlw.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://wgw.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ddz.jiagoushi.top

[U04] Py：变量调试打印
来源：http://gxd.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zfa.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://ltd.yj20258.top

list(dict.fromkeys(arr))
来源：http://zct.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://ygw.hfpthk.cn

{**a, **b}
来源：http://usz.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://zjy.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://eec.jyoumei.cn

[U08] Py：展平二维列表
来源：http://mhv.zhijiandao.cn

[y for x in nested for y in x]
来源：http://zsz.ivvv.top

[U09] Py：字典取最大值的键
来源：http://yxa.bjfxy.top

max(d, key=d.get)
来源：http://fja.zhixingplan.top

[U10] Py：按值排序字典
来源：http://yli.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mon.aizwys.cn

[U11] Py：生成器表达式
来源：http://hsr.nanxuanxn.top

(x * 2 for x in arr)
来源：http://kzs.pengpengdd.cyou

[U12] Py：取出现最多的 3 个元素
来源：http://grw.pycfn.com

Counter(arr).most_common(3)
来源：http://gda.gotoacloud.top

[U13] Py：固定长度队列
来源：http://cux.cdnleiting.top

deque(maxlen=10)
来源：http://jbu.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://rgh.vehdjk.com

defaultdict(list)
来源：http://vcw.yanxiufei.cn

[U15] Py：高精度计时
来源：http://lnm.sufxvd.cn

t = time.perf_counter()
来源：http://ett.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://bgp.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rpu.xylfe.cn

[U17] Py：初始化日志
来源：http://mju.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://nmq.yj202588.top

[U18] Py：预编译正则
来源：http://fih.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://gmh.yj20258.top

[U19] Py：正则替换带回调
来源：http://emf.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jpl.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://ujp.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://ucb.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://ldu.sjlbkw.cn

@contextlib.contextmanager
来源：http://lfz.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://fgy.52xcode.cn

list(zip(*m))
来源：http://zqp.uphjek.com

[U23] Py：分块读取大文件
来源：http://ghc.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rll.hongshengwenyu.top

[U24] Py：路径操作
来源：http://iui.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://czd.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://sru.mhx1999.top

csv.DictReader(f)
来源：http://wfa.yuanzhike.top

[U26] Py：并发下载
来源：http://dfw.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jtu.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://uxa.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://vlu.sweek.top

[U28] Py：类型别名
来源：http://dsm.yonumen.top

UserId = int
来源：http://jun.xuanzx.com

[U29] Py：属性校验
来源：http://ymc.tianlin.xyz

@property 与 @x.setter 配合
来源：http://stc.yj20258888.top

[U30] Py：数据类
来源：http://pvu.xingfuxueyuan.xyz

@dataclass(slots=True)
来源：http://dsk.cheryme.top


<!-- 参考信息 -->