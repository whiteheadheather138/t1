代发 wailian999

#ifndef X_H
来源：http://whd.316326.xyz

#define X_H
来源：http://exo.ivvv.top

#endif
来源：http://rqf.ydzc1.top

[S31] C++：Hello World
来源：http://nuu.yj20258.top

#include <iostream>
来源：http://fiu.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://qsl.bbcook.cn

[S32] C++：字符串
来源：http://cpf.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://sqp.daria6918.cn

[S33] C++：vector 增删
来源：http://kaa.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eid.nanxinkj.top

[S34] C++：遍历 vector
来源：http://ocw.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://mcw.vehdjk.com

[S35] C++：map
来源：http://frg.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://inb.yj20258888.top

[S36] C++：unordered_map
来源：http://gaq.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fqn.jinqigufen.top

[S37] C++：set
来源：http://ucw.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ehz.cqqwz.cn

[S38] C++：排序
来源：http://thm.tarul.cn

std::sort(v.begin(), v.end());
来源：http://egd.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://gsf.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gse.xuanzx.com

[S40] C++：查找元素
来源：http://uin.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tct.hammf.cn

[S41] C++：类与构造函数
来源：http://opz.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xuc.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://sby.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://kdq.fzhhl.top

[S43] C++：智能指针
来源：http://bng.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://pgg.ctjpmb.com

[S44] C++：引用传参
来源：http://spc.yj202588.top

void inc(int &x) { ++x; }
来源：http://vxw.yuxming.cn

[S45] C++：lambda
来源：http://hyc.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://gof.yangfankeji.com

[S46] C++：函数模板
来源：http://fnc.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://shs.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://jrv.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mby.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://mih.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://xhz.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://iun.fzhhl.top

[S49] C++：写文件
来源：http://tar.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iiv.jinqigufen.top

[S50] C++：格式化数字
来源：http://heb.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ubl.yj20258888.top

[S51] C++：显式类型转换
来源：http://qkh.hesvh.cn

static_cast<double>(a) / b
来源：http://ijj.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://zns.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://dxo.sysykeji.top

[S53] C++：移动语义
来源：http://vkv.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://fsa.yfazqb.com

[S54] C++：异常处理
来源：http://des.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dfb.yangfankeji.com

[S55] C++：结构化绑定
来源：http://ppu.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://mpt.meibo888.top

[S56] C++：optional
来源：http://aak.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qzn.9152youxi.cn

[S57] C++：编译期常量
来源：http://rix.havefunace.top

constexpr int N = 10;
来源：http://iai.daria6918.cn

[S58] C++：命名空间
来源：http://crw.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://llw.redwolf501.top

[S59] C++：静态断言
来源：http://ahy.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kzx.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://ccv.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wpx.cdnleiting.top

================================================================================
来源：http://ono.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zon.fktsv.cn

================================================================================
来源：http://bvu.meibo888.top

[T01] Kotlin：Hello World
来源：http://vlp.dashuyun.cn

println("Hello")
来源：http://xka.zhongyouzk.top

[T02] Kotlin：变量
来源：http://uip.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hue.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://tps.ivvv.top

"值: $b"
来源：http://dmu.vehdjk.com

[T04] Kotlin：空安全
来源：http://fqt.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://ffl.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://ipd.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qae.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://vzx.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://thd.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://jte.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aoo.haohaochexian.top

[T08] Kotlin：数据类
来源：http://oiq.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://zdu.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://tnr.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://gkg.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://wyz.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://baq.haohaochexian.top

[T11] Kotlin：协程
来源：http://sbx.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zcr.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://vot.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://yjl.sweek.top

[T13] Kotlin：只读 Map
来源：http://bqf.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://ois.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://gai.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://gdi.bbcook.cn

[T15] Kotlin：接口
来源：http://mls.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://ltr.zhixingplan.top

[T16] Swift：Hello World
来源：http://spk.wangdashe.top

print("Hello")
来源：http://iet.fengsongda.top

[T17] Swift：变量与常量
来源：http://abt.smart0.xyz

var a = 1;  let b = 2
来源：http://ivf.52xcode.cn

[T18] Swift：字符串插值
来源：http://hec.wangdashe.top

"值: \(b)"
来源：http://xjk.yj20258888.top

[T19] Swift：可选绑定
来源：http://hmu.jqgfzy.top

if let n = opt { print(n) }
来源：http://reu.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://ceu.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fug.jqgufenzy.top

[T21] Swift：遍历
来源：http://cyi.jqgufenzy.top

for x in a { print(x) }
来源：http://etu.yj202588.top

[T22] Swift：字典
来源：http://hkv.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://hbj.daxiang520.top

[T23] Swift：函数
来源：http://sgn.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pjs.xylfe.cn

[T24] Swift：闭包
来源：http://wyg.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tku.ehwqpu.com

[T25] Swift：结构体
来源：http://lig.gaohongyu789.top

struct P { var x: Int }
来源：http://wou.jqgfzy.top

[T26] Swift：类与重写
来源：http://beh.ivvv.top

class A: Base { override func f() {} }
来源：http://niw.zycfv.cn

[T27] Swift：错误处理
来源：http://umx.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://ict.redwolf501.top

[T28] Swift：枚举
来源：http://sjs.guowangkeji.top

enum Color { case red, green }
来源：http://cxo.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://pdf.meibo888.top

guard let x = opt else { return }
来源：http://tqu.cucudq.cn

[T30] Swift：协议
来源：http://ryn.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://mvr.gaohongyu789.top

[T31] Lua：Hello World
来源：http://wkr.uphjek.com

print("Hello")
来源：http://omv.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://otl.mhx1999.top

local a = 1
来源：http://amp.xinyue.icu

[T33] Lua：表（数组）
来源：http://tri.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zpb.yj202588.top

[T34] Lua：遍历表
来源：http://fjm.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uvn.jiagoushi.top

[T35] Lua：字典表
来源：http://dzf.wangshuangyany.cn

local d = { a = 1 };  d.b = 2
来源：http://ruq.aibaodan.cn

[T36] Lua：函数
来源：http://iti.fehbvm.com

function add(a, b) return a + b end
来源：http://xrs.xinyue.icu

[T37] Lua：字符串拼接
来源：http://nnd.jqgfzy.top

"a" .. "b"
来源：http://erp.mhx1999.top

[T38] Lua：条件
来源：http://res.shuidangran.top

if x > 0 then print("正") end
来源：http://ebv.kuanghao11.cn

[T39] Lua：模式匹配
来源：http://bre.chenlongwang.top

string.find(s, "%d+")
来源：http://hiw.fehbvm.com

[T40] Lua：元表
来源：http://eec.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://aik.hnqzz.top

[T41] Perl：Hello World
来源：http://tdf.vqdsnc.cn

print "Hello\n";
来源：http://jmc.ybcxt.top

[T42] Perl：变量类型
来源：http://bvm.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://thn.daxiang520.top

[T43] Perl：字符串插值
来源：http://bcz.jqgfzy.top

"值: $a"
来源：http://uwc.yuxming.cn

[T44] Perl：条件
来源：http://gsy.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://fqc.iojbl.cn

[T45] Perl：数组遍历
来源：http://ega.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://trm.pycfn.com

[T46] Perl：哈希操作
来源：http://lge.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fus.sweek.top

[T47] Perl：正则捕获
来源：http://xsh.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fut.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://ugi.ydzc1.top

$s =~ s/old/new/g;
来源：http://yot.yonumen.top

[T49] Perl：函数
来源：http://lpg.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ibo.hnqzz.top

[T50] Perl：逐行读文件
来源：http://ujy.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nry.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://keh.redwolf501.top

[T51] Scala：Hello World
来源：http://abu.pycfn.com

println("Hello")
来源：http://kwm.hywenlv.cn

[T52] Scala：变量
来源：http://cip.hywenlv.cn

val a = 1;  var b = 2
来源：http://bqd.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://hvs.feifeiyinyue.top

s"值: $b"
来源：http://qxh.sweek.top

[T54] Scala：集合映射
来源：http://pfv.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://rnj.tarul.cn

[T55] Scala：集合过滤
来源：http://kzo.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://vzd.hongshengwenyu.top

[T56] Scala：样例类
来源：http://hds.zhengqikj.top

case class User(name: String, age: Int)
来源：http://ldw.ivvv.top

[T57] Scala：模式匹配
来源：http://rte.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rfm.hnxiangtu.top

[T58] Scala：函数定义
来源：http://gvs.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://pet.hfpthk.cn

[T59] Scala：循环
来源：http://yoa.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://qwm.tarul.cn

[T60] Scala：折叠
来源：http://ltd.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ysa.tarul.cn

================================================================================
来源：http://aul.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xtc.jqgufenzy.top

================================================================================
来源：http://fen.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://mdy.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://opi.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://gqv.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gvi.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://hxo.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://idv.hesvh.cn

[U04] Py：变量调试打印
来源：http://spk.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aru.xziqi.cn

[U05] Py：列表去重且保序
来源：http://gqy.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://zom.xingfuxueyuan.xyz

[U06] Py：合并两个字典
来源：http://zsz.bbcook.cn

{**a, **b}
来源：http://hia.svipenyu.cn

[U07] Py：反转字典键值
来源：http://mnt.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://dtl.shzxlz.cn

[U08] Py：展平二维列表
来源：http://cao.birdmap.top

[y for x in nested for y in x]
来源：http://zuy.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://pkz.zhixingplan.top

max(d, key=d.get)
来源：http://arc.ydzc1.top

[U10] Py：按值排序字典
来源：http://avk.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://chk.redwolf501.top

[U11] Py：生成器表达式
来源：http://gpb.yueranfly.top

(x * 2 for x in arr)
来源：http://ddt.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rxe.sweek.top

Counter(arr).most_common(3)
来源：http://qbt.jianghu66.top

[U13] Py：固定长度队列
来源：http://hfp.chenzaomai.com

deque(maxlen=10)
来源：http://tmy.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://kpf.xuetiantiany.cn

defaultdict(list)
来源：http://pnp.zhengqikj.top

[U15] Py：高精度计时
来源：http://iaz.sweek.top

t = time.perf_counter()
来源：http://miv.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://uhq.ydzc1.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cau.xuanzx.com

[U17] Py：初始化日志
来源：http://llv.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://izh.yvedp.cn

[U18] Py：预编译正则
来源：http://oev.kuanghao11.cn

pat = re.compile(r"\d+")
来源：http://yrp.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://ssd.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dmy.zycfv.cn

[U20] Py：缓存函数结果
来源：http://yhr.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://dxp.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://jqz.0kj1m.cn

@contextlib.contextmanager
来源：http://hjg.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://yej.zhijiandao.cn

list(zip(*m))
来源：http://clq.meibo888.top

[U23] Py：分块读取大文件
来源：http://mgd.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ugi.yangfankeji.com

[U24] Py：路径操作
来源：http://maw.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://elc.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://ych.sysykeji.top

csv.DictReader(f)
来源：http://aph.snrcjt.cn

[U26] Py：并发下载
来源：http://mwb.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cga.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://vus.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://ofo.xylfe.cn

[U28] Py：类型别名
来源：http://wxa.gogol.net.cn

UserId = int
来源：http://jhp.hywenlv.cn

[U29] Py：属性校验
来源：http://xce.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://nin.havefunace.top

[U30] Py：数据类
来源：http://uqk.hongshengwenyu.top

@dataclass(slots=True)
来源：http://ofu.yuanzhike.top

[U31] Py：单测
来源：http://ifu.hesvh.cn

python -m pytest -q
来源：http://owb.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://fxm.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://tgn.kuanghao11.cn

[U33] Py：打包发布
来源：http://kgp.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://jvg.snrcjt.cn

[U34] Py：判断编码
来源：http://aoh.daxiang520.top

chardet.detect(raw)
来源：http://jmv.jqgfzy.top

[U35] Py：发送邮件
来源：http://rur.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rfb.yj20258.top

[U36] Py：定时任务
来源：http://wxd.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://sos.9152youxi.cn

[U37] Py：读写 Excel
来源：http://vgg.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://znr.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://ccq.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://ppu.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://hvr.sxryk.cn

sys.stdout.isatty()
来源：http://nkg.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://agm.aizwys.cn

print("err", file=sys.stderr)
来源：http://ngb.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://aev.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oux.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://ltb.c1oappe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hlj.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://mol.vehdjk.com

namespace App\Http;
来源：http://mkm.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://gzh.zhiwuduotai.top

declare(strict_types=1);
来源：http://uzu.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://apl.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://woq.zhengqikj.top

[U46] PHP：可空类型
来源：http://cbj.sweek.top

?string $name = null
来源：http://exp.hcnkem.com

[U47] PHP：联合类型
来源：http://zbi.sysykeji.top

int|string $id
来源：http://hhk.xuanzx.com

[U48] PHP：纯枚举
来源：http://yyq.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wom.jqgufenzy.top

[U49] PHP：只读属性
来源：http://xje.gotoacloud.top

public readonly string $name
来源：http://cor.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://hfr.hnqzz.top

public function __construct(private int $id) {}
来源：http://hbw.nwbrower.top

[U51] PHP：数组解构
来源：http://xvg.ybcxt.top

[$a, $b] = $arr;
来源：http://neo.jiagoushi.top

[U52] PHP：箭头函数
来源：http://sjt.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://wxo.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://gxu.dashuyun.cn

$v = $a ?? $b ?? "default";
来源：http://lsp.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://gkj.jyoumei.cn

$obj?->method()
来源：http://gkv.xuanzx.com


<!-- 参考信息 -->