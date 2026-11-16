代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uxx.9152youxi.cn

[S10] C：指针与解引用
来源：http://hfw.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://wlp.fktsv.cn

[S11] C：逐行读文件
来源：http://qpx.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://dmi.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ueg.havefunace.top

fclose(f);
来源：http://lgs.hnxiangtu.top

[S12] C：写文件
来源：http://ttu.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ggp.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://yrj.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dcq.jqgfzy.top

[S14] C：枚举
来源：http://wbo.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://ruf.fzhhl.top

[S15] C：类型转换
来源：http://vck.nanxuanxn.top

(double) a / b
来源：http://ysf.chenjidiqi.icu

[S16] C：位操作置位
来源：http://vhe.yonumen.top

x |= (1 << 3);
来源：http://oer.gzhubu.top

[S17] C：安全拼接字符串
来源：http://jgn.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zbs.yuanzhike.top

[S18] C：命令行参数
来源：http://glj.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://veq.dashuyun.cn

[S19] C：快速排序
来源：http://gke.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://tow.ivvv.top

[S20] C：二分查找
来源：http://fmf.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yxh.nwbrower.top

[S21] C：字符类别判断
来源：http://tdp.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bmu.ehwqpu.com

[S22] C：字符串转数字
来源：http://kgn.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://xuj.iojbl.cn

[S23] C：随机数
来源：http://qms.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://nrs.havefunace.top

[S24] C：获取本地时间
来源：http://fdb.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tzj.zhoulong.xyz

[S25] C：内存拷贝
来源：http://ljc.fengsongda.top

memcpy(dst, src, n);
来源：http://sho.sjlbkw.cn

[S26] C：内存清零
来源：http://zsn.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://cck.ivvv.top

[S27] C：定义常量
来源：http://nyz.uphjek.com

const double PI = 3.14159;
来源：http://fix.jyoumei.cn

[S28] C：静态变量
来源：http://wey.hammf.cn

static int counter = 0;
来源：http://ybf.chenzaomai.com

[S29] C：变参函数
来源：http://zwc.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mje.hfpthk.cn

[S30] C：头文件保护
来源：http://dzl.shangyingyoupin.top

#ifndef X_H
来源：http://kcv.ybcxt.top

#define X_H
来源：http://ryy.xuanzx.com

#endif
来源：http://qbn.havefunace.top

[S31] C++：Hello World
来源：http://wzz.9152youxi.cn

#include <iostream>
来源：http://bqp.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://qki.cqqwz.cn

[S32] C++：字符串
来源：http://nih.sweek.top

std::string s = "hi";  s += "!";
来源：http://yhn.redwolf501.top

[S33] C++：vector 增删
来源：http://ged.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://trd.yongpay.top

[S34] C++：遍历 vector
来源：http://zzk.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://igw.yuxming.cn

[S35] C++：map
来源：http://kcz.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eju.jinqigufen.top

[S36] C++：unordered_map
来源：http://aed.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nla.wangshuangyany.cn

[S37] C++：set
来源：http://qgs.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jnj.xylfe.cn

[S38] C++：排序
来源：http://kam.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://tok.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://uki.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://osu.smart0.xyz

[S40] C++：查找元素
来源：http://ifi.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mjx.xziqi.cn

[S41] C++：类与构造函数
来源：http://nff.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tze.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://yod.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://xey.ydzc1.top

[S43] C++：智能指针
来源：http://yri.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://owd.wangshuangyany.cn

[S44] C++：引用传参
来源：http://lum.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://tra.bjfxy.top

[S45] C++：lambda
来源：http://jxy.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://okk.jiagoushi.top

[S46] C++：函数模板
来源：http://gso.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vkj.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://tkj.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jss.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://bjk.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://vai.andypj.xyz

while (std::getline(in, line)) { }
来源：http://gmh.shangyingyoupin.top

[S49] C++：写文件
来源：http://acp.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://luv.meibo888.top

[S50] C++：格式化数字
来源：http://cdc.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dlc.yangfankeji.com

[S51] C++：显式类型转换
来源：http://mni.jqgfzy.top

static_cast<double>(a) / b
来源：http://twg.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://vrw.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://rhi.jinqigufen.top

[S53] C++：移动语义
来源：http://xsk.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://gex.bjfxy.top

[S54] C++：异常处理
来源：http://lgc.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tjq.iojbl.cn

[S55] C++：结构化绑定
来源：http://bsy.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cqw.yonumen.top

[S56] C++：optional
来源：http://pdj.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://amt.aizwys.cn

[S57] C++：编译期常量
来源：http://zam.snrcjt.cn

constexpr int N = 10;
来源：http://jxp.9152youxi.cn

[S58] C++：命名空间
来源：http://ksk.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://nvu.fktsv.cn

[S59] C++：静态断言
来源：http://rpk.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hwf.cashguo.top

[S60] C++：遍历并删除元素
来源：http://utd.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbi.xziqi.cn

================================================================================
来源：http://epo.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfa.wangdashe.top

================================================================================
来源：http://jin.cucudq.cn

[T01] Kotlin：Hello World
来源：http://rzj.chenzaomai.com

println("Hello")
来源：http://gfu.guannengcc.top

[T02] Kotlin：变量
来源：http://ncr.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rll.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://slr.daxiang520.top

"值: $b"
来源：http://uly.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://ihv.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://ijf.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://iyj.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lfr.epnwcf.com

[T06] Kotlin：集合映射
来源：http://fbc.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dgg.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://jfb.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://upv.jinqigufen.top

[T08] Kotlin：数据类
来源：http://zwf.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://jdn.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://ela.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://uzt.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://eip.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mzs.yj20258888.top

[T11] Kotlin：协程
来源：http://dtk.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xlv.ybcxt.top

[T12] Kotlin：解构声明
来源：http://yhn.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://pne.316326.xyz

[T13] Kotlin：只读 Map
来源：http://xea.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://pab.svipenyu.cn

[T14] Kotlin：循环
来源：http://gmv.shuidangran.top

for (i in 1..10) println(i)
来源：http://kbp.0kj1m.cn

[T15] Kotlin：接口
来源：http://riq.ybcxt.top

interface Shape { fun area(): Double }
来源：http://ozc.tianlin.xyz

[T16] Swift：Hello World
来源：http://tca.jianghu66.top

print("Hello")
来源：http://nef.cucudq.cn

[T17] Swift：变量与常量
来源：http://fmb.shuidangran.top

var a = 1;  let b = 2
来源：http://qqf.aizwys.cn

[T18] Swift：字符串插值
来源：http://tel.fanxiaobao.xyz

"值: \(b)"
来源：http://bgf.hywenlv.cn

[T19] Swift：可选绑定
来源：http://fii.yangfankeji.com

if let n = opt { print(n) }
来源：http://sgg.redwolf501.top

[T20] Swift：数组操作
来源：http://jcv.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vof.9152youxi.cn

[T21] Swift：遍历
来源：http://csw.meibo888.top

for x in a { print(x) }
来源：http://frl.snrcjt.cn

[T22] Swift：字典
来源：http://rdh.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://irp.jyoumei.cn

[T23] Swift：函数
来源：http://czl.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jyi.ybcxt.top

[T24] Swift：闭包
来源：http://ful.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://urn.hammf.cn

[T25] Swift：结构体
来源：http://cqu.yvedp.cn

struct P { var x: Int }
来源：http://tow.tarul.cn

[T26] Swift：类与重写
来源：http://sps.zhengqikj.top

class A: Base { override func f() {} }
来源：http://wkr.sjlbkw.cn

[T27] Swift：错误处理
来源：http://ijy.xuanzx.com

do { try f() } catch { print(error) }
来源：http://huy.zhengqikj.top

[T28] Swift：枚举
来源：http://zpa.xylfe.cn

enum Color { case red, green }
来源：http://ilv.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://vdk.jinqigfzy.top

guard let x = opt else { return }
来源：http://oex.jianghu66.top

[T30] Swift：协议
来源：http://dem.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://ruz.yonumen.top

[T31] Lua：Hello World
来源：http://ovk.hysaishi.cn

print("Hello")
来源：http://utm.ctjpmb.com

[T32] Lua：局部变量
来源：http://zsp.zhixingplan.top

local a = 1
来源：http://dis.ybcxt.top

[T33] Lua：表（数组）
来源：http://ykd.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://puf.shzxlz.cn

[T34] Lua：遍历表
来源：http://vli.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wfx.yanxiufei.cn

[T35] Lua：字典表
来源：http://kty.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://lvn.uphjek.com

[T36] Lua：函数
来源：http://nka.quarkkingdee.top

function add(a, b) return a + b end
来源：http://tja.daxiang520.top

[T37] Lua：字符串拼接
来源：http://rvy.52xcode.cn

"a" .. "b"
来源：http://vkr.iojbl.cn

[T38] Lua：条件
来源：http://rdx.ehwqpu.com

if x > 0 then print("正") end
来源：http://hdx.xuanzx.com

[T39] Lua：模式匹配
来源：http://pwa.tarul.cn

string.find(s, "%d+")
来源：http://vuo.jinghuilouyu.cn

[T40] Lua：元表
来源：http://jib.yfazqb.com

setmetatable({}, { __index = base })
来源：http://drw.nanxinkj.top

[T41] Perl：Hello World
来源：http://qwx.cheryme.top

print "Hello\n";
来源：http://wej.ydjk.org.cn

[T42] Perl：变量类型
来源：http://kdo.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xrp.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://cyt.fanxiaobao.xyz

"值: $a"
来源：http://cmd.haohaochexian.top

[T44] Perl：条件
来源：http://oqy.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://oqk.hnqzz.top

[T45] Perl：数组遍历
来源：http://lho.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://nsm.yuxming.cn

[T46] Perl：哈希操作
来源：http://rra.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tuo.hammf.cn

[T47] Perl：正则捕获
来源：http://yvl.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eid.xylfe.cn

[T48] Perl：正则替换
来源：http://lyp.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://wrt.yueranfly.top

[T49] Perl：函数
来源：http://smk.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mrt.hywenlv.cn

[T50] Perl：逐行读文件
来源：http://jgi.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wkl.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://sty.aibaodan.cn

[T51] Scala：Hello World
来源：http://aid.fanxiaobao.xyz

println("Hello")
来源：http://twv.birdmap.top

[T52] Scala：变量
来源：http://qka.ydzc1.top

val a = 1;  var b = 2
来源：http://nae.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://flh.yj20258888.top

s"值: $b"
来源：http://gzs.tian-w.cn

[T54] Scala：集合映射
来源：http://lxg.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://ibt.bbcook.cn

[T55] Scala：集合过滤
来源：http://xpd.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iij.yj20258.top

[T56] Scala：样例类
来源：http://jnj.hnqzz.top

case class User(name: String, age: Int)
来源：http://adx.hywenlv.cn

[T57] Scala：模式匹配
来源：http://wwk.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://njo.zhengqikj.top

[T58] Scala：函数定义
来源：http://fek.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://lsm.ydzc1.top

[T59] Scala：循环
来源：http://bhf.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://gyt.ctjpmb.com

[T60] Scala：折叠
来源：http://zom.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xdr.chenlongwang.top

================================================================================
来源：http://jic.xinyue.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yzn.nanxinkj.top

================================================================================
来源：http://dvc.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://rod.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://myu.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://ken.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aav.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://wno.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xvj.fengsongda.top

[U04] Py：变量调试打印
来源：http://wrv.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mpy.meibo888.top

[U05] Py：列表去重且保序
来源：http://waf.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://klu.zhixingplan.top

[U06] Py：合并两个字典
来源：http://zes.yj202588.top

{**a, **b}
来源：http://ttw.9152youxi.cn

[U07] Py：反转字典键值
来源：http://yxu.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://bip.xuanzx.com

[U08] Py：展平二维列表
来源：http://vny.yuxming.cn

[y for x in nested for y in x]
来源：http://thj.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://lfz.ybcxt.top

max(d, key=d.get)
来源：http://jwp.shanyushiyangtech.top

[U10] Py：按值排序字典
来源：http://zwa.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wkk.tarul.cn

[U11] Py：生成器表达式
来源：http://rhq.hnqzz.top

(x * 2 for x in arr)
来源：http://eow.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://tcz.9152youxi.cn

Counter(arr).most_common(3)
来源：http://bwp.ehwqpu.com

[U13] Py：固定长度队列
来源：http://chx.sxryk.cn

deque(maxlen=10)
来源：http://xro.fengsongda.top

[U14] Py：分组收集到列表
来源：http://mzg.zycfv.cn

defaultdict(list)
来源：http://vdm.shuidangran.top

[U15] Py：高精度计时
来源：http://cvk.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://bsi.iojbl.cn

[U16] Py：命令行参数解析
来源：http://otq.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://scq.gogol.net.cn

[U17] Py：初始化日志
来源：http://mav.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://akp.birdmap.top

[U18] Py：预编译正则
来源：http://mpu.yj202588.top

pat = re.compile(r"\d+")
来源：http://ces.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://tic.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jmb.iojbl.cn

[U20] Py：缓存函数结果
来源：http://dng.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://bhx.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://rah.zhoulong.xyz

@contextlib.contextmanager
来源：http://ssp.yfazqb.com

[U22] Py：矩阵转置
来源：http://wsi.cashguo.top

list(zip(*m))
来源：http://qgw.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://wdz.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://viv.hnqzz.top

[U24] Py：路径操作
来源：http://nug.xylfe.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qzy.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://sdu.gaohongyu789.top

csv.DictReader(f)
来源：http://pjw.haohaochexian.top

[U26] Py：并发下载
来源：http://zkq.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mav.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://ssn.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://wlw.pengpengdd.cyou

[U28] Py：类型别名
来源：http://bcd.c1oappe.top

UserId = int
来源：http://yjg.zycfv.cn

[U29] Py：属性校验
来源：http://szp.jiagoushi.top

@property 与 @x.setter 配合
来源：http://fpw.shzxlz.cn

[U30] Py：数据类
来源：http://xxw.jlsjyb.cn

@dataclass(slots=True)
来源：http://rsd.xuanzx.com

[U31] Py：单测
来源：http://leu.9152youxi.cn

python -m pytest -q
来源：http://rfl.tianlin.xyz

[U32] Py：代码格式化
来源：http://xao.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://zup.gogol.net.cn


<!-- 参考信息 -->