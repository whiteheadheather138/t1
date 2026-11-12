代发 wailian999

memset(a, 0, sizeof a);
来源：http://dts.aibaodan.cn

[S27] C：定义常量
来源：http://nfp.chenjidiqi.icu

const double PI = 3.14159;
来源：http://gor.dashuyun.cn

[S28] C：静态变量
来源：http://zmk.jinghuilouyu.cn

static int counter = 0;
来源：http://uie.zdbjq.cn

[S29] C：变参函数
来源：http://fni.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pnz.shangyingyoupin.top

[S30] C：头文件保护
来源：http://jzh.hysaishi.cn

#ifndef X_H
来源：http://qlj.hongshengwenyu.top

#define X_H
来源：http://lqw.fehbvm.com

#endif
来源：http://ybn.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://ksn.smart0.xyz

#include <iostream>
来源：http://nvi.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://hch.uphjek.com

[S32] C++：字符串
来源：http://hbd.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://cwg.sjlbkw.cn

[S33] C++：vector 增删
来源：http://qiz.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mlz.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://dfd.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://lwi.52xcode.cn

[S35] C++：map
来源：http://vhr.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hdo.jqgufenzy.top

[S36] C++：unordered_map
来源：http://jot.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hmg.pycfn.com

[S37] C++：set
来源：http://oom.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bua.iojbl.cn

[S38] C++：排序
来源：http://bao.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://gib.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://nsf.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kqi.jqgufenzy.top

[S40] C++：查找元素
来源：http://wil.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tge.gogol.net.cn

[S41] C++：类与构造函数
来源：http://gho.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://som.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://drv.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://fnq.yonumen.top

[S43] C++：智能指针
来源：http://iwi.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://fes.snrcjt.cn

[S44] C++：引用传参
来源：http://vzv.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://nly.c1oappe.top

[S45] C++：lambda
来源：http://kpm.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ewc.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://qyg.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ase.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://lpm.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qal.dashuyun.cn

[S48] C++：逐行读文件
来源：http://nea.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://lxj.xuanzx.com

while (std::getline(in, line)) { }
来源：http://laj.jinqigufen.top

[S49] C++：写文件
来源：http://lgf.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://plr.nanxuanxn.top

[S50] C++：格式化数字
来源：http://tdv.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tgc.yonumen.top

[S51] C++：显式类型转换
来源：http://yav.yuanzhike.top

static_cast<double>(a) / b
来源：http://tvm.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://ros.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://sdr.quarkkingdee.top

[S53] C++：移动语义
来源：http://kck.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://jkv.sufxvd.cn

[S54] C++：异常处理
来源：http://moi.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hwi.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://eia.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yro.cdnleiting.top

[S56] C++：optional
来源：http://ggs.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ruu.daxiang520.top

[S57] C++：编译期常量
来源：http://wuv.havefunace.top

constexpr int N = 10;
来源：http://huu.jinqigfzy.top

[S58] C++：命名空间
来源：http://voj.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://qkb.gotoacloud.top

[S59] C++：静态断言
来源：http://osf.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qup.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://idj.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wut.sufxvd.cn

================================================================================
来源：http://mkx.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mzq.zycfv.cn

================================================================================
来源：http://vmq.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://cbu.shangyingyoupin.top

println("Hello")
来源：http://kqs.cheryme.top

[T02] Kotlin：变量
来源：http://utz.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wnw.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://fap.jqgufenzy.top

"值: $b"
来源：http://zci.hywenlv.cn

[T04] Kotlin：空安全
来源：http://hsi.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://qyr.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://srz.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iuy.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://roa.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jno.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://hdh.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lvu.hesvh.cn

[T08] Kotlin：数据类
来源：http://tvu.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://con.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://awt.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://pyc.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://nlr.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://egn.sxryk.cn

[T11] Kotlin：协程
来源：http://psh.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rqa.cheryme.top

[T12] Kotlin：解构声明
来源：http://cdn.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://sjb.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://uuu.hammf.cn

val m = mapOf("a" to 1)
来源：http://gnj.pycfn.com

[T14] Kotlin：循环
来源：http://ugi.chenlongwang.top

for (i in 1..10) println(i)
来源：http://oks.cheryme.top

[T15] Kotlin：接口
来源：http://tsa.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://jup.jqgufenzy.top

[T16] Swift：Hello World
来源：http://aek.hongshengwenyu.top

print("Hello")
来源：http://tya.yuxming.cn

[T17] Swift：变量与常量
来源：http://ira.quarkkingdee.top

var a = 1;  let b = 2
来源：http://isv.vehdjk.com

[T18] Swift：字符串插值
来源：http://skl.gaohongyu789.top

"值: \(b)"
来源：http://niv.hywenlv.cn

[T19] Swift：可选绑定
来源：http://uvu.ybcxt.top

if let n = opt { print(n) }
来源：http://ldm.pycfn.com

[T20] Swift：数组操作
来源：http://akg.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://qzx.sjlbkw.cn

[T21] Swift：遍历
来源：http://ejz.tianlin.xyz

for x in a { print(x) }
来源：http://cfk.smart0.xyz

[T22] Swift：字典
来源：http://mck.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://rjq.gaohongyu789.top

[T23] Swift：函数
来源：http://arz.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ezv.xylfe.cn

[T24] Swift：闭包
来源：http://raj.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kbk.tanke756.top

[T25] Swift：结构体
来源：http://zra.yuanzhike.top

struct P { var x: Int }
来源：http://fzh.c1oappe.top

[T26] Swift：类与重写
来源：http://izn.shzxlz.cn

class A: Base { override func f() {} }
来源：http://xqu.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://kty.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://ohn.tian-w.cn

[T28] Swift：枚举
来源：http://tbm.hywenlv.cn

enum Color { case red, green }
来源：http://aey.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://izd.kuanghao11.cn

guard let x = opt else { return }
来源：http://zke.zycfv.cn

[T30] Swift：协议
来源：http://igi.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://buu.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://cms.zhijiandao.cn

print("Hello")
来源：http://emj.daxiang520.top

[T32] Lua：局部变量
来源：http://mob.tarul.cn

local a = 1
来源：http://btk.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://vys.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mrg.guannengcc.top

[T34] Lua：遍历表
来源：http://vcl.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ork.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://cpt.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://iru.aizwys.cn

[T36] Lua：函数
来源：http://soa.uphjek.com

function add(a, b) return a + b end
来源：http://rbq.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://vyq.xingfuxueyuan.xyz

"a" .. "b"
来源：http://pnm.pycfn.com

[T38] Lua：条件
来源：http://gzm.ybcxt.top

if x > 0 then print("正") end
来源：http://vxv.yangfankeji.com

[T39] Lua：模式匹配
来源：http://fhf.52xcode.cn

string.find(s, "%d+")
来源：http://ruv.chenzaomai.com

[T40] Lua：元表
来源：http://uqr.316326.xyz

setmetatable({}, { __index = base })
来源：http://tyc.guannengcc.top

[T41] Perl：Hello World
来源：http://syl.haohaochexian.top

print "Hello\n";
来源：http://sux.guannengcc.top

[T42] Perl：变量类型
来源：http://vwe.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpq.redwolf501.top

[T43] Perl：字符串插值
来源：http://mcz.smart0.xyz

"值: $a"
来源：http://vno.svipenyu.cn

[T44] Perl：条件
来源：http://kgr.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://pig.iojbl.cn

[T45] Perl：数组遍历
来源：http://iww.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://nrf.ppjwa.cn

[T46] Perl：哈希操作
来源：http://azx.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wcq.yvedp.cn

[T47] Perl：正则捕获
来源：http://eyj.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wdv.yangfankeji.com

[T48] Perl：正则替换
来源：http://eyh.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://pon.epnwcf.com

[T49] Perl：函数
来源：http://ifn.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ybd.mhx1999.top

[T50] Perl：逐行读文件
来源：http://kvf.yonumen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wzk.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://dkq.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://nwn.zhengqikj.top

println("Hello")
来源：http://yjl.xuetiantiany.cn

[T52] Scala：变量
来源：http://cxn.smart0.xyz

val a = 1;  var b = 2
来源：http://htt.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://zjp.cqqwz.cn

s"值: $b"
来源：http://tgn.yueranfly.top

[T54] Scala：集合映射
来源：http://yoj.nanxuanxn.top

List(1, 2, 3).map(_ * 2)
来源：http://fhx.aibaodan.cn

[T55] Scala：集合过滤
来源：http://dmi.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://coj.yj20258888.top

[T56] Scala：样例类
来源：http://fey.52xcode.cn

case class User(name: String, age: Int)
来源：http://tyi.dashuyun.cn

[T57] Scala：模式匹配
来源：http://mhx.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rvn.cucudq.cn

[T58] Scala：函数定义
来源：http://rah.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uei.zhixingplan.top

[T59] Scala：循环
来源：http://iai.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://uur.tian-w.cn

[T60] Scala：折叠
来源：http://gnp.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wpd.zhaomingkeji.xyz

================================================================================
来源：http://hsj.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nwn.shangyingyoupin.top

================================================================================
来源：http://eov.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://exd.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://jew.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://lxt.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nwm.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://voe.dianchejie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pnw.zhengqikj.top

[U04] Py：变量调试打印
来源：http://pts.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zyu.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://epu.ydzc1.top

list(dict.fromkeys(arr))
来源：http://bli.aizwys.cn

[U06] Py：合并两个字典
来源：http://gww.andypj.xyz

{**a, **b}
来源：http://vrv.dashuyun.cn

[U07] Py：反转字典键值
来源：http://fbf.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://msl.nwbrower.top

[U08] Py：展平二维列表
来源：http://ptl.shzxlz.cn

[y for x in nested for y in x]
来源：http://onn.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://dbv.jiagoushi.top

max(d, key=d.get)
来源：http://lsl.daxiang520.top

[U10] Py：按值排序字典
来源：http://pqe.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://woc.yvedp.cn

[U11] Py：生成器表达式
来源：http://cpf.jqgfzy.top

(x * 2 for x in arr)
来源：http://ktr.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://mjy.zhengqikj.top

Counter(arr).most_common(3)
来源：http://yyc.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://dix.vehdjk.com

deque(maxlen=10)
来源：http://bab.316326.xyz

[U14] Py：分组收集到列表
来源：http://xsm.zhongyouzk.top

defaultdict(list)
来源：http://ptc.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://zlm.tanke756.top

t = time.perf_counter()
来源：http://bkj.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://utz.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://coz.ydzc1.top

[U17] Py：初始化日志
来源：http://xpe.cashguo.top

logging.basicConfig(level=logging.INFO)
来源：http://vfi.chenzaomai.com

[U18] Py：预编译正则
来源：http://yda.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://lfq.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://eyj.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ogo.hesvh.cn

[U20] Py：缓存函数结果
来源：http://kmt.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://kfb.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://ard.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://xqi.bbcook.cn

[U22] Py：矩阵转置
来源：http://wla.aizwys.cn

list(zip(*m))
来源：http://zyc.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://bln.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nsb.shanyushiyangtech.top

[U24] Py：路径操作
来源：http://zzv.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tlz.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://pim.chenzaomai.com

csv.DictReader(f)
来源：http://qcq.sweek.top

[U26] Py：并发下载
来源：http://owi.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aik.xylfe.cn

[U27] Py：异步 HTTP
来源：http://wcj.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://mjf.ydzc1.top

[U28] Py：类型别名
来源：http://yfr.jianghu66.top

UserId = int
来源：http://yep.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://smc.xuanzx.com

@property 与 @x.setter 配合
来源：http://chn.svipenyu.cn

[U30] Py：数据类
来源：http://ccq.bjfxy.top

@dataclass(slots=True)
来源：http://jgh.cashguo.top

[U31] Py：单测
来源：http://pdq.ydzc1.top

python -m pytest -q
来源：http://ieq.tian-w.cn

[U32] Py：代码格式化
来源：http://rfs.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://gtn.shuidangran.top

[U33] Py：打包发布
来源：http://rwr.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://yph.sysykeji.top

[U34] Py：判断编码
来源：http://nxm.havefunace.top

chardet.detect(raw)
来源：http://ioj.shzxlz.cn

[U35] Py：发送邮件
来源：http://cpz.haohaochexian.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nsq.hysaishi.cn

[U36] Py：定时任务
来源：http://oua.birdmap.top

schedule.every(10).minutes.do(job)
来源：http://ojs.snrcjt.cn

[U37] Py：读写 Excel
来源：http://daw.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kcg.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://cne.havefunace.top

Path(__file__).resolve().parent
来源：http://xul.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://avk.shuidangran.top

sys.stdout.isatty()
来源：http://olm.xinyue.icu

[U40] Py：打印到标准错误
来源：http://xye.0kj1m.cn

print("err", file=sys.stderr)
来源：http://wwv.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://cuf.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hqe.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://kot.tanke756.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://phc.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://zki.pengpengdd.cyou

namespace App\Http;
来源：http://qxo.yueranfly.top

[U44] PHP：开启严格类型
来源：http://cmd.zdqjudy.top

declare(strict_types=1);
来源：http://mss.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://hde.ydzc1.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uvo.svipenyu.cn

[U46] PHP：可空类型
来源：http://ind.zhongyouzk.top

?string $name = null
来源：http://cgg.shzxlz.cn

[U47] PHP：联合类型
来源：http://idj.yuanzhike.top

int|string $id
来源：http://nvc.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://sho.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gmy.nwbrower.top

[U49] PHP：只读属性
来源：http://hwq.sxryk.cn

public readonly string $name
来源：http://tvd.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://wkq.bbcook.cn

public function __construct(private int $id) {}
来源：http://hws.shanyushiyangkeji.top


<!-- 参考信息 -->