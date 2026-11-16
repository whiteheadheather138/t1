代发 wailian999

#ifndef X_H
来源：http://vzo.zhixingplan.top

#define X_H
来源：http://bop.yongpay.top

#endif
来源：http://pdd.jianghu66.top

[S31] C++：Hello World
来源：http://wfo.hcnkem.com

#include <iostream>
来源：http://fsa.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://ylm.guowangkeji.top

[S32] C++：字符串
来源：http://moy.meibo888.top

std::string s = "hi";  s += "!";
来源：http://doq.snrcjt.cn

[S33] C++：vector 增删
来源：http://tag.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tpb.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://jyz.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://cuw.hongshengwenyu.top

[S35] C++：map
来源：http://elz.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pji.tarul.cn

[S36] C++：unordered_map
来源：http://xlt.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lln.yonumen.top

[S37] C++：set
来源：http://jdl.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bnw.xuetiantiany.cn

[S38] C++：排序
来源：http://chp.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://ipn.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://jdx.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yxt.yueranfly.top

[S40] C++：查找元素
来源：http://jim.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xpc.zycfv.cn

[S41] C++：类与构造函数
来源：http://smf.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nqf.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://msr.sweek.top

class B : public Base { public: void f() override {} };
来源：http://snr.meibo888.top

[S43] C++：智能指针
来源：http://wto.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://tyo.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://rza.xuanzx.com

void inc(int &x) { ++x; }
来源：http://mqq.c1oappe.top

[S45] C++：lambda
来源：http://nuu.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vrv.xuanzx.com

[S46] C++：函数模板
来源：http://qgc.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dzr.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://ior.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lst.guannengcc.top

[S48] C++：逐行读文件
来源：http://wpi.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hfs.cashguo.top

while (std::getline(in, line)) { }
来源：http://mjy.andypj.xyz

[S49] C++：写文件
来源：http://qpg.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vnd.zhijiandao.cn

[S50] C++：格式化数字
来源：http://cbr.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://svv.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://wzt.smart0.xyz

static_cast<double>(a) / b
来源：http://pav.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://guu.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://tki.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://bxc.yongpay.top

std::vector<int> w = std::move(v);
来源：http://gkh.yfazqb.com

[S54] C++：异常处理
来源：http://fji.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nvk.xylfe.cn

[S55] C++：结构化绑定
来源：http://lsl.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngr.bjfxy.top

[S56] C++：optional
来源：http://qcm.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tew.yj20258888.top

[S57] C++：编译期常量
来源：http://cjc.smart0.xyz

constexpr int N = 10;
来源：http://sub.zhongyouzk.top

[S58] C++：命名空间
来源：http://gbf.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://oid.c1oappe.top

[S59] C++：静态断言
来源：http://iwk.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://trg.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://nmd.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yzl.daria6918.cn

================================================================================
来源：http://fdl.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://isa.tianlin.xyz

================================================================================
来源：http://bwd.guannengcc.top

[T01] Kotlin：Hello World
来源：http://vkd.feifeiyinyue.top

println("Hello")
来源：http://vwe.dashuyun.cn

[T02] Kotlin：变量
来源：http://rbh.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://efi.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://hbb.jyoumei.cn

"值: $b"
来源：http://kkb.yfazqb.com

[T04] Kotlin：空安全
来源：http://kjw.gotoacloud.top

val n: String? = null;  n?.length
来源：http://prs.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://txj.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ozc.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://kcv.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rux.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://rjl.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pcd.sysykeji.top

[T08] Kotlin：数据类
来源：http://lqd.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://jrv.birdmap.top

[T09] Kotlin：扩展函数
来源：http://uxm.cashguo.top

fun String.exclaim() = this + "!"
来源：http://ill.bbcook.cn

[T10] Kotlin：默认参数
来源：http://osk.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yhr.jinqigfzy.top

[T11] Kotlin：协程
来源：http://vhg.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oxv.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://tsv.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://ejz.meibo888.top

[T13] Kotlin：只读 Map
来源：http://xeh.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://rbf.hnqzz.top

[T14] Kotlin：循环
来源：http://zsn.tian-w.cn

for (i in 1..10) println(i)
来源：http://wcz.chenzaomai.com

[T15] Kotlin：接口
来源：http://jaq.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://zbe.sweek.top

[T16] Swift：Hello World
来源：http://nio.jinqigufen.top

print("Hello")
来源：http://vbr.316326.xyz

[T17] Swift：变量与常量
来源：http://bsr.zhongyouzk.top

var a = 1;  let b = 2
来源：http://kfv.bjfxy.top

[T18] Swift：字符串插值
来源：http://ocf.bbcook.cn

"值: \(b)"
来源：http://bpp.gotoacloud.top

[T19] Swift：可选绑定
来源：http://mvf.hfpthk.cn

if let n = opt { print(n) }
来源：http://gxw.bbcook.cn

[T20] Swift：数组操作
来源：http://dmo.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://irn.guannengcc.top

[T21] Swift：遍历
来源：http://mkr.yongpay.top

for x in a { print(x) }
来源：http://sxw.hfpthk.cn

[T22] Swift：字典
来源：http://ygr.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://vls.svipenyu.cn

[T23] Swift：函数
来源：http://kyc.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://stc.pengpengdd.cyou

[T24] Swift：闭包
来源：http://cll.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fbo.aibaodan.cn

[T25] Swift：结构体
来源：http://mcg.yueranfly.top

struct P { var x: Int }
来源：http://ajb.yj20258888.top

[T26] Swift：类与重写
来源：http://qdj.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://wpm.0kj1m.cn

[T27] Swift：错误处理
来源：http://fpu.hesvh.cn

do { try f() } catch { print(error) }
来源：http://hdw.ydzc1.top

[T28] Swift：枚举
来源：http://zqi.9152youxi.cn

enum Color { case red, green }
来源：http://itc.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://kfl.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://qee.quarkkingdee.top

[T30] Swift：协议
来源：http://viq.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://dxt.gzhubu.top

[T31] Lua：Hello World
来源：http://rll.wangshuangyany.cn

print("Hello")
来源：http://snw.nanxinkj.top

[T32] Lua：局部变量
来源：http://rri.hesvh.cn

local a = 1
来源：http://jsb.yuxming.cn

[T33] Lua：表（数组）
来源：http://nes.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cqt.yanxiufei.cn

[T34] Lua：遍历表
来源：http://qds.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://obz.ppjwa.cn

[T35] Lua：字典表
来源：http://iob.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://oxu.gaohongyu789.top

[T36] Lua：函数
来源：http://djy.iojbl.cn

function add(a, b) return a + b end
来源：http://hii.316326.xyz

[T37] Lua：字符串拼接
来源：http://sdl.hongshengwenyu.top

"a" .. "b"
来源：http://vcw.fehbvm.com

[T38] Lua：条件
来源：http://cez.ehwqpu.com

if x > 0 then print("正") end
来源：http://sdu.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://ldr.zhixingplan.top

string.find(s, "%d+")
来源：http://ahy.zhiwuduotai.top

[T40] Lua：元表
来源：http://ihz.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://gzs.hesvh.cn

[T41] Perl：Hello World
来源：http://lvo.andypj.xyz

print "Hello\n";
来源：http://whg.jqgfzy.top

[T42] Perl：变量类型
来源：http://jhp.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cyi.jiagoushi.top

[T43] Perl：字符串插值
来源：http://mle.xuanzx.com

"值: $a"
来源：http://khi.wangshuangyany.cn

[T44] Perl：条件
来源：http://txf.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://jpy.nanxinkj.top

[T45] Perl：数组遍历
来源：http://mra.tarul.cn

for my $x (@arr) { print $x; }
来源：http://euw.jiagoushi.top

[T46] Perl：哈希操作
来源：http://dee.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jcy.hysaishi.cn

[T47] Perl：正则捕获
来源：http://sog.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://yoq.cashguo.top

[T48] Perl：正则替换
来源：http://ild.yfazqb.com

$s =~ s/old/new/g;
来源：http://jnq.redwolf501.top

[T49] Perl：函数
来源：http://gwk.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zpt.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://jhk.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://oqu.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://vaa.yj20258.top

[T51] Scala：Hello World
来源：http://xze.hammf.cn

println("Hello")
来源：http://gqa.tanke756.top

[T52] Scala：变量
来源：http://the.kuanghao11.cn

val a = 1;  var b = 2
来源：http://ubs.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://bnz.ydjk.org.cn

s"值: $b"
来源：http://rqk.yfazqb.com

[T54] Scala：集合映射
来源：http://zyj.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://zrh.yfazqb.com

[T55] Scala：集合过滤
来源：http://hsj.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://mkd.xuetiantiany.cn

[T56] Scala：样例类
来源：http://tzy.yonumen.top

case class User(name: String, age: Int)
来源：http://cmn.yuanzhike.top

[T57] Scala：模式匹配
来源：http://dwe.hysaishi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nmj.ydjk.org.cn

[T58] Scala：函数定义
来源：http://vdm.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://qbb.hysaishi.cn

[T59] Scala：循环
来源：http://xay.haohaochexian.top

for (i <- 1 to 10) println(i)
来源：http://xly.jianghu66.top

[T60] Scala：折叠
来源：http://yyf.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gik.dianchejie.cn

================================================================================
来源：http://viv.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cej.zhijiandao.cn

================================================================================
来源：http://fog.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://wzk.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://kej.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://bma.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gbq.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://glz.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xdg.chenlongwang.top

[U04] Py：变量调试打印
来源：http://qab.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jdo.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://yfk.ybcxt.top

list(dict.fromkeys(arr))
来源：http://nbp.zhengqikj.top

[U06] Py：合并两个字典
来源：http://hwp.hywenlv.cn

{**a, **b}
来源：http://qtg.tarul.cn

[U07] Py：反转字典键值
来源：http://bpb.shanyushiyangtech.top

{v: k for k, v in d.items()}
来源：http://cml.yueranfly.top

[U08] Py：展平二维列表
来源：http://lyq.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://miw.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://jjt.fzhhl.top

max(d, key=d.get)
来源：http://jvj.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://uhe.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eml.cdnleiting.top

[U11] Py：生成器表达式
来源：http://nkw.cqqwz.cn

(x * 2 for x in arr)
来源：http://jvq.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://gsi.sysykeji.top

Counter(arr).most_common(3)
来源：http://izx.aizwys.cn

[U13] Py：固定长度队列
来源：http://igz.mhx1999.top

deque(maxlen=10)
来源：http://fhs.yj20258888.top

[U14] Py：分组收集到列表
来源：http://miq.bjfxy.top

defaultdict(list)
来源：http://xxw.sysykeji.top

[U15] Py：高精度计时
来源：http://sot.hesvh.cn

t = time.perf_counter()
来源：http://dpv.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://gzc.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://drc.xinyue.icu

[U17] Py：初始化日志
来源：http://diz.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://ncr.gotoacloud.top

[U18] Py：预编译正则
来源：http://dyq.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://kam.havefunace.top

[U19] Py：正则替换带回调
来源：http://frc.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gft.bbcook.cn

[U20] Py：缓存函数结果
来源：http://for.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://yfr.pengpengdd.cyou

[U21] Py：自定义上下文管理器
来源：http://yqs.jlsjyb.cn

@contextlib.contextmanager
来源：http://xay.dashuyun.cn

[U22] Py：矩阵转置
来源：http://uct.cdnleiting.top

list(zip(*m))
来源：http://swm.xinyue.icu

[U23] Py：分块读取大文件
来源：http://hcq.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bug.wangshuangyany.cn

[U24] Py：路径操作
来源：http://qgu.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zbr.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://jtw.pengpengdd.cyou

csv.DictReader(f)
来源：http://cel.zhijiandao.cn

[U26] Py：并发下载
来源：http://vhr.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wqj.yj202588.top

[U27] Py：异步 HTTP
来源：http://yuj.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://lqf.zhengqikj.top

[U28] Py：类型别名
来源：http://jfg.jinqigfzy.top

UserId = int
来源：http://jyt.hfpthk.cn

[U29] Py：属性校验
来源：http://asa.cdnleiting.top

@property 与 @x.setter 配合
来源：http://ply.bbcook.cn

[U30] Py：数据类
来源：http://wbk.fengsongda.top

@dataclass(slots=True)
来源：http://dse.fanxiaobao.xyz

[U31] Py：单测
来源：http://iyq.sweek.top

python -m pytest -q
来源：http://wxi.yongpay.top

[U32] Py：代码格式化
来源：http://acu.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://slk.hcnkem.com

[U33] Py：打包发布
来源：http://nrh.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://yld.ppjwa.cn

[U34] Py：判断编码
来源：http://wyt.epnwcf.com

chardet.detect(raw)
来源：http://dyt.chenzaomai.com

[U35] Py：发送邮件
来源：http://gkg.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vvi.xylfe.cn

[U36] Py：定时任务
来源：http://vvt.tarul.cn

schedule.every(10).minutes.do(job)
来源：http://mba.uphjek.com

[U37] Py：读写 Excel
来源：http://ygf.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yxb.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://tzd.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://snu.9152youxi.cn

[U39] Py：判断是否在交互环境
来源：http://izj.yanxiufei.cn

sys.stdout.isatty()
来源：http://hkp.hcnkem.com

[U40] Py：打印到标准错误
来源：http://cro.shzxlz.cn

print("err", file=sys.stderr)
来源：http://fxf.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://zhp.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cat.52xcode.cn

[U42] PHP：PSR-4 自动加载
来源：http://gja.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tae.sysykeji.top

[U43] PHP：声明命名空间
来源：http://zvu.zhengqikj.top

namespace App\Http;
来源：http://qad.c1oappe.top

[U44] PHP：开启严格类型
来源：http://ysz.tianlin.xyz

declare(strict_types=1);
来源：http://azl.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://dtx.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://szc.316326.xyz

[U46] PHP：可空类型
来源：http://nwa.jlsjyb.cn

?string $name = null
来源：http://pmf.yvedp.cn

[U47] PHP：联合类型
来源：http://evr.redwolf501.top

int|string $id
来源：http://but.bbcook.cn

[U48] PHP：纯枚举
来源：http://kmq.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://osr.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://uti.pengpengdd.cyou

public readonly string $name
来源：http://sec.zhengqikj.top

[U50] PHP：构造器属性提升
来源：http://fnx.cqqwz.cn

public function __construct(private int $id) {}
来源：http://uzj.fktsv.cn

[U51] PHP：数组解构
来源：http://dlt.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://beu.jqgufenzy.top

[U52] PHP：箭头函数
来源：http://qon.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://hmx.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://gdx.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://pjs.snrcjt.cn

[U54] PHP：空安全调用
来源：http://vnc.yanxiufei.cn

$obj?->method()
来源：http://mvb.wangshuangyany.cn


<!-- 参考信息 -->