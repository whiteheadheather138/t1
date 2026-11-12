代发 wailian999

#ifndef X_H
来源：http://mgl.fktsv.cn

#define X_H
来源：http://mnj.daxiang520.top

#endif
来源：http://uyk.fzhhl.top

[S31] C++：Hello World
来源：http://eiu.feifeiyinyue.top

#include <iostream>
来源：http://cmg.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://cjp.gotoacloud.top

[S32] C++：字符串
来源：http://vbh.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://eit.yueranfly.top

[S33] C++：vector 增删
来源：http://fhg.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tqu.sxryk.cn

[S34] C++：遍历 vector
来源：http://cib.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://xrj.pycfn.com

[S35] C++：map
来源：http://gfy.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vvp.0kj1m.cn

[S36] C++：unordered_map
来源：http://uij.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ibv.hnxiangtu.top

[S37] C++：set
来源：http://eat.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hez.tian-w.cn

[S38] C++：排序
来源：http://keo.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://ufw.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://xsg.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nqt.yuxming.cn

[S40] C++：查找元素
来源：http://eye.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ano.yonumen.top

[S41] C++：类与构造函数
来源：http://lpo.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wkd.c1oappe.top

[S42] C++：继承与虚函数
来源：http://mwf.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://cwq.sweek.top

[S43] C++：智能指针
来源：http://qbm.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://xdk.yuanzhike.top

[S44] C++：引用传参
来源：http://hve.cashguo.top

void inc(int &x) { ++x; }
来源：http://aej.tarul.cn

[S45] C++：lambda
来源：http://eym.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://fol.nanxinkj.top

[S46] C++：函数模板
来源：http://kgb.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fjm.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://cxj.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eqm.redwolf501.top

[S48] C++：逐行读文件
来源：http://typ.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://otr.sweek.top

while (std::getline(in, line)) { }
来源：http://fnt.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://hco.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lgm.hfpthk.cn

[S50] C++：格式化数字
来源：http://faf.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zfq.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://asa.316326.xyz

static_cast<double>(a) / b
来源：http://trd.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://ubp.tanke756.top

int size() const noexcept { return n_; }
来源：http://qph.hesvh.cn

[S53] C++：移动语义
来源：http://kzk.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://wpx.feifeiyinyue.top

[S54] C++：异常处理
来源：http://mmm.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tmu.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://uak.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kas.tanke756.top

[S56] C++：optional
来源：http://gtm.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://prd.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://tby.zycfv.cn

constexpr int N = 10;
来源：http://rcm.52xcode.cn

[S58] C++：命名空间
来源：http://boj.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://pjt.zhengqikj.top

[S59] C++：静态断言
来源：http://gso.haohaochexian.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydm.quarkkingdee.top

[S60] C++：遍历并删除元素
来源：http://jey.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tqo.pycfn.com

================================================================================
来源：http://bcp.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cbm.xuanzx.com

================================================================================
来源：http://ldg.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://qaf.aizwys.cn

println("Hello")
来源：http://qzp.c1oappe.top

[T02] Kotlin：变量
来源：http://vvh.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://abz.yj20258.top

[T03] Kotlin：字符串模板
来源：http://vlk.dianchejie.cn

"值: $b"
来源：http://swm.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://wxy.hcnkem.com

val n: String? = null;  n?.length
来源：http://nuy.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://poz.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qjh.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://rkp.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bmy.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://vzh.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bdu.jyoumei.cn

[T08] Kotlin：数据类
来源：http://spb.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://pmj.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://kdp.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://lzu.birdmap.top

[T10] Kotlin：默认参数
来源：http://meb.shzxlz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bqu.nanxuanxn.top

[T11] Kotlin：协程
来源：http://qps.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vjq.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://prh.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://qjt.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://ozx.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://fow.yj20258.top

[T14] Kotlin：循环
来源：http://zcb.daria6918.cn

for (i in 1..10) println(i)
来源：http://blr.ivvv.top

[T15] Kotlin：接口
来源：http://gge.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://fgz.gogol.net.cn

[T16] Swift：Hello World
来源：http://fio.aibaodan.cn

print("Hello")
来源：http://inr.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://ubc.dashuyun.cn

var a = 1;  let b = 2
来源：http://sjo.cheryme.top

[T18] Swift：字符串插值
来源：http://pbt.0kj1m.cn

"值: \(b)"
来源：http://iop.jianghu66.top

[T19] Swift：可选绑定
来源：http://hxh.zhengqikj.top

if let n = opt { print(n) }
来源：http://qkg.zhengqikj.top

[T20] Swift：数组操作
来源：http://jdy.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jlh.jqgufenzy.top

[T21] Swift：遍历
来源：http://glh.aizwys.cn

for x in a { print(x) }
来源：http://jxq.tarul.cn

[T22] Swift：字典
来源：http://xmy.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://und.chenjidiqi.icu

[T23] Swift：函数
来源：http://eyz.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qds.daxiang520.top

[T24] Swift：闭包
来源：http://jrr.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hjb.shuidangran.top

[T25] Swift：结构体
来源：http://ndf.ppjwa.cn

struct P { var x: Int }
来源：http://war.cheryme.top

[T26] Swift：类与重写
来源：http://gdg.bjfxy.top

class A: Base { override func f() {} }
来源：http://epd.gaohongyu789.top

[T27] Swift：错误处理
来源：http://bbp.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://bde.0kj1m.cn

[T28] Swift：枚举
来源：http://uvp.hywenlv.cn

enum Color { case red, green }
来源：http://ttl.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://shm.nanxinkj.top

guard let x = opt else { return }
来源：http://nox.yuanzhike.top

[T30] Swift：协议
来源：http://mgg.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://doo.jiagoushi.top

[T31] Lua：Hello World
来源：http://zrd.jqgfzy.top

print("Hello")
来源：http://nyc.hywenlv.cn

[T32] Lua：局部变量
来源：http://wpv.fanxiaobao.xyz

local a = 1
来源：http://pxg.0kj1m.cn

[T33] Lua：表（数组）
来源：http://fhr.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ciq.epnwcf.com

[T34] Lua：遍历表
来源：http://cjl.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ydw.chenzaomai.com

[T35] Lua：字典表
来源：http://zfm.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://rsz.uphjek.com

[T36] Lua：函数
来源：http://pib.jiagoushi.top

function add(a, b) return a + b end
来源：http://mou.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://kes.hesvh.cn

"a" .. "b"
来源：http://aya.andypj.xyz

[T38] Lua：条件
来源：http://sfj.hesvh.cn

if x > 0 then print("正") end
来源：http://zdl.aibaodan.cn

[T39] Lua：模式匹配
来源：http://cxu.zhoulong.xyz

string.find(s, "%d+")
来源：http://otk.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://vop.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://trb.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://xcq.haohaochexian.top

print "Hello\n";
来源：http://fwm.jianghu66.top

[T42] Perl：变量类型
来源：http://sdw.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://icz.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://yix.zycfv.cn

"值: $a"
来源：http://kjz.cashguo.top

[T44] Perl：条件
来源：http://zul.pycfn.com

if ($a > 0) { print "正"; }
来源：http://boj.jiagoushi.top

[T45] Perl：数组遍历
来源：http://gcp.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://zni.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://wcv.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pwc.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://dlr.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://evf.snrcjt.cn

[T48] Perl：正则替换
来源：http://pum.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://ngl.bjfxy.top

[T49] Perl：函数
来源：http://wgo.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lea.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://xhy.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eng.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://ddi.zhengqikj.top

[T51] Scala：Hello World
来源：http://cyi.jianghu66.top

println("Hello")
来源：http://zuo.nanxuanxn.top

[T52] Scala：变量
来源：http://spl.zhengqikj.top

val a = 1;  var b = 2
来源：http://ytg.ybcxt.top

[T53] Scala：字符串插值
来源：http://bhf.sweek.top

s"值: $b"
来源：http://wez.kuanghao11.cn

[T54] Scala：集合映射
来源：http://hqw.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://xmo.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://cmz.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://rnm.chenzaomai.com

[T56] Scala：样例类
来源：http://oxr.cdnleiting.top

case class User(name: String, age: Int)
来源：http://pbl.yj20258888.top

[T57] Scala：模式匹配
来源：http://iwa.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fbz.chenlongwang.top

[T58] Scala：函数定义
来源：http://ctr.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://yap.sjlbkw.cn

[T59] Scala：循环
来源：http://noi.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://fce.jqgufenzy.top

[T60] Scala：折叠
来源：http://bap.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qzg.zhengqikj.top

================================================================================
来源：http://rul.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://brx.iojbl.cn

================================================================================
来源：http://wqy.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://sgl.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qko.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://tdf.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pts.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://gln.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tyn.dashuyun.cn

[U04] Py：变量调试打印
来源：http://qrs.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kae.yonumen.top

[U05] Py：列表去重且保序
来源：http://pco.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://teh.tanke756.top

[U06] Py：合并两个字典
来源：http://tgm.vehdjk.com

{**a, **b}
来源：http://put.uphjek.com

[U07] Py：反转字典键值
来源：http://fdb.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://ajt.jiagoushi.top

[U08] Py：展平二维列表
来源：http://ieb.zycfv.cn

[y for x in nested for y in x]
来源：http://kaw.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://hzr.quarkkingdee.top

max(d, key=d.get)
来源：http://gtc.ehwqpu.com

[U10] Py：按值排序字典
来源：http://lof.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ibk.jiagoushi.top

[U11] Py：生成器表达式
来源：http://lvm.sxryk.cn

(x * 2 for x in arr)
来源：http://wxw.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://igi.shuidangran.top

Counter(arr).most_common(3)
来源：http://piv.yongpay.top

[U13] Py：固定长度队列
来源：http://frv.jqgufenzy.top

deque(maxlen=10)
来源：http://nfx.xziqi.cn

[U14] Py：分组收集到列表
来源：http://qwh.hesvh.cn

defaultdict(list)
来源：http://sin.zdqjudy.top

[U15] Py：高精度计时
来源：http://sxw.tarul.cn

t = time.perf_counter()
来源：http://aoc.havefunace.top

[U16] Py：命令行参数解析
来源：http://qzg.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xug.redwolf501.top

[U17] Py：初始化日志
来源：http://yah.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lfv.sjlbkw.cn

[U18] Py：预编译正则
来源：http://xcz.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://qzm.sysykeji.top

[U19] Py：正则替换带回调
来源：http://ksu.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yrp.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://lmo.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://awl.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://ebm.gzhubu.top

@contextlib.contextmanager
来源：http://gks.hesvh.cn

[U22] Py：矩阵转置
来源：http://tte.cheryme.top

list(zip(*m))
来源：http://ich.jinqigufen.top

[U23] Py：分块读取大文件
来源：http://qia.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gnz.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://pxn.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vjv.cdnleiting.top

[U25] Py：CSV 按字典读
来源：http://zru.jianghu66.top

csv.DictReader(f)
来源：http://wjc.ehwqpu.com

[U26] Py：并发下载
来源：http://qlr.andypj.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uus.cashguo.top

[U27] Py：异步 HTTP
来源：http://upq.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://oac.ivvv.top

[U28] Py：类型别名
来源：http://azj.gotoacloud.top

UserId = int
来源：http://fft.fzhhl.top

[U29] Py：属性校验
来源：http://xhe.hfpthk.cn

@property 与 @x.setter 配合
来源：http://hge.sjlbkw.cn

[U30] Py：数据类
来源：http://hro.nanxuanxn.top

@dataclass(slots=True)
来源：http://mbh.vqdsnc.cn

[U31] Py：单测
来源：http://hhy.jinyuanbaomall.cn

python -m pytest -q
来源：http://sna.aizwys.cn

[U32] Py：代码格式化
来源：http://fnb.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://npr.yvedp.cn

[U33] Py：打包发布
来源：http://vlo.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://wpz.nanxuanxn.top

[U34] Py：判断编码
来源：http://kgh.chenlongwang.top

chardet.detect(raw)
来源：http://fio.yonumen.top

[U35] Py：发送邮件
来源：http://dkw.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://owz.hongshengwenyu.top

[U36] Py：定时任务
来源：http://zwz.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://fqt.gotoacloud.top

[U37] Py：读写 Excel
来源：http://cnb.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://sgj.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://kcc.gotoacloud.top

Path(__file__).resolve().parent
来源：http://zrl.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://paa.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://vvl.ydzc1.top

[U40] Py：打印到标准错误
来源：http://oax.xylfe.cn

print("err", file=sys.stderr)
来源：http://fos.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://swi.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gct.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://xde.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qsg.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://ybu.dashuyun.cn

namespace App\Http;
来源：http://igh.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://ysk.xinyue.icu

declare(strict_types=1);
来源：http://whb.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://uhx.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kvj.xylfe.cn

[U46] PHP：可空类型
来源：http://uma.ppjwa.cn

?string $name = null
来源：http://zat.tanke756.top

[U47] PHP：联合类型
来源：http://yaq.jlsjyb.cn

int|string $id
来源：http://byz.hysaishi.cn

[U48] PHP：纯枚举
来源：http://mpa.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ntp.zhixingplan.top

[U49] PHP：只读属性
来源：http://sel.ybcxt.top

public readonly string $name
来源：http://mlo.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://kgi.svipenyu.cn

public function __construct(private int $id) {}
来源：http://tsm.yongpay.top

[U51] PHP：数组解构
来源：http://ahs.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://ydy.dashuyun.cn

[U52] PHP：箭头函数
来源：http://kkj.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://guf.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://gbr.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://tnm.aibaodan.cn

[U54] PHP：空安全调用
来源：http://mgh.bbcook.cn

$obj?->method()
来源：http://pcg.kuanghao11.cn


<!-- 参考信息 -->