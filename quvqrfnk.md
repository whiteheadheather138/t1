代发 wailian999

int x; scanf("%d", &x);
来源：http://ucv.guannengcc.top

[S04] C：字符串复制
来源：http://scb.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://aro.xinyue.icu

[S05] C：字符串长度
来源：http://zkz.yanxiufei.cn

strlen(s)
来源：http://xmj.gaohongyu789.top

[S06] C：字符串比较
来源：http://dkj.ydjk.org.cn

strcmp(a, b) == 0
来源：http://usi.cqqwz.cn

[S07] C：数组遍历求和
来源：http://hqg.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tav.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://hht.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ida.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://spe.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qap.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://pcf.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://gyk.fengsongda.top

[S11] C：逐行读文件
来源：http://edm.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://yjy.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmz.ybcxt.top

fclose(f);
来源：http://nsp.aibaodan.cn

[S12] C：写文件
来源：http://bwq.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://waf.hcnkem.com

[S13] C：宏定义
来源：http://yyz.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://skh.sxryk.cn

[S14] C：枚举
来源：http://vow.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://mcp.fanxiaobao.xyz

[S15] C：类型转换
来源：http://lor.jianghu66.top

(double) a / b
来源：http://lls.chenlongwang.top

[S16] C：位操作置位
来源：http://ouz.guannengcc.top

x |= (1 << 3);
来源：http://evw.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://psm.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ytd.zhijiandao.cn

[S18] C：命令行参数
来源：http://vzm.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://uvj.tianlin.xyz

[S19] C：快速排序
来源：http://tvn.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://zrq.hongshengwenyu.top

[S20] C：二分查找
来源：http://cyt.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qyq.zhoulong.xyz

[S21] C：字符类别判断
来源：http://wdj.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zfw.yj20258888.top

[S22] C：字符串转数字
来源：http://qti.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://haz.gzhubu.top

[S23] C：随机数
来源：http://kql.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lfx.ehwqpu.com

[S24] C：获取本地时间
来源：http://gxe.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jms.daria6918.cn

[S25] C：内存拷贝
来源：http://xyi.gzhubu.top

memcpy(dst, src, n);
来源：http://lcq.cucudq.cn

[S26] C：内存清零
来源：http://opw.cashguo.top

memset(a, 0, sizeof a);
来源：http://vxb.cucudq.cn

[S27] C：定义常量
来源：http://wua.aibaodan.cn

const double PI = 3.14159;
来源：http://ueu.aibaodan.cn

[S28] C：静态变量
来源：http://kfr.ppjwa.cn

static int counter = 0;
来源：http://txw.fehbvm.com

[S29] C：变参函数
来源：http://bow.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ltq.zdqjudy.top

[S30] C：头文件保护
来源：http://dud.guowangkeji.top

#ifndef X_H
来源：http://jbb.zhengqikj.top

#define X_H
来源：http://bwj.fzhhl.top

#endif
来源：http://gxs.jiagoushi.top

[S31] C++：Hello World
来源：http://znj.fengsongda.top

#include <iostream>
来源：http://uze.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://hmg.ydjk.org.cn

[S32] C++：字符串
来源：http://skh.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://rmm.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://mbg.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ezv.c1oappe.top

[S34] C++：遍历 vector
来源：http://byv.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://vig.zhijiandao.cn

[S35] C++：map
来源：http://jvo.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ktr.yuxming.cn

[S36] C++：unordered_map
来源：http://tct.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aqa.zhijiandao.cn

[S37] C++：set
来源：http://khl.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ldp.redwolf501.top

[S38] C++：排序
来源：http://kpp.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://jfz.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://yol.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mbw.fktsv.cn

[S40] C++：查找元素
来源：http://qcl.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wys.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://ssv.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xkf.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://lug.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://crt.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://yqr.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://nsk.jqgufenzy.top

[S44] C++：引用传参
来源：http://nfg.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://gco.epnwcf.com

[S45] C++：lambda
来源：http://imj.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://qqz.chenjidiqi.icu

[S46] C++：函数模板
来源：http://bvf.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uma.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://qgg.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsi.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://hqd.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://deh.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://rap.xinyue.icu

[S49] C++：写文件
来源：http://hhw.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvm.cashguo.top

[S50] C++：格式化数字
来源：http://mtz.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://res.sufxvd.cn

[S51] C++：显式类型转换
来源：http://qij.yj20258888.top

static_cast<double>(a) / b
来源：http://oeg.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://kdi.bjfxy.top

int size() const noexcept { return n_; }
来源：http://rgx.hnqzz.top

[S53] C++：移动语义
来源：http://qct.sweek.top

std::vector<int> w = std::move(v);
来源：http://wvb.tian-w.cn

[S54] C++：异常处理
来源：http://qjm.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zyx.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://ock.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ryo.pengpengdd.cyou

[S56] C++：optional
来源：http://qao.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://paf.birdmap.top

[S57] C++：编译期常量
来源：http://frk.c1oappe.top

constexpr int N = 10;
来源：http://jer.wangshuangyany.cn

[S58] C++：命名空间
来源：http://ypb.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://cju.fzhhl.top

[S59] C++：静态断言
来源：http://khe.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kme.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://tqb.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rmd.xingfuxueyuan.xyz

================================================================================
来源：http://pvi.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzk.ctjpmb.com

================================================================================
来源：http://umf.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://jja.cheryme.top

println("Hello")
来源：http://bri.nwbrower.top

[T02] Kotlin：变量
来源：http://ceq.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dof.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://kvv.vqdsnc.cn

"值: $b"
来源：http://fow.havefunace.top

[T04] Kotlin：空安全
来源：http://dti.fehbvm.com

val n: String? = null;  n?.length
来源：http://hbm.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://stv.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kad.zycfv.cn

[T06] Kotlin：集合映射
来源：http://inp.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mzv.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://wpu.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qqx.zdbjq.cn

[T08] Kotlin：数据类
来源：http://pii.ivvv.top

data class User(val name: String, val age: Int)
来源：http://taj.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://gkr.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://bsr.xziqi.cn

[T10] Kotlin：默认参数
来源：http://gvt.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://njf.ehwqpu.com

[T11] Kotlin：协程
来源：http://ows.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bxg.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://lmm.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://khq.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://pke.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://ugv.epnwcf.com

[T14] Kotlin：循环
来源：http://cip.cdnleiting.top

for (i in 1..10) println(i)
来源：http://uwq.guannengcc.top

[T15] Kotlin：接口
来源：http://uvg.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://xeg.ybcxt.top

[T16] Swift：Hello World
来源：http://huc.chenzaomai.com

print("Hello")
来源：http://dyx.nwbrower.top

[T17] Swift：变量与常量
来源：http://rac.tanke756.top

var a = 1;  let b = 2
来源：http://ucv.yfazqb.com

[T18] Swift：字符串插值
来源：http://fxf.havefunace.top

"值: \(b)"
来源：http://evb.aizwys.cn

[T19] Swift：可选绑定
来源：http://yhc.yuxming.cn

if let n = opt { print(n) }
来源：http://gdv.c1oappe.top

[T20] Swift：数组操作
来源：http://azz.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aqr.hnqzz.top

[T21] Swift：遍历
来源：http://qmg.gotoacloud.top

for x in a { print(x) }
来源：http://biq.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://vhy.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ywm.feifeiyinyue.top

[T23] Swift：函数
来源：http://yvk.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iqk.jyoumei.cn

[T24] Swift：闭包
来源：http://tvk.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://xcr.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://mur.wangdashe.top

struct P { var x: Int }
来源：http://oea.zhixingplan.top

[T26] Swift：类与重写
来源：http://fhw.tianlin.xyz

class A: Base { override func f() {} }
来源：http://vtl.yanxiufei.cn

[T27] Swift：错误处理
来源：http://bub.vehdjk.com

do { try f() } catch { print(error) }
来源：http://hbr.daria6918.cn

[T28] Swift：枚举
来源：http://fqp.redwolf501.top

enum Color { case red, green }
来源：http://oyl.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://sjk.sxryk.cn

guard let x = opt else { return }
来源：http://akk.guowangkeji.top

[T30] Swift：协议
来源：http://qpc.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://wwq.tanke756.top

[T31] Lua：Hello World
来源：http://tfv.chenzaomai.com

print("Hello")
来源：http://ewk.gogol.net.cn

[T32] Lua：局部变量
来源：http://gbc.shuidangran.top

local a = 1
来源：http://rxj.jqgfzy.top

[T33] Lua：表（数组）
来源：http://dqe.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://frj.daxiang520.top

[T34] Lua：遍历表
来源：http://brb.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ywb.yangfankeji.com

[T35] Lua：字典表
来源：http://eet.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://cif.ctjpmb.com

[T36] Lua：函数
来源：http://nau.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://oub.nwbrower.top

[T37] Lua：字符串拼接
来源：http://cqp.wangshuangyany.cn

"a" .. "b"
来源：http://mra.9152youxi.cn

[T38] Lua：条件
来源：http://spf.gzhubu.top

if x > 0 then print("正") end
来源：http://xkv.meibo888.top

[T39] Lua：模式匹配
来源：http://nap.shangyingyoupin.top

string.find(s, "%d+")
来源：http://tqj.nanxuanxn.top

[T40] Lua：元表
来源：http://pni.c1oappe.top

setmetatable({}, { __index = base })
来源：http://mjr.xuanzx.com

[T41] Perl：Hello World
来源：http://mit.zhengqikj.top

print "Hello\n";
来源：http://aax.guowangkeji.top

[T42] Perl：变量类型
来源：http://fgj.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uly.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://rvq.xuetiantiany.cn

"值: $a"
来源：http://qav.fktsv.cn

[T44] Perl：条件
来源：http://sdy.yj202588.top

if ($a > 0) { print "正"; }
来源：http://opo.iojbl.cn

[T45] Perl：数组遍历
来源：http://nge.ivvv.top

for my $x (@arr) { print $x; }
来源：http://hju.snrcjt.cn

[T46] Perl：哈希操作
来源：http://jtw.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ixs.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://qcf.sweek.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xfl.yangfankeji.com

[T48] Perl：正则替换
来源：http://pal.zhixingplan.top

$s =~ s/old/new/g;
来源：http://gpp.ehwqpu.com

[T49] Perl：函数
来源：http://bfa.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vmb.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://uyc.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qtz.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://zwc.zdqjudy.top

[T51] Scala：Hello World
来源：http://rvn.smart0.xyz

println("Hello")
来源：http://bnr.chenzaomai.com

[T52] Scala：变量
来源：http://tww.ctjpmb.com

val a = 1;  var b = 2
来源：http://fuq.iojbl.cn

[T53] Scala：字符串插值
来源：http://llc.hysaishi.cn

s"值: $b"
来源：http://bmd.hammf.cn

[T54] Scala：集合映射
来源：http://fua.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://eeu.316326.xyz

[T55] Scala：集合过滤
来源：http://wwb.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://tdv.fehbvm.com

[T56] Scala：样例类
来源：http://otv.bbcook.cn

case class User(name: String, age: Int)
来源：http://waz.zdbjq.cn

[T57] Scala：模式匹配
来源：http://ywc.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eqs.yj20258.top

[T58] Scala：函数定义
来源：http://ooy.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lnq.tian-w.cn

[T59] Scala：循环
来源：http://luo.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://tkj.jinqigufen.top

[T60] Scala：折叠
来源：http://nbw.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tqx.yuxming.cn

================================================================================
来源：http://krb.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zrm.yangfankeji.com

================================================================================
来源：http://ukm.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://mtk.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://doc.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://sfg.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kzd.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://hle.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rtd.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://itx.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fjn.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://jao.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://rmp.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://fjy.jlsjyb.cn

{**a, **b}
来源：http://eye.ybcxt.top

[U07] Py：反转字典键值
来源：http://fat.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://klx.cashguo.top

[U08] Py：展平二维列表
来源：http://mpo.hnqzz.top

[y for x in nested for y in x]
来源：http://qke.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://fdl.gzhubu.top

max(d, key=d.get)
来源：http://xxn.yj20258.top

[U10] Py：按值排序字典
来源：http://plk.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fjm.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://jfl.aibaodan.cn

(x * 2 for x in arr)
来源：http://ekb.pycfn.com

[U12] Py：取出现最多的 3 个元素
来源：http://nys.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://bbw.hesvh.cn

[U13] Py：固定长度队列
来源：http://hsj.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://tuf.meibo888.top

[U14] Py：分组收集到列表
来源：http://btv.smart0.xyz

defaultdict(list)
来源：http://edb.tian-w.cn

[U15] Py：高精度计时
来源：http://cli.feifeiyinyue.top

t = time.perf_counter()
来源：http://rad.cheryme.top

[U16] Py：命令行参数解析
来源：http://ivf.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nvi.sxryk.cn

[U17] Py：初始化日志
来源：http://gtj.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://sdk.iojbl.cn

[U18] Py：预编译正则
来源：http://fuc.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://hde.52xcode.cn

[U19] Py：正则替换带回调
来源：http://ojx.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zcm.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://cre.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://rty.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://ine.aibaodan.cn

@contextlib.contextmanager
来源：http://xom.fehbvm.com

[U22] Py：矩阵转置
来源：http://ttq.redwolf501.top

list(zip(*m))
来源：http://dpl.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://cyp.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tim.fzhhl.top

[U24] Py：路径操作
来源：http://ohs.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://stw.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://xyt.jinghuilouyu.cn

csv.DictReader(f)
来源：http://ojl.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://idw.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eir.tianlin.xyz


<!-- 参考信息 -->