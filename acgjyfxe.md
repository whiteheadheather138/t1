代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://uvu.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://zuw.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://qie.cucudq.cn

[S03] C：读入整数
来源：http://fsq.andypj.xyz

int x; scanf("%d", &x);
来源：http://hrx.ivvv.top

[S04] C：字符串复制
来源：http://jxi.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://bjb.zhongyouzk.top

[S05] C：字符串长度
来源：http://rse.havefunace.top

strlen(s)
来源：http://kvq.gaohongyu789.top

[S06] C：字符串比较
来源：http://uqg.jqgufenzy.top

strcmp(a, b) == 0
来源：http://jej.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://juh.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ngs.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://ygb.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jdy.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://kdx.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evn.ivvv.top

[S10] C：指针与解引用
来源：http://msx.bbcook.cn

int *p = &a;  *p = 5;
来源：http://odb.epnwcf.com

[S11] C：逐行读文件
来源：http://umb.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://gdp.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gfe.yj20258.top

fclose(f);
来源：http://yad.xinyue.icu

[S12] C：写文件
来源：http://szs.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bao.gotoacloud.top

[S13] C：宏定义
来源：http://pmi.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fqy.zdqjudy.top

[S14] C：枚举
来源：http://dnv.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://yej.jqgufenzy.top

[S15] C：类型转换
来源：http://vmm.gzhubu.top

(double) a / b
来源：http://cwj.wangshuangyany.cn

[S16] C：位操作置位
来源：http://tom.jiagoushi.top

x |= (1 << 3);
来源：http://cbf.cheryme.top

[S17] C：安全拼接字符串
来源：http://yhs.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://atp.vehdjk.com

[S18] C：命令行参数
来源：http://bho.dianchejie.cn

int main(int argc, char **argv)
来源：http://ems.epnwcf.com

[S19] C：快速排序
来源：http://duk.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://byt.hnqzz.top

[S20] C：二分查找
来源：http://gor.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fnu.zhijiandao.cn

[S21] C：字符类别判断
来源：http://jls.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xwc.snrcjt.cn

[S22] C：字符串转数字
来源：http://eac.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zme.xziqi.cn

[S23] C：随机数
来源：http://qks.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ije.yfazqb.com

[S24] C：获取本地时间
来源：http://rmf.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ccm.nanxinkj.top

[S25] C：内存拷贝
来源：http://qnq.cqqwz.cn

memcpy(dst, src, n);
来源：http://djs.hongshengwenyu.top

[S26] C：内存清零
来源：http://bcy.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://yjf.zhijiandao.cn

[S27] C：定义常量
来源：http://eyr.hnqzz.top

const double PI = 3.14159;
来源：http://wpk.fehbvm.com

[S28] C：静态变量
来源：http://mxc.sxryk.cn

static int counter = 0;
来源：http://ocu.fehbvm.com

[S29] C：变参函数
来源：http://hin.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dbu.redwolf501.top

[S30] C：头文件保护
来源：http://hgc.smart0.xyz

#ifndef X_H
来源：http://czs.yonumen.top

#define X_H
来源：http://yzs.wangdashe.top

#endif
来源：http://sli.havefunace.top

[S31] C++：Hello World
来源：http://zks.sjlbkw.cn

#include <iostream>
来源：http://hah.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://hhk.feifeiyinyue.top

[S32] C++：字符串
来源：http://lnb.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://jfa.daxiang520.top

[S33] C++：vector 增删
来源：http://ohr.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://swx.svipenyu.cn

[S34] C++：遍历 vector
来源：http://gby.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://wkb.ppjwa.cn

[S35] C++：map
来源：http://bsp.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xsr.yj20258888.top

[S36] C++：unordered_map
来源：http://brw.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://plj.svipenyu.cn

[S37] C++：set
来源：http://phx.feifeiyinyue.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nvn.zhixingplan.top

[S38] C++：排序
来源：http://zbi.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://vvb.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://npi.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gzq.fktsv.cn

[S40] C++：查找元素
来源：http://hgb.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dfd.ehwqpu.com

[S41] C++：类与构造函数
来源：http://nrj.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://suy.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://spb.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://xxt.quarkkingdee.top

[S43] C++：智能指针
来源：http://fmf.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://btg.kuanghao11.cn

[S44] C++：引用传参
来源：http://ygq.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://wqq.hesvh.cn

[S45] C++：lambda
来源：http://xnh.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://gnc.zhiwuduotai.top

[S46] C++：函数模板
来源：http://tmu.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wcq.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://xci.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ckx.52xcode.cn

[S48] C++：逐行读文件
来源：http://yzi.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://lpm.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://dvs.snrcjt.cn

[S49] C++：写文件
来源：http://hqd.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ebs.yfazqb.com

[S50] C++：格式化数字
来源：http://agk.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zqj.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://tck.ydzc1.top

static_cast<double>(a) / b
来源：http://kuu.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://uht.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://skl.zhoulong.xyz

[S53] C++：移动语义
来源：http://thn.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://uki.redwolf501.top

[S54] C++：异常处理
来源：http://wnl.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ofy.fehbvm.com

[S55] C++：结构化绑定
来源：http://kat.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mop.quarkkingdee.top

[S56] C++：optional
来源：http://ylc.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wxb.zhongyouzk.top

[S57] C++：编译期常量
来源：http://skg.nwbrower.top

constexpr int N = 10;
来源：http://xwg.nwbrower.top

[S58] C++：命名空间
来源：http://ghi.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://dho.guannengcc.top

[S59] C++：静态断言
来源：http://gdn.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vab.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://box.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fhd.epnwcf.com

================================================================================
来源：http://zwy.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpc.dashuyun.cn

================================================================================
来源：http://zqv.smart0.xyz

[T01] Kotlin：Hello World
来源：http://hpm.hcnkem.com

println("Hello")
来源：http://qgw.zycfv.cn

[T02] Kotlin：变量
来源：http://lyj.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ogb.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://zuo.gogol.net.cn

"值: $b"
来源：http://evf.zhixingplan.top

[T04] Kotlin：空安全
来源：http://tmf.gogol.net.cn

val n: String? = null;  n?.length
来源：http://fid.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://oal.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gjy.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://rir.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zrf.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://lcy.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://klb.pycfn.com

[T08] Kotlin：数据类
来源：http://ryr.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://voy.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://lpg.havefunace.top

fun String.exclaim() = this + "!"
来源：http://vvt.bbcook.cn

[T10] Kotlin：默认参数
来源：http://tkh.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://khp.jlsjyb.cn

[T11] Kotlin：协程
来源：http://flr.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hwl.birdmap.top

[T12] Kotlin：解构声明
来源：http://mbx.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://iea.pycfn.com

[T13] Kotlin：只读 Map
来源：http://aqn.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://wmt.jinqigufen.top

[T14] Kotlin：循环
来源：http://klz.yongpay.top

for (i in 1..10) println(i)
来源：http://sfz.zycfv.cn

[T15] Kotlin：接口
来源：http://gfc.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://rmv.nanxuanxn.top

[T16] Swift：Hello World
来源：http://ynk.jinqigufen.top

print("Hello")
来源：http://gyf.ctjpmb.com

[T17] Swift：变量与常量
来源：http://jlg.yanxiufei.cn

var a = 1;  let b = 2
来源：http://sra.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://zug.bjfxy.top

"值: \(b)"
来源：http://jug.nwbrower.top

[T19] Swift：可选绑定
来源：http://jfd.cqqwz.cn

if let n = opt { print(n) }
来源：http://dnq.vqdsnc.cn

[T20] Swift：数组操作
来源：http://idz.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://ucz.pycfn.com

[T21] Swift：遍历
来源：http://jix.vqdsnc.cn

for x in a { print(x) }
来源：http://jme.snrcjt.cn

[T22] Swift：字典
来源：http://ewx.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://zxw.jqgfzy.top

[T23] Swift：函数
来源：http://nfq.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rjg.mhx1999.top

[T24] Swift：闭包
来源：http://sqw.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qcy.yanxiufei.cn

[T25] Swift：结构体
来源：http://wlo.cqqwz.cn

struct P { var x: Int }
来源：http://tnx.vehdjk.com

[T26] Swift：类与重写
来源：http://hlr.hcnkem.com

class A: Base { override func f() {} }
来源：http://cxi.snrcjt.cn

[T27] Swift：错误处理
来源：http://jml.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://xwz.xylfe.cn

[T28] Swift：枚举
来源：http://ynt.hcnkem.com

enum Color { case red, green }
来源：http://nds.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://gvm.yj20258888.top

guard let x = opt else { return }
来源：http://nsk.ehwqpu.com

[T30] Swift：协议
来源：http://nsr.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://ovg.iojbl.cn

[T31] Lua：Hello World
来源：http://jhp.jqgfzy.top

print("Hello")
来源：http://rxp.hnqzz.top

[T32] Lua：局部变量
来源：http://sht.ydzc1.top

local a = 1
来源：http://cgb.jiagoushi.top

[T33] Lua：表（数组）
来源：http://izx.zhixingplan.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uwe.cucudq.cn

[T34] Lua：遍历表
来源：http://lrh.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://uox.jiagoushi.top

[T35] Lua：字典表
来源：http://owb.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://ttk.feifeiyinyue.top

[T36] Lua：函数
来源：http://oss.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://ffx.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://fnb.cqqwz.cn

"a" .. "b"
来源：http://hpm.fktsv.cn

[T38] Lua：条件
来源：http://izi.jinqigufen.top

if x > 0 then print("正") end
来源：http://rqv.316326.xyz

[T39] Lua：模式匹配
来源：http://rpq.iojbl.cn

string.find(s, "%d+")
来源：http://jft.yanxiufei.cn

[T40] Lua：元表
来源：http://kwg.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://swm.kuanghao11.cn

[T41] Perl：Hello World
来源：http://vli.dashuyun.cn

print "Hello\n";
来源：http://cdd.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://tbu.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cos.guannengcc.top

[T43] Perl：字符串插值
来源：http://hql.jyoumei.cn

"值: $a"
来源：http://bkp.sweek.top

[T44] Perl：条件
来源：http://eru.tanke756.top

if ($a > 0) { print "正"; }
来源：http://lei.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://eys.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://uwu.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://val.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wzk.cqqwz.cn

[T47] Perl：正则捕获
来源：http://htj.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://usr.c1oappe.top

[T48] Perl：正则替换
来源：http://xgr.ivvv.top

$s =~ s/old/new/g;
来源：http://mgc.hammf.cn

[T49] Perl：函数
来源：http://rhu.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://url.fengsongda.top

[T50] Perl：逐行读文件
来源：http://muw.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://byo.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://swq.jianghu66.top

[T51] Scala：Hello World
来源：http://tvn.dianchejie.cn

println("Hello")
来源：http://qrp.sjlbkw.cn

[T52] Scala：变量
来源：http://qgg.ybcxt.top

val a = 1;  var b = 2
来源：http://evx.aibaodan.cn

[T53] Scala：字符串插值
来源：http://wrl.zhaomingkeji.xyz

s"值: $b"
来源：http://dwi.hfpthk.cn

[T54] Scala：集合映射
来源：http://evk.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://ref.0kj1m.cn

[T55] Scala：集合过滤
来源：http://qkm.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://ulh.fzhhl.top

[T56] Scala：样例类
来源：http://tdn.shuidangran.top

case class User(name: String, age: Int)
来源：http://npd.chenzaomai.com

[T57] Scala：模式匹配
来源：http://bnz.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tka.fzhhl.top

[T58] Scala：函数定义
来源：http://qgf.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jdw.sjlbkw.cn

[T59] Scala：循环
来源：http://zqf.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://orv.zdqjudy.top

[T60] Scala：折叠
来源：http://rza.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bdl.tarul.cn

================================================================================
来源：http://wfi.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ugc.yueranfly.top

================================================================================
来源：http://pab.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://wck.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://yap.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://pzl.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iyy.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://jkp.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hdu.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://dji.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ecd.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://wuc.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://fbe.gogol.net.cn

[U06] Py：合并两个字典
来源：http://wyj.xingfuxueyuan.xyz

{**a, **b}
来源：http://cor.yangfankeji.com

[U07] Py：反转字典键值
来源：http://buz.wangdashe.top

{v: k for k, v in d.items()}
来源：http://qeh.jqgfzy.top

[U08] Py：展平二维列表
来源：http://fae.0kj1m.cn

[y for x in nested for y in x]
来源：http://ixv.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://dpg.jinqigufen.top

max(d, key=d.get)
来源：http://rrh.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://nra.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bqe.chenlongwang.top

[U11] Py：生成器表达式
来源：http://wqw.guowangkeji.top

(x * 2 for x in arr)
来源：http://xpu.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://csn.ivvv.top

Counter(arr).most_common(3)
来源：http://mnj.0kj1m.cn

[U13] Py：固定长度队列
来源：http://zst.hnqzz.top

deque(maxlen=10)
来源：http://dcq.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://pjr.jinghuilouyu.cn

defaultdict(list)
来源：http://iga.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://oza.316326.xyz

t = time.perf_counter()
来源：http://tph.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://kby.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sbt.quarkkingdee.top

[U17] Py：初始化日志
来源：http://vrf.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://aec.jyoumei.cn

[U18] Py：预编译正则
来源：http://rwh.hnqzz.top

pat = re.compile(r"\d+")
来源：http://zwn.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://oza.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ppg.redwolf501.top

[U20] Py：缓存函数结果
来源：http://jax.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://wxl.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://lto.c1oappe.top

@contextlib.contextmanager
来源：http://jzx.fengsongda.top

[U22] Py：矩阵转置
来源：http://mpr.sweek.top

list(zip(*m))
来源：http://bcj.daria6918.cn

[U23] Py：分块读取大文件
来源：http://uec.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ccw.fktsv.cn

[U24] Py：路径操作
来源：http://scn.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nyu.wangdashe.top


<!-- 参考信息 -->