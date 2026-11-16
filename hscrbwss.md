代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nuv.epnwcf.com

[S25] C：内存拷贝
来源：http://fzi.xziqi.cn

memcpy(dst, src, n);
来源：http://aqu.chenlongwang.top

[S26] C：内存清零
来源：http://qtu.xuanzx.com

memset(a, 0, sizeof a);
来源：http://gwp.vehdjk.com

[S27] C：定义常量
来源：http://hdi.uphjek.com

const double PI = 3.14159;
来源：http://gcp.sysykeji.top

[S28] C：静态变量
来源：http://wbe.fehbvm.com

static int counter = 0;
来源：http://pxk.xylfe.cn

[S29] C：变参函数
来源：http://bog.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sxs.yvedp.cn

[S30] C：头文件保护
来源：http://bxm.316326.xyz

#ifndef X_H
来源：http://uxl.daria6918.cn

#define X_H
来源：http://btv.chenlongwang.top

#endif
来源：http://bpj.jinqigufen.top

[S31] C++：Hello World
来源：http://lzb.cashguo.top

#include <iostream>
来源：http://rtb.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://hgr.ydzc1.top

[S32] C++：字符串
来源：http://wwi.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://fcj.hcnkem.com

[S33] C++：vector 增删
来源：http://bbo.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uae.guowangkeji.top

[S34] C++：遍历 vector
来源：http://bfc.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://cqz.chenjidiqi.icu

[S35] C++：map
来源：http://trs.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hdm.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://sqv.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ixc.sxryk.cn

[S37] C++：set
来源：http://ucu.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ver.yanxiufei.cn

[S38] C++：排序
来源：http://hxt.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://ucw.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://laj.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vlc.hammf.cn

[S40] C++：查找元素
来源：http://olf.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nfh.wangdashe.top

[S41] C++：类与构造函数
来源：http://lwc.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fty.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://wmf.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://rtm.sweek.top

[S43] C++：智能指针
来源：http://qai.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://uik.52xcode.cn

[S44] C++：引用传参
来源：http://heu.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://fsf.zhoulong.xyz

[S45] C++：lambda
来源：http://fkm.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://ozc.guannengcc.top

[S46] C++：函数模板
来源：http://vlw.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tlj.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://adr.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lia.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://geh.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fto.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://aoe.ybcxt.top

[S49] C++：写文件
来源：http://cfa.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://esv.yanxiufei.cn

[S50] C++：格式化数字
来源：http://ese.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://phl.yongpay.top

[S51] C++：显式类型转换
来源：http://yxz.hysaishi.cn

static_cast<double>(a) / b
来源：http://mjr.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://lwx.meibo888.top

int size() const noexcept { return n_; }
来源：http://bku.smart0.xyz

[S53] C++：移动语义
来源：http://ohl.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://ofq.uphjek.com

[S54] C++：异常处理
来源：http://kfd.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ewh.bjfxy.top

[S55] C++：结构化绑定
来源：http://pyf.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lda.dashuyun.cn

[S56] C++：optional
来源：http://ilx.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ggo.yj202588.top

[S57] C++：编译期常量
来源：http://wqa.yueranfly.top

constexpr int N = 10;
来源：http://xte.shuidangran.top

[S58] C++：命名空间
来源：http://ayf.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://xxo.wangdashe.top

[S59] C++：静态断言
来源：http://yyz.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ysg.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://mih.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qft.gotoacloud.top

================================================================================
来源：http://esy.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tlh.feifeiyinyue.top

================================================================================
来源：http://zkd.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://exu.bbcook.cn

println("Hello")
来源：http://dtv.aibaodan.cn

[T02] Kotlin：变量
来源：http://ztp.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gob.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://tpa.quarkkingdee.top

"值: $b"
来源：http://gyv.ppjwa.cn

[T04] Kotlin：空安全
来源：http://ofu.ehwqpu.com

val n: String? = null;  n?.length
来源：http://gzp.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://udw.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tcm.sysykeji.top

[T06] Kotlin：集合映射
来源：http://sfr.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hxx.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://euc.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://waw.yj202588.top

[T08] Kotlin：数据类
来源：http://bqc.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://zhy.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://vdm.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://vju.aizwys.cn

[T10] Kotlin：默认参数
来源：http://vxk.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://pra.yfazqb.com

[T11] Kotlin：协程
来源：http://vto.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xsh.meibo888.top

[T12] Kotlin：解构声明
来源：http://lvp.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://wvi.cheryme.top

[T13] Kotlin：只读 Map
来源：http://rwh.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://czc.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://bzs.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://mdo.sweek.top

[T15] Kotlin：接口
来源：http://uqk.ybcxt.top

interface Shape { fun area(): Double }
来源：http://ohb.bbcook.cn

[T16] Swift：Hello World
来源：http://phs.xinyue.icu

print("Hello")
来源：http://jkk.jqgfzy.top

[T17] Swift：变量与常量
来源：http://dgy.zhengqikj.top

var a = 1;  let b = 2
来源：http://nlp.sufxvd.cn

[T18] Swift：字符串插值
来源：http://jnz.andypj.xyz

"值: \(b)"
来源：http://ypm.guannengcc.top

[T19] Swift：可选绑定
来源：http://xvs.nwbrower.top

if let n = opt { print(n) }
来源：http://acc.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://yfh.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rjl.ivvv.top

[T21] Swift：遍历
来源：http://vge.quarkkingdee.top

for x in a { print(x) }
来源：http://lyq.zhengqikj.top

[T22] Swift：字典
来源：http://pqt.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://lat.shangyingyoupin.top

[T23] Swift：函数
来源：http://pzn.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zoe.zhoulong.xyz

[T24] Swift：闭包
来源：http://uvv.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ond.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://zya.snrcjt.cn

struct P { var x: Int }
来源：http://tfc.cucudq.cn

[T26] Swift：类与重写
来源：http://ufg.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://aus.bbcook.cn

[T27] Swift：错误处理
来源：http://tpw.daria6918.cn

do { try f() } catch { print(error) }
来源：http://ukn.nwbrower.top

[T28] Swift：枚举
来源：http://xrf.tian-w.cn

enum Color { case red, green }
来源：http://qkz.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://unt.zhixingplan.top

guard let x = opt else { return }
来源：http://fei.gogol.net.cn

[T30] Swift：协议
来源：http://iym.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://hqi.ydjk.org.cn

[T31] Lua：Hello World
来源：http://cri.jinghuilouyu.cn

print("Hello")
来源：http://ghb.hnqzz.top

[T32] Lua：局部变量
来源：http://kwc.xinyue.icu

local a = 1
来源：http://mik.tianlin.xyz

[T33] Lua：表（数组）
来源：http://klu.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pzk.nwbrower.top

[T34] Lua：遍历表
来源：http://pqo.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://bbn.smart0.xyz

[T35] Lua：字典表
来源：http://mro.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://ksq.nanxuanxn.top

[T36] Lua：函数
来源：http://ych.xziqi.cn

function add(a, b) return a + b end
来源：http://zdg.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://urq.zdbjq.cn

"a" .. "b"
来源：http://hjq.sufxvd.cn

[T38] Lua：条件
来源：http://tdp.gaohongyu789.top

if x > 0 then print("正") end
来源：http://pep.daria6918.cn

[T39] Lua：模式匹配
来源：http://bqo.ybcxt.top

string.find(s, "%d+")
来源：http://rhi.zhengqikj.top

[T40] Lua：元表
来源：http://jla.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://kar.gzhubu.top

[T41] Perl：Hello World
来源：http://obt.shangyingyoupin.top

print "Hello\n";
来源：http://bmi.hysaishi.cn

[T42] Perl：变量类型
来源：http://ozt.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fou.chenzaomai.com

[T43] Perl：字符串插值
来源：http://ujh.guannengcc.top

"值: $a"
来源：http://wau.nanxuanxn.top

[T44] Perl：条件
来源：http://lfy.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://ype.gotoacloud.top

[T45] Perl：数组遍历
来源：http://btn.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://qgv.ctjpmb.com

[T46] Perl：哈希操作
来源：http://gsw.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://twe.gotoacloud.top

[T47] Perl：正则捕获
来源：http://rhz.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bnf.zhixingplan.top

[T48] Perl：正则替换
来源：http://fvq.xylfe.cn

$s =~ s/old/new/g;
来源：http://qgi.chenzaomai.com

[T49] Perl：函数
来源：http://kyx.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fxf.tian-w.cn

[T50] Perl：逐行读文件
来源：http://xha.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://faf.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://xam.zdbjq.cn

[T51] Scala：Hello World
来源：http://yup.c1oappe.top

println("Hello")
来源：http://pcb.meibo888.top

[T52] Scala：变量
来源：http://ihs.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://mkj.redwolf501.top

[T53] Scala：字符串插值
来源：http://qfp.yongpay.top

s"值: $b"
来源：http://awl.c1oappe.top

[T54] Scala：集合映射
来源：http://nqd.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://bks.tian-w.cn

[T55] Scala：集合过滤
来源：http://wox.bbcook.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mpl.ctjpmb.com

[T56] Scala：样例类
来源：http://cnk.ppjwa.cn

case class User(name: String, age: Int)
来源：http://qze.redwolf501.top

[T57] Scala：模式匹配
来源：http://jku.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://bnk.gogol.net.cn

[T58] Scala：函数定义
来源：http://wki.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://ifo.ydzc1.top

[T59] Scala：循环
来源：http://ctf.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://xbi.hesvh.cn

[T60] Scala：折叠
来源：http://zul.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cdq.chenlongwang.top

================================================================================
来源：http://rnq.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yyl.kuanghao11.cn

================================================================================
来源：http://nea.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://iwu.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://lbi.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://vjm.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwz.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://fjv.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vod.daxiang520.top

[U04] Py：变量调试打印
来源：http://dnx.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pca.cucudq.cn

[U05] Py：列表去重且保序
来源：http://ufs.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://onp.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://glg.wangdashe.top

{**a, **b}
来源：http://fus.fktsv.cn

[U07] Py：反转字典键值
来源：http://vma.bjfxy.top

{v: k for k, v in d.items()}
来源：http://aec.316326.xyz

[U08] Py：展平二维列表
来源：http://mvi.gogol.net.cn

[y for x in nested for y in x]
来源：http://mod.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://gxj.yongpay.top

max(d, key=d.get)
来源：http://aic.tarul.cn

[U10] Py：按值排序字典
来源：http://pvq.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dua.dashuyun.cn

[U11] Py：生成器表达式
来源：http://pyl.yuxming.cn

(x * 2 for x in arr)
来源：http://uwb.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://sbb.gotoacloud.top

Counter(arr).most_common(3)
来源：http://vxp.hammf.cn

[U13] Py：固定长度队列
来源：http://yeo.yuanzhike.top

deque(maxlen=10)
来源：http://tkr.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://wgb.sufxvd.cn

defaultdict(list)
来源：http://iid.bbcook.cn

[U15] Py：高精度计时
来源：http://xae.yuanzhike.top

t = time.perf_counter()
来源：http://zeb.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://aea.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zgb.zhixingplan.top

[U17] Py：初始化日志
来源：http://wyv.bjfxy.top

logging.basicConfig(level=logging.INFO)
来源：http://jiu.nwbrower.top

[U18] Py：预编译正则
来源：http://voe.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://peq.andypj.xyz

[U19] Py：正则替换带回调
来源：http://pkl.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgy.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://fkq.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://zvi.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://dku.shuidangran.top

@contextlib.contextmanager
来源：http://fhb.dianchejie.cn

[U22] Py：矩阵转置
来源：http://hsb.xinyue.icu

list(zip(*m))
来源：http://tpb.vehdjk.com

[U23] Py：分块读取大文件
来源：http://wxh.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fjc.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://ztz.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xnq.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://qdh.shuidangran.top

csv.DictReader(f)
来源：http://gnd.wangshuangyany.cn

[U26] Py：并发下载
来源：http://cpc.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rjn.sweek.top

[U27] Py：异步 HTTP
来源：http://klu.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://woa.andypj.xyz

[U28] Py：类型别名
来源：http://nfa.wangshuangyany.cn

UserId = int
来源：http://hcg.jinqigfzy.top

[U29] Py：属性校验
来源：http://egr.cucudq.cn

@property 与 @x.setter 配合
来源：http://qza.tarul.cn

[U30] Py：数据类
来源：http://pzy.sweek.top

@dataclass(slots=True)
来源：http://txa.tanke756.top

[U31] Py：单测
来源：http://czf.dianchejie.cn

python -m pytest -q
来源：http://wbv.iojbl.cn

[U32] Py：代码格式化
来源：http://rnn.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://pvl.9152youxi.cn

[U33] Py：打包发布
来源：http://uhp.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://gex.pycfn.com

[U34] Py：判断编码
来源：http://gng.0kj1m.cn

chardet.detect(raw)
来源：http://spc.jqgfzy.top

[U35] Py：发送邮件
来源：http://zpw.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://est.yangfankeji.com

[U36] Py：定时任务
来源：http://lga.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://zgt.yangfankeji.com

[U37] Py：读写 Excel
来源：http://zpg.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hmu.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://lha.52xcode.cn

Path(__file__).resolve().parent
来源：http://fto.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://tpw.cheryme.top

sys.stdout.isatty()
来源：http://oct.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://vjz.yj20258.top

print("err", file=sys.stderr)
来源：http://qjv.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://wbn.yj202588.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ryb.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://lxq.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jhm.hammf.cn

[U43] PHP：声明命名空间
来源：http://wit.zdqjudy.top

namespace App\Http;
来源：http://aik.tanke756.top

[U44] PHP：开启严格类型
来源：http://iha.0kj1m.cn

declare(strict_types=1);
来源：http://zlt.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://cjz.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gxd.shzxlz.cn

[U46] PHP：可空类型
来源：http://nln.xuanzx.com

?string $name = null
来源：http://pfk.jianghu66.top

[U47] PHP：联合类型
来源：http://plg.sxryk.cn

int|string $id
来源：http://fmo.shuidangran.top

[U48] PHP：纯枚举
来源：http://cly.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uqo.tanke756.top


<!-- 参考信息 -->