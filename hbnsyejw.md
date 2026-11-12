代发 wailian999

#ifndef X_H
来源：http://hmp.cqqwz.cn

#define X_H
来源：http://mlf.hesvh.cn

#endif
来源：http://xmo.hcnkem.com

[S31] C++：Hello World
来源：http://fvq.yueranfly.top

#include <iostream>
来源：http://fjw.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://rie.haohaochexian.top

[S32] C++：字符串
来源：http://bwa.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://jdv.sufxvd.cn

[S33] C++：vector 增删
来源：http://mbb.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cbp.tian-w.cn

[S34] C++：遍历 vector
来源：http://akj.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://nuk.gogol.net.cn

[S35] C++：map
来源：http://bym.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rpq.fehbvm.com

[S36] C++：unordered_map
来源：http://lnr.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lpi.yongpay.top

[S37] C++：set
来源：http://eyu.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ykv.jinqigufen.top

[S38] C++：排序
来源：http://tjx.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://jvc.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://kdr.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dkp.jyoumei.cn

[S40] C++：查找元素
来源：http://fsl.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pva.yfazqb.com

[S41] C++：类与构造函数
来源：http://cbi.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hdz.52xcode.cn

[S42] C++：继承与虚函数
来源：http://ilz.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://lxg.9152youxi.cn

[S43] C++：智能指针
来源：http://zti.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://rgk.gzhubu.top

[S44] C++：引用传参
来源：http://lgn.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://kyb.zdqjudy.top

[S45] C++：lambda
来源：http://mrz.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://ekb.ydzc1.top

[S46] C++：函数模板
来源：http://yvi.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqk.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://tdd.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsz.vehdjk.com

[S48] C++：逐行读文件
来源：http://meq.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://sue.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://izr.snrcjt.cn

[S49] C++：写文件
来源：http://wjx.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wkj.hysaishi.cn

[S50] C++：格式化数字
来源：http://brd.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dui.xinyue.icu

[S51] C++：显式类型转换
来源：http://ptx.yj202588.top

static_cast<double>(a) / b
来源：http://hug.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://yhb.hesvh.cn

int size() const noexcept { return n_; }
来源：http://ors.xuetiantiany.cn

[S53] C++：移动语义
来源：http://qsk.yongpay.top

std::vector<int> w = std::move(v);
来源：http://fon.gotoacloud.top

[S54] C++：异常处理
来源：http://ahi.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nii.9152youxi.cn

[S55] C++：结构化绑定
来源：http://tft.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uyk.havefunace.top

[S56] C++：optional
来源：http://zek.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zth.shzxlz.cn

[S57] C++：编译期常量
来源：http://ucs.cdnleiting.top

constexpr int N = 10;
来源：http://aor.zhoulong.xyz

[S58] C++：命名空间
来源：http://snp.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://vge.dianchejie.cn

[S59] C++：静态断言
来源：http://egz.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://exm.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://sqw.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dzs.aibaodan.cn

================================================================================
来源：http://ugj.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bhw.xuanzx.com

================================================================================
来源：http://taf.jianghu66.top

[T01] Kotlin：Hello World
来源：http://tpp.guowangkeji.top

println("Hello")
来源：http://trr.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://idq.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tll.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://njt.sysykeji.top

"值: $b"
来源：http://vwk.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://fas.sweek.top

val n: String? = null;  n?.length
来源：http://xgu.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://kle.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iux.meibo888.top

[T06] Kotlin：集合映射
来源：http://pdv.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://egh.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://oxm.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lty.andypj.xyz

[T08] Kotlin：数据类
来源：http://clu.cheryme.top

data class User(val name: String, val age: Int)
来源：http://idp.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://dkr.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://oau.shuidangran.top

[T10] Kotlin：默认参数
来源：http://chy.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sfg.hywenlv.cn

[T11] Kotlin：协程
来源：http://nzz.redwolf501.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gta.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://hfx.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://ulq.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://lrc.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://ikb.daria6918.cn

[T14] Kotlin：循环
来源：http://zej.316326.xyz

for (i in 1..10) println(i)
来源：http://ztt.sufxvd.cn

[T15] Kotlin：接口
来源：http://mvc.epnwcf.com

interface Shape { fun area(): Double }
来源：http://aqm.cashguo.top

[T16] Swift：Hello World
来源：http://aan.yj202588.top

print("Hello")
来源：http://cqj.c1oappe.top

[T17] Swift：变量与常量
来源：http://odc.gzhubu.top

var a = 1;  let b = 2
来源：http://hhu.sufxvd.cn

[T18] Swift：字符串插值
来源：http://osl.haohaochexian.top

"值: \(b)"
来源：http://job.zdqjudy.top

[T19] Swift：可选绑定
来源：http://vke.ybcxt.top

if let n = opt { print(n) }
来源：http://kwy.tian-w.cn

[T20] Swift：数组操作
来源：http://xxt.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://szv.guannengcc.top

[T21] Swift：遍历
来源：http://nqm.yuxming.cn

for x in a { print(x) }
来源：http://ydp.yanxiufei.cn

[T22] Swift：字典
来源：http://kny.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://tte.xylfe.cn

[T23] Swift：函数
来源：http://zhm.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://trx.jlsjyb.cn

[T24] Swift：闭包
来源：http://dza.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://own.hywenlv.cn

[T25] Swift：结构体
来源：http://fbb.jqgfzy.top

struct P { var x: Int }
来源：http://hpj.havefunace.top

[T26] Swift：类与重写
来源：http://xsr.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://vdr.ehwqpu.com

[T27] Swift：错误处理
来源：http://lfm.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://lxp.nanxinkj.top

[T28] Swift：枚举
来源：http://pkr.redwolf501.top

enum Color { case red, green }
来源：http://aqn.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://jhl.snrcjt.cn

guard let x = opt else { return }
来源：http://hyq.xylfe.cn

[T30] Swift：协议
来源：http://qeu.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://dmv.aibaodan.cn

[T31] Lua：Hello World
来源：http://npy.jinyuanbaomall.cn

print("Hello")
来源：http://pow.yfazqb.com

[T32] Lua：局部变量
来源：http://owu.gaohongyu789.top

local a = 1
来源：http://xwa.epnwcf.com

[T33] Lua：表（数组）
来源：http://jfh.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pkl.cashguo.top

[T34] Lua：遍历表
来源：http://wnv.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ibb.svipenyu.cn

[T35] Lua：字典表
来源：http://pjl.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://ina.jyoumei.cn

[T36] Lua：函数
来源：http://odx.ydzc1.top

function add(a, b) return a + b end
来源：http://vlu.epnwcf.com

[T37] Lua：字符串拼接
来源：http://yte.yj20258888.top

"a" .. "b"
来源：http://pvr.hongshengwenyu.top

[T38] Lua：条件
来源：http://tzh.gotoacloud.top

if x > 0 then print("正") end
来源：http://sjj.gotoacloud.top

[T39] Lua：模式匹配
来源：http://hen.zdbjq.cn

string.find(s, "%d+")
来源：http://iij.vehdjk.com

[T40] Lua：元表
来源：http://yjf.andypj.xyz

setmetatable({}, { __index = base })
来源：http://bcm.xylfe.cn

[T41] Perl：Hello World
来源：http://bap.hnxiangtu.top

print "Hello\n";
来源：http://rfb.jqgfzy.top

[T42] Perl：变量类型
来源：http://gog.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ary.ppjwa.cn

[T43] Perl：字符串插值
来源：http://swr.52xcode.cn

"值: $a"
来源：http://mao.kuanghao11.cn

[T44] Perl：条件
来源：http://kbc.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://rft.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://lwb.yj20258.top

for my $x (@arr) { print $x; }
来源：http://alg.svipenyu.cn

[T46] Perl：哈希操作
来源：http://ddn.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://upf.epnwcf.com

[T47] Perl：正则捕获
来源：http://srz.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://tbv.xinyue.icu

[T48] Perl：正则替换
来源：http://znz.jqgfzy.top

$s =~ s/old/new/g;
来源：http://wuj.aizwys.cn

[T49] Perl：函数
来源：http://xkx.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zut.yonumen.top

[T50] Perl：逐行读文件
来源：http://yeb.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://oiu.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://mcr.316326.xyz

[T51] Scala：Hello World
来源：http://hzc.gogol.net.cn

println("Hello")
来源：http://ehk.zhengqikj.top

[T52] Scala：变量
来源：http://fnn.andypj.xyz

val a = 1;  var b = 2
来源：http://sjy.yvedp.cn

[T53] Scala：字符串插值
来源：http://dgw.zhaomingkeji.xyz

s"值: $b"
来源：http://gtx.meibo888.top

[T54] Scala：集合映射
来源：http://uwl.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://hji.yfazqb.com

[T55] Scala：集合过滤
来源：http://eqo.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://cvt.jinqigfzy.top

[T56] Scala：样例类
来源：http://rwm.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://vyb.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://dzy.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tvw.ydzc1.top

[T58] Scala：函数定义
来源：http://zdd.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qyf.andypj.xyz

[T59] Scala：循环
来源：http://szj.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://tki.yj20258.top

[T60] Scala：折叠
来源：http://knr.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jnz.vehdjk.com

================================================================================
来源：http://aly.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dsl.haohaochexian.top

================================================================================
来源：http://qvf.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://pdc.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://ypv.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://vko.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibq.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://kde.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://pge.ppjwa.cn

[U04] Py：变量调试打印
来源：http://ypx.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mvl.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://mew.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://udo.hysaishi.cn

[U06] Py：合并两个字典
来源：http://sct.fktsv.cn

{**a, **b}
来源：http://gxx.hnqzz.top

[U07] Py：反转字典键值
来源：http://upl.yvedp.cn

{v: k for k, v in d.items()}
来源：http://gtg.redwolf501.top

[U08] Py：展平二维列表
来源：http://sap.zdqjudy.top

[y for x in nested for y in x]
来源：http://yog.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://opd.fengsongda.top

max(d, key=d.get)
来源：http://vtn.xinyue.icu

[U10] Py：按值排序字典
来源：http://yxv.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tnn.zdqjudy.top

[U11] Py：生成器表达式
来源：http://sue.ppjwa.cn

(x * 2 for x in arr)
来源：http://awn.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hnx.sufxvd.cn

Counter(arr).most_common(3)
来源：http://kdb.cheryme.top

[U13] Py：固定长度队列
来源：http://qjg.fengsongda.top

deque(maxlen=10)
来源：http://zwq.yj20258.top

[U14] Py：分组收集到列表
来源：http://kzo.yueranfly.top

defaultdict(list)
来源：http://wjh.sweek.top

[U15] Py：高精度计时
来源：http://hfn.shangyingyoupin.top

t = time.perf_counter()
来源：http://mjq.havefunace.top

[U16] Py：命令行参数解析
来源：http://ifa.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ttl.yj202588.top

[U17] Py：初始化日志
来源：http://jiy.smart0.xyz

logging.basicConfig(level=logging.INFO)
来源：http://vvl.9152youxi.cn

[U18] Py：预编译正则
来源：http://rct.uphjek.com

pat = re.compile(r"\d+")
来源：http://ohc.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://tkh.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dte.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://iiq.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://iuv.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://pzp.gaohongyu789.top

@contextlib.contextmanager
来源：http://erj.xinyue.icu

[U22] Py：矩阵转置
来源：http://jko.jinqigfzy.top

list(zip(*m))
来源：http://pst.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://slb.jinqigufen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://urm.shuidangran.top

[U24] Py：路径操作
来源：http://ery.gzhubu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xaq.ybcxt.top

[U25] Py：CSV 按字典读
来源：http://lub.birdmap.top

csv.DictReader(f)
来源：http://sbr.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://gqe.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ndt.birdmap.top

[U27] Py：异步 HTTP
来源：http://nlt.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://srv.haohaochexian.top

[U28] Py：类型别名
来源：http://kgj.jianghu66.top

UserId = int
来源：http://mda.gogol.net.cn

[U29] Py：属性校验
来源：http://cla.chenlongwang.top

@property 与 @x.setter 配合
来源：http://bjb.shzxlz.cn

[U30] Py：数据类
来源：http://tyh.hcnkem.com

@dataclass(slots=True)
来源：http://jul.tanke756.top

[U31] Py：单测
来源：http://pkj.yj20258.top

python -m pytest -q
来源：http://hlo.zhixingplan.top

[U32] Py：代码格式化
来源：http://fas.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://ubb.chenlongwang.top

[U33] Py：打包发布
来源：http://aip.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://mge.birdmap.top

[U34] Py：判断编码
来源：http://tzo.nanxuanxn.top

chardet.detect(raw)
来源：http://nhg.hfpthk.cn

[U35] Py：发送邮件
来源：http://rxp.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pyy.sxryk.cn

[U36] Py：定时任务
来源：http://xgn.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://ghj.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://jub.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xpb.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://kdd.zycfv.cn

Path(__file__).resolve().parent
来源：http://dim.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://nnc.guannengcc.top

sys.stdout.isatty()
来源：http://baq.xziqi.cn

[U40] Py：打印到标准错误
来源：http://drq.dianchejie.cn

print("err", file=sys.stderr)
来源：http://agb.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://dpt.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rhk.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://hkt.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://faz.nwbrower.top

[U43] PHP：声明命名空间
来源：http://jlh.gzhubu.top

namespace App\Http;
来源：http://kzb.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://ruv.meibo888.top

declare(strict_types=1);
来源：http://shw.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://zee.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://fyw.yj202588.top

[U46] PHP：可空类型
来源：http://xay.tanke756.top

?string $name = null
来源：http://hei.cqqwz.cn

[U47] PHP：联合类型
来源：http://ghr.fanxiaobao.xyz

int|string $id
来源：http://sie.jyoumei.cn

[U48] PHP：纯枚举
来源：http://agp.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qhw.jinqigufen.top

[U49] PHP：只读属性
来源：http://fat.hywenlv.cn

public readonly string $name
来源：http://tbv.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://ifu.shuidangran.top

public function __construct(private int $id) {}
来源：http://jnf.zdbjq.cn

[U51] PHP：数组解构
来源：http://nyr.kuanghao11.cn

[$a, $b] = $arr;
来源：http://qqu.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://feb.0kj1m.cn

$double = fn($x) => $x * 2;
来源：http://hsa.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://toq.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://hpb.ydzc1.top

[U54] PHP：空安全调用
来源：http://lmy.jianghu66.top

$obj?->method()
来源：http://ght.yj20258888.top


<!-- 参考信息 -->