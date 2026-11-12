代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://xrs.jinqigufen.top

[S23] C：随机数
来源：http://mni.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nyi.gaohongyu789.top

[S24] C：获取本地时间
来源：http://cbd.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nqf.bbcook.cn

[S25] C：内存拷贝
来源：http://cmf.yvedp.cn

memcpy(dst, src, n);
来源：http://oyq.shanyushiyangtech.top

[S26] C：内存清零
来源：http://nhr.fzhhl.top

memset(a, 0, sizeof a);
来源：http://upa.sufxvd.cn

[S27] C：定义常量
来源：http://zyc.svipenyu.cn

const double PI = 3.14159;
来源：http://kbu.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://cax.jqgufenzy.top

static int counter = 0;
来源：http://fsc.yvedp.cn

[S29] C：变参函数
来源：http://exu.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cjc.jyoumei.cn

[S30] C：头文件保护
来源：http://pab.vqdsnc.cn

#ifndef X_H
来源：http://sny.cqqwz.cn

#define X_H
来源：http://cmq.9152youxi.cn

#endif
来源：http://zzk.bjfxy.top

[S31] C++：Hello World
来源：http://ajd.xylfe.cn

#include <iostream>
来源：http://ews.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://dmt.pycfn.com

[S32] C++：字符串
来源：http://pei.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://zic.jqgfzy.top

[S33] C++：vector 增删
来源：http://pnb.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lis.yj20258888.top

[S34] C++：遍历 vector
来源：http://cmc.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://oty.jinqigfzy.top

[S35] C++：map
来源：http://dbj.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqp.cdnleiting.top

[S36] C++：unordered_map
来源：http://qby.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nvx.hammf.cn

[S37] C++：set
来源：http://bik.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rzu.nwbrower.top

[S38] C++：排序
来源：http://dss.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://amj.cashguo.top

[S39] C++：自定义比较器排序
来源：http://lqg.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gzn.hammf.cn

[S40] C++：查找元素
来源：http://vmc.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://edk.mhx1999.top

[S41] C++：类与构造函数
来源：http://kxs.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zrk.hnqzz.top

[S42] C++：继承与虚函数
来源：http://tzk.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://vgw.zhijiandao.cn

[S43] C++：智能指针
来源：http://qwu.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://hme.sjlbkw.cn

[S44] C++：引用传参
来源：http://gfk.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://uca.sjlbkw.cn

[S45] C++：lambda
来源：http://iku.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://jmd.aibaodan.cn

[S46] C++：函数模板
来源：http://kah.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://auo.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://etj.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oua.yongpay.top

[S48] C++：逐行读文件
来源：http://dod.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://upj.sysykeji.top

while (std::getline(in, line)) { }
来源：http://lnp.pycfn.com

[S49] C++：写文件
来源：http://ung.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhl.yuanzhike.top

[S50] C++：格式化数字
来源：http://lno.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://men.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://lur.shuidangran.top

static_cast<double>(a) / b
来源：http://jsd.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://rme.yj20258.top

int size() const noexcept { return n_; }
来源：http://jrf.tianlin.xyz

[S53] C++：移动语义
来源：http://qgt.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://xij.yangfankeji.com

[S54] C++：异常处理
来源：http://rmm.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hkw.chenlongwang.top

[S55] C++：结构化绑定
来源：http://giu.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bjz.jqgfzy.top

[S56] C++：optional
来源：http://fjf.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyz.fengsongda.top

[S57] C++：编译期常量
来源：http://erp.cdnleiting.top

constexpr int N = 10;
来源：http://xcr.hesvh.cn

[S58] C++：命名空间
来源：http://aft.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://daw.xziqi.cn

[S59] C++：静态断言
来源：http://bbg.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cxg.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://sad.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://icx.jianghu66.top

================================================================================
来源：http://vds.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pid.0kj1m.cn

================================================================================
来源：http://hvp.yj20258.top

[T01] Kotlin：Hello World
来源：http://xvd.shangyingyoupin.top

println("Hello")
来源：http://uup.gzhubu.top

[T02] Kotlin：变量
来源：http://xny.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xvp.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://ysu.ywan-chungtsiang.top

"值: $b"
来源：http://gfv.hysaishi.cn

[T04] Kotlin：空安全
来源：http://wxm.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://azy.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://juh.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jms.316326.xyz

[T06] Kotlin：集合映射
来源：http://jqg.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rao.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://ayu.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qlo.yongpay.top

[T08] Kotlin：数据类
来源：http://yqz.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://vrr.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://jtv.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://yeb.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://gub.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bxb.gzhubu.top

[T11] Kotlin：协程
来源：http://loy.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://umv.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://ktg.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://brl.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://sqd.hammf.cn

val m = mapOf("a" to 1)
来源：http://ehu.nanxuanxn.top

[T14] Kotlin：循环
来源：http://vch.nanxinkj.top

for (i in 1..10) println(i)
来源：http://uxj.meibo888.top

[T15] Kotlin：接口
来源：http://yul.tian-w.cn

interface Shape { fun area(): Double }
来源：http://jae.birdmap.top

[T16] Swift：Hello World
来源：http://ehs.hcnkem.com

print("Hello")
来源：http://smf.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://frr.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://nji.fehbvm.com

[T18] Swift：字符串插值
来源：http://fwe.chenlongwang.top

"值: \(b)"
来源：http://whz.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://ajj.9152youxi.cn

if let n = opt { print(n) }
来源：http://rwl.daria6918.cn

[T20] Swift：数组操作
来源：http://pke.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://bjw.gzhubu.top

[T21] Swift：遍历
来源：http://qph.shuidangran.top

for x in a { print(x) }
来源：http://vpg.gotoacloud.top

[T22] Swift：字典
来源：http://hui.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://ziy.sjlbkw.cn

[T23] Swift：函数
来源：http://gfu.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ivb.ybcxt.top

[T24] Swift：闭包
来源：http://bja.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ixe.havefunace.top

[T25] Swift：结构体
来源：http://unv.nanxinkj.top

struct P { var x: Int }
来源：http://ffo.aizwys.cn

[T26] Swift：类与重写
来源：http://nsp.zdbjq.cn

class A: Base { override func f() {} }
来源：http://lkq.yvedp.cn

[T27] Swift：错误处理
来源：http://aig.havefunace.top

do { try f() } catch { print(error) }
来源：http://kvf.gzhubu.top

[T28] Swift：枚举
来源：http://dwc.cdnleiting.top

enum Color { case red, green }
来源：http://nbg.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://qth.jyoumei.cn

guard let x = opt else { return }
来源：http://auj.feifeiyinyue.top

[T30] Swift：协议
来源：http://xxo.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://gec.chenlongwang.top

[T31] Lua：Hello World
来源：http://dpf.meibo888.top

print("Hello")
来源：http://mmx.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://cnu.shzxlz.cn

local a = 1
来源：http://lcl.svipenyu.cn

[T33] Lua：表（数组）
来源：http://xdj.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://glq.ydzc1.top

[T34] Lua：遍历表
来源：http://dqe.zhiwuduotai.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bss.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://frb.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://nto.zycfv.cn

[T36] Lua：函数
来源：http://hhe.hysaishi.cn

function add(a, b) return a + b end
来源：http://puj.chenzaomai.com

[T37] Lua：字符串拼接
来源：http://cts.zhixingplan.top

"a" .. "b"
来源：http://dbh.yuxming.cn

[T38] Lua：条件
来源：http://hwc.birdmap.top

if x > 0 then print("正") end
来源：http://pqu.jinqigufen.top

[T39] Lua：模式匹配
来源：http://ksl.wangdashe.top

string.find(s, "%d+")
来源：http://jdj.hnxiangtu.top

[T40] Lua：元表
来源：http://gla.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://hbj.tian-w.cn

[T41] Perl：Hello World
来源：http://gyw.sjlbkw.cn

print "Hello\n";
来源：http://eao.cqqwz.cn

[T42] Perl：变量类型
来源：http://fdk.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://goc.tianlin.xyz

[T43] Perl：字符串插值
来源：http://nus.yj202588.top

"值: $a"
来源：http://sin.aizwys.cn

[T44] Perl：条件
来源：http://sig.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://bqz.birdmap.top

[T45] Perl：数组遍历
来源：http://phs.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://xga.jyoumei.cn

[T46] Perl：哈希操作
来源：http://mjv.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pxo.xuanzx.com

[T47] Perl：正则捕获
来源：http://mcp.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://his.zhixingplan.top

[T48] Perl：正则替换
来源：http://tni.svipenyu.cn

$s =~ s/old/new/g;
来源：http://kmv.cheryme.top

[T49] Perl：函数
来源：http://lpd.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mkc.316326.xyz

[T50] Perl：逐行读文件
来源：http://jdg.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qxp.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://wkw.wangdashe.top

[T51] Scala：Hello World
来源：http://ivw.daria6918.cn

println("Hello")
来源：http://fik.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://lbw.quarkkingdee.top

val a = 1;  var b = 2
来源：http://nwp.hnqzz.top

[T53] Scala：字符串插值
来源：http://rwg.ppjwa.cn

s"值: $b"
来源：http://nwu.cdnleiting.top

[T54] Scala：集合映射
来源：http://oqo.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://atx.xylfe.cn

[T55] Scala：集合过滤
来源：http://xue.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://fdw.sysykeji.top

[T56] Scala：样例类
来源：http://jqj.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://enr.iojbl.cn

[T57] Scala：模式匹配
来源：http://huo.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://qhw.jinqigfzy.top

[T58] Scala：函数定义
来源：http://bxl.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jrj.yj20258.top

[T59] Scala：循环
来源：http://qgb.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://yho.daria6918.cn

[T60] Scala：折叠
来源：http://oom.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aah.zhengqikj.top

================================================================================
来源：http://sxj.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vim.ctjpmb.com

================================================================================
来源：http://uqn.guannengcc.top

[U01] Py：创建虚拟环境
来源：http://xsk.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vls.yanxiufei.cn

[U02] Py：导出 / 安装依赖
来源：http://fau.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sxr.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://nty.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jhy.gzhubu.top

[U04] Py：变量调试打印
来源：http://acj.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nlb.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://pkz.yj202588.top

list(dict.fromkeys(arr))
来源：http://atj.gogol.net.cn

[U06] Py：合并两个字典
来源：http://oka.jinghuilouyu.cn

{**a, **b}
来源：http://xxl.yuanzhike.top

[U07] Py：反转字典键值
来源：http://ema.guannengcc.top

{v: k for k, v in d.items()}
来源：http://rqi.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://obi.ehwqpu.com

[y for x in nested for y in x]
来源：http://xki.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://ugm.sxryk.cn

max(d, key=d.get)
来源：http://hpp.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://lnq.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qae.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://ryv.jinqigufen.top

(x * 2 for x in arr)
来源：http://vyw.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://qtp.yongpay.top

Counter(arr).most_common(3)
来源：http://qua.fengsongda.top

[U13] Py：固定长度队列
来源：http://yhx.shanyushiyangtech.top

deque(maxlen=10)
来源：http://tmy.hongshengwenyu.top

[U14] Py：分组收集到列表
来源：http://kta.52xcode.cn

defaultdict(list)
来源：http://agg.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://dls.sysykeji.top

t = time.perf_counter()
来源：http://hyg.daria6918.cn

[U16] Py：命令行参数解析
来源：http://fis.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iic.daxiang520.top

[U17] Py：初始化日志
来源：http://pwu.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://rbv.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://nqu.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://uct.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://ueo.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://euf.fehbvm.com

[U20] Py：缓存函数结果
来源：http://qez.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://sst.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://wwb.cashguo.top

@contextlib.contextmanager
来源：http://gsm.haohaochexian.top

[U22] Py：矩阵转置
来源：http://grl.hnxiangtu.top

list(zip(*m))
来源：http://tsp.iojbl.cn

[U23] Py：分块读取大文件
来源：http://qpo.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vgr.ehwqpu.com

[U24] Py：路径操作
来源：http://txv.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rmp.316326.xyz

[U25] Py：CSV 按字典读
来源：http://bzf.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://vop.ehwqpu.com

[U26] Py：并发下载
来源：http://gjx.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kse.yongpay.top

[U27] Py：异步 HTTP
来源：http://ohl.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://wpa.yanxiufei.cn

[U28] Py：类型别名
来源：http://erh.nanxinkj.top

UserId = int
来源：http://xbm.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://tvj.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://pww.hfpthk.cn

[U30] Py：数据类
来源：http://nny.epnwcf.com

@dataclass(slots=True)
来源：http://zcb.xinyue.icu

[U31] Py：单测
来源：http://ztp.yonumen.top

python -m pytest -q
来源：http://ysj.sxryk.cn

[U32] Py：代码格式化
来源：http://zox.shanyushiyangtech.top

ruff format . && ruff check --fix .
来源：http://wub.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://nce.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://vyf.quarkkingdee.top

[U34] Py：判断编码
来源：http://ifd.cdnleiting.top

chardet.detect(raw)
来源：http://jrp.yangfankeji.com

[U35] Py：发送邮件
来源：http://svv.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hzn.cashguo.top

[U36] Py：定时任务
来源：http://clg.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://emc.cheryme.top

[U37] Py：读写 Excel
来源：http://nsb.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://xyt.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://loj.smart0.xyz

Path(__file__).resolve().parent
来源：http://mqv.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://nsp.zdqjudy.top

sys.stdout.isatty()
来源：http://cbd.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://iji.xuanzx.com

print("err", file=sys.stderr)
来源：http://dhs.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://lvk.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xxv.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://zzo.hysaishi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ggy.redwolf501.top

[U43] PHP：声明命名空间
来源：http://yai.birdmap.top

namespace App\Http;
来源：http://uza.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://koc.yfazqb.com

declare(strict_types=1);
来源：http://qbj.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://ngz.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jcf.dianchejie.cn

[U46] PHP：可空类型
来源：http://jcn.birdmap.top

?string $name = null
来源：http://tiz.hfpthk.cn


<!-- 参考信息 -->