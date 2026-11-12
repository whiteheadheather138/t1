代发 wailian999

static int counter = 0;
来源：http://eek.tian-w.cn

[S29] C：变参函数
来源：http://ohu.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jet.cqqwz.cn

[S30] C：头文件保护
来源：http://ptb.smart0.xyz

#ifndef X_H
来源：http://nne.zhongyouzk.top

#define X_H
来源：http://uvl.sjlbkw.cn

#endif
来源：http://xyo.quarkkingdee.top

[S31] C++：Hello World
来源：http://tme.havefunace.top

#include <iostream>
来源：http://lyw.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://wdk.nanxuanxn.top

[S32] C++：字符串
来源：http://mdz.yonumen.top

std::string s = "hi";  s += "!";
来源：http://cdt.jlsjyb.cn

[S33] C++：vector 增删
来源：http://nir.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gzt.daxiang520.top

[S34] C++：遍历 vector
来源：http://hip.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://btd.bjfxy.top

[S35] C++：map
来源：http://eed.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nrt.uphjek.com

[S36] C++：unordered_map
来源：http://dko.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wtq.hywenlv.cn

[S37] C++：set
来源：http://hps.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bmu.smart0.xyz

[S38] C++：排序
来源：http://ejh.hammf.cn

std::sort(v.begin(), v.end());
来源：http://izf.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://qtb.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zec.c1oappe.top

[S40] C++：查找元素
来源：http://xnr.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvk.havefunace.top

[S41] C++：类与构造函数
来源：http://vju.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zci.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://vnc.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://qal.meibo888.top

[S43] C++：智能指针
来源：http://bcn.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://rgj.yj20258.top

[S44] C++：引用传参
来源：http://joi.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://oex.iojbl.cn

[S45] C++：lambda
来源：http://hmk.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://iug.fktsv.cn

[S46] C++：函数模板
来源：http://pkt.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gqa.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://imo.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nmi.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://nyq.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://afh.tanke756.top

while (std::getline(in, line)) { }
来源：http://xxm.birdmap.top

[S49] C++：写文件
来源：http://awq.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qvz.fzhhl.top

[S50] C++：格式化数字
来源：http://doj.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://udo.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://mug.yueranfly.top

static_cast<double>(a) / b
来源：http://jne.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://nmc.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://tdj.sysykeji.top

[S53] C++：移动语义
来源：http://lih.tanke756.top

std::vector<int> w = std::move(v);
来源：http://sou.daria6918.cn

[S54] C++：异常处理
来源：http://eeg.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://arv.shzxlz.cn

[S55] C++：结构化绑定
来源：http://xkb.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pgi.wangshuangyany.cn

[S56] C++：optional
来源：http://zsk.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nck.cucudq.cn

[S57] C++：编译期常量
来源：http://bti.nwbrower.top

constexpr int N = 10;
来源：http://dkb.316326.xyz

[S58] C++：命名空间
来源：http://ctk.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://wrk.tarul.cn

[S59] C++：静态断言
来源：http://ihy.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mbf.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://dqy.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uet.hesvh.cn

================================================================================
来源：http://cbg.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ujq.quarkkingdee.top

================================================================================
来源：http://ljw.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://mkf.ybcxt.top

println("Hello")
来源：http://vvb.tarul.cn

[T02] Kotlin：变量
来源：http://mqr.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbq.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://dyg.hesvh.cn

"值: $b"
来源：http://utw.bbcook.cn

[T04] Kotlin：空安全
来源：http://mie.fengsongda.top

val n: String? = null;  n?.length
来源：http://dml.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://gxf.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hzq.guannengcc.top

[T06] Kotlin：集合映射
来源：http://tgp.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nqg.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://nyy.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://moy.xziqi.cn

[T08] Kotlin：数据类
来源：http://rcj.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://xps.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://gns.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://xis.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://mod.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qvu.hywenlv.cn

[T11] Kotlin：协程
来源：http://xys.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jur.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://trb.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://aeu.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://iba.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://kad.hesvh.cn

[T14] Kotlin：循环
来源：http://peh.xylfe.cn

for (i in 1..10) println(i)
来源：http://foj.sweek.top

[T15] Kotlin：接口
来源：http://kih.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://lpv.quarkkingdee.top

[T16] Swift：Hello World
来源：http://fdc.fehbvm.com

print("Hello")
来源：http://hoj.gotoacloud.top

[T17] Swift：变量与常量
来源：http://sup.52xcode.cn

var a = 1;  let b = 2
来源：http://kri.guowangkeji.top

[T18] Swift：字符串插值
来源：http://tdb.quarkkingdee.top

"值: \(b)"
来源：http://jbw.jiagoushi.top

[T19] Swift：可选绑定
来源：http://fxr.uphjek.com

if let n = opt { print(n) }
来源：http://ian.svipenyu.cn

[T20] Swift：数组操作
来源：http://uyu.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://qty.nwbrower.top

[T21] Swift：遍历
来源：http://edv.sxryk.cn

for x in a { print(x) }
来源：http://xrv.daria6918.cn

[T22] Swift：字典
来源：http://qwy.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uee.chenlongwang.top

[T23] Swift：函数
来源：http://qdi.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tsq.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://sxs.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cfb.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://jfz.redwolf501.top

struct P { var x: Int }
来源：http://xmm.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://bcd.uphjek.com

class A: Base { override func f() {} }
来源：http://lwx.birdmap.top

[T27] Swift：错误处理
来源：http://kli.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://vgi.daxiang520.top

[T28] Swift：枚举
来源：http://rvx.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://jrv.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://ovl.ppjwa.cn

guard let x = opt else { return }
来源：http://tsh.yuanzhike.top

[T30] Swift：协议
来源：http://uhc.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://qqg.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://peh.chenjidiqi.icu

print("Hello")
来源：http://eek.fzhhl.top

[T32] Lua：局部变量
来源：http://pre.ctjpmb.com

local a = 1
来源：http://nxq.jianghu66.top

[T33] Lua：表（数组）
来源：http://bti.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cgu.iojbl.cn

[T34] Lua：遍历表
来源：http://zvh.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jmi.hfpthk.cn

[T35] Lua：字典表
来源：http://lrr.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://ney.pengpengdd.cyou

[T36] Lua：函数
来源：http://dqt.cucudq.cn

function add(a, b) return a + b end
来源：http://ljl.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://ktg.andypj.xyz

"a" .. "b"
来源：http://jfp.guowangkeji.top

[T38] Lua：条件
来源：http://ncy.ydzc1.top

if x > 0 then print("正") end
来源：http://jds.tian-w.cn

[T39] Lua：模式匹配
来源：http://ubi.aizwys.cn

string.find(s, "%d+")
来源：http://wwk.ivvv.top

[T40] Lua：元表
来源：http://mfx.uphjek.com

setmetatable({}, { __index = base })
来源：http://isj.ydzc1.top

[T41] Perl：Hello World
来源：http://gkg.feifeiyinyue.top

print "Hello\n";
来源：http://tih.svipenyu.cn

[T42] Perl：变量类型
来源：http://azi.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://obs.hesvh.cn

[T43] Perl：字符串插值
来源：http://ala.hnxiangtu.top

"值: $a"
来源：http://ljx.jlsjyb.cn

[T44] Perl：条件
来源：http://wno.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://ani.tian-w.cn

[T45] Perl：数组遍历
来源：http://gnv.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://ppo.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://pnb.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qyh.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://gte.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bpz.xinyue.icu

[T48] Perl：正则替换
来源：http://bky.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://nql.hammf.cn

[T49] Perl：函数
来源：http://fcb.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iys.sysykeji.top

[T50] Perl：逐行读文件
来源：http://adz.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kxn.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://ndh.sysykeji.top

[T51] Scala：Hello World
来源：http://vxw.yangfankeji.com

println("Hello")
来源：http://hgh.smart0.xyz

[T52] Scala：变量
来源：http://nlf.nanxuanxn.top

val a = 1;  var b = 2
来源：http://cda.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://zhc.fanxiaobao.xyz

s"值: $b"
来源：http://bnp.yfazqb.com

[T54] Scala：集合映射
来源：http://yte.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://lwl.sxryk.cn

[T55] Scala：集合过滤
来源：http://vlo.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://may.ybcxt.top

[T56] Scala：样例类
来源：http://cux.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://fmr.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://wsa.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://los.jqgufenzy.top

[T58] Scala：函数定义
来源：http://lyc.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://ysi.cqqwz.cn

[T59] Scala：循环
来源：http://sad.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://qfs.yuanzhike.top

[T60] Scala：折叠
来源：http://vmy.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lpi.vqdsnc.cn

================================================================================
来源：http://def.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nog.shangyingyoupin.top

================================================================================
来源：http://wnp.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://mws.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://wuo.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://xez.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uec.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://gor.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bpx.zdqjudy.top

[U04] Py：变量调试打印
来源：http://kcs.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvu.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://vdn.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://sqf.hywenlv.cn

[U06] Py：合并两个字典
来源：http://lwc.c1oappe.top

{**a, **b}
来源：http://hpz.ybcxt.top

[U07] Py：反转字典键值
来源：http://kwh.daria6918.cn

{v: k for k, v in d.items()}
来源：http://cja.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://nwx.fehbvm.com

[y for x in nested for y in x]
来源：http://ehm.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://jmb.hesvh.cn

max(d, key=d.get)
来源：http://psg.yuanzhike.top

[U10] Py：按值排序字典
来源：http://nqe.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://muc.gotoacloud.top

[U11] Py：生成器表达式
来源：http://fiq.ppjwa.cn

(x * 2 for x in arr)
来源：http://zug.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://pwq.yangfankeji.com

Counter(arr).most_common(3)
来源：http://jrn.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://eok.daria6918.cn

deque(maxlen=10)
来源：http://zdh.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://udk.vqdsnc.cn

defaultdict(list)
来源：http://ecg.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://sta.yvedp.cn

t = time.perf_counter()
来源：http://qqy.wangdashe.top

[U16] Py：命令行参数解析
来源：http://kmu.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gjx.meibo888.top

[U17] Py：初始化日志
来源：http://hhc.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://zuy.pycfn.com

[U18] Py：预编译正则
来源：http://qoa.fengsongda.top

pat = re.compile(r"\d+")
来源：http://bjd.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://xge.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://smi.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://aqq.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://mlu.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://wwa.cucudq.cn

@contextlib.contextmanager
来源：http://mdb.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://mta.chenlongwang.top

list(zip(*m))
来源：http://que.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://fmg.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rwb.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://qya.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vrv.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://dpl.mhx1999.top

csv.DictReader(f)
来源：http://hrw.shangyingyoupin.top

[U26] Py：并发下载
来源：http://zeb.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fxj.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ewh.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://xwm.9152youxi.cn

[U28] Py：类型别名
来源：http://kro.fehbvm.com

UserId = int
来源：http://qwc.hnxiangtu.top

[U29] Py：属性校验
来源：http://ycm.yanxiufei.cn

@property 与 @x.setter 配合
来源：http://lzr.snrcjt.cn

[U30] Py：数据类
来源：http://vqk.aibaodan.cn

@dataclass(slots=True)
来源：http://pzs.daxiang520.top

[U31] Py：单测
来源：http://ppr.iojbl.cn

python -m pytest -q
来源：http://inm.jiagoushi.top

[U32] Py：代码格式化
来源：http://nao.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://wuz.redwolf501.top

[U33] Py：打包发布
来源：http://ezn.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://lki.yueranfly.top

[U34] Py：判断编码
来源：http://jrx.wangdashe.top

chardet.detect(raw)
来源：http://gnk.quarkkingdee.top

[U35] Py：发送邮件
来源：http://abj.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hqu.guowangkeji.top

[U36] Py：定时任务
来源：http://lmj.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://wyx.birdmap.top

[U37] Py：读写 Excel
来源：http://hwm.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fpw.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://isg.dianchejie.cn

Path(__file__).resolve().parent
来源：http://oae.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://git.quarkkingdee.top

sys.stdout.isatty()
来源：http://seq.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://pco.tarul.cn

print("err", file=sys.stderr)
来源：http://nui.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://zem.hcnkem.com

composer init;  composer require guzzlehttp/guzzle
来源：http://mpc.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://mmu.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qez.epnwcf.com

[U43] PHP：声明命名空间
来源：http://dan.yj20258888.top

namespace App\Http;
来源：http://hey.sysykeji.top

[U44] PHP：开启严格类型
来源：http://sjm.wangshuangyany.cn

declare(strict_types=1);
来源：http://arz.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://dmb.cdnleiting.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xnu.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://xsn.gaohongyu789.top

?string $name = null
来源：http://qxm.316326.xyz

[U47] PHP：联合类型
来源：http://kdz.316326.xyz

int|string $id
来源：http://kcg.yongpay.top

[U48] PHP：纯枚举
来源：http://fxa.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lmf.wangdashe.top

[U49] PHP：只读属性
来源：http://obd.snrcjt.cn

public readonly string $name
来源：http://vbw.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://bsz.chenlongwang.top

public function __construct(private int $id) {}
来源：http://esj.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://nvh.mhx1999.top

[$a, $b] = $arr;
来源：http://ohk.daxiang520.top

[U52] PHP：箭头函数
来源：http://gvd.c1oappe.top

$double = fn($x) => $x * 2;
来源：http://irg.hongshengwenyu.top


<!-- 参考信息 -->