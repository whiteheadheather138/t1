代发 wailian999

x |= (1 << 3);
来源：http://ezn.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://dsa.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xbc.bjfxy.top

[S18] C：命令行参数
来源：http://cbc.nanxinkj.top

int main(int argc, char **argv)
来源：http://exd.aizwys.cn

[S19] C：快速排序
来源：http://xuu.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vzh.sufxvd.cn

[S20] C：二分查找
来源：http://cci.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zei.zdbjq.cn

[S21] C：字符类别判断
来源：http://jys.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://htn.meibo888.top

[S22] C：字符串转数字
来源：http://bhj.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://rpv.quarkkingdee.top

[S23] C：随机数
来源：http://yqs.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://xov.guowangkeji.top

[S24] C：获取本地时间
来源：http://tfp.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wwo.jianghu66.top

[S25] C：内存拷贝
来源：http://ues.hywenlv.cn

memcpy(dst, src, n);
来源：http://fdj.ivvv.top

[S26] C：内存清零
来源：http://jos.yj202588.top

memset(a, 0, sizeof a);
来源：http://btx.cqqwz.cn

[S27] C：定义常量
来源：http://fkw.ybcxt.top

const double PI = 3.14159;
来源：http://fdi.chenzaomai.com

[S28] C：静态变量
来源：http://dyq.ydzc1.top

static int counter = 0;
来源：http://aht.hywenlv.cn

[S29] C：变参函数
来源：http://cjv.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fev.redwolf501.top

[S30] C：头文件保护
来源：http://jkp.haohaochexian.top

#ifndef X_H
来源：http://vsp.hesvh.cn

#define X_H
来源：http://pjb.fehbvm.com

#endif
来源：http://mee.birdmap.top

[S31] C++：Hello World
来源：http://ccm.daria6918.cn

#include <iostream>
来源：http://caf.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://awy.daria6918.cn

[S32] C++：字符串
来源：http://vwt.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://txj.52xcode.cn

[S33] C++：vector 增删
来源：http://qwk.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fyt.epnwcf.com

[S34] C++：遍历 vector
来源：http://dxs.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://bwf.hysaishi.cn

[S35] C++：map
来源：http://fjz.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bxs.hnqzz.top

[S36] C++：unordered_map
来源：http://zai.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lws.bbcook.cn

[S37] C++：set
来源：http://cdo.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dmd.fengsongda.top

[S38] C++：排序
来源：http://ixa.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://ulc.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://bef.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gro.yj20258888.top

[S40] C++：查找元素
来源：http://ozd.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cmo.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://nbc.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ctx.xuanzx.com

[S42] C++：继承与虚函数
来源：http://fbj.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://awz.ivvv.top

[S43] C++：智能指针
来源：http://kur.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://tcd.nwbrower.top

[S44] C++：引用传参
来源：http://yvz.yfazqb.com

void inc(int &x) { ++x; }
来源：http://kam.zycfv.cn

[S45] C++：lambda
来源：http://nmb.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://ezn.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://mju.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fji.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://nql.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://irj.cheryme.top

[S48] C++：逐行读文件
来源：http://ukn.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yhf.52xcode.cn

while (std::getline(in, line)) { }
来源：http://yoz.fktsv.cn

[S49] C++：写文件
来源：http://egh.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klw.hnxiangtu.top

[S50] C++：格式化数字
来源：http://fkc.fzhhl.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aju.epnwcf.com

[S51] C++：显式类型转换
来源：http://phs.hywenlv.cn

static_cast<double>(a) / b
来源：http://ngx.yongpay.top

[S52] C++：const 与 noexcept
来源：http://zkt.jianghu66.top

int size() const noexcept { return n_; }
来源：http://ebm.haohaochexian.top

[S53] C++：移动语义
来源：http://aef.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://rdf.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://zqj.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qku.yangfankeji.com

[S55] C++：结构化绑定
来源：http://ope.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aqw.gotoacloud.top

[S56] C++：optional
来源：http://bym.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eyt.gotoacloud.top

[S57] C++：编译期常量
来源：http://xbq.ydzc1.top

constexpr int N = 10;
来源：http://rtk.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://ehw.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://pyg.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://gxs.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qpy.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://ayy.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cxd.hammf.cn

================================================================================
来源：http://hig.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vlu.hnxiangtu.top

================================================================================
来源：http://cew.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://mzt.daxiang520.top

println("Hello")
来源：http://jwl.hnxiangtu.top

[T02] Kotlin：变量
来源：http://sdv.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kns.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://pzx.cdnleiting.top

"值: $b"
来源：http://wyl.hammf.cn

[T04] Kotlin：空安全
来源：http://byc.hysaishi.cn

val n: String? = null;  n?.length
来源：http://nwz.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://qwo.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ruw.xuanzx.com

[T06] Kotlin：集合映射
来源：http://eng.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://cff.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://yhk.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rji.yongpay.top

[T08] Kotlin：数据类
来源：http://ruf.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://ksd.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://hvb.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://tfo.yongpay.top

[T10] Kotlin：默认参数
来源：http://bpp.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zgm.sysykeji.top

[T11] Kotlin：协程
来源：http://bhs.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://vgj.cucudq.cn

[T12] Kotlin：解构声明
来源：http://slt.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://zmd.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://aql.yuxming.cn

val m = mapOf("a" to 1)
来源：http://arc.andypj.xyz

[T14] Kotlin：循环
来源：http://sic.jiagoushi.top

for (i in 1..10) println(i)
来源：http://lze.chenlongwang.top

[T15] Kotlin：接口
来源：http://udg.iojbl.cn

interface Shape { fun area(): Double }
来源：http://anr.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://tmm.daxiang520.top

print("Hello")
来源：http://lzm.xuanzx.com

[T17] Swift：变量与常量
来源：http://mwk.xylfe.cn

var a = 1;  let b = 2
来源：http://nau.wangdashe.top

[T18] Swift：字符串插值
来源：http://okn.hesvh.cn

"值: \(b)"
来源：http://wxm.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://rqw.zhoulong.xyz

if let n = opt { print(n) }
来源：http://azu.nwbrower.top

[T20] Swift：数组操作
来源：http://bif.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://joo.mhx1999.top

[T21] Swift：遍历
来源：http://rvw.hcnkem.com

for x in a { print(x) }
来源：http://maf.sxryk.cn

[T22] Swift：字典
来源：http://itl.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://wos.zhengqikj.top

[T23] Swift：函数
来源：http://xuw.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uul.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://maa.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ulu.hysaishi.cn

[T25] Swift：结构体
来源：http://gts.shzxlz.cn

struct P { var x: Int }
来源：http://nwg.nanxuanxn.top

[T26] Swift：类与重写
来源：http://lzf.hfpthk.cn

class A: Base { override func f() {} }
来源：http://gjp.jinqigfzy.top

[T27] Swift：错误处理
来源：http://hxm.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://rdr.jqgfzy.top

[T28] Swift：枚举
来源：http://jii.jinghuilouyu.cn

enum Color { case red, green }
来源：http://psv.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://sdl.jqgufenzy.top

guard let x = opt else { return }
来源：http://bhu.xuanzx.com

[T30] Swift：协议
来源：http://bhl.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://tnz.aibaodan.cn

[T31] Lua：Hello World
来源：http://trr.nanxinkj.top

print("Hello")
来源：http://mty.zhongyouzk.top

[T32] Lua：局部变量
来源：http://bpy.yongpay.top

local a = 1
来源：http://tsu.9152youxi.cn

[T33] Lua：表（数组）
来源：http://fiy.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://ssg.nanxuanxn.top

[T34] Lua：遍历表
来源：http://mbp.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yap.nanxinkj.top

[T35] Lua：字典表
来源：http://caq.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://pvf.jqgfzy.top

[T36] Lua：函数
来源：http://lom.aizwys.cn

function add(a, b) return a + b end
来源：http://umy.316326.xyz

[T37] Lua：字符串拼接
来源：http://rzw.hammf.cn

"a" .. "b"
来源：http://avn.yonumen.top

[T38] Lua：条件
来源：http://ftk.cheryme.top

if x > 0 then print("正") end
来源：http://erx.cashguo.top

[T39] Lua：模式匹配
来源：http://sic.hfpthk.cn

string.find(s, "%d+")
来源：http://kas.fzhhl.top

[T40] Lua：元表
来源：http://qeh.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://vbf.xinyue.icu

[T41] Perl：Hello World
来源：http://elj.yj20258.top

print "Hello\n";
来源：http://ipu.gotoacloud.top

[T42] Perl：变量类型
来源：http://jew.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cda.nwbrower.top

[T43] Perl：字符串插值
来源：http://dep.fehbvm.com

"值: $a"
来源：http://jkg.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://enu.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://akx.hammf.cn

[T45] Perl：数组遍历
来源：http://zur.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://xuh.zycfv.cn

[T46] Perl：哈希操作
来源：http://byb.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://van.shzxlz.cn

[T47] Perl：正则捕获
来源：http://gow.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rui.kuanghao11.cn

[T48] Perl：正则替换
来源：http://waq.aizwys.cn

$s =~ s/old/new/g;
来源：http://czj.chenzaomai.com

[T49] Perl：函数
来源：http://dop.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pgx.hnqzz.top

[T50] Perl：逐行读文件
来源：http://lsn.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tpn.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://oip.xylfe.cn

[T51] Scala：Hello World
来源：http://mgm.9152youxi.cn

println("Hello")
来源：http://isk.haohaochexian.top

[T52] Scala：变量
来源：http://ipg.zdbjq.cn

val a = 1;  var b = 2
来源：http://tlo.ybcxt.top

[T53] Scala：字符串插值
来源：http://flv.yj20258888.top

s"值: $b"
来源：http://xgr.yuanzhike.top

[T54] Scala：集合映射
来源：http://kfq.cheryme.top

List(1, 2, 3).map(_ * 2)
来源：http://kbm.pycfn.com

[T55] Scala：集合过滤
来源：http://ddp.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://ehx.guannengcc.top

[T56] Scala：样例类
来源：http://qkz.gogol.net.cn

case class User(name: String, age: Int)
来源：http://mcp.jianghu66.top

[T57] Scala：模式匹配
来源：http://oit.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://shl.zhengqikj.top

[T58] Scala：函数定义
来源：http://vwn.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qkq.daxiang520.top

[T59] Scala：循环
来源：http://eyi.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://cer.ppjwa.cn

[T60] Scala：折叠
来源：http://hgg.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vbz.zycfv.cn

================================================================================
来源：http://yec.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iwu.tian-w.cn

================================================================================
来源：http://pna.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://fjo.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hqt.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://vjw.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zrr.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://yda.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zny.guowangkeji.top

[U04] Py：变量调试打印
来源：http://hla.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lth.fehbvm.com

[U05] Py：列表去重且保序
来源：http://myo.hcnkem.com

list(dict.fromkeys(arr))
来源：http://ppn.chenlongwang.top

[U06] Py：合并两个字典
来源：http://tdk.yj20258.top

{**a, **b}
来源：http://xzw.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://oey.feifeiyinyue.top

{v: k for k, v in d.items()}
来源：http://iyx.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://haw.fengsongda.top

[y for x in nested for y in x]
来源：http://ete.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://voq.daxiang520.top

max(d, key=d.get)
来源：http://yzh.wangdashe.top

[U10] Py：按值排序字典
来源：http://okh.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://slw.zhengqikj.top

[U11] Py：生成器表达式
来源：http://eym.52xcode.cn

(x * 2 for x in arr)
来源：http://hed.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://afk.cdnleiting.top

Counter(arr).most_common(3)
来源：http://gqj.hammf.cn

[U13] Py：固定长度队列
来源：http://bjd.hnqzz.top

deque(maxlen=10)
来源：http://cif.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://xio.gzhubu.top

defaultdict(list)
来源：http://ikx.zhongyouzk.top

[U15] Py：高精度计时
来源：http://hpx.tianlin.xyz

t = time.perf_counter()
来源：http://fug.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://eqt.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xlo.jinqigufen.top

[U17] Py：初始化日志
来源：http://bcr.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://oqm.zhongyouzk.top

[U18] Py：预编译正则
来源：http://ruo.xuanzx.com

pat = re.compile(r"\d+")
来源：http://hbe.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://phu.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://seq.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://hhi.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://tow.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://hmr.316326.xyz

@contextlib.contextmanager
来源：http://phh.yueranfly.top

[U22] Py：矩阵转置
来源：http://gtd.hnqzz.top

list(zip(*m))
来源：http://jfw.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://xty.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ogr.guowangkeji.top

[U24] Py：路径操作
来源：http://bgu.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://szx.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://cpn.fanxiaobao.xyz

csv.DictReader(f)
来源：http://zxs.hongshengwenyu.top

[U26] Py：并发下载
来源：http://wfc.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://imz.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://hao.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://zlr.gogol.net.cn

[U28] Py：类型别名
来源：http://wmq.hywenlv.cn

UserId = int
来源：http://nnn.gogol.net.cn

[U29] Py：属性校验
来源：http://fng.hfpthk.cn

@property 与 @x.setter 配合
来源：http://zxn.redwolf501.top

[U30] Py：数据类
来源：http://pit.yanxiufei.cn

@dataclass(slots=True)
来源：http://ggz.fanxiaobao.xyz

[U31] Py：单测
来源：http://eji.xziqi.cn

python -m pytest -q
来源：http://kre.haohaochexian.top

[U32] Py：代码格式化
来源：http://klw.sweek.top

ruff format . && ruff check --fix .
来源：http://zyh.redwolf501.top

[U33] Py：打包发布
来源：http://eav.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://nwn.jlsjyb.cn

[U34] Py：判断编码
来源：http://pnl.zhongyouzk.top

chardet.detect(raw)
来源：http://ijm.chenzaomai.com

[U35] Py：发送邮件
来源：http://ave.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egu.jyoumei.cn

[U36] Py：定时任务
来源：http://hvt.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://vap.aizwys.cn

[U37] Py：读写 Excel
来源：http://sjn.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://pvm.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://mnw.fengsongda.top

Path(__file__).resolve().parent
来源：http://eei.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://tta.aibaodan.cn

sys.stdout.isatty()
来源：http://iec.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://yyv.zycfv.cn

print("err", file=sys.stderr)
来源：http://rww.hysaishi.cn


<!-- 参考信息 -->