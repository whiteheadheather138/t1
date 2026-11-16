代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://qeh.zycfv.cn

[S15] C：类型转换
来源：http://qti.chenzaomai.com

(double) a / b
来源：http://fle.meibo888.top

[S16] C：位操作置位
来源：http://nxe.zhixingplan.top

x |= (1 << 3);
来源：http://mwc.ivvv.top

[S17] C：安全拼接字符串
来源：http://tqc.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sji.dashuyun.cn

[S18] C：命令行参数
来源：http://woy.aizwys.cn

int main(int argc, char **argv)
来源：http://ics.zhijiandao.cn

[S19] C：快速排序
来源：http://isi.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ncl.yangfankeji.com

[S20] C：二分查找
来源：http://nxy.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ucy.yfazqb.com

[S21] C：字符类别判断
来源：http://oea.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kig.yangfankeji.com

[S22] C：字符串转数字
来源：http://ckd.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://abw.wangshuangyany.cn

[S23] C：随机数
来源：http://uzx.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qhf.yonumen.top

[S24] C：获取本地时间
来源：http://reo.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vtg.vqdsnc.cn

[S25] C：内存拷贝
来源：http://ndy.zhoulong.xyz

memcpy(dst, src, n);
来源：http://qbs.jianghu66.top

[S26] C：内存清零
来源：http://yks.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://nkz.ehwqpu.com

[S27] C：定义常量
来源：http://ddr.chenjidiqi.icu

const double PI = 3.14159;
来源：http://vzx.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://kjx.zdbjq.cn

static int counter = 0;
来源：http://gap.sufxvd.cn

[S29] C：变参函数
来源：http://ubn.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dzd.fehbvm.com

[S30] C：头文件保护
来源：http://lud.jinqigfzy.top

#ifndef X_H
来源：http://xgv.daxiang520.top

#define X_H
来源：http://are.ywan-chungtsiang.top

#endif
来源：http://ldv.gzhubu.top

[S31] C++：Hello World
来源：http://wiz.xuetiantiany.cn

#include <iostream>
来源：http://jfa.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://zwk.yj20258.top

[S32] C++：字符串
来源：http://akv.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://xqj.birdmap.top

[S33] C++：vector 增删
来源：http://rac.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lje.cdnleiting.top

[S34] C++：遍历 vector
来源：http://ggr.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://oja.xinyue.icu

[S35] C++：map
来源：http://chf.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ybg.yj20258.top

[S36] C++：unordered_map
来源：http://jld.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uis.xuanzx.com

[S37] C++：set
来源：http://pis.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zgm.guowangkeji.top

[S38] C++：排序
来源：http://wsv.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://mij.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://aav.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cts.yongpay.top

[S40] C++：查找元素
来源：http://nze.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ydh.cucudq.cn

[S41] C++：类与构造函数
来源：http://yuw.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://biq.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://ckm.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://pgn.gaohongyu789.top

[S43] C++：智能指针
来源：http://vmm.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://fys.zhijiandao.cn

[S44] C++：引用传参
来源：http://utd.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://cgf.zhixingplan.top

[S45] C++：lambda
来源：http://ahe.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uda.dashuyun.cn

[S46] C++：函数模板
来源：http://kix.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://khr.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://pfa.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dkt.yj202588.top

[S48] C++：逐行读文件
来源：http://cnr.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://cdc.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://rws.haohaochexian.top

[S49] C++：写文件
来源：http://uus.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iip.yfazqb.com

[S50] C++：格式化数字
来源：http://juq.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fvk.epnwcf.com

[S51] C++：显式类型转换
来源：http://axl.mhx1999.top

static_cast<double>(a) / b
来源：http://nfo.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://nsy.daria6918.cn

int size() const noexcept { return n_; }
来源：http://zrj.nwbrower.top

[S53] C++：移动语义
来源：http://fzh.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://enh.chenlongwang.top

[S54] C++：异常处理
来源：http://igc.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nel.yuxming.cn

[S55] C++：结构化绑定
来源：http://yds.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zph.zdbjq.cn

[S56] C++：optional
来源：http://uwy.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dnz.sufxvd.cn

[S57] C++：编译期常量
来源：http://ehq.yuanzhike.top

constexpr int N = 10;
来源：http://ffr.jqgufenzy.top

[S58] C++：命名空间
来源：http://rha.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://szg.iojbl.cn

[S59] C++：静态断言
来源：http://pcf.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://onv.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://qbd.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmi.vehdjk.com

================================================================================
来源：http://sdg.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fai.daria6918.cn

================================================================================
来源：http://lsi.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://afk.hongshengwenyu.top

println("Hello")
来源：http://hnh.9152youxi.cn

[T02] Kotlin：变量
来源：http://grm.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fiv.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://wxu.dashuyun.cn

"值: $b"
来源：http://ils.gotoacloud.top

[T04] Kotlin：空安全
来源：http://vij.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://kci.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://rqh.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pil.yueranfly.top

[T06] Kotlin：集合映射
来源：http://jio.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://qzv.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://nbt.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pqg.iojbl.cn

[T08] Kotlin：数据类
来源：http://uvx.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://vjy.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://tnu.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://bdm.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://kxy.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jjg.gaohongyu789.top

[T11] Kotlin：协程
来源：http://fib.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xob.tian-w.cn

[T12] Kotlin：解构声明
来源：http://poy.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://nhj.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://ovu.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://bbf.epnwcf.com

[T14] Kotlin：循环
来源：http://gdj.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://ujo.vqdsnc.cn

[T15] Kotlin：接口
来源：http://qvs.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://lsh.hesvh.cn

[T16] Swift：Hello World
来源：http://kxh.316326.xyz

print("Hello")
来源：http://mib.meibo888.top

[T17] Swift：变量与常量
来源：http://wqc.jqgfzy.top

var a = 1;  let b = 2
来源：http://tri.feifeiyinyue.top

[T18] Swift：字符串插值
来源：http://lmm.shanyushiyangkeji.top

"值: \(b)"
来源：http://zez.hysaishi.cn

[T19] Swift：可选绑定
来源：http://orb.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://lof.wangdashe.top

[T20] Swift：数组操作
来源：http://iol.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://vxy.zhijiandao.cn

[T21] Swift：遍历
来源：http://amz.tianlin.xyz

for x in a { print(x) }
来源：http://wsx.chenlongwang.top

[T22] Swift：字典
来源：http://pec.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://vbm.sjlbkw.cn

[T23] Swift：函数
来源：http://uma.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://svc.jqgufenzy.top

[T24] Swift：闭包
来源：http://kyl.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://phk.hcnkem.com

[T25] Swift：结构体
来源：http://dxo.birdmap.top

struct P { var x: Int }
来源：http://fbu.hnxiangtu.top

[T26] Swift：类与重写
来源：http://nfr.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://klc.mhx1999.top

[T27] Swift：错误处理
来源：http://qpw.daxiang520.top

do { try f() } catch { print(error) }
来源：http://wrz.cheryme.top

[T28] Swift：枚举
来源：http://mre.chenjidiqi.icu

enum Color { case red, green }
来源：http://qfq.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://ljv.daria6918.cn

guard let x = opt else { return }
来源：http://vvy.hnxiangtu.top

[T30] Swift：协议
来源：http://jok.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://ehq.snrcjt.cn

[T31] Lua：Hello World
来源：http://vuj.pycfn.com

print("Hello")
来源：http://hfo.zycfv.cn

[T32] Lua：局部变量
来源：http://wlx.cashguo.top

local a = 1
来源：http://aop.ybcxt.top

[T33] Lua：表（数组）
来源：http://rbe.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dof.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://uws.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cyf.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://jzi.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://yyg.tianlin.xyz

[T36] Lua：函数
来源：http://tbj.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://tli.epnwcf.com

[T37] Lua：字符串拼接
来源：http://pxc.fehbvm.com

"a" .. "b"
来源：http://xbf.jiagoushi.top

[T38] Lua：条件
来源：http://hdt.vqdsnc.cn

if x > 0 then print("正") end
来源：http://kul.yuxming.cn

[T39] Lua：模式匹配
来源：http://rea.yuanzhike.top

string.find(s, "%d+")
来源：http://zzc.yj202588.top

[T40] Lua：元表
来源：http://oxi.bbcook.cn

setmetatable({}, { __index = base })
来源：http://qcz.ctjpmb.com

[T41] Perl：Hello World
来源：http://xrn.ivvv.top

print "Hello\n";
来源：http://uxz.ppjwa.cn

[T42] Perl：变量类型
来源：http://heb.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqy.hysaishi.cn

[T43] Perl：字符串插值
来源：http://xuq.nanxinkj.top

"值: $a"
来源：http://uug.shanyushiyangtech.top

[T44] Perl：条件
来源：http://lin.havefunace.top

if ($a > 0) { print "正"; }
来源：http://ulo.cdnleiting.top

[T45] Perl：数组遍历
来源：http://npq.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://nsm.tian-w.cn

[T46] Perl：哈希操作
来源：http://jgp.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mfl.yj202588.top

[T47] Perl：正则捕获
来源：http://czu.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://nui.xylfe.cn

[T48] Perl：正则替换
来源：http://fhu.aizwys.cn

$s =~ s/old/new/g;
来源：http://mnx.jlsjyb.cn

[T49] Perl：函数
来源：http://qdq.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tsy.mhx1999.top

[T50] Perl：逐行读文件
来源：http://lok.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://nug.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://jwt.hammf.cn

[T51] Scala：Hello World
来源：http://kne.dianchejie.cn

println("Hello")
来源：http://lua.nanxinkj.top

[T52] Scala：变量
来源：http://npf.0kj1m.cn

val a = 1;  var b = 2
来源：http://ttz.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://zbp.sysykeji.top

s"值: $b"
来源：http://mrl.zycfv.cn

[T54] Scala：集合映射
来源：http://qhm.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://obt.snrcjt.cn

[T55] Scala：集合过滤
来源：http://waz.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://wbz.gogol.net.cn

[T56] Scala：样例类
来源：http://gjk.tanke756.top

case class User(name: String, age: Int)
来源：http://baw.hywenlv.cn

[T57] Scala：模式匹配
来源：http://ldf.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://snt.redwolf501.top

[T58] Scala：函数定义
来源：http://mej.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://owg.guannengcc.top

[T59] Scala：循环
来源：http://ubq.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://uhd.epnwcf.com

[T60] Scala：折叠
来源：http://zjc.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yxv.jianghu66.top

================================================================================
来源：http://wdi.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vyw.ybcxt.top

================================================================================
来源：http://xdn.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://bji.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zjw.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://obu.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jqp.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://cby.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wem.snrcjt.cn

[U04] Py：变量调试打印
来源：http://wuv.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jlv.feifeiyinyue.top

[U05] Py：列表去重且保序
来源：http://vos.yongpay.top

list(dict.fromkeys(arr))
来源：http://eoe.vehdjk.com

[U06] Py：合并两个字典
来源：http://vbo.ivvv.top

{**a, **b}
来源：http://kuy.andypj.xyz

[U07] Py：反转字典键值
来源：http://xie.cdnleiting.top

{v: k for k, v in d.items()}
来源：http://kzp.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://avr.shanyushiyangtech.top

[y for x in nested for y in x]
来源：http://zxe.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://plr.yuxming.cn

max(d, key=d.get)
来源：http://ovj.ctjpmb.com

[U10] Py：按值排序字典
来源：http://qyb.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qnv.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://pgh.zdbjq.cn

(x * 2 for x in arr)
来源：http://emk.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lsv.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://czu.cashguo.top

[U13] Py：固定长度队列
来源：http://ywh.zhoulong.xyz

deque(maxlen=10)
来源：http://cvo.sweek.top

[U14] Py：分组收集到列表
来源：http://zdv.cqqwz.cn

defaultdict(list)
来源：http://bss.hcnkem.com

[U15] Py：高精度计时
来源：http://pqb.smart0.xyz

t = time.perf_counter()
来源：http://uwd.jianghu66.top

[U16] Py：命令行参数解析
来源：http://skn.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zfy.quarkkingdee.top

[U17] Py：初始化日志
来源：http://ksw.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://rlz.pycfn.com

[U18] Py：预编译正则
来源：http://vtf.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://tpq.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://ooi.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qhj.hcnkem.com

[U20] Py：缓存函数结果
来源：http://gdj.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://idx.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://jsa.yongpay.top

@contextlib.contextmanager
来源：http://tgf.zdqjudy.top

[U22] Py：矩阵转置
来源：http://ilh.guowangkeji.top

list(zip(*m))
来源：http://iux.jianghu66.top

[U23] Py：分块读取大文件
来源：http://fut.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nog.hywenlv.cn

[U24] Py：路径操作
来源：http://qyu.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ebd.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://tlq.ivvv.top

csv.DictReader(f)
来源：http://tpr.zhengqikj.top

[U26] Py：并发下载
来源：http://dlx.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mvp.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://pvg.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://nyv.shuidangran.top

[U28] Py：类型别名
来源：http://ydn.ydzc1.top

UserId = int
来源：http://ssk.jinqigufen.top

[U29] Py：属性校验
来源：http://onf.xingfuxueyuan.xyz

@property 与 @x.setter 配合
来源：http://tak.ehwqpu.com

[U30] Py：数据类
来源：http://jks.zhiwuduotai.top

@dataclass(slots=True)
来源：http://yvf.bjfxy.top

[U31] Py：单测
来源：http://hec.zdbjq.cn

python -m pytest -q
来源：http://tpo.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://dzv.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://wes.xylfe.cn

[U33] Py：打包发布
来源：http://nob.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://jpn.kuanghao11.cn

[U34] Py：判断编码
来源：http://tbg.zhengqikj.top

chardet.detect(raw)
来源：http://gqn.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://oad.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://htr.daxiang520.top

[U36] Py：定时任务
来源：http://nmo.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://bkq.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://hfp.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://ejp.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://pgk.sysykeji.top

Path(__file__).resolve().parent
来源：http://qsn.ivvv.top


<!-- 参考信息 -->