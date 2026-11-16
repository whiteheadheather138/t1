代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://dtn.jqgfzy.top

[S23] C：随机数
来源：http://tqq.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pdv.quarkkingdee.top

[S24] C：获取本地时间
来源：http://lzf.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://djn.jianghu66.top

[S25] C：内存拷贝
来源：http://prn.zycfv.cn

memcpy(dst, src, n);
来源：http://vkw.jinghuilouyu.cn

[S26] C：内存清零
来源：http://elf.yuxming.cn

memset(a, 0, sizeof a);
来源：http://ebt.hnqzz.top

[S27] C：定义常量
来源：http://gcy.cqqwz.cn

const double PI = 3.14159;
来源：http://flz.vehdjk.com

[S28] C：静态变量
来源：http://ncl.c1oappe.top

static int counter = 0;
来源：http://sih.tarul.cn

[S29] C：变参函数
来源：http://ccw.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwe.cqqwz.cn

[S30] C：头文件保护
来源：http://vfi.zhijiandao.cn

#ifndef X_H
来源：http://rzz.jqgfzy.top

#define X_H
来源：http://jvf.aizwys.cn

#endif
来源：http://jyh.yj202588.top

[S31] C++：Hello World
来源：http://ziy.nwbrower.top

#include <iostream>
来源：http://ggh.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://diu.feifeiyinyue.top

[S32] C++：字符串
来源：http://ymf.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://mgt.pycfn.com

[S33] C++：vector 增删
来源：http://uro.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wsh.yj202588.top

[S34] C++：遍历 vector
来源：http://ywd.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://kyy.gogol.net.cn

[S35] C++：map
来源：http://xnn.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ncv.vqdsnc.cn

[S36] C++：unordered_map
来源：http://ngw.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aav.zdqjudy.top

[S37] C++：set
来源：http://atq.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uju.zhaomingkeji.xyz

[S38] C++：排序
来源：http://ask.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://ejv.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://yee.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yed.9152youxi.cn

[S40] C++：查找元素
来源：http://uay.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fuq.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://yqd.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://imi.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://klh.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://whx.0kj1m.cn

[S43] C++：智能指针
来源：http://rct.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://dbu.havefunace.top

[S44] C++：引用传参
来源：http://kpe.tanke756.top

void inc(int &x) { ++x; }
来源：http://qgi.hysaishi.cn

[S45] C++：lambda
来源：http://tyf.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zak.zhongyouzk.top

[S46] C++：函数模板
来源：http://dho.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zdj.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://uep.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://egf.dashuyun.cn

[S48] C++：逐行读文件
来源：http://cgx.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://osu.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://ckg.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://eca.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hly.jqgfzy.top

[S50] C++：格式化数字
来源：http://lpf.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qsr.yuxming.cn

[S51] C++：显式类型转换
来源：http://ccq.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://nca.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://yqk.tarul.cn

int size() const noexcept { return n_; }
来源：http://tvk.vqdsnc.cn

[S53] C++：移动语义
来源：http://usp.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://esv.zhiwuduotai.top

[S54] C++：异常处理
来源：http://ocd.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pyi.hysaishi.cn

[S55] C++：结构化绑定
来源：http://bry.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://odv.ppjwa.cn

[S56] C++：optional
来源：http://psg.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hlz.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://pyw.yanxiufei.cn

constexpr int N = 10;
来源：http://nfd.havefunace.top

[S58] C++：命名空间
来源：http://xkz.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://ojd.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://nkl.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kij.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://qiw.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kej.yfazqb.com

================================================================================
来源：http://rpa.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zyh.andypj.xyz

================================================================================
来源：http://zfk.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://zwx.bbcook.cn

println("Hello")
来源：http://jia.sweek.top

[T02] Kotlin：变量
来源：http://qhe.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://olt.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://rxb.daxiang520.top

"值: $b"
来源：http://hpm.yuxming.cn

[T04] Kotlin：空安全
来源：http://vol.yongpay.top

val n: String? = null;  n?.length
来源：http://mgl.birdmap.top

[T05] Kotlin：when 表达式
来源：http://olf.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dez.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://kfu.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://etw.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://ece.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://axp.jqgfzy.top

[T08] Kotlin：数据类
来源：http://kxj.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://mpi.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://zcp.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://nvm.yonumen.top

[T10] Kotlin：默认参数
来源：http://jsh.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ils.gogol.net.cn

[T11] Kotlin：协程
来源：http://kqi.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xrx.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://ewz.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://mml.cheryme.top

[T13] Kotlin：只读 Map
来源：http://tev.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://nza.shzxlz.cn

[T14] Kotlin：循环
来源：http://mgy.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://mwk.yanxiufei.cn

[T15] Kotlin：接口
来源：http://zik.fengsongda.top

interface Shape { fun area(): Double }
来源：http://hmm.ehwqpu.com

[T16] Swift：Hello World
来源：http://mnu.hysaishi.cn

print("Hello")
来源：http://vvk.xuanzx.com

[T17] Swift：变量与常量
来源：http://kcg.yuanzhike.top

var a = 1;  let b = 2
来源：http://oyn.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://qjv.snrcjt.cn

"值: \(b)"
来源：http://ifl.yuxming.cn

[T19] Swift：可选绑定
来源：http://mky.bjfxy.top

if let n = opt { print(n) }
来源：http://spu.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://hpi.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://obz.yonumen.top

[T21] Swift：遍历
来源：http://egk.chenzaomai.com

for x in a { print(x) }
来源：http://emh.meibo888.top

[T22] Swift：字典
来源：http://jan.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://gvb.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://hyr.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uzj.wangdashe.top

[T24] Swift：闭包
来源：http://hub.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cir.yfazqb.com

[T25] Swift：结构体
来源：http://nns.zhoulong.xyz

struct P { var x: Int }
来源：http://nvk.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://ljj.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://yed.fengsongda.top

[T27] Swift：错误处理
来源：http://sum.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://sgn.bbcook.cn

[T28] Swift：枚举
来源：http://cuk.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://iex.chenjidiqi.icu

[T29] Swift：guard 提前返回
来源：http://eub.wangdashe.top

guard let x = opt else { return }
来源：http://ypp.cashguo.top

[T30] Swift：协议
来源：http://vuz.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://gqq.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://xcv.zdqjudy.top

print("Hello")
来源：http://ogl.tanke756.top

[T32] Lua：局部变量
来源：http://spt.hcnkem.com

local a = 1
来源：http://fkv.yj20258.top

[T33] Lua：表（数组）
来源：http://izw.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://czy.ybcxt.top

[T34] Lua：遍历表
来源：http://dte.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ogc.zhiwuduotai.top

[T35] Lua：字典表
来源：http://try.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://gty.svipenyu.cn

[T36] Lua：函数
来源：http://xev.mhx1999.top

function add(a, b) return a + b end
来源：http://rgj.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://qkz.shanyushiyangkeji.top

"a" .. "b"
来源：http://szr.yueranfly.top

[T38] Lua：条件
来源：http://klx.ydjk.org.cn

if x > 0 then print("正") end
来源：http://eso.pycfn.com

[T39] Lua：模式匹配
来源：http://bzl.jinqigufen.top

string.find(s, "%d+")
来源：http://lht.kuanghao11.cn

[T40] Lua：元表
来源：http://feg.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://wso.zdbjq.cn

[T41] Perl：Hello World
来源：http://fqf.hysaishi.cn

print "Hello\n";
来源：http://uuu.dashuyun.cn

[T42] Perl：变量类型
来源：http://tov.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sxv.guannengcc.top

[T43] Perl：字符串插值
来源：http://vzc.9152youxi.cn

"值: $a"
来源：http://rby.hcnkem.com

[T44] Perl：条件
来源：http://owz.uphjek.com

if ($a > 0) { print "正"; }
来源：http://bdj.hywenlv.cn

[T45] Perl：数组遍历
来源：http://hvh.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://use.guowangkeji.top

[T46] Perl：哈希操作
来源：http://ofd.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fif.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://cvk.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://wlv.gotoacloud.top

[T48] Perl：正则替换
来源：http://agm.iojbl.cn

$s =~ s/old/new/g;
来源：http://xie.sjlbkw.cn

[T49] Perl：函数
来源：http://hyc.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zwd.xinyue.icu

[T50] Perl：逐行读文件
来源：http://iep.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://rtv.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://hrl.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://ohd.jyoumei.cn

println("Hello")
来源：http://qkx.c1oappe.top

[T52] Scala：变量
来源：http://xjg.jiagoushi.top

val a = 1;  var b = 2
来源：http://wwb.cqqwz.cn

[T53] Scala：字符串插值
来源：http://xoh.nanxuanxn.top

s"值: $b"
来源：http://ydg.c1oappe.top

[T54] Scala：集合映射
来源：http://cbn.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://zdp.jyoumei.cn

[T55] Scala：集合过滤
来源：http://hsd.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ghe.fehbvm.com

[T56] Scala：样例类
来源：http://rvi.jqgfzy.top

case class User(name: String, age: Int)
来源：http://kas.gogol.net.cn

[T57] Scala：模式匹配
来源：http://fuq.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sgf.zdqjudy.top

[T58] Scala：函数定义
来源：http://utb.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mgq.jinqigfzy.top

[T59] Scala：循环
来源：http://ock.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://vdk.ehwqpu.com

[T60] Scala：折叠
来源：http://eed.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xot.ydzc1.top

================================================================================
来源：http://doq.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njj.dashuyun.cn

================================================================================
来源：http://sez.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://lse.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qlh.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://hlj.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ffv.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://zei.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://msu.hnqzz.top

[U04] Py：变量调试打印
来源：http://rzd.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jsk.yuxming.cn

[U05] Py：列表去重且保序
来源：http://rvp.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://gnm.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://qca.bbcook.cn

{**a, **b}
来源：http://aed.jyoumei.cn

[U07] Py：反转字典键值
来源：http://swz.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://brk.vehdjk.com

[U08] Py：展平二维列表
来源：http://grp.ppjwa.cn

[y for x in nested for y in x]
来源：http://njc.tanke756.top

[U09] Py：字典取最大值的键
来源：http://noe.xziqi.cn

max(d, key=d.get)
来源：http://kai.guannengcc.top

[U10] Py：按值排序字典
来源：http://osl.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://brq.gzhubu.top

[U11] Py：生成器表达式
来源：http://tfg.tianlin.xyz

(x * 2 for x in arr)
来源：http://kub.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://rfx.ybcxt.top

Counter(arr).most_common(3)
来源：http://tsq.fengsongda.top

[U13] Py：固定长度队列
来源：http://fxu.cashguo.top

deque(maxlen=10)
来源：http://tid.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://ldo.svipenyu.cn

defaultdict(list)
来源：http://bpn.bjfxy.top

[U15] Py：高精度计时
来源：http://kjn.nwbrower.top

t = time.perf_counter()
来源：http://cwu.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://ibl.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cxu.fzhhl.top

[U17] Py：初始化日志
来源：http://ckz.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://npo.ivvv.top

[U18] Py：预编译正则
来源：http://nwk.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://thh.cucudq.cn

[U19] Py：正则替换带回调
来源：http://kps.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://stf.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://bih.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://xwp.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://kfw.fehbvm.com

@contextlib.contextmanager
来源：http://mgt.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://skr.yj202588.top

list(zip(*m))
来源：http://huu.fehbvm.com

[U23] Py：分块读取大文件
来源：http://fkx.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sfe.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://kqv.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ijg.yanxiufei.cn

[U25] Py：CSV 按字典读
来源：http://jvy.xziqi.cn

csv.DictReader(f)
来源：http://zbd.hfpthk.cn

[U26] Py：并发下载
来源：http://nlt.jyoumei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dej.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://jut.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://wuc.gzhubu.top

[U28] Py：类型别名
来源：http://gjh.0kj1m.cn

UserId = int
来源：http://knz.cucudq.cn

[U29] Py：属性校验
来源：http://zfs.birdmap.top

@property 与 @x.setter 配合
来源：http://uxr.haohaochexian.top

[U30] Py：数据类
来源：http://ngl.fengsongda.top

@dataclass(slots=True)
来源：http://hft.zhijiandao.cn

[U31] Py：单测
来源：http://vvu.52xcode.cn

python -m pytest -q
来源：http://xvh.zhoulong.xyz

[U32] Py：代码格式化
来源：http://bqa.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://qvg.havefunace.top

[U33] Py：打包发布
来源：http://ixv.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://aim.shuidangran.top

[U34] Py：判断编码
来源：http://xwv.haohaochexian.top

chardet.detect(raw)
来源：http://akq.zdqjudy.top

[U35] Py：发送邮件
来源：http://ybe.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bmf.0kj1m.cn

[U36] Py：定时任务
来源：http://ojg.tianlin.xyz

schedule.every(10).minutes.do(job)
来源：http://pau.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://pds.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jna.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://jow.iojbl.cn

Path(__file__).resolve().parent
来源：http://vwb.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://zoh.svipenyu.cn

sys.stdout.isatty()
来源：http://qci.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://dha.hywenlv.cn

print("err", file=sys.stderr)
来源：http://gbw.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://eqk.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://amh.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://tix.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjr.redwolf501.top

[U43] PHP：声明命名空间
来源：http://ixi.chenlongwang.top

namespace App\Http;
来源：http://ulr.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://yre.fktsv.cn

declare(strict_types=1);
来源：http://kiz.ivvv.top

[U45] PHP：类型声明与返回类型
来源：http://ale.hfpthk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cdv.hcnkem.com

[U46] PHP：可空类型
来源：http://fld.daxiang520.top

?string $name = null
来源：http://mjq.meibo888.top


<!-- 参考信息 -->