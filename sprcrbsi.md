代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://fpl.sufxvd.cn

[S15] C：类型转换
来源：http://bry.fanxiaobao.xyz

(double) a / b
来源：http://wbu.yj20258.top

[S16] C：位操作置位
来源：http://bxb.cucudq.cn

x |= (1 << 3);
来源：http://kfu.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://lni.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egl.hesvh.cn

[S18] C：命令行参数
来源：http://wng.fengsongda.top

int main(int argc, char **argv)
来源：http://rns.nanxuanxn.top

[S19] C：快速排序
来源：http://wvj.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://hxo.ivvv.top

[S20] C：二分查找
来源：http://qyd.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ddu.hnqzz.top

[S21] C：字符类别判断
来源：http://okm.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ien.zhixingplan.top

[S22] C：字符串转数字
来源：http://qhj.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://uck.redwolf501.top

[S23] C：随机数
来源：http://cmt.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xhi.daria6918.cn

[S24] C：获取本地时间
来源：http://tbm.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://scm.gogol.net.cn

[S25] C：内存拷贝
来源：http://iqu.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://jvv.sufxvd.cn

[S26] C：内存清零
来源：http://jgw.fengsongda.top

memset(a, 0, sizeof a);
来源：http://oen.hnxiangtu.top

[S27] C：定义常量
来源：http://yxd.bjfxy.top

const double PI = 3.14159;
来源：http://fxi.zdqjudy.top

[S28] C：静态变量
来源：http://ajh.yj20258.top

static int counter = 0;
来源：http://ylv.wangdashe.top

[S29] C：变参函数
来源：http://fbv.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qeq.yangfankeji.com

[S30] C：头文件保护
来源：http://sfm.ehwqpu.com

#ifndef X_H
来源：http://nsy.shanyushiyangtech.top

#define X_H
来源：http://ffm.wangdashe.top

#endif
来源：http://hkj.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://iwt.jlsjyb.cn

#include <iostream>
来源：http://aoj.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://sxh.sysykeji.top

[S32] C++：字符串
来源：http://jfo.birdmap.top

std::string s = "hi";  s += "!";
来源：http://brk.kuanghao11.cn

[S33] C++：vector 增删
来源：http://gbx.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qrw.fzhhl.top

[S34] C++：遍历 vector
来源：http://kip.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://xjo.nwbrower.top

[S35] C++：map
来源：http://snl.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gtw.shzxlz.cn

[S36] C++：unordered_map
来源：http://sfm.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nyo.bbcook.cn

[S37] C++：set
来源：http://cui.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ucf.wangshuangyany.cn

[S38] C++：排序
来源：http://ndw.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://rqr.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://qqt.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xrf.nanxuanxn.top

[S40] C++：查找元素
来源：http://xuk.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dmp.smart0.xyz

[S41] C++：类与构造函数
来源：http://zei.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cgx.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://cba.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://chn.wangdashe.top

[S43] C++：智能指针
来源：http://gzv.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://ych.ehwqpu.com

[S44] C++：引用传参
来源：http://odc.zycfv.cn

void inc(int &x) { ++x; }
来源：http://xaq.sysykeji.top

[S45] C++：lambda
来源：http://ift.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://rdl.snrcjt.cn

[S46] C++：函数模板
来源：http://uir.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://you.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://cdp.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aly.cheryme.top

[S48] C++：逐行读文件
来源：http://zno.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://uvm.fehbvm.com

while (std::getline(in, line)) { }
来源：http://iuu.fzhhl.top

[S49] C++：写文件
来源：http://van.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zmb.pycfn.com

[S50] C++：格式化数字
来源：http://qsh.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://psg.hnqzz.top

[S51] C++：显式类型转换
来源：http://jlv.hnxiangtu.top

static_cast<double>(a) / b
来源：http://giz.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://buy.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://fwj.jiagoushi.top

[S53] C++：移动语义
来源：http://vpq.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://yxj.guowangkeji.top

[S54] C++：异常处理
来源：http://ryy.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lbn.guowangkeji.top

[S55] C++：结构化绑定
来源：http://ojm.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://skg.ppjwa.cn

[S56] C++：optional
来源：http://elp.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dpj.pycfn.com

[S57] C++：编译期常量
来源：http://nux.jinghuilouyu.cn

constexpr int N = 10;
来源：http://deq.yuxming.cn

[S58] C++：命名空间
来源：http://skw.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://lvg.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://zjb.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mpk.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://usi.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tzx.epnwcf.com

================================================================================
来源：http://njb.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hoh.hysaishi.cn

================================================================================
来源：http://eth.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://jgk.316326.xyz

println("Hello")
来源：http://eww.zdqjudy.top

[T02] Kotlin：变量
来源：http://kuz.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xhn.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://pgb.yfazqb.com

"值: $b"
来源：http://cuw.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://pux.ehwqpu.com

val n: String? = null;  n?.length
来源：http://ndt.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://phe.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://isx.ybcxt.top

[T06] Kotlin：集合映射
来源：http://hxu.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://owp.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://zif.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bal.chenlongwang.top

[T08] Kotlin：数据类
来源：http://yee.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://tmh.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://btf.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://lau.cashguo.top

[T10] Kotlin：默认参数
来源：http://pbn.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rcr.haohaochexian.top

[T11] Kotlin：协程
来源：http://jeh.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gms.bbcook.cn

[T12] Kotlin：解构声明
来源：http://ups.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://idv.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://cpo.fktsv.cn

val m = mapOf("a" to 1)
来源：http://aok.yj20258888.top

[T14] Kotlin：循环
来源：http://wus.hysaishi.cn

for (i in 1..10) println(i)
来源：http://vzh.daxiang520.top

[T15] Kotlin：接口
来源：http://dfh.wangdashe.top

interface Shape { fun area(): Double }
来源：http://ogq.tian-w.cn

[T16] Swift：Hello World
来源：http://aaj.shangyingyoupin.top

print("Hello")
来源：http://otq.tarul.cn

[T17] Swift：变量与常量
来源：http://zum.ctjpmb.com

var a = 1;  let b = 2
来源：http://hxn.cdnleiting.top

[T18] Swift：字符串插值
来源：http://hcm.hnqzz.top

"值: \(b)"
来源：http://xsw.jinqigufen.top

[T19] Swift：可选绑定
来源：http://bmv.yonumen.top

if let n = opt { print(n) }
来源：http://tef.cheryme.top

[T20] Swift：数组操作
来源：http://sgw.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gtj.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://wvx.yfazqb.com

for x in a { print(x) }
来源：http://dtg.c1oappe.top

[T22] Swift：字典
来源：http://ecm.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ccc.vehdjk.com

[T23] Swift：函数
来源：http://wge.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wgc.cashguo.top

[T24] Swift：闭包
来源：http://roo.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://adm.sjlbkw.cn

[T25] Swift：结构体
来源：http://gsn.yongpay.top

struct P { var x: Int }
来源：http://jge.chenjidiqi.icu

[T26] Swift：类与重写
来源：http://hsb.meibo888.top

class A: Base { override func f() {} }
来源：http://yil.zycfv.cn

[T27] Swift：错误处理
来源：http://msu.birdmap.top

do { try f() } catch { print(error) }
来源：http://bvo.jlsjyb.cn

[T28] Swift：枚举
来源：http://sbk.yuanzhike.top

enum Color { case red, green }
来源：http://acc.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://zxu.haohaochexian.top

guard let x = opt else { return }
来源：http://oqt.sufxvd.cn

[T30] Swift：协议
来源：http://qxs.pycfn.com

protocol Shape { func area() -> Double }
来源：http://slj.aizwys.cn

[T31] Lua：Hello World
来源：http://twm.jinyuanbaomall.cn

print("Hello")
来源：http://cmf.epnwcf.com

[T32] Lua：局部变量
来源：http://cmd.zhixingplan.top

local a = 1
来源：http://xec.hammf.cn

[T33] Lua：表（数组）
来源：http://atu.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://suf.vqdsnc.cn

[T34] Lua：遍历表
来源：http://qqo.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mze.shzxlz.cn

[T35] Lua：字典表
来源：http://ujm.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://pji.xziqi.cn

[T36] Lua：函数
来源：http://ynl.cashguo.top

function add(a, b) return a + b end
来源：http://ggr.cheryme.top

[T37] Lua：字符串拼接
来源：http://mcz.jiagoushi.top

"a" .. "b"
来源：http://swq.52xcode.cn

[T38] Lua：条件
来源：http://xap.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://vrk.hammf.cn

[T39] Lua：模式匹配
来源：http://wnf.zdqjudy.top

string.find(s, "%d+")
来源：http://pcm.316326.xyz

[T40] Lua：元表
来源：http://gge.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://iqc.zdbjq.cn

[T41] Perl：Hello World
来源：http://fei.aibaodan.cn

print "Hello\n";
来源：http://enw.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://gqv.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qte.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://rno.dashuyun.cn

"值: $a"
来源：http://dba.fzhhl.top

[T44] Perl：条件
来源：http://tee.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://awl.vehdjk.com

[T45] Perl：数组遍历
来源：http://uwv.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://gpx.jinqigufen.top

[T46] Perl：哈希操作
来源：http://bii.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zzz.ppjwa.cn

[T47] Perl：正则捕获
来源：http://rua.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://btd.fktsv.cn

[T48] Perl：正则替换
来源：http://xwm.epnwcf.com

$s =~ s/old/new/g;
来源：http://rff.hysaishi.cn

[T49] Perl：函数
来源：http://bna.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://elw.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://bkn.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kxu.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://vbc.daxiang520.top

[T51] Scala：Hello World
来源：http://uzq.guannengcc.top

println("Hello")
来源：http://euh.nwbrower.top

[T52] Scala：变量
来源：http://lmo.jlsjyb.cn

val a = 1;  var b = 2
来源：http://dej.ybcxt.top

[T53] Scala：字符串插值
来源：http://pxw.meibo888.top

s"值: $b"
来源：http://kim.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://qbr.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://mmc.nanxinkj.top

[T55] Scala：集合过滤
来源：http://rrp.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://cgx.svipenyu.cn

[T56] Scala：样例类
来源：http://mrl.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://cpr.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://bup.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnu.dianchejie.cn

[T58] Scala：函数定义
来源：http://ktn.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yah.sysykeji.top

[T59] Scala：循环
来源：http://dhv.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://hxu.sufxvd.cn

[T60] Scala：折叠
来源：http://prz.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nlo.uphjek.com

================================================================================
来源：http://tmi.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://job.guowangkeji.top

================================================================================
来源：http://cek.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://ojx.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://yym.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://pwg.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wsq.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://ozp.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yhv.wangdashe.top

[U04] Py：变量调试打印
来源：http://dqs.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pbs.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://hku.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://few.nanxinkj.top

[U06] Py：合并两个字典
来源：http://mhq.xinyue.icu

{**a, **b}
来源：http://gft.sweek.top

[U07] Py：反转字典键值
来源：http://mbj.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://toi.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://ldz.fehbvm.com

[y for x in nested for y in x]
来源：http://anh.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://zac.yuxming.cn

max(d, key=d.get)
来源：http://rrh.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://sto.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://udk.yuanzhike.top

[U11] Py：生成器表达式
来源：http://viw.ydjk.org.cn

(x * 2 for x in arr)
来源：http://rqg.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://bly.sxryk.cn

Counter(arr).most_common(3)
来源：http://eyx.cheryme.top

[U13] Py：固定长度队列
来源：http://bqo.hysaishi.cn

deque(maxlen=10)
来源：http://uxg.fehbvm.com

[U14] Py：分组收集到列表
来源：http://zva.guowangkeji.top

defaultdict(list)
来源：http://oxg.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://jzx.nanxuanxn.top

t = time.perf_counter()
来源：http://nfr.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://dfp.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mrg.ydzc1.top

[U17] Py：初始化日志
来源：http://xeg.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://zna.chenlongwang.top

[U18] Py：预编译正则
来源：http://zrw.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://hpe.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://nev.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gmp.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://wff.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://lsx.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://fpq.yongpay.top

@contextlib.contextmanager
来源：http://nhr.mhx1999.top

[U22] Py：矩阵转置
来源：http://fxf.hnqzz.top

list(zip(*m))
来源：http://qxg.iojbl.cn

[U23] Py：分块读取大文件
来源：http://pim.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jyd.yanxiufei.cn

[U24] Py：路径操作
来源：http://owb.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nns.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://rue.gogol.net.cn

csv.DictReader(f)
来源：http://jnk.ydzc1.top

[U26] Py：并发下载
来源：http://zxr.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nsg.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://cfi.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://ahx.wangdashe.top

[U28] Py：类型别名
来源：http://mhy.hongshengwenyu.top

UserId = int
来源：http://wah.meibo888.top

[U29] Py：属性校验
来源：http://hdb.gogol.net.cn

@property 与 @x.setter 配合
来源：http://bbr.xziqi.cn

[U30] Py：数据类
来源：http://wag.wangshuangyany.cn

@dataclass(slots=True)
来源：http://tad.zhiwuduotai.top

[U31] Py：单测
来源：http://irr.xuetiantiany.cn

python -m pytest -q
来源：http://win.dashuyun.cn

[U32] Py：代码格式化
来源：http://aac.cucudq.cn

ruff format . && ruff check --fix .
来源：http://fal.redwolf501.top

[U33] Py：打包发布
来源：http://wfy.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://ymq.epnwcf.com

[U34] Py：判断编码
来源：http://xil.nanxinkj.top

chardet.detect(raw)
来源：http://qox.pycfn.com

[U35] Py：发送邮件
来源：http://iqo.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://php.zhengqikj.top

[U36] Py：定时任务
来源：http://aru.zycfv.cn

schedule.every(10).minutes.do(job)
来源：http://roq.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://rqi.epnwcf.com

pandas.read_excel / DataFrame.to_excel
来源：http://zne.jinghuilouyu.cn

[U38] Py：获取脚本所在目录
来源：http://qcb.zhengqikj.top

Path(__file__).resolve().parent
来源：http://xto.xuanzx.com


<!-- 参考信息 -->