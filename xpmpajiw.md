代发 wailian999

strlen(s)
来源：http://hwo.xuanzx.com

[S06] C：字符串比较
来源：http://ntr.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://hne.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://clu.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gzg.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://gee.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zba.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://vbz.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dzy.tianlin.xyz

[S10] C：指针与解引用
来源：http://jyh.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://qcp.daxiang520.top

[S11] C：逐行读文件
来源：http://pno.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://ler.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wpw.aizwys.cn

fclose(f);
来源：http://mkb.xziqi.cn

[S12] C：写文件
来源：http://dyn.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zor.fzhhl.top

[S13] C：宏定义
来源：http://xom.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://klg.feifeiyinyue.top

[S14] C：枚举
来源：http://xcf.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://nej.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://mqk.iojbl.cn

(double) a / b
来源：http://ejf.xylfe.cn

[S16] C：位操作置位
来源：http://bsn.zdbjq.cn

x |= (1 << 3);
来源：http://axf.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://jrb.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://igw.meibo888.top

[S18] C：命令行参数
来源：http://xmj.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://zjt.hammf.cn

[S19] C：快速排序
来源：http://myo.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://otk.ivvv.top

[S20] C：二分查找
来源：http://psi.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vrg.cdnleiting.top

[S21] C：字符类别判断
来源：http://qyn.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rid.wangdashe.top

[S22] C：字符串转数字
来源：http://sfw.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://wva.yuxming.cn

[S23] C：随机数
来源：http://rxs.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dkk.yj20258.top

[S24] C：获取本地时间
来源：http://rov.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jta.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://trp.chenzaomai.com

memcpy(dst, src, n);
来源：http://qfv.gogol.net.cn

[S26] C：内存清零
来源：http://xxk.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://aoq.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://giy.yj20258.top

const double PI = 3.14159;
来源：http://mjj.gotoacloud.top

[S28] C：静态变量
来源：http://kyc.nanxuanxn.top

static int counter = 0;
来源：http://cly.c1oappe.top

[S29] C：变参函数
来源：http://suq.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bet.chenlongwang.top

[S30] C：头文件保护
来源：http://bbb.quarkkingdee.top

#ifndef X_H
来源：http://auy.kuanghao11.cn

#define X_H
来源：http://ije.epnwcf.com

#endif
来源：http://whi.tian-w.cn

[S31] C++：Hello World
来源：http://tdf.xuetiantiany.cn

#include <iostream>
来源：http://ady.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://ucf.zhongyouzk.top

[S32] C++：字符串
来源：http://dfg.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://ycz.sufxvd.cn

[S33] C++：vector 增删
来源：http://sxc.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tpk.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://gyu.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://reo.jinqigufen.top

[S35] C++：map
来源：http://ypt.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zon.52xcode.cn

[S36] C++：unordered_map
来源：http://xpq.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bhz.zhaomingkeji.xyz

[S37] C++：set
来源：http://iaw.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://obv.hywenlv.cn

[S38] C++：排序
来源：http://qxq.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://sek.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://bje.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hfc.zhongyouzk.top

[S40] C++：查找元素
来源：http://qkw.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hsh.yj20258888.top

[S41] C++：类与构造函数
来源：http://rrm.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qcq.ybcxt.top

[S42] C++：继承与虚函数
来源：http://jsx.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://piu.52xcode.cn

[S43] C++：智能指针
来源：http://cop.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://eck.daria6918.cn

[S44] C++：引用传参
来源：http://omj.yj202588.top

void inc(int &x) { ++x; }
来源：http://hpd.pengpengdd.cyou

[S45] C++：lambda
来源：http://tsn.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://cpn.zhixingplan.top

[S46] C++：函数模板
来源：http://hgu.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pge.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://sfh.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bna.zycfv.cn

[S48] C++：逐行读文件
来源：http://yag.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://gwn.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://gtd.gzhubu.top

[S49] C++：写文件
来源：http://naf.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mbo.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://rdy.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ebq.hesvh.cn

[S51] C++：显式类型转换
来源：http://sih.gotoacloud.top

static_cast<double>(a) / b
来源：http://gxg.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://tfi.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://zmm.cdnleiting.top

[S53] C++：移动语义
来源：http://xkp.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://txr.fktsv.cn

[S54] C++：异常处理
来源：http://odc.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://phz.gzhubu.top

[S55] C++：结构化绑定
来源：http://nqw.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dyd.iojbl.cn

[S56] C++：optional
来源：http://mkr.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fkv.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://vgp.epnwcf.com

constexpr int N = 10;
来源：http://bwy.pengpengdd.cyou

[S58] C++：命名空间
来源：http://hlb.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://vmj.ydjk.org.cn

[S59] C++：静态断言
来源：http://pem.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://civ.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://och.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zvc.52xcode.cn

================================================================================
来源：http://omu.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypw.andypj.xyz

================================================================================
来源：http://xbc.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://hyd.nanxuanxn.top

println("Hello")
来源：http://sqb.yj20258888.top

[T02] Kotlin：变量
来源：http://tkp.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rwt.yj20258.top

[T03] Kotlin：字符串模板
来源：http://qsk.vqdsnc.cn

"值: $b"
来源：http://ffk.0kj1m.cn

[T04] Kotlin：空安全
来源：http://shm.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://lxe.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://czo.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qnm.andypj.xyz

[T06] Kotlin：集合映射
来源：http://hhv.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qao.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://guv.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://spy.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://qcv.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://zbk.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://nfi.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://quw.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://mim.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iuv.hywenlv.cn

[T11] Kotlin：协程
来源：http://wgi.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cyg.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://esh.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://kbw.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://fre.xuanzx.com

val m = mapOf("a" to 1)
来源：http://zyx.pycfn.com

[T14] Kotlin：循环
来源：http://rpl.yongpay.top

for (i in 1..10) println(i)
来源：http://xow.gotoacloud.top

[T15] Kotlin：接口
来源：http://fhi.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://cle.316326.xyz

[T16] Swift：Hello World
来源：http://eel.aibaodan.cn

print("Hello")
来源：http://atx.ybcxt.top

[T17] Swift：变量与常量
来源：http://kgn.chenlongwang.top

var a = 1;  let b = 2
来源：http://nky.zhixingplan.top

[T18] Swift：字符串插值
来源：http://lqc.redwolf501.top

"值: \(b)"
来源：http://our.hywenlv.cn

[T19] Swift：可选绑定
来源：http://ahr.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://pyn.ctjpmb.com

[T20] Swift：数组操作
来源：http://fat.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ccx.bjfxy.top

[T21] Swift：遍历
来源：http://myd.fktsv.cn

for x in a { print(x) }
来源：http://jrx.xuetiantiany.cn

[T22] Swift：字典
来源：http://ovt.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://dnj.hongshengwenyu.top

[T23] Swift：函数
来源：http://mni.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dzd.ivvv.top

[T24] Swift：闭包
来源：http://yyy.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxg.zhongyouzk.top

[T25] Swift：结构体
来源：http://tqh.guowangkeji.top

struct P { var x: Int }
来源：http://fdl.redwolf501.top

[T26] Swift：类与重写
来源：http://dal.ppjwa.cn

class A: Base { override func f() {} }
来源：http://gvl.yonumen.top

[T27] Swift：错误处理
来源：http://hfa.yongpay.top

do { try f() } catch { print(error) }
来源：http://mia.vehdjk.com

[T28] Swift：枚举
来源：http://ylh.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://ejs.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://kkb.shangyingyoupin.top

guard let x = opt else { return }
来源：http://kwz.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://dsa.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://xrv.hnqzz.top

[T31] Lua：Hello World
来源：http://vfn.guannengcc.top

print("Hello")
来源：http://qkt.gzhubu.top

[T32] Lua：局部变量
来源：http://hzd.hnxiangtu.top

local a = 1
来源：http://eiq.hnqzz.top

[T33] Lua：表（数组）
来源：http://jmn.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://stq.yangfankeji.com

[T34] Lua：遍历表
来源：http://imn.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tcw.pengpengdd.cyou

[T35] Lua：字典表
来源：http://vav.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://gzw.jinqigufen.top

[T36] Lua：函数
来源：http://uwg.aibaodan.cn

function add(a, b) return a + b end
来源：http://wky.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://tiq.sweek.top

"a" .. "b"
来源：http://hhd.chenjidiqi.icu

[T38] Lua：条件
来源：http://yeu.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://ebq.pycfn.com

[T39] Lua：模式匹配
来源：http://sek.gotoacloud.top

string.find(s, "%d+")
来源：http://bea.jqgufenzy.top

[T40] Lua：元表
来源：http://gjd.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://itw.epnwcf.com

[T41] Perl：Hello World
来源：http://irk.zhaomingkeji.xyz

print "Hello\n";
来源：http://dzr.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://ftu.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://avk.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://emq.zhiwuduotai.top

"值: $a"
来源：http://xzf.fktsv.cn

[T44] Perl：条件
来源：http://zfo.cashguo.top

if ($a > 0) { print "正"; }
来源：http://ygn.sxryk.cn

[T45] Perl：数组遍历
来源：http://knq.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://lcj.zycfv.cn

[T46] Perl：哈希操作
来源：http://xbg.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lau.vehdjk.com

[T47] Perl：正则捕获
来源：http://fwc.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gaj.bjfxy.top

[T48] Perl：正则替换
来源：http://hts.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://yvm.gaohongyu789.top

[T49] Perl：函数
来源：http://wun.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://alq.smart0.xyz

[T50] Perl：逐行读文件
来源：http://vvu.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://vxq.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://pyu.bbcook.cn

[T51] Scala：Hello World
来源：http://tcg.jyoumei.cn

println("Hello")
来源：http://jsl.ehwqpu.com

[T52] Scala：变量
来源：http://qxo.uphjek.com

val a = 1;  var b = 2
来源：http://yin.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://jbc.zdbjq.cn

s"值: $b"
来源：http://gkd.yongpay.top

[T54] Scala：集合映射
来源：http://zwf.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://slm.zhengqikj.top

[T55] Scala：集合过滤
来源：http://ofo.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://kro.jlsjyb.cn

[T56] Scala：样例类
来源：http://bkn.bbcook.cn

case class User(name: String, age: Int)
来源：http://vmt.smart0.xyz

[T57] Scala：模式匹配
来源：http://ccn.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wwd.tianlin.xyz

[T58] Scala：函数定义
来源：http://pzo.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bgz.yfazqb.com

[T59] Scala：循环
来源：http://wge.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://oyi.uphjek.com

[T60] Scala：折叠
来源：http://kyy.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tof.0kj1m.cn

================================================================================
来源：http://spg.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ghb.feifeiyinyue.top

================================================================================
来源：http://aza.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://kiu.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wly.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://sjl.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cfw.9152youxi.cn

[U03] Py：加载 .env 配置
来源：http://psf.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://czo.zdbjq.cn

[U04] Py：变量调试打印
来源：http://qnj.epnwcf.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bcr.tarul.cn

[U05] Py：列表去重且保序
来源：http://wkg.smart0.xyz

list(dict.fromkeys(arr))
来源：http://rjw.bbcook.cn

[U06] Py：合并两个字典
来源：http://npg.sxryk.cn

{**a, **b}
来源：http://joq.smart0.xyz

[U07] Py：反转字典键值
来源：http://sgw.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://edj.cucudq.cn

[U08] Py：展平二维列表
来源：http://icg.yuanzhike.top

[y for x in nested for y in x]
来源：http://mpn.iojbl.cn

[U09] Py：字典取最大值的键
来源：http://fzw.feifeiyinyue.top

max(d, key=d.get)
来源：http://sre.yvedp.cn

[U10] Py：按值排序字典
来源：http://dzt.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mxg.jqgfzy.top

[U11] Py：生成器表达式
来源：http://brx.sjlbkw.cn

(x * 2 for x in arr)
来源：http://jdb.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://jas.guowangkeji.top

Counter(arr).most_common(3)
来源：http://rcu.cashguo.top

[U13] Py：固定长度队列
来源：http://ilv.gzhubu.top

deque(maxlen=10)
来源：http://esa.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://egm.zhengqikj.top

defaultdict(list)
来源：http://lro.yj20258.top

[U15] Py：高精度计时
来源：http://hph.zhijiandao.cn

t = time.perf_counter()
来源：http://opz.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://psh.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dle.fehbvm.com

[U17] Py：初始化日志
来源：http://pcs.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://jlz.tianlin.xyz

[U18] Py：预编译正则
来源：http://xus.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://ylf.havefunace.top

[U19] Py：正则替换带回调
来源：http://ury.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yqa.nwbrower.top

[U20] Py：缓存函数结果
来源：http://rei.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://blg.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://njt.quarkkingdee.top

@contextlib.contextmanager
来源：http://ffm.jqgfzy.top

[U22] Py：矩阵转置
来源：http://moj.tanke756.top

list(zip(*m))
来源：http://isv.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://zci.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ozj.yangfankeji.com

[U24] Py：路径操作
来源：http://xdm.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jem.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://gou.jinghuilouyu.cn

csv.DictReader(f)
来源：http://qmn.ydjk.org.cn

[U26] Py：并发下载
来源：http://zhz.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://snd.fzhhl.top

[U27] Py：异步 HTTP
来源：http://rhn.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://vje.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://aut.yj20258888.top

UserId = int
来源：http://bdt.tanke756.top


<!-- 参考信息 -->