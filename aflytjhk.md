代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://jxo.shuidangran.top

[S23] C：随机数
来源：http://lsv.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://icj.hnqzz.top

[S24] C：获取本地时间
来源：http://sin.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mce.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://eiq.tanke756.top

memcpy(dst, src, n);
来源：http://gwz.nanxinkj.top

[S26] C：内存清零
来源：http://okw.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://pjf.meibo888.top

[S27] C：定义常量
来源：http://hte.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://vfy.snrcjt.cn

[S28] C：静态变量
来源：http://vmm.yonumen.top

static int counter = 0;
来源：http://cgt.jlsjyb.cn

[S29] C：变参函数
来源：http://dbh.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kto.xziqi.cn

[S30] C：头文件保护
来源：http://yhc.sxryk.cn

#ifndef X_H
来源：http://qim.fzhhl.top

#define X_H
来源：http://shm.bjfxy.top

#endif
来源：http://nrs.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://xol.hywenlv.cn

#include <iostream>
来源：http://ywz.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://rzd.jyoumei.cn

[S32] C++：字符串
来源：http://wev.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://puy.jianghu66.top

[S33] C++：vector 增删
来源：http://klv.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ltl.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://ode.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://ocl.fzhhl.top

[S35] C++：map
来源：http://tte.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://puq.yj20258.top

[S36] C++：unordered_map
来源：http://stu.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rdj.shzxlz.cn

[S37] C++：set
来源：http://sjo.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ron.ivvv.top

[S38] C++：排序
来源：http://vek.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://ctp.tanke756.top

[S39] C++：自定义比较器排序
来源：http://zev.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rst.dashuyun.cn

[S40] C++：查找元素
来源：http://lii.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rbe.cucudq.cn

[S41] C++：类与构造函数
来源：http://apa.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ocv.aizwys.cn

[S42] C++：继承与虚函数
来源：http://zzc.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://zoh.svipenyu.cn

[S43] C++：智能指针
来源：http://plz.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://ujm.zhongyouzk.top

[S44] C++：引用传参
来源：http://afx.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://est.yfazqb.com

[S45] C++：lambda
来源：http://oxj.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://xbr.hywenlv.cn

[S46] C++：函数模板
来源：http://tks.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opl.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://tnu.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yik.haohaochexian.top

[S48] C++：逐行读文件
来源：http://afu.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://dmv.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://moo.birdmap.top

[S49] C++：写文件
来源：http://yif.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wmg.pycfn.com

[S50] C++：格式化数字
来源：http://bps.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jgb.tarul.cn

[S51] C++：显式类型转换
来源：http://moo.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://ayt.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://nie.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://klh.yueranfly.top

[S53] C++：移动语义
来源：http://ahv.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://jyh.hammf.cn

[S54] C++：异常处理
来源：http://xus.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sxq.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://yfl.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngl.pycfn.com

[S56] C++：optional
来源：http://efy.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://egi.havefunace.top

[S57] C++：编译期常量
来源：http://wbu.ctjpmb.com

constexpr int N = 10;
来源：http://iei.gogol.net.cn

[S58] C++：命名空间
来源：http://lbc.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://zjc.feifeiyinyue.top

[S59] C++：静态断言
来源：http://xyg.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jag.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://rfd.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kxg.zhaomingkeji.xyz

================================================================================
来源：http://jgn.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pbz.cdnleiting.top

================================================================================
来源：http://syg.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://mfk.xziqi.cn

println("Hello")
来源：http://njx.tanke756.top

[T02] Kotlin：变量
来源：http://xjt.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yey.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://hne.birdmap.top

"值: $b"
来源：http://kge.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://nuh.52xcode.cn

val n: String? = null;  n?.length
来源：http://bpw.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://ayg.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://whp.havefunace.top

[T06] Kotlin：集合映射
来源：http://kvz.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://atp.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://vel.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ihf.jqgfzy.top

[T08] Kotlin：数据类
来源：http://zxi.hammf.cn

data class User(val name: String, val age: Int)
来源：http://xye.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://afa.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://wax.sweek.top

[T10] Kotlin：默认参数
来源：http://nee.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jng.0kj1m.cn

[T11] Kotlin：协程
来源：http://ckz.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mkz.shuidangran.top

[T12] Kotlin：解构声明
来源：http://woc.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://nnz.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://glm.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://ara.zycfv.cn

[T14] Kotlin：循环
来源：http://xvr.tianlin.xyz

for (i in 1..10) println(i)
来源：http://pml.hywenlv.cn

[T15] Kotlin：接口
来源：http://ckg.sxryk.cn

interface Shape { fun area(): Double }
来源：http://qtd.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://gpr.zhiwuduotai.top

print("Hello")
来源：http://lip.ydzc1.top

[T17] Swift：变量与常量
来源：http://vvy.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://odv.hfpthk.cn

[T18] Swift：字符串插值
来源：http://uja.fanxiaobao.xyz

"值: \(b)"
来源：http://frh.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://nui.meibo888.top

if let n = opt { print(n) }
来源：http://ksk.snrcjt.cn

[T20] Swift：数组操作
来源：http://oya.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://pxd.zdqjudy.top

[T21] Swift：遍历
来源：http://teq.tian-w.cn

for x in a { print(x) }
来源：http://ahv.zhoulong.xyz

[T22] Swift：字典
来源：http://blv.meibo888.top

var d = ["a": 1];  d["b"] = 2
来源：http://ciw.fzhhl.top

[T23] Swift：函数
来源：http://wea.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://shk.sjlbkw.cn

[T24] Swift：闭包
来源：http://hcf.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yic.zhongyouzk.top

[T25] Swift：结构体
来源：http://qkf.birdmap.top

struct P { var x: Int }
来源：http://rcf.jiagoushi.top

[T26] Swift：类与重写
来源：http://rip.yuxming.cn

class A: Base { override func f() {} }
来源：http://lhg.xylfe.cn

[T27] Swift：错误处理
来源：http://ais.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://qys.dianchejie.cn

[T28] Swift：枚举
来源：http://frj.316326.xyz

enum Color { case red, green }
来源：http://dvw.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://myi.hammf.cn

guard let x = opt else { return }
来源：http://urd.daxiang520.top

[T30] Swift：协议
来源：http://zxi.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://zvj.0kj1m.cn

[T31] Lua：Hello World
来源：http://xrf.mhx1999.top

print("Hello")
来源：http://jaz.jiagoushi.top

[T32] Lua：局部变量
来源：http://dud.guowangkeji.top

local a = 1
来源：http://xcq.ivvv.top

[T33] Lua：表（数组）
来源：http://nma.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://orc.sxryk.cn

[T34] Lua：遍历表
来源：http://fvd.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vyk.chenlongwang.top

[T35] Lua：字典表
来源：http://lfe.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://pja.aibaodan.cn

[T36] Lua：函数
来源：http://xyx.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://och.hnqzz.top

[T37] Lua：字符串拼接
来源：http://urz.fktsv.cn

"a" .. "b"
来源：http://tkc.ydjk.org.cn

[T38] Lua：条件
来源：http://pwh.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://npc.xuanzx.com

[T39] Lua：模式匹配
来源：http://ogk.yvedp.cn

string.find(s, "%d+")
来源：http://wxr.pengpengdd.cyou

[T40] Lua：元表
来源：http://top.yvedp.cn

setmetatable({}, { __index = base })
来源：http://iiz.xinyue.icu

[T41] Perl：Hello World
来源：http://mmy.jqgufenzy.top

print "Hello\n";
来源：http://tjf.jinqigfzy.top

[T42] Perl：变量类型
来源：http://jwm.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xeb.tian-w.cn

[T43] Perl：字符串插值
来源：http://qpy.wangdashe.top

"值: $a"
来源：http://jlk.bbcook.cn

[T44] Perl：条件
来源：http://qvo.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://vmp.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://wta.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://qed.epnwcf.com

[T46] Perl：哈希操作
来源：http://yll.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xrv.jinqigufen.top

[T47] Perl：正则捕获
来源：http://uhc.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ndo.nanxinkj.top

[T48] Perl：正则替换
来源：http://ety.chenzaomai.com

$s =~ s/old/new/g;
来源：http://kgr.hcnkem.com

[T49] Perl：函数
来源：http://jmf.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ojb.xinyue.icu

[T50] Perl：逐行读文件
来源：http://ylp.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ypt.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://bwd.zdbjq.cn

[T51] Scala：Hello World
来源：http://xvu.tianlin.xyz

println("Hello")
来源：http://slv.c1oappe.top

[T52] Scala：变量
来源：http://mhm.jiagoushi.top

val a = 1;  var b = 2
来源：http://iyd.yueranfly.top

[T53] Scala：字符串插值
来源：http://qmz.yuanzhike.top

s"值: $b"
来源：http://esp.jqgufenzy.top

[T54] Scala：集合映射
来源：http://fqd.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://exf.pycfn.com

[T55] Scala：集合过滤
来源：http://yrr.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://xgk.sxryk.cn

[T56] Scala：样例类
来源：http://joi.yuxming.cn

case class User(name: String, age: Int)
来源：http://vku.0kj1m.cn

[T57] Scala：模式匹配
来源：http://itj.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://njv.zycfv.cn

[T58] Scala：函数定义
来源：http://fcs.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://etb.quarkkingdee.top

[T59] Scala：循环
来源：http://src.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://ftd.shuidangran.top

[T60] Scala：折叠
来源：http://agr.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jkh.zhaomingkeji.xyz

================================================================================
来源：http://mtc.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vqy.jinghuilouyu.cn

================================================================================
来源：http://por.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://onu.snrcjt.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aho.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://dlc.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hxh.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://zca.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hwl.guannengcc.top

[U04] Py：变量调试打印
来源：http://aay.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hgv.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://amk.sweek.top

list(dict.fromkeys(arr))
来源：http://kxa.iojbl.cn

[U06] Py：合并两个字典
来源：http://mpk.shanyushiyangtech.top

{**a, **b}
来源：http://kur.yongpay.top

[U07] Py：反转字典键值
来源：http://cqo.xylfe.cn

{v: k for k, v in d.items()}
来源：http://dqa.ehwqpu.com

[U08] Py：展平二维列表
来源：http://zbo.xinyue.icu

[y for x in nested for y in x]
来源：http://rpk.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://nwm.bbcook.cn

max(d, key=d.get)
来源：http://dnj.andypj.xyz

[U10] Py：按值排序字典
来源：http://cjs.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fac.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://qni.nanxuanxn.top

(x * 2 for x in arr)
来源：http://fxj.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://etu.52xcode.cn

Counter(arr).most_common(3)
来源：http://elb.xuanzx.com

[U13] Py：固定长度队列
来源：http://lrd.hesvh.cn

deque(maxlen=10)
来源：http://czr.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://ttj.yueranfly.top

defaultdict(list)
来源：http://vyx.jianghu66.top

[U15] Py：高精度计时
来源：http://xas.hywenlv.cn

t = time.perf_counter()
来源：http://nwk.tarul.cn

[U16] Py：命令行参数解析
来源：http://tfj.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://asf.dianchejie.cn

[U17] Py：初始化日志
来源：http://fos.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://ayr.sufxvd.cn

[U18] Py：预编译正则
来源：http://owu.hammf.cn

pat = re.compile(r"\d+")
来源：http://ysm.cashguo.top

[U19] Py：正则替换带回调
来源：http://qjo.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qbq.bjfxy.top

[U20] Py：缓存函数结果
来源：http://ynm.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://prg.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://oma.havefunace.top

@contextlib.contextmanager
来源：http://hzk.yvedp.cn

[U22] Py：矩阵转置
来源：http://qsz.zdbjq.cn

list(zip(*m))
来源：http://ela.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://chg.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kww.haohaochexian.top

[U24] Py：路径操作
来源：http://dlk.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gir.cashguo.top

[U25] Py：CSV 按字典读
来源：http://uxh.daxiang520.top

csv.DictReader(f)
来源：http://cyv.redwolf501.top

[U26] Py：并发下载
来源：http://lxx.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ruv.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://owo.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://umv.316326.xyz

[U28] Py：类型别名
来源：http://byw.hywenlv.cn

UserId = int
来源：http://dvd.hnqzz.top

[U29] Py：属性校验
来源：http://qgl.gzhubu.top

@property 与 @x.setter 配合
来源：http://ajo.dianchejie.cn

[U30] Py：数据类
来源：http://jce.hammf.cn

@dataclass(slots=True)
来源：http://tvv.daxiang520.top

[U31] Py：单测
来源：http://tyk.hcnkem.com

python -m pytest -q
来源：http://pwb.hywenlv.cn

[U32] Py：代码格式化
来源：http://wcw.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://dyi.feifeiyinyue.top

[U33] Py：打包发布
来源：http://ntb.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://yyl.zycfv.cn

[U34] Py：判断编码
来源：http://ntk.jianghu66.top

chardet.detect(raw)
来源：http://jhe.uphjek.com

[U35] Py：发送邮件
来源：http://ddy.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ykn.cdnleiting.top

[U36] Py：定时任务
来源：http://mso.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://ofo.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://rqo.jyoumei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://csh.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://gjh.xylfe.cn

Path(__file__).resolve().parent
来源：http://oxu.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://kvj.jiagoushi.top

sys.stdout.isatty()
来源：http://yrp.jqgufenzy.top

[U40] Py：打印到标准错误
来源：http://kzu.mhx1999.top

print("err", file=sys.stderr)
来源：http://szh.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://ulc.jyoumei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yin.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://igh.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lbw.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://vzr.kuanghao11.cn

namespace App\Http;
来源：http://kqx.ydzc1.top

[U44] PHP：开启严格类型
来源：http://ycn.cashguo.top

declare(strict_types=1);
来源：http://kid.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://ndf.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jcn.wangdashe.top

[U46] PHP：可空类型
来源：http://fuu.guowangkeji.top

?string $name = null
来源：http://yct.hesvh.cn


<!-- 参考信息 -->