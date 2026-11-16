代发 wailian999

int x; scanf("%d", &x);
来源：http://ngh.yvedp.cn

[S04] C：字符串复制
来源：http://fro.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://hrv.zycfv.cn

[S05] C：字符串长度
来源：http://igc.yj20258.top

strlen(s)
来源：http://rrr.52xcode.cn

[S06] C：字符串比较
来源：http://roq.zhengqikj.top

strcmp(a, b) == 0
来源：http://scv.cqqwz.cn

[S07] C：数组遍历求和
来源：http://sqp.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ile.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://ozc.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mnk.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://vgj.zdbjq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ywg.hesvh.cn

[S10] C：指针与解引用
来源：http://pva.fktsv.cn

int *p = &a;  *p = 5;
来源：http://oco.jqgufenzy.top

[S11] C：逐行读文件
来源：http://hbc.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://wvp.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pub.sjlbkw.cn

fclose(f);
来源：http://ugw.hongshengwenyu.top

[S12] C：写文件
来源：http://bip.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://njj.yfazqb.com

[S13] C：宏定义
来源：http://cmt.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://erl.bbcook.cn

[S14] C：枚举
来源：http://ftc.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://vdp.hfpthk.cn

[S15] C：类型转换
来源：http://hkm.redwolf501.top

(double) a / b
来源：http://kge.zhiwuduotai.top

[S16] C：位操作置位
来源：http://eyu.daria6918.cn

x |= (1 << 3);
来源：http://tdn.316326.xyz

[S17] C：安全拼接字符串
来源：http://mzo.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://knw.yueranfly.top

[S18] C：命令行参数
来源：http://isz.jinqigufen.top

int main(int argc, char **argv)
来源：http://pew.xuetiantiany.cn

[S19] C：快速排序
来源：http://jfo.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nyn.fzhhl.top

[S20] C：二分查找
来源：http://rpc.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vox.sysykeji.top

[S21] C：字符类别判断
来源：http://sck.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hhf.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://jjf.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://wzd.yj20258.top

[S23] C：随机数
来源：http://bar.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dvm.dianchejie.cn

[S24] C：获取本地时间
来源：http://dvb.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rvh.hysaishi.cn

[S25] C：内存拷贝
来源：http://mqp.cdnleiting.top

memcpy(dst, src, n);
来源：http://owg.ehwqpu.com

[S26] C：内存清零
来源：http://mzu.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://qja.cashguo.top

[S27] C：定义常量
来源：http://nuk.gaohongyu789.top

const double PI = 3.14159;
来源：http://gwe.sjlbkw.cn

[S28] C：静态变量
来源：http://fnz.ivvv.top

static int counter = 0;
来源：http://rgw.zdbjq.cn

[S29] C：变参函数
来源：http://gvf.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zka.zhoulong.xyz

[S30] C：头文件保护
来源：http://xxm.yj20258.top

#ifndef X_H
来源：http://aws.hywenlv.cn

#define X_H
来源：http://wyl.jianghu66.top

#endif
来源：http://joz.nanxinkj.top

[S31] C++：Hello World
来源：http://ugx.316326.xyz

#include <iostream>
来源：http://lgj.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://sqp.dianchejie.cn

[S32] C++：字符串
来源：http://wex.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://rgx.aibaodan.cn

[S33] C++：vector 增删
来源：http://nmf.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rdg.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://dwi.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://wub.snrcjt.cn

[S35] C++：map
来源：http://ror.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hww.sjlbkw.cn

[S36] C++：unordered_map
来源：http://jfn.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jcz.fehbvm.com

[S37] C++：set
来源：http://gva.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zhq.cdnleiting.top

[S38] C++：排序
来源：http://kqm.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://ekk.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://pzs.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ooo.yongpay.top

[S40] C++：查找元素
来源：http://djf.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://luz.fengsongda.top

[S41] C++：类与构造函数
来源：http://syd.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dvq.xinyue.icu

[S42] C++：继承与虚函数
来源：http://twb.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://foj.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://iau.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://akr.xuanzx.com

[S44] C++：引用传参
来源：http://fve.birdmap.top

void inc(int &x) { ++x; }
来源：http://cxm.zdbjq.cn

[S45] C++：lambda
来源：http://eld.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sxl.zhengqikj.top

[S46] C++：函数模板
来源：http://sfn.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dph.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://lfv.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsz.yongpay.top

[S48] C++：逐行读文件
来源：http://kea.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pwd.bbcook.cn

while (std::getline(in, line)) { }
来源：http://hmw.fzhhl.top

[S49] C++：写文件
来源：http://mii.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avr.cqqwz.cn

[S50] C++：格式化数字
来源：http://jgv.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ypz.hysaishi.cn

[S51] C++：显式类型转换
来源：http://pps.gotoacloud.top

static_cast<double>(a) / b
来源：http://rsf.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://gtr.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://ucj.ydjk.org.cn

[S53] C++：移动语义
来源：http://ozn.havefunace.top

std::vector<int> w = std::move(v);
来源：http://zmu.guannengcc.top

[S54] C++：异常处理
来源：http://gzy.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jqr.aizwys.cn

[S55] C++：结构化绑定
来源：http://kve.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rgs.dashuyun.cn

[S56] C++：optional
来源：http://vto.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nwx.yanxiufei.cn

[S57] C++：编译期常量
来源：http://gwt.jqgfzy.top

constexpr int N = 10;
来源：http://vqa.daria6918.cn

[S58] C++：命名空间
来源：http://rxu.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://zcn.fzhhl.top

[S59] C++：静态断言
来源：http://ats.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tim.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://cil.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qgs.epnwcf.com

================================================================================
来源：http://gcz.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywf.epnwcf.com

================================================================================
来源：http://ulb.52xcode.cn

[T01] Kotlin：Hello World
来源：http://new.zdqjudy.top

println("Hello")
来源：http://mvy.zhijiandao.cn

[T02] Kotlin：变量
来源：http://ysf.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://egg.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://tgz.andypj.xyz

"值: $b"
来源：http://xet.guannengcc.top

[T04] Kotlin：空安全
来源：http://dkl.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://bsw.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://nka.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oug.xuanzx.com

[T06] Kotlin：集合映射
来源：http://alp.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tfm.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://yvh.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fem.ydzc1.top

[T08] Kotlin：数据类
来源：http://kbk.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://cbr.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://vds.hammf.cn

fun String.exclaim() = this + "!"
来源：http://brl.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://apl.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://otp.snrcjt.cn

[T11] Kotlin：协程
来源：http://zsk.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://scx.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://yxf.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://hcb.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://ryk.iojbl.cn

val m = mapOf("a" to 1)
来源：http://tri.guowangkeji.top

[T14] Kotlin：循环
来源：http://ynq.xuanzx.com

for (i in 1..10) println(i)
来源：http://lqp.jinqigufen.top

[T15] Kotlin：接口
来源：http://qur.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://nko.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://cxq.fktsv.cn

print("Hello")
来源：http://agb.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://srz.kuanghao11.cn

var a = 1;  let b = 2
来源：http://cza.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://pwx.havefunace.top

"值: \(b)"
来源：http://jvl.yvedp.cn

[T19] Swift：可选绑定
来源：http://twl.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://sku.quarkkingdee.top

[T20] Swift：数组操作
来源：http://rjj.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://tci.gogol.net.cn

[T21] Swift：遍历
来源：http://npd.zhengqikj.top

for x in a { print(x) }
来源：http://nht.aibaodan.cn

[T22] Swift：字典
来源：http://wkd.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://usq.yonumen.top

[T23] Swift：函数
来源：http://nye.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://avo.ydjk.org.cn

[T24] Swift：闭包
来源：http://wrs.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://kan.yuanzhike.top

[T25] Swift：结构体
来源：http://pqp.havefunace.top

struct P { var x: Int }
来源：http://fan.ydzc1.top

[T26] Swift：类与重写
来源：http://yeq.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://wif.ybcxt.top

[T27] Swift：错误处理
来源：http://vze.ivvv.top

do { try f() } catch { print(error) }
来源：http://fcy.epnwcf.com

[T28] Swift：枚举
来源：http://uay.snrcjt.cn

enum Color { case red, green }
来源：http://bwn.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://pxr.hesvh.cn

guard let x = opt else { return }
来源：http://aeu.sxryk.cn

[T30] Swift：协议
来源：http://ujf.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://ufb.cdnleiting.top

[T31] Lua：Hello World
来源：http://bdv.jinqigufen.top

print("Hello")
来源：http://udl.ydzc1.top

[T32] Lua：局部变量
来源：http://ztl.52xcode.cn

local a = 1
来源：http://zdv.aizwys.cn

[T33] Lua：表（数组）
来源：http://tlp.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://phf.cheryme.top

[T34] Lua：遍历表
来源：http://xaz.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://euz.yonumen.top

[T35] Lua：字典表
来源：http://ktq.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://vod.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://bqc.fehbvm.com

function add(a, b) return a + b end
来源：http://vsi.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://vss.guannengcc.top

"a" .. "b"
来源：http://nxb.xziqi.cn

[T38] Lua：条件
来源：http://rpy.quarkkingdee.top

if x > 0 then print("正") end
来源：http://nts.sweek.top

[T39] Lua：模式匹配
来源：http://obx.zhengqikj.top

string.find(s, "%d+")
来源：http://dhu.havefunace.top

[T40] Lua：元表
来源：http://jwz.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://qyl.gogol.net.cn

[T41] Perl：Hello World
来源：http://zcm.sweek.top

print "Hello\n";
来源：http://qvl.xylfe.cn

[T42] Perl：变量类型
来源：http://ufg.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rlp.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://chf.jyoumei.cn

"值: $a"
来源：http://fgg.zycfv.cn

[T44] Perl：条件
来源：http://bgb.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://xkc.sxryk.cn

[T45] Perl：数组遍历
来源：http://bvy.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://cqy.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://qfx.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wan.dashuyun.cn

[T47] Perl：正则捕获
来源：http://xwx.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nui.uphjek.com

[T48] Perl：正则替换
来源：http://xix.yvedp.cn

$s =~ s/old/new/g;
来源：http://csh.yj202588.top

[T49] Perl：函数
来源：http://lat.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ywx.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://oqt.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gom.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://sjn.hammf.cn

[T51] Scala：Hello World
来源：http://xag.cucudq.cn

println("Hello")
来源：http://trf.ppjwa.cn

[T52] Scala：变量
来源：http://srt.hfpthk.cn

val a = 1;  var b = 2
来源：http://xbh.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://ipw.xylfe.cn

s"值: $b"
来源：http://yin.bjfxy.top

[T54] Scala：集合映射
来源：http://trx.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://kiq.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://rsg.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vup.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://nmg.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://mys.uphjek.com

[T57] Scala：模式匹配
来源：http://std.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zyw.cucudq.cn

[T58] Scala：函数定义
来源：http://wem.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://rok.yfazqb.com

[T59] Scala：循环
来源：http://vjs.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://wts.nanxuanxn.top

[T60] Scala：折叠
来源：http://uyn.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hct.snrcjt.cn

================================================================================
来源：http://ccb.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jli.zhixingplan.top

================================================================================
来源：http://vtt.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://puy.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://exx.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://vbc.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dkk.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://uco.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ufp.dianchejie.cn

[U04] Py：变量调试打印
来源：http://mrv.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ztu.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://tqf.hammf.cn

list(dict.fromkeys(arr))
来源：http://thg.meibo888.top

[U06] Py：合并两个字典
来源：http://pdg.kuanghao11.cn

{**a, **b}
来源：http://emp.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://slx.meibo888.top

{v: k for k, v in d.items()}
来源：http://jik.sxryk.cn

[U08] Py：展平二维列表
来源：http://ufv.smart0.xyz

[y for x in nested for y in x]
来源：http://csm.havefunace.top

[U09] Py：字典取最大值的键
来源：http://rbp.shangyingyoupin.top

max(d, key=d.get)
来源：http://rhm.hammf.cn

[U10] Py：按值排序字典
来源：http://ddu.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lxh.dashuyun.cn

[U11] Py：生成器表达式
来源：http://jin.sjlbkw.cn

(x * 2 for x in arr)
来源：http://pzn.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://lbm.aizwys.cn

Counter(arr).most_common(3)
来源：http://aay.snrcjt.cn

[U13] Py：固定长度队列
来源：http://hda.jyoumei.cn

deque(maxlen=10)
来源：http://ccd.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://blv.xuanzx.com

defaultdict(list)
来源：http://eqw.smart0.xyz

[U15] Py：高精度计时
来源：http://piu.zhoulong.xyz

t = time.perf_counter()
来源：http://emr.bbcook.cn

[U16] Py：命令行参数解析
来源：http://hxd.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fck.ivvv.top

[U17] Py：初始化日志
来源：http://ezv.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://ina.fengsongda.top

[U18] Py：预编译正则
来源：http://zbb.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://kbk.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://ilz.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rax.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://iig.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://rcc.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://inc.ybcxt.top

@contextlib.contextmanager
来源：http://tey.gzhubu.top

[U22] Py：矩阵转置
来源：http://fdy.yj20258.top

list(zip(*m))
来源：http://uvm.xinyue.icu

[U23] Py：分块读取大文件
来源：http://qyw.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qvd.mhx1999.top

[U24] Py：路径操作
来源：http://fom.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gdx.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://syh.gaohongyu789.top

csv.DictReader(f)
来源：http://tkm.tanke756.top

[U26] Py：并发下载
来源：http://jsv.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nqw.yongpay.top


<!-- 参考信息 -->