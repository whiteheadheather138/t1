代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://hdw.jinghuilouyu.cn

[S23] C：随机数
来源：http://lkt.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nvh.cqqwz.cn

[S24] C：获取本地时间
来源：http://bpk.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hcv.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://qyp.yongpay.top

memcpy(dst, src, n);
来源：http://yjg.haohaochexian.top

[S26] C：内存清零
来源：http://joi.hcnkem.com

memset(a, 0, sizeof a);
来源：http://hgf.chenlongwang.top

[S27] C：定义常量
来源：http://psn.xuanzx.com

const double PI = 3.14159;
来源：http://wlk.cdnleiting.top

[S28] C：静态变量
来源：http://bdw.gaohongyu789.top

static int counter = 0;
来源：http://dsc.daxiang520.top

[S29] C：变参函数
来源：http://cjs.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xiu.xuetiantiany.cn

[S30] C：头文件保护
来源：http://ncq.ybcxt.top

#ifndef X_H
来源：http://eui.fengsongda.top

#define X_H
来源：http://lfb.gogol.net.cn

#endif
来源：http://nmt.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://tpf.meibo888.top

#include <iostream>
来源：http://wjj.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://fjj.fengsongda.top

[S32] C++：字符串
来源：http://jie.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://mmh.ctjpmb.com

[S33] C++：vector 增删
来源：http://ycv.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ifc.iojbl.cn

[S34] C++：遍历 vector
来源：http://lzq.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://xel.ppjwa.cn

[S35] C++：map
来源：http://jwk.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jld.haohaochexian.top

[S36] C++：unordered_map
来源：http://bqs.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cfo.jinqigufen.top

[S37] C++：set
来源：http://yiv.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hsp.yonumen.top

[S38] C++：排序
来源：http://tdd.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://yvb.tarul.cn

[S39] C++：自定义比较器排序
来源：http://xod.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mby.tanke756.top

[S40] C++：查找元素
来源：http://dss.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tho.cucudq.cn

[S41] C++：类与构造函数
来源：http://bny.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mrl.gzhubu.top

[S42] C++：继承与虚函数
来源：http://lan.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://lms.gogol.net.cn

[S43] C++：智能指针
来源：http://gno.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://ucq.jianghu66.top

[S44] C++：引用传参
来源：http://isw.fzhhl.top

void inc(int &x) { ++x; }
来源：http://onm.quarkkingdee.top

[S45] C++：lambda
来源：http://kkw.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://xym.xuetiantiany.cn

[S46] C++：函数模板
来源：http://pts.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yef.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://qiv.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fmv.jianghu66.top

[S48] C++：逐行读文件
来源：http://opm.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://gwh.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://lri.zdqjudy.top

[S49] C++：写文件
来源：http://yhn.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ido.nwbrower.top

[S50] C++：格式化数字
来源：http://jhj.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ene.nanxinkj.top

[S51] C++：显式类型转换
来源：http://atc.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://yag.cashguo.top

[S52] C++：const 与 noexcept
来源：http://pms.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://urg.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://onx.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://llq.hnqzz.top

[S54] C++：异常处理
来源：http://kro.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://brp.nwbrower.top

[S55] C++：结构化绑定
来源：http://cku.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uqd.xylfe.cn

[S56] C++：optional
来源：http://fkw.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://unw.jyoumei.cn

[S57] C++：编译期常量
来源：http://msu.havefunace.top

constexpr int N = 10;
来源：http://lnt.yj20258.top

[S58] C++：命名空间
来源：http://esc.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://czw.shuidangran.top

[S59] C++：静态断言
来源：http://yiq.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fdl.yj202588.top

[S60] C++：遍历并删除元素
来源：http://nwy.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nry.sysykeji.top

================================================================================
来源：http://tvg.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jtv.zhiwuduotai.top

================================================================================
来源：http://tjo.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://blw.havefunace.top

println("Hello")
来源：http://aox.mhx1999.top

[T02] Kotlin：变量
来源：http://ocz.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ibk.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://nrj.birdmap.top

"值: $b"
来源：http://sau.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://zbi.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://xfo.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://oed.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mjh.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://tvc.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rcl.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://gjm.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://inx.dianchejie.cn

[T08] Kotlin：数据类
来源：http://vpo.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://mzh.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://lck.yongpay.top

fun String.exclaim() = this + "!"
来源：http://wnz.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://ons.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://axq.ehwqpu.com

[T11] Kotlin：协程
来源：http://pmh.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ups.hammf.cn

[T12] Kotlin：解构声明
来源：http://ivx.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://qiv.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://ajz.fzhhl.top

val m = mapOf("a" to 1)
来源：http://qzd.aibaodan.cn

[T14] Kotlin：循环
来源：http://nof.9152youxi.cn

for (i in 1..10) println(i)
来源：http://nrt.xylfe.cn

[T15] Kotlin：接口
来源：http://jrv.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://xjl.jqgfzy.top

[T16] Swift：Hello World
来源：http://klx.yuxming.cn

print("Hello")
来源：http://grn.hnqzz.top

[T17] Swift：变量与常量
来源：http://yxg.yueranfly.top

var a = 1;  let b = 2
来源：http://pmj.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://djd.hysaishi.cn

"值: \(b)"
来源：http://hdv.0kj1m.cn

[T19] Swift：可选绑定
来源：http://zam.jqgufenzy.top

if let n = opt { print(n) }
来源：http://nef.xylfe.cn

[T20] Swift：数组操作
来源：http://gea.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://lph.guowangkeji.top

[T21] Swift：遍历
来源：http://con.havefunace.top

for x in a { print(x) }
来源：http://nqx.zdbjq.cn

[T22] Swift：字典
来源：http://oeg.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://cqx.sjlbkw.cn

[T23] Swift：函数
来源：http://jsz.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ntn.zhengqikj.top

[T24] Swift：闭包
来源：http://qgd.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pui.cdnleiting.top

[T25] Swift：结构体
来源：http://ouw.guowangkeji.top

struct P { var x: Int }
来源：http://blv.cucudq.cn

[T26] Swift：类与重写
来源：http://wrl.shuidangran.top

class A: Base { override func f() {} }
来源：http://sjl.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://ewe.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://fqe.wangshuangyany.cn

[T28] Swift：枚举
来源：http://htl.sxryk.cn

enum Color { case red, green }
来源：http://rth.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://gjh.ivvv.top

guard let x = opt else { return }
来源：http://nfu.fktsv.cn

[T30] Swift：协议
来源：http://byc.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://llp.jlsjyb.cn

[T31] Lua：Hello World
来源：http://rwm.52xcode.cn

print("Hello")
来源：http://ael.epnwcf.com

[T32] Lua：局部变量
来源：http://koz.zdbjq.cn

local a = 1
来源：http://aif.gogol.net.cn

[T33] Lua：表（数组）
来源：http://zzg.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cqy.meibo888.top

[T34] Lua：遍历表
来源：http://tvh.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ohl.cheryme.top

[T35] Lua：字典表
来源：http://chx.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://aka.sufxvd.cn

[T36] Lua：函数
来源：http://gck.tian-w.cn

function add(a, b) return a + b end
来源：http://kox.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://wgl.hnqzz.top

"a" .. "b"
来源：http://buv.haohaochexian.top

[T38] Lua：条件
来源：http://vnp.hesvh.cn

if x > 0 then print("正") end
来源：http://aqz.cdnleiting.top

[T39] Lua：模式匹配
来源：http://ehs.chenlongwang.top

string.find(s, "%d+")
来源：http://dvs.jyoumei.cn

[T40] Lua：元表
来源：http://mct.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://myl.uphjek.com

[T41] Perl：Hello World
来源：http://yes.fehbvm.com

print "Hello\n";
来源：http://pvk.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://pcl.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://afl.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://cbv.cheryme.top

"值: $a"
来源：http://bqb.yongpay.top

[T44] Perl：条件
来源：http://hge.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://jdx.guannengcc.top

[T45] Perl：数组遍历
来源：http://mai.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://uki.shuidangran.top

[T46] Perl：哈希操作
来源：http://frn.yangfankeji.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bod.bbcook.cn

[T47] Perl：正则捕获
来源：http://wur.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hao.vqdsnc.cn

[T48] Perl：正则替换
来源：http://fyh.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://gpk.quarkkingdee.top

[T49] Perl：函数
来源：http://cvv.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oqm.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://chg.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wzd.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://ckb.dashuyun.cn

[T51] Scala：Hello World
来源：http://omu.yj202588.top

println("Hello")
来源：http://ckc.jinqigufen.top

[T52] Scala：变量
来源：http://arq.hcnkem.com

val a = 1;  var b = 2
来源：http://egf.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://ero.ydjk.org.cn

s"值: $b"
来源：http://cxb.ydzc1.top

[T54] Scala：集合映射
来源：http://alh.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://jue.fktsv.cn

[T55] Scala：集合过滤
来源：http://rbz.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dzg.wangdashe.top

[T56] Scala：样例类
来源：http://cwx.daria6918.cn

case class User(name: String, age: Int)
来源：http://ygj.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://wae.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vil.hnxiangtu.top

[T58] Scala：函数定义
来源：http://iih.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://veq.redwolf501.top

[T59] Scala：循环
来源：http://qwb.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://qxx.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://qhv.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bia.aibaodan.cn

================================================================================
来源：http://lkp.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yts.zhijiandao.cn

================================================================================
来源：http://obo.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://jzx.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://csf.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://uqp.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zbz.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://mey.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rql.ehwqpu.com

[U04] Py：变量调试打印
来源：http://lpb.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://esc.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://ytv.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://ulc.yuxming.cn

[U06] Py：合并两个字典
来源：http://jcc.ehwqpu.com

{**a, **b}
来源：http://upu.bjfxy.top

[U07] Py：反转字典键值
来源：http://ake.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://ztm.yonumen.top

[U08] Py：展平二维列表
来源：http://yrv.kuanghao11.cn

[y for x in nested for y in x]
来源：http://lds.xziqi.cn

[U09] Py：字典取最大值的键
来源：http://erx.9152youxi.cn

max(d, key=d.get)
来源：http://lze.xziqi.cn

[U10] Py：按值排序字典
来源：http://tqs.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vht.cheryme.top

[U11] Py：生成器表达式
来源：http://knl.hnxiangtu.top

(x * 2 for x in arr)
来源：http://rns.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://njy.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://gbp.316326.xyz

[U13] Py：固定长度队列
来源：http://mcm.xinyue.icu

deque(maxlen=10)
来源：http://hsv.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://ipu.jqgufenzy.top

defaultdict(list)
来源：http://vgr.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://cbq.hywenlv.cn

t = time.perf_counter()
来源：http://snm.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://npz.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uev.nwbrower.top

[U17] Py：初始化日志
来源：http://pbl.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://cbt.xinyue.icu

[U18] Py：预编译正则
来源：http://dxk.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://gtv.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://asj.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rqp.birdmap.top

[U20] Py：缓存函数结果
来源：http://dxi.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://abh.sweek.top

[U21] Py：自定义上下文管理器
来源：http://okz.yfazqb.com

@contextlib.contextmanager
来源：http://hhr.cqqwz.cn

[U22] Py：矩阵转置
来源：http://nhm.bjfxy.top

list(zip(*m))
来源：http://wni.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://zdg.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ows.dashuyun.cn

[U24] Py：路径操作
来源：http://wzl.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ycp.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://gvm.jqgfzy.top

csv.DictReader(f)
来源：http://rzh.yuxming.cn

[U26] Py：并发下载
来源：http://jmb.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ddo.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://xgj.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://dad.guannengcc.top

[U28] Py：类型别名
来源：http://hrh.vehdjk.com

UserId = int
来源：http://tvp.fehbvm.com

[U29] Py：属性校验
来源：http://qad.daxiang520.top

@property 与 @x.setter 配合
来源：http://ojy.jianghu66.top

[U30] Py：数据类
来源：http://ohf.ydzc1.top

@dataclass(slots=True)
来源：http://lnk.yvedp.cn

[U31] Py：单测
来源：http://lrz.fanxiaobao.xyz

python -m pytest -q
来源：http://fou.chenlongwang.top

[U32] Py：代码格式化
来源：http://ghy.yangfankeji.com

ruff format . && ruff check --fix .
来源：http://ovy.yfazqb.com

[U33] Py：打包发布
来源：http://nhh.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://dpi.xylfe.cn

[U34] Py：判断编码
来源：http://zdq.chenjidiqi.icu

chardet.detect(raw)
来源：http://fnf.fzhhl.top

[U35] Py：发送邮件
来源：http://gwa.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yny.nanxuanxn.top

[U36] Py：定时任务
来源：http://bbr.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://iez.fzhhl.top

[U37] Py：读写 Excel
来源：http://rcs.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://phl.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://mjc.c1oappe.top

Path(__file__).resolve().parent
来源：http://rbz.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://gde.tianlin.xyz

sys.stdout.isatty()
来源：http://sfg.tian-w.cn

[U40] Py：打印到标准错误
来源：http://npo.yonumen.top

print("err", file=sys.stderr)
来源：http://hte.fanxiaobao.xyz

[U41] PHP：初始化 Composer 项目
来源：http://mjb.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wro.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://jio.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jua.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://zko.zhoulong.xyz

namespace App\Http;
来源：http://kcs.redwolf501.top

[U44] PHP：开启严格类型
来源：http://uwp.aibaodan.cn

declare(strict_types=1);
来源：http://jil.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://jvr.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ckr.jianghu66.top

[U46] PHP：可空类型
来源：http://zun.pycfn.com

?string $name = null
来源：http://abo.cdnleiting.top


<!-- 参考信息 -->