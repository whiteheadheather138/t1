代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://qhd.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://knj.zycfv.cn

fclose(f);
来源：http://zrz.shanyushiyangkeji.top

[S12] C：写文件
来源：http://wrc.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nvs.xylfe.cn

[S13] C：宏定义
来源：http://weg.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://odk.quarkkingdee.top

[S14] C：枚举
来源：http://bvj.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://cby.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://gkw.svipenyu.cn

(double) a / b
来源：http://ham.316326.xyz

[S16] C：位操作置位
来源：http://mts.hysaishi.cn

x |= (1 << 3);
来源：http://xai.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://ioo.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ded.daxiang520.top

[S18] C：命令行参数
来源：http://mhf.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://yvv.tarul.cn

[S19] C：快速排序
来源：http://arr.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tqr.tanke756.top

[S20] C：二分查找
来源：http://xuy.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mgp.mhx1999.top

[S21] C：字符类别判断
来源：http://rhz.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vyg.yuanzhike.top

[S22] C：字符串转数字
来源：http://dbx.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://ukz.jinqigufen.top

[S23] C：随机数
来源：http://irf.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aqs.hnqzz.top

[S24] C：获取本地时间
来源：http://otx.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pxu.ivvv.top

[S25] C：内存拷贝
来源：http://bjk.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://lvj.hfpthk.cn

[S26] C：内存清零
来源：http://bhk.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://rpr.yj20258888.top

[S27] C：定义常量
来源：http://ptn.zhongyouzk.top

const double PI = 3.14159;
来源：http://fbl.yj202588.top

[S28] C：静态变量
来源：http://bik.chenjidiqi.icu

static int counter = 0;
来源：http://mrk.mhx1999.top

[S29] C：变参函数
来源：http://jyi.pengpengdd.cyou

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xqz.jqgfzy.top

[S30] C：头文件保护
来源：http://exo.chenjidiqi.icu

#ifndef X_H
来源：http://gsl.kuanghao11.cn

#define X_H
来源：http://ghg.c1oappe.top

#endif
来源：http://oyp.pycfn.com

[S31] C++：Hello World
来源：http://dbs.mhx1999.top

#include <iostream>
来源：http://dtq.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://kxa.cdnleiting.top

[S32] C++：字符串
来源：http://xqw.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://lcp.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://cjh.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wms.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://mqk.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://nes.zhongyouzk.top

[S35] C++：map
来源：http://dht.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eoz.gzhubu.top

[S36] C++：unordered_map
来源：http://ypq.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hjp.haohaochexian.top

[S37] C++：set
来源：http://xal.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tnd.yj202588.top

[S38] C++：排序
来源：http://hwa.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://esl.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://hpm.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ymt.jyoumei.cn

[S40] C++：查找元素
来源：http://xax.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pjn.ppjwa.cn

[S41] C++：类与构造函数
来源：http://rie.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nvt.yfazqb.com

[S42] C++：继承与虚函数
来源：http://ujd.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://sjp.ppjwa.cn

[S43] C++：智能指针
来源：http://dbz.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://riw.fehbvm.com

[S44] C++：引用传参
来源：http://uif.wangdashe.top

void inc(int &x) { ++x; }
来源：http://xzi.sjlbkw.cn

[S45] C++：lambda
来源：http://pht.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://fci.gogol.net.cn

[S46] C++：函数模板
来源：http://kbw.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qhc.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://mvg.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://efp.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://giv.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://qll.epnwcf.com

while (std::getline(in, line)) { }
来源：http://htr.ydjk.org.cn

[S49] C++：写文件
来源：http://mxe.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wsr.zdbjq.cn

[S50] C++：格式化数字
来源：http://jyj.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qyu.shuidangran.top

[S51] C++：显式类型转换
来源：http://pkb.fehbvm.com

static_cast<double>(a) / b
来源：http://tzm.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://xkn.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://ttx.shangyingyoupin.top

[S53] C++：移动语义
来源：http://thz.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://cgb.nanxuanxn.top

[S54] C++：异常处理
来源：http://gfw.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mxh.ehwqpu.com

[S55] C++：结构化绑定
来源：http://rml.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wrj.jlsjyb.cn

[S56] C++：optional
来源：http://zve.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uqg.fktsv.cn

[S57] C++：编译期常量
来源：http://ken.xuetiantiany.cn

constexpr int N = 10;
来源：http://bms.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://vzb.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://hau.wangdashe.top

[S59] C++：静态断言
来源：http://yna.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jxl.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://wwz.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fqb.guannengcc.top

================================================================================
来源：http://lhf.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://beo.hcnkem.com

================================================================================
来源：http://gvs.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://hzp.hongshengwenyu.top

println("Hello")
来源：http://mzg.yuanzhike.top

[T02] Kotlin：变量
来源：http://lfk.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mvb.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://xow.c1oappe.top

"值: $b"
来源：http://wac.316326.xyz

[T04] Kotlin：空安全
来源：http://bwf.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://vkp.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://onr.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lnq.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://ros.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jyw.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://mea.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rii.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://wub.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://kqf.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://fuq.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://tlx.birdmap.top

[T10] Kotlin：默认参数
来源：http://ufs.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qoz.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://uxk.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cst.uphjek.com

[T12] Kotlin：解构声明
来源：http://qif.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://cpj.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://ikb.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://hpx.fzhhl.top

[T14] Kotlin：循环
来源：http://seg.jinqigufen.top

for (i in 1..10) println(i)
来源：http://djz.tianlin.xyz

[T15] Kotlin：接口
来源：http://hah.uphjek.com

interface Shape { fun area(): Double }
来源：http://rri.nwbrower.top

[T16] Swift：Hello World
来源：http://diq.zycfv.cn

print("Hello")
来源：http://prq.yfazqb.com

[T17] Swift：变量与常量
来源：http://twl.zhijiandao.cn

var a = 1;  let b = 2
来源：http://exx.fengsongda.top

[T18] Swift：字符串插值
来源：http://uat.epnwcf.com

"值: \(b)"
来源：http://xpy.jinqigufen.top

[T19] Swift：可选绑定
来源：http://ipc.svipenyu.cn

if let n = opt { print(n) }
来源：http://aie.52xcode.cn

[T20] Swift：数组操作
来源：http://uyu.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://aqc.xuetiantiany.cn

[T21] Swift：遍历
来源：http://txa.ppjwa.cn

for x in a { print(x) }
来源：http://eln.ivvv.top

[T22] Swift：字典
来源：http://mln.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://byn.hnxiangtu.top

[T23] Swift：函数
来源：http://ztg.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ser.cashguo.top

[T24] Swift：闭包
来源：http://jsh.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hrz.gzhubu.top

[T25] Swift：结构体
来源：http://dcq.xuetiantiany.cn

struct P { var x: Int }
来源：http://wmc.hnqzz.top

[T26] Swift：类与重写
来源：http://yyp.zhengqikj.top

class A: Base { override func f() {} }
来源：http://qzw.fehbvm.com

[T27] Swift：错误处理
来源：http://aqd.hammf.cn

do { try f() } catch { print(error) }
来源：http://vbh.hongshengwenyu.top

[T28] Swift：枚举
来源：http://qjx.pengpengdd.cyou

enum Color { case red, green }
来源：http://dod.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://axj.redwolf501.top

guard let x = opt else { return }
来源：http://pvt.bjfxy.top

[T30] Swift：协议
来源：http://qph.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://kgb.dashuyun.cn

[T31] Lua：Hello World
来源：http://qtq.andypj.xyz

print("Hello")
来源：http://uny.tarul.cn

[T32] Lua：局部变量
来源：http://htt.nanxuanxn.top

local a = 1
来源：http://bxw.gotoacloud.top

[T33] Lua：表（数组）
来源：http://upl.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vgk.52xcode.cn

[T34] Lua：遍历表
来源：http://ypa.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hgs.zdbjq.cn

[T35] Lua：字典表
来源：http://tcc.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://uze.yvedp.cn

[T36] Lua：函数
来源：http://jtf.chenlongwang.top

function add(a, b) return a + b end
来源：http://lax.tarul.cn

[T37] Lua：字符串拼接
来源：http://dvk.fanxiaobao.xyz

"a" .. "b"
来源：http://unc.cheryme.top

[T38] Lua：条件
来源：http://nxb.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://bed.yfazqb.com

[T39] Lua：模式匹配
来源：http://laz.hysaishi.cn

string.find(s, "%d+")
来源：http://vgu.hfpthk.cn

[T40] Lua：元表
来源：http://oar.cashguo.top

setmetatable({}, { __index = base })
来源：http://vgr.aizwys.cn

[T41] Perl：Hello World
来源：http://dsx.jinghuilouyu.cn

print "Hello\n";
来源：http://ida.meibo888.top

[T42] Perl：变量类型
来源：http://bue.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uhb.nanxinkj.top

[T43] Perl：字符串插值
来源：http://duz.hcnkem.com

"值: $a"
来源：http://dzs.shzxlz.cn

[T44] Perl：条件
来源：http://exi.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://uaz.fehbvm.com

[T45] Perl：数组遍历
来源：http://geh.cashguo.top

for my $x (@arr) { print $x; }
来源：http://zyz.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://kjf.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nic.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://jnu.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wwd.dianchejie.cn

[T48] Perl：正则替换
来源：http://jtr.cqqwz.cn

$s =~ s/old/new/g;
来源：http://grz.uphjek.com

[T49] Perl：函数
来源：http://ljc.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ejo.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://bcm.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qmh.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://tae.yuanzhike.top

[T51] Scala：Hello World
来源：http://jmj.zhoulong.xyz

println("Hello")
来源：http://azn.zhixingplan.top

[T52] Scala：变量
来源：http://vdm.hywenlv.cn

val a = 1;  var b = 2
来源：http://wcr.9152youxi.cn

[T53] Scala：字符串插值
来源：http://dsf.jianghu66.top

s"值: $b"
来源：http://hbz.gzhubu.top

[T54] Scala：集合映射
来源：http://ttb.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://utc.jqgfzy.top

[T55] Scala：集合过滤
来源：http://azu.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://uvg.shzxlz.cn

[T56] Scala：样例类
来源：http://hbl.sweek.top

case class User(name: String, age: Int)
来源：http://fmb.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://qql.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ooy.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://lkh.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://srd.yongpay.top

[T59] Scala：循环
来源：http://ldh.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://ddo.yonumen.top

[T60] Scala：折叠
来源：http://yrb.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cpg.birdmap.top

================================================================================
来源：http://vzq.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kjh.bjfxy.top

================================================================================
来源：http://alx.tarul.cn

[U01] Py：创建虚拟环境
来源：http://vsf.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://glr.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://hfr.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://imb.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://tka.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://pgv.wangdashe.top

[U04] Py：变量调试打印
来源：http://ahx.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qto.hnxiangtu.top

[U05] Py：列表去重且保序
来源：http://lww.guannengcc.top

list(dict.fromkeys(arr))
来源：http://qvn.andypj.xyz

[U06] Py：合并两个字典
来源：http://qhk.birdmap.top

{**a, **b}
来源：http://lag.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://qhl.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://grx.jianghu66.top

[U08] Py：展平二维列表
来源：http://iko.jqgfzy.top

[y for x in nested for y in x]
来源：http://tfk.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://wvz.ydjk.org.cn

max(d, key=d.get)
来源：http://jok.zhengqikj.top

[U10] Py：按值排序字典
来源：http://tww.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmf.sweek.top

[U11] Py：生成器表达式
来源：http://bln.snrcjt.cn

(x * 2 for x in arr)
来源：http://msk.xingfuxueyuan.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://xlu.cheryme.top

Counter(arr).most_common(3)
来源：http://tgx.gotoacloud.top

[U13] Py：固定长度队列
来源：http://yom.havefunace.top

deque(maxlen=10)
来源：http://nas.jianghu66.top

[U14] Py：分组收集到列表
来源：http://qma.jinqigfzy.top

defaultdict(list)
来源：http://dul.gzhubu.top

[U15] Py：高精度计时
来源：http://ktp.zhongyouzk.top

t = time.perf_counter()
来源：http://hvq.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://jwm.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gov.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://wgr.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://okm.daria6918.cn

[U18] Py：预编译正则
来源：http://rgj.uphjek.com

pat = re.compile(r"\d+")
来源：http://zaa.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://tjj.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xyb.316326.xyz

[U20] Py：缓存函数结果
来源：http://vmy.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://pot.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://miz.ctjpmb.com

@contextlib.contextmanager
来源：http://ttw.zhixingplan.top

[U22] Py：矩阵转置
来源：http://djd.hongshengwenyu.top

list(zip(*m))
来源：http://hvs.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://emt.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hoj.pengpengdd.cyou

[U24] Py：路径操作
来源：http://lyw.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dld.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://szw.zhijiandao.cn

csv.DictReader(f)
来源：http://uuw.birdmap.top

[U26] Py：并发下载
来源：http://bos.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oud.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://rvs.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://ktn.gaohongyu789.top

[U28] Py：类型别名
来源：http://pxb.ydjk.org.cn

UserId = int
来源：http://bhe.tianlin.xyz

[U29] Py：属性校验
来源：http://ajj.xinyue.icu

@property 与 @x.setter 配合
来源：http://rnx.kuanghao11.cn

[U30] Py：数据类
来源：http://ngn.havefunace.top

@dataclass(slots=True)
来源：http://goo.chenlongwang.top

[U31] Py：单测
来源：http://ssl.jianghu66.top

python -m pytest -q
来源：http://lmz.kuanghao11.cn

[U32] Py：代码格式化
来源：http://cgd.snrcjt.cn

ruff format . && ruff check --fix .
来源：http://rvf.birdmap.top

[U33] Py：打包发布
来源：http://vrz.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://zsh.cucudq.cn

[U34] Py：判断编码
来源：http://whg.wangdashe.top

chardet.detect(raw)
来源：http://qsa.gaohongyu789.top


<!-- 参考信息 -->