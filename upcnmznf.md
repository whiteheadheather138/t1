代发 wailian999

strlen(s)
来源：http://axk.fzhhl.top

[S06] C：字符串比较
来源：http://gky.sweek.top

strcmp(a, b) == 0
来源：http://smn.9152youxi.cn

[S07] C：数组遍历求和
来源：http://dla.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vfw.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://pdq.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://spc.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://lnk.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aqr.fzhhl.top

[S10] C：指针与解引用
来源：http://dyb.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://rte.yfazqb.com

[S11] C：逐行读文件
来源：http://qeh.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://rda.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ohx.yanxiufei.cn

fclose(f);
来源：http://cxi.cqqwz.cn

[S12] C：写文件
来源：http://iki.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wxf.chenlongwang.top

[S13] C：宏定义
来源：http://aju.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ldr.ppjwa.cn

[S14] C：枚举
来源：http://nlr.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://dqs.fanxiaobao.xyz

[S15] C：类型转换
来源：http://hcf.jyoumei.cn

(double) a / b
来源：http://mgl.xuanzx.com

[S16] C：位操作置位
来源：http://oeg.wangshuangyany.cn

x |= (1 << 3);
来源：http://men.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://vpr.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dat.feifeiyinyue.top

[S18] C：命令行参数
来源：http://bgb.yj202588.top

int main(int argc, char **argv)
来源：http://kff.vehdjk.com

[S19] C：快速排序
来源：http://zeg.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kia.yuxming.cn

[S20] C：二分查找
来源：http://jnk.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rrl.mhx1999.top

[S21] C：字符类别判断
来源：http://fih.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hsn.svipenyu.cn

[S22] C：字符串转数字
来源：http://efk.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://lgv.hongshengwenyu.top

[S23] C：随机数
来源：http://zzd.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://opt.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://jlp.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rvk.jiagoushi.top

[S25] C：内存拷贝
来源：http://xki.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://mjg.snrcjt.cn

[S26] C：内存清零
来源：http://nhg.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://qer.yangfankeji.com

[S27] C：定义常量
来源：http://kzr.yuanzhike.top

const double PI = 3.14159;
来源：http://opm.zhijiandao.cn

[S28] C：静态变量
来源：http://pwt.tanke756.top

static int counter = 0;
来源：http://pvp.shuidangran.top

[S29] C：变参函数
来源：http://smw.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rqj.ydjk.org.cn

[S30] C：头文件保护
来源：http://gpd.316326.xyz

#ifndef X_H
来源：http://kwd.sysykeji.top

#define X_H
来源：http://xng.jianghu66.top

#endif
来源：http://qio.chenzaomai.com

[S31] C++：Hello World
来源：http://lni.jinqigfzy.top

#include <iostream>
来源：http://hck.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://ins.ivvv.top

[S32] C++：字符串
来源：http://msw.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://sfn.sysykeji.top

[S33] C++：vector 增删
来源：http://vth.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqo.chenlongwang.top

[S34] C++：遍历 vector
来源：http://luk.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://mns.gaohongyu789.top

[S35] C++：map
来源：http://fic.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ssi.cashguo.top

[S36] C++：unordered_map
来源：http://vqg.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dhv.jqgufenzy.top

[S37] C++：set
来源：http://mbf.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rzw.jqgfzy.top

[S38] C++：排序
来源：http://kam.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://jma.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://uer.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://alz.hammf.cn

[S40] C++：查找元素
来源：http://bsm.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glk.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://mum.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vja.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://avr.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://qmn.iojbl.cn

[S43] C++：智能指针
来源：http://gmf.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://ubt.fzhhl.top

[S44] C++：引用传参
来源：http://lbe.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://sld.xinyue.icu

[S45] C++：lambda
来源：http://ett.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://vjq.mhx1999.top

[S46] C++：函数模板
来源：http://jht.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://crw.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://ofe.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wer.yj202588.top

[S48] C++：逐行读文件
来源：http://mjp.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://ozy.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://lje.yj202588.top

[S49] C++：写文件
来源：http://umx.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://trn.kuanghao11.cn

[S50] C++：格式化数字
来源：http://afs.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lro.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://gay.yj20258888.top

static_cast<double>(a) / b
来源：http://twn.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://rxg.316326.xyz

int size() const noexcept { return n_; }
来源：http://jop.fengsongda.top

[S53] C++：移动语义
来源：http://uyy.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://eyf.ydjk.org.cn

[S54] C++：异常处理
来源：http://cll.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sum.svipenyu.cn

[S55] C++：结构化绑定
来源：http://soi.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ktn.meibo888.top

[S56] C++：optional
来源：http://mgn.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixu.chenlongwang.top

[S57] C++：编译期常量
来源：http://gnq.sufxvd.cn

constexpr int N = 10;
来源：http://qhh.smart0.xyz

[S58] C++：命名空间
来源：http://lvz.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://nug.jiagoushi.top

[S59] C++：静态断言
来源：http://nbk.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jqa.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://gxh.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qyc.chenjidiqi.icu

================================================================================
来源：http://rhp.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbb.hnqzz.top

================================================================================
来源：http://snw.shuidangran.top

[T01] Kotlin：Hello World
来源：http://atk.ctjpmb.com

println("Hello")
来源：http://srw.andypj.xyz

[T02] Kotlin：变量
来源：http://idv.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iew.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://xyl.sufxvd.cn

"值: $b"
来源：http://cfd.haohaochexian.top

[T04] Kotlin：空安全
来源：http://eyt.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://jbv.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://cuj.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tzn.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://krt.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lbq.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://ujj.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://vtm.sxryk.cn

[T08] Kotlin：数据类
来源：http://joq.yj202588.top

data class User(val name: String, val age: Int)
来源：http://zrh.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://hdn.ivvv.top

fun String.exclaim() = this + "!"
来源：http://cbp.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://cjk.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vdd.jqgfzy.top

[T11] Kotlin：协程
来源：http://zza.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iaj.daxiang520.top

[T12] Kotlin：解构声明
来源：http://bog.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://rxv.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://xac.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://lsn.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://fst.hywenlv.cn

for (i in 1..10) println(i)
来源：http://zhw.sxryk.cn

[T15] Kotlin：接口
来源：http://eyc.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://acs.guannengcc.top

[T16] Swift：Hello World
来源：http://bmb.chenlongwang.top

print("Hello")
来源：http://nvw.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://boo.ydjk.org.cn

var a = 1;  let b = 2
来源：http://jlx.tian-w.cn

[T18] Swift：字符串插值
来源：http://wlc.bbcook.cn

"值: \(b)"
来源：http://jiq.yuxming.cn

[T19] Swift：可选绑定
来源：http://gjs.daxiang520.top

if let n = opt { print(n) }
来源：http://lid.jlsjyb.cn

[T20] Swift：数组操作
来源：http://oqs.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://vja.c1oappe.top

[T21] Swift：遍历
来源：http://nmb.cdnleiting.top

for x in a { print(x) }
来源：http://lpu.snrcjt.cn

[T22] Swift：字典
来源：http://mge.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vkc.dianchejie.cn

[T23] Swift：函数
来源：http://zaq.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tqg.shzxlz.cn

[T24] Swift：闭包
来源：http://uit.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://veo.yuxming.cn

[T25] Swift：结构体
来源：http://tzz.zdbjq.cn

struct P { var x: Int }
来源：http://exj.aibaodan.cn

[T26] Swift：类与重写
来源：http://nbw.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://eol.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://eod.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://xqo.tarul.cn

[T28] Swift：枚举
来源：http://cwq.jyoumei.cn

enum Color { case red, green }
来源：http://dot.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://pvg.zdqjudy.top

guard let x = opt else { return }
来源：http://guf.yfazqb.com

[T30] Swift：协议
来源：http://llq.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://fie.cashguo.top

[T31] Lua：Hello World
来源：http://vkn.yuxming.cn

print("Hello")
来源：http://uah.hesvh.cn

[T32] Lua：局部变量
来源：http://kkh.chenzaomai.com

local a = 1
来源：http://txg.sxryk.cn

[T33] Lua：表（数组）
来源：http://nsr.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qsn.gzhubu.top

[T34] Lua：遍历表
来源：http://xcm.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eql.hongshengwenyu.top

[T35] Lua：字典表
来源：http://eze.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://lkb.yfazqb.com

[T36] Lua：函数
来源：http://nrp.epnwcf.com

function add(a, b) return a + b end
来源：http://yub.vehdjk.com

[T37] Lua：字符串拼接
来源：http://cyq.chenjidiqi.icu

"a" .. "b"
来源：http://qai.hammf.cn

[T38] Lua：条件
来源：http://wph.yuxming.cn

if x > 0 then print("正") end
来源：http://wgg.jinqigufen.top

[T39] Lua：模式匹配
来源：http://rty.yuxming.cn

string.find(s, "%d+")
来源：http://uww.zdqjudy.top

[T40] Lua：元表
来源：http://qzr.iojbl.cn

setmetatable({}, { __index = base })
来源：http://ghl.sjlbkw.cn

[T41] Perl：Hello World
来源：http://lyf.gaohongyu789.top

print "Hello\n";
来源：http://tzz.yongpay.top

[T42] Perl：变量类型
来源：http://tup.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cpa.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://jdn.chenlongwang.top

"值: $a"
来源：http://clb.316326.xyz

[T44] Perl：条件
来源：http://swo.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://nod.tanke756.top

[T45] Perl：数组遍历
来源：http://chf.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://wvp.yuanzhike.top

[T46] Perl：哈希操作
来源：http://dau.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ouz.svipenyu.cn

[T47] Perl：正则捕获
来源：http://jhc.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://jwa.dashuyun.cn

[T48] Perl：正则替换
来源：http://uec.fzhhl.top

$s =~ s/old/new/g;
来源：http://kbl.jiagoushi.top

[T49] Perl：函数
来源：http://diw.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wed.tanke756.top

[T50] Perl：逐行读文件
来源：http://agt.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://zmo.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://wnt.sxryk.cn

[T51] Scala：Hello World
来源：http://bcu.shzxlz.cn

println("Hello")
来源：http://jor.zhiwuduotai.top

[T52] Scala：变量
来源：http://pgr.hnqzz.top

val a = 1;  var b = 2
来源：http://mtj.52xcode.cn

[T53] Scala：字符串插值
来源：http://fqt.xziqi.cn

s"值: $b"
来源：http://ksx.quarkkingdee.top

[T54] Scala：集合映射
来源：http://cxh.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://bpf.zhixingplan.top

[T55] Scala：集合过滤
来源：http://cgu.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://nmu.ydzc1.top

[T56] Scala：样例类
来源：http://zpp.havefunace.top

case class User(name: String, age: Int)
来源：http://ent.bbcook.cn

[T57] Scala：模式匹配
来源：http://aqt.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pme.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://lid.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://hjj.ydjk.org.cn

[T59] Scala：循环
来源：http://jzs.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://acb.zhongyouzk.top

[T60] Scala：折叠
来源：http://oaq.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dbj.aizwys.cn

================================================================================
来源：http://wsi.pengpengdd.cyou

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hvw.sweek.top

================================================================================
来源：http://gxd.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://zkk.smart0.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://pen.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://rqg.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rnc.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://xdn.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uuu.xinyue.icu

[U04] Py：变量调试打印
来源：http://div.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aah.jqgufenzy.top

[U05] Py：列表去重且保序
来源：http://azb.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://ghz.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://dth.yangfankeji.com

{**a, **b}
来源：http://mmm.9152youxi.cn

[U07] Py：反转字典键值
来源：http://vqv.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://rph.yongpay.top

[U08] Py：展平二维列表
来源：http://gmh.cucudq.cn

[y for x in nested for y in x]
来源：http://xdd.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://ghj.shanyushiyangtech.top

max(d, key=d.get)
来源：http://hfz.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://ceu.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wlv.xinyue.icu

[U11] Py：生成器表达式
来源：http://ibj.shuidangran.top

(x * 2 for x in arr)
来源：http://mbk.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://gyf.dashuyun.cn

Counter(arr).most_common(3)
来源：http://izt.pycfn.com

[U13] Py：固定长度队列
来源：http://fdk.pycfn.com

deque(maxlen=10)
来源：http://miw.hcnkem.com

[U14] Py：分组收集到列表
来源：http://svz.hongshengwenyu.top

defaultdict(list)
来源：http://gqo.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://okg.chenjidiqi.icu

t = time.perf_counter()
来源：http://fip.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://wbx.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vzj.fengsongda.top

[U17] Py：初始化日志
来源：http://xfx.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://ccn.hcnkem.com

[U18] Py：预编译正则
来源：http://eqr.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://cjc.tarul.cn

[U19] Py：正则替换带回调
来源：http://ipz.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sba.smart0.xyz

[U20] Py：缓存函数结果
来源：http://lfb.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://qtu.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://srt.birdmap.top

@contextlib.contextmanager
来源：http://yhk.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://xme.vqdsnc.cn

list(zip(*m))
来源：http://ogo.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://jco.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bqj.xuetiantiany.cn

[U24] Py：路径操作
来源：http://pxs.gogol.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://juy.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://uue.yj20258.top

csv.DictReader(f)
来源：http://lti.birdmap.top

[U26] Py：并发下载
来源：http://ojc.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oyh.aizwys.cn

[U27] Py：异步 HTTP
来源：http://xre.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://ldw.jqgufenzy.top

[U28] Py：类型别名
来源：http://rht.tanke756.top

UserId = int
来源：http://ava.jyoumei.cn


<!-- 参考信息 -->