代发 wailian999

int x; scanf("%d", &x);
来源：http://itl.zhongyouzk.top

[S04] C：字符串复制
来源：http://dtf.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://etd.hywenlv.cn

[S05] C：字符串长度
来源：http://grs.sxryk.cn

strlen(s)
来源：http://fsl.316326.xyz

[S06] C：字符串比较
来源：http://tul.cqqwz.cn

strcmp(a, b) == 0
来源：http://svp.hywenlv.cn

[S07] C：数组遍历求和
来源：http://htr.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jkg.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://auf.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ade.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://lfl.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iuw.gaohongyu789.top

[S10] C：指针与解引用
来源：http://yab.meibo888.top

int *p = &a;  *p = 5;
来源：http://dmn.svipenyu.cn

[S11] C：逐行读文件
来源：http://rwn.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://cwg.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xwp.xuetiantiany.cn

fclose(f);
来源：http://tqb.pengpengdd.cyou

[S12] C：写文件
来源：http://rsa.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wnw.hnxiangtu.top

[S13] C：宏定义
来源：http://dsf.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hsa.hnqzz.top

[S14] C：枚举
来源：http://caa.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ads.yj202588.top

[S15] C：类型转换
来源：http://fto.yj20258888.top

(double) a / b
来源：http://exh.kuanghao11.cn

[S16] C：位操作置位
来源：http://iuk.guannengcc.top

x |= (1 << 3);
来源：http://bff.yvedp.cn

[S17] C：安全拼接字符串
来源：http://tqb.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gcr.yongpay.top

[S18] C：命令行参数
来源：http://pib.ctjpmb.com

int main(int argc, char **argv)
来源：http://wzd.hnxiangtu.top

[S19] C：快速排序
来源：http://fxt.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://myo.cdnleiting.top

[S20] C：二分查找
来源：http://xhn.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jka.haohaochexian.top

[S21] C：字符类别判断
来源：http://aea.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ckf.hnxiangtu.top

[S22] C：字符串转数字
来源：http://tbs.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nub.shanyushiyangtech.top

[S23] C：随机数
来源：http://qln.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ehh.zhijiandao.cn

[S24] C：获取本地时间
来源：http://ywt.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qdw.yanxiufei.cn

[S25] C：内存拷贝
来源：http://pkj.birdmap.top

memcpy(dst, src, n);
来源：http://okf.chenzaomai.com

[S26] C：内存清零
来源：http://ttu.tanke756.top

memset(a, 0, sizeof a);
来源：http://vox.daxiang520.top

[S27] C：定义常量
来源：http://xsq.havefunace.top

const double PI = 3.14159;
来源：http://hvt.hysaishi.cn

[S28] C：静态变量
来源：http://djo.fanxiaobao.xyz

static int counter = 0;
来源：http://gbl.zhengqikj.top

[S29] C：变参函数
来源：http://hxr.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aqh.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://pmh.zhengqikj.top

#ifndef X_H
来源：http://yoy.wangdashe.top

#define X_H
来源：http://daa.jyoumei.cn

#endif
来源：http://hou.daria6918.cn

[S31] C++：Hello World
来源：http://gjt.zhiwuduotai.top

#include <iostream>
来源：http://exs.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://gxt.bbcook.cn

[S32] C++：字符串
来源：http://aed.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://quh.havefunace.top

[S33] C++：vector 增删
来源：http://udl.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pfh.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://tje.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://xjg.cdnleiting.top

[S35] C++：map
来源：http://cpz.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kpm.iojbl.cn

[S36] C++：unordered_map
来源：http://lxm.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rwd.hesvh.cn

[S37] C++：set
来源：http://yyl.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://con.sufxvd.cn

[S38] C++：排序
来源：http://qoq.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://ydd.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://fmo.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qqg.fktsv.cn

[S40] C++：查找元素
来源：http://zkt.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kds.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://hge.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qvw.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://vtx.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://cul.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://qac.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://dzx.pengpengdd.cyou

[S44] C++：引用传参
来源：http://tsi.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://pio.jinqigfzy.top

[S45] C++：lambda
来源：http://lgm.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://zio.yj20258888.top

[S46] C++：函数模板
来源：http://ops.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kxg.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://txh.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://orl.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://jdm.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://vwm.uphjek.com

while (std::getline(in, line)) { }
来源：http://lyy.shuidangran.top

[S49] C++：写文件
来源：http://ywk.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mvz.dianchejie.cn

[S50] C++：格式化数字
来源：http://cax.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://egn.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://zky.jinqigfzy.top

static_cast<double>(a) / b
来源：http://zse.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://duw.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://dhz.wangdashe.top

[S53] C++：移动语义
来源：http://dfs.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://yqi.xylfe.cn

[S54] C++：异常处理
来源：http://ywa.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zdx.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://eph.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fcv.zhijiandao.cn

[S56] C++：optional
来源：http://dka.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lcp.nanxinkj.top

[S57] C++：编译期常量
来源：http://rcf.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://ory.bjfxy.top

[S58] C++：命名空间
来源：http://nig.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://vkf.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://ure.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://txv.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://aad.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gvs.redwolf501.top

================================================================================
来源：http://nwl.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aew.dashuyun.cn

================================================================================
来源：http://fcr.xziqi.cn

[T01] Kotlin：Hello World
来源：http://jdu.ydjk.org.cn

println("Hello")
来源：http://dyx.yj20258.top

[T02] Kotlin：变量
来源：http://nxo.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://saf.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://bwo.guowangkeji.top

"值: $b"
来源：http://mfn.tarul.cn

[T04] Kotlin：空安全
来源：http://nqj.zycfv.cn

val n: String? = null;  n?.length
来源：http://rtc.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://zdt.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pzz.daxiang520.top

[T06] Kotlin：集合映射
来源：http://eqq.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eog.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://ktx.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hjt.ydzc1.top

[T08] Kotlin：数据类
来源：http://vhs.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://tse.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://qfv.yj20258.top

fun String.exclaim() = this + "!"
来源：http://iky.shuidangran.top

[T10] Kotlin：默认参数
来源：http://zem.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://trd.sysykeji.top

[T11] Kotlin：协程
来源：http://tvv.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wia.sysykeji.top

[T12] Kotlin：解构声明
来源：http://pce.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://bei.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://xrj.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://lfc.chenlongwang.top

[T14] Kotlin：循环
来源：http://hkw.yj20258.top

for (i in 1..10) println(i)
来源：http://pee.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://twy.xziqi.cn

interface Shape { fun area(): Double }
来源：http://ymw.hysaishi.cn

[T16] Swift：Hello World
来源：http://off.xingfuxueyuan.xyz

print("Hello")
来源：http://lok.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://jsi.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://tyu.daria6918.cn

[T18] Swift：字符串插值
来源：http://rwk.wangshuangyany.cn

"值: \(b)"
来源：http://izq.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://izb.ydjk.org.cn

if let n = opt { print(n) }
来源：http://lbo.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://zjs.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://tpw.tian-w.cn

[T21] Swift：遍历
来源：http://ptk.fzhhl.top

for x in a { print(x) }
来源：http://axe.jinqigufen.top

[T22] Swift：字典
来源：http://jdt.epnwcf.com

var d = ["a": 1];  d["b"] = 2
来源：http://xds.bbcook.cn

[T23] Swift：函数
来源：http://wsj.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jki.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://gkq.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xuj.fehbvm.com

[T25] Swift：结构体
来源：http://gul.nanxinkj.top

struct P { var x: Int }
来源：http://bop.yj20258888.top

[T26] Swift：类与重写
来源：http://apl.xylfe.cn

class A: Base { override func f() {} }
来源：http://esx.birdmap.top

[T27] Swift：错误处理
来源：http://nkr.bjfxy.top

do { try f() } catch { print(error) }
来源：http://lws.hywenlv.cn

[T28] Swift：枚举
来源：http://idl.redwolf501.top

enum Color { case red, green }
来源：http://heu.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://bgj.0kj1m.cn

guard let x = opt else { return }
来源：http://sby.smart0.xyz

[T30] Swift：协议
来源：http://txb.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://foq.fzhhl.top

[T31] Lua：Hello World
来源：http://tpk.vehdjk.com

print("Hello")
来源：http://jej.yfazqb.com

[T32] Lua：局部变量
来源：http://rhm.zdbjq.cn

local a = 1
来源：http://dwj.sweek.top

[T33] Lua：表（数组）
来源：http://lpx.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://xlt.hfpthk.cn

[T34] Lua：遍历表
来源：http://faz.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wxv.0kj1m.cn

[T35] Lua：字典表
来源：http://nxk.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://lsv.cashguo.top

[T36] Lua：函数
来源：http://zft.tarul.cn

function add(a, b) return a + b end
来源：http://wpi.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://btq.yj20258888.top

"a" .. "b"
来源：http://eoa.havefunace.top

[T38] Lua：条件
来源：http://vwr.vqdsnc.cn

if x > 0 then print("正") end
来源：http://gke.yuxming.cn

[T39] Lua：模式匹配
来源：http://pcx.ivvv.top

string.find(s, "%d+")
来源：http://cic.uphjek.com

[T40] Lua：元表
来源：http://sly.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://xlo.smart0.xyz

[T41] Perl：Hello World
来源：http://iqa.chenzaomai.com

print "Hello\n";
来源：http://qat.svipenyu.cn

[T42] Perl：变量类型
来源：http://vsz.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hbd.zycfv.cn

[T43] Perl：字符串插值
来源：http://bgr.chenlongwang.top

"值: $a"
来源：http://unw.daria6918.cn

[T44] Perl：条件
来源：http://ard.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://hvq.fehbvm.com

[T45] Perl：数组遍历
来源：http://yzm.xuanzx.com

for my $x (@arr) { print $x; }
来源：http://tgj.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://llz.hysaishi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fcr.smart0.xyz

[T47] Perl：正则捕获
来源：http://iou.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://une.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://bfe.daria6918.cn

$s =~ s/old/new/g;
来源：http://rpl.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://dqb.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qus.vehdjk.com

[T50] Perl：逐行读文件
来源：http://vpz.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vhs.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://nix.hnqzz.top

[T51] Scala：Hello World
来源：http://xmk.jiagoushi.top

println("Hello")
来源：http://kni.yuxming.cn

[T52] Scala：变量
来源：http://epg.zhijiandao.cn

val a = 1;  var b = 2
来源：http://rgp.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://vkp.zhiwuduotai.top

s"值: $b"
来源：http://vhu.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://unf.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://tgw.cdnleiting.top

[T55] Scala：集合过滤
来源：http://ras.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://xmv.feifeiyinyue.top

[T56] Scala：样例类
来源：http://fbd.yangfankeji.com

case class User(name: String, age: Int)
来源：http://ukb.yongpay.top

[T57] Scala：模式匹配
来源：http://qxz.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsl.cheryme.top

[T58] Scala：函数定义
来源：http://wcb.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://hhr.jqgufenzy.top

[T59] Scala：循环
来源：http://pyc.sxryk.cn

for (i <- 1 to 10) println(i)
来源：http://ndb.gzhubu.top

[T60] Scala：折叠
来源：http://mmb.yueranfly.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lie.hesvh.cn

================================================================================
来源：http://sbm.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cys.daria6918.cn

================================================================================
来源：http://gcn.yonumen.top

[U01] Py：创建虚拟环境
来源：http://xhv.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vou.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://cyz.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kue.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://jgr.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jnb.fktsv.cn

[U04] Py：变量调试打印
来源：http://rem.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mec.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://iil.yj20258.top

list(dict.fromkeys(arr))
来源：http://oij.dianchejie.cn

[U06] Py：合并两个字典
来源：http://ovd.yueranfly.top

{**a, **b}
来源：http://hii.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://qvf.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://psz.tian-w.cn

[U08] Py：展平二维列表
来源：http://kjc.fengsongda.top

[y for x in nested for y in x]
来源：http://avs.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://frd.zdbjq.cn

max(d, key=d.get)
来源：http://hru.gotoacloud.top

[U10] Py：按值排序字典
来源：http://wno.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nrj.chenzaomai.com

[U11] Py：生成器表达式
来源：http://flu.hammf.cn

(x * 2 for x in arr)
来源：http://eor.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://cps.vehdjk.com

Counter(arr).most_common(3)
来源：http://ywa.ctjpmb.com

[U13] Py：固定长度队列
来源：http://swd.nwbrower.top

deque(maxlen=10)
来源：http://qkg.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://mrj.dianchejie.cn

defaultdict(list)
来源：http://ooz.ybcxt.top

[U15] Py：高精度计时
来源：http://ymu.redwolf501.top

t = time.perf_counter()
来源：http://vau.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://ilr.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://his.pycfn.com

[U17] Py：初始化日志
来源：http://pqt.nanxinkj.top

logging.basicConfig(level=logging.INFO)
来源：http://quf.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://cfv.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://ldd.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://fyk.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ufo.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://mnj.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://opg.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://fus.zycfv.cn

@contextlib.contextmanager
来源：http://bgi.jqgfzy.top

[U22] Py：矩阵转置
来源：http://jrp.bbcook.cn

list(zip(*m))
来源：http://nux.daxiang520.top

[U23] Py：分块读取大文件
来源：http://hob.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aya.chenlongwang.top

[U24] Py：路径操作
来源：http://tbd.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yyr.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://ioc.xuetiantiany.cn

csv.DictReader(f)
来源：http://ihk.guowangkeji.top

[U26] Py：并发下载
来源：http://uvn.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ymn.wangshuangyany.cn


<!-- 参考信息 -->