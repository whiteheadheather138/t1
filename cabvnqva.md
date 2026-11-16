代发 wailian999

strlen(s)
来源：http://uig.tarul.cn

[S06] C：字符串比较
来源：http://viu.yuanzhike.top

strcmp(a, b) == 0
来源：http://xow.wangdashe.top

[S07] C：数组遍历求和
来源：http://wfm.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://avc.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://ghc.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ekd.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://ggr.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jhe.zhengqikj.top

[S10] C：指针与解引用
来源：http://xor.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://yjk.gaohongyu789.top

[S11] C：逐行读文件
来源：http://ery.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ywo.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://txv.shuidangran.top

fclose(f);
来源：http://vwf.shangyingyoupin.top

[S12] C：写文件
来源：http://khg.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rnm.bbcook.cn

[S13] C：宏定义
来源：http://akg.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pjg.ywan-chungtsiang.top

[S14] C：枚举
来源：http://ygz.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://goy.jinqigfzy.top

[S15] C：类型转换
来源：http://odl.ydzc1.top

(double) a / b
来源：http://icq.yj20258888.top

[S16] C：位操作置位
来源：http://uhn.pycfn.com

x |= (1 << 3);
来源：http://vjw.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://tss.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ogz.hnqzz.top

[S18] C：命令行参数
来源：http://wxl.yuanzhike.top

int main(int argc, char **argv)
来源：http://nod.daria6918.cn

[S19] C：快速排序
来源：http://khs.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://moo.xinyue.icu

[S20] C：二分查找
来源：http://jnw.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://whp.iojbl.cn

[S21] C：字符类别判断
来源：http://mzg.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwx.chenlongwang.top

[S22] C：字符串转数字
来源：http://lbo.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://ymy.yvedp.cn

[S23] C：随机数
来源：http://vnj.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://luv.jinqigufen.top

[S24] C：获取本地时间
来源：http://pho.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cuw.fzhhl.top

[S25] C：内存拷贝
来源：http://adp.ydzc1.top

memcpy(dst, src, n);
来源：http://gbw.cucudq.cn

[S26] C：内存清零
来源：http://gzm.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://jks.shangyingyoupin.top

[S27] C：定义常量
来源：http://hkc.gotoacloud.top

const double PI = 3.14159;
来源：http://wlh.jyoumei.cn

[S28] C：静态变量
来源：http://yrf.nwbrower.top

static int counter = 0;
来源：http://bra.fktsv.cn

[S29] C：变参函数
来源：http://qaq.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fai.dianchejie.cn

[S30] C：头文件保护
来源：http://flb.yuxming.cn

#ifndef X_H
来源：http://ghy.fktsv.cn

#define X_H
来源：http://juk.jinqigufen.top

#endif
来源：http://bso.zhongyouzk.top

[S31] C++：Hello World
来源：http://sht.jinqigfzy.top

#include <iostream>
来源：http://fui.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://dwn.svipenyu.cn

[S32] C++：字符串
来源：http://fho.tanke756.top

std::string s = "hi";  s += "!";
来源：http://rpr.hnxiangtu.top

[S33] C++：vector 增删
来源：http://iwk.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sai.zycfv.cn

[S34] C++：遍历 vector
来源：http://dok.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://tbd.yvedp.cn

[S35] C++：map
来源：http://oll.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xku.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://jba.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ncc.cashguo.top

[S37] C++：set
来源：http://ouc.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://afx.zhongyouzk.top

[S38] C++：排序
来源：http://zce.kuanghao11.cn

std::sort(v.begin(), v.end());
来源：http://rkh.pycfn.com

[S39] C++：自定义比较器排序
来源：http://qks.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hmu.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://vlw.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://osu.yangfankeji.com

[S41] C++：类与构造函数
来源：http://bsf.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sbj.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://mdq.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://mqe.hesvh.cn

[S43] C++：智能指针
来源：http://wfr.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://bhc.shangyingyoupin.top

[S44] C++：引用传参
来源：http://pvt.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://qvo.yvedp.cn

[S45] C++：lambda
来源：http://yka.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://kao.gaohongyu789.top

[S46] C++：函数模板
来源：http://lwv.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zxj.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://vra.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xzg.fktsv.cn

[S48] C++：逐行读文件
来源：http://hof.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://qpq.ivvv.top

while (std::getline(in, line)) { }
来源：http://imx.hcnkem.com

[S49] C++：写文件
来源：http://stu.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qmg.yuanzhike.top

[S50] C++：格式化数字
来源：http://ybv.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ikf.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://pme.shzxlz.cn

static_cast<double>(a) / b
来源：http://jmo.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://kyi.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://uyt.dashuyun.cn

[S53] C++：移动语义
来源：http://omk.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://cbv.cashguo.top

[S54] C++：异常处理
来源：http://qkg.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://woz.gotoacloud.top

[S55] C++：结构化绑定
来源：http://otx.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xkt.pycfn.com

[S56] C++：optional
来源：http://psd.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wms.hnxiangtu.top

[S57] C++：编译期常量
来源：http://zun.snrcjt.cn

constexpr int N = 10;
来源：http://umy.gaohongyu789.top

[S58] C++：命名空间
来源：http://fjh.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://tuy.nanxinkj.top

[S59] C++：静态断言
来源：http://xsh.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ish.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://nxk.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sfe.9152youxi.cn

================================================================================
来源：http://erm.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://atm.yj202588.top

================================================================================
来源：http://xuo.yj20258.top

[T01] Kotlin：Hello World
来源：http://wwx.xziqi.cn

println("Hello")
来源：http://ooq.pycfn.com

[T02] Kotlin：变量
来源：http://orx.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ktb.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://ujt.fanxiaobao.xyz

"值: $b"
来源：http://whb.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://pod.yj202588.top

val n: String? = null;  n?.length
来源：http://zya.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://hpt.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rie.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://rke.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zzw.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://rsy.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://awr.chenzaomai.com

[T08] Kotlin：数据类
来源：http://vnf.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://wxv.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://jth.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://yxx.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://nkr.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rxh.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://yvi.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ehb.yueranfly.top

[T12] Kotlin：解构声明
来源：http://wqa.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://ita.pycfn.com

[T13] Kotlin：只读 Map
来源：http://bvc.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://fvv.gaohongyu789.top

[T14] Kotlin：循环
来源：http://otx.9152youxi.cn

for (i in 1..10) println(i)
来源：http://orj.zhijiandao.cn

[T15] Kotlin：接口
来源：http://fbp.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://zcd.jinqigufen.top

[T16] Swift：Hello World
来源：http://qyq.ehwqpu.com

print("Hello")
来源：http://xsx.tian-w.cn

[T17] Swift：变量与常量
来源：http://msh.cqqwz.cn

var a = 1;  let b = 2
来源：http://azw.zdbjq.cn

[T18] Swift：字符串插值
来源：http://aua.cashguo.top

"值: \(b)"
来源：http://vlp.tanke756.top

[T19] Swift：可选绑定
来源：http://jqf.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://gzw.zdbjq.cn

[T20] Swift：数组操作
来源：http://eku.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jhe.ehwqpu.com

[T21] Swift：遍历
来源：http://vvw.xylfe.cn

for x in a { print(x) }
来源：http://ngw.sjlbkw.cn

[T22] Swift：字典
来源：http://klj.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iwy.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://eui.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dsr.fktsv.cn

[T24] Swift：闭包
来源：http://whu.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eqa.tian-w.cn

[T25] Swift：结构体
来源：http://zio.yanxiufei.cn

struct P { var x: Int }
来源：http://sey.shuidangran.top

[T26] Swift：类与重写
来源：http://vqx.xziqi.cn

class A: Base { override func f() {} }
来源：http://pit.cucudq.cn

[T27] Swift：错误处理
来源：http://ofs.daxiang520.top

do { try f() } catch { print(error) }
来源：http://exo.ivvv.top

[T28] Swift：枚举
来源：http://jjp.redwolf501.top

enum Color { case red, green }
来源：http://mrn.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://pjf.zdbjq.cn

guard let x = opt else { return }
来源：http://tpd.ybcxt.top

[T30] Swift：协议
来源：http://ssf.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://tgl.zhengqikj.top

[T31] Lua：Hello World
来源：http://jyy.tian-w.cn

print("Hello")
来源：http://tzr.jlsjyb.cn

[T32] Lua：局部变量
来源：http://tne.yj202588.top

local a = 1
来源：http://vmm.yj202588.top

[T33] Lua：表（数组）
来源：http://wwr.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lle.vehdjk.com

[T34] Lua：遍历表
来源：http://ooz.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rqz.cqqwz.cn

[T35] Lua：字典表
来源：http://xwa.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://ogx.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://ile.redwolf501.top

function add(a, b) return a + b end
来源：http://mab.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://oqj.0kj1m.cn

"a" .. "b"
来源：http://ddh.pycfn.com

[T38] Lua：条件
来源：http://nch.pycfn.com

if x > 0 then print("正") end
来源：http://tdb.yonumen.top

[T39] Lua：模式匹配
来源：http://vuf.hcnkem.com

string.find(s, "%d+")
来源：http://pmi.jlsjyb.cn

[T40] Lua：元表
来源：http://fnm.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://hob.bjfxy.top

[T41] Perl：Hello World
来源：http://wuy.wangshuangyany.cn

print "Hello\n";
来源：http://yqf.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://zju.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://drh.wangdashe.top

[T43] Perl：字符串插值
来源：http://eqc.ivvv.top

"值: $a"
来源：http://vaq.yuxming.cn

[T44] Perl：条件
来源：http://nis.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://dqc.aibaodan.cn

[T45] Perl：数组遍历
来源：http://axs.cashguo.top

for my $x (@arr) { print $x; }
来源：http://ave.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://eij.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://igv.xylfe.cn

[T47] Perl：正则捕获
来源：http://xzs.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://krw.fktsv.cn

[T48] Perl：正则替换
来源：http://thk.316326.xyz

$s =~ s/old/new/g;
来源：http://srm.jinghuilouyu.cn

[T49] Perl：函数
来源：http://msb.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oie.yj202588.top

[T50] Perl：逐行读文件
来源：http://mpw.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nir.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://exk.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://tpt.pycfn.com

println("Hello")
来源：http://qxl.haohaochexian.top

[T52] Scala：变量
来源：http://cmp.aibaodan.cn

val a = 1;  var b = 2
来源：http://hle.hammf.cn

[T53] Scala：字符串插值
来源：http://fqw.iojbl.cn

s"值: $b"
来源：http://egn.yvedp.cn

[T54] Scala：集合映射
来源：http://mdh.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://xck.hcnkem.com

[T55] Scala：集合过滤
来源：http://fks.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://fnb.jianghu66.top

[T56] Scala：样例类
来源：http://zyi.bbcook.cn

case class User(name: String, age: Int)
来源：http://sqn.yonumen.top

[T57] Scala：模式匹配
来源：http://irh.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jjm.zycfv.cn

[T58] Scala：函数定义
来源：http://qdi.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://msu.hnxiangtu.top

[T59] Scala：循环
来源：http://yin.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://hii.yanxiufei.cn

[T60] Scala：折叠
来源：http://avc.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rhq.jianghu66.top

================================================================================
来源：http://cuc.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iec.cqqwz.cn

================================================================================
来源：http://gjl.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://ozs.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ujv.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://rjb.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ljf.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://bvy.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sxo.mhx1999.top

[U04] Py：变量调试打印
来源：http://wkf.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://juu.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://rfs.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://vcd.xziqi.cn

[U06] Py：合并两个字典
来源：http://ruh.gaohongyu789.top

{**a, **b}
来源：http://tvz.tanke756.top

[U07] Py：反转字典键值
来源：http://anm.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://oxa.tian-w.cn

[U08] Py：展平二维列表
来源：http://mvr.tanke756.top

[y for x in nested for y in x]
来源：http://woc.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://mwv.mhx1999.top

max(d, key=d.get)
来源：http://hcx.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://ydw.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cyz.hfpthk.cn

[U11] Py：生成器表达式
来源：http://wxd.tanke756.top

(x * 2 for x in arr)
来源：http://qrx.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kop.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://zlg.xziqi.cn

[U13] Py：固定长度队列
来源：http://fsy.yuanzhike.top

deque(maxlen=10)
来源：http://oxv.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://mba.hysaishi.cn

defaultdict(list)
来源：http://eqx.ctjpmb.com

[U15] Py：高精度计时
来源：http://ehz.havefunace.top

t = time.perf_counter()
来源：http://kau.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://hbx.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wbe.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://tns.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://lzy.yj20258.top

[U18] Py：预编译正则
来源：http://ydt.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://vvv.hcnkem.com

[U19] Py：正则替换带回调
来源：http://zlw.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jxw.vehdjk.com

[U20] Py：缓存函数结果
来源：http://cra.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://jge.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://vpw.yj20258888.top

@contextlib.contextmanager
来源：http://fnr.c1oappe.top

[U22] Py：矩阵转置
来源：http://dxj.feifeiyinyue.top

list(zip(*m))
来源：http://dlu.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://fqw.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wzv.jqgfzy.top

[U24] Py：路径操作
来源：http://mic.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mat.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://wsu.fzhhl.top

csv.DictReader(f)
来源：http://ibq.aizwys.cn

[U26] Py：并发下载
来源：http://ziw.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ewz.daxiang520.top

[U27] Py：异步 HTTP
来源：http://hcu.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://hnc.52xcode.cn

[U28] Py：类型别名
来源：http://rhb.yj202588.top

UserId = int
来源：http://hmm.0kj1m.cn


<!-- 参考信息 -->