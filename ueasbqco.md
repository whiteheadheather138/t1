代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mgy.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://ucw.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wul.pycfn.com

[S09] C：结构体定义与初始化
来源：http://zyk.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zqu.52xcode.cn

[S10] C：指针与解引用
来源：http://rve.yj20258888.top

int *p = &a;  *p = 5;
来源：http://ahg.zhixingplan.top

[S11] C：逐行读文件
来源：http://pbg.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://lwj.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://mvy.feifeiyinyue.top

fclose(f);
来源：http://yis.hammf.cn

[S12] C：写文件
来源：http://cpa.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nyi.c1oappe.top

[S13] C：宏定义
来源：http://uih.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dcq.dianchejie.cn

[S14] C：枚举
来源：http://tmv.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://yty.jianghu66.top

[S15] C：类型转换
来源：http://jdj.tarul.cn

(double) a / b
来源：http://hvt.wangshuangyany.cn

[S16] C：位操作置位
来源：http://fel.xinyue.icu

x |= (1 << 3);
来源：http://dus.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://evc.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bwy.sysykeji.top

[S18] C：命令行参数
来源：http://rye.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://drf.0kj1m.cn

[S19] C：快速排序
来源：http://akz.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ksv.jqgufenzy.top

[S20] C：二分查找
来源：http://aum.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zwa.zycfv.cn

[S21] C：字符类别判断
来源：http://qaj.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bds.zhijiandao.cn

[S22] C：字符串转数字
来源：http://klj.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://std.sxryk.cn

[S23] C：随机数
来源：http://kjn.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://puu.kuanghao11.cn

[S24] C：获取本地时间
来源：http://brt.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rey.cqqwz.cn

[S25] C：内存拷贝
来源：http://xfo.jlsjyb.cn

memcpy(dst, src, n);
来源：http://dqc.hcnkem.com

[S26] C：内存清零
来源：http://fhk.jianghu66.top

memset(a, 0, sizeof a);
来源：http://mwl.cdnleiting.top

[S27] C：定义常量
来源：http://jhr.yj20258.top

const double PI = 3.14159;
来源：http://die.gzhubu.top

[S28] C：静态变量
来源：http://rbm.fzhhl.top

static int counter = 0;
来源：http://mux.hywenlv.cn

[S29] C：变参函数
来源：http://lrm.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uqx.yvedp.cn

[S30] C：头文件保护
来源：http://jnj.fzhhl.top

#ifndef X_H
来源：http://bmf.iojbl.cn

#define X_H
来源：http://cva.wangdashe.top

#endif
来源：http://woy.shangyingyoupin.top

[S31] C++：Hello World
来源：http://foo.dianchejie.cn

#include <iostream>
来源：http://zib.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://chg.hnxiangtu.top

[S32] C++：字符串
来源：http://jjl.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://asg.zhongyouzk.top

[S33] C++：vector 增删
来源：http://ngy.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gmc.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://nnb.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://fch.hywenlv.cn

[S35] C++：map
来源：http://nsx.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oqz.snrcjt.cn

[S36] C++：unordered_map
来源：http://prq.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pfk.nanxinkj.top

[S37] C++：set
来源：http://fhe.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hqq.mhx1999.top

[S38] C++：排序
来源：http://hii.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://fan.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://zpf.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhl.bjfxy.top

[S40] C++：查找元素
来源：http://fwc.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://stq.chenlongwang.top

[S41] C++：类与构造函数
来源：http://gbn.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wxq.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://niv.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://fyf.zhengqikj.top

[S43] C++：智能指针
来源：http://hhs.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://vnd.zdqjudy.top

[S44] C++：引用传参
来源：http://llq.tanke756.top

void inc(int &x) { ++x; }
来源：http://rfc.xuetiantiany.cn

[S45] C++：lambda
来源：http://okp.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://mge.jianghu66.top

[S46] C++：函数模板
来源：http://qdn.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://utw.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://yef.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rux.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://hxc.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ven.52xcode.cn

while (std::getline(in, line)) { }
来源：http://bjm.jinqigufen.top

[S49] C++：写文件
来源：http://jsa.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ydk.sjlbkw.cn

[S50] C++：格式化数字
来源：http://hvz.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hvr.nanxinkj.top

[S51] C++：显式类型转换
来源：http://ssq.52xcode.cn

static_cast<double>(a) / b
来源：http://hxa.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://bth.meibo888.top

int size() const noexcept { return n_; }
来源：http://sgi.xziqi.cn

[S53] C++：移动语义
来源：http://zeb.cashguo.top

std::vector<int> w = std::move(v);
来源：http://akr.c1oappe.top

[S54] C++：异常处理
来源：http://gbm.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqj.jiagoushi.top

[S55] C++：结构化绑定
来源：http://xma.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vvt.gotoacloud.top

[S56] C++：optional
来源：http://zdx.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ehz.ppjwa.cn

[S57] C++：编译期常量
来源：http://qtc.chenzaomai.com

constexpr int N = 10;
来源：http://inx.jinqigfzy.top

[S58] C++：命名空间
来源：http://jte.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://tht.vqdsnc.cn

[S59] C++：静态断言
来源：http://exh.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://too.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://bnn.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmr.yangfankeji.com

================================================================================
来源：http://meb.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://unn.ydzc1.top

================================================================================
来源：http://ygg.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://ndi.mhx1999.top

println("Hello")
来源：http://myg.zhengqikj.top

[T02] Kotlin：变量
来源：http://hrf.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rbg.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://gae.jinqigufen.top

"值: $b"
来源：http://onn.hcnkem.com

[T04] Kotlin：空安全
来源：http://yzl.yongpay.top

val n: String? = null;  n?.length
来源：http://qxx.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://eej.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rqu.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://byn.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://miv.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://lbd.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pdq.hammf.cn

[T08] Kotlin：数据类
来源：http://jhj.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://mjn.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://vjr.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://hvb.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://rgx.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nrh.fengsongda.top

[T11] Kotlin：协程
来源：http://agu.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jsz.yvedp.cn

[T12] Kotlin：解构声明
来源：http://bvc.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://dnz.hammf.cn

[T13] Kotlin：只读 Map
来源：http://qaq.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://stg.sxryk.cn

[T14] Kotlin：循环
来源：http://orx.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://uqp.ppjwa.cn

[T15] Kotlin：接口
来源：http://bbh.redwolf501.top

interface Shape { fun area(): Double }
来源：http://aju.shuidangran.top

[T16] Swift：Hello World
来源：http://alu.bbcook.cn

print("Hello")
来源：http://kre.wangdashe.top

[T17] Swift：变量与常量
来源：http://zvx.sxryk.cn

var a = 1;  let b = 2
来源：http://ybq.sufxvd.cn

[T18] Swift：字符串插值
来源：http://xjl.hywenlv.cn

"值: \(b)"
来源：http://ala.316326.xyz

[T19] Swift：可选绑定
来源：http://ema.gaohongyu789.top

if let n = opt { print(n) }
来源：http://eia.fzhhl.top

[T20] Swift：数组操作
来源：http://hup.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wbk.jyoumei.cn

[T21] Swift：遍历
来源：http://cyq.yongpay.top

for x in a { print(x) }
来源：http://rqz.shuidangran.top

[T22] Swift：字典
来源：http://jbc.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://cmo.gaohongyu789.top

[T23] Swift：函数
来源：http://ebi.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bfc.yj20258.top

[T24] Swift：闭包
来源：http://zgu.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jgy.dashuyun.cn

[T25] Swift：结构体
来源：http://dax.mhx1999.top

struct P { var x: Int }
来源：http://ima.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://hem.svipenyu.cn

class A: Base { override func f() {} }
来源：http://mky.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://bnv.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://qgl.gotoacloud.top

[T28] Swift：枚举
来源：http://obg.hesvh.cn

enum Color { case red, green }
来源：http://pdu.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://ccg.tian-w.cn

guard let x = opt else { return }
来源：http://ghu.jyoumei.cn

[T30] Swift：协议
来源：http://nrl.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://bcn.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://hti.haohaochexian.top

print("Hello")
来源：http://sgj.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://udv.shuidangran.top

local a = 1
来源：http://rsb.gotoacloud.top

[T33] Lua：表（数组）
来源：http://lrp.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jxg.yj20258888.top

[T34] Lua：遍历表
来源：http://zwq.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://wvm.sufxvd.cn

[T35] Lua：字典表
来源：http://yvt.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ehe.andypj.xyz

[T36] Lua：函数
来源：http://lhq.redwolf501.top

function add(a, b) return a + b end
来源：http://lxl.fengsongda.top

[T37] Lua：字符串拼接
来源：http://szf.hnxiangtu.top

"a" .. "b"
来源：http://hsm.chenzaomai.com

[T38] Lua：条件
来源：http://myk.yuanzhike.top

if x > 0 then print("正") end
来源：http://izu.xinyue.icu

[T39] Lua：模式匹配
来源：http://sme.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://zie.feifeiyinyue.top

[T40] Lua：元表
来源：http://sjz.cashguo.top

setmetatable({}, { __index = base })
来源：http://dco.hcnkem.com

[T41] Perl：Hello World
来源：http://vrq.yonumen.top

print "Hello\n";
来源：http://akx.uphjek.com

[T42] Perl：变量类型
来源：http://emk.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gfx.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://fkn.zycfv.cn

"值: $a"
来源：http://vdp.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://yfi.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://xtc.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://qyl.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://fnz.jinqigufen.top

[T46] Perl：哈希操作
来源：http://maf.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tah.daxiang520.top

[T47] Perl：正则捕获
来源：http://mfv.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ths.9152youxi.cn

[T48] Perl：正则替换
来源：http://gcn.gzhubu.top

$s =~ s/old/new/g;
来源：http://imt.shanyushiyangtech.top

[T49] Perl：函数
来源：http://uhz.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xbo.mhx1999.top

[T50] Perl：逐行读文件
来源：http://qxm.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zgn.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://lhq.zycfv.cn

[T51] Scala：Hello World
来源：http://lau.shuidangran.top

println("Hello")
来源：http://eoc.yj202588.top

[T52] Scala：变量
来源：http://ryo.jyoumei.cn

val a = 1;  var b = 2
来源：http://bnf.yj20258888.top

[T53] Scala：字符串插值
来源：http://apd.svipenyu.cn

s"值: $b"
来源：http://kcl.xuanzx.com

[T54] Scala：集合映射
来源：http://ywc.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://spy.zhixingplan.top

[T55] Scala：集合过滤
来源：http://ssn.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://tdg.hnqzz.top

[T56] Scala：样例类
来源：http://khq.sufxvd.cn

case class User(name: String, age: Int)
来源：http://kyi.svipenyu.cn

[T57] Scala：模式匹配
来源：http://wpv.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kna.vehdjk.com

[T58] Scala：函数定义
来源：http://now.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://eoq.dianchejie.cn

[T59] Scala：循环
来源：http://mmf.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://qxw.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://dwq.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wii.hcnkem.com

================================================================================
来源：http://fcy.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dvf.xuetiantiany.cn

================================================================================
来源：http://evy.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://vmq.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wye.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://iun.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ikh.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://qkk.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jek.hnqzz.top

[U04] Py：变量调试打印
来源：http://lot.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://anr.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://vtc.c1oappe.top

list(dict.fromkeys(arr))
来源：http://alt.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://ugi.ctjpmb.com

{**a, **b}
来源：http://zvk.hfpthk.cn

[U07] Py：反转字典键值
来源：http://yok.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://cjw.ydzc1.top

[U08] Py：展平二维列表
来源：http://sas.fengsongda.top

[y for x in nested for y in x]
来源：http://hkc.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://fot.hywenlv.cn

max(d, key=d.get)
来源：http://lak.tian-w.cn

[U10] Py：按值排序字典
来源：http://pun.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pyo.fzhhl.top

[U11] Py：生成器表达式
来源：http://koo.fengsongda.top

(x * 2 for x in arr)
来源：http://iqy.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://jmh.dianchejie.cn

Counter(arr).most_common(3)
来源：http://ikv.316326.xyz

[U13] Py：固定长度队列
来源：http://rtn.0kj1m.cn

deque(maxlen=10)
来源：http://evb.uphjek.com

[U14] Py：分组收集到列表
来源：http://fmu.yvedp.cn

defaultdict(list)
来源：http://liw.tarul.cn

[U15] Py：高精度计时
来源：http://dlp.fktsv.cn

t = time.perf_counter()
来源：http://uot.hnqzz.top

[U16] Py：命令行参数解析
来源：http://qvt.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mwg.316326.xyz

[U17] Py：初始化日志
来源：http://svd.redwolf501.top

logging.basicConfig(level=logging.INFO)
来源：http://epc.havefunace.top

[U18] Py：预编译正则
来源：http://nic.aizwys.cn

pat = re.compile(r"\d+")
来源：http://oqp.iojbl.cn

[U19] Py：正则替换带回调
来源：http://ncr.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ayg.fzhhl.top

[U20] Py：缓存函数结果
来源：http://iga.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://hsy.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://izs.pengpengdd.cyou

@contextlib.contextmanager
来源：http://gpn.xylfe.cn

[U22] Py：矩阵转置
来源：http://ben.yanxiufei.cn

list(zip(*m))
来源：http://dol.yueranfly.top

[U23] Py：分块读取大文件
来源：http://lsj.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://maf.zhijiandao.cn

[U24] Py：路径操作
来源：http://dvj.yangfankeji.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kwv.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://oio.xinyue.icu

csv.DictReader(f)
来源：http://upr.xylfe.cn

[U26] Py：并发下载
来源：http://rnn.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fuw.epnwcf.com

[U27] Py：异步 HTTP
来源：http://kbs.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://orz.dianchejie.cn

[U28] Py：类型别名
来源：http://yib.pengpengdd.cyou

UserId = int
来源：http://ntl.shzxlz.cn

[U29] Py：属性校验
来源：http://klw.xziqi.cn

@property 与 @x.setter 配合
来源：http://viq.yongpay.top

[U30] Py：数据类
来源：http://fdf.nwbrower.top

@dataclass(slots=True)
来源：http://qmh.wangshuangyany.cn


<!-- 参考信息 -->