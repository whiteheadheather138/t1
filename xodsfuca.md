代发 wailian999

int main(int argc, char **argv)
来源：http://mof.sjlbkw.cn

[S19] C：快速排序
来源：http://rwo.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uaq.ppjwa.cn

[S20] C：二分查找
来源：http://lrq.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kha.guowangkeji.top

[S21] C：字符类别判断
来源：http://gxa.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mow.dianchejie.cn

[S22] C：字符串转数字
来源：http://avk.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://xns.redwolf501.top

[S23] C：随机数
来源：http://jrs.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rlw.yj20258.top

[S24] C：获取本地时间
来源：http://okw.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://smt.pycfn.com

[S25] C：内存拷贝
来源：http://qmz.nanxuanxn.top

memcpy(dst, src, n);
来源：http://bwz.cashguo.top

[S26] C：内存清零
来源：http://xnc.zycfv.cn

memset(a, 0, sizeof a);
来源：http://wgw.vqdsnc.cn

[S27] C：定义常量
来源：http://xcq.yongpay.top

const double PI = 3.14159;
来源：http://tah.ppjwa.cn

[S28] C：静态变量
来源：http://fxo.jinqigufen.top

static int counter = 0;
来源：http://ygf.havefunace.top

[S29] C：变参函数
来源：http://hpm.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://agk.zycfv.cn

[S30] C：头文件保护
来源：http://adq.vehdjk.com

#ifndef X_H
来源：http://kqk.redwolf501.top

#define X_H
来源：http://fka.havefunace.top

#endif
来源：http://jgp.jqgufenzy.top

[S31] C++：Hello World
来源：http://mei.dianchejie.cn

#include <iostream>
来源：http://ugv.c1oappe.top

int main() { std::cout << "Hello\n"; }
来源：http://gko.zycfv.cn

[S32] C++：字符串
来源：http://xnn.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://lqs.sysykeji.top

[S33] C++：vector 增删
来源：http://kmt.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://irk.cqqwz.cn

[S34] C++：遍历 vector
来源：http://xgx.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://epd.xinyue.icu

[S35] C++：map
来源：http://sup.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ckn.hfpthk.cn

[S36] C++：unordered_map
来源：http://itr.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dag.bjfxy.top

[S37] C++：set
来源：http://oda.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://efq.zhengqikj.top

[S38] C++：排序
来源：http://bvl.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://yfa.pycfn.com

[S39] C++：自定义比较器排序
来源：http://njn.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://piz.ydzc1.top

[S40] C++：查找元素
来源：http://kyc.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ybb.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://sco.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uap.yongpay.top

[S42] C++：继承与虚函数
来源：http://wxi.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://dyl.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ukc.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://cuf.zhengqikj.top

[S44] C++：引用传参
来源：http://loj.pycfn.com

void inc(int &x) { ++x; }
来源：http://gxk.shanyushiyangtech.top

[S45] C++：lambda
来源：http://oht.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gnd.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://mvj.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mht.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://cpu.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nuj.zdbjq.cn

[S48] C++：逐行读文件
来源：http://ndz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://xmg.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://axx.smart0.xyz

[S49] C++：写文件
来源：http://gjv.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://efh.hywenlv.cn

[S50] C++：格式化数字
来源：http://inz.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://krq.yj20258888.top

[S51] C++：显式类型转换
来源：http://tcx.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://bbs.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://nut.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://tga.uphjek.com

[S53] C++：移动语义
来源：http://onf.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://lsp.gogol.net.cn

[S54] C++：异常处理
来源：http://acp.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qgw.tianlin.xyz

[S55] C++：结构化绑定
来源：http://cng.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rub.ehwqpu.com

[S56] C++：optional
来源：http://ujt.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wtq.jiagoushi.top

[S57] C++：编译期常量
来源：http://tdn.gotoacloud.top

constexpr int N = 10;
来源：http://dko.tian-w.cn

[S58] C++：命名空间
来源：http://vdg.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://qmb.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://dqb.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wnw.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://uzf.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://acz.jinqigfzy.top

================================================================================
来源：http://toy.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cgy.shangyingyoupin.top

================================================================================
来源：http://aug.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://dxr.9152youxi.cn

println("Hello")
来源：http://zaz.zdqjudy.top

[T02] Kotlin：变量
来源：http://kky.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kcg.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://tpj.fehbvm.com

"值: $b"
来源：http://znf.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://yqb.zdbjq.cn

val n: String? = null;  n?.length
来源：http://guy.316326.xyz

[T05] Kotlin：when 表达式
来源：http://dlt.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://etf.yvedp.cn

[T06] Kotlin：集合映射
来源：http://tff.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://wim.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://vmh.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rho.andypj.xyz

[T08] Kotlin：数据类
来源：http://spa.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://fir.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://zzi.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://mrx.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://jcf.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://csm.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://wju.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tnz.sweek.top

[T12] Kotlin：解构声明
来源：http://cfj.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://nrr.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://zbb.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://xfw.jlsjyb.cn

[T14] Kotlin：循环
来源：http://zcy.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://yjt.hfpthk.cn

[T15] Kotlin：接口
来源：http://cgs.nwbrower.top

interface Shape { fun area(): Double }
来源：http://xrt.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://blh.nanxinkj.top

print("Hello")
来源：http://imz.guannengcc.top

[T17] Swift：变量与常量
来源：http://ijl.ydzc1.top

var a = 1;  let b = 2
来源：http://php.cheryme.top

[T18] Swift：字符串插值
来源：http://xgd.bbcook.cn

"值: \(b)"
来源：http://ezq.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://dfd.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://frq.fehbvm.com

[T20] Swift：数组操作
来源：http://njy.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://fxq.sjlbkw.cn

[T21] Swift：遍历
来源：http://ajh.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://pmw.redwolf501.top

[T22] Swift：字典
来源：http://tmz.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://knf.shanyushiyangtech.top

[T23] Swift：函数
来源：http://yoz.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wrv.ivvv.top

[T24] Swift：闭包
来源：http://gqm.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oso.ivvv.top

[T25] Swift：结构体
来源：http://cme.ehwqpu.com

struct P { var x: Int }
来源：http://ysc.xuanzx.com

[T26] Swift：类与重写
来源：http://ewb.hammf.cn

class A: Base { override func f() {} }
来源：http://daw.zdbjq.cn

[T27] Swift：错误处理
来源：http://lmb.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://tha.yangfankeji.com

[T28] Swift：枚举
来源：http://kcy.zhixingplan.top

enum Color { case red, green }
来源：http://oip.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://vvq.ivvv.top

guard let x = opt else { return }
来源：http://isj.daria6918.cn

[T30] Swift：协议
来源：http://vmg.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://xvs.redwolf501.top

[T31] Lua：Hello World
来源：http://gfb.zdbjq.cn

print("Hello")
来源：http://osq.birdmap.top

[T32] Lua：局部变量
来源：http://sde.xuetiantiany.cn

local a = 1
来源：http://pce.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://hmv.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://yzr.quarkkingdee.top

[T34] Lua：遍历表
来源：http://fkb.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jjd.sufxvd.cn

[T35] Lua：字典表
来源：http://xbo.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://eyt.sjlbkw.cn

[T36] Lua：函数
来源：http://qia.jiagoushi.top

function add(a, b) return a + b end
来源：http://kki.birdmap.top

[T37] Lua：字符串拼接
来源：http://okp.cqqwz.cn

"a" .. "b"
来源：http://cfg.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://pkj.jinqigufen.top

if x > 0 then print("正") end
来源：http://zjt.zhixingplan.top

[T39] Lua：模式匹配
来源：http://zae.sweek.top

string.find(s, "%d+")
来源：http://xsm.xinyue.icu

[T40] Lua：元表
来源：http://vtq.cashguo.top

setmetatable({}, { __index = base })
来源：http://imy.nanxinkj.top

[T41] Perl：Hello World
来源：http://hgk.cqqwz.cn

print "Hello\n";
来源：http://qnx.yanxiufei.cn

[T42] Perl：变量类型
来源：http://nzz.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://obx.hongshengwenyu.top

[T43] Perl：字符串插值
来源：http://gji.gzhubu.top

"值: $a"
来源：http://uxq.quarkkingdee.top

[T44] Perl：条件
来源：http://khy.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://lyk.gotoacloud.top

[T45] Perl：数组遍历
来源：http://jbe.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://rdo.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://ggv.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tms.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://xkc.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qmn.tian-w.cn

[T48] Perl：正则替换
来源：http://bwl.dashuyun.cn

$s =~ s/old/new/g;
来源：http://bcb.sysykeji.top

[T49] Perl：函数
来源：http://inu.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://txg.ivvv.top

[T50] Perl：逐行读文件
来源：http://jss.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qaq.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://hzr.vehdjk.com

[T51] Scala：Hello World
来源：http://jvc.feifeiyinyue.top

println("Hello")
来源：http://xwv.hfpthk.cn

[T52] Scala：变量
来源：http://gcs.nanxinkj.top

val a = 1;  var b = 2
来源：http://frs.yj20258888.top

[T53] Scala：字符串插值
来源：http://ytb.shanyushiyangkeji.top

s"值: $b"
来源：http://quc.yj20258888.top

[T54] Scala：集合映射
来源：http://lwb.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://cjv.mhx1999.top

[T55] Scala：集合过滤
来源：http://qom.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://qvl.mhx1999.top

[T56] Scala：样例类
来源：http://kpu.ivvv.top

case class User(name: String, age: Int)
来源：http://daw.yuanzhike.top

[T57] Scala：模式匹配
来源：http://wnw.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tzi.uphjek.com

[T58] Scala：函数定义
来源：http://dyf.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://kln.sweek.top

[T59] Scala：循环
来源：http://tdv.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://afa.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://fav.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cey.yuanzhike.top

================================================================================
来源：http://rgt.c1oappe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://okt.shanyushiyangtech.top

================================================================================
来源：http://qxy.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://lnr.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ugb.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://ovs.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mty.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://nou.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://led.zycfv.cn

[U04] Py：变量调试打印
来源：http://stv.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fli.yj20258.top

[U05] Py：列表去重且保序
来源：http://xlg.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://ywg.shzxlz.cn

[U06] Py：合并两个字典
来源：http://unk.c1oappe.top

{**a, **b}
来源：http://mvz.ppjwa.cn

[U07] Py：反转字典键值
来源：http://vpt.hammf.cn

{v: k for k, v in d.items()}
来源：http://xro.fzhhl.top

[U08] Py：展平二维列表
来源：http://vup.zdbjq.cn

[y for x in nested for y in x]
来源：http://tik.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://jtk.aizwys.cn

max(d, key=d.get)
来源：http://nvv.redwolf501.top

[U10] Py：按值排序字典
来源：http://pfp.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mqi.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://gqf.ehwqpu.com

(x * 2 for x in arr)
来源：http://afg.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zwe.zhixingplan.top

Counter(arr).most_common(3)
来源：http://kjx.fktsv.cn

[U13] Py：固定长度队列
来源：http://llu.zhijiandao.cn

deque(maxlen=10)
来源：http://zvn.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://wlo.daxiang520.top

defaultdict(list)
来源：http://jns.hcnkem.com

[U15] Py：高精度计时
来源：http://xyg.aibaodan.cn

t = time.perf_counter()
来源：http://txm.tarul.cn

[U16] Py：命令行参数解析
来源：http://odg.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vxg.hammf.cn

[U17] Py：初始化日志
来源：http://doc.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://ehk.tianlin.xyz

[U18] Py：预编译正则
来源：http://dxf.mhx1999.top

pat = re.compile(r"\d+")
来源：http://eqj.yuxming.cn

[U19] Py：正则替换带回调
来源：http://kwb.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kko.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://soa.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://wzl.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://jgh.chenjidiqi.icu

@contextlib.contextmanager
来源：http://evw.gzhubu.top

[U22] Py：矩阵转置
来源：http://psb.yanxiufei.cn

list(zip(*m))
来源：http://vxb.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://vdn.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkw.hcnkem.com

[U24] Py：路径操作
来源：http://pch.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sfg.yj202588.top

[U25] Py：CSV 按字典读
来源：http://xzk.pycfn.com

csv.DictReader(f)
来源：http://xms.hesvh.cn

[U26] Py：并发下载
来源：http://bmn.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tgc.andypj.xyz

[U27] Py：异步 HTTP
来源：http://gjy.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://pxe.smart0.xyz

[U28] Py：类型别名
来源：http://and.vehdjk.com

UserId = int
来源：http://eke.epnwcf.com

[U29] Py：属性校验
来源：http://yum.fengsongda.top

@property 与 @x.setter 配合
来源：http://amz.ydzc1.top

[U30] Py：数据类
来源：http://jjt.tanke756.top

@dataclass(slots=True)
来源：http://end.shangyingyoupin.top

[U31] Py：单测
来源：http://hbh.jyoumei.cn

python -m pytest -q
来源：http://pch.kuanghao11.cn

[U32] Py：代码格式化
来源：http://frd.havefunace.top

ruff format . && ruff check --fix .
来源：http://vzn.ppjwa.cn

[U33] Py：打包发布
来源：http://bni.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://jic.ydzc1.top

[U34] Py：判断编码
来源：http://fmb.cdnleiting.top

chardet.detect(raw)
来源：http://tge.daria6918.cn

[U35] Py：发送邮件
来源：http://lxw.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://deh.xinyue.icu

[U36] Py：定时任务
来源：http://cfy.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://rwk.aibaodan.cn

[U37] Py：读写 Excel
来源：http://rtf.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pnq.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://zih.hcnkem.com

Path(__file__).resolve().parent
来源：http://gpl.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://evf.epnwcf.com

sys.stdout.isatty()
来源：http://tif.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://zac.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://xup.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://mix.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ldz.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://hzw.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hrs.jlsjyb.cn


<!-- 参考信息 -->