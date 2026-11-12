代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://gzu.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qjj.52xcode.cn

fclose(f);
来源：http://hau.shangyingyoupin.top

[S12] C：写文件
来源：http://hyy.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kfp.c1oappe.top

[S13] C：宏定义
来源：http://xuj.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yir.sufxvd.cn

[S14] C：枚举
来源：http://rlr.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://sgr.sufxvd.cn

[S15] C：类型转换
来源：http://ahl.shangyingyoupin.top

(double) a / b
来源：http://rxn.pengpengdd.cyou

[S16] C：位操作置位
来源：http://gxe.jiagoushi.top

x |= (1 << 3);
来源：http://loq.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://cji.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qdo.chenjidiqi.icu

[S18] C：命令行参数
来源：http://iou.hnxiangtu.top

int main(int argc, char **argv)
来源：http://bsb.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://ikh.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lar.ybcxt.top

[S20] C：二分查找
来源：http://ubq.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gky.bbcook.cn

[S21] C：字符类别判断
来源：http://wlo.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vac.uphjek.com

[S22] C：字符串转数字
来源：http://xgu.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://xft.birdmap.top

[S23] C：随机数
来源：http://bxs.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sfz.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://zzd.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iwo.yfazqb.com

[S25] C：内存拷贝
来源：http://rbk.iojbl.cn

memcpy(dst, src, n);
来源：http://noq.vqdsnc.cn

[S26] C：内存清零
来源：http://jhz.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://tmq.xziqi.cn

[S27] C：定义常量
来源：http://mdk.hfpthk.cn

const double PI = 3.14159;
来源：http://cuc.nanxuanxn.top

[S28] C：静态变量
来源：http://ytu.jinyuanbaomall.cn

static int counter = 0;
来源：http://agv.ydjk.org.cn

[S29] C：变参函数
来源：http://ret.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hrz.yongpay.top

[S30] C：头文件保护
来源：http://nht.nanxinkj.top

#ifndef X_H
来源：http://zhp.dashuyun.cn

#define X_H
来源：http://geu.mhx1999.top

#endif
来源：http://kws.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://fpm.nanxinkj.top

#include <iostream>
来源：http://oth.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://vlu.daria6918.cn

[S32] C++：字符串
来源：http://lhd.ivvv.top

std::string s = "hi";  s += "!";
来源：http://nrz.ehwqpu.com

[S33] C++：vector 增删
来源：http://sqd.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dzm.yj202588.top

[S34] C++：遍历 vector
来源：http://tvg.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://fuk.sweek.top

[S35] C++：map
来源：http://xxy.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kwy.kuanghao11.cn

[S36] C++：unordered_map
来源：http://flw.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahn.bjfxy.top

[S37] C++：set
来源：http://lws.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ygl.hongshengwenyu.top

[S38] C++：排序
来源：http://bdm.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://cyl.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://cab.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kms.hfpthk.cn

[S40] C++：查找元素
来源：http://umu.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jrr.bbcook.cn

[S41] C++：类与构造函数
来源：http://fpo.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ezz.cucudq.cn

[S42] C++：继承与虚函数
来源：http://kem.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://pqr.iojbl.cn

[S43] C++：智能指针
来源：http://ace.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://nmg.bbcook.cn

[S44] C++：引用传参
来源：http://hhs.316326.xyz

void inc(int &x) { ++x; }
来源：http://hhe.kuanghao11.cn

[S45] C++：lambda
来源：http://umf.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://pjr.nanxinkj.top

[S46] C++：函数模板
来源：http://rxc.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zwd.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://phg.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wab.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://fbk.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://wei.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://ojl.ehwqpu.com

[S49] C++：写文件
来源：http://uss.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lkl.cdnleiting.top

[S50] C++：格式化数字
来源：http://ovc.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bhs.zdbjq.cn

[S51] C++：显式类型转换
来源：http://nju.xinyue.icu

static_cast<double>(a) / b
来源：http://dvx.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://lcj.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://uxq.gotoacloud.top

[S53] C++：移动语义
来源：http://qnm.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://vdw.hongshengwenyu.top

[S54] C++：异常处理
来源：http://efn.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fih.ppjwa.cn

[S55] C++：结构化绑定
来源：http://zbk.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oad.xuetiantiany.cn

[S56] C++：optional
来源：http://yeu.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pza.hywenlv.cn

[S57] C++：编译期常量
来源：http://xmc.zhoulong.xyz

constexpr int N = 10;
来源：http://jyc.ydzc1.top

[S58] C++：命名空间
来源：http://tej.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://dom.zycfv.cn

[S59] C++：静态断言
来源：http://rbm.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yuf.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://xqe.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lbf.nanxinkj.top

================================================================================
来源：http://kun.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pox.daxiang520.top

================================================================================
来源：http://rzl.316326.xyz

[T01] Kotlin：Hello World
来源：http://mkh.vqdsnc.cn

println("Hello")
来源：http://jvl.shuidangran.top

[T02] Kotlin：变量
来源：http://vtv.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ele.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://ust.zhongyouzk.top

"值: $b"
来源：http://jzx.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://gdt.yangfankeji.com

val n: String? = null;  n?.length
来源：http://hta.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://eed.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://atw.meibo888.top

[T06] Kotlin：集合映射
来源：http://try.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vyc.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://ycv.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://uds.guowangkeji.top

[T08] Kotlin：数据类
来源：http://quw.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://eoj.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://vnx.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://bft.pycfn.com

[T10] Kotlin：默认参数
来源：http://dpg.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yik.ybcxt.top

[T11] Kotlin：协程
来源：http://tbb.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dcn.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://gvl.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://rut.sweek.top

[T13] Kotlin：只读 Map
来源：http://tlf.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://cjv.fehbvm.com

[T14] Kotlin：循环
来源：http://ijn.tarul.cn

for (i in 1..10) println(i)
来源：http://lcs.epnwcf.com

[T15] Kotlin：接口
来源：http://znh.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://urx.guowangkeji.top

[T16] Swift：Hello World
来源：http://mhr.guannengcc.top

print("Hello")
来源：http://hur.guannengcc.top

[T17] Swift：变量与常量
来源：http://fcb.hesvh.cn

var a = 1;  let b = 2
来源：http://iqu.cqqwz.cn

[T18] Swift：字符串插值
来源：http://akd.yuxming.cn

"值: \(b)"
来源：http://jqh.guannengcc.top

[T19] Swift：可选绑定
来源：http://bcn.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://jmp.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://upz.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yyq.pycfn.com

[T21] Swift：遍历
来源：http://kkt.0kj1m.cn

for x in a { print(x) }
来源：http://uca.cqqwz.cn

[T22] Swift：字典
来源：http://jlk.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ott.yvedp.cn

[T23] Swift：函数
来源：http://vbi.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gxx.cqqwz.cn

[T24] Swift：闭包
来源：http://lsc.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wyh.hnqzz.top

[T25] Swift：结构体
来源：http://uqg.gogol.net.cn

struct P { var x: Int }
来源：http://wey.ydjk.org.cn

[T26] Swift：类与重写
来源：http://djf.hammf.cn

class A: Base { override func f() {} }
来源：http://gsm.sjlbkw.cn

[T27] Swift：错误处理
来源：http://dkh.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://wkf.hesvh.cn

[T28] Swift：枚举
来源：http://kzm.zhijiandao.cn

enum Color { case red, green }
来源：http://ahp.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://elm.andypj.xyz

guard let x = opt else { return }
来源：http://suq.hnqzz.top

[T30] Swift：协议
来源：http://tot.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://xuu.hywenlv.cn

[T31] Lua：Hello World
来源：http://zlp.hongshengwenyu.top

print("Hello")
来源：http://gnk.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://ntl.316326.xyz

local a = 1
来源：http://ajw.hammf.cn

[T33] Lua：表（数组）
来源：http://erh.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cth.jinqigufen.top

[T34] Lua：遍历表
来源：http://zmh.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://blb.hongshengwenyu.top

[T35] Lua：字典表
来源：http://dqd.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://cpg.snrcjt.cn

[T36] Lua：函数
来源：http://tgf.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://nad.shuidangran.top

[T37] Lua：字符串拼接
来源：http://utr.hywenlv.cn

"a" .. "b"
来源：http://kxu.cqqwz.cn

[T38] Lua：条件
来源：http://ygj.ehwqpu.com

if x > 0 then print("正") end
来源：http://dnt.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://kte.hcnkem.com

string.find(s, "%d+")
来源：http://bff.svipenyu.cn

[T40] Lua：元表
来源：http://kmy.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://kzy.cucudq.cn

[T41] Perl：Hello World
来源：http://wxa.zhiwuduotai.top

print "Hello\n";
来源：http://hmy.daxiang520.top

[T42] Perl：变量类型
来源：http://moe.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uwi.bjfxy.top

[T43] Perl：字符串插值
来源：http://jwb.ydzc1.top

"值: $a"
来源：http://flj.meibo888.top

[T44] Perl：条件
来源：http://tsg.sweek.top

if ($a > 0) { print "正"; }
来源：http://htk.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://hbw.xuetiantiany.cn

for my $x (@arr) { print $x; }
来源：http://pmi.snrcjt.cn

[T46] Perl：哈希操作
来源：http://zqa.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://prj.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://sqc.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://hkh.andypj.xyz

[T48] Perl：正则替换
来源：http://nws.chenlongwang.top

$s =~ s/old/new/g;
来源：http://zkg.shzxlz.cn

[T49] Perl：函数
来源：http://ybz.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uub.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://zfn.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xfe.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://wtl.9152youxi.cn

[T51] Scala：Hello World
来源：http://yof.ppjwa.cn

println("Hello")
来源：http://iyd.xuanzx.com

[T52] Scala：变量
来源：http://nfx.epnwcf.com

val a = 1;  var b = 2
来源：http://huy.tarul.cn

[T53] Scala：字符串插值
来源：http://lbv.hywenlv.cn

s"值: $b"
来源：http://xcz.yj20258.top

[T54] Scala：集合映射
来源：http://nvl.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://pkc.yueranfly.top

[T55] Scala：集合过滤
来源：http://koi.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://kau.jianghu66.top

[T56] Scala：样例类
来源：http://zmn.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://xlu.gotoacloud.top

[T57] Scala：模式匹配
来源：http://wca.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hfg.fzhhl.top

[T58] Scala：函数定义
来源：http://pnh.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://jqy.andypj.xyz

[T59] Scala：循环
来源：http://fgm.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://lhm.0kj1m.cn

[T60] Scala：折叠
来源：http://ols.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qjv.daxiang520.top

================================================================================
来源：http://lfj.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mof.gaohongyu789.top

================================================================================
来源：http://rdk.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://krq.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lgr.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://lbn.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://npo.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://kzs.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://voz.cashguo.top

[U04] Py：变量调试打印
来源：http://ozg.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xan.guannengcc.top

[U05] Py：列表去重且保序
来源：http://qaf.cheryme.top

list(dict.fromkeys(arr))
来源：http://vae.uphjek.com

[U06] Py：合并两个字典
来源：http://asm.bbcook.cn

{**a, **b}
来源：http://gmo.ctjpmb.com

[U07] Py：反转字典键值
来源：http://gqb.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://ykz.chenzaomai.com

[U08] Py：展平二维列表
来源：http://wwv.uphjek.com

[y for x in nested for y in x]
来源：http://rna.yj20258.top

[U09] Py：字典取最大值的键
来源：http://ova.ctjpmb.com

max(d, key=d.get)
来源：http://irz.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://rwy.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yvf.c1oappe.top

[U11] Py：生成器表达式
来源：http://iyl.shuidangran.top

(x * 2 for x in arr)
来源：http://xjz.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://tom.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://age.ehwqpu.com

[U13] Py：固定长度队列
来源：http://nso.nwbrower.top

deque(maxlen=10)
来源：http://rpi.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://egy.fzhhl.top

defaultdict(list)
来源：http://ctn.tarul.cn

[U15] Py：高精度计时
来源：http://hjg.jinqigfzy.top

t = time.perf_counter()
来源：http://vgx.xylfe.cn

[U16] Py：命令行参数解析
来源：http://ewt.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://btt.jiagoushi.top

[U17] Py：初始化日志
来源：http://tjr.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://sih.sysykeji.top

[U18] Py：预编译正则
来源：http://pky.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://zhm.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://vdh.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fxi.hcnkem.com

[U20] Py：缓存函数结果
来源：http://tta.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://iub.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://otx.sjlbkw.cn

@contextlib.contextmanager
来源：http://lmj.meibo888.top

[U22] Py：矩阵转置
来源：http://ewx.cdnleiting.top

list(zip(*m))
来源：http://pkc.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://hla.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fda.tian-w.cn

[U24] Py：路径操作
来源：http://bmu.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gxx.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://atd.yueranfly.top

csv.DictReader(f)
来源：http://puv.daxiang520.top

[U26] Py：并发下载
来源：http://voc.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cup.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://lvl.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://gjp.yvedp.cn

[U28] Py：类型别名
来源：http://krf.fengsongda.top

UserId = int
来源：http://ncg.cdnleiting.top

[U29] Py：属性校验
来源：http://bzy.ctjpmb.com

@property 与 @x.setter 配合
来源：http://duk.jqgfzy.top

[U30] Py：数据类
来源：http://svg.hcnkem.com

@dataclass(slots=True)
来源：http://gra.sxryk.cn

[U31] Py：单测
来源：http://ltt.shuidangran.top

python -m pytest -q
来源：http://dsl.yuxming.cn

[U32] Py：代码格式化
来源：http://bov.jianghu66.top

ruff format . && ruff check --fix .
来源：http://jfl.yuanzhike.top

[U33] Py：打包发布
来源：http://ukf.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://tts.c1oappe.top

[U34] Py：判断编码
来源：http://ink.quarkkingdee.top

chardet.detect(raw)
来源：http://xla.xziqi.cn


<!-- 参考信息 -->