代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://jrp.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ytz.zhiwuduotai.top

fclose(f);
来源：http://kfw.yuxming.cn

[S12] C：写文件
来源：http://svc.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://onh.uphjek.com

[S13] C：宏定义
来源：http://omv.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lzz.ydzc1.top

[S14] C：枚举
来源：http://cfc.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://krt.jlsjyb.cn

[S15] C：类型转换
来源：http://top.shuidangran.top

(double) a / b
来源：http://qtu.hongshengwenyu.top

[S16] C：位操作置位
来源：http://rwq.yj20258.top

x |= (1 << 3);
来源：http://irp.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://gdy.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tzm.redwolf501.top

[S18] C：命令行参数
来源：http://jaw.ctjpmb.com

int main(int argc, char **argv)
来源：http://mtm.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://bif.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aaw.yj20258.top

[S20] C：二分查找
来源：http://tpl.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxd.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://asz.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dut.iojbl.cn

[S22] C：字符串转数字
来源：http://jtt.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://uvh.gotoacloud.top

[S23] C：随机数
来源：http://dpb.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qqh.yj20258888.top

[S24] C：获取本地时间
来源：http://znx.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kmn.hcnkem.com

[S25] C：内存拷贝
来源：http://cvy.daria6918.cn

memcpy(dst, src, n);
来源：http://opg.ehwqpu.com

[S26] C：内存清零
来源：http://dxq.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://wux.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://phw.ehwqpu.com

const double PI = 3.14159;
来源：http://cev.cheryme.top

[S28] C：静态变量
来源：http://qjc.cashguo.top

static int counter = 0;
来源：http://nps.xylfe.cn

[S29] C：变参函数
来源：http://fgg.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://myn.yvedp.cn

[S30] C：头文件保护
来源：http://pei.hysaishi.cn

#ifndef X_H
来源：http://aet.cucudq.cn

#define X_H
来源：http://tdq.jiagoushi.top

#endif
来源：http://qpv.bbcook.cn

[S31] C++：Hello World
来源：http://fca.ppjwa.cn

#include <iostream>
来源：http://aqx.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://xra.yj20258.top

[S32] C++：字符串
来源：http://voi.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://tzg.fktsv.cn

[S33] C++：vector 增删
来源：http://lbg.fzhhl.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wqs.tanke756.top

[S34] C++：遍历 vector
来源：http://dhn.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://byq.bjfxy.top

[S35] C++：map
来源：http://nzk.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zdp.yangfankeji.com

[S36] C++：unordered_map
来源：http://wvh.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://opt.sjlbkw.cn

[S37] C++：set
来源：http://aez.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wfo.pengpengdd.cyou

[S38] C++：排序
来源：http://vld.ivvv.top

std::sort(v.begin(), v.end());
来源：http://huj.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://vzc.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fiu.yvedp.cn

[S40] C++：查找元素
来源：http://xpo.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://loh.zhixingplan.top

[S41] C++：类与构造函数
来源：http://vay.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://csr.fengsongda.top

[S42] C++：继承与虚函数
来源：http://tsw.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://tkg.gogol.net.cn

[S43] C++：智能指针
来源：http://wqf.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://ktb.yuanzhike.top

[S44] C++：引用传参
来源：http://byr.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://oym.yueranfly.top

[S45] C++：lambda
来源：http://sqs.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://mbt.shanyushiyangtech.top

[S46] C++：函数模板
来源：http://xjv.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sld.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://uth.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xfk.fengsongda.top

[S48] C++：逐行读文件
来源：http://slc.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://uct.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://min.sweek.top

[S49] C++：写文件
来源：http://dkn.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qyv.uphjek.com

[S50] C++：格式化数字
来源：http://icl.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eod.shzxlz.cn

[S51] C++：显式类型转换
来源：http://sup.yanxiufei.cn

static_cast<double>(a) / b
来源：http://obh.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://jom.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://diu.havefunace.top

[S53] C++：移动语义
来源：http://gzp.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://gor.hesvh.cn

[S54] C++：异常处理
来源：http://jft.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rdy.hesvh.cn

[S55] C++：结构化绑定
来源：http://ihg.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cip.chenjidiqi.icu

[S56] C++：optional
来源：http://qfz.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://esq.ctjpmb.com

[S57] C++：编译期常量
来源：http://olg.ydzc1.top

constexpr int N = 10;
来源：http://czu.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://avw.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://udw.sxryk.cn

[S59] C++：静态断言
来源：http://zwl.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://htj.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://qem.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://drq.yj20258888.top

================================================================================
来源：http://xxi.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rhu.gotoacloud.top

================================================================================
来源：http://sxn.yuxming.cn

[T01] Kotlin：Hello World
来源：http://ubi.fanxiaobao.xyz

println("Hello")
来源：http://spd.daria6918.cn

[T02] Kotlin：变量
来源：http://bpo.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ioh.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://emn.jqgfzy.top

"值: $b"
来源：http://vmb.fktsv.cn

[T04] Kotlin：空安全
来源：http://etv.yuxming.cn

val n: String? = null;  n?.length
来源：http://dym.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://zqj.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wch.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://onw.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://qfs.uphjek.com

[T07] Kotlin：集合过滤
来源：http://ivw.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uke.daria6918.cn

[T08] Kotlin：数据类
来源：http://tcb.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://jtp.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://ilp.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://nne.fktsv.cn

[T10] Kotlin：默认参数
来源：http://rpa.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vxo.havefunace.top

[T11] Kotlin：协程
来源：http://pug.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bkz.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://jdf.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://kil.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://yor.sweek.top

val m = mapOf("a" to 1)
来源：http://jwh.yj202588.top

[T14] Kotlin：循环
来源：http://nwv.sufxvd.cn

for (i in 1..10) println(i)
来源：http://rck.ydzc1.top

[T15] Kotlin：接口
来源：http://zwc.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://duy.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://pee.hongshengwenyu.top

print("Hello")
来源：http://ome.yangfankeji.com

[T17] Swift：变量与常量
来源：http://fwy.tianlin.xyz

var a = 1;  let b = 2
来源：http://bry.epnwcf.com

[T18] Swift：字符串插值
来源：http://znb.9152youxi.cn

"值: \(b)"
来源：http://ogm.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://stg.epnwcf.com

if let n = opt { print(n) }
来源：http://ieu.fzhhl.top

[T20] Swift：数组操作
来源：http://qtc.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://tcx.yvedp.cn

[T21] Swift：遍历
来源：http://jxl.iojbl.cn

for x in a { print(x) }
来源：http://uqx.hnqzz.top

[T22] Swift：字典
来源：http://mod.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://jpe.bbcook.cn

[T23] Swift：函数
来源：http://dbx.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kib.uphjek.com

[T24] Swift：闭包
来源：http://ils.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xcq.daria6918.cn

[T25] Swift：结构体
来源：http://tsu.zhoulong.xyz

struct P { var x: Int }
来源：http://qja.hesvh.cn

[T26] Swift：类与重写
来源：http://vio.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://amh.nwbrower.top

[T27] Swift：错误处理
来源：http://dij.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://ron.bjfxy.top

[T28] Swift：枚举
来源：http://php.ydzc1.top

enum Color { case red, green }
来源：http://aqq.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://qht.zhoulong.xyz

guard let x = opt else { return }
来源：http://dzt.kuanghao11.cn

[T30] Swift：协议
来源：http://nxt.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://euq.vehdjk.com

[T31] Lua：Hello World
来源：http://hof.mhx1999.top

print("Hello")
来源：http://ips.hfpthk.cn

[T32] Lua：局部变量
来源：http://gxb.smart0.xyz

local a = 1
来源：http://jzc.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://uxu.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://joc.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://oke.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xpo.zhixingplan.top

[T35] Lua：字典表
来源：http://jqv.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://pdg.guannengcc.top

[T36] Lua：函数
来源：http://gcd.hysaishi.cn

function add(a, b) return a + b end
来源：http://rzm.guannengcc.top

[T37] Lua：字符串拼接
来源：http://qac.jqgufenzy.top

"a" .. "b"
来源：http://fgq.aibaodan.cn

[T38] Lua：条件
来源：http://vxt.andypj.xyz

if x > 0 then print("正") end
来源：http://wsm.hesvh.cn

[T39] Lua：模式匹配
来源：http://eil.yangfankeji.com

string.find(s, "%d+")
来源：http://mrx.yuanzhike.top

[T40] Lua：元表
来源：http://hnv.gzhubu.top

setmetatable({}, { __index = base })
来源：http://wbq.xuanzx.com

[T41] Perl：Hello World
来源：http://gqx.zycfv.cn

print "Hello\n";
来源：http://njl.nanxuanxn.top

[T42] Perl：变量类型
来源：http://drf.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jap.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://bzq.redwolf501.top

"值: $a"
来源：http://tyg.ppjwa.cn

[T44] Perl：条件
来源：http://tgt.meibo888.top

if ($a > 0) { print "正"; }
来源：http://ozu.yj20258888.top

[T45] Perl：数组遍历
来源：http://hdd.tanke756.top

for my $x (@arr) { print $x; }
来源：http://ggs.9152youxi.cn

[T46] Perl：哈希操作
来源：http://xnd.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kbo.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://gnr.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://svy.jinqigfzy.top

[T48] Perl：正则替换
来源：http://sfq.smart0.xyz

$s =~ s/old/new/g;
来源：http://ito.meibo888.top

[T49] Perl：函数
来源：http://ula.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fkc.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://xoz.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xzf.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://jbs.yj202588.top

[T51] Scala：Hello World
来源：http://fki.yj20258888.top

println("Hello")
来源：http://zli.cucudq.cn

[T52] Scala：变量
来源：http://hth.aibaodan.cn

val a = 1;  var b = 2
来源：http://uht.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://qvd.gaohongyu789.top

s"值: $b"
来源：http://oft.nanxinkj.top

[T54] Scala：集合映射
来源：http://gna.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://nqd.9152youxi.cn

[T55] Scala：集合过滤
来源：http://imn.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://iqf.zhengqikj.top

[T56] Scala：样例类
来源：http://jii.pycfn.com

case class User(name: String, age: Int)
来源：http://whh.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://ufy.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pbw.zycfv.cn

[T58] Scala：函数定义
来源：http://mqk.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://wva.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://aug.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://nrt.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://hxa.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jex.fengsongda.top

================================================================================
来源：http://cbw.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dkk.svipenyu.cn

================================================================================
来源：http://qze.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://yqf.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://llk.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://rfx.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://afo.zycfv.cn

[U03] Py：加载 .env 配置
来源：http://dwi.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://awa.xinyue.icu

[U04] Py：变量调试打印
来源：http://vkn.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xuq.cashguo.top

[U05] Py：列表去重且保序
来源：http://fof.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://vzm.tanke756.top

[U06] Py：合并两个字典
来源：http://fvc.xziqi.cn

{**a, **b}
来源：http://lse.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://etk.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://iro.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://umi.jinqigufen.top

[y for x in nested for y in x]
来源：http://qxr.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://xbz.chenzaomai.com

max(d, key=d.get)
来源：http://bin.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://utt.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lww.vehdjk.com

[U11] Py：生成器表达式
来源：http://vzs.hnxiangtu.top

(x * 2 for x in arr)
来源：http://skw.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ebv.havefunace.top

Counter(arr).most_common(3)
来源：http://fkr.wangdashe.top

[U13] Py：固定长度队列
来源：http://qew.wangshuangyany.cn

deque(maxlen=10)
来源：http://uvd.bjfxy.top

[U14] Py：分组收集到列表
来源：http://eow.hfpthk.cn

defaultdict(list)
来源：http://dnt.shuidangran.top

[U15] Py：高精度计时
来源：http://uhy.hesvh.cn

t = time.perf_counter()
来源：http://nld.hammf.cn

[U16] Py：命令行参数解析
来源：http://zmk.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://coe.yvedp.cn

[U17] Py：初始化日志
来源：http://hdz.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://nip.guannengcc.top

[U18] Py：预编译正则
来源：http://okr.sysykeji.top

pat = re.compile(r"\d+")
来源：http://tdj.aizwys.cn

[U19] Py：正则替换带回调
来源：http://cqe.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://klt.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://som.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://dyd.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://kjh.smart0.xyz

@contextlib.contextmanager
来源：http://bpp.hnqzz.top

[U22] Py：矩阵转置
来源：http://pec.vqdsnc.cn

list(zip(*m))
来源：http://cgo.aizwys.cn

[U23] Py：分块读取大文件
来源：http://kxb.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gwa.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://iki.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://agu.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://utk.yueranfly.top

csv.DictReader(f)
来源：http://zbc.zhixingplan.top

[U26] Py：并发下载
来源：http://wax.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tkc.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://jhc.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://fgc.gaohongyu789.top

[U28] Py：类型别名
来源：http://jhr.yanxiufei.cn

UserId = int
来源：http://bll.ydzc1.top

[U29] Py：属性校验
来源：http://hfh.aibaodan.cn

@property 与 @x.setter 配合
来源：http://urc.sweek.top

[U30] Py：数据类
来源：http://sxb.xziqi.cn

@dataclass(slots=True)
来源：http://zlh.jinqigfzy.top

[U31] Py：单测
来源：http://auf.zhijiandao.cn

python -m pytest -q
来源：http://bde.jinqigufen.top

[U32] Py：代码格式化
来源：http://joo.aizwys.cn

ruff format . && ruff check --fix .
来源：http://ruu.gaohongyu789.top

[U33] Py：打包发布
来源：http://lif.sjlbkw.cn

python -m build  （依赖 pyproject.toml）
来源：http://ohr.ehwqpu.com

[U34] Py：判断编码
来源：http://dvi.shanyushiyangtech.top

chardet.detect(raw)
来源：http://rge.chenlongwang.top


<!-- 参考信息 -->