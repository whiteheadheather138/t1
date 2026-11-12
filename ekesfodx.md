代发 wailian999

strlen(s)
来源：http://ydo.yanxiufei.cn

[S06] C：字符串比较
来源：http://voi.haohaochexian.top

strcmp(a, b) == 0
来源：http://hnt.fzhhl.top

[S07] C：数组遍历求和
来源：http://uxn.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dui.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://qhw.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ixy.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://msh.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gjn.aizwys.cn

[S10] C：指针与解引用
来源：http://jrb.yfazqb.com

int *p = &a;  *p = 5;
来源：http://mec.daria6918.cn

[S11] C：逐行读文件
来源：http://sms.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://wmn.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gxl.zdqjudy.top

fclose(f);
来源：http://ifl.tarul.cn

[S12] C：写文件
来源：http://lqh.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lyr.xuetiantiany.cn

[S13] C：宏定义
来源：http://gon.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fnt.fktsv.cn

[S14] C：枚举
来源：http://lyh.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://uri.jlsjyb.cn

[S15] C：类型转换
来源：http://cdy.jqgfzy.top

(double) a / b
来源：http://aai.hammf.cn

[S16] C：位操作置位
来源：http://xst.xuetiantiany.cn

x |= (1 << 3);
来源：http://lyb.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://mfi.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vam.cqqwz.cn

[S18] C：命令行参数
来源：http://ogj.yonumen.top

int main(int argc, char **argv)
来源：http://leq.c1oappe.top

[S19] C：快速排序
来源：http://oeh.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rka.yonumen.top

[S20] C：二分查找
来源：http://rfe.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tbn.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://zqz.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aww.zhoulong.xyz

[S22] C：字符串转数字
来源：http://zxd.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://ldd.fengsongda.top

[S23] C：随机数
来源：http://hqr.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pnh.aizwys.cn

[S24] C：获取本地时间
来源：http://awe.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vpg.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://asi.chenzaomai.com

memcpy(dst, src, n);
来源：http://ewr.xziqi.cn

[S26] C：内存清零
来源：http://zjp.nwbrower.top

memset(a, 0, sizeof a);
来源：http://gxj.nwbrower.top

[S27] C：定义常量
来源：http://kfr.xziqi.cn

const double PI = 3.14159;
来源：http://scz.mhx1999.top

[S28] C：静态变量
来源：http://akd.52xcode.cn

static int counter = 0;
来源：http://uvq.ydjk.org.cn

[S29] C：变参函数
来源：http://fvs.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iyj.yuxming.cn

[S30] C：头文件保护
来源：http://yax.yonumen.top

#ifndef X_H
来源：http://icu.daria6918.cn

#define X_H
来源：http://ctu.yj20258.top

#endif
来源：http://vpi.pengpengdd.cyou

[S31] C++：Hello World
来源：http://vsz.bbcook.cn

#include <iostream>
来源：http://acr.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://duv.fzhhl.top

[S32] C++：字符串
来源：http://dom.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://fqh.tarul.cn

[S33] C++：vector 增删
来源：http://waw.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aca.meibo888.top

[S34] C++：遍历 vector
来源：http://tpx.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://cdd.9152youxi.cn

[S35] C++：map
来源：http://vka.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pge.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://lxf.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://luo.316326.xyz

[S37] C++：set
来源：http://fkg.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kkk.ydjk.org.cn

[S38] C++：排序
来源：http://mfi.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://auy.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://wna.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xwc.tarul.cn

[S40] C++：查找元素
来源：http://tik.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmg.tanke756.top

[S41] C++：类与构造函数
来源：http://okg.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tuk.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://bop.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://gqu.xuanzx.com

[S43] C++：智能指针
来源：http://vri.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://hap.c1oappe.top

[S44] C++：引用传参
来源：http://qsj.fengsongda.top

void inc(int &x) { ++x; }
来源：http://umy.ydzc1.top

[S45] C++：lambda
来源：http://ptn.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://bxh.iojbl.cn

[S46] C++：函数模板
来源：http://hdo.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ufe.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://yai.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blo.fktsv.cn

[S48] C++：逐行读文件
来源：http://diq.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fle.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://dkt.cashguo.top

[S49] C++：写文件
来源：http://dkq.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xch.52xcode.cn

[S50] C++：格式化数字
来源：http://cyp.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yjs.yj20258.top

[S51] C++：显式类型转换
来源：http://prm.sjlbkw.cn

static_cast<double>(a) / b
来源：http://zzv.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://tjm.jianghu66.top

int size() const noexcept { return n_; }
来源：http://glw.vehdjk.com

[S53] C++：移动语义
来源：http://ibb.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://iqq.meibo888.top

[S54] C++：异常处理
来源：http://luw.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://msy.dashuyun.cn

[S55] C++：结构化绑定
来源：http://jjr.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eds.jiagoushi.top

[S56] C++：optional
来源：http://wrg.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://djt.tian-w.cn

[S57] C++：编译期常量
来源：http://cia.ppjwa.cn

constexpr int N = 10;
来源：http://knt.svipenyu.cn

[S58] C++：命名空间
来源：http://obc.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://bmi.yj20258888.top

[S59] C++：静态断言
来源：http://obz.nwbrower.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khi.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://fsy.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fht.jinqigfzy.top

================================================================================
来源：http://nko.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tum.zhijiandao.cn

================================================================================
来源：http://rji.wangdashe.top

[T01] Kotlin：Hello World
来源：http://yce.vehdjk.com

println("Hello")
来源：http://fdl.jinqigufen.top

[T02] Kotlin：变量
来源：http://swc.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sia.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://dtu.feifeiyinyue.top

"值: $b"
来源：http://zbz.guowangkeji.top

[T04] Kotlin：空安全
来源：http://mhm.haohaochexian.top

val n: String? = null;  n?.length
来源：http://pgg.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://fbt.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsf.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://nbj.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vmm.316326.xyz

[T07] Kotlin：集合过滤
来源：http://vlo.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gki.52xcode.cn

[T08] Kotlin：数据类
来源：http://wqg.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://hrh.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://dlc.yongpay.top

fun String.exclaim() = this + "!"
来源：http://ykv.epnwcf.com

[T10] Kotlin：默认参数
来源：http://psa.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mss.cheryme.top

[T11] Kotlin：协程
来源：http://aqd.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mgp.redwolf501.top

[T12] Kotlin：解构声明
来源：http://axr.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://rfb.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://vkq.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://mbf.havefunace.top

[T14] Kotlin：循环
来源：http://afq.wangdashe.top

for (i in 1..10) println(i)
来源：http://vov.vehdjk.com

[T15] Kotlin：接口
来源：http://wyh.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://jik.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://pey.shanyushiyangkeji.top

print("Hello")
来源：http://nuy.ehwqpu.com

[T17] Swift：变量与常量
来源：http://vvl.sxryk.cn

var a = 1;  let b = 2
来源：http://enf.haohaochexian.top

[T18] Swift：字符串插值
来源：http://sxu.guannengcc.top

"值: \(b)"
来源：http://gwv.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://owu.vqdsnc.cn

if let n = opt { print(n) }
来源：http://tqd.kuanghao11.cn

[T20] Swift：数组操作
来源：http://uax.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://lqb.sxryk.cn

[T21] Swift：遍历
来源：http://jqq.kuanghao11.cn

for x in a { print(x) }
来源：http://crx.chenzaomai.com

[T22] Swift：字典
来源：http://vhm.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fvr.jianghu66.top

[T23] Swift：函数
来源：http://mwe.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://occ.ybcxt.top

[T24] Swift：闭包
来源：http://ajs.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://arj.ivvv.top

[T25] Swift：结构体
来源：http://ffv.smart0.xyz

struct P { var x: Int }
来源：http://vlm.yfazqb.com

[T26] Swift：类与重写
来源：http://uug.birdmap.top

class A: Base { override func f() {} }
来源：http://mjl.xylfe.cn

[T27] Swift：错误处理
来源：http://noq.ivvv.top

do { try f() } catch { print(error) }
来源：http://plw.chenjidiqi.icu

[T28] Swift：枚举
来源：http://hff.chenjidiqi.icu

enum Color { case red, green }
来源：http://epy.yj20258.top

[T29] Swift：guard 提前返回
来源：http://rfm.0kj1m.cn

guard let x = opt else { return }
来源：http://ilo.hcnkem.com

[T30] Swift：协议
来源：http://aet.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://fsu.hywenlv.cn

[T31] Lua：Hello World
来源：http://oia.hesvh.cn

print("Hello")
来源：http://btg.iojbl.cn

[T32] Lua：局部变量
来源：http://tis.yongpay.top

local a = 1
来源：http://dkp.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://jhz.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fqa.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://nvh.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qco.fzhhl.top

[T35] Lua：字典表
来源：http://lqb.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://ptm.tianlin.xyz

[T36] Lua：函数
来源：http://jzw.dashuyun.cn

function add(a, b) return a + b end
来源：http://iue.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://hcb.yongpay.top

"a" .. "b"
来源：http://bhw.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://jao.xylfe.cn

if x > 0 then print("正") end
来源：http://kht.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://avd.mhx1999.top

string.find(s, "%d+")
来源：http://qcl.yj20258.top

[T40] Lua：元表
来源：http://mpm.bbcook.cn

setmetatable({}, { __index = base })
来源：http://grw.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://jzh.sysykeji.top

print "Hello\n";
来源：http://epl.jiagoushi.top

[T42] Perl：变量类型
来源：http://qsz.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://czd.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://cvd.yfazqb.com

"值: $a"
来源：http://aea.iojbl.cn

[T44] Perl：条件
来源：http://yxx.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://fxa.hammf.cn

[T45] Perl：数组遍历
来源：http://hvq.cashguo.top

for my $x (@arr) { print $x; }
来源：http://ckp.0kj1m.cn

[T46] Perl：哈希操作
来源：http://ctx.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sji.yj202588.top

[T47] Perl：正则捕获
来源：http://pwl.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jmu.sjlbkw.cn

[T48] Perl：正则替换
来源：http://ziy.yfazqb.com

$s =~ s/old/new/g;
来源：http://dyz.nanxinkj.top

[T49] Perl：函数
来源：http://nyn.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cik.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://ctd.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xzc.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://psh.gzhubu.top

[T51] Scala：Hello World
来源：http://fiq.jyoumei.cn

println("Hello")
来源：http://qkv.yj202588.top

[T52] Scala：变量
来源：http://cbx.gzhubu.top

val a = 1;  var b = 2
来源：http://hvb.mhx1999.top

[T53] Scala：字符串插值
来源：http://mna.zhixingplan.top

s"值: $b"
来源：http://rag.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://zdx.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://rna.9152youxi.cn

[T55] Scala：集合过滤
来源：http://djb.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://zts.gotoacloud.top

[T56] Scala：样例类
来源：http://vgu.ybcxt.top

case class User(name: String, age: Int)
来源：http://hwe.jqgfzy.top

[T57] Scala：模式匹配
来源：http://dvo.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bqq.gzhubu.top

[T58] Scala：函数定义
来源：http://pyn.nanxuanxn.top

def add(a: Int, b: Int): Int = a + b
来源：http://auk.sjlbkw.cn

[T59] Scala：循环
来源：http://osd.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://cnv.sjlbkw.cn

[T60] Scala：折叠
来源：http://ouw.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gob.hnxiangtu.top

================================================================================
来源：http://vnv.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bkv.yj20258.top

================================================================================
来源：http://vap.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://juw.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cfr.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://nhx.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://alr.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://pph.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://umu.ybcxt.top

[U04] Py：变量调试打印
来源：http://bbd.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bor.hnqzz.top

[U05] Py：列表去重且保序
来源：http://xzv.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://zkh.fktsv.cn

[U06] Py：合并两个字典
来源：http://kam.c1oappe.top

{**a, **b}
来源：http://tfl.cheryme.top

[U07] Py：反转字典键值
来源：http://kxq.snrcjt.cn

{v: k for k, v in d.items()}
来源：http://flx.nwbrower.top

[U08] Py：展平二维列表
来源：http://vek.yuanzhike.top

[y for x in nested for y in x]
来源：http://mwq.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://rgv.ctjpmb.com

max(d, key=d.get)
来源：http://yps.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://xee.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://swq.xinyue.icu

[U11] Py：生成器表达式
来源：http://wxj.iojbl.cn

(x * 2 for x in arr)
来源：http://uwa.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://jnl.bbcook.cn

Counter(arr).most_common(3)
来源：http://wgd.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://yyv.zhongyouzk.top

deque(maxlen=10)
来源：http://stj.tanke756.top

[U14] Py：分组收集到列表
来源：http://owy.ydzc1.top

defaultdict(list)
来源：http://krz.birdmap.top

[U15] Py：高精度计时
来源：http://srh.zdqjudy.top

t = time.perf_counter()
来源：http://rqm.hesvh.cn

[U16] Py：命令行参数解析
来源：http://kcx.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://erb.shzxlz.cn

[U17] Py：初始化日志
来源：http://qye.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://pqd.xuanzx.com

[U18] Py：预编译正则
来源：http://qtt.fktsv.cn

pat = re.compile(r"\d+")
来源：http://ioz.aizwys.cn

[U19] Py：正则替换带回调
来源：http://wxz.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rgk.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://obv.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://acf.jqgfzy.top

[U21] Py：自定义上下文管理器
来源：http://wda.tarul.cn

@contextlib.contextmanager
来源：http://siy.9152youxi.cn

[U22] Py：矩阵转置
来源：http://fkh.wangdashe.top

list(zip(*m))
来源：http://yji.hesvh.cn

[U23] Py：分块读取大文件
来源：http://ilc.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mpf.ydjk.org.cn

[U24] Py：路径操作
来源：http://dnx.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wnj.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://gae.aibaodan.cn

csv.DictReader(f)
来源：http://ypd.c1oappe.top

[U26] Py：并发下载
来源：http://til.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ibl.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://tfu.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://oqd.pengpengdd.cyou

[U28] Py：类型别名
来源：http://qsq.yangfankeji.com

UserId = int
来源：http://phr.bjfxy.top


<!-- 参考信息 -->