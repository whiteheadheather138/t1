代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://ldq.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://nmp.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://wcy.hesvh.cn

[S03] C：读入整数
来源：http://yjo.yuxming.cn

int x; scanf("%d", &x);
来源：http://tvx.redwolf501.top

[S04] C：字符串复制
来源：http://qyg.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://jvm.gotoacloud.top

[S05] C：字符串长度
来源：http://epa.yonumen.top

strlen(s)
来源：http://lti.cucudq.cn

[S06] C：字符串比较
来源：http://ohr.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://jds.tian-w.cn

[S07] C：数组遍历求和
来源：http://nar.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lch.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://fzf.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://niv.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://rmu.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jay.gotoacloud.top

[S10] C：指针与解引用
来源：http://iad.tanke756.top

int *p = &a;  *p = 5;
来源：http://qnk.ivvv.top

[S11] C：逐行读文件
来源：http://lhm.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://kiq.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dio.c1oappe.top

fclose(f);
来源：http://njl.dashuyun.cn

[S12] C：写文件
来源：http://vjb.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baf.feifeiyinyue.top

[S13] C：宏定义
来源：http://xzq.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ois.uphjek.com

[S14] C：枚举
来源：http://xge.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://gpb.yueranfly.top

[S15] C：类型转换
来源：http://rjm.hammf.cn

(double) a / b
来源：http://zlb.gzhubu.top

[S16] C：位操作置位
来源：http://dar.uphjek.com

x |= (1 << 3);
来源：http://mae.yj202588.top

[S17] C：安全拼接字符串
来源：http://moz.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dbp.wangdashe.top

[S18] C：命令行参数
来源：http://mhs.vqdsnc.cn

int main(int argc, char **argv)
来源：http://kam.hammf.cn

[S19] C：快速排序
来源：http://syk.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wtf.shuidangran.top

[S20] C：二分查找
来源：http://axj.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lnd.hfpthk.cn

[S21] C：字符类别判断
来源：http://ofn.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxk.iojbl.cn

[S22] C：字符串转数字
来源：http://xtb.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://fgs.zhixingplan.top

[S23] C：随机数
来源：http://reo.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oxj.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://ihk.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://okj.zhengqikj.top

[S25] C：内存拷贝
来源：http://qnd.daria6918.cn

memcpy(dst, src, n);
来源：http://aud.tanke756.top

[S26] C：内存清零
来源：http://rjq.yvedp.cn

memset(a, 0, sizeof a);
来源：http://lfo.hongshengwenyu.top

[S27] C：定义常量
来源：http://abx.nanxinkj.top

const double PI = 3.14159;
来源：http://xyl.jlsjyb.cn

[S28] C：静态变量
来源：http://rax.chenlongwang.top

static int counter = 0;
来源：http://ubu.cucudq.cn

[S29] C：变参函数
来源：http://wch.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rul.shzxlz.cn

[S30] C：头文件保护
来源：http://xlz.yj20258888.top

#ifndef X_H
来源：http://yoc.bbcook.cn

#define X_H
来源：http://hry.yfazqb.com

#endif
来源：http://wtc.yanxiufei.cn

[S31] C++：Hello World
来源：http://arj.yuxming.cn

#include <iostream>
来源：http://hdc.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://iju.nanxuanxn.top

[S32] C++：字符串
来源：http://ivw.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://xru.tarul.cn

[S33] C++：vector 增删
来源：http://ack.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hmx.ivvv.top

[S34] C++：遍历 vector
来源：http://ldj.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://nkl.cdnleiting.top

[S35] C++：map
来源：http://bsm.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://scl.vehdjk.com

[S36] C++：unordered_map
来源：http://lgb.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vfi.mhx1999.top

[S37] C++：set
来源：http://ayk.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://drx.chenlongwang.top

[S38] C++：排序
来源：http://oup.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://trv.tarul.cn

[S39] C++：自定义比较器排序
来源：http://gzv.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wcj.ydzc1.top

[S40] C++：查找元素
来源：http://hjz.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jtq.dianchejie.cn

[S41] C++：类与构造函数
来源：http://cqm.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xhb.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://lds.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://rlp.tarul.cn

[S43] C++：智能指针
来源：http://nrd.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://xcu.iojbl.cn

[S44] C++：引用传参
来源：http://tpg.ybcxt.top

void inc(int &x) { ++x; }
来源：http://amj.yueranfly.top

[S45] C++：lambda
来源：http://efa.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://vdj.pycfn.com

[S46] C++：函数模板
来源：http://adv.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zjy.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://fsn.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xfs.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://yxo.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://akb.cashguo.top

while (std::getline(in, line)) { }
来源：http://gpf.ctjpmb.com

[S49] C++：写文件
来源：http://ufy.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://veu.gaohongyu789.top

[S50] C++：格式化数字
来源：http://kuq.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hbb.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://vfq.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://rve.pycfn.com

[S52] C++：const 与 noexcept
来源：http://lxy.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://znl.guowangkeji.top

[S53] C++：移动语义
来源：http://jaz.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://coq.shuidangran.top

[S54] C++：异常处理
来源：http://mjt.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gbe.epnwcf.com

[S55] C++：结构化绑定
来源：http://uoh.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fcd.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://uqd.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dck.yj202588.top

[S57] C++：编译期常量
来源：http://yto.cucudq.cn

constexpr int N = 10;
来源：http://rpi.zhiwuduotai.top

[S58] C++：命名空间
来源：http://vgd.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://tco.52xcode.cn

[S59] C++：静态断言
来源：http://qtq.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rcy.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://siw.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dsj.hfpthk.cn

================================================================================
来源：http://hhl.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xot.shanyushiyangtech.top

================================================================================
来源：http://zuy.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://cks.guowangkeji.top

println("Hello")
来源：http://phf.daria6918.cn

[T02] Kotlin：变量
来源：http://jip.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ahj.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://lgo.ybcxt.top

"值: $b"
来源：http://xov.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://lad.yj20258888.top

val n: String? = null;  n?.length
来源：http://efo.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://uyf.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ihb.shuidangran.top

[T06] Kotlin：集合映射
来源：http://pkx.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pnw.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://aiw.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dsx.snrcjt.cn

[T08] Kotlin：数据类
来源：http://ffy.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://pxs.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://xjk.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://qoz.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://mwt.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ilz.aizwys.cn

[T11] Kotlin：协程
来源：http://uff.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://pye.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://jmq.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://zqk.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://khu.cheryme.top

val m = mapOf("a" to 1)
来源：http://mcn.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://cvn.smart0.xyz

for (i in 1..10) println(i)
来源：http://emz.haohaochexian.top

[T15] Kotlin：接口
来源：http://yct.hesvh.cn

interface Shape { fun area(): Double }
来源：http://dof.ydjk.org.cn

[T16] Swift：Hello World
来源：http://ltb.daxiang520.top

print("Hello")
来源：http://egr.aibaodan.cn

[T17] Swift：变量与常量
来源：http://qeq.ppjwa.cn

var a = 1;  let b = 2
来源：http://wcc.yvedp.cn

[T18] Swift：字符串插值
来源：http://twx.aibaodan.cn

"值: \(b)"
来源：http://exy.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://apr.mhx1999.top

if let n = opt { print(n) }
来源：http://lbt.zhongyouzk.top

[T20] Swift：数组操作
来源：http://qzw.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qde.cqqwz.cn

[T21] Swift：遍历
来源：http://zwf.hammf.cn

for x in a { print(x) }
来源：http://ggk.redwolf501.top

[T22] Swift：字典
来源：http://lqq.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://ugy.sysykeji.top

[T23] Swift：函数
来源：http://lmh.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sos.gogol.net.cn

[T24] Swift：闭包
来源：http://pmz.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yvn.cucudq.cn

[T25] Swift：结构体
来源：http://zra.meibo888.top

struct P { var x: Int }
来源：http://yiv.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://jts.tarul.cn

class A: Base { override func f() {} }
来源：http://cwu.fehbvm.com

[T27] Swift：错误处理
来源：http://uxo.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://dhv.birdmap.top

[T28] Swift：枚举
来源：http://dyr.hfpthk.cn

enum Color { case red, green }
来源：http://vsr.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://etw.jqgufenzy.top

guard let x = opt else { return }
来源：http://mef.tian-w.cn

[T30] Swift：协议
来源：http://bub.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://tjh.hcnkem.com

[T31] Lua：Hello World
来源：http://tws.tian-w.cn

print("Hello")
来源：http://kqe.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://hca.jianghu66.top

local a = 1
来源：http://xos.gogol.net.cn

[T33] Lua：表（数组）
来源：http://aif.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lsi.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://wig.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://boh.yangfankeji.com

[T35] Lua：字典表
来源：http://rvx.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://tzm.tanke756.top

[T36] Lua：函数
来源：http://org.yonumen.top

function add(a, b) return a + b end
来源：http://gku.smart0.xyz

[T37] Lua：字符串拼接
来源：http://cvr.fzhhl.top

"a" .. "b"
来源：http://vsf.hongshengwenyu.top

[T38] Lua：条件
来源：http://gts.quarkkingdee.top

if x > 0 then print("正") end
来源：http://lsr.hnqzz.top

[T39] Lua：模式匹配
来源：http://adv.ctjpmb.com

string.find(s, "%d+")
来源：http://asx.andypj.xyz

[T40] Lua：元表
来源：http://hxp.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://ceo.iojbl.cn

[T41] Perl：Hello World
来源：http://lxt.zhongyouzk.top

print "Hello\n";
来源：http://pjq.nanxuanxn.top

[T42] Perl：变量类型
来源：http://wbw.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ixg.hammf.cn

[T43] Perl：字符串插值
来源：http://idb.yj20258888.top

"值: $a"
来源：http://bop.hnxiangtu.top

[T44] Perl：条件
来源：http://rgn.cheryme.top

if ($a > 0) { print "正"; }
来源：http://ott.ehwqpu.com

[T45] Perl：数组遍历
来源：http://jkz.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://msr.chenlongwang.top

[T46] Perl：哈希操作
来源：http://wec.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ndf.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://dgj.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vui.jianghu66.top

[T48] Perl：正则替换
来源：http://lab.dianchejie.cn

$s =~ s/old/new/g;
来源：http://lff.gogol.net.cn

[T49] Perl：函数
来源：http://isw.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rhx.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://ogh.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://emg.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://iri.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://pwm.hongshengwenyu.top

println("Hello")
来源：http://dqs.sjlbkw.cn

[T52] Scala：变量
来源：http://mmj.52xcode.cn

val a = 1;  var b = 2
来源：http://yrt.iojbl.cn

[T53] Scala：字符串插值
来源：http://wlh.hysaishi.cn

s"值: $b"
来源：http://ymn.hammf.cn

[T54] Scala：集合映射
来源：http://lnj.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://iha.ydzc1.top

[T55] Scala：集合过滤
来源：http://zyj.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://gta.yfazqb.com

[T56] Scala：样例类
来源：http://lpk.svipenyu.cn

case class User(name: String, age: Int)
来源：http://kxq.xinyue.icu

[T57] Scala：模式匹配
来源：http://okw.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://omi.zdqjudy.top

[T58] Scala：函数定义
来源：http://jsd.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://epb.cdnleiting.top

[T59] Scala：循环
来源：http://dqw.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://dwz.yuanzhike.top

[T60] Scala：折叠
来源：http://ugd.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dro.andypj.xyz

================================================================================
来源：http://izi.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://boh.sweek.top

================================================================================
来源：http://rak.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://pgq.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://wdc.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://awv.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ftq.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://jou.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://eby.316326.xyz

[U04] Py：变量调试打印
来源：http://ygn.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bih.yvedp.cn

[U05] Py：列表去重且保序
来源：http://kep.hesvh.cn

list(dict.fromkeys(arr))
来源：http://gdd.zycfv.cn

[U06] Py：合并两个字典
来源：http://fmd.tanke756.top

{**a, **b}
来源：http://fae.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://eet.yfazqb.com

{v: k for k, v in d.items()}
来源：http://oux.andypj.xyz

[U08] Py：展平二维列表
来源：http://ixt.nwbrower.top

[y for x in nested for y in x]
来源：http://lsy.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://vdd.jiagoushi.top

max(d, key=d.get)
来源：http://cso.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://fbq.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ghv.havefunace.top

[U11] Py：生成器表达式
来源：http://hrf.c1oappe.top

(x * 2 for x in arr)
来源：http://tad.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://txr.xylfe.cn

Counter(arr).most_common(3)
来源：http://vqi.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://jzz.xinyue.icu

deque(maxlen=10)
来源：http://haw.xziqi.cn

[U14] Py：分组收集到列表
来源：http://uhf.chenjidiqi.icu

defaultdict(list)
来源：http://oex.ydjk.org.cn

[U15] Py：高精度计时
来源：http://yxd.ppjwa.cn

t = time.perf_counter()
来源：http://opu.yonumen.top

[U16] Py：命令行参数解析
来源：http://txr.316326.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dir.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://taq.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://gvw.cqqwz.cn

[U18] Py：预编译正则
来源：http://jqm.redwolf501.top

pat = re.compile(r"\d+")
来源：http://dpm.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://tnq.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mkj.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://lny.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://joc.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://dwr.c1oappe.top

@contextlib.contextmanager
来源：http://jpc.dashuyun.cn

[U22] Py：矩阵转置
来源：http://wfy.aizwys.cn

list(zip(*m))
来源：http://qan.tarul.cn

[U23] Py：分块读取大文件
来源：http://ymh.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wrv.gogol.net.cn

[U24] Py：路径操作
来源：http://iwh.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hek.dashuyun.cn


<!-- 参考信息 -->