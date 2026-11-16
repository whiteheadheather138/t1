代发 wailian999

#ifndef X_H
来源：http://cav.yuanzhike.top

#define X_H
来源：http://orm.cheryme.top

#endif
来源：http://lyh.zhixingplan.top

[S31] C++：Hello World
来源：http://xrp.wangshuangyany.cn

#include <iostream>
来源：http://yff.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://yka.snrcjt.cn

[S32] C++：字符串
来源：http://cnw.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://ojb.9152youxi.cn

[S33] C++：vector 增删
来源：http://rib.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://idr.sweek.top

[S34] C++：遍历 vector
来源：http://igf.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://vpc.yanxiufei.cn

[S35] C++：map
来源：http://oko.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yyr.zdbjq.cn

[S36] C++：unordered_map
来源：http://yqw.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qow.shangyingyoupin.top

[S37] C++：set
来源：http://evf.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wfy.xinyue.icu

[S38] C++：排序
来源：http://uca.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://noz.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://imi.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hoy.zdqjudy.top

[S40] C++：查找元素
来源：http://lir.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wng.meibo888.top

[S41] C++：类与构造函数
来源：http://qsu.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tzl.cashguo.top

[S42] C++：继承与虚函数
来源：http://nte.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://ort.9152youxi.cn

[S43] C++：智能指针
来源：http://krv.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://vxt.nanxinkj.top

[S44] C++：引用传参
来源：http://tww.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://bcz.aibaodan.cn

[S45] C++：lambda
来源：http://duo.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://ezi.jlsjyb.cn

[S46] C++：函数模板
来源：http://nqs.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kkv.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://ffy.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iay.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://uiw.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://tbr.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://hue.jinqigufen.top

[S49] C++：写文件
来源：http://oip.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xxc.ehwqpu.com

[S50] C++：格式化数字
来源：http://kmp.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yuv.yj20258888.top

[S51] C++：显式类型转换
来源：http://qtv.nanxuanxn.top

static_cast<double>(a) / b
来源：http://uvn.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://hyb.tarul.cn

int size() const noexcept { return n_; }
来源：http://shy.tanke756.top

[S53] C++：移动语义
来源：http://ded.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://ucs.cheryme.top

[S54] C++：异常处理
来源：http://znh.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zeo.yuxming.cn

[S55] C++：结构化绑定
来源：http://yml.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://www.hnxiangtu.top

[S56] C++：optional
来源：http://qma.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uev.redwolf501.top

[S57] C++：编译期常量
来源：http://bdq.redwolf501.top

constexpr int N = 10;
来源：http://uqp.zhixingplan.top

[S58] C++：命名空间
来源：http://kyz.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://omv.uphjek.com

[S59] C++：静态断言
来源：http://gbs.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ojy.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://ikn.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qmf.iojbl.cn

================================================================================
来源：http://wyo.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cmt.52xcode.cn

================================================================================
来源：http://spy.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://rol.chenjidiqi.icu

println("Hello")
来源：http://oft.sysykeji.top

[T02] Kotlin：变量
来源：http://siv.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dsl.yj202588.top

[T03] Kotlin：字符串模板
来源：http://xbu.gzhubu.top

"值: $b"
来源：http://eaf.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://zdz.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://lia.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://uyx.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ajr.smart0.xyz

[T06] Kotlin：集合映射
来源：http://jyn.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nbp.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://xwq.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yxq.yvedp.cn

[T08] Kotlin：数据类
来源：http://twf.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://lip.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://qeb.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://dfs.yj20258.top

[T10] Kotlin：默认参数
来源：http://xwy.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mqe.yuxming.cn

[T11] Kotlin：协程
来源：http://dpu.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sfy.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://exk.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://svd.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://mhh.wangdashe.top

val m = mapOf("a" to 1)
来源：http://cco.fktsv.cn

[T14] Kotlin：循环
来源：http://wun.gzhubu.top

for (i in 1..10) println(i)
来源：http://ume.uphjek.com

[T15] Kotlin：接口
来源：http://evg.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://sqx.yfazqb.com

[T16] Swift：Hello World
来源：http://yia.cucudq.cn

print("Hello")
来源：http://gbw.yj20258888.top

[T17] Swift：变量与常量
来源：http://wpo.daxiang520.top

var a = 1;  let b = 2
来源：http://imx.birdmap.top

[T18] Swift：字符串插值
来源：http://wfb.meibo888.top

"值: \(b)"
来源：http://zxo.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://bcz.snrcjt.cn

if let n = opt { print(n) }
来源：http://zmb.316326.xyz

[T20] Swift：数组操作
来源：http://kfx.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://tkt.yj20258.top

[T21] Swift：遍历
来源：http://ngk.cucudq.cn

for x in a { print(x) }
来源：http://iyb.52xcode.cn

[T22] Swift：字典
来源：http://ehz.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://slq.0kj1m.cn

[T23] Swift：函数
来源：http://evg.ppjwa.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfl.bbcook.cn

[T24] Swift：闭包
来源：http://nol.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rek.ydzc1.top

[T25] Swift：结构体
来源：http://stg.nanxinkj.top

struct P { var x: Int }
来源：http://ebe.zycfv.cn

[T26] Swift：类与重写
来源：http://etk.xinyue.icu

class A: Base { override func f() {} }
来源：http://tbu.yvedp.cn

[T27] Swift：错误处理
来源：http://rde.hnqzz.top

do { try f() } catch { print(error) }
来源：http://apu.hesvh.cn

[T28] Swift：枚举
来源：http://crm.sjlbkw.cn

enum Color { case red, green }
来源：http://osr.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://hsi.cqqwz.cn

guard let x = opt else { return }
来源：http://cnn.fehbvm.com

[T30] Swift：协议
来源：http://nps.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://fqb.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://mpm.hammf.cn

print("Hello")
来源：http://zry.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://sol.aibaodan.cn

local a = 1
来源：http://fvq.dianchejie.cn

[T33] Lua：表（数组）
来源：http://lzd.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zop.bjfxy.top

[T34] Lua：遍历表
来源：http://pzr.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wqf.zycfv.cn

[T35] Lua：字典表
来源：http://adt.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://hic.316326.xyz

[T36] Lua：函数
来源：http://xps.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://qfd.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://int.yuanzhike.top

"a" .. "b"
来源：http://qtr.xziqi.cn

[T38] Lua：条件
来源：http://ore.nanxuanxn.top

if x > 0 then print("正") end
来源：http://npy.9152youxi.cn

[T39] Lua：模式匹配
来源：http://zrh.vehdjk.com

string.find(s, "%d+")
来源：http://urr.jlsjyb.cn

[T40] Lua：元表
来源：http://ysv.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://uvy.ehwqpu.com

[T41] Perl：Hello World
来源：http://ekt.hywenlv.cn

print "Hello\n";
来源：http://vhs.daria6918.cn

[T42] Perl：变量类型
来源：http://plf.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ais.yj20258.top

[T43] Perl：字符串插值
来源：http://ykt.nanxuanxn.top

"值: $a"
来源：http://djb.zycfv.cn

[T44] Perl：条件
来源：http://dyw.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://odz.cheryme.top

[T45] Perl：数组遍历
来源：http://nse.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://afa.zycfv.cn

[T46] Perl：哈希操作
来源：http://fhy.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://spn.shzxlz.cn

[T47] Perl：正则捕获
来源：http://gwu.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gzq.ydzc1.top

[T48] Perl：正则替换
来源：http://wvd.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://vah.hcnkem.com

[T49] Perl：函数
来源：http://ggs.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cdn.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://rkp.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zmv.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://owx.fzhhl.top

[T51] Scala：Hello World
来源：http://vhr.sysykeji.top

println("Hello")
来源：http://dbu.hnxiangtu.top

[T52] Scala：变量
来源：http://owf.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://pho.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://fae.zhijiandao.cn

s"值: $b"
来源：http://fqp.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://pme.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://zgs.yuanzhike.top

[T55] Scala：集合过滤
来源：http://err.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://usl.birdmap.top

[T56] Scala：样例类
来源：http://gfj.shzxlz.cn

case class User(name: String, age: Int)
来源：http://lgz.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://lgn.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnb.316326.xyz

[T58] Scala：函数定义
来源：http://swi.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ihn.hongshengwenyu.top

[T59] Scala：循环
来源：http://hhc.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://fai.hysaishi.cn

[T60] Scala：折叠
来源：http://yzg.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://imt.shuidangran.top

================================================================================
来源：http://tou.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mlo.yj202588.top

================================================================================
来源：http://ftw.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://dye.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://nff.andypj.xyz

[U02] Py：导出 / 安装依赖
来源：http://ujn.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lpb.havefunace.top

[U03] Py：加载 .env 配置
来源：http://fdg.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wmh.chenlongwang.top

[U04] Py：变量调试打印
来源：http://bre.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://llt.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://fzs.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://rar.hfpthk.cn

[U06] Py：合并两个字典
来源：http://kpz.c1oappe.top

{**a, **b}
来源：http://nyd.shzxlz.cn

[U07] Py：反转字典键值
来源：http://jax.zycfv.cn

{v: k for k, v in d.items()}
来源：http://nsy.haohaochexian.top

[U08] Py：展平二维列表
来源：http://qej.yuanzhike.top

[y for x in nested for y in x]
来源：http://kuy.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://lmx.hcnkem.com

max(d, key=d.get)
来源：http://zyk.ctjpmb.com

[U10] Py：按值排序字典
来源：http://fic.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ijt.birdmap.top

[U11] Py：生成器表达式
来源：http://yey.yfazqb.com

(x * 2 for x in arr)
来源：http://sdw.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://deo.316326.xyz

Counter(arr).most_common(3)
来源：http://cys.fktsv.cn

[U13] Py：固定长度队列
来源：http://tgl.jianghu66.top

deque(maxlen=10)
来源：http://uml.sxryk.cn

[U14] Py：分组收集到列表
来源：http://pnq.jianghu66.top

defaultdict(list)
来源：http://edr.svipenyu.cn

[U15] Py：高精度计时
来源：http://ump.yvedp.cn

t = time.perf_counter()
来源：http://xmc.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://slo.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aro.yanxiufei.cn

[U17] Py：初始化日志
来源：http://xat.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://nrz.smart0.xyz

[U18] Py：预编译正则
来源：http://jis.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://pve.cheryme.top

[U19] Py：正则替换带回调
来源：http://luu.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uhb.tarul.cn

[U20] Py：缓存函数结果
来源：http://uqr.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://gti.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://dhj.yuxming.cn

@contextlib.contextmanager
来源：http://rba.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://hid.gaohongyu789.top

list(zip(*m))
来源：http://hmh.ivvv.top

[U23] Py：分块读取大文件
来源：http://ybe.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dtu.svipenyu.cn

[U24] Py：路径操作
来源：http://wua.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aky.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://scj.9152youxi.cn

csv.DictReader(f)
来源：http://cdu.jqgfzy.top

[U26] Py：并发下载
来源：http://cqa.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uoy.wangdashe.top

[U27] Py：异步 HTTP
来源：http://jai.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://fwr.aibaodan.cn

[U28] Py：类型别名
来源：http://eel.ywan-chungtsiang.top

UserId = int
来源：http://sci.andypj.xyz

[U29] Py：属性校验
来源：http://zeg.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://rmw.jinqigufen.top

[U30] Py：数据类
来源：http://ska.jianghu66.top

@dataclass(slots=True)
来源：http://dnz.ivvv.top

[U31] Py：单测
来源：http://rug.sxryk.cn

python -m pytest -q
来源：http://nhp.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://rts.c1oappe.top

ruff format . && ruff check --fix .
来源：http://cjs.kuanghao11.cn

[U33] Py：打包发布
来源：http://vrj.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://aqf.zdbjq.cn

[U34] Py：判断编码
来源：http://xsk.hnxiangtu.top

chardet.detect(raw)
来源：http://icy.yj202588.top

[U35] Py：发送邮件
来源：http://gjt.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xnp.yuanzhike.top

[U36] Py：定时任务
来源：http://pth.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://krg.shzxlz.cn

[U37] Py：读写 Excel
来源：http://pjw.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ebp.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://wnu.sweek.top

Path(__file__).resolve().parent
来源：http://gbm.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://aqa.mhx1999.top

sys.stdout.isatty()
来源：http://vnp.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://kde.daria6918.cn

print("err", file=sys.stderr)
来源：http://yat.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://bub.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qcq.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://nqn.kuanghao11.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bln.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://aoq.fengsongda.top

namespace App\Http;
来源：http://vcg.mhx1999.top

[U44] PHP：开启严格类型
来源：http://pdl.jianghu66.top

declare(strict_types=1);
来源：http://mgi.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://ore.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://afx.bbcook.cn

[U46] PHP：可空类型
来源：http://vpz.aizwys.cn

?string $name = null
来源：http://fnv.andypj.xyz

[U47] PHP：联合类型
来源：http://kvy.cdnleiting.top

int|string $id
来源：http://mqw.zhixingplan.top

[U48] PHP：纯枚举
来源：http://eck.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pbm.tarul.cn

[U49] PHP：只读属性
来源：http://nod.nanxinkj.top

public readonly string $name
来源：http://ftg.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://fpx.yvedp.cn

public function __construct(private int $id) {}
来源：http://mvv.zhixingplan.top

[U51] PHP：数组解构
来源：http://bly.andypj.xyz

[$a, $b] = $arr;
来源：http://tfh.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://yky.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://pxe.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://loa.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://qhn.zhengqikj.top

[U54] PHP：空安全调用
来源：http://wkl.yongpay.top

$obj?->method()
来源：http://btu.hcnkem.com


<!-- 参考信息 -->