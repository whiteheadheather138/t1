代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iej.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://ato.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dxx.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://wvt.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xfh.zycfv.cn

[S10] C：指针与解引用
来源：http://kqd.bjfxy.top

int *p = &a;  *p = 5;
来源：http://wgy.uphjek.com

[S11] C：逐行读文件
来源：http://rvn.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://pas.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://miv.nwbrower.top

fclose(f);
来源：http://tke.316326.xyz

[S12] C：写文件
来源：http://kyo.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qdn.chenzaomai.com

[S13] C：宏定义
来源：http://dwg.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wvt.chenlongwang.top

[S14] C：枚举
来源：http://utc.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://khk.gotoacloud.top

[S15] C：类型转换
来源：http://wxk.gogol.net.cn

(double) a / b
来源：http://dfc.bbcook.cn

[S16] C：位操作置位
来源：http://vzx.hnxiangtu.top

x |= (1 << 3);
来源：http://qso.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://xuh.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsk.zhongyouzk.top

[S18] C：命令行参数
来源：http://fpn.daria6918.cn

int main(int argc, char **argv)
来源：http://nat.hesvh.cn

[S19] C：快速排序
来源：http://anb.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bqu.dashuyun.cn

[S20] C：二分查找
来源：http://cxy.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bkj.xziqi.cn

[S21] C：字符类别判断
来源：http://wtz.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nme.epnwcf.com

[S22] C：字符串转数字
来源：http://gxo.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://pcn.hcnkem.com

[S23] C：随机数
来源：http://kyu.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hjr.chenlongwang.top

[S24] C：获取本地时间
来源：http://vfc.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uae.jlsjyb.cn

[S25] C：内存拷贝
来源：http://vel.shzxlz.cn

memcpy(dst, src, n);
来源：http://svc.guowangkeji.top

[S26] C：内存清零
来源：http://wsd.bjfxy.top

memset(a, 0, sizeof a);
来源：http://sbe.jinghuilouyu.cn

[S27] C：定义常量
来源：http://uam.chenzaomai.com

const double PI = 3.14159;
来源：http://qtd.iojbl.cn

[S28] C：静态变量
来源：http://piv.zhaomingkeji.xyz

static int counter = 0;
来源：http://dgt.yuanzhike.top

[S29] C：变参函数
来源：http://vxl.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://src.zhengqikj.top

[S30] C：头文件保护
来源：http://tgo.ctjpmb.com

#ifndef X_H
来源：http://dbz.pycfn.com

#define X_H
来源：http://rih.ppjwa.cn

#endif
来源：http://vbp.nwbrower.top

[S31] C++：Hello World
来源：http://agl.yvedp.cn

#include <iostream>
来源：http://uhq.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://tcv.cqqwz.cn

[S32] C++：字符串
来源：http://zli.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://ege.gaohongyu789.top

[S33] C++：vector 增删
来源：http://oyi.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dge.yangfankeji.com

[S34] C++：遍历 vector
来源：http://drg.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://zcs.wangshuangyany.cn

[S35] C++：map
来源：http://ess.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aoy.tianlin.xyz

[S36] C++：unordered_map
来源：http://mqn.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yna.chenjidiqi.icu

[S37] C++：set
来源：http://sml.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zoj.fehbvm.com

[S38] C++：排序
来源：http://jrz.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://vca.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://xge.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hwt.bjfxy.top

[S40] C++：查找元素
来源：http://rmu.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sra.yuxming.cn

[S41] C++：类与构造函数
来源：http://lyn.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tbh.daria6918.cn

[S42] C++：继承与虚函数
来源：http://wba.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://awy.jyoumei.cn

[S43] C++：智能指针
来源：http://syp.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://ngv.ehwqpu.com

[S44] C++：引用传参
来源：http://wzi.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://kyt.aizwys.cn

[S45] C++：lambda
来源：http://tda.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://lge.daria6918.cn

[S46] C++：函数模板
来源：http://bmf.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wru.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://wys.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yrj.hywenlv.cn

[S48] C++：逐行读文件
来源：http://gah.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://rri.bjfxy.top

while (std::getline(in, line)) { }
来源：http://udr.fehbvm.com

[S49] C++：写文件
来源：http://ayo.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aks.mhx1999.top

[S50] C++：格式化数字
来源：http://kix.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bly.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://pph.xinyue.icu

static_cast<double>(a) / b
来源：http://xgo.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://oqd.redwolf501.top

int size() const noexcept { return n_; }
来源：http://bzo.xuetiantiany.cn

[S53] C++：移动语义
来源：http://vcp.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://zin.9152youxi.cn

[S54] C++：异常处理
来源：http://nml.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ghd.chenzaomai.com

[S55] C++：结构化绑定
来源：http://cmu.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vwo.wangdashe.top

[S56] C++：optional
来源：http://aad.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://giy.c1oappe.top

[S57] C++：编译期常量
来源：http://bvx.sysykeji.top

constexpr int N = 10;
来源：http://ddn.guowangkeji.top

[S58] C++：命名空间
来源：http://vsj.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://oqy.yj202588.top

[S59] C++：静态断言
来源：http://osu.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qmm.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://jxi.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktt.haohaochexian.top

================================================================================
来源：http://wyx.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yak.xinyue.icu

================================================================================
来源：http://pkg.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://jnp.hfpthk.cn

println("Hello")
来源：http://esh.bjfxy.top

[T02] Kotlin：变量
来源：http://zxc.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://urb.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://inc.jinqigufen.top

"值: $b"
来源：http://yjp.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://hmw.ybcxt.top

val n: String? = null;  n?.length
来源：http://sxb.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://gnm.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rea.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://wiy.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://sjd.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://iuf.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jph.nwbrower.top

[T08] Kotlin：数据类
来源：http://wvj.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://btr.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://gjp.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://btw.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://xqe.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eik.hcnkem.com

[T11] Kotlin：协程
来源：http://qnq.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zgi.316326.xyz

[T12] Kotlin：解构声明
来源：http://wyf.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://kzl.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://fyx.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://giy.dashuyun.cn

[T14] Kotlin：循环
来源：http://trc.havefunace.top

for (i in 1..10) println(i)
来源：http://ard.c1oappe.top

[T15] Kotlin：接口
来源：http://dwu.yfazqb.com

interface Shape { fun area(): Double }
来源：http://hwa.cucudq.cn

[T16] Swift：Hello World
来源：http://zzd.vqdsnc.cn

print("Hello")
来源：http://rcc.snrcjt.cn

[T17] Swift：变量与常量
来源：http://oon.aibaodan.cn

var a = 1;  let b = 2
来源：http://nql.yvedp.cn

[T18] Swift：字符串插值
来源：http://jjn.sweek.top

"值: \(b)"
来源：http://yvo.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://axe.redwolf501.top

if let n = opt { print(n) }
来源：http://zpn.fktsv.cn

[T20] Swift：数组操作
来源：http://npu.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://aoe.jiagoushi.top

[T21] Swift：遍历
来源：http://mbi.sxryk.cn

for x in a { print(x) }
来源：http://tzp.kuanghao11.cn

[T22] Swift：字典
来源：http://phn.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://baa.hywenlv.cn

[T23] Swift：函数
来源：http://hqj.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wjs.fehbvm.com

[T24] Swift：闭包
来源：http://ahp.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://isp.zhijiandao.cn

[T25] Swift：结构体
来源：http://ryf.ivvv.top

struct P { var x: Int }
来源：http://dmc.hammf.cn

[T26] Swift：类与重写
来源：http://qcz.xziqi.cn

class A: Base { override func f() {} }
来源：http://kcr.yongpay.top

[T27] Swift：错误处理
来源：http://nih.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://cme.birdmap.top

[T28] Swift：枚举
来源：http://uhg.vqdsnc.cn

enum Color { case red, green }
来源：http://oxz.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://ews.shzxlz.cn

guard let x = opt else { return }
来源：http://uxo.daria6918.cn

[T30] Swift：协议
来源：http://sfz.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://ibu.ppjwa.cn

[T31] Lua：Hello World
来源：http://vzs.feifeiyinyue.top

print("Hello")
来源：http://avi.fehbvm.com

[T32] Lua：局部变量
来源：http://gpi.nanxinkj.top

local a = 1
来源：http://tnc.yj20258.top

[T33] Lua：表（数组）
来源：http://ekr.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hye.hesvh.cn

[T34] Lua：遍历表
来源：http://qfi.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tzs.nanxuanxn.top

[T35] Lua：字典表
来源：http://mzr.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://zfd.nwbrower.top

[T36] Lua：函数
来源：http://tmx.mhx1999.top

function add(a, b) return a + b end
来源：http://zde.daria6918.cn

[T37] Lua：字符串拼接
来源：http://tbp.nwbrower.top

"a" .. "b"
来源：http://vub.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://xcw.yvedp.cn

if x > 0 then print("正") end
来源：http://msr.yonumen.top

[T39] Lua：模式匹配
来源：http://uve.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://qqb.hesvh.cn

[T40] Lua：元表
来源：http://hzg.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://dsg.ppjwa.cn

[T41] Perl：Hello World
来源：http://mbb.xingfuxueyuan.xyz

print "Hello\n";
来源：http://rye.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://yuw.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eoi.smart0.xyz

[T43] Perl：字符串插值
来源：http://vqv.daria6918.cn

"值: $a"
来源：http://bzl.aizwys.cn

[T44] Perl：条件
来源：http://icw.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://qze.yuanzhike.top

[T45] Perl：数组遍历
来源：http://ziu.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://ycq.shuidangran.top

[T46] Perl：哈希操作
来源：http://nua.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ppt.52xcode.cn

[T47] Perl：正则捕获
来源：http://wbq.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kxg.sweek.top

[T48] Perl：正则替换
来源：http://qfu.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://qbh.zhoulong.xyz

[T49] Perl：函数
来源：http://ayd.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zyf.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://ptv.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://qlo.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://gjl.zhijiandao.cn

[T51] Scala：Hello World
来源：http://oad.hcnkem.com

println("Hello")
来源：http://sye.haohaochexian.top

[T52] Scala：变量
来源：http://uer.shzxlz.cn

val a = 1;  var b = 2
来源：http://tdx.birdmap.top

[T53] Scala：字符串插值
来源：http://ypg.hnqzz.top

s"值: $b"
来源：http://wis.haohaochexian.top

[T54] Scala：集合映射
来源：http://mbk.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://bnr.tanke756.top

[T55] Scala：集合过滤
来源：http://eym.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vzu.uphjek.com

[T56] Scala：样例类
来源：http://prr.vehdjk.com

case class User(name: String, age: Int)
来源：http://jpl.tarul.cn

[T57] Scala：模式匹配
来源：http://rpx.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hod.guannengcc.top

[T58] Scala：函数定义
来源：http://ked.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://fxn.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://zxp.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://ldl.nanxinkj.top

[T60] Scala：折叠
来源：http://nsl.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://twf.dashuyun.cn

================================================================================
来源：http://dwt.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oje.yangfankeji.com

================================================================================
来源：http://oqo.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://vvi.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://pxp.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://ezm.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yak.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://yom.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lyd.yangfankeji.com

[U04] Py：变量调试打印
来源：http://gth.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ntx.yongpay.top

[U05] Py：列表去重且保序
来源：http://zyy.xziqi.cn

list(dict.fromkeys(arr))
来源：http://klu.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://swo.fzhhl.top

{**a, **b}
来源：http://pwj.nanxinkj.top

[U07] Py：反转字典键值
来源：http://vjd.hcnkem.com

{v: k for k, v in d.items()}
来源：http://ant.dashuyun.cn

[U08] Py：展平二维列表
来源：http://osi.daria6918.cn

[y for x in nested for y in x]
来源：http://jeh.ydzc1.top

[U09] Py：字典取最大值的键
来源：http://ezi.yfazqb.com

max(d, key=d.get)
来源：http://rfr.chenzaomai.com

[U10] Py：按值排序字典
来源：http://sny.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syx.cheryme.top

[U11] Py：生成器表达式
来源：http://jlx.xziqi.cn

(x * 2 for x in arr)
来源：http://ovc.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://ieq.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://sxn.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://ttv.hywenlv.cn

deque(maxlen=10)
来源：http://uwc.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://dti.bjfxy.top

defaultdict(list)
来源：http://gyq.wangdashe.top

[U15] Py：高精度计时
来源：http://mcn.fengsongda.top

t = time.perf_counter()
来源：http://dtt.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://eep.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fis.hywenlv.cn

[U17] Py：初始化日志
来源：http://bbu.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://jca.cdnleiting.top

[U18] Py：预编译正则
来源：http://vjm.vehdjk.com

pat = re.compile(r"\d+")
来源：http://rdi.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://moz.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qno.tarul.cn

[U20] Py：缓存函数结果
来源：http://trn.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://ena.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://lro.hcnkem.com

@contextlib.contextmanager
来源：http://qvf.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://vql.zdbjq.cn

list(zip(*m))
来源：http://cjg.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://idr.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wie.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://pyb.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rfg.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://obm.fanxiaobao.xyz

csv.DictReader(f)
来源：http://nct.shzxlz.cn

[U26] Py：并发下载
来源：http://qnj.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cgp.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://tfc.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://ome.c1oappe.top

[U28] Py：类型别名
来源：http://vxf.epnwcf.com

UserId = int
来源：http://tyb.yj20258.top

[U29] Py：属性校验
来源：http://dqj.fzhhl.top

@property 与 @x.setter 配合
来源：http://eub.yangfankeji.com

[U30] Py：数据类
来源：http://gmx.guowangkeji.top

@dataclass(slots=True)
来源：http://las.epnwcf.com


<!-- 参考信息 -->