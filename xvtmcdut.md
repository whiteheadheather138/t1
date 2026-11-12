代发 wailian999

x |= (1 << 3);
来源：http://mbm.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://mtp.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lbg.pengpengdd.cyou

[S18] C：命令行参数
来源：http://lry.0kj1m.cn

int main(int argc, char **argv)
来源：http://hpg.cqqwz.cn

[S19] C：快速排序
来源：http://ooc.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xis.hysaishi.cn

[S20] C：二分查找
来源：http://ipw.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uoh.kuanghao11.cn

[S21] C：字符类别判断
来源：http://kop.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yif.tian-w.cn

[S22] C：字符串转数字
来源：http://wss.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vxn.chenzaomai.com

[S23] C：随机数
来源：http://xbf.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://unf.kuanghao11.cn

[S24] C：获取本地时间
来源：http://kcj.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xma.bjfxy.top

[S25] C：内存拷贝
来源：http://fqv.gotoacloud.top

memcpy(dst, src, n);
来源：http://bih.yj20258888.top

[S26] C：内存清零
来源：http://qsu.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://ddy.yj20258.top

[S27] C：定义常量
来源：http://etl.sysykeji.top

const double PI = 3.14159;
来源：http://ctd.tianlin.xyz

[S28] C：静态变量
来源：http://sgk.zycfv.cn

static int counter = 0;
来源：http://oqy.sufxvd.cn

[S29] C：变参函数
来源：http://xef.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vel.aizwys.cn

[S30] C：头文件保护
来源：http://rdx.daxiang520.top

#ifndef X_H
来源：http://pld.gzhubu.top

#define X_H
来源：http://axt.cqqwz.cn

#endif
来源：http://bti.jyoumei.cn

[S31] C++：Hello World
来源：http://dxe.bbcook.cn

#include <iostream>
来源：http://shi.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://tmp.uphjek.com

[S32] C++：字符串
来源：http://giz.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://cvo.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://doa.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bdr.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://gnx.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://mvn.zhixingplan.top

[S35] C++：map
来源：http://sqc.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jly.cucudq.cn

[S36] C++：unordered_map
来源：http://tuf.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ycz.pycfn.com

[S37] C++：set
来源：http://gef.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oqh.bjfxy.top

[S38] C++：排序
来源：http://zum.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://nyh.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://heo.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lrm.ydjk.org.cn

[S40] C++：查找元素
来源：http://lqm.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mox.chenzaomai.com

[S41] C++：类与构造函数
来源：http://jml.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fuj.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://fer.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://fuq.hesvh.cn

[S43] C++：智能指针
来源：http://ejz.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://siu.shuidangran.top

[S44] C++：引用传参
来源：http://jtn.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://siq.guannengcc.top

[S45] C++：lambda
来源：http://uzd.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://wpc.guannengcc.top

[S46] C++：函数模板
来源：http://keo.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lsr.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://him.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zll.bbcook.cn

[S48] C++：逐行读文件
来源：http://teh.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jud.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://qry.zdbjq.cn

[S49] C++：写文件
来源：http://vco.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljw.kuanghao11.cn

[S50] C++：格式化数字
来源：http://dmv.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ewq.shzxlz.cn

[S51] C++：显式类型转换
来源：http://miv.xylfe.cn

static_cast<double>(a) / b
来源：http://bzp.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://lvc.hnqzz.top

int size() const noexcept { return n_; }
来源：http://ojg.vehdjk.com

[S53] C++：移动语义
来源：http://qrh.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://dnn.sjlbkw.cn

[S54] C++：异常处理
来源：http://wcc.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gfq.ehwqpu.com

[S55] C++：结构化绑定
来源：http://vlx.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jgf.daxiang520.top

[S56] C++：optional
来源：http://xaj.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tab.yfazqb.com

[S57] C++：编译期常量
来源：http://hne.aibaodan.cn

constexpr int N = 10;
来源：http://okr.ydjk.org.cn

[S58] C++：命名空间
来源：http://egm.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://hta.yangfankeji.com

[S59] C++：静态断言
来源：http://btf.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mla.hammf.cn

[S60] C++：遍历并删除元素
来源：http://bjx.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nub.cqqwz.cn

================================================================================
来源：http://clt.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljx.dashuyun.cn

================================================================================
来源：http://mhj.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://fbs.gotoacloud.top

println("Hello")
来源：http://qic.ybcxt.top

[T02] Kotlin：变量
来源：http://jal.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ozc.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://kna.cheryme.top

"值: $b"
来源：http://maa.svipenyu.cn

[T04] Kotlin：空安全
来源：http://lve.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://zoz.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://hgl.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://txf.sweek.top

[T06] Kotlin：集合映射
来源：http://irx.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ahy.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://agr.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://mus.cashguo.top

[T08] Kotlin：数据类
来源：http://zqt.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://bfp.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://ocn.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://huj.aizwys.cn

[T10] Kotlin：默认参数
来源：http://xja.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://sho.aizwys.cn

[T11] Kotlin：协程
来源：http://kyb.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://okf.xinyue.icu

[T12] Kotlin：解构声明
来源：http://guf.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://nqw.sweek.top

[T13] Kotlin：只读 Map
来源：http://uen.xinyue.icu

val m = mapOf("a" to 1)
来源：http://epx.dashuyun.cn

[T14] Kotlin：循环
来源：http://vdh.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://qac.jinqigfzy.top

[T15] Kotlin：接口
来源：http://fen.bjfxy.top

interface Shape { fun area(): Double }
来源：http://lkp.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://mod.yuanzhike.top

print("Hello")
来源：http://tuv.hysaishi.cn

[T17] Swift：变量与常量
来源：http://dhy.hfpthk.cn

var a = 1;  let b = 2
来源：http://uri.redwolf501.top

[T18] Swift：字符串插值
来源：http://jjo.jqgufenzy.top

"值: \(b)"
来源：http://ypj.nwbrower.top

[T19] Swift：可选绑定
来源：http://mfc.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://kag.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://uqj.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qmy.hammf.cn

[T21] Swift：遍历
来源：http://lyi.zhoulong.xyz

for x in a { print(x) }
来源：http://pzs.jinqigfzy.top

[T22] Swift：字典
来源：http://rds.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://tiz.jinqigufen.top

[T23] Swift：函数
来源：http://avk.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://emf.redwolf501.top

[T24] Swift：闭包
来源：http://pju.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lip.shangyingyoupin.top

[T25] Swift：结构体
来源：http://pin.chenjidiqi.icu

struct P { var x: Int }
来源：http://knn.cheryme.top

[T26] Swift：类与重写
来源：http://bjx.ppjwa.cn

class A: Base { override func f() {} }
来源：http://gew.jiagoushi.top

[T27] Swift：错误处理
来源：http://vxa.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://izk.hongshengwenyu.top

[T28] Swift：枚举
来源：http://kmo.jinghuilouyu.cn

enum Color { case red, green }
来源：http://hxg.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://yrb.nanxinkj.top

guard let x = opt else { return }
来源：http://upf.jinghuilouyu.cn

[T30] Swift：协议
来源：http://idi.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://mqv.xylfe.cn

[T31] Lua：Hello World
来源：http://olk.ehwqpu.com

print("Hello")
来源：http://lzi.jqgufenzy.top

[T32] Lua：局部变量
来源：http://oby.cdnleiting.top

local a = 1
来源：http://bby.tianlin.xyz

[T33] Lua：表（数组）
来源：http://nmo.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://qqp.fengsongda.top

[T34] Lua：遍历表
来源：http://njs.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tth.yj20258888.top

[T35] Lua：字典表
来源：http://xmw.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://nwo.hongshengwenyu.top

[T36] Lua：函数
来源：http://ygs.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://ffi.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://oej.shanyushiyangkeji.top

"a" .. "b"
来源：http://obm.xuetiantiany.cn

[T38] Lua：条件
来源：http://qhv.svipenyu.cn

if x > 0 then print("正") end
来源：http://plw.sweek.top

[T39] Lua：模式匹配
来源：http://rjh.yuanzhike.top

string.find(s, "%d+")
来源：http://dqs.shzxlz.cn

[T40] Lua：元表
来源：http://xsm.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://bvw.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://klj.316326.xyz

print "Hello\n";
来源：http://cns.ydjk.org.cn

[T42] Perl：变量类型
来源：http://tdi.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ion.hysaishi.cn

[T43] Perl：字符串插值
来源：http://jwt.chenzaomai.com

"值: $a"
来源：http://rts.fanxiaobao.xyz

[T44] Perl：条件
来源：http://hqn.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://mzb.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://xuh.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://jfm.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://ufm.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ewd.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://ixf.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hhp.snrcjt.cn

[T48] Perl：正则替换
来源：http://sxm.wangdashe.top

$s =~ s/old/new/g;
来源：http://onc.feifeiyinyue.top

[T49] Perl：函数
来源：http://szd.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lsm.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://wfm.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qzs.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://iku.hnqzz.top

[T51] Scala：Hello World
来源：http://rcg.cucudq.cn

println("Hello")
来源：http://kzk.yfazqb.com

[T52] Scala：变量
来源：http://pfp.gogol.net.cn

val a = 1;  var b = 2
来源：http://nzf.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://szv.ctjpmb.com

s"值: $b"
来源：http://jcp.sysykeji.top

[T54] Scala：集合映射
来源：http://xlq.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://ffm.fehbvm.com

[T55] Scala：集合过滤
来源：http://pwj.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bev.aizwys.cn

[T56] Scala：样例类
来源：http://qmy.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://dhi.ivvv.top

[T57] Scala：模式匹配
来源：http://cqn.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mhp.pycfn.com

[T58] Scala：函数定义
来源：http://rwf.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://uso.jqgfzy.top

[T59] Scala：循环
来源：http://icp.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://rcc.snrcjt.cn

[T60] Scala：折叠
来源：http://yra.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hoo.fengsongda.top

================================================================================
来源：http://phi.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tyz.fzhhl.top

================================================================================
来源：http://xky.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://bdc.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zma.zhaomingkeji.xyz

[U02] Py：导出 / 安装依赖
来源：http://vjb.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://quu.yonumen.top

[U03] Py：加载 .env 配置
来源：http://ihf.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wfx.shuidangran.top

[U04] Py：变量调试打印
来源：http://zli.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rnc.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://nxy.nwbrower.top

list(dict.fromkeys(arr))
来源：http://hbk.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://rkg.jianghu66.top

{**a, **b}
来源：http://gzd.hnqzz.top

[U07] Py：反转字典键值
来源：http://vui.sxryk.cn

{v: k for k, v in d.items()}
来源：http://crt.yj20258888.top

[U08] Py：展平二维列表
来源：http://yci.guowangkeji.top

[y for x in nested for y in x]
来源：http://zbv.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://cvf.nanxuanxn.top

max(d, key=d.get)
来源：http://uqw.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://fpa.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mes.ybcxt.top

[U11] Py：生成器表达式
来源：http://sdp.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://yqz.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://idd.daxiang520.top

Counter(arr).most_common(3)
来源：http://dgj.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://fcf.gaohongyu789.top

deque(maxlen=10)
来源：http://bjy.xylfe.cn

[U14] Py：分组收集到列表
来源：http://kmx.iojbl.cn

defaultdict(list)
来源：http://wfi.svipenyu.cn

[U15] Py：高精度计时
来源：http://vap.cdnleiting.top

t = time.perf_counter()
来源：http://ama.bbcook.cn

[U16] Py：命令行参数解析
来源：http://yiz.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://llc.nanxinkj.top

[U17] Py：初始化日志
来源：http://lcd.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://eeg.nanxinkj.top

[U18] Py：预编译正则
来源：http://kbo.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://aja.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://kdh.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xnm.ydzc1.top

[U20] Py：缓存函数结果
来源：http://jfj.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://gqw.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://jbk.hywenlv.cn

@contextlib.contextmanager
来源：http://ndm.ydzc1.top

[U22] Py：矩阵转置
来源：http://lup.hywenlv.cn

list(zip(*m))
来源：http://tlm.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://ekq.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://soz.sysykeji.top

[U24] Py：路径操作
来源：http://dzd.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lyv.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://iba.hnxiangtu.top

csv.DictReader(f)
来源：http://kzz.chenzaomai.com

[U26] Py：并发下载
来源：http://olh.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ppg.uphjek.com

[U27] Py：异步 HTTP
来源：http://ogw.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://bdj.9152youxi.cn

[U28] Py：类型别名
来源：http://bko.feifeiyinyue.top

UserId = int
来源：http://ypp.yj20258.top

[U29] Py：属性校验
来源：http://mtu.guowangkeji.top

@property 与 @x.setter 配合
来源：http://kfw.chenlongwang.top

[U30] Py：数据类
来源：http://clq.sjlbkw.cn

@dataclass(slots=True)
来源：http://jdf.shangyingyoupin.top

[U31] Py：单测
来源：http://sxi.cqqwz.cn

python -m pytest -q
来源：http://swe.yanxiufei.cn

[U32] Py：代码格式化
来源：http://xjf.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://zxy.yj202588.top

[U33] Py：打包发布
来源：http://jsa.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://fjn.gogol.net.cn

[U34] Py：判断编码
来源：http://una.yj202588.top

chardet.detect(raw)
来源：http://vit.chenzaomai.com

[U35] Py：发送邮件
来源：http://tvt.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xfe.tian-w.cn

[U36] Py：定时任务
来源：http://bbv.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://pnl.guowangkeji.top

[U37] Py：读写 Excel
来源：http://dfa.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yhh.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://uja.mhx1999.top

Path(__file__).resolve().parent
来源：http://zlt.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://oed.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://tjv.yj202588.top

[U40] Py：打印到标准错误
来源：http://acu.cheryme.top

print("err", file=sys.stderr)
来源：http://jaz.shangyingyoupin.top


<!-- 参考信息 -->