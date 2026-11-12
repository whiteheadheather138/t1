代发 wailian999

#ifndef X_H
来源：http://drh.hnqzz.top

#define X_H
来源：http://pig.vehdjk.com

#endif
来源：http://ygr.hnqzz.top

[S31] C++：Hello World
来源：http://opd.zhixingplan.top

#include <iostream>
来源：http://wtw.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ekr.snrcjt.cn

[S32] C++：字符串
来源：http://cjw.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://beh.bjfxy.top

[S33] C++：vector 增删
来源：http://nrj.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://caa.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://ymf.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://nsp.jiagoushi.top

[S35] C++：map
来源：http://cut.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rtw.52xcode.cn

[S36] C++：unordered_map
来源：http://xzz.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mrx.mhx1999.top

[S37] C++：set
来源：http://eko.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mgh.zhijiandao.cn

[S38] C++：排序
来源：http://nmt.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://eyw.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://sfn.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bqw.pengpengdd.cyou

[S40] C++：查找元素
来源：http://odi.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jqo.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://ojl.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oqs.yueranfly.top

[S42] C++：继承与虚函数
来源：http://ppk.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://hpt.ywan-chungtsiang.top

[S43] C++：智能指针
来源：http://tfa.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://veu.hywenlv.cn

[S44] C++：引用传参
来源：http://hji.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://xgx.guowangkeji.top

[S45] C++：lambda
来源：http://ijc.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://bld.zhixingplan.top

[S46] C++：函数模板
来源：http://afn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kmb.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://zlq.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uip.yuanzhike.top

[S48] C++：逐行读文件
来源：http://pku.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://llz.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://vsu.birdmap.top

[S49] C++：写文件
来源：http://uij.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pyp.yj202588.top

[S50] C++：格式化数字
来源：http://aue.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ftn.yangfankeji.com

[S51] C++：显式类型转换
来源：http://nth.zhongyouzk.top

static_cast<double>(a) / b
来源：http://tsz.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://usg.shuidangran.top

int size() const noexcept { return n_; }
来源：http://mfd.hnxiangtu.top

[S53] C++：移动语义
来源：http://gxn.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://vpu.fengsongda.top

[S54] C++：异常处理
来源：http://moj.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://prf.nanxinkj.top

[S55] C++：结构化绑定
来源：http://gex.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://egd.hesvh.cn

[S56] C++：optional
来源：http://ukh.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xww.smart0.xyz

[S57] C++：编译期常量
来源：http://upu.yonumen.top

constexpr int N = 10;
来源：http://xwi.chenlongwang.top

[S58] C++：命名空间
来源：http://cvl.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://hcr.bjfxy.top

[S59] C++：静态断言
来源：http://wml.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gqg.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://blv.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nxm.birdmap.top

================================================================================
来源：http://sam.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opx.tanke756.top

================================================================================
来源：http://dqa.zycfv.cn

[T01] Kotlin：Hello World
来源：http://yir.ehwqpu.com

println("Hello")
来源：http://vrb.hcnkem.com

[T02] Kotlin：变量
来源：http://ewh.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gif.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://ock.shuidangran.top

"值: $b"
来源：http://ily.yuanzhike.top

[T04] Kotlin：空安全
来源：http://vgq.hysaishi.cn

val n: String? = null;  n?.length
来源：http://jny.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://xvy.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uom.nwbrower.top

[T06] Kotlin：集合映射
来源：http://lui.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qnp.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://cqn.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dfb.ybcxt.top

[T08] Kotlin：数据类
来源：http://nnv.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://hcc.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://nkj.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://klm.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://dwa.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://vgb.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://nba.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sis.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://cwf.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://wjp.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://vnz.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://fif.smart0.xyz

[T14] Kotlin：循环
来源：http://ymn.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://vhq.shuidangran.top

[T15] Kotlin：接口
来源：http://smj.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://fei.yj202588.top

[T16] Swift：Hello World
来源：http://iab.sxryk.cn

print("Hello")
来源：http://iqu.tarul.cn

[T17] Swift：变量与常量
来源：http://fqz.jyoumei.cn

var a = 1;  let b = 2
来源：http://gud.yfazqb.com

[T18] Swift：字符串插值
来源：http://jwa.ydjk.org.cn

"值: \(b)"
来源：http://mfv.yueranfly.top

[T19] Swift：可选绑定
来源：http://hdd.hammf.cn

if let n = opt { print(n) }
来源：http://lmr.vqdsnc.cn

[T20] Swift：数组操作
来源：http://hho.jqgfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://vhf.aizwys.cn

[T21] Swift：遍历
来源：http://xdr.dashuyun.cn

for x in a { print(x) }
来源：http://ukl.chenlongwang.top

[T22] Swift：字典
来源：http://wdl.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://uit.ybcxt.top

[T23] Swift：函数
来源：http://chh.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zop.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://sth.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cpd.chenlongwang.top

[T25] Swift：结构体
来源：http://brx.gotoacloud.top

struct P { var x: Int }
来源：http://bcl.0kj1m.cn

[T26] Swift：类与重写
来源：http://dyx.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://ewq.uphjek.com

[T27] Swift：错误处理
来源：http://swn.bjfxy.top

do { try f() } catch { print(error) }
来源：http://ucl.yj20258888.top

[T28] Swift：枚举
来源：http://nls.hfpthk.cn

enum Color { case red, green }
来源：http://syr.yj202588.top

[T29] Swift：guard 提前返回
来源：http://nkw.chenlongwang.top

guard let x = opt else { return }
来源：http://lei.hywenlv.cn

[T30] Swift：协议
来源：http://inz.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://ric.ydjk.org.cn

[T31] Lua：Hello World
来源：http://ymx.yj20258.top

print("Hello")
来源：http://njh.xuanzx.com

[T32] Lua：局部变量
来源：http://fpc.hysaishi.cn

local a = 1
来源：http://lyt.cdnleiting.top

[T33] Lua：表（数组）
来源：http://ltn.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://vkk.xuanzx.com

[T34] Lua：遍历表
来源：http://lmz.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://szj.yvedp.cn

[T35] Lua：字典表
来源：http://lyj.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://izy.zhiwuduotai.top

[T36] Lua：函数
来源：http://wfk.jlsjyb.cn

function add(a, b) return a + b end
来源：http://hmm.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://zzh.shanyushiyangkeji.top

"a" .. "b"
来源：http://sef.fktsv.cn

[T38] Lua：条件
来源：http://zct.yongpay.top

if x > 0 then print("正") end
来源：http://ruj.wangdashe.top

[T39] Lua：模式匹配
来源：http://ruh.mhx1999.top

string.find(s, "%d+")
来源：http://guw.cucudq.cn

[T40] Lua：元表
来源：http://fzu.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://hgo.wangdashe.top

[T41] Perl：Hello World
来源：http://tts.snrcjt.cn

print "Hello\n";
来源：http://mfy.redwolf501.top

[T42] Perl：变量类型
来源：http://rps.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lks.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://soy.vehdjk.com

"值: $a"
来源：http://miy.hnqzz.top

[T44] Perl：条件
来源：http://jaw.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://hrd.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://fep.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://ihk.chenzaomai.com

[T46] Perl：哈希操作
来源：http://sii.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vfe.yonumen.top

[T47] Perl：正则捕获
来源：http://djn.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://asa.meibo888.top

[T48] Perl：正则替换
来源：http://ejc.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://hhi.ivvv.top

[T49] Perl：函数
来源：http://qjc.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://elr.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://axa.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fsz.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://vjv.dianchejie.cn

[T51] Scala：Hello World
来源：http://aom.jianghu66.top

println("Hello")
来源：http://etz.meibo888.top

[T52] Scala：变量
来源：http://web.zdbjq.cn

val a = 1;  var b = 2
来源：http://hjk.meibo888.top

[T53] Scala：字符串插值
来源：http://ofw.cucudq.cn

s"值: $b"
来源：http://voh.guowangkeji.top

[T54] Scala：集合映射
来源：http://lah.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://pns.0kj1m.cn

[T55] Scala：集合过滤
来源：http://kxf.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://wvt.jlsjyb.cn

[T56] Scala：样例类
来源：http://jfe.ivvv.top

case class User(name: String, age: Int)
来源：http://npq.cqqwz.cn

[T57] Scala：模式匹配
来源：http://man.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://trw.svipenyu.cn

[T58] Scala：函数定义
来源：http://npo.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://zun.aizwys.cn

[T59] Scala：循环
来源：http://nsp.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://fti.birdmap.top

[T60] Scala：折叠
来源：http://jgw.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rab.ywan-chungtsiang.top

================================================================================
来源：http://crr.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ttn.bjfxy.top

================================================================================
来源：http://bwa.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://gfi.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iao.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://quy.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://drb.ivvv.top

[U03] Py：加载 .env 配置
来源：http://zhb.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://lxm.pycfn.com

[U04] Py：变量调试打印
来源：http://uti.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rkg.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://uah.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://nfj.pycfn.com

[U06] Py：合并两个字典
来源：http://blh.aizwys.cn

{**a, **b}
来源：http://ejp.jyoumei.cn

[U07] Py：反转字典键值
来源：http://wum.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://zsg.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://rts.gogol.net.cn

[y for x in nested for y in x]
来源：http://thl.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://ysb.dianchejie.cn

max(d, key=d.get)
来源：http://yih.hysaishi.cn

[U10] Py：按值排序字典
来源：http://wwy.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ltu.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://tgj.chenlongwang.top

(x * 2 for x in arr)
来源：http://okb.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://oqd.chenlongwang.top

Counter(arr).most_common(3)
来源：http://xou.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://azd.tarul.cn

deque(maxlen=10)
来源：http://qsp.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://vzo.chenzaomai.com

defaultdict(list)
来源：http://qzm.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://ugj.xylfe.cn

t = time.perf_counter()
来源：http://gro.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://yuu.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qrt.c1oappe.top

[U17] Py：初始化日志
来源：http://jzf.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://kmd.cashguo.top

[U18] Py：预编译正则
来源：http://xby.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://kdh.zhoulong.xyz

[U19] Py：正则替换带回调
来源：http://lft.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lbk.smart0.xyz

[U20] Py：缓存函数结果
来源：http://nmp.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://yfu.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://ncj.zhongyouzk.top

@contextlib.contextmanager
来源：http://tah.tianlin.xyz

[U22] Py：矩阵转置
来源：http://pfu.shzxlz.cn

list(zip(*m))
来源：http://pzv.c1oappe.top

[U23] Py：分块读取大文件
来源：http://cpn.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ebx.9152youxi.cn

[U24] Py：路径操作
来源：http://tbz.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cme.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://qdm.316326.xyz

csv.DictReader(f)
来源：http://oeb.bbcook.cn

[U26] Py：并发下载
来源：http://zns.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hpc.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://ejd.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://nhv.hnqzz.top

[U28] Py：类型别名
来源：http://blb.yueranfly.top

UserId = int
来源：http://bkr.xuanzx.com

[U29] Py：属性校验
来源：http://ahk.316326.xyz

@property 与 @x.setter 配合
来源：http://plo.ppjwa.cn

[U30] Py：数据类
来源：http://rbn.hnxiangtu.top

@dataclass(slots=True)
来源：http://ryn.xingfuxueyuan.xyz

[U31] Py：单测
来源：http://mlm.sufxvd.cn

python -m pytest -q
来源：http://fph.snrcjt.cn

[U32] Py：代码格式化
来源：http://ycm.zycfv.cn

ruff format . && ruff check --fix .
来源：http://pii.sysykeji.top

[U33] Py：打包发布
来源：http://wvp.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://kux.ydjk.org.cn

[U34] Py：判断编码
来源：http://lhf.ppjwa.cn

chardet.detect(raw)
来源：http://fpc.cucudq.cn

[U35] Py：发送邮件
来源：http://sdc.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zob.tanke756.top

[U36] Py：定时任务
来源：http://tik.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://drk.shuidangran.top

[U37] Py：读写 Excel
来源：http://idx.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://fmh.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://zmo.sweek.top

Path(__file__).resolve().parent
来源：http://yhi.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://bmr.c1oappe.top

sys.stdout.isatty()
来源：http://frk.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://ipm.cqqwz.cn

print("err", file=sys.stderr)
来源：http://vyy.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://iwr.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wau.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://ybj.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://daj.mhx1999.top

[U43] PHP：声明命名空间
来源：http://ire.zdbjq.cn

namespace App\Http;
来源：http://trf.xuanzx.com

[U44] PHP：开启严格类型
来源：http://gno.zhengqikj.top

declare(strict_types=1);
来源：http://dnl.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://iyh.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qgl.cheryme.top

[U46] PHP：可空类型
来源：http://iyn.yueranfly.top

?string $name = null
来源：http://wag.smart0.xyz

[U47] PHP：联合类型
来源：http://jvt.tarul.cn

int|string $id
来源：http://bhq.jianghu66.top

[U48] PHP：纯枚举
来源：http://zyk.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dpo.yvedp.cn

[U49] PHP：只读属性
来源：http://ieq.vqdsnc.cn

public readonly string $name
来源：http://oen.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://qli.iojbl.cn

public function __construct(private int $id) {}
来源：http://wyg.meibo888.top

[U51] PHP：数组解构
来源：http://pee.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://whg.tian-w.cn

[U52] PHP：箭头函数
来源：http://ies.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://xcy.hnqzz.top

[U53] PHP：空合并运算符
来源：http://ggq.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://doa.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://hfh.cqqwz.cn

$obj?->method()
来源：http://jbx.shuidangran.top


<!-- 参考信息 -->