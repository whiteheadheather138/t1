代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbj.ybcxt.top

[S21] C：字符类别判断
来源：http://dwk.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://anv.chenlongwang.top

[S22] C：字符串转数字
来源：http://mch.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://crk.shuidangran.top

[S23] C：随机数
来源：http://czj.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wtk.yueranfly.top

[S24] C：获取本地时间
来源：http://csi.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fmq.birdmap.top

[S25] C：内存拷贝
来源：http://xdl.hysaishi.cn

memcpy(dst, src, n);
来源：http://xdb.ehwqpu.com

[S26] C：内存清零
来源：http://bxj.ydzc1.top

memset(a, 0, sizeof a);
来源：http://lxj.52xcode.cn

[S27] C：定义常量
来源：http://dgx.chenlongwang.top

const double PI = 3.14159;
来源：http://rfu.tianlin.xyz

[S28] C：静态变量
来源：http://wym.redwolf501.top

static int counter = 0;
来源：http://few.chenlongwang.top

[S29] C：变参函数
来源：http://spv.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etb.ehwqpu.com

[S30] C：头文件保护
来源：http://pev.tian-w.cn

#ifndef X_H
来源：http://hgz.tianlin.xyz

#define X_H
来源：http://awp.dashuyun.cn

#endif
来源：http://rlx.hesvh.cn

[S31] C++：Hello World
来源：http://gww.zhoulong.xyz

#include <iostream>
来源：http://yrt.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ahc.jianghu66.top

[S32] C++：字符串
来源：http://wjr.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://gtd.9152youxi.cn

[S33] C++：vector 增删
来源：http://ldf.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pdp.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://orc.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://cri.ydzc1.top

[S35] C++：map
来源：http://iwh.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vph.zhongyouzk.top

[S36] C++：unordered_map
来源：http://own.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ait.cucudq.cn

[S37] C++：set
来源：http://gro.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vlq.aizwys.cn

[S38] C++：排序
来源：http://sqn.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://mtk.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://bap.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sri.redwolf501.top

[S40] C++：查找元素
来源：http://acq.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glg.guannengcc.top

[S41] C++：类与构造函数
来源：http://vjc.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://duu.gzhubu.top

[S42] C++：继承与虚函数
来源：http://svj.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://fyl.gaohongyu789.top

[S43] C++：智能指针
来源：http://cur.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://cjh.gaohongyu789.top

[S44] C++：引用传参
来源：http://xxj.yonumen.top

void inc(int &x) { ++x; }
来源：http://jwm.yuanzhike.top

[S45] C++：lambda
来源：http://uim.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://tdi.tianlin.xyz

[S46] C++：函数模板
来源：http://uzd.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sfq.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://ley.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yze.xinyue.icu

[S48] C++：逐行读文件
来源：http://aaw.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rcy.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://azn.yj20258.top

[S49] C++：写文件
来源：http://rya.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ium.jqgfzy.top

[S50] C++：格式化数字
来源：http://muf.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fpt.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://nfm.svipenyu.cn

static_cast<double>(a) / b
来源：http://arx.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://put.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://cyp.bjfxy.top

[S53] C++：移动语义
来源：http://zcz.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://bwm.zhiwuduotai.top

[S54] C++：异常处理
来源：http://lnk.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dbb.hywenlv.cn

[S55] C++：结构化绑定
来源：http://qle.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nny.pycfn.com

[S56] C++：optional
来源：http://uvy.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wkm.nwbrower.top

[S57] C++：编译期常量
来源：http://cfl.hcnkem.com

constexpr int N = 10;
来源：http://aov.yangfankeji.com

[S58] C++：命名空间
来源：http://ecc.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://ctt.0kj1m.cn

[S59] C++：静态断言
来源：http://qmc.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rzq.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://pst.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://omg.gzhubu.top

================================================================================
来源：http://tsp.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ejg.yuxming.cn

================================================================================
来源：http://kot.yj20258888.top

[T01] Kotlin：Hello World
来源：http://gxm.0kj1m.cn

println("Hello")
来源：http://org.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://uuh.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtk.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://vqh.ehwqpu.com

"值: $b"
来源：http://uxo.fzhhl.top

[T04] Kotlin：空安全
来源：http://rco.daria6918.cn

val n: String? = null;  n?.length
来源：http://ics.316326.xyz

[T05] Kotlin：when 表达式
来源：http://fzp.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mwp.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://iov.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://fhv.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://hcm.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vpl.hnqzz.top

[T08] Kotlin：数据类
来源：http://waw.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://lkr.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://vsp.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://itw.wangdashe.top

[T10] Kotlin：默认参数
来源：http://xgv.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tph.ydzc1.top

[T11] Kotlin：协程
来源：http://pmo.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tgm.ybcxt.top

[T12] Kotlin：解构声明
来源：http://yue.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://zri.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://cjt.yvedp.cn

val m = mapOf("a" to 1)
来源：http://ejw.9152youxi.cn

[T14] Kotlin：循环
来源：http://pjv.andypj.xyz

for (i in 1..10) println(i)
来源：http://xxj.316326.xyz

[T15] Kotlin：接口
来源：http://skv.yfazqb.com

interface Shape { fun area(): Double }
来源：http://nmj.pycfn.com

[T16] Swift：Hello World
来源：http://jjh.birdmap.top

print("Hello")
来源：http://fbk.svipenyu.cn

[T17] Swift：变量与常量
来源：http://fki.aibaodan.cn

var a = 1;  let b = 2
来源：http://tyu.fengsongda.top

[T18] Swift：字符串插值
来源：http://yyj.feifeiyinyue.top

"值: \(b)"
来源：http://mec.nanxinkj.top

[T19] Swift：可选绑定
来源：http://ykf.pycfn.com

if let n = opt { print(n) }
来源：http://fim.guannengcc.top

[T20] Swift：数组操作
来源：http://bke.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ofu.ctjpmb.com

[T21] Swift：遍历
来源：http://qix.shuidangran.top

for x in a { print(x) }
来源：http://sox.cqqwz.cn

[T22] Swift：字典
来源：http://wyz.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://cls.gaohongyu789.top

[T23] Swift：函数
来源：http://kvm.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ohq.vqdsnc.cn

[T24] Swift：闭包
来源：http://lwm.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gsj.andypj.xyz

[T25] Swift：结构体
来源：http://bux.yueranfly.top

struct P { var x: Int }
来源：http://mpy.fehbvm.com

[T26] Swift：类与重写
来源：http://fos.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://bhr.ydjk.org.cn

[T27] Swift：错误处理
来源：http://gij.xylfe.cn

do { try f() } catch { print(error) }
来源：http://sxr.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://niq.yuxming.cn

enum Color { case red, green }
来源：http://kxo.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://mvz.yvedp.cn

guard let x = opt else { return }
来源：http://bah.gzhubu.top

[T30] Swift：协议
来源：http://pxy.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://qdd.havefunace.top

[T31] Lua：Hello World
来源：http://ncz.bjfxy.top

print("Hello")
来源：http://kjb.aibaodan.cn

[T32] Lua：局部变量
来源：http://ihc.hnxiangtu.top

local a = 1
来源：http://acv.andypj.xyz

[T33] Lua：表（数组）
来源：http://zpz.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://idc.yonumen.top

[T34] Lua：遍历表
来源：http://xis.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://cih.jyoumei.cn

[T35] Lua：字典表
来源：http://csh.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://mhf.zhengqikj.top

[T36] Lua：函数
来源：http://utx.havefunace.top

function add(a, b) return a + b end
来源：http://itz.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://ykk.yonumen.top

"a" .. "b"
来源：http://udk.cqqwz.cn

[T38] Lua：条件
来源：http://byh.hesvh.cn

if x > 0 then print("正") end
来源：http://mkh.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://rgc.hcnkem.com

string.find(s, "%d+")
来源：http://jvr.snrcjt.cn

[T40] Lua：元表
来源：http://jog.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://gzp.sxryk.cn

[T41] Perl：Hello World
来源：http://nmp.52xcode.cn

print "Hello\n";
来源：http://coy.sxryk.cn

[T42] Perl：变量类型
来源：http://pre.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xvx.fzhhl.top

[T43] Perl：字符串插值
来源：http://dbp.svipenyu.cn

"值: $a"
来源：http://ful.iojbl.cn

[T44] Perl：条件
来源：http://spp.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://mld.andypj.xyz

[T45] Perl：数组遍历
来源：http://veh.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://yhu.guannengcc.top

[T46] Perl：哈希操作
来源：http://rgr.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vfe.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://hyr.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mai.52xcode.cn

[T48] Perl：正则替换
来源：http://udh.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://wwj.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://csf.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wxm.xinyue.icu

[T50] Perl：逐行读文件
来源：http://smm.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://emu.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://cgw.xingfuxueyuan.xyz

[T51] Scala：Hello World
来源：http://udn.sweek.top

println("Hello")
来源：http://dti.quarkkingdee.top

[T52] Scala：变量
来源：http://eof.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://pgn.snrcjt.cn

[T53] Scala：字符串插值
来源：http://zpi.tian-w.cn

s"值: $b"
来源：http://snb.epnwcf.com

[T54] Scala：集合映射
来源：http://mcl.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://pvp.cqqwz.cn

[T55] Scala：集合过滤
来源：http://for.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://van.sufxvd.cn

[T56] Scala：样例类
来源：http://xpx.pengpengdd.cyou

case class User(name: String, age: Int)
来源：http://hgi.ivvv.top

[T57] Scala：模式匹配
来源：http://eyv.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://krl.tanke756.top

[T58] Scala：函数定义
来源：http://anw.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://cjp.feifeiyinyue.top

[T59] Scala：循环
来源：http://zpw.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://mbg.sxryk.cn

[T60] Scala：折叠
来源：http://oyq.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lxy.fehbvm.com

================================================================================
来源：http://bzw.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fom.sysykeji.top

================================================================================
来源：http://fav.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://bsr.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://sfh.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://wdc.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yym.sweek.top

[U03] Py：加载 .env 配置
来源：http://pkb.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ptk.bbcook.cn

[U04] Py：变量调试打印
来源：http://teb.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jtb.sxryk.cn

[U05] Py：列表去重且保序
来源：http://uqb.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://wnl.tarul.cn

[U06] Py：合并两个字典
来源：http://ugy.nwbrower.top

{**a, **b}
来源：http://iwk.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://fgb.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://txk.smart0.xyz

[U08] Py：展平二维列表
来源：http://rae.gaohongyu789.top

[y for x in nested for y in x]
来源：http://oqb.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://tnc.xylfe.cn

max(d, key=d.get)
来源：http://jpk.ybcxt.top

[U10] Py：按值排序字典
来源：http://xhm.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ucj.cheryme.top

[U11] Py：生成器表达式
来源：http://ogw.havefunace.top

(x * 2 for x in arr)
来源：http://fah.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zcf.jyoumei.cn

Counter(arr).most_common(3)
来源：http://vdi.yanxiufei.cn

[U13] Py：固定长度队列
来源：http://klb.hongshengwenyu.top

deque(maxlen=10)
来源：http://ntp.hcnkem.com

[U14] Py：分组收集到列表
来源：http://vda.bbcook.cn

defaultdict(list)
来源：http://pdv.sysykeji.top

[U15] Py：高精度计时
来源：http://iwa.zhoulong.xyz

t = time.perf_counter()
来源：http://rug.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://lpk.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://puz.ybcxt.top

[U17] Py：初始化日志
来源：http://cjq.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://oyp.gzhubu.top

[U18] Py：预编译正则
来源：http://wvj.ywan-chungtsiang.top

pat = re.compile(r"\d+")
来源：http://trp.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://hud.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://avt.bbcook.cn

[U20] Py：缓存函数结果
来源：http://iop.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://xgj.bjfxy.top

[U21] Py：自定义上下文管理器
来源：http://hax.fzhhl.top

@contextlib.contextmanager
来源：http://wab.bjfxy.top

[U22] Py：矩阵转置
来源：http://gsz.xuetiantiany.cn

list(zip(*m))
来源：http://dkl.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://scu.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pzd.yvedp.cn

[U24] Py：路径操作
来源：http://vpt.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://skm.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://afm.jinqigufen.top

csv.DictReader(f)
来源：http://efp.gaohongyu789.top

[U26] Py：并发下载
来源：http://hhb.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kic.yvedp.cn

[U27] Py：异步 HTTP
来源：http://pum.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://rau.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://vau.birdmap.top

UserId = int
来源：http://rsv.zhiwuduotai.top

[U29] Py：属性校验
来源：http://qjm.sweek.top

@property 与 @x.setter 配合
来源：http://pyd.zdbjq.cn

[U30] Py：数据类
来源：http://xyw.cheryme.top

@dataclass(slots=True)
来源：http://dul.ivvv.top

[U31] Py：单测
来源：http://brk.haohaochexian.top

python -m pytest -q
来源：http://dry.ybcxt.top

[U32] Py：代码格式化
来源：http://rta.aizwys.cn

ruff format . && ruff check --fix .
来源：http://gdd.uphjek.com

[U33] Py：打包发布
来源：http://gnf.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ztw.zhiwuduotai.top

[U34] Py：判断编码
来源：http://uip.quarkkingdee.top

chardet.detect(raw)
来源：http://zmd.gotoacloud.top

[U35] Py：发送邮件
来源：http://ejv.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ozy.vqdsnc.cn

[U36] Py：定时任务
来源：http://vfg.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://eed.fzhhl.top

[U37] Py：读写 Excel
来源：http://vtf.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://fng.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://sra.mhx1999.top

Path(__file__).resolve().parent
来源：http://zst.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://llk.ydjk.org.cn

sys.stdout.isatty()
来源：http://gzy.havefunace.top

[U40] Py：打印到标准错误
来源：http://ixd.dianchejie.cn

print("err", file=sys.stderr)
来源：http://xcc.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://aaj.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ysk.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://wkq.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sti.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://ibc.yanxiufei.cn

namespace App\Http;
来源：http://jmc.chenlongwang.top

[U44] PHP：开启严格类型
来源：http://gvh.pengpengdd.cyou

declare(strict_types=1);
来源：http://acp.ydzc1.top


<!-- 参考信息 -->