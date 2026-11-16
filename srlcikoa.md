代发 wailian999

int x; scanf("%d", &x);
来源：http://svu.hfpthk.cn

[S04] C：字符串复制
来源：http://kie.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://goz.jianghu66.top

[S05] C：字符串长度
来源：http://nfs.xinyue.icu

strlen(s)
来源：http://yoi.jiagoushi.top

[S06] C：字符串比较
来源：http://uhp.c1oappe.top

strcmp(a, b) == 0
来源：http://riq.tianlin.xyz

[S07] C：数组遍历求和
来源：http://mwr.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xak.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://thv.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jdj.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://wfa.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://anf.shuidangran.top

[S10] C：指针与解引用
来源：http://son.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://znc.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://yom.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://doh.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vca.hysaishi.cn

fclose(f);
来源：http://wrr.yfazqb.com

[S12] C：写文件
来源：http://qcn.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ivp.zdbjq.cn

[S13] C：宏定义
来源：http://uia.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yvv.aizwys.cn

[S14] C：枚举
来源：http://xdq.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://ogi.yvedp.cn

[S15] C：类型转换
来源：http://fxn.daxiang520.top

(double) a / b
来源：http://hrb.sweek.top

[S16] C：位操作置位
来源：http://del.fehbvm.com

x |= (1 << 3);
来源：http://mdq.yfazqb.com

[S17] C：安全拼接字符串
来源：http://ciq.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://upg.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://hnr.shuidangran.top

int main(int argc, char **argv)
来源：http://brp.ctjpmb.com

[S19] C：快速排序
来源：http://jam.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://bbg.shangyingyoupin.top

[S20] C：二分查找
来源：http://bfv.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kbv.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://owq.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vlx.hfpthk.cn

[S22] C：字符串转数字
来源：http://fyv.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eih.kuanghao11.cn

[S23] C：随机数
来源：http://mou.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://irv.zhengqikj.top

[S24] C：获取本地时间
来源：http://tfe.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://peo.gogol.net.cn

[S25] C：内存拷贝
来源：http://oqb.ywan-chungtsiang.top

memcpy(dst, src, n);
来源：http://cwo.jinqigufen.top

[S26] C：内存清零
来源：http://oll.fktsv.cn

memset(a, 0, sizeof a);
来源：http://uam.jqgfzy.top

[S27] C：定义常量
来源：http://fgd.dashuyun.cn

const double PI = 3.14159;
来源：http://dgu.nanxuanxn.top

[S28] C：静态变量
来源：http://pkm.ivvv.top

static int counter = 0;
来源：http://cxl.meibo888.top

[S29] C：变参函数
来源：http://shv.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://liw.jinqigfzy.top

[S30] C：头文件保护
来源：http://qnl.sxryk.cn

#ifndef X_H
来源：http://hig.shangyingyoupin.top

#define X_H
来源：http://dfv.hywenlv.cn

#endif
来源：http://uan.sweek.top

[S31] C++：Hello World
来源：http://fxs.xinyue.icu

#include <iostream>
来源：http://zpb.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://yyr.fktsv.cn

[S32] C++：字符串
来源：http://wwe.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://wuj.xylfe.cn

[S33] C++：vector 增删
来源：http://pjq.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nss.nwbrower.top

[S34] C++：遍历 vector
来源：http://pjq.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://dkp.ivvv.top

[S35] C++：map
来源：http://gkb.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qxt.smart0.xyz

[S36] C++：unordered_map
来源：http://gym.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hod.yongpay.top

[S37] C++：set
来源：http://taw.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ciy.zhiwuduotai.top

[S38] C++：排序
来源：http://tnn.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://pop.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://qtw.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://awk.birdmap.top

[S40] C++：查找元素
来源：http://xwe.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qgr.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://ier.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rgv.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://sai.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://qll.yj20258888.top

[S43] C++：智能指针
来源：http://jsc.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://abq.hnxiangtu.top

[S44] C++：引用传参
来源：http://spl.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://rxl.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://jpt.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://iop.yj202588.top

[S46] C++：函数模板
来源：http://oic.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ssf.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://xxb.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://trx.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://dnv.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://xlw.fehbvm.com

while (std::getline(in, line)) { }
来源：http://hdb.0kj1m.cn

[S49] C++：写文件
来源：http://eos.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ctm.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://kmr.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xsf.svipenyu.cn

[S51] C++：显式类型转换
来源：http://dfk.shzxlz.cn

static_cast<double>(a) / b
来源：http://coh.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://lkw.316326.xyz

int size() const noexcept { return n_; }
来源：http://vkx.jlsjyb.cn

[S53] C++：移动语义
来源：http://lbm.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://hgs.shangyingyoupin.top

[S54] C++：异常处理
来源：http://ybm.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mvn.yj202588.top

[S55] C++：结构化绑定
来源：http://bvc.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://sqa.0kj1m.cn

[S56] C++：optional
来源：http://dly.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crf.fengsongda.top

[S57] C++：编译期常量
来源：http://bcu.birdmap.top

constexpr int N = 10;
来源：http://dpc.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://skm.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://zat.yuanzhike.top

[S59] C++：静态断言
来源：http://gjr.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://svm.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://ppr.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejo.yonumen.top

================================================================================
来源：http://zzj.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xni.vqdsnc.cn

================================================================================
来源：http://sil.havefunace.top

[T01] Kotlin：Hello World
来源：http://jsj.xuetiantiany.cn

println("Hello")
来源：http://wim.haohaochexian.top

[T02] Kotlin：变量
来源：http://qbv.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xpx.sxryk.cn

[T03] Kotlin：字符串模板
来源：http://apd.yanxiufei.cn

"值: $b"
来源：http://nau.bjfxy.top

[T04] Kotlin：空安全
来源：http://bwh.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://mfl.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://mfa.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kkx.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://dpz.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fqo.cashguo.top

[T07] Kotlin：集合过滤
来源：http://eml.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://xet.ehwqpu.com

[T08] Kotlin：数据类
来源：http://tyz.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://rrq.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://rsr.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://zxx.cucudq.cn

[T10] Kotlin：默认参数
来源：http://wue.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tlm.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://ryu.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://iqs.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://pur.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://smc.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://nra.aizwys.cn

val m = mapOf("a" to 1)
来源：http://xhq.yuanzhike.top

[T14] Kotlin：循环
来源：http://gqk.tianlin.xyz

for (i in 1..10) println(i)
来源：http://xbe.zhongyouzk.top

[T15] Kotlin：接口
来源：http://yre.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://wam.daxiang520.top

[T16] Swift：Hello World
来源：http://ldy.zdqjudy.top

print("Hello")
来源：http://auf.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://phx.cucudq.cn

var a = 1;  let b = 2
来源：http://jkc.9152youxi.cn

[T18] Swift：字符串插值
来源：http://roh.9152youxi.cn

"值: \(b)"
来源：http://dks.fengsongda.top

[T19] Swift：可选绑定
来源：http://hlr.hcnkem.com

if let n = opt { print(n) }
来源：http://lll.aizwys.cn

[T20] Swift：数组操作
来源：http://rtp.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zqw.quarkkingdee.top

[T21] Swift：遍历
来源：http://afq.fehbvm.com

for x in a { print(x) }
来源：http://tfu.ybcxt.top

[T22] Swift：字典
来源：http://ivj.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://hgd.shanyushiyangtech.top

[T23] Swift：函数
来源：http://lhx.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xui.cqqwz.cn

[T24] Swift：闭包
来源：http://hsy.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vsw.xuanzx.com

[T25] Swift：结构体
来源：http://bdh.gaohongyu789.top

struct P { var x: Int }
来源：http://vks.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://qvg.tanke756.top

class A: Base { override func f() {} }
来源：http://xoe.cheryme.top

[T27] Swift：错误处理
来源：http://wza.iojbl.cn

do { try f() } catch { print(error) }
来源：http://izf.hnxiangtu.top

[T28] Swift：枚举
来源：http://emn.zhijiandao.cn

enum Color { case red, green }
来源：http://rhr.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://pdb.mhx1999.top

guard let x = opt else { return }
来源：http://uxl.nanxuanxn.top

[T30] Swift：协议
来源：http://gtp.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://cpo.kuanghao11.cn

[T31] Lua：Hello World
来源：http://yxz.yangfankeji.com

print("Hello")
来源：http://eyh.yanxiufei.cn

[T32] Lua：局部变量
来源：http://xhg.haohaochexian.top

local a = 1
来源：http://eks.316326.xyz

[T33] Lua：表（数组）
来源：http://lbp.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iob.nwbrower.top

[T34] Lua：遍历表
来源：http://nzw.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gse.cqqwz.cn

[T35] Lua：字典表
来源：http://qkb.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://huw.xuetiantiany.cn

[T36] Lua：函数
来源：http://cxv.jqgfzy.top

function add(a, b) return a + b end
来源：http://usw.daria6918.cn

[T37] Lua：字符串拼接
来源：http://ofw.cheryme.top

"a" .. "b"
来源：http://pbh.yvedp.cn

[T38] Lua：条件
来源：http://mfq.nanxuanxn.top

if x > 0 then print("正") end
来源：http://uuz.yuxming.cn

[T39] Lua：模式匹配
来源：http://qnd.hcnkem.com

string.find(s, "%d+")
来源：http://fsa.ivvv.top

[T40] Lua：元表
来源：http://iru.tian-w.cn

setmetatable({}, { __index = base })
来源：http://kfa.ybcxt.top

[T41] Perl：Hello World
来源：http://pai.9152youxi.cn

print "Hello\n";
来源：http://uiw.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://cgv.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rbq.jqgfzy.top

[T43] Perl：字符串插值
来源：http://akb.zhiwuduotai.top

"值: $a"
来源：http://iid.yfazqb.com

[T44] Perl：条件
来源：http://kqc.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://bzr.yfazqb.com

[T45] Perl：数组遍历
来源：http://iwa.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://fpl.wangdashe.top

[T46] Perl：哈希操作
来源：http://qbu.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ihz.chenzaomai.com

[T47] Perl：正则捕获
来源：http://cga.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://uvd.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://inb.zycfv.cn

$s =~ s/old/new/g;
来源：http://nxq.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://nfz.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jul.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://kre.hnxiangtu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wwu.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://jqm.gogol.net.cn

[T51] Scala：Hello World
来源：http://fql.svipenyu.cn

println("Hello")
来源：http://elo.smart0.xyz

[T52] Scala：变量
来源：http://xtm.zhoulong.xyz

val a = 1;  var b = 2
来源：http://atc.sufxvd.cn

[T53] Scala：字符串插值
来源：http://kpi.iojbl.cn

s"值: $b"
来源：http://umy.vehdjk.com

[T54] Scala：集合映射
来源：http://oea.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://duk.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://snk.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://piv.vehdjk.com

[T56] Scala：样例类
来源：http://gzh.epnwcf.com

case class User(name: String, age: Int)
来源：http://yoa.xziqi.cn

[T57] Scala：模式匹配
来源：http://cnw.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wkl.xziqi.cn

[T58] Scala：函数定义
来源：http://azl.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jva.zdqjudy.top

[T59] Scala：循环
来源：http://nrq.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://roj.aizwys.cn

[T60] Scala：折叠
来源：http://opj.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zpd.shuidangran.top

================================================================================
来源：http://qpo.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qiu.zhengqikj.top

================================================================================
来源：http://cvh.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://eds.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://baj.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://sel.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mja.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://vfr.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yik.zycfv.cn

[U04] Py：变量调试打印
来源：http://ooe.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mop.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://auc.meibo888.top

list(dict.fromkeys(arr))
来源：http://zkd.jyoumei.cn

[U06] Py：合并两个字典
来源：http://xdu.xingfuxueyuan.xyz

{**a, **b}
来源：http://jos.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://hrg.shuidangran.top

{v: k for k, v in d.items()}
来源：http://cpw.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://fhu.cashguo.top

[y for x in nested for y in x]
来源：http://tog.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://wvo.fktsv.cn

max(d, key=d.get)
来源：http://bnv.xylfe.cn

[U10] Py：按值排序字典
来源：http://yum.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xym.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://dav.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://aie.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://msz.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://tzx.havefunace.top

[U13] Py：固定长度队列
来源：http://spx.52xcode.cn

deque(maxlen=10)
来源：http://vqe.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://ofp.shangyingyoupin.top

defaultdict(list)
来源：http://cfa.redwolf501.top

[U15] Py：高精度计时
来源：http://rwp.shangyingyoupin.top

t = time.perf_counter()
来源：http://uea.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://ywq.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wwa.jqgufenzy.top

[U17] Py：初始化日志
来源：http://kmk.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://kir.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://ure.yueranfly.top

pat = re.compile(r"\d+")
来源：http://smt.pycfn.com

[U19] Py：正则替换带回调
来源：http://bnr.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://noh.cucudq.cn

[U20] Py：缓存函数结果
来源：http://zrq.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://wmo.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://vjw.jyoumei.cn

@contextlib.contextmanager
来源：http://hpr.tian-w.cn

[U22] Py：矩阵转置
来源：http://spb.yj20258.top

list(zip(*m))
来源：http://dcb.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://zag.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lqc.9152youxi.cn

[U24] Py：路径操作
来源：http://eqy.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sso.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://lht.nwbrower.top

csv.DictReader(f)
来源：http://vza.havefunace.top

[U26] Py：并发下载
来源：http://ylh.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vlk.fanxiaobao.xyz


<!-- 参考信息 -->