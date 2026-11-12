代发 wailian999

strlen(s)
来源：http://ysa.chenzaomai.com

[S06] C：字符串比较
来源：http://rxz.bbcook.cn

strcmp(a, b) == 0
来源：http://ebe.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://zfd.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ldy.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://niy.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wkw.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://nip.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xlg.yvedp.cn

[S10] C：指针与解引用
来源：http://kmt.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://fos.bbcook.cn

[S11] C：逐行读文件
来源：http://zho.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://gro.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://guq.fengsongda.top

fclose(f);
来源：http://wra.sxryk.cn

[S12] C：写文件
来源：http://oqp.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dok.aizwys.cn

[S13] C：宏定义
来源：http://wsl.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dam.chenlongwang.top

[S14] C：枚举
来源：http://ovg.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://ulr.hesvh.cn

[S15] C：类型转换
来源：http://vjx.9152youxi.cn

(double) a / b
来源：http://zae.daxiang520.top

[S16] C：位操作置位
来源：http://vyi.tanke756.top

x |= (1 << 3);
来源：http://ltj.hnqzz.top

[S17] C：安全拼接字符串
来源：http://dpw.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ezr.zdbjq.cn

[S18] C：命令行参数
来源：http://euv.jlsjyb.cn

int main(int argc, char **argv)
来源：http://pmf.jinqigfzy.top

[S19] C：快速排序
来源：http://biq.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gug.316326.xyz

[S20] C：二分查找
来源：http://mkp.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pav.yonumen.top

[S21] C：字符类别判断
来源：http://luk.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syi.52xcode.cn

[S22] C：字符串转数字
来源：http://sqh.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://rkd.zhijiandao.cn

[S23] C：随机数
来源：http://aen.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vjc.zycfv.cn

[S24] C：获取本地时间
来源：http://juk.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cmn.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://agd.9152youxi.cn

memcpy(dst, src, n);
来源：http://who.dianchejie.cn

[S26] C：内存清零
来源：http://cti.tanke756.top

memset(a, 0, sizeof a);
来源：http://hkz.jqgfzy.top

[S27] C：定义常量
来源：http://jbp.aizwys.cn

const double PI = 3.14159;
来源：http://xcg.feifeiyinyue.top

[S28] C：静态变量
来源：http://vwg.xingfuxueyuan.xyz

static int counter = 0;
来源：http://vjl.aizwys.cn

[S29] C：变参函数
来源：http://yzg.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ggj.yongpay.top

[S30] C：头文件保护
来源：http://uta.hesvh.cn

#ifndef X_H
来源：http://nos.fzhhl.top

#define X_H
来源：http://isr.daria6918.cn

#endif
来源：http://nde.fengsongda.top

[S31] C++：Hello World
来源：http://pzx.jianghu66.top

#include <iostream>
来源：http://wuo.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://den.sjlbkw.cn

[S32] C++：字符串
来源：http://jdm.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://tke.zhijiandao.cn

[S33] C++：vector 增删
来源：http://kik.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cgo.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://pnf.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://dyx.0kj1m.cn

[S35] C++：map
来源：http://hac.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://syv.jinqigfzy.top

[S36] C++：unordered_map
来源：http://xvj.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hhn.wangdashe.top

[S37] C++：set
来源：http://nnr.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xdq.shzxlz.cn

[S38] C++：排序
来源：http://eix.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://ivc.yongpay.top

[S39] C++：自定义比较器排序
来源：http://xgj.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qch.jqgfzy.top

[S40] C++：查找元素
来源：http://xot.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olp.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://hmb.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlx.wangdashe.top

[S42] C++：继承与虚函数
来源：http://vir.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://zrk.cdnleiting.top

[S43] C++：智能指针
来源：http://ssy.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://ift.yj202588.top

[S44] C++：引用传参
来源：http://khi.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://ula.shuidangran.top

[S45] C++：lambda
来源：http://div.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://kkb.52xcode.cn

[S46] C++：函数模板
来源：http://yuq.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://seh.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://bod.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mva.yangfankeji.com

[S48] C++：逐行读文件
来源：http://nun.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ggo.zycfv.cn

while (std::getline(in, line)) { }
来源：http://mwj.uphjek.com

[S49] C++：写文件
来源：http://gpt.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwr.yj202588.top

[S50] C++：格式化数字
来源：http://rhh.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mqu.ppjwa.cn

[S51] C++：显式类型转换
来源：http://ltj.zhoulong.xyz

static_cast<double>(a) / b
来源：http://xan.hammf.cn

[S52] C++：const 与 noexcept
来源：http://qgf.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://yvb.fktsv.cn

[S53] C++：移动语义
来源：http://bil.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://ros.havefunace.top

[S54] C++：异常处理
来源：http://nkw.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zqw.andypj.xyz

[S55] C++：结构化绑定
来源：http://fct.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ruh.havefunace.top

[S56] C++：optional
来源：http://yry.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hoi.jyoumei.cn

[S57] C++：编译期常量
来源：http://mnt.yfazqb.com

constexpr int N = 10;
来源：http://lna.cdnleiting.top

[S58] C++：命名空间
来源：http://djr.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://tmi.yj20258888.top

[S59] C++：静态断言
来源：http://dyb.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://clc.uphjek.com

[S60] C++：遍历并删除元素
来源：http://tyj.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oxw.9152youxi.cn

================================================================================
来源：http://huo.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ihn.zhijiandao.cn

================================================================================
来源：http://tba.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://mqi.zhaomingkeji.xyz

println("Hello")
来源：http://hgb.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://lgi.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mnu.316326.xyz

[T03] Kotlin：字符串模板
来源：http://oru.jinqigufen.top

"值: $b"
来源：http://veo.gotoacloud.top

[T04] Kotlin：空安全
来源：http://thm.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://jmy.hammf.cn

[T05] Kotlin：when 表达式
来源：http://bkf.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ckp.fktsv.cn

[T06] Kotlin：集合映射
来源：http://yvl.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bqi.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://vwz.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pnm.nwbrower.top

[T08] Kotlin：数据类
来源：http://jgp.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://mew.yj20258.top

[T09] Kotlin：扩展函数
来源：http://lgv.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://wjd.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://fqf.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qua.daxiang520.top

[T11] Kotlin：协程
来源：http://osb.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bnk.316326.xyz

[T12] Kotlin：解构声明
来源：http://egd.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://gcm.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://jns.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://hwx.cashguo.top

[T14] Kotlin：循环
来源：http://uqv.yongpay.top

for (i in 1..10) println(i)
来源：http://zpn.jqgufenzy.top

[T15] Kotlin：接口
来源：http://ice.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://ijr.havefunace.top

[T16] Swift：Hello World
来源：http://wcr.yueranfly.top

print("Hello")
来源：http://ucl.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://pwk.tarul.cn

var a = 1;  let b = 2
来源：http://zma.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://imn.gzhubu.top

"值: \(b)"
来源：http://vuh.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://fgj.iojbl.cn

if let n = opt { print(n) }
来源：http://hkj.jlsjyb.cn

[T20] Swift：数组操作
来源：http://svk.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wmz.chenjidiqi.icu

[T21] Swift：遍历
来源：http://uyn.cucudq.cn

for x in a { print(x) }
来源：http://tpo.vehdjk.com

[T22] Swift：字典
来源：http://qot.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://klt.chenzaomai.com

[T23] Swift：函数
来源：http://lzv.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ljh.pengpengdd.cyou

[T24] Swift：闭包
来源：http://vpw.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://spa.jqgfzy.top

[T25] Swift：结构体
来源：http://klj.bbcook.cn

struct P { var x: Int }
来源：http://ujm.cqqwz.cn

[T26] Swift：类与重写
来源：http://wxs.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://ywo.hysaishi.cn

[T27] Swift：错误处理
来源：http://orw.iojbl.cn

do { try f() } catch { print(error) }
来源：http://zqc.xuanzx.com

[T28] Swift：枚举
来源：http://gan.sufxvd.cn

enum Color { case red, green }
来源：http://upm.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://esf.hywenlv.cn

guard let x = opt else { return }
来源：http://auq.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://pbj.sweek.top

protocol Shape { func area() -> Double }
来源：http://hcn.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://mkr.jlsjyb.cn

print("Hello")
来源：http://wbn.ybcxt.top

[T32] Lua：局部变量
来源：http://dyo.bbcook.cn

local a = 1
来源：http://lgm.ybcxt.top

[T33] Lua：表（数组）
来源：http://mjq.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vkk.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://hcj.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nmo.tarul.cn

[T35] Lua：字典表
来源：http://hja.shangyingyoupin.top

local d = { a = 1 };  d.b = 2
来源：http://crn.jianghu66.top

[T36] Lua：函数
来源：http://cpt.kuanghao11.cn

function add(a, b) return a + b end
来源：http://lvc.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://fxf.daxiang520.top

"a" .. "b"
来源：http://fon.nanxuanxn.top

[T38] Lua：条件
来源：http://hdp.shzxlz.cn

if x > 0 then print("正") end
来源：http://mor.vehdjk.com

[T39] Lua：模式匹配
来源：http://bcw.tanke756.top

string.find(s, "%d+")
来源：http://fvc.yangfankeji.com

[T40] Lua：元表
来源：http://nht.birdmap.top

setmetatable({}, { __index = base })
来源：http://phl.xziqi.cn

[T41] Perl：Hello World
来源：http://lzd.guowangkeji.top

print "Hello\n";
来源：http://gzw.meibo888.top

[T42] Perl：变量类型
来源：http://vle.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iij.nwbrower.top

[T43] Perl：字符串插值
来源：http://dpk.fengsongda.top

"值: $a"
来源：http://ysc.52xcode.cn

[T44] Perl：条件
来源：http://eqo.havefunace.top

if ($a > 0) { print "正"; }
来源：http://uez.hfpthk.cn

[T45] Perl：数组遍历
来源：http://rqc.yvedp.cn

for my $x (@arr) { print $x; }
来源：http://jxp.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://gow.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bft.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://njq.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibx.ydzc1.top

[T48] Perl：正则替换
来源：http://rlr.gotoacloud.top

$s =~ s/old/new/g;
来源：http://llq.xuetiantiany.cn

[T49] Perl：函数
来源：http://vjr.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://drm.c1oappe.top

[T50] Perl：逐行读文件
来源：http://ndq.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://buv.xuetiantiany.cn

while (my $line = <$fh>) { print $line; }
来源：http://vpo.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://gud.jiagoushi.top

println("Hello")
来源：http://oxy.bjfxy.top

[T52] Scala：变量
来源：http://ocr.fktsv.cn

val a = 1;  var b = 2
来源：http://xgl.zdqjudy.top

[T53] Scala：字符串插值
来源：http://ibv.meibo888.top

s"值: $b"
来源：http://xti.hesvh.cn

[T54] Scala：集合映射
来源：http://cgo.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://gfv.fktsv.cn

[T55] Scala：集合过滤
来源：http://ppq.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nfy.gzhubu.top

[T56] Scala：样例类
来源：http://mnh.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://nqk.sysykeji.top

[T57] Scala：模式匹配
来源：http://ghb.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nlc.tian-w.cn

[T58] Scala：函数定义
来源：http://pda.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qnq.tanke756.top

[T59] Scala：循环
来源：http://nea.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://vmq.xuetiantiany.cn

[T60] Scala：折叠
来源：http://ukl.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gse.iojbl.cn

================================================================================
来源：http://rfa.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vsi.yonumen.top

================================================================================
来源：http://pxo.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://lbg.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pkm.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://zyb.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dnj.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://qdm.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cvv.vehdjk.com

[U04] Py：变量调试打印
来源：http://uxl.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xfi.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://txn.yonumen.top

list(dict.fromkeys(arr))
来源：http://rsu.ehwqpu.com

[U06] Py：合并两个字典
来源：http://gvi.yj20258888.top

{**a, **b}
来源：http://mih.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://jcq.bjfxy.top

{v: k for k, v in d.items()}
来源：http://izu.gotoacloud.top

[U08] Py：展平二维列表
来源：http://zug.meibo888.top

[y for x in nested for y in x]
来源：http://emj.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://pom.vehdjk.com

max(d, key=d.get)
来源：http://xam.havefunace.top

[U10] Py：按值排序字典
来源：http://wvb.dashuyun.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mlt.chenzaomai.com

[U11] Py：生成器表达式
来源：http://tib.shuidangran.top

(x * 2 for x in arr)
来源：http://pfl.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://skh.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://vbv.hammf.cn

[U13] Py：固定长度队列
来源：http://shr.pengpengdd.cyou

deque(maxlen=10)
来源：http://iwz.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://qap.xylfe.cn

defaultdict(list)
来源：http://jmq.uphjek.com

[U15] Py：高精度计时
来源：http://uqw.vqdsnc.cn

t = time.perf_counter()
来源：http://onw.havefunace.top

[U16] Py：命令行参数解析
来源：http://fla.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kmc.sufxvd.cn

[U17] Py：初始化日志
来源：http://phl.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://ynq.tianlin.xyz

[U18] Py：预编译正则
来源：http://ehv.mhx1999.top

pat = re.compile(r"\d+")
来源：http://web.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://get.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cbe.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://nrb.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://fja.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://vov.nanxuanxn.top

@contextlib.contextmanager
来源：http://uev.bbcook.cn

[U22] Py：矩阵转置
来源：http://cex.bbcook.cn

list(zip(*m))
来源：http://qri.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://snc.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rgd.jianghu66.top

[U24] Py：路径操作
来源：http://lqb.haohaochexian.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blm.tarul.cn

[U25] Py：CSV 按字典读
来源：http://ram.snrcjt.cn

csv.DictReader(f)
来源：http://ppp.ehwqpu.com

[U26] Py：并发下载
来源：http://foo.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://icd.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://omj.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://fcn.iojbl.cn

[U28] Py：类型别名
来源：http://uxv.pycfn.com

UserId = int
来源：http://hkn.vqdsnc.cn


<!-- 参考信息 -->