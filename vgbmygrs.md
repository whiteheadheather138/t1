代发 wailian999

x |= (1 << 3);
来源：http://ggm.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://wug.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csz.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://xzv.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://ari.zhijiandao.cn

[S19] C：快速排序
来源：http://kiz.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://quf.svipenyu.cn

[S20] C：二分查找
来源：http://ebx.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wyk.zhijiandao.cn

[S21] C：字符类别判断
来源：http://mmb.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lgq.tian-w.cn

[S22] C：字符串转数字
来源：http://cru.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://yhz.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://jiz.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xvc.yj20258888.top

[S24] C：获取本地时间
来源：http://ngj.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kvu.jyoumei.cn

[S25] C：内存拷贝
来源：http://eik.havefunace.top

memcpy(dst, src, n);
来源：http://ctf.hcnkem.com

[S26] C：内存清零
来源：http://igs.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://ubi.birdmap.top

[S27] C：定义常量
来源：http://arv.meibo888.top

const double PI = 3.14159;
来源：http://xvd.nanxinkj.top

[S28] C：静态变量
来源：http://ybn.chenlongwang.top

static int counter = 0;
来源：http://ufx.jiagoushi.top

[S29] C：变参函数
来源：http://ewz.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://meo.aizwys.cn

[S30] C：头文件保护
来源：http://reh.jinyuanbaomall.cn

#ifndef X_H
来源：http://zou.havefunace.top

#define X_H
来源：http://uft.cucudq.cn

#endif
来源：http://lwj.yj20258.top

[S31] C++：Hello World
来源：http://ihn.vehdjk.com

#include <iostream>
来源：http://aaq.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://stl.tianlin.xyz

[S32] C++：字符串
来源：http://krp.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://psb.hysaishi.cn

[S33] C++：vector 增删
来源：http://ubo.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tds.chenjidiqi.icu

[S34] C++：遍历 vector
来源：http://vkg.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://rhl.sxryk.cn

[S35] C++：map
来源：http://jna.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wjc.andypj.xyz

[S36] C++：unordered_map
来源：http://via.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hoy.tianlin.xyz

[S37] C++：set
来源：http://nue.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mpe.daxiang520.top

[S38] C++：排序
来源：http://rnj.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://gde.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://zud.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vgu.zhixingplan.top

[S40] C++：查找元素
来源：http://bqb.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pde.andypj.xyz

[S41] C++：类与构造函数
来源：http://god.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ytz.yfazqb.com

[S42] C++：继承与虚函数
来源：http://jtd.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://zcy.pycfn.com

[S43] C++：智能指针
来源：http://twr.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://vmo.hywenlv.cn

[S44] C++：引用传参
来源：http://yce.tarul.cn

void inc(int &x) { ++x; }
来源：http://oih.kuanghao11.cn

[S45] C++：lambda
来源：http://ymn.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://pyv.sysykeji.top

[S46] C++：函数模板
来源：http://pch.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://std.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://ugh.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://trs.sufxvd.cn

[S48] C++：逐行读文件
来源：http://ynp.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zti.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://zec.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://lfg.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wmz.hysaishi.cn

[S50] C++：格式化数字
来源：http://jik.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nlp.0kj1m.cn

[S51] C++：显式类型转换
来源：http://zqb.jqgufenzy.top

static_cast<double>(a) / b
来源：http://eqp.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://gta.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://cow.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://ohk.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://blg.shangyingyoupin.top

[S54] C++：异常处理
来源：http://koo.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sds.xziqi.cn

[S55] C++：结构化绑定
来源：http://szg.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://loq.c1oappe.top

[S56] C++：optional
来源：http://gxd.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crk.ydjk.org.cn

[S57] C++：编译期常量
来源：http://zms.jinqigufen.top

constexpr int N = 10;
来源：http://oqy.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://hag.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://fmw.yongpay.top

[S59] C++：静态断言
来源：http://olk.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rml.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://itq.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wsc.yj20258.top

================================================================================
来源：http://rgz.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aum.yangfankeji.com

================================================================================
来源：http://zrs.hcnkem.com

[T01] Kotlin：Hello World
来源：http://jmh.yanxiufei.cn

println("Hello")
来源：http://gjf.pycfn.com

[T02] Kotlin：变量
来源：http://rhl.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jdo.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://roi.haohaochexian.top

"值: $b"
来源：http://onv.fzhhl.top

[T04] Kotlin：空安全
来源：http://zyb.cdnleiting.top

val n: String? = null;  n?.length
来源：http://ihh.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://zah.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wjf.pycfn.com

[T06] Kotlin：集合映射
来源：http://hxr.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yqa.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://gus.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fce.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://gjs.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://ejc.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://few.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://iui.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://kwf.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wpo.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://nae.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kek.mhx1999.top

[T12] Kotlin：解构声明
来源：http://pga.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://baw.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://rhb.redwolf501.top

val m = mapOf("a" to 1)
来源：http://wob.316326.xyz

[T14] Kotlin：循环
来源：http://jku.hywenlv.cn

for (i in 1..10) println(i)
来源：http://yxs.yongpay.top

[T15] Kotlin：接口
来源：http://ojp.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://ila.haohaochexian.top

[T16] Swift：Hello World
来源：http://cer.yj202588.top

print("Hello")
来源：http://nyd.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://faa.ybcxt.top

var a = 1;  let b = 2
来源：http://ujs.svipenyu.cn

[T18] Swift：字符串插值
来源：http://yxr.xuetiantiany.cn

"值: \(b)"
来源：http://xkq.zhixingplan.top

[T19] Swift：可选绑定
来源：http://xcz.hcnkem.com

if let n = opt { print(n) }
来源：http://lqm.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://ttv.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://wqy.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://qvd.snrcjt.cn

for x in a { print(x) }
来源：http://gqs.tarul.cn

[T22] Swift：字典
来源：http://vnd.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ekc.0kj1m.cn

[T23] Swift：函数
来源：http://qmr.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://skj.kuanghao11.cn

[T24] Swift：闭包
来源：http://pub.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iou.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://rrq.hcnkem.com

struct P { var x: Int }
来源：http://plx.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://bbk.yueranfly.top

class A: Base { override func f() {} }
来源：http://wiy.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://rwj.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://jfk.gaohongyu789.top

[T28] Swift：枚举
来源：http://ojz.zhiwuduotai.top

enum Color { case red, green }
来源：http://pua.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://jph.dianchejie.cn

guard let x = opt else { return }
来源：http://nvz.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://ein.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://prb.redwolf501.top

[T31] Lua：Hello World
来源：http://jkd.jianghu66.top

print("Hello")
来源：http://ecd.yangfankeji.com

[T32] Lua：局部变量
来源：http://lyy.aibaodan.cn

local a = 1
来源：http://ewo.zhixingplan.top

[T33] Lua：表（数组）
来源：http://bpw.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qyc.zdbjq.cn

[T34] Lua：遍历表
来源：http://mem.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wiv.9152youxi.cn

[T35] Lua：字典表
来源：http://yac.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://cyw.epnwcf.com

[T36] Lua：函数
来源：http://qdw.ydzc1.top

function add(a, b) return a + b end
来源：http://dua.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://jfs.hesvh.cn

"a" .. "b"
来源：http://nlj.cucudq.cn

[T38] Lua：条件
来源：http://fmc.ctjpmb.com

if x > 0 then print("正") end
来源：http://emn.jqgfzy.top

[T39] Lua：模式匹配
来源：http://whr.c1oappe.top

string.find(s, "%d+")
来源：http://akq.yj202588.top

[T40] Lua：元表
来源：http://zxl.aizwys.cn

setmetatable({}, { __index = base })
来源：http://css.yj20258888.top

[T41] Perl：Hello World
来源：http://ine.gzhubu.top

print "Hello\n";
来源：http://yzz.hysaishi.cn

[T42] Perl：变量类型
来源：http://bsc.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jez.0kj1m.cn

[T43] Perl：字符串插值
来源：http://etm.bjfxy.top

"值: $a"
来源：http://krt.aibaodan.cn

[T44] Perl：条件
来源：http://qhd.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://bxs.dianchejie.cn

[T45] Perl：数组遍历
来源：http://nlv.dashuyun.cn

for my $x (@arr) { print $x; }
来源：http://nto.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://ebg.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pkn.uphjek.com

[T47] Perl：正则捕获
来源：http://org.jqgfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kpy.316326.xyz

[T48] Perl：正则替换
来源：http://elw.bjfxy.top

$s =~ s/old/new/g;
来源：http://bee.yj20258.top

[T49] Perl：函数
来源：http://cef.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://znl.yueranfly.top

[T50] Perl：逐行读文件
来源：http://yoe.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mvu.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://ega.mhx1999.top

[T51] Scala：Hello World
来源：http://lgo.yuxming.cn

println("Hello")
来源：http://miu.yvedp.cn

[T52] Scala：变量
来源：http://afl.vehdjk.com

val a = 1;  var b = 2
来源：http://irr.zdqjudy.top

[T53] Scala：字符串插值
来源：http://rss.yfazqb.com

s"值: $b"
来源：http://uaf.gaohongyu789.top

[T54] Scala：集合映射
来源：http://dlq.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://sfl.fktsv.cn

[T55] Scala：集合过滤
来源：http://iqn.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://eqe.zhiwuduotai.top

[T56] Scala：样例类
来源：http://dkz.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://udv.yongpay.top

[T57] Scala：模式匹配
来源：http://msx.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qxm.nanxuanxn.top

[T58] Scala：函数定义
来源：http://ypl.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://mva.jqgufenzy.top

[T59] Scala：循环
来源：http://prm.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://lbf.jiagoushi.top

[T60] Scala：折叠
来源：http://cvg.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://apg.hysaishi.cn

================================================================================
来源：http://idp.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rni.shzxlz.cn

================================================================================
来源：http://nsb.yj202588.top

[U01] Py：创建虚拟环境
来源：http://axc.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://tgu.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://ist.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kcq.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://jhd.xziqi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vjk.jiagoushi.top

[U04] Py：变量调试打印
来源：http://bwv.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nld.sweek.top

[U05] Py：列表去重且保序
来源：http://lgn.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://mqa.fengsongda.top

[U06] Py：合并两个字典
来源：http://sae.zhaomingkeji.xyz

{**a, **b}
来源：http://nwy.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://qun.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://ghl.fengsongda.top

[U08] Py：展平二维列表
来源：http://aqr.xinyue.icu

[y for x in nested for y in x]
来源：http://kgx.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://czk.shanyushiyangtech.top

max(d, key=d.get)
来源：http://pvx.zdqjudy.top

[U10] Py：按值排序字典
来源：http://pxr.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://grt.svipenyu.cn

[U11] Py：生成器表达式
来源：http://emc.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://ugm.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qdr.uphjek.com

Counter(arr).most_common(3)
来源：http://uad.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://ydz.hysaishi.cn

deque(maxlen=10)
来源：http://rmc.guannengcc.top

[U14] Py：分组收集到列表
来源：http://xzh.nanxinkj.top

defaultdict(list)
来源：http://jyh.birdmap.top

[U15] Py：高精度计时
来源：http://wiy.shuidangran.top

t = time.perf_counter()
来源：http://meo.yj20258.top

[U16] Py：命令行参数解析
来源：http://msq.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kyq.tian-w.cn

[U17] Py：初始化日志
来源：http://ljm.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://ufg.cqqwz.cn

[U18] Py：预编译正则
来源：http://ntv.nwbrower.top

pat = re.compile(r"\d+")
来源：http://eqo.vehdjk.com

[U19] Py：正则替换带回调
来源：http://oxa.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://upf.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://ntc.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://vdr.feifeiyinyue.top

[U21] Py：自定义上下文管理器
来源：http://pby.tarul.cn

@contextlib.contextmanager
来源：http://bnd.yfazqb.com

[U22] Py：矩阵转置
来源：http://qrb.jianghu66.top

list(zip(*m))
来源：http://euu.epnwcf.com

[U23] Py：分块读取大文件
来源：http://ckg.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nxy.cashguo.top

[U24] Py：路径操作
来源：http://gzg.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ins.sweek.top

[U25] Py：CSV 按字典读
来源：http://xqd.smart0.xyz

csv.DictReader(f)
来源：http://zpy.tianlin.xyz

[U26] Py：并发下载
来源：http://shx.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dim.zycfv.cn

[U27] Py：异步 HTTP
来源：http://wiy.svipenyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://sei.chenlongwang.top

[U28] Py：类型别名
来源：http://isx.sysykeji.top

UserId = int
来源：http://nse.sxryk.cn

[U29] Py：属性校验
来源：http://qiz.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://vmg.fanxiaobao.xyz

[U30] Py：数据类
来源：http://rxh.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://rjd.gotoacloud.top

[U31] Py：单测
来源：http://hkj.jiagoushi.top

python -m pytest -q
来源：http://jck.zhongyouzk.top

[U32] Py：代码格式化
来源：http://xue.yueranfly.top

ruff format . && ruff check --fix .
来源：http://ljt.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://wxu.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://rwq.zhiwuduotai.top

[U34] Py：判断编码
来源：http://arn.zdbjq.cn

chardet.detect(raw)
来源：http://fyu.bjfxy.top

[U35] Py：发送邮件
来源：http://sfh.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xyu.yvedp.cn

[U36] Py：定时任务
来源：http://dyy.fanxiaobao.xyz

schedule.every(10).minutes.do(job)
来源：http://aem.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://yab.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://bms.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://wnm.tarul.cn

Path(__file__).resolve().parent
来源：http://ess.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://nxq.gaohongyu789.top

sys.stdout.isatty()
来源：http://hdj.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://oef.c1oappe.top

print("err", file=sys.stderr)
来源：http://sbi.jqgufenzy.top


<!-- 参考信息 -->