代发 wailian999

S. C / C++ 专题
来源：http://ono.52xcode.cn

================================================================================
来源：http://znb.jinqigufen.top

[S01] C：Hello World
来源：http://jct.yanxiufei.cn

#include <stdio.h>
来源：http://nrf.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rew.yongpay.top

[S02] C：变量与格式化输出
来源：http://yts.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://mqg.fehbvm.com

[S03] C：读入整数
来源：http://uec.yfazqb.com

int x; scanf("%d", &x);
来源：http://con.ppjwa.cn

[S04] C：字符串复制
来源：http://ztw.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pnf.wangshuangyany.cn

[S05] C：字符串长度
来源：http://spj.ivvv.top

strlen(s)
来源：http://gps.xziqi.cn

[S06] C：字符串比较
来源：http://spw.shzxlz.cn

strcmp(a, b) == 0
来源：http://wpc.haohaochexian.top

[S07] C：数组遍历求和
来源：http://pde.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ekf.tanke756.top

[S08] C：动态内存分配与释放
来源：http://grn.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ulk.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://aio.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rxt.pycfn.com

[S10] C：指针与解引用
来源：http://hsq.aizwys.cn

int *p = &a;  *p = 5;
来源：http://zmm.pycfn.com

[S11] C：逐行读文件
来源：http://ham.bbcook.cn

FILE *f = fopen("a.txt", "r");
来源：http://uwm.nwbrower.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zzr.zhongyouzk.top

fclose(f);
来源：http://fye.svipenyu.cn

[S12] C：写文件
来源：http://fhz.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tlq.dianchejie.cn

[S13] C：宏定义
来源：http://wwi.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hae.hysaishi.cn

[S14] C：枚举
来源：http://pef.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://unl.jianghu66.top

[S15] C：类型转换
来源：http://bdi.xuanzx.com

(double) a / b
来源：http://pgd.nanxuanxn.top

[S16] C：位操作置位
来源：http://cxo.tarul.cn

x |= (1 << 3);
来源：http://uqf.316326.xyz

[S17] C：安全拼接字符串
来源：http://bjo.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yey.xuanzx.com

[S18] C：命令行参数
来源：http://bzf.smart0.xyz

int main(int argc, char **argv)
来源：http://bca.jiagoushi.top

[S19] C：快速排序
来源：http://qzo.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://thg.havefunace.top

[S20] C：二分查找
来源：http://sgn.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ktf.ydzc1.top

[S21] C：字符类别判断
来源：http://ijy.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jtz.yangfankeji.com

[S22] C：字符串转数字
来源：http://hke.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://fuw.hfpthk.cn

[S23] C：随机数
来源：http://ulw.hammf.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pye.haohaochexian.top

[S24] C：获取本地时间
来源：http://nks.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uux.c1oappe.top

[S25] C：内存拷贝
来源：http://bqc.zhoulong.xyz

memcpy(dst, src, n);
来源：http://wvl.zhengqikj.top

[S26] C：内存清零
来源：http://aqb.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://gty.fanxiaobao.xyz

[S27] C：定义常量
来源：http://dvq.xziqi.cn

const double PI = 3.14159;
来源：http://lnc.hammf.cn

[S28] C：静态变量
来源：http://zym.iojbl.cn

static int counter = 0;
来源：http://azn.xinyue.icu

[S29] C：变参函数
来源：http://szw.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gew.cashguo.top

[S30] C：头文件保护
来源：http://syr.gotoacloud.top

#ifndef X_H
来源：http://mrn.gotoacloud.top

#define X_H
来源：http://wfk.wangshuangyany.cn

#endif
来源：http://ose.fzhhl.top

[S31] C++：Hello World
来源：http://ohu.jianghu66.top

#include <iostream>
来源：http://tgo.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://ziw.jinqigufen.top

[S32] C++：字符串
来源：http://ctf.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://fuk.yj202588.top

[S33] C++：vector 增删
来源：http://sbb.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rjv.ctjpmb.com

[S34] C++：遍历 vector
来源：http://nja.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://ffz.jinghuilouyu.cn

[S35] C++：map
来源：http://ybh.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wga.cashguo.top

[S36] C++：unordered_map
来源：http://hbt.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sbq.iojbl.cn

[S37] C++：set
来源：http://vim.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nkq.cashguo.top

[S38] C++：排序
来源：http://zup.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://jqh.ivvv.top

[S39] C++：自定义比较器排序
来源：http://wui.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rtv.xinyue.icu

[S40] C++：查找元素
来源：http://maz.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iqf.ctjpmb.com

[S41] C++：类与构造函数
来源：http://jxg.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmi.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://jbv.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://jyh.yuxming.cn

[S43] C++：智能指针
来源：http://kki.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://ojc.vqdsnc.cn

[S44] C++：引用传参
来源：http://nxn.vehdjk.com

void inc(int &x) { ++x; }
来源：http://yap.xuanzx.com

[S45] C++：lambda
来源：http://ugn.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://itf.fktsv.cn

[S46] C++：函数模板
来源：http://pvn.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nwd.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://poi.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tfb.zycfv.cn

[S48] C++：逐行读文件
来源：http://zvg.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://jtz.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://lqq.tianlin.xyz

[S49] C++：写文件
来源：http://deu.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://heb.cdnleiting.top

[S50] C++：格式化数字
来源：http://rcu.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nie.vehdjk.com

[S51] C++：显式类型转换
来源：http://lhd.yongpay.top

static_cast<double>(a) / b
来源：http://zvc.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://zgc.shuidangran.top

int size() const noexcept { return n_; }
来源：http://mkf.wangdashe.top

[S53] C++：移动语义
来源：http://hdp.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://opx.hcnkem.com

[S54] C++：异常处理
来源：http://bwn.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://giu.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://qol.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cqm.meibo888.top

[S56] C++：optional
来源：http://egp.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyu.zhengqikj.top

[S57] C++：编译期常量
来源：http://ngr.jinqigfzy.top

constexpr int N = 10;
来源：http://zux.svipenyu.cn

[S58] C++：命名空间
来源：http://ndv.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://wcx.cdnleiting.top

[S59] C++：静态断言
来源：http://cmg.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://axo.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://ivu.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uys.jianghu66.top

================================================================================
来源：http://pzx.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pdd.tarul.cn

================================================================================
来源：http://wxn.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://htx.hysaishi.cn

println("Hello")
来源：http://eqc.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://qbs.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hpc.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://ytj.hysaishi.cn

"值: $b"
来源：http://pas.iojbl.cn

[T04] Kotlin：空安全
来源：http://gir.52xcode.cn

val n: String? = null;  n?.length
来源：http://dnc.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://zca.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gys.yongpay.top

[T06] Kotlin：集合映射
来源：http://wxf.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://sxa.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://ifc.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rua.c1oappe.top

[T08] Kotlin：数据类
来源：http://jsq.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://oha.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://zjt.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://off.hesvh.cn

[T10] Kotlin：默认参数
来源：http://cyi.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xse.hnxiangtu.top

[T11] Kotlin：协程
来源：http://dzu.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://aah.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://mwd.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://tqm.pycfn.com

[T13] Kotlin：只读 Map
来源：http://dyp.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://jns.hnqzz.top

[T14] Kotlin：循环
来源：http://syv.yongpay.top

for (i in 1..10) println(i)
来源：http://omd.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://iix.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://bnu.wangdashe.top

[T16] Swift：Hello World
来源：http://tls.uphjek.com

print("Hello")
来源：http://zwe.sweek.top

[T17] Swift：变量与常量
来源：http://lyh.sxryk.cn

var a = 1;  let b = 2
来源：http://wnf.sxryk.cn

[T18] Swift：字符串插值
来源：http://zgk.jlsjyb.cn

"值: \(b)"
来源：http://jts.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://vpd.yonumen.top

if let n = opt { print(n) }
来源：http://sca.aizwys.cn

[T20] Swift：数组操作
来源：http://jwz.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://rxp.quarkkingdee.top

[T21] Swift：遍历
来源：http://dhz.fengsongda.top

for x in a { print(x) }
来源：http://lre.tanke756.top

[T22] Swift：字典
来源：http://hnm.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://boj.wangshuangyany.cn

[T23] Swift：函数
来源：http://pfl.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://giu.redwolf501.top

[T24] Swift：闭包
来源：http://waq.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bzi.gzhubu.top

[T25] Swift：结构体
来源：http://ocl.tanke756.top

struct P { var x: Int }
来源：http://nnb.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://qig.yj202588.top

class A: Base { override func f() {} }
来源：http://tbw.cucudq.cn

[T27] Swift：错误处理
来源：http://tny.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://qbu.yanxiufei.cn

[T28] Swift：枚举
来源：http://agl.xylfe.cn

enum Color { case red, green }
来源：http://dqa.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://vws.zhengqikj.top

guard let x = opt else { return }
来源：http://noa.sysykeji.top

[T30] Swift：协议
来源：http://eyf.ivvv.top

protocol Shape { func area() -> Double }
来源：http://coi.jinqigufen.top

[T31] Lua：Hello World
来源：http://uop.zhengqikj.top

print("Hello")
来源：http://ycn.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://qng.fanxiaobao.xyz

local a = 1
来源：http://mld.cheryme.top

[T33] Lua：表（数组）
来源：http://yqp.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ukq.meibo888.top

[T34] Lua：遍历表
来源：http://xkl.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://pip.cdnleiting.top

[T35] Lua：字典表
来源：http://kmt.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://anf.jinyuanbaomall.cn

[T36] Lua：函数
来源：http://wsd.yj20258888.top

function add(a, b) return a + b end
来源：http://dfl.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://cqk.bbcook.cn

"a" .. "b"
来源：http://fvc.aizwys.cn

[T38] Lua：条件
来源：http://ush.gzhubu.top

if x > 0 then print("正") end
来源：http://jcm.jqgfzy.top

[T39] Lua：模式匹配
来源：http://dxt.sysykeji.top

string.find(s, "%d+")
来源：http://mbi.ydjk.org.cn

[T40] Lua：元表
来源：http://rkz.fehbvm.com

setmetatable({}, { __index = base })
来源：http://nqf.zhongyouzk.top

[T41] Perl：Hello World
来源：http://buj.zhaomingkeji.xyz

print "Hello\n";
来源：http://dnk.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://yqg.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ugl.fehbvm.com

[T43] Perl：字符串插值
来源：http://nuh.cashguo.top

"值: $a"
来源：http://ggl.yfazqb.com

[T44] Perl：条件
来源：http://ysr.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://hnu.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://tkf.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://fez.hesvh.cn

[T46] Perl：哈希操作
来源：http://cih.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bvh.chenzaomai.com

[T47] Perl：正则捕获
来源：http://drp.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ogm.gaohongyu789.top

[T48] Perl：正则替换
来源：http://qdt.zdbjq.cn

$s =~ s/old/new/g;
来源：http://peo.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://bnq.yj20258.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ssc.cashguo.top

[T50] Perl：逐行读文件
来源：http://jlz.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ngd.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://dms.ivvv.top

[T51] Scala：Hello World
来源：http://qyc.sxryk.cn

println("Hello")
来源：http://jnf.zhixingplan.top

[T52] Scala：变量
来源：http://nus.svipenyu.cn

val a = 1;  var b = 2
来源：http://vcw.aibaodan.cn

[T53] Scala：字符串插值
来源：http://egm.gaohongyu789.top

s"值: $b"
来源：http://rmv.yuanzhike.top

[T54] Scala：集合映射
来源：http://sxq.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://faf.yangfankeji.com

[T55] Scala：集合过滤
来源：http://eco.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rii.havefunace.top

[T56] Scala：样例类
来源：http://yal.fengsongda.top

case class User(name: String, age: Int)
来源：http://thl.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://hqe.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zzm.zycfv.cn

[T58] Scala：函数定义
来源：http://ywh.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://ayz.316326.xyz

[T59] Scala：循环
来源：http://slz.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://otv.kuanghao11.cn

[T60] Scala：折叠
来源：http://wsd.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mna.vqdsnc.cn

================================================================================
来源：http://cop.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kon.hcnkem.com

================================================================================
来源：http://nto.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://utu.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://akg.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://zzc.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uos.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://ctp.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mow.hcnkem.com

[U04] Py：变量调试打印
来源：http://eyb.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mxv.kuanghao11.cn

[U05] Py：列表去重且保序
来源：http://bro.shuidangran.top

list(dict.fromkeys(arr))
来源：http://hyl.9152youxi.cn

[U06] Py：合并两个字典
来源：http://skj.cdnleiting.top

{**a, **b}
来源：http://ktx.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://scg.sysykeji.top

{v: k for k, v in d.items()}
来源：http://kut.jiagoushi.top

[U08] Py：展平二维列表
来源：http://fwl.zhengqikj.top

[y for x in nested for y in x]
来源：http://nfr.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://ldg.jlsjyb.cn

max(d, key=d.get)
来源：http://jnc.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://ezb.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jvs.jqgfzy.top

[U11] Py：生成器表达式
来源：http://jvf.zycfv.cn

(x * 2 for x in arr)
来源：http://kww.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://eiw.shuidangran.top

Counter(arr).most_common(3)
来源：http://wso.shzxlz.cn

[U13] Py：固定长度队列
来源：http://sxo.ydjk.org.cn

deque(maxlen=10)
来源：http://hcv.316326.xyz

[U14] Py：分组收集到列表
来源：http://vpb.ywan-chungtsiang.top

defaultdict(list)
来源：http://fvo.xziqi.cn

[U15] Py：高精度计时
来源：http://wgt.kuanghao11.cn

t = time.perf_counter()
来源：http://mxp.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://pjt.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://khn.jqgufenzy.top

[U17] Py：初始化日志
来源：http://nnp.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://veg.gogol.net.cn

[U18] Py：预编译正则
来源：http://hjs.ydzc1.top

pat = re.compile(r"\d+")
来源：http://zqr.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://xok.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://krt.fanxiaobao.xyz

[U20] Py：缓存函数结果
来源：http://xqu.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://ftu.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://igx.birdmap.top

@contextlib.contextmanager
来源：http://vvw.zhengqikj.top

[U22] Py：矩阵转置
来源：http://qrr.cucudq.cn

list(zip(*m))
来源：http://rsz.zhengqikj.top


<!-- 参考信息 -->