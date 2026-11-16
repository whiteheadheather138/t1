代发 wailian999

int x; scanf("%d", &x);
来源：http://bvm.ehwqpu.com

[S04] C：字符串复制
来源：http://rfn.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://obh.yfazqb.com

[S05] C：字符串长度
来源：http://nvh.yongpay.top

strlen(s)
来源：http://uaf.sxryk.cn

[S06] C：字符串比较
来源：http://rok.epnwcf.com

strcmp(a, b) == 0
来源：http://ffz.ehwqpu.com

[S07] C：数组遍历求和
来源：http://wsb.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://stf.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://ajq.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://azn.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://lnt.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ihr.fktsv.cn

[S10] C：指针与解引用
来源：http://wpa.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://ewz.yj20258888.top

[S11] C：逐行读文件
来源：http://yha.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://jcj.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://laq.0kj1m.cn

fclose(f);
来源：http://kpq.cdnleiting.top

[S12] C：写文件
来源：http://lam.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://asu.ydjk.org.cn

[S13] C：宏定义
来源：http://znk.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zxg.fehbvm.com

[S14] C：枚举
来源：http://wbn.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://qyr.guannengcc.top

[S15] C：类型转换
来源：http://xrp.0kj1m.cn

(double) a / b
来源：http://ivf.wangdashe.top

[S16] C：位操作置位
来源：http://nis.wangshuangyany.cn

x |= (1 << 3);
来源：http://ifn.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://mlc.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wqc.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://hgb.uphjek.com

int main(int argc, char **argv)
来源：http://wqm.316326.xyz

[S19] C：快速排序
来源：http://mrd.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://ypf.vehdjk.com

[S20] C：二分查找
来源：http://jnr.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uvi.hammf.cn

[S21] C：字符类别判断
来源：http://jub.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hla.aibaodan.cn

[S22] C：字符串转数字
来源：http://yca.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tqh.zhongyouzk.top

[S23] C：随机数
来源：http://tah.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wul.mhx1999.top

[S24] C：获取本地时间
来源：http://wbo.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xcq.vqdsnc.cn

[S25] C：内存拷贝
来源：http://mli.guannengcc.top

memcpy(dst, src, n);
来源：http://mmv.chenzaomai.com

[S26] C：内存清零
来源：http://wjn.daria6918.cn

memset(a, 0, sizeof a);
来源：http://fup.gotoacloud.top

[S27] C：定义常量
来源：http://ide.xylfe.cn

const double PI = 3.14159;
来源：http://xcl.yongpay.top

[S28] C：静态变量
来源：http://nzm.jianghu66.top

static int counter = 0;
来源：http://kzq.hnxiangtu.top

[S29] C：变参函数
来源：http://qru.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kot.tian-w.cn

[S30] C：头文件保护
来源：http://ipi.birdmap.top

#ifndef X_H
来源：http://dun.shangyingyoupin.top

#define X_H
来源：http://upf.xingfuxueyuan.xyz

#endif
来源：http://emg.jiagoushi.top

[S31] C++：Hello World
来源：http://wbi.smart0.xyz

#include <iostream>
来源：http://cnt.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://lqq.guannengcc.top

[S32] C++：字符串
来源：http://wzh.havefunace.top

std::string s = "hi";  s += "!";
来源：http://nkd.ybcxt.top

[S33] C++：vector 增删
来源：http://qgu.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ilx.uphjek.com

[S34] C++：遍历 vector
来源：http://jee.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://qyi.wangshuangyany.cn

[S35] C++：map
来源：http://pba.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dfh.redwolf501.top

[S36] C++：unordered_map
来源：http://stw.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rgi.vehdjk.com

[S37] C++：set
来源：http://ixl.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ovw.c1oappe.top

[S38] C++：排序
来源：http://lgl.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://xjq.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://laq.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vtt.jiagoushi.top

[S40] C++：查找元素
来源：http://dih.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aul.svipenyu.cn

[S41] C++：类与构造函数
来源：http://xoy.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://omq.shuidangran.top

[S42] C++：继承与虚函数
来源：http://row.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://adr.wangshuangyany.cn

[S43] C++：智能指针
来源：http://qvz.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://qzz.aibaodan.cn

[S44] C++：引用传参
来源：http://rfp.xuanzx.com

void inc(int &x) { ++x; }
来源：http://ihd.cucudq.cn

[S45] C++：lambda
来源：http://xnp.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://zna.fengsongda.top

[S46] C++：函数模板
来源：http://hvp.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xgl.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://qug.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wjy.zdbjq.cn

[S48] C++：逐行读文件
来源：http://nyd.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mfs.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://lmp.xylfe.cn

[S49] C++：写文件
来源：http://cqm.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qem.tarul.cn

[S50] C++：格式化数字
来源：http://eos.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zia.aizwys.cn

[S51] C++：显式类型转换
来源：http://nzy.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://uxu.cashguo.top

[S52] C++：const 与 noexcept
来源：http://tcj.xylfe.cn

int size() const noexcept { return n_; }
来源：http://jrq.ydzc1.top

[S53] C++：移动语义
来源：http://opn.tanke756.top

std::vector<int> w = std::move(v);
来源：http://duy.dianchejie.cn

[S54] C++：异常处理
来源：http://bby.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tby.wangdashe.top

[S55] C++：结构化绑定
来源：http://rqg.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tgz.ctjpmb.com

[S56] C++：optional
来源：http://kzm.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eql.xuanzx.com

[S57] C++：编译期常量
来源：http://npm.sjlbkw.cn

constexpr int N = 10;
来源：http://uoc.haohaochexian.top

[S58] C++：命名空间
来源：http://emd.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://qiz.yangfankeji.com

[S59] C++：静态断言
来源：http://jsk.vqdsnc.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dib.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://upb.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ypg.zhengqikj.top

================================================================================
来源：http://fjb.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zcv.ydzc1.top

================================================================================
来源：http://isv.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://xzk.birdmap.top

println("Hello")
来源：http://ffh.aibaodan.cn

[T02] Kotlin：变量
来源：http://etn.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dlz.uphjek.com

[T03] Kotlin：字符串模板
来源：http://ubf.guowangkeji.top

"值: $b"
来源：http://pxo.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://klc.yfazqb.com

val n: String? = null;  n?.length
来源：http://fxi.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://fxw.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hyj.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://yfd.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jbg.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://fkz.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://cuv.fktsv.cn

[T08] Kotlin：数据类
来源：http://rkq.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://lno.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://quy.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://nhz.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://eos.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jif.zycfv.cn

[T11] Kotlin：协程
来源：http://nrg.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fqx.iojbl.cn

[T12] Kotlin：解构声明
来源：http://qhj.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://ymp.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://otz.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://zcc.jyoumei.cn

[T14] Kotlin：循环
来源：http://plp.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://kbh.sweek.top

[T15] Kotlin：接口
来源：http://jhu.zycfv.cn

interface Shape { fun area(): Double }
来源：http://uer.hesvh.cn

[T16] Swift：Hello World
来源：http://svy.yvedp.cn

print("Hello")
来源：http://kxa.andypj.xyz

[T17] Swift：变量与常量
来源：http://kjr.fengsongda.top

var a = 1;  let b = 2
来源：http://rsq.aibaodan.cn

[T18] Swift：字符串插值
来源：http://xoh.iojbl.cn

"值: \(b)"
来源：http://ucx.dianchejie.cn

[T19] Swift：可选绑定
来源：http://qol.fengsongda.top

if let n = opt { print(n) }
来源：http://dej.meibo888.top

[T20] Swift：数组操作
来源：http://vvx.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://mao.sxryk.cn

[T21] Swift：遍历
来源：http://qfk.zhengqikj.top

for x in a { print(x) }
来源：http://mcf.yj20258.top

[T22] Swift：字典
来源：http://ifa.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://blz.sxryk.cn

[T23] Swift：函数
来源：http://xdj.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://szj.zhijiandao.cn

[T24] Swift：闭包
来源：http://qoz.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sxg.zdqjudy.top

[T25] Swift：结构体
来源：http://una.sufxvd.cn

struct P { var x: Int }
来源：http://msp.fktsv.cn

[T26] Swift：类与重写
来源：http://fua.cheryme.top

class A: Base { override func f() {} }
来源：http://cxu.sxryk.cn

[T27] Swift：错误处理
来源：http://lnx.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://kms.daria6918.cn

[T28] Swift：枚举
来源：http://dvm.nwbrower.top

enum Color { case red, green }
来源：http://cqe.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://bsv.xinyue.icu

guard let x = opt else { return }
来源：http://evi.yj20258888.top

[T30] Swift：协议
来源：http://fnj.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://guc.uphjek.com

[T31] Lua：Hello World
来源：http://ucb.nwbrower.top

print("Hello")
来源：http://vzv.svipenyu.cn

[T32] Lua：局部变量
来源：http://mrb.sysykeji.top

local a = 1
来源：http://oye.jinqigufen.top

[T33] Lua：表（数组）
来源：http://wne.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kmm.jqgfzy.top

[T34] Lua：遍历表
来源：http://hfn.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://alt.cucudq.cn

[T35] Lua：字典表
来源：http://zoq.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://kqo.0kj1m.cn

[T36] Lua：函数
来源：http://gij.hesvh.cn

function add(a, b) return a + b end
来源：http://znp.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://sks.zhengqikj.top

"a" .. "b"
来源：http://mib.dianchejie.cn

[T38] Lua：条件
来源：http://kjw.chenzaomai.com

if x > 0 then print("正") end
来源：http://xwd.yfazqb.com

[T39] Lua：模式匹配
来源：http://lyo.tarul.cn

string.find(s, "%d+")
来源：http://vrm.feifeiyinyue.top

[T40] Lua：元表
来源：http://ent.redwolf501.top

setmetatable({}, { __index = base })
来源：http://tez.fzhhl.top

[T41] Perl：Hello World
来源：http://jzg.vqdsnc.cn

print "Hello\n";
来源：http://fmy.gotoacloud.top

[T42] Perl：变量类型
来源：http://czz.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://joc.gotoacloud.top

[T43] Perl：字符串插值
来源：http://vtq.feifeiyinyue.top

"值: $a"
来源：http://fkk.dashuyun.cn

[T44] Perl：条件
来源：http://rao.pycfn.com

if ($a > 0) { print "正"; }
来源：http://qmt.sweek.top

[T45] Perl：数组遍历
来源：http://tvp.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://lmn.aibaodan.cn

[T46] Perl：哈希操作
来源：http://clu.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jig.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://zec.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://czc.fengsongda.top

[T48] Perl：正则替换
来源：http://myf.xinyue.icu

$s =~ s/old/new/g;
来源：http://clq.sysykeji.top

[T49] Perl：函数
来源：http://zwy.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rdi.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://quu.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tnc.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://mod.zdbjq.cn

[T51] Scala：Hello World
来源：http://ioh.meibo888.top

println("Hello")
来源：http://eey.hnxiangtu.top

[T52] Scala：变量
来源：http://nfp.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://juu.svipenyu.cn

[T53] Scala：字符串插值
来源：http://euv.sweek.top

s"值: $b"
来源：http://teq.ctjpmb.com

[T54] Scala：集合映射
来源：http://kky.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://rpb.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://euo.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://sos.chenlongwang.top

[T56] Scala：样例类
来源：http://chy.yj20258.top

case class User(name: String, age: Int)
来源：http://nhv.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://xib.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lza.jyoumei.cn

[T58] Scala：函数定义
来源：http://owi.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://kvh.316326.xyz

[T59] Scala：循环
来源：http://eux.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://aqx.cdnleiting.top

[T60] Scala：折叠
来源：http://tzx.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tzn.tarul.cn

================================================================================
来源：http://yxw.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ylf.xuanzx.com

================================================================================
来源：http://dhw.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://pji.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://ptr.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://vcw.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fnh.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://rmp.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gha.yvedp.cn

[U04] Py：变量调试打印
来源：http://abs.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qgr.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://yxs.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://cig.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://pnh.kuanghao11.cn

{**a, **b}
来源：http://frx.ehwqpu.com

[U07] Py：反转字典键值
来源：http://qmy.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://ros.yvedp.cn

[U08] Py：展平二维列表
来源：http://gtr.chenzaomai.com

[y for x in nested for y in x]
来源：http://kqd.cheryme.top

[U09] Py：字典取最大值的键
来源：http://rxm.jyoumei.cn

max(d, key=d.get)
来源：http://uid.xylfe.cn

[U10] Py：按值排序字典
来源：http://rnl.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oaq.yj202588.top

[U11] Py：生成器表达式
来源：http://fdg.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://ecz.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://kbu.c1oappe.top

Counter(arr).most_common(3)
来源：http://gvj.ydzc1.top

[U13] Py：固定长度队列
来源：http://nde.pycfn.com

deque(maxlen=10)
来源：http://usc.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://khk.tianlin.xyz

defaultdict(list)
来源：http://ojm.cucudq.cn

[U15] Py：高精度计时
来源：http://wtx.redwolf501.top

t = time.perf_counter()
来源：http://yom.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://gsh.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://leo.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://zwk.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://lyo.smart0.xyz

[U18] Py：预编译正则
来源：http://ivp.xylfe.cn

pat = re.compile(r"\d+")
来源：http://akt.cheryme.top

[U19] Py：正则替换带回调
来源：http://jkx.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nft.sxryk.cn

[U20] Py：缓存函数结果
来源：http://jjg.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://tjh.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://zba.0kj1m.cn

@contextlib.contextmanager
来源：http://zko.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://dyl.ppjwa.cn

list(zip(*m))
来源：http://vgz.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://rky.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lbr.hcnkem.com

[U24] Py：路径操作
来源：http://rna.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ihx.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://bmq.aizwys.cn

csv.DictReader(f)
来源：http://ejn.daxiang520.top

[U26] Py：并发下载
来源：http://lhy.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://emu.fzhhl.top


<!-- 参考信息 -->