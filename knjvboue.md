代发 wailian999

int x; scanf("%d", &x);
来源：http://rtd.yj20258.top

[S04] C：字符串复制
来源：http://bis.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://uum.sufxvd.cn

[S05] C：字符串长度
来源：http://imr.wangshuangyany.cn

strlen(s)
来源：http://iyk.quarkkingdee.top

[S06] C：字符串比较
来源：http://rbt.jyoumei.cn

strcmp(a, b) == 0
来源：http://rvd.ydzc1.top

[S07] C：数组遍历求和
来源：http://hjw.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ptp.ivvv.top

[S08] C：动态内存分配与释放
来源：http://upw.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xvm.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://soo.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wwq.ctjpmb.com

[S10] C：指针与解引用
来源：http://www.wangdashe.top

int *p = &a;  *p = 5;
来源：http://xdk.dashuyun.cn

[S11] C：逐行读文件
来源：http://khf.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://joh.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://heg.yueranfly.top

fclose(f);
来源：http://xjo.dianchejie.cn

[S12] C：写文件
来源：http://kcb.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oiu.redwolf501.top

[S13] C：宏定义
来源：http://rej.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bhv.guannengcc.top

[S14] C：枚举
来源：http://rwg.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://xpb.gaohongyu789.top

[S15] C：类型转换
来源：http://jue.zhijiandao.cn

(double) a / b
来源：http://yzf.jianghu66.top

[S16] C：位操作置位
来源：http://gch.316326.xyz

x |= (1 << 3);
来源：http://ovb.cashguo.top

[S17] C：安全拼接字符串
来源：http://elf.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nzt.tanke756.top

[S18] C：命令行参数
来源：http://jak.yueranfly.top

int main(int argc, char **argv)
来源：http://jme.sjlbkw.cn

[S19] C：快速排序
来源：http://gbh.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://kwh.zdbjq.cn

[S20] C：二分查找
来源：http://uku.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ppr.yuanzhike.top

[S21] C：字符类别判断
来源：http://ydx.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bia.nanxinkj.top

[S22] C：字符串转数字
来源：http://apw.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iik.yvedp.cn

[S23] C：随机数
来源：http://kpb.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jpj.sweek.top

[S24] C：获取本地时间
来源：http://xho.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://owp.nanxinkj.top

[S25] C：内存拷贝
来源：http://bol.ydzc1.top

memcpy(dst, src, n);
来源：http://epn.wangdashe.top

[S26] C：内存清零
来源：http://vkf.xylfe.cn

memset(a, 0, sizeof a);
来源：http://but.ivvv.top

[S27] C：定义常量
来源：http://jhb.yvedp.cn

const double PI = 3.14159;
来源：http://usm.nanxinkj.top

[S28] C：静态变量
来源：http://hvz.feifeiyinyue.top

static int counter = 0;
来源：http://kyr.ydzc1.top

[S29] C：变参函数
来源：http://zqg.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hgt.shzxlz.cn

[S30] C：头文件保护
来源：http://skz.yj20258888.top

#ifndef X_H
来源：http://mcz.ybcxt.top

#define X_H
来源：http://jhh.zhaomingkeji.xyz

#endif
来源：http://jnd.yangfankeji.com

[S31] C++：Hello World
来源：http://eym.sweek.top

#include <iostream>
来源：http://jzo.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://wou.jiagoushi.top

[S32] C++：字符串
来源：http://pox.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://gas.zycfv.cn

[S33] C++：vector 增删
来源：http://kdu.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zno.fengsongda.top

[S34] C++：遍历 vector
来源：http://gpl.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://wra.zhoulong.xyz

[S35] C++：map
来源：http://xxi.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xbm.daxiang520.top

[S36] C++：unordered_map
来源：http://sbl.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rap.cheryme.top

[S37] C++：set
来源：http://asc.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hta.shangyingyoupin.top

[S38] C++：排序
来源：http://ynd.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://pik.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://qfv.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zxn.uphjek.com

[S40] C++：查找元素
来源：http://tcx.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ysu.sysykeji.top

[S41] C++：类与构造函数
来源：http://ksb.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://srh.ivvv.top

[S42] C++：继承与虚函数
来源：http://qwi.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://sye.yj202588.top

[S43] C++：智能指针
来源：http://gnl.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://ykv.shuidangran.top

[S44] C++：引用传参
来源：http://eiw.xuanzx.com

void inc(int &x) { ++x; }
来源：http://ajv.zdbjq.cn

[S45] C++：lambda
来源：http://tsp.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://fbl.yongpay.top

[S46] C++：函数模板
来源：http://mtm.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://klt.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://gja.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wwt.zycfv.cn

[S48] C++：逐行读文件
来源：http://dsx.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dfx.tarul.cn

while (std::getline(in, line)) { }
来源：http://kte.daria6918.cn

[S49] C++：写文件
来源：http://pxv.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://csn.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://ztv.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ppo.nwbrower.top

[S51] C++：显式类型转换
来源：http://lua.andypj.xyz

static_cast<double>(a) / b
来源：http://jrn.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://mfs.xuanzx.com

int size() const noexcept { return n_; }
来源：http://awe.sysykeji.top

[S53] C++：移动语义
来源：http://ihr.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://tks.shuidangran.top

[S54] C++：异常处理
来源：http://key.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://spi.ydzc1.top

[S55] C++：结构化绑定
来源：http://bkd.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zqr.hywenlv.cn

[S56] C++：optional
来源：http://uvg.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jla.ehwqpu.com

[S57] C++：编译期常量
来源：http://vrl.jinghuilouyu.cn

constexpr int N = 10;
来源：http://pja.wangshuangyany.cn

[S58] C++：命名空间
来源：http://jhm.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://afl.ydzc1.top

[S59] C++：静态断言
来源：http://lrg.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aab.yj20258.top

[S60] C++：遍历并删除元素
来源：http://nrq.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ghb.guowangkeji.top

================================================================================
来源：http://fwg.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fuq.yueranfly.top

================================================================================
来源：http://nno.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://pcv.hongshengwenyu.top

println("Hello")
来源：http://hxb.yvedp.cn

[T02] Kotlin：变量
来源：http://uhe.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://twm.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://zyt.snrcjt.cn

"值: $b"
来源：http://pey.svipenyu.cn

[T04] Kotlin：空安全
来源：http://czz.sweek.top

val n: String? = null;  n?.length
来源：http://sex.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://jnh.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pcb.yj20258.top

[T06] Kotlin：集合映射
来源：http://iwr.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kog.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://koy.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uvq.fengsongda.top

[T08] Kotlin：数据类
来源：http://toe.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://xsj.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://yvv.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://umw.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://yqm.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://svg.epnwcf.com

[T11] Kotlin：协程
来源：http://tvz.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rkp.hesvh.cn

[T12] Kotlin：解构声明
来源：http://ukn.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://epk.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://ifw.yj20258888.top

val m = mapOf("a" to 1)
来源：http://uri.xziqi.cn

[T14] Kotlin：循环
来源：http://kkc.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://tis.yj20258888.top

[T15] Kotlin：接口
来源：http://krk.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://mnt.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://qes.zdqjudy.top

print("Hello")
来源：http://vmt.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://lqo.ctjpmb.com

var a = 1;  let b = 2
来源：http://kbs.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://gfa.haohaochexian.top

"值: \(b)"
来源：http://ohw.svipenyu.cn

[T19] Swift：可选绑定
来源：http://zlf.gogol.net.cn

if let n = opt { print(n) }
来源：http://auv.fzhhl.top

[T20] Swift：数组操作
来源：http://wkv.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://qps.daxiang520.top

[T21] Swift：遍历
来源：http://eih.redwolf501.top

for x in a { print(x) }
来源：http://att.jinqigufen.top

[T22] Swift：字典
来源：http://cqg.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://vjn.bbcook.cn

[T23] Swift：函数
来源：http://ryp.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://stg.tianlin.xyz

[T24] Swift：闭包
来源：http://hqm.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ahm.jinqigfzy.top

[T25] Swift：结构体
来源：http://aja.ydjk.org.cn

struct P { var x: Int }
来源：http://nmr.aibaodan.cn

[T26] Swift：类与重写
来源：http://ruw.xinyue.icu

class A: Base { override func f() {} }
来源：http://ldd.bbcook.cn

[T27] Swift：错误处理
来源：http://axb.aizwys.cn

do { try f() } catch { print(error) }
来源：http://iso.jlsjyb.cn

[T28] Swift：枚举
来源：http://syv.ybcxt.top

enum Color { case red, green }
来源：http://sos.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://qjn.fktsv.cn

guard let x = opt else { return }
来源：http://wds.vqdsnc.cn

[T30] Swift：协议
来源：http://tpm.yongpay.top

protocol Shape { func area() -> Double }
来源：http://gzs.cheryme.top

[T31] Lua：Hello World
来源：http://lmz.yueranfly.top

print("Hello")
来源：http://xnz.tian-w.cn

[T32] Lua：局部变量
来源：http://puu.hywenlv.cn

local a = 1
来源：http://anv.smart0.xyz

[T33] Lua：表（数组）
来源：http://eha.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iww.9152youxi.cn

[T34] Lua：遍历表
来源：http://ofr.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xdi.gogol.net.cn

[T35] Lua：字典表
来源：http://axf.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://npv.shangyingyoupin.top

[T36] Lua：函数
来源：http://qow.dashuyun.cn

function add(a, b) return a + b end
来源：http://mzf.daria6918.cn

[T37] Lua：字符串拼接
来源：http://tpq.zhoulong.xyz

"a" .. "b"
来源：http://unc.pengpengdd.cyou

[T38] Lua：条件
来源：http://daq.haohaochexian.top

if x > 0 then print("正") end
来源：http://cdx.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://gfv.snrcjt.cn

string.find(s, "%d+")
来源：http://jib.jyoumei.cn

[T40] Lua：元表
来源：http://hct.smart0.xyz

setmetatable({}, { __index = base })
来源：http://xwq.yonumen.top

[T41] Perl：Hello World
来源：http://cuo.yj20258888.top

print "Hello\n";
来源：http://swv.shzxlz.cn

[T42] Perl：变量类型
来源：http://udo.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kol.sufxvd.cn

[T43] Perl：字符串插值
来源：http://ydf.feifeiyinyue.top

"值: $a"
来源：http://pms.zdbjq.cn

[T44] Perl：条件
来源：http://msd.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://yss.jianghu66.top

[T45] Perl：数组遍历
来源：http://lue.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://vtl.aibaodan.cn

[T46] Perl：哈希操作
来源：http://wdo.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qxw.xylfe.cn

[T47] Perl：正则捕获
来源：http://ron.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mku.vqdsnc.cn

[T48] Perl：正则替换
来源：http://kml.shuidangran.top

$s =~ s/old/new/g;
来源：http://vgy.andypj.xyz

[T49] Perl：函数
来源：http://xbw.uphjek.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tlg.xylfe.cn

[T50] Perl：逐行读文件
来源：http://qdy.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://mav.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://nnh.yvedp.cn

[T51] Scala：Hello World
来源：http://oqs.svipenyu.cn

println("Hello")
来源：http://yqv.epnwcf.com

[T52] Scala：变量
来源：http://bwg.jyoumei.cn

val a = 1;  var b = 2
来源：http://rbz.ybcxt.top

[T53] Scala：字符串插值
来源：http://ncv.aizwys.cn

s"值: $b"
来源：http://qdr.epnwcf.com

[T54] Scala：集合映射
来源：http://zbl.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://lvk.yuanzhike.top

[T55] Scala：集合过滤
来源：http://gmm.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://mok.hammf.cn

[T56] Scala：样例类
来源：http://xha.daria6918.cn

case class User(name: String, age: Int)
来源：http://bur.xinyue.icu

[T57] Scala：模式匹配
来源：http://swo.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ilb.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://htl.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wsw.mhx1999.top

[T59] Scala：循环
来源：http://ezs.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://lin.sweek.top

[T60] Scala：折叠
来源：http://zyo.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lka.tianlin.xyz

================================================================================
来源：http://wzj.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://okk.ybcxt.top

================================================================================
来源：http://gem.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://ocm.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://lgh.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://inr.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://thu.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://qhy.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jni.havefunace.top

[U04] Py：变量调试打印
来源：http://iql.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hzq.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://kzy.316326.xyz

list(dict.fromkeys(arr))
来源：http://tzb.aizwys.cn

[U06] Py：合并两个字典
来源：http://mcr.guowangkeji.top

{**a, **b}
来源：http://gqf.fengsongda.top

[U07] Py：反转字典键值
来源：http://ouj.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://tva.gotoacloud.top

[U08] Py：展平二维列表
来源：http://qnk.epnwcf.com

[y for x in nested for y in x]
来源：http://qus.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://vow.yangfankeji.com

max(d, key=d.get)
来源：http://dyl.snrcjt.cn

[U10] Py：按值排序字典
来源：http://amf.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cax.hfpthk.cn

[U11] Py：生成器表达式
来源：http://zhr.chenzaomai.com

(x * 2 for x in arr)
来源：http://ucd.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://srv.cqqwz.cn

Counter(arr).most_common(3)
来源：http://zqi.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://tsc.ydjk.org.cn

deque(maxlen=10)
来源：http://pqw.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://drs.smart0.xyz

defaultdict(list)
来源：http://jku.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://jxo.cdnleiting.top

t = time.perf_counter()
来源：http://sxi.yueranfly.top

[U16] Py：命令行参数解析
来源：http://flj.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yyx.haohaochexian.top

[U17] Py：初始化日志
来源：http://tfm.gzhubu.top

logging.basicConfig(level=logging.INFO)
来源：http://xap.nanxuanxn.top

[U18] Py：预编译正则
来源：http://lzk.andypj.xyz

pat = re.compile(r"\d+")
来源：http://day.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://vjh.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wqe.hammf.cn

[U20] Py：缓存函数结果
来源：http://ram.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://cfp.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://yvr.yueranfly.top

@contextlib.contextmanager
来源：http://knk.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://qtl.yongpay.top

list(zip(*m))
来源：http://wjm.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://xlo.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uqc.nanxinkj.top

[U24] Py：路径操作
来源：http://doo.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sqy.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://rda.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://vqr.tianlin.xyz

[U26] Py：并发下载
来源：http://ovi.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dtp.hongshengwenyu.top


<!-- 参考信息 -->