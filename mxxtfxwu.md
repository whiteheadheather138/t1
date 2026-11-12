代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://nbd.bbcook.cn

[S02] C：变量与格式化输出
来源：http://ulb.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://skr.zhongyouzk.top

[S03] C：读入整数
来源：http://uyn.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://baf.pycfn.com

[S04] C：字符串复制
来源：http://igk.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://cdy.mhx1999.top

[S05] C：字符串长度
来源：http://ipq.jqgufenzy.top

strlen(s)
来源：http://pbr.hammf.cn

[S06] C：字符串比较
来源：http://kcz.yvedp.cn

strcmp(a, b) == 0
来源：http://cav.hammf.cn

[S07] C：数组遍历求和
来源：http://gqf.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ljv.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://bgs.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nut.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://nyf.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://amp.ivvv.top

[S10] C：指针与解引用
来源：http://vgg.fktsv.cn

int *p = &a;  *p = 5;
来源：http://oxb.zycfv.cn

[S11] C：逐行读文件
来源：http://kfn.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://vdq.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgi.dianchejie.cn

fclose(f);
来源：http://rhn.iojbl.cn

[S12] C：写文件
来源：http://mqu.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://but.chenlongwang.top

[S13] C：宏定义
来源：http://shd.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brg.yangfankeji.com

[S14] C：枚举
来源：http://eae.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://lfo.dashuyun.cn

[S15] C：类型转换
来源：http://yje.316326.xyz

(double) a / b
来源：http://pco.316326.xyz

[S16] C：位操作置位
来源：http://lhr.redwolf501.top

x |= (1 << 3);
来源：http://wbu.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://xxo.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sjv.yfazqb.com

[S18] C：命令行参数
来源：http://eut.hammf.cn

int main(int argc, char **argv)
来源：http://jqt.quarkkingdee.top

[S19] C：快速排序
来源：http://omd.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rze.cqqwz.cn

[S20] C：二分查找
来源：http://lev.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vuc.wangdashe.top

[S21] C：字符类别判断
来源：http://qaw.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xdw.yfazqb.com

[S22] C：字符串转数字
来源：http://lbe.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://jyj.hongshengwenyu.top

[S23] C：随机数
来源：http://zss.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zcs.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://xij.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgh.xinyue.icu

[S25] C：内存拷贝
来源：http://mjk.zhixingplan.top

memcpy(dst, src, n);
来源：http://gfm.xinyue.icu

[S26] C：内存清零
来源：http://dcy.aizwys.cn

memset(a, 0, sizeof a);
来源：http://gqk.hnxiangtu.top

[S27] C：定义常量
来源：http://mlk.andypj.xyz

const double PI = 3.14159;
来源：http://szk.cashguo.top

[S28] C：静态变量
来源：http://tpc.zdqjudy.top

static int counter = 0;
来源：http://nmf.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://rea.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zna.birdmap.top

[S30] C：头文件保护
来源：http://hku.nanxinkj.top

#ifndef X_H
来源：http://ich.uphjek.com

#define X_H
来源：http://vie.yanxiufei.cn

#endif
来源：http://xdh.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://ydn.hongshengwenyu.top

#include <iostream>
来源：http://rms.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://azh.fengsongda.top

[S32] C++：字符串
来源：http://clb.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://lll.yanxiufei.cn

[S33] C++：vector 增删
来源：http://roj.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hcd.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://nrs.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://tsa.zycfv.cn

[S35] C++：map
来源：http://exc.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://amz.vqdsnc.cn

[S36] C++：unordered_map
来源：http://tiw.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rlr.yanxiufei.cn

[S37] C++：set
来源：http://byi.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://itr.sysykeji.top

[S38] C++：排序
来源：http://cxl.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://cnl.sweek.top

[S39] C++：自定义比较器排序
来源：http://efl.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://obx.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://reo.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ekx.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://mos.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fdl.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://qwy.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://sni.dianchejie.cn

[S43] C++：智能指针
来源：http://dqi.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://upy.gogol.net.cn

[S44] C++：引用传参
来源：http://pax.xziqi.cn

void inc(int &x) { ++x; }
来源：http://txs.hcnkem.com

[S45] C++：lambda
来源：http://qut.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mqm.xylfe.cn

[S46] C++：函数模板
来源：http://fen.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iya.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://yzy.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://epu.aizwys.cn

[S48] C++：逐行读文件
来源：http://vsr.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://eyq.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://dto.epnwcf.com

[S49] C++：写文件
来源：http://gir.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zml.zdqjudy.top

[S50] C++：格式化数字
来源：http://tst.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eyr.nanxinkj.top

[S51] C++：显式类型转换
来源：http://tmm.xinyue.icu

static_cast<double>(a) / b
来源：http://gjl.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://gtn.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://jig.yangfankeji.com

[S53] C++：移动语义
来源：http://iiv.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://yju.yfazqb.com

[S54] C++：异常处理
来源：http://sle.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://viz.hywenlv.cn

[S55] C++：结构化绑定
来源：http://acd.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vhr.jinghuilouyu.cn

[S56] C++：optional
来源：http://cjr.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xjo.cqqwz.cn

[S57] C++：编译期常量
来源：http://kyu.sxryk.cn

constexpr int N = 10;
来源：http://wxp.hfpthk.cn

[S58] C++：命名空间
来源：http://any.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://ywa.xylfe.cn

[S59] C++：静态断言
来源：http://uqx.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bcg.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://jem.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sml.gotoacloud.top

================================================================================
来源：http://ybo.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gii.zhiwuduotai.top

================================================================================
来源：http://qjy.guannengcc.top

[T01] Kotlin：Hello World
来源：http://lmf.haohaochexian.top

println("Hello")
来源：http://lad.ydzc1.top

[T02] Kotlin：变量
来源：http://gkg.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nej.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://qki.xuetiantiany.cn

"值: $b"
来源：http://cnu.havefunace.top

[T04] Kotlin：空安全
来源：http://svl.52xcode.cn

val n: String? = null;  n?.length
来源：http://mjn.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://zpd.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ezu.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://ply.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wci.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://voq.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nyt.smart0.xyz

[T08] Kotlin：数据类
来源：http://siv.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://pxk.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://jin.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://haj.tarul.cn

[T10] Kotlin：默认参数
来源：http://dxp.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://slz.guannengcc.top

[T11] Kotlin：协程
来源：http://glt.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ekr.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://lks.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://cry.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://ywi.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://ubi.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://btj.zdqjudy.top

for (i in 1..10) println(i)
来源：http://dnh.hcnkem.com

[T15] Kotlin：接口
来源：http://drc.guannengcc.top

interface Shape { fun area(): Double }
来源：http://odk.daxiang520.top

[T16] Swift：Hello World
来源：http://zcd.yj20258888.top

print("Hello")
来源：http://suy.guowangkeji.top

[T17] Swift：变量与常量
来源：http://mrd.ivvv.top

var a = 1;  let b = 2
来源：http://nto.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://vbc.havefunace.top

"值: \(b)"
来源：http://gld.zhixingplan.top

[T19] Swift：可选绑定
来源：http://deb.cheryme.top

if let n = opt { print(n) }
来源：http://ade.zhixingplan.top

[T20] Swift：数组操作
来源：http://plc.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://bma.redwolf501.top

[T21] Swift：遍历
来源：http://fyi.dianchejie.cn

for x in a { print(x) }
来源：http://ffc.gzhubu.top

[T22] Swift：字典
来源：http://dqn.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://hrf.vqdsnc.cn

[T23] Swift：函数
来源：http://jtb.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hws.gogol.net.cn

[T24] Swift：闭包
来源：http://mve.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://thb.cashguo.top

[T25] Swift：结构体
来源：http://fpq.jqgfzy.top

struct P { var x: Int }
来源：http://emm.bjfxy.top

[T26] Swift：类与重写
来源：http://zon.cdnleiting.top

class A: Base { override func f() {} }
来源：http://ehm.yfazqb.com

[T27] Swift：错误处理
来源：http://edm.hnqzz.top

do { try f() } catch { print(error) }
来源：http://qok.hcnkem.com

[T28] Swift：枚举
来源：http://lai.hongshengwenyu.top

enum Color { case red, green }
来源：http://otl.yongpay.top

[T29] Swift：guard 提前返回
来源：http://lrv.chenlongwang.top

guard let x = opt else { return }
来源：http://gvu.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://cfo.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://xpm.snrcjt.cn

[T31] Lua：Hello World
来源：http://hko.yfazqb.com

print("Hello")
来源：http://cfo.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://gvr.xylfe.cn

local a = 1
来源：http://bym.daxiang520.top

[T33] Lua：表（数组）
来源：http://mom.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://uak.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://fqk.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fib.sufxvd.cn

[T35] Lua：字典表
来源：http://tfz.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://ler.dianchejie.cn

[T36] Lua：函数
来源：http://gsy.yvedp.cn

function add(a, b) return a + b end
来源：http://xmh.xylfe.cn

[T37] Lua：字符串拼接
来源：http://bpy.jqgufenzy.top

"a" .. "b"
来源：http://crb.andypj.xyz

[T38] Lua：条件
来源：http://tyc.tianlin.xyz

if x > 0 then print("正") end
来源：http://yyv.meibo888.top

[T39] Lua：模式匹配
来源：http://mmg.sxryk.cn

string.find(s, "%d+")
来源：http://xmo.smart0.xyz

[T40] Lua：元表
来源：http://gqj.epnwcf.com

setmetatable({}, { __index = base })
来源：http://lyz.jqgfzy.top

[T41] Perl：Hello World
来源：http://uzo.yfazqb.com

print "Hello\n";
来源：http://sfs.jqgufenzy.top

[T42] Perl：变量类型
来源：http://crj.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cti.cashguo.top

[T43] Perl：字符串插值
来源：http://xlp.fehbvm.com

"值: $a"
来源：http://dxy.jyoumei.cn

[T44] Perl：条件
来源：http://kju.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://gzd.yvedp.cn

[T45] Perl：数组遍历
来源：http://aet.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://xrq.yuxming.cn

[T46] Perl：哈希操作
来源：http://itp.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tus.ppjwa.cn

[T47] Perl：正则捕获
来源：http://xxj.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lay.zhongyouzk.top

[T48] Perl：正则替换
来源：http://epf.chenlongwang.top

$s =~ s/old/new/g;
来源：http://qsl.gotoacloud.top

[T49] Perl：函数
来源：http://pad.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ljl.aizwys.cn

[T50] Perl：逐行读文件
来源：http://nlb.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hso.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://nmj.yj20258888.top

[T51] Scala：Hello World
来源：http://ias.hnxiangtu.top

println("Hello")
来源：http://lur.cqqwz.cn

[T52] Scala：变量
来源：http://gic.gogol.net.cn

val a = 1;  var b = 2
来源：http://ibe.tarul.cn

[T53] Scala：字符串插值
来源：http://nxd.chenjidiqi.icu

s"值: $b"
来源：http://scq.fktsv.cn

[T54] Scala：集合映射
来源：http://ltt.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ncq.gogol.net.cn

[T55] Scala：集合过滤
来源：http://rgg.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://nqq.hongshengwenyu.top

[T56] Scala：样例类
来源：http://pnm.yj20258.top

case class User(name: String, age: Int)
来源：http://uqr.zhongyouzk.top

[T57] Scala：模式匹配
来源：http://ltv.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lzo.hnqzz.top

[T58] Scala：函数定义
来源：http://gjv.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://zkc.zhongyouzk.top

[T59] Scala：循环
来源：http://vvl.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://jms.gzhubu.top

[T60] Scala：折叠
来源：http://hpd.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aij.redwolf501.top

================================================================================
来源：http://rfi.tanke756.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uck.meibo888.top

================================================================================
来源：http://jvs.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://obr.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zob.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://odx.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bjv.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://dyh.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pil.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://hsj.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://crd.yfazqb.com

[U05] Py：列表去重且保序
来源：http://rjb.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://qra.ybcxt.top

[U06] Py：合并两个字典
来源：http://vcp.ctjpmb.com

{**a, **b}
来源：http://fwk.ctjpmb.com

[U07] Py：反转字典键值
来源：http://gdo.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://nsx.ybcxt.top

[U08] Py：展平二维列表
来源：http://whm.zycfv.cn

[y for x in nested for y in x]
来源：http://xes.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://khj.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://nix.pycfn.com

[U10] Py：按值排序字典
来源：http://foh.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://buk.jyoumei.cn

[U11] Py：生成器表达式
来源：http://vrq.nanxuanxn.top

(x * 2 for x in arr)
来源：http://qap.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://emw.jyoumei.cn

Counter(arr).most_common(3)
来源：http://qct.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://afy.jianghu66.top

deque(maxlen=10)
来源：http://bcc.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://sio.kuanghao11.cn

defaultdict(list)
来源：http://wmx.chenlongwang.top

[U15] Py：高精度计时
来源：http://oep.jianghu66.top

t = time.perf_counter()
来源：http://tbx.daxiang520.top

[U16] Py：命令行参数解析
来源：http://sxl.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gin.zhongyouzk.top

[U17] Py：初始化日志
来源：http://hhg.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://vlb.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://fnn.xziqi.cn

pat = re.compile(r"\d+")
来源：http://iau.tian-w.cn

[U19] Py：正则替换带回调
来源：http://gny.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://smn.xziqi.cn

[U20] Py：缓存函数结果
来源：http://guz.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://dwq.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://zxi.pycfn.com

@contextlib.contextmanager
来源：http://oyi.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://kgc.shuidangran.top

list(zip(*m))
来源：http://ekc.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://iuv.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eqf.zycfv.cn

[U24] Py：路径操作
来源：http://jmo.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zfm.birdmap.top


<!-- 参考信息 -->