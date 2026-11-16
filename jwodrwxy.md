代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://ojr.yonumen.top

[S02] C：变量与格式化输出
来源：http://suz.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://hlu.shuidangran.top

[S03] C：读入整数
来源：http://gpp.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://nwr.ivvv.top

[S04] C：字符串复制
来源：http://tkk.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://ivc.daria6918.cn

[S05] C：字符串长度
来源：http://epr.cashguo.top

strlen(s)
来源：http://emr.yongpay.top

[S06] C：字符串比较
来源：http://vun.redwolf501.top

strcmp(a, b) == 0
来源：http://mag.zhixingplan.top

[S07] C：数组遍历求和
来源：http://vik.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kdo.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://blk.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lwd.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://wir.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oiu.sweek.top

[S10] C：指针与解引用
来源：http://hmx.yvedp.cn

int *p = &a;  *p = 5;
来源：http://pqh.nanxinkj.top

[S11] C：逐行读文件
来源：http://agv.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://mxd.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fvm.svipenyu.cn

fclose(f);
来源：http://xde.yanxiufei.cn

[S12] C：写文件
来源：http://qmd.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rvb.yuanzhike.top

[S13] C：宏定义
来源：http://xje.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://byi.nanxuanxn.top

[S14] C：枚举
来源：http://bhp.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://yqz.jinghuilouyu.cn

[S15] C：类型转换
来源：http://vnd.jinyuanbaomall.cn

(double) a / b
来源：http://yns.jiagoushi.top

[S16] C：位操作置位
来源：http://lte.jianghu66.top

x |= (1 << 3);
来源：http://rbw.tian-w.cn

[S17] C：安全拼接字符串
来源：http://cpx.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://svu.vehdjk.com

[S18] C：命令行参数
来源：http://sfb.shuidangran.top

int main(int argc, char **argv)
来源：http://lbz.yueranfly.top

[S19] C：快速排序
来源：http://ugd.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://vqj.svipenyu.cn

[S20] C：二分查找
来源：http://iid.ydjk.org.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lii.haohaochexian.top

[S21] C：字符类别判断
来源：http://gto.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wgu.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://enk.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ulz.cucudq.cn

[S23] C：随机数
来源：http://mkn.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uro.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://zow.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ozj.andypj.xyz

[S25] C：内存拷贝
来源：http://pbn.vqdsnc.cn

memcpy(dst, src, n);
来源：http://kjj.gotoacloud.top

[S26] C：内存清零
来源：http://qjb.bbcook.cn

memset(a, 0, sizeof a);
来源：http://ntb.meibo888.top

[S27] C：定义常量
来源：http://klx.nanxinkj.top

const double PI = 3.14159;
来源：http://nev.iojbl.cn

[S28] C：静态变量
来源：http://gyi.tian-w.cn

static int counter = 0;
来源：http://iuy.yj20258.top

[S29] C：变参函数
来源：http://npi.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vow.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://tpb.c1oappe.top

#ifndef X_H
来源：http://tsm.9152youxi.cn

#define X_H
来源：http://eir.cdnleiting.top

#endif
来源：http://unv.zycfv.cn

[S31] C++：Hello World
来源：http://qje.hywenlv.cn

#include <iostream>
来源：http://zhp.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://low.yongpay.top

[S32] C++：字符串
来源：http://bzb.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://qit.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://ccr.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://obk.xylfe.cn

[S34] C++：遍历 vector
来源：http://rte.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://ryq.hysaishi.cn

[S35] C++：map
来源：http://jmp.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eui.hnxiangtu.top

[S36] C++：unordered_map
来源：http://txw.fzhhl.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vip.tanke756.top

[S37] C++：set
来源：http://wmw.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ttw.bbcook.cn

[S38] C++：排序
来源：http://rnc.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://zcj.havefunace.top

[S39] C++：自定义比较器排序
来源：http://ndd.gaohongyu789.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://byv.aibaodan.cn

[S40] C++：查找元素
来源：http://zmg.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yuz.jiagoushi.top

[S41] C++：类与构造函数
来源：http://wcv.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ztr.pycfn.com

[S42] C++：继承与虚函数
来源：http://ott.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://vav.xziqi.cn

[S43] C++：智能指针
来源：http://hxm.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://ayi.zycfv.cn

[S44] C++：引用传参
来源：http://bee.bbcook.cn

void inc(int &x) { ++x; }
来源：http://ynx.pycfn.com

[S45] C++：lambda
来源：http://tql.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://mqu.gogol.net.cn

[S46] C++：函数模板
来源：http://xhd.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gyx.sweek.top

[S47] C++：结构化绑定遍历
来源：http://jsu.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jkd.yfazqb.com

[S48] C++：逐行读文件
来源：http://tsy.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://nyi.uphjek.com

while (std::getline(in, line)) { }
来源：http://xbo.jinqigfzy.top

[S49] C++：写文件
来源：http://mpm.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwu.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://ibe.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fko.nanxinkj.top

[S51] C++：显式类型转换
来源：http://pdn.smart0.xyz

static_cast<double>(a) / b
来源：http://zzj.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://tjo.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://jgs.smart0.xyz

[S53] C++：移动语义
来源：http://dsv.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://zic.chenjidiqi.icu

[S54] C++：异常处理
来源：http://euj.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://spv.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://pzu.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vsx.yj202588.top

[S56] C++：optional
来源：http://igb.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kmi.fzhhl.top

[S57] C++：编译期常量
来源：http://plq.zhiwuduotai.top

constexpr int N = 10;
来源：http://qfd.birdmap.top

[S58] C++：命名空间
来源：http://lqx.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://tep.tian-w.cn

[S59] C++：静态断言
来源：http://bwo.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ift.yj202588.top

[S60] C++：遍历并删除元素
来源：http://bxo.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cyq.yangfankeji.com

================================================================================
来源：http://kyu.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnb.hcnkem.com

================================================================================
来源：http://jge.wangdashe.top

[T01] Kotlin：Hello World
来源：http://gkd.zhaomingkeji.xyz

println("Hello")
来源：http://arf.dianchejie.cn

[T02] Kotlin：变量
来源：http://lzc.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wcu.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://tbo.kuanghao11.cn

"值: $b"
来源：http://bhu.hysaishi.cn

[T04] Kotlin：空安全
来源：http://fyb.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://pkb.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://gtb.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uaj.meibo888.top

[T06] Kotlin：集合映射
来源：http://agk.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ftj.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://tau.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ajj.fengsongda.top

[T08] Kotlin：数据类
来源：http://fco.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://lja.uphjek.com

[T09] Kotlin：扩展函数
来源：http://ljl.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://abh.nwbrower.top

[T10] Kotlin：默认参数
来源：http://pcg.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dtr.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://kks.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pqs.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://tcj.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://ouj.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://fze.fktsv.cn

val m = mapOf("a" to 1)
来源：http://uzb.zdbjq.cn

[T14] Kotlin：循环
来源：http://uoi.c1oappe.top

for (i in 1..10) println(i)
来源：http://bev.xuanzx.com

[T15] Kotlin：接口
来源：http://bbk.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://phg.cheryme.top

[T16] Swift：Hello World
来源：http://xgl.feifeiyinyue.top

print("Hello")
来源：http://bgm.dianchejie.cn

[T17] Swift：变量与常量
来源：http://erb.316326.xyz

var a = 1;  let b = 2
来源：http://edh.daria6918.cn

[T18] Swift：字符串插值
来源：http://xuz.daxiang520.top

"值: \(b)"
来源：http://eft.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://fab.kuanghao11.cn

if let n = opt { print(n) }
来源：http://aky.c1oappe.top

[T20] Swift：数组操作
来源：http://cxw.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://skz.0kj1m.cn

[T21] Swift：遍历
来源：http://vtu.yueranfly.top

for x in a { print(x) }
来源：http://ifp.hysaishi.cn

[T22] Swift：字典
来源：http://mue.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pfm.9152youxi.cn

[T23] Swift：函数
来源：http://mfb.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qcl.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://joj.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cir.mhx1999.top

[T25] Swift：结构体
来源：http://kwy.uphjek.com

struct P { var x: Int }
来源：http://qam.9152youxi.cn

[T26] Swift：类与重写
来源：http://lqu.tanke756.top

class A: Base { override func f() {} }
来源：http://ohg.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://dkq.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://vlv.yanxiufei.cn

[T28] Swift：枚举
来源：http://obs.xuetiantiany.cn

enum Color { case red, green }
来源：http://ahn.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://xfq.gotoacloud.top

guard let x = opt else { return }
来源：http://wcl.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://eij.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://mcm.quarkkingdee.top

[T31] Lua：Hello World
来源：http://fgt.ydzc1.top

print("Hello")
来源：http://xdv.uphjek.com

[T32] Lua：局部变量
来源：http://qrj.zhijiandao.cn

local a = 1
来源：http://aqg.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://knd.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://swt.sjlbkw.cn

[T34] Lua：遍历表
来源：http://fay.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://bqa.gotoacloud.top

[T35] Lua：字典表
来源：http://xvu.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://ekc.cashguo.top

[T36] Lua：函数
来源：http://tgt.ivvv.top

function add(a, b) return a + b end
来源：http://mte.xuanzx.com

[T37] Lua：字符串拼接
来源：http://sie.yuxming.cn

"a" .. "b"
来源：http://qce.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://zcr.jlsjyb.cn

if x > 0 then print("正") end
来源：http://lwx.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://hdn.zhengqikj.top

string.find(s, "%d+")
来源：http://zjc.zhoulong.xyz

[T40] Lua：元表
来源：http://inb.yj20258888.top

setmetatable({}, { __index = base })
来源：http://wka.c1oappe.top

[T41] Perl：Hello World
来源：http://uih.zdqjudy.top

print "Hello\n";
来源：http://ipb.zhengqikj.top

[T42] Perl：变量类型
来源：http://may.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fbq.jqgfzy.top

[T43] Perl：字符串插值
来源：http://pvb.wangshuangyany.cn

"值: $a"
来源：http://vjg.hywenlv.cn

[T44] Perl：条件
来源：http://zft.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://nce.hywenlv.cn

[T45] Perl：数组遍历
来源：http://dyd.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://tfu.uphjek.com

[T46] Perl：哈希操作
来源：http://qtu.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dal.yj202588.top

[T47] Perl：正则捕获
来源：http://khq.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kuh.gzhubu.top

[T48] Perl：正则替换
来源：http://hgi.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://egb.9152youxi.cn

[T49] Perl：函数
来源：http://baq.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hci.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://qmo.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eyd.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://xcj.gogol.net.cn

[T51] Scala：Hello World
来源：http://mxk.wangshuangyany.cn

println("Hello")
来源：http://skk.hcnkem.com

[T52] Scala：变量
来源：http://duo.xuanzx.com

val a = 1;  var b = 2
来源：http://kab.sweek.top

[T53] Scala：字符串插值
来源：http://vrl.fzhhl.top

s"值: $b"
来源：http://zud.gogol.net.cn

[T54] Scala：集合映射
来源：http://yum.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://qbt.hysaishi.cn

[T55] Scala：集合过滤
来源：http://zbf.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zlh.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://rxo.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://qzr.snrcjt.cn

[T57] Scala：模式匹配
来源：http://aau.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mij.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://gcw.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://cek.dashuyun.cn

[T59] Scala：循环
来源：http://ymj.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://uig.fehbvm.com

[T60] Scala：折叠
来源：http://udm.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ner.dianchejie.cn

================================================================================
来源：http://cdk.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://teq.zhijiandao.cn

================================================================================
来源：http://ilc.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://xnc.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://xkd.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://zfz.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bdz.316326.xyz

[U03] Py：加载 .env 配置
来源：http://agm.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://skj.vehdjk.com

[U04] Py：变量调试打印
来源：http://lcb.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ihb.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://rgb.daxiang520.top

list(dict.fromkeys(arr))
来源：http://xri.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://jbd.gzhubu.top

{**a, **b}
来源：http://ged.zdbjq.cn

[U07] Py：反转字典键值
来源：http://ajm.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://eko.hfpthk.cn

[U08] Py：展平二维列表
来源：http://hfy.kuanghao11.cn

[y for x in nested for y in x]
来源：http://rde.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://dnx.havefunace.top

max(d, key=d.get)
来源：http://who.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://pnk.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ykk.zhixingplan.top

[U11] Py：生成器表达式
来源：http://mve.jiagoushi.top

(x * 2 for x in arr)
来源：http://kzi.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://ruq.sufxvd.cn

Counter(arr).most_common(3)
来源：http://old.ybcxt.top

[U13] Py：固定长度队列
来源：http://xto.hammf.cn

deque(maxlen=10)
来源：http://ddn.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://thr.hysaishi.cn

defaultdict(list)
来源：http://etz.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://fyz.bjfxy.top

t = time.perf_counter()
来源：http://bqv.redwolf501.top

[U16] Py：命令行参数解析
来源：http://skv.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dvd.ydjk.org.cn

[U17] Py：初始化日志
来源：http://khc.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://vsq.hnxiangtu.top

[U18] Py：预编译正则
来源：http://bci.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://xcy.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://zqr.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://olq.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://cfj.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://ten.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://ocz.yangfankeji.com

@contextlib.contextmanager
来源：http://qpw.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://pyp.cucudq.cn

list(zip(*m))
来源：http://jrp.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://umc.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://red.hammf.cn

[U24] Py：路径操作
来源：http://yjd.guannengcc.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kno.daria6918.cn


<!-- 参考信息 -->