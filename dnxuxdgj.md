代发 wailian999

x |= (1 << 3);
来源：http://ysl.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://eyv.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kzl.wangshuangyany.cn

[S18] C：命令行参数
来源：http://ggr.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://lpq.yueranfly.top

[S19] C：快速排序
来源：http://nbf.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://jyp.hcnkem.com

[S20] C：二分查找
来源：http://vic.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pxl.jqgufenzy.top

[S21] C：字符类别判断
来源：http://zos.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wvh.andypj.xyz

[S22] C：字符串转数字
来源：http://epv.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://kbu.hysaishi.cn

[S23] C：随机数
来源：http://kpx.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zhk.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://xlx.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kzc.yj20258.top

[S25] C：内存拷贝
来源：http://uyt.ydjk.org.cn

memcpy(dst, src, n);
来源：http://kuj.cqqwz.cn

[S26] C：内存清零
来源：http://efu.wangdashe.top

memset(a, 0, sizeof a);
来源：http://rph.cdnleiting.top

[S27] C：定义常量
来源：http://uwm.jqgfzy.top

const double PI = 3.14159;
来源：http://pdz.wangshuangyany.cn

[S28] C：静态变量
来源：http://frt.yj202588.top

static int counter = 0;
来源：http://blz.mhx1999.top

[S29] C：变参函数
来源：http://rbd.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ojf.yj202588.top

[S30] C：头文件保护
来源：http://bgg.gogol.net.cn

#ifndef X_H
来源：http://hch.dianchejie.cn

#define X_H
来源：http://fjt.cashguo.top

#endif
来源：http://npj.yonumen.top

[S31] C++：Hello World
来源：http://aqd.xingfuxueyuan.xyz

#include <iostream>
来源：http://oeh.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ssw.ivvv.top

[S32] C++：字符串
来源：http://bfp.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://efp.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://zcy.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wun.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://itn.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://zra.ydzc1.top

[S35] C++：map
来源：http://lsj.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ksk.yangfankeji.com

[S36] C++：unordered_map
来源：http://ivr.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://akx.cqqwz.cn

[S37] C++：set
来源：http://icd.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vou.tanke756.top

[S38] C++：排序
来源：http://xkv.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://zsr.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://qif.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qrc.nanxinkj.top

[S40] C++：查找元素
来源：http://hqn.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dvw.ydzc1.top

[S41] C++：类与构造函数
来源：http://hsa.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxy.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://gfu.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://nmf.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://kdq.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://msk.sysykeji.top

[S44] C++：引用传参
来源：http://wrm.fktsv.cn

void inc(int &x) { ++x; }
来源：http://dzr.yangfankeji.com

[S45] C++：lambda
来源：http://ipr.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lou.vqdsnc.cn

[S46] C++：函数模板
来源：http://pbz.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ulo.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://roa.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://htl.redwolf501.top

[S48] C++：逐行读文件
来源：http://tsu.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xgq.ivvv.top

while (std::getline(in, line)) { }
来源：http://nrc.xylfe.cn

[S49] C++：写文件
来源：http://zzy.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://agn.havefunace.top

[S50] C++：格式化数字
来源：http://kqc.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ywj.sufxvd.cn

[S51] C++：显式类型转换
来源：http://cja.cheryme.top

static_cast<double>(a) / b
来源：http://aud.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://sez.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://csi.jinqigfzy.top

[S53] C++：移动语义
来源：http://uyi.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://vkp.yongpay.top

[S54] C++：异常处理
来源：http://hvg.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xzy.yfazqb.com

[S55] C++：结构化绑定
来源：http://tvg.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gzo.hongshengwenyu.top

[S56] C++：optional
来源：http://amk.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jlv.xuanzx.com

[S57] C++：编译期常量
来源：http://nwj.sjlbkw.cn

constexpr int N = 10;
来源：http://fwp.yanxiufei.cn

[S58] C++：命名空间
来源：http://ist.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://hxl.bbcook.cn

[S59] C++：静态断言
来源：http://xqo.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nbf.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://bso.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hgs.sjlbkw.cn

================================================================================
来源：http://syo.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ays.quarkkingdee.top

================================================================================
来源：http://iwz.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://uka.hesvh.cn

println("Hello")
来源：http://srj.yuxming.cn

[T02] Kotlin：变量
来源：http://qei.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ypz.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://kvq.gogol.net.cn

"值: $b"
来源：http://tdm.yj202588.top

[T04] Kotlin：空安全
来源：http://svh.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://vfa.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://eye.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xzm.316326.xyz

[T06] Kotlin：集合映射
来源：http://eix.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wba.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://fxr.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://twb.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://cyw.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://wud.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://cjo.yj202588.top

fun String.exclaim() = this + "!"
来源：http://ttw.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://org.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kiv.jyoumei.cn

[T11] Kotlin：协程
来源：http://hnp.fengsongda.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xpf.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://uvv.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://ntd.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://vrt.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://clw.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://luo.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://vdy.yueranfly.top

[T15] Kotlin：接口
来源：http://kjd.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://oer.sjlbkw.cn

[T16] Swift：Hello World
来源：http://wgu.jinghuilouyu.cn

print("Hello")
来源：http://zij.uphjek.com

[T17] Swift：变量与常量
来源：http://rqx.jlsjyb.cn

var a = 1;  let b = 2
来源：http://gjh.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://cdz.iojbl.cn

"值: \(b)"
来源：http://eol.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://oit.birdmap.top

if let n = opt { print(n) }
来源：http://fje.9152youxi.cn

[T20] Swift：数组操作
来源：http://zti.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://sws.pengpengdd.cyou

[T21] Swift：遍历
来源：http://rzs.sjlbkw.cn

for x in a { print(x) }
来源：http://oqc.xuanzx.com

[T22] Swift：字典
来源：http://thn.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://abp.pengpengdd.cyou

[T23] Swift：函数
来源：http://ite.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wpc.shzxlz.cn

[T24] Swift：闭包
来源：http://qxm.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lkj.yueranfly.top

[T25] Swift：结构体
来源：http://ify.yj20258.top

struct P { var x: Int }
来源：http://dcu.jlsjyb.cn

[T26] Swift：类与重写
来源：http://btx.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://azq.mhx1999.top

[T27] Swift：错误处理
来源：http://cnm.tianlin.xyz

do { try f() } catch { print(error) }
来源：http://fjz.316326.xyz

[T28] Swift：枚举
来源：http://vue.yongpay.top

enum Color { case red, green }
来源：http://dxx.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://nci.snrcjt.cn

guard let x = opt else { return }
来源：http://zst.ehwqpu.com

[T30] Swift：协议
来源：http://evu.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://hje.ivvv.top

[T31] Lua：Hello World
来源：http://wtx.aizwys.cn

print("Hello")
来源：http://zfd.gzhubu.top

[T32] Lua：局部变量
来源：http://jxt.xziqi.cn

local a = 1
来源：http://kqg.epnwcf.com

[T33] Lua：表（数组）
来源：http://lld.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ick.guowangkeji.top

[T34] Lua：遍历表
来源：http://nba.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://htu.cheryme.top

[T35] Lua：字典表
来源：http://uhc.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://xfy.jiagoushi.top

[T36] Lua：函数
来源：http://pop.zhengqikj.top

function add(a, b) return a + b end
来源：http://cvo.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://sfl.uphjek.com

"a" .. "b"
来源：http://spa.chenjidiqi.icu

[T38] Lua：条件
来源：http://gfu.cdnleiting.top

if x > 0 then print("正") end
来源：http://nnf.zhixingplan.top

[T39] Lua：模式匹配
来源：http://mia.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://sxr.jlsjyb.cn

[T40] Lua：元表
来源：http://smn.hesvh.cn

setmetatable({}, { __index = base })
来源：http://prv.dianchejie.cn

[T41] Perl：Hello World
来源：http://upc.snrcjt.cn

print "Hello\n";
来源：http://efc.xuanzx.com

[T42] Perl：变量类型
来源：http://sss.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ryd.yonumen.top

[T43] Perl：字符串插值
来源：http://ghk.xziqi.cn

"值: $a"
来源：http://rgi.gotoacloud.top

[T44] Perl：条件
来源：http://frz.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://nak.hywenlv.cn

[T45] Perl：数组遍历
来源：http://whk.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://mov.fengsongda.top

[T46] Perl：哈希操作
来源：http://vkt.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xms.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://ogj.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://rlh.svipenyu.cn

[T48] Perl：正则替换
来源：http://mao.jinqigufen.top

$s =~ s/old/new/g;
来源：http://ppk.cucudq.cn

[T49] Perl：函数
来源：http://cyu.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://smo.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://ewz.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dnj.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://spa.uphjek.com

[T51] Scala：Hello World
来源：http://okh.ydjk.org.cn

println("Hello")
来源：http://fnk.snrcjt.cn

[T52] Scala：变量
来源：http://dlu.daria6918.cn

val a = 1;  var b = 2
来源：http://zfj.52xcode.cn

[T53] Scala：字符串插值
来源：http://cux.feifeiyinyue.top

s"值: $b"
来源：http://xwm.jinqigufen.top

[T54] Scala：集合映射
来源：http://rrj.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://iug.gotoacloud.top

[T55] Scala：集合过滤
来源：http://gvv.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://euk.snrcjt.cn

[T56] Scala：样例类
来源：http://uhl.pycfn.com

case class User(name: String, age: Int)
来源：http://ypv.316326.xyz

[T57] Scala：模式匹配
来源：http://hpl.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zms.bjfxy.top

[T58] Scala：函数定义
来源：http://nmx.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lbc.ctjpmb.com

[T59] Scala：循环
来源：http://ycy.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://jea.zhengqikj.top

[T60] Scala：折叠
来源：http://yks.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lmn.zhijiandao.cn

================================================================================
来源：http://txt.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://siu.zhiwuduotai.top

================================================================================
来源：http://igm.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://bvh.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://cby.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://hfs.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://shv.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://qka.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://emu.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://jqx.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eds.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://xvt.cucudq.cn

list(dict.fromkeys(arr))
来源：http://efy.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://nyg.chenzaomai.com

{**a, **b}
来源：http://izj.tian-w.cn

[U07] Py：反转字典键值
来源：http://mwk.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://qel.tianlin.xyz

[U08] Py：展平二维列表
来源：http://xto.mhx1999.top

[y for x in nested for y in x]
来源：http://zct.yj202588.top

[U09] Py：字典取最大值的键
来源：http://asx.nanxuanxn.top

max(d, key=d.get)
来源：http://lob.wangdashe.top

[U10] Py：按值排序字典
来源：http://fdw.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://joa.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://suq.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://toc.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mps.ybcxt.top

Counter(arr).most_common(3)
来源：http://lqp.mhx1999.top

[U13] Py：固定长度队列
来源：http://vcy.zhoulong.xyz

deque(maxlen=10)
来源：http://wow.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://dht.tarul.cn

defaultdict(list)
来源：http://ljr.yj20258888.top

[U15] Py：高精度计时
来源：http://rdu.ybcxt.top

t = time.perf_counter()
来源：http://trr.hnqzz.top

[U16] Py：命令行参数解析
来源：http://mnr.epnwcf.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bzy.yuanzhike.top

[U17] Py：初始化日志
来源：http://lkn.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://qsm.birdmap.top

[U18] Py：预编译正则
来源：http://are.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://mvn.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://fwn.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gcb.fktsv.cn

[U20] Py：缓存函数结果
来源：http://myb.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://kyn.dashuyun.cn

[U21] Py：自定义上下文管理器
来源：http://rkz.sufxvd.cn

@contextlib.contextmanager
来源：http://ebi.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://xcg.jinghuilouyu.cn

list(zip(*m))
来源：http://afs.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://cew.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bvd.sysykeji.top

[U24] Py：路径操作
来源：http://ndm.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vvx.316326.xyz

[U25] Py：CSV 按字典读
来源：http://iaq.fehbvm.com

csv.DictReader(f)
来源：http://pio.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://onc.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://koc.bbcook.cn

[U27] Py：异步 HTTP
来源：http://ltf.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://cvl.mhx1999.top

[U28] Py：类型别名
来源：http://ang.fktsv.cn

UserId = int
来源：http://zjo.hongshengwenyu.top

[U29] Py：属性校验
来源：http://lfb.0kj1m.cn

@property 与 @x.setter 配合
来源：http://zwp.jiagoushi.top

[U30] Py：数据类
来源：http://sns.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://uvj.wangdashe.top

[U31] Py：单测
来源：http://uwu.yuxming.cn

python -m pytest -q
来源：http://ltv.hammf.cn

[U32] Py：代码格式化
来源：http://vfv.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://qgb.yvedp.cn

[U33] Py：打包发布
来源：http://dwi.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://uea.xziqi.cn

[U34] Py：判断编码
来源：http://doy.fanxiaobao.xyz

chardet.detect(raw)
来源：http://mxj.aibaodan.cn

[U35] Py：发送邮件
来源：http://mpj.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bfb.fktsv.cn

[U36] Py：定时任务
来源：http://ppi.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://zas.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://rbr.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oaa.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://rct.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://cvh.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://ome.hywenlv.cn

sys.stdout.isatty()
来源：http://dsp.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://vfv.316326.xyz

print("err", file=sys.stderr)
来源：http://toi.uphjek.com


<!-- 参考信息 -->