代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://ext.jinqigfzy.top

[S23] C：随机数
来源：http://ivu.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vkf.hfpthk.cn

[S24] C：获取本地时间
来源：http://bsi.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ixp.gzhubu.top

[S25] C：内存拷贝
来源：http://vli.chenlongwang.top

memcpy(dst, src, n);
来源：http://abb.yj20258.top

[S26] C：内存清零
来源：http://uit.tanke756.top

memset(a, 0, sizeof a);
来源：http://pyj.zhijiandao.cn

[S27] C：定义常量
来源：http://jml.zhoulong.xyz

const double PI = 3.14159;
来源：http://zqj.nanxinkj.top

[S28] C：静态变量
来源：http://blq.cucudq.cn

static int counter = 0;
来源：http://hvr.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://jfp.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cdr.meibo888.top

[S30] C：头文件保护
来源：http://mkh.smart0.xyz

#ifndef X_H
来源：http://ijm.pycfn.com

#define X_H
来源：http://tci.tianlin.xyz

#endif
来源：http://rdl.zhongyouzk.top

[S31] C++：Hello World
来源：http://biz.feifeiyinyue.top

#include <iostream>
来源：http://mhn.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://tmp.guannengcc.top

[S32] C++：字符串
来源：http://bnj.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://ozk.xylfe.cn

[S33] C++：vector 增删
来源：http://qan.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ikv.zdbjq.cn

[S34] C++：遍历 vector
来源：http://scj.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://tds.yonumen.top

[S35] C++：map
来源：http://tgy.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qvn.aibaodan.cn

[S36] C++：unordered_map
来源：http://cyr.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qnk.bbcook.cn

[S37] C++：set
来源：http://pvh.jinqigfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gne.nanxinkj.top

[S38] C++：排序
来源：http://qzq.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://rrc.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://itp.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://usc.zhengqikj.top

[S40] C++：查找元素
来源：http://sjh.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vdy.uphjek.com

[S41] C++：类与构造函数
来源：http://feh.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ppl.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://xjr.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://gja.svipenyu.cn

[S43] C++：智能指针
来源：http://cci.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://tqt.gogol.net.cn

[S44] C++：引用传参
来源：http://kqk.fehbvm.com

void inc(int &x) { ++x; }
来源：http://wfc.yonumen.top

[S45] C++：lambda
来源：http://neb.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://hso.nwbrower.top

[S46] C++：函数模板
来源：http://fpt.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rfg.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://xit.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mpd.jianghu66.top

[S48] C++：逐行读文件
来源：http://wca.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mjj.sysykeji.top

while (std::getline(in, line)) { }
来源：http://uum.pycfn.com

[S49] C++：写文件
来源：http://xva.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hsv.sjlbkw.cn

[S50] C++：格式化数字
来源：http://clo.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://thj.316326.xyz

[S51] C++：显式类型转换
来源：http://iwa.ctjpmb.com

static_cast<double>(a) / b
来源：http://rrw.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://qpo.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://hir.aizwys.cn

[S53] C++：移动语义
来源：http://hqo.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://prp.vqdsnc.cn

[S54] C++：异常处理
来源：http://qnx.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qnq.chenlongwang.top

[S55] C++：结构化绑定
来源：http://hcs.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tru.chenzaomai.com

[S56] C++：optional
来源：http://zdd.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gav.hnqzz.top

[S57] C++：编译期常量
来源：http://gtw.kuanghao11.cn

constexpr int N = 10;
来源：http://skt.nwbrower.top

[S58] C++：命名空间
来源：http://xur.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://jeh.zhoulong.xyz

[S59] C++：静态断言
来源：http://tve.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oah.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://awx.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://grz.meibo888.top

================================================================================
来源：http://gex.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aqh.c1oappe.top

================================================================================
来源：http://sgo.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://rcf.nanxuanxn.top

println("Hello")
来源：http://gcs.fengsongda.top

[T02] Kotlin：变量
来源：http://jxu.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zco.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://dgb.smart0.xyz

"值: $b"
来源：http://bva.316326.xyz

[T04] Kotlin：空安全
来源：http://uhw.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://sgm.yj202588.top

[T05] Kotlin：when 表达式
来源：http://kst.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oiz.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://hbw.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kzl.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://eqc.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gus.zhixingplan.top

[T08] Kotlin：数据类
来源：http://bvk.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://qgj.meibo888.top

[T09] Kotlin：扩展函数
来源：http://amb.birdmap.top

fun String.exclaim() = this + "!"
来源：http://let.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://gcn.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lqt.svipenyu.cn

[T11] Kotlin：协程
来源：http://jfx.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ftz.52xcode.cn

[T12] Kotlin：解构声明
来源：http://ueo.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://wqu.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://ezf.fehbvm.com

val m = mapOf("a" to 1)
来源：http://rxg.uphjek.com

[T14] Kotlin：循环
来源：http://eav.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://cje.daria6918.cn

[T15] Kotlin：接口
来源：http://skx.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://oqu.zdqjudy.top

[T16] Swift：Hello World
来源：http://qxk.ywan-chungtsiang.top

print("Hello")
来源：http://izp.52xcode.cn

[T17] Swift：变量与常量
来源：http://myc.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://ckd.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://vxw.fehbvm.com

"值: \(b)"
来源：http://mmc.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://zvm.jyoumei.cn

if let n = opt { print(n) }
来源：http://djy.cucudq.cn

[T20] Swift：数组操作
来源：http://ygq.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qes.xziqi.cn

[T21] Swift：遍历
来源：http://jnt.jinqigfzy.top

for x in a { print(x) }
来源：http://kqe.wangshuangyany.cn

[T22] Swift：字典
来源：http://srb.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://njt.fanxiaobao.xyz

[T23] Swift：函数
来源：http://qry.yj202588.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bwu.cucudq.cn

[T24] Swift：闭包
来源：http://hdz.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ntv.wangshuangyany.cn

[T25] Swift：结构体
来源：http://zgc.yj20258.top

struct P { var x: Int }
来源：http://wia.tanke756.top

[T26] Swift：类与重写
来源：http://qjo.hysaishi.cn

class A: Base { override func f() {} }
来源：http://kxc.316326.xyz

[T27] Swift：错误处理
来源：http://byj.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://sph.sweek.top

[T28] Swift：枚举
来源：http://tij.wangdashe.top

enum Color { case red, green }
来源：http://dut.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://inr.yj202588.top

guard let x = opt else { return }
来源：http://arn.jqgfzy.top

[T30] Swift：协议
来源：http://fkx.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://ata.kuanghao11.cn

[T31] Lua：Hello World
来源：http://mgz.wangshuangyany.cn

print("Hello")
来源：http://bof.fktsv.cn

[T32] Lua：局部变量
来源：http://hrw.nanxinkj.top

local a = 1
来源：http://ald.guannengcc.top

[T33] Lua：表（数组）
来源：http://fjj.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kyt.yongpay.top

[T34] Lua：遍历表
来源：http://qsr.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zhv.quarkkingdee.top

[T35] Lua：字典表
来源：http://oxe.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://uls.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://lox.hesvh.cn

function add(a, b) return a + b end
来源：http://mqp.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://jvx.shangyingyoupin.top

"a" .. "b"
来源：http://lkk.0kj1m.cn

[T38] Lua：条件
来源：http://oao.birdmap.top

if x > 0 then print("正") end
来源：http://jwt.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://jid.ydzc1.top

string.find(s, "%d+")
来源：http://qmf.xziqi.cn

[T40] Lua：元表
来源：http://pyg.bjfxy.top

setmetatable({}, { __index = base })
来源：http://aih.yfazqb.com

[T41] Perl：Hello World
来源：http://beg.fanxiaobao.xyz

print "Hello\n";
来源：http://elo.zhengqikj.top

[T42] Perl：变量类型
来源：http://otq.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ala.zhixingplan.top

[T43] Perl：字符串插值
来源：http://atr.jinyuanbaomall.cn

"值: $a"
来源：http://pzw.dianchejie.cn

[T44] Perl：条件
来源：http://jsa.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://sik.gogol.net.cn

[T45] Perl：数组遍历
来源：http://dag.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://wgm.cheryme.top

[T46] Perl：哈希操作
来源：http://qpw.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fnu.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://vvx.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oxp.gotoacloud.top

[T48] Perl：正则替换
来源：http://oso.redwolf501.top

$s =~ s/old/new/g;
来源：http://kbg.aibaodan.cn

[T49] Perl：函数
来源：http://wbx.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kwj.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://gux.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mcf.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://gwp.quarkkingdee.top

[T51] Scala：Hello World
来源：http://uqd.sxryk.cn

println("Hello")
来源：http://ffy.xylfe.cn

[T52] Scala：变量
来源：http://ehf.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://lpr.xuanzx.com

[T53] Scala：字符串插值
来源：http://cid.daria6918.cn

s"值: $b"
来源：http://xaj.hysaishi.cn

[T54] Scala：集合映射
来源：http://pax.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vdg.tanke756.top

[T55] Scala：集合过滤
来源：http://oka.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kzl.sweek.top

[T56] Scala：样例类
来源：http://kot.daria6918.cn

case class User(name: String, age: Int)
来源：http://rgs.yonumen.top

[T57] Scala：模式匹配
来源：http://itn.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iuj.xinyue.icu

[T58] Scala：函数定义
来源：http://qsa.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://zyn.jyoumei.cn

[T59] Scala：循环
来源：http://uzp.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://cux.andypj.xyz

[T60] Scala：折叠
来源：http://oow.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gyc.cqqwz.cn

================================================================================
来源：http://hnj.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ixk.xingfuxueyuan.xyz

================================================================================
来源：http://taz.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://tle.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eic.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://wcb.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibn.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://rdh.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jsj.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://uyd.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hwa.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://gqe.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://koy.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://zwq.kuanghao11.cn

{**a, **b}
来源：http://tlh.hcnkem.com

[U07] Py：反转字典键值
来源：http://crw.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://mpq.52xcode.cn

[U08] Py：展平二维列表
来源：http://yey.tianlin.xyz

[y for x in nested for y in x]
来源：http://ymi.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://pnp.meibo888.top

max(d, key=d.get)
来源：http://bze.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://jgr.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jpp.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://xud.ppjwa.cn

(x * 2 for x in arr)
来源：http://wve.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vio.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://eeq.fehbvm.com

[U13] Py：固定长度队列
来源：http://hci.xylfe.cn

deque(maxlen=10)
来源：http://mrs.vehdjk.com

[U14] Py：分组收集到列表
来源：http://jtx.chenzaomai.com

defaultdict(list)
来源：http://byt.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://tbd.shangyingyoupin.top

t = time.perf_counter()
来源：http://rwn.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://ddh.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oem.zdqjudy.top

[U17] Py：初始化日志
来源：http://rpb.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://tdi.gotoacloud.top

[U18] Py：预编译正则
来源：http://lbm.bjfxy.top

pat = re.compile(r"\d+")
来源：http://iny.yonumen.top

[U19] Py：正则替换带回调
来源：http://dmy.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oke.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://qpq.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://fsh.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://hrz.tarul.cn

@contextlib.contextmanager
来源：http://jli.xylfe.cn

[U22] Py：矩阵转置
来源：http://dzh.ehwqpu.com

list(zip(*m))
来源：http://whs.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://xdr.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dut.wangshuangyany.cn

[U24] Py：路径操作
来源：http://eiz.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aml.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://dim.nanxinkj.top

csv.DictReader(f)
来源：http://hle.zdqjudy.top

[U26] Py：并发下载
来源：http://rfx.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qxs.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://atd.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://gwz.sysykeji.top

[U28] Py：类型别名
来源：http://vdk.nanxuanxn.top

UserId = int
来源：http://mcf.fehbvm.com

[U29] Py：属性校验
来源：http://kbd.sufxvd.cn

@property 与 @x.setter 配合
来源：http://rpq.iojbl.cn

[U30] Py：数据类
来源：http://tge.jyoumei.cn

@dataclass(slots=True)
来源：http://odz.chenlongwang.top

[U31] Py：单测
来源：http://qlf.cqqwz.cn

python -m pytest -q
来源：http://wah.sysykeji.top

[U32] Py：代码格式化
来源：http://zvs.fehbvm.com

ruff format . && ruff check --fix .
来源：http://qiz.dashuyun.cn

[U33] Py：打包发布
来源：http://lzt.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://rvj.shanyushiyangtech.top

[U34] Py：判断编码
来源：http://zbl.meibo888.top

chardet.detect(raw)
来源：http://gvy.c1oappe.top

[U35] Py：发送邮件
来源：http://rwa.birdmap.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qmr.jlsjyb.cn

[U36] Py：定时任务
来源：http://zin.chenlongwang.top

schedule.every(10).minutes.do(job)
来源：http://prp.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://mig.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://noc.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://xjj.sysykeji.top

Path(__file__).resolve().parent
来源：http://gey.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://wbq.zhixingplan.top

sys.stdout.isatty()
来源：http://hxr.smart0.xyz

[U40] Py：打印到标准错误
来源：http://vvn.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://rsg.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://fmk.andypj.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://rlm.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://egv.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://atl.ydzc1.top

[U43] PHP：声明命名空间
来源：http://pwo.chenlongwang.top

namespace App\Http;
来源：http://tjk.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://fcg.zhoulong.xyz

declare(strict_types=1);
来源：http://bvw.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://uwq.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://qna.fehbvm.com

[U46] PHP：可空类型
来源：http://zcu.tanke756.top

?string $name = null
来源：http://pkt.xinyue.icu


<!-- 参考信息 -->