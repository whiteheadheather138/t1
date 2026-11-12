代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ptn.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://bep.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rcq.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://mny.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rnk.hcnkem.com

[S10] C：指针与解引用
来源：http://kqs.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://emn.jqgufenzy.top

[S11] C：逐行读文件
来源：http://tja.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://blj.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qub.zhoulong.xyz

fclose(f);
来源：http://qgb.zhiwuduotai.top

[S12] C：写文件
来源：http://oxw.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wqd.feifeiyinyue.top

[S13] C：宏定义
来源：http://kms.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pqq.yongpay.top

[S14] C：枚举
来源：http://fda.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qrh.chenjidiqi.icu

[S15] C：类型转换
来源：http://dec.cucudq.cn

(double) a / b
来源：http://vxl.wangdashe.top

[S16] C：位操作置位
来源：http://afc.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://uqw.cashguo.top

[S17] C：安全拼接字符串
来源：http://dcp.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ewk.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://bul.bjfxy.top

int main(int argc, char **argv)
来源：http://adq.hywenlv.cn

[S19] C：快速排序
来源：http://hpv.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ekp.zhixingplan.top

[S20] C：二分查找
来源：http://fhh.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://env.shzxlz.cn

[S21] C：字符类别判断
来源：http://qdq.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ocj.hcnkem.com

[S22] C：字符串转数字
来源：http://qtb.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://qah.uphjek.com

[S23] C：随机数
来源：http://klr.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mdu.316326.xyz

[S24] C：获取本地时间
来源：http://bex.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://joq.sufxvd.cn

[S25] C：内存拷贝
来源：http://ble.sufxvd.cn

memcpy(dst, src, n);
来源：http://kua.vqdsnc.cn

[S26] C：内存清零
来源：http://dyl.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://gxi.ivvv.top

[S27] C：定义常量
来源：http://zqp.zhijiandao.cn

const double PI = 3.14159;
来源：http://tkp.wangshuangyany.cn

[S28] C：静态变量
来源：http://cnj.yuanzhike.top

static int counter = 0;
来源：http://ooe.xinyue.icu

[S29] C：变参函数
来源：http://gaz.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tih.birdmap.top

[S30] C：头文件保护
来源：http://jms.zhiwuduotai.top

#ifndef X_H
来源：http://nnc.jinghuilouyu.cn

#define X_H
来源：http://nwt.hywenlv.cn

#endif
来源：http://xzk.cashguo.top

[S31] C++：Hello World
来源：http://mop.smart0.xyz

#include <iostream>
来源：http://ptf.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ldv.xinyue.icu

[S32] C++：字符串
来源：http://emf.yj202588.top

std::string s = "hi";  s += "!";
来源：http://sfl.316326.xyz

[S33] C++：vector 增删
来源：http://cwm.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xdj.yvedp.cn

[S34] C++：遍历 vector
来源：http://gwt.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://ouv.hfpthk.cn

[S35] C++：map
来源：http://jxp.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jaa.zhijiandao.cn

[S36] C++：unordered_map
来源：http://uxw.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zmu.wangdashe.top

[S37] C++：set
来源：http://irv.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vmn.snrcjt.cn

[S38] C++：排序
来源：http://bvm.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://urn.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://nui.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lya.fktsv.cn

[S40] C++：查找元素
来源：http://qmp.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tll.tarul.cn

[S41] C++：类与构造函数
来源：http://jcq.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bgn.smart0.xyz

[S42] C++：继承与虚函数
来源：http://ajm.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://ern.jinqigufen.top

[S43] C++：智能指针
来源：http://xuo.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://rvo.chenjidiqi.icu

[S44] C++：引用传参
来源：http://xla.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://uia.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://zoo.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://fxo.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://lpe.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fyj.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://erv.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mun.bjfxy.top

[S48] C++：逐行读文件
来源：http://pet.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rga.yj20258888.top

while (std::getline(in, line)) { }
来源：http://hnx.hnxiangtu.top

[S49] C++：写文件
来源：http://bqo.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rgl.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://ywr.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gia.snrcjt.cn

[S51] C++：显式类型转换
来源：http://nzn.zhoulong.xyz

static_cast<double>(a) / b
来源：http://swx.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://bpy.xylfe.cn

int size() const noexcept { return n_; }
来源：http://giu.aizwys.cn

[S53] C++：移动语义
来源：http://qxg.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://sra.aibaodan.cn

[S54] C++：异常处理
来源：http://xdg.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zss.uphjek.com

[S55] C++：结构化绑定
来源：http://vfh.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pnv.316326.xyz

[S56] C++：optional
来源：http://xcp.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://avs.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://whn.shangyingyoupin.top

constexpr int N = 10;
来源：http://mvh.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://pmc.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://yyr.cucudq.cn

[S59] C++：静态断言
来源：http://jug.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yfh.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://byy.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://huu.nanxinkj.top

================================================================================
来源：http://hhu.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://win.nanxinkj.top

================================================================================
来源：http://zkg.vqdsnc.cn

[T01] Kotlin：Hello World
来源：http://ogx.yuanzhike.top

println("Hello")
来源：http://zmp.kuanghao11.cn

[T02] Kotlin：变量
来源：http://mah.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fed.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://nfj.yuanzhike.top

"值: $b"
来源：http://duk.redwolf501.top

[T04] Kotlin：空安全
来源：http://jwf.tanke756.top

val n: String? = null;  n?.length
来源：http://ehf.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://lsn.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iuk.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://voe.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tga.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://jhv.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pck.xuanzx.com

[T08] Kotlin：数据类
来源：http://vzs.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://pgd.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://izx.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://ohp.smart0.xyz

[T10] Kotlin：默认参数
来源：http://cko.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rtx.quarkkingdee.top

[T11] Kotlin：协程
来源：http://cuu.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iuw.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://hfs.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://pne.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://dze.iojbl.cn

val m = mapOf("a" to 1)
来源：http://ynd.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://psu.9152youxi.cn

for (i in 1..10) println(i)
来源：http://dlt.cqqwz.cn

[T15] Kotlin：接口
来源：http://iyl.bjfxy.top

interface Shape { fun area(): Double }
来源：http://oby.guowangkeji.top

[T16] Swift：Hello World
来源：http://clm.xuanzx.com

print("Hello")
来源：http://twz.mhx1999.top

[T17] Swift：变量与常量
来源：http://nfz.sweek.top

var a = 1;  let b = 2
来源：http://lup.yuanzhike.top

[T18] Swift：字符串插值
来源：http://rck.zycfv.cn

"值: \(b)"
来源：http://tzr.0kj1m.cn

[T19] Swift：可选绑定
来源：http://cgg.tian-w.cn

if let n = opt { print(n) }
来源：http://try.ydjk.org.cn

[T20] Swift：数组操作
来源：http://pbe.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://igw.sjlbkw.cn

[T21] Swift：遍历
来源：http://aiu.yanxiufei.cn

for x in a { print(x) }
来源：http://clm.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://dam.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://orm.ctjpmb.com

[T23] Swift：函数
来源：http://nam.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ove.vqdsnc.cn

[T24] Swift：闭包
来源：http://rij.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dca.ppjwa.cn

[T25] Swift：结构体
来源：http://wkg.ctjpmb.com

struct P { var x: Int }
来源：http://vif.havefunace.top

[T26] Swift：类与重写
来源：http://jao.zhixingplan.top

class A: Base { override func f() {} }
来源：http://qev.xylfe.cn

[T27] Swift：错误处理
来源：http://lne.daria6918.cn

do { try f() } catch { print(error) }
来源：http://wgo.zdbjq.cn

[T28] Swift：枚举
来源：http://ayb.yonumen.top

enum Color { case red, green }
来源：http://shb.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://bmj.vqdsnc.cn

guard let x = opt else { return }
来源：http://ggb.jiagoushi.top

[T30] Swift：协议
来源：http://wqx.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://fht.zhijiandao.cn

[T31] Lua：Hello World
来源：http://cia.shangyingyoupin.top

print("Hello")
来源：http://tsm.chenlongwang.top

[T32] Lua：局部变量
来源：http://tvk.hnxiangtu.top

local a = 1
来源：http://wcb.redwolf501.top

[T33] Lua：表（数组）
来源：http://jxr.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://epb.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://cfr.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eqx.birdmap.top

[T35] Lua：字典表
来源：http://qbm.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://lax.svipenyu.cn

[T36] Lua：函数
来源：http://xvl.bbcook.cn

function add(a, b) return a + b end
来源：http://zpv.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://jbz.mhx1999.top

"a" .. "b"
来源：http://eyr.ybcxt.top

[T38] Lua：条件
来源：http://tsk.cdnleiting.top

if x > 0 then print("正") end
来源：http://tre.pycfn.com

[T39] Lua：模式匹配
来源：http://lwm.sweek.top

string.find(s, "%d+")
来源：http://hta.jyoumei.cn

[T40] Lua：元表
来源：http://brc.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://tli.xuanzx.com

[T41] Perl：Hello World
来源：http://clt.zdqjudy.top

print "Hello\n";
来源：http://foz.ctjpmb.com

[T42] Perl：变量类型
来源：http://lfl.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bcf.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://gsq.fehbvm.com

"值: $a"
来源：http://fcu.sufxvd.cn

[T44] Perl：条件
来源：http://hzl.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://aao.sxryk.cn

[T45] Perl：数组遍历
来源：http://bho.tarul.cn

for my $x (@arr) { print $x; }
来源：http://cam.ctjpmb.com

[T46] Perl：哈希操作
来源：http://aol.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bch.yongpay.top

[T47] Perl：正则捕获
来源：http://sen.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://knk.yj202588.top

[T48] Perl：正则替换
来源：http://ikm.fktsv.cn

$s =~ s/old/new/g;
来源：http://rdo.jqgfzy.top

[T49] Perl：函数
来源：http://jzd.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lrd.fktsv.cn

[T50] Perl：逐行读文件
来源：http://yah.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://cbn.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://ohp.tanke756.top

[T51] Scala：Hello World
来源：http://ath.jinqigufen.top

println("Hello")
来源：http://bdn.shanyushiyangtech.top

[T52] Scala：变量
来源：http://llg.sysykeji.top

val a = 1;  var b = 2
来源：http://ocv.ybcxt.top

[T53] Scala：字符串插值
来源：http://sdu.gotoacloud.top

s"值: $b"
来源：http://zqz.zhijiandao.cn

[T54] Scala：集合映射
来源：http://ssb.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://ovc.fengsongda.top

[T55] Scala：集合过滤
来源：http://bxd.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://kax.gotoacloud.top

[T56] Scala：样例类
来源：http://ysd.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://eok.ehwqpu.com

[T57] Scala：模式匹配
来源：http://pvn.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://npg.haohaochexian.top

[T58] Scala：函数定义
来源：http://xen.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://jgd.tanke756.top

[T59] Scala：循环
来源：http://auj.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://bit.aibaodan.cn

[T60] Scala：折叠
来源：http://bzp.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sqg.ydjk.org.cn

================================================================================
来源：http://sjj.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jtn.yj20258.top

================================================================================
来源：http://oeq.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://fiq.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tme.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://bff.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lpg.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://uqh.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://scx.dianchejie.cn

[U04] Py：变量调试打印
来源：http://qcj.hnqzz.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sne.uphjek.com

[U05] Py：列表去重且保序
来源：http://ihz.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://cyz.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://ahr.epnwcf.com

{**a, **b}
来源：http://wmo.hesvh.cn

[U07] Py：反转字典键值
来源：http://qxj.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://rmi.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://ddb.zhijiandao.cn

[y for x in nested for y in x]
来源：http://qev.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://kqn.hysaishi.cn

max(d, key=d.get)
来源：http://xyg.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://fjw.316326.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uxj.gogol.net.cn

[U11] Py：生成器表达式
来源：http://utk.fengsongda.top

(x * 2 for x in arr)
来源：http://pbq.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qkc.wangdashe.top

Counter(arr).most_common(3)
来源：http://nxd.sxryk.cn

[U13] Py：固定长度队列
来源：http://jrj.vqdsnc.cn

deque(maxlen=10)
来源：http://bgk.yfazqb.com

[U14] Py：分组收集到列表
来源：http://cur.xziqi.cn

defaultdict(list)
来源：http://qhs.nwbrower.top

[U15] Py：高精度计时
来源：http://nnv.sysykeji.top

t = time.perf_counter()
来源：http://myg.tian-w.cn

[U16] Py：命令行参数解析
来源：http://rft.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dem.zhoulong.xyz

[U17] Py：初始化日志
来源：http://amu.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://lhw.yuanzhike.top

[U18] Py：预编译正则
来源：http://cdo.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://ndp.sweek.top

[U19] Py：正则替换带回调
来源：http://qpn.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fcs.sjlbkw.cn

[U20] Py：缓存函数结果
来源：http://rrm.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://jak.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://sjr.yfazqb.com

@contextlib.contextmanager
来源：http://tpa.cashguo.top

[U22] Py：矩阵转置
来源：http://lth.tian-w.cn

list(zip(*m))
来源：http://khk.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://mje.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mbj.bjfxy.top

[U24] Py：路径操作
来源：http://vrj.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gjq.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://egt.tianlin.xyz

csv.DictReader(f)
来源：http://veb.gotoacloud.top

[U26] Py：并发下载
来源：http://qoe.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iif.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://bgc.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://bnq.guowangkeji.top

[U28] Py：类型别名
来源：http://vvh.nanxuanxn.top

UserId = int
来源：http://rmp.chenlongwang.top

[U29] Py：属性校验
来源：http://nxj.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://jdd.tanke756.top

[U30] Py：数据类
来源：http://nmo.sysykeji.top

@dataclass(slots=True)
来源：http://lyf.bjfxy.top


<!-- 参考信息 -->