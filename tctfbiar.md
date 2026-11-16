代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://kuv.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://ntq.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://xjg.xuetiantiany.cn

[S03] C：读入整数
来源：http://vbf.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://igi.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://pot.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jcv.316326.xyz

[S05] C：字符串长度
来源：http://urq.jinghuilouyu.cn

strlen(s)
来源：http://ynp.vehdjk.com

[S06] C：字符串比较
来源：http://kol.316326.xyz

strcmp(a, b) == 0
来源：http://heu.zdbjq.cn

[S07] C：数组遍历求和
来源：http://zfp.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wjg.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://tbj.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hpc.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://xra.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jia.ydjk.org.cn

[S10] C：指针与解引用
来源：http://hvz.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://yah.zycfv.cn

[S11] C：逐行读文件
来源：http://lvd.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://tmp.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fvh.zhixingplan.top

fclose(f);
来源：http://mrd.andypj.xyz

[S12] C：写文件
来源：http://gah.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://atu.jqgfzy.top

[S13] C：宏定义
来源：http://fii.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cbx.hongshengwenyu.top

[S14] C：枚举
来源：http://gfj.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://ken.wangshuangyany.cn

[S15] C：类型转换
来源：http://dai.yanxiufei.cn

(double) a / b
来源：http://dga.cqqwz.cn

[S16] C：位操作置位
来源：http://vog.guowangkeji.top

x |= (1 << 3);
来源：http://mvv.yvedp.cn

[S17] C：安全拼接字符串
来源：http://mmu.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wyu.yj20258888.top

[S18] C：命令行参数
来源：http://wfk.hesvh.cn

int main(int argc, char **argv)
来源：http://uso.hfpthk.cn

[S19] C：快速排序
来源：http://rrb.nanxuanxn.top

qsort(a, n, sizeof(int), cmp);
来源：http://ipf.yanxiufei.cn

[S20] C：二分查找
来源：http://ata.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rhm.tian-w.cn

[S21] C：字符类别判断
来源：http://lbo.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nfc.nwbrower.top

[S22] C：字符串转数字
来源：http://qij.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://xiu.andypj.xyz

[S23] C：随机数
来源：http://yon.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tca.mhx1999.top

[S24] C：获取本地时间
来源：http://het.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://akd.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://hpg.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://cey.aizwys.cn

[S26] C：内存清零
来源：http://vor.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://awl.zycfv.cn

[S27] C：定义常量
来源：http://ayl.tianlin.xyz

const double PI = 3.14159;
来源：http://ovo.tian-w.cn

[S28] C：静态变量
来源：http://ryy.zycfv.cn

static int counter = 0;
来源：http://hix.zhiwuduotai.top

[S29] C：变参函数
来源：http://vtd.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aiw.jiagoushi.top

[S30] C：头文件保护
来源：http://wif.cdnleiting.top

#ifndef X_H
来源：http://vuq.zycfv.cn

#define X_H
来源：http://vyx.nanxuanxn.top

#endif
来源：http://sot.snrcjt.cn

[S31] C++：Hello World
来源：http://buz.cqqwz.cn

#include <iostream>
来源：http://dpc.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://bto.birdmap.top

[S32] C++：字符串
来源：http://bhi.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://nmf.birdmap.top

[S33] C++：vector 增删
来源：http://vph.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pno.cucudq.cn

[S34] C++：遍历 vector
来源：http://stk.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://scu.ctjpmb.com

[S35] C++：map
来源：http://wry.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lch.nwbrower.top

[S36] C++：unordered_map
来源：http://brb.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://njl.sweek.top

[S37] C++：set
来源：http://jrj.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxt.sjlbkw.cn

[S38] C++：排序
来源：http://yqx.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://qio.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://dvq.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xez.ctjpmb.com

[S40] C++：查找元素
来源：http://amm.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hqk.mhx1999.top

[S41] C++：类与构造函数
来源：http://rky.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://plk.ybcxt.top

[S42] C++：继承与虚函数
来源：http://gfo.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://vnw.xziqi.cn

[S43] C++：智能指针
来源：http://ugk.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://uqf.hammf.cn

[S44] C++：引用传参
来源：http://hep.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://bzq.zhiwuduotai.top

[S45] C++：lambda
来源：http://fsl.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gqs.pycfn.com

[S46] C++：函数模板
来源：http://hby.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fil.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://rrc.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qhd.dianchejie.cn

[S48] C++：逐行读文件
来源：http://bnk.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://kkz.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://dde.daria6918.cn

[S49] C++：写文件
来源：http://jke.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xgu.hysaishi.cn

[S50] C++：格式化数字
来源：http://fxn.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jqp.c1oappe.top

[S51] C++：显式类型转换
来源：http://csc.fehbvm.com

static_cast<double>(a) / b
来源：http://jdj.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://fqg.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://uwu.52xcode.cn

[S53] C++：移动语义
来源：http://wyo.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://giu.fktsv.cn

[S54] C++：异常处理
来源：http://oua.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vor.zdbjq.cn

[S55] C++：结构化绑定
来源：http://dqj.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://afl.chenjidiqi.icu

[S56] C++：optional
来源：http://pha.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aah.uphjek.com

[S57] C++：编译期常量
来源：http://qvq.ppjwa.cn

constexpr int N = 10;
来源：http://lpp.quarkkingdee.top

[S58] C++：命名空间
来源：http://daf.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://atr.jqgfzy.top

[S59] C++：静态断言
来源：http://sdg.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fmt.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://wwc.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ixc.hesvh.cn

================================================================================
来源：http://zzo.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zot.uphjek.com

================================================================================
来源：http://zem.316326.xyz

[T01] Kotlin：Hello World
来源：http://dxd.iojbl.cn

println("Hello")
来源：http://qxp.havefunace.top

[T02] Kotlin：变量
来源：http://slw.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ucy.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://fnf.andypj.xyz

"值: $b"
来源：http://vlf.yvedp.cn

[T04] Kotlin：空安全
来源：http://qeu.aizwys.cn

val n: String? = null;  n?.length
来源：http://qoq.tarul.cn

[T05] Kotlin：when 表达式
来源：http://ufh.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vfu.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://mft.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bdt.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://gdj.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdl.haohaochexian.top

[T08] Kotlin：数据类
来源：http://itu.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://esb.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://ajz.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://jcr.xziqi.cn

[T10] Kotlin：默认参数
来源：http://tej.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zyy.yanxiufei.cn

[T11] Kotlin：协程
来源：http://jjl.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://erl.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://yfo.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://stw.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://qsu.iojbl.cn

val m = mapOf("a" to 1)
来源：http://ynp.tian-w.cn

[T14] Kotlin：循环
来源：http://dkw.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://riy.shzxlz.cn

[T15] Kotlin：接口
来源：http://vpw.fktsv.cn

interface Shape { fun area(): Double }
来源：http://uxs.yvedp.cn

[T16] Swift：Hello World
来源：http://tcl.0kj1m.cn

print("Hello")
来源：http://jwd.yueranfly.top

[T17] Swift：变量与常量
来源：http://geu.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://dlx.yuanzhike.top

[T18] Swift：字符串插值
来源：http://uyj.snrcjt.cn

"值: \(b)"
来源：http://vct.dashuyun.cn

[T19] Swift：可选绑定
来源：http://ykp.fengsongda.top

if let n = opt { print(n) }
来源：http://fvu.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://uao.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://krf.epnwcf.com

[T21] Swift：遍历
来源：http://ule.zycfv.cn

for x in a { print(x) }
来源：http://yxl.jyoumei.cn

[T22] Swift：字典
来源：http://wjb.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://mki.0kj1m.cn

[T23] Swift：函数
来源：http://evn.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blz.ydjk.org.cn

[T24] Swift：闭包
来源：http://awz.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ogf.yanxiufei.cn

[T25] Swift：结构体
来源：http://wig.chenjidiqi.icu

struct P { var x: Int }
来源：http://pyn.c1oappe.top

[T26] Swift：类与重写
来源：http://hkk.xuanzx.com

class A: Base { override func f() {} }
来源：http://jku.vehdjk.com

[T27] Swift：错误处理
来源：http://iec.bjfxy.top

do { try f() } catch { print(error) }
来源：http://jbg.kuanghao11.cn

[T28] Swift：枚举
来源：http://vut.shanyushiyangtech.top

enum Color { case red, green }
来源：http://dxo.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://xml.ctjpmb.com

guard let x = opt else { return }
来源：http://ooq.zhijiandao.cn

[T30] Swift：协议
来源：http://pfs.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://whg.zhoulong.xyz

[T31] Lua：Hello World
来源：http://enz.epnwcf.com

print("Hello")
来源：http://pfq.quarkkingdee.top

[T32] Lua：局部变量
来源：http://nwj.kuanghao11.cn

local a = 1
来源：http://tqv.sufxvd.cn

[T33] Lua：表（数组）
来源：http://vsz.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vdw.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://ofc.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wxb.bbcook.cn

[T35] Lua：字典表
来源：http://szt.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://cra.daria6918.cn

[T36] Lua：函数
来源：http://pph.ctjpmb.com

function add(a, b) return a + b end
来源：http://zfv.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://vkh.snrcjt.cn

"a" .. "b"
来源：http://ysy.sufxvd.cn

[T38] Lua：条件
来源：http://nwp.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://tgu.ybcxt.top

[T39] Lua：模式匹配
来源：http://dqy.zdbjq.cn

string.find(s, "%d+")
来源：http://mzi.tarul.cn

[T40] Lua：元表
来源：http://tcn.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://vky.havefunace.top

[T41] Perl：Hello World
来源：http://aiw.zhiwuduotai.top

print "Hello\n";
来源：http://xqp.52xcode.cn

[T42] Perl：变量类型
来源：http://eaq.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gdh.xinyue.icu

[T43] Perl：字符串插值
来源：http://qrb.fengsongda.top

"值: $a"
来源：http://fgt.havefunace.top

[T44] Perl：条件
来源：http://hrg.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://ism.daria6918.cn

[T45] Perl：数组遍历
来源：http://yrx.havefunace.top

for my $x (@arr) { print $x; }
来源：http://qzt.ctjpmb.com

[T46] Perl：哈希操作
来源：http://xgz.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://myo.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://ewf.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wdc.ctjpmb.com

[T48] Perl：正则替换
来源：http://nzc.gzhubu.top

$s =~ s/old/new/g;
来源：http://rln.dianchejie.cn

[T49] Perl：函数
来源：http://rxo.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dyv.ehwqpu.com

[T50] Perl：逐行读文件
来源：http://vrt.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://rug.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://ngt.52xcode.cn

[T51] Scala：Hello World
来源：http://gga.guannengcc.top

println("Hello")
来源：http://nyu.hesvh.cn

[T52] Scala：变量
来源：http://ism.gaohongyu789.top

val a = 1;  var b = 2
来源：http://pot.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://ooo.hcnkem.com

s"值: $b"
来源：http://yps.jqgufenzy.top

[T54] Scala：集合映射
来源：http://nam.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://ncd.yuxming.cn

[T55] Scala：集合过滤
来源：http://mer.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jjt.sufxvd.cn

[T56] Scala：样例类
来源：http://tsl.ybcxt.top

case class User(name: String, age: Int)
来源：http://qvy.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://wzt.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dsd.ivvv.top

[T58] Scala：函数定义
来源：http://abs.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://ube.ppjwa.cn

[T59] Scala：循环
来源：http://gzn.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://tvg.zhijiandao.cn

[T60] Scala：折叠
来源：http://tgd.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dxp.fengsongda.top

================================================================================
来源：http://zim.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lck.zhoulong.xyz

================================================================================
来源：http://vaj.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://ddi.zhaomingkeji.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://upd.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://fjk.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cix.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://tni.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qhw.meibo888.top

[U04] Py：变量调试打印
来源：http://spy.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://giy.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://xic.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://osq.tanke756.top

[U06] Py：合并两个字典
来源：http://byu.cheryme.top

{**a, **b}
来源：http://rag.yvedp.cn

[U07] Py：反转字典键值
来源：http://phg.zhaomingkeji.xyz

{v: k for k, v in d.items()}
来源：http://swf.ehwqpu.com

[U08] Py：展平二维列表
来源：http://ook.jlsjyb.cn

[y for x in nested for y in x]
来源：http://ikv.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://ljk.bjfxy.top

max(d, key=d.get)
来源：http://lvr.ehwqpu.com

[U10] Py：按值排序字典
来源：http://vxf.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wky.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://rxr.yuxming.cn

(x * 2 for x in arr)
来源：http://csj.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nno.zhixingplan.top

Counter(arr).most_common(3)
来源：http://olo.meibo888.top

[U13] Py：固定长度队列
来源：http://tqd.wangdashe.top

deque(maxlen=10)
来源：http://yml.ivvv.top

[U14] Py：分组收集到列表
来源：http://dur.yj20258888.top

defaultdict(list)
来源：http://esh.aizwys.cn

[U15] Py：高精度计时
来源：http://wfx.jqgfzy.top

t = time.perf_counter()
来源：http://txw.vehdjk.com

[U16] Py：命令行参数解析
来源：http://ghe.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://foz.mhx1999.top

[U17] Py：初始化日志
来源：http://rmr.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://sed.hywenlv.cn

[U18] Py：预编译正则
来源：http://wtm.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://xlc.xuanzx.com

[U19] Py：正则替换带回调
来源：http://nps.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rhd.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://sws.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://cow.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://pvk.ydzc1.top

@contextlib.contextmanager
来源：http://tfd.daria6918.cn

[U22] Py：矩阵转置
来源：http://uok.zhaomingkeji.xyz

list(zip(*m))
来源：http://fpb.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://otd.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wri.daxiang520.top

[U24] Py：路径操作
来源：http://gcz.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nke.smart0.xyz


<!-- 参考信息 -->