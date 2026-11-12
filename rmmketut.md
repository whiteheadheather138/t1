代发 wailian999

#include <iostream>
来源：http://ons.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://pyw.yongpay.top

[S32] C++：字符串
来源：http://hdd.yj20258.top

std::string s = "hi";  s += "!";
来源：http://arx.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://cpe.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ogy.cqqwz.cn

[S34] C++：遍历 vector
来源：http://ldm.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://xvh.hcnkem.com

[S35] C++：map
来源：http://gbt.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dkz.vehdjk.com

[S36] C++：unordered_map
来源：http://ivh.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lmz.yongpay.top

[S37] C++：set
来源：http://gxd.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kxe.aibaodan.cn

[S38] C++：排序
来源：http://zst.tanke756.top

std::sort(v.begin(), v.end());
来源：http://yvw.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://lfx.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rwo.bbcook.cn

[S40] C++：查找元素
来源：http://jes.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lmn.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://twd.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ovq.yongpay.top

[S42] C++：继承与虚函数
来源：http://jyw.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://oru.guannengcc.top

[S43] C++：智能指针
来源：http://gzu.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://brg.sxryk.cn

[S44] C++：引用传参
来源：http://alx.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://dqp.jyoumei.cn

[S45] C++：lambda
来源：http://ylg.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jws.yvedp.cn

[S46] C++：函数模板
来源：http://ixa.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mps.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://zsg.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iaj.sweek.top

[S48] C++：逐行读文件
来源：http://ykh.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://ylz.andypj.xyz

while (std::getline(in, line)) { }
来源：http://bgd.hysaishi.cn

[S49] C++：写文件
来源：http://nhf.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hir.c1oappe.top

[S50] C++：格式化数字
来源：http://ina.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rmp.ybcxt.top

[S51] C++：显式类型转换
来源：http://umu.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://gde.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://fhh.sweek.top

int size() const noexcept { return n_; }
来源：http://qof.cucudq.cn

[S53] C++：移动语义
来源：http://uky.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://khg.daxiang520.top

[S54] C++：异常处理
来源：http://mjj.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cwf.sysykeji.top

[S55] C++：结构化绑定
来源：http://sda.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ybq.xuetiantiany.cn

[S56] C++：optional
来源：http://vpf.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crg.gzhubu.top

[S57] C++：编译期常量
来源：http://osx.fktsv.cn

constexpr int N = 10;
来源：http://mrn.shuidangran.top

[S58] C++：命名空间
来源：http://zof.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://www.uphjek.com

[S59] C++：静态断言
来源：http://jpm.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gud.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://fdb.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ztd.xuanzx.com

================================================================================
来源：http://jxz.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://erg.52xcode.cn

================================================================================
来源：http://xnl.iojbl.cn

[T01] Kotlin：Hello World
来源：http://usj.jinyuanbaomall.cn

println("Hello")
来源：http://ppr.yonumen.top

[T02] Kotlin：变量
来源：http://qzo.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dls.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://nis.fehbvm.com

"值: $b"
来源：http://fav.zhengqikj.top

[T04] Kotlin：空安全
来源：http://glz.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://wfy.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://dyh.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tfb.mhx1999.top

[T06] Kotlin：集合映射
来源：http://kpf.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nfb.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://ogn.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://kme.zdbjq.cn

[T08] Kotlin：数据类
来源：http://gkh.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://tyt.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://zsc.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://ayl.yfazqb.com

[T10] Kotlin：默认参数
来源：http://bta.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oao.yj202588.top

[T11] Kotlin：协程
来源：http://jae.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://mqs.yfazqb.com

[T12] Kotlin：解构声明
来源：http://pjr.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://ung.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://guy.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://gvb.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://ngw.xuanzx.com

for (i in 1..10) println(i)
来源：http://crr.cashguo.top

[T15] Kotlin：接口
来源：http://ubb.hcnkem.com

interface Shape { fun area(): Double }
来源：http://oiz.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://tew.yj202588.top

print("Hello")
来源：http://cml.zdqjudy.top

[T17] Swift：变量与常量
来源：http://seu.ctjpmb.com

var a = 1;  let b = 2
来源：http://izh.aibaodan.cn

[T18] Swift：字符串插值
来源：http://hfd.sjlbkw.cn

"值: \(b)"
来源：http://pyk.havefunace.top

[T19] Swift：可选绑定
来源：http://smy.zhengqikj.top

if let n = opt { print(n) }
来源：http://joz.cdnleiting.top

[T20] Swift：数组操作
来源：http://con.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rqx.zhijiandao.cn

[T21] Swift：遍历
来源：http://mks.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://lwm.zhijiandao.cn

[T22] Swift：字典
来源：http://jmf.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gan.jinqigufen.top

[T23] Swift：函数
来源：http://jgo.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ndv.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://nzm.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bqx.chenzaomai.com

[T25] Swift：结构体
来源：http://hut.kuanghao11.cn

struct P { var x: Int }
来源：http://nms.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://fda.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://vte.havefunace.top

[T27] Swift：错误处理
来源：http://pma.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://nfx.svipenyu.cn

[T28] Swift：枚举
来源：http://uhb.cdnleiting.top

enum Color { case red, green }
来源：http://xat.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://fpf.hfpthk.cn

guard let x = opt else { return }
来源：http://evq.hysaishi.cn

[T30] Swift：协议
来源：http://jps.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://dad.gotoacloud.top

[T31] Lua：Hello World
来源：http://mdi.shanyushiyangkeji.top

print("Hello")
来源：http://zfv.nanxinkj.top

[T32] Lua：局部变量
来源：http://xaq.aibaodan.cn

local a = 1
来源：http://ots.yuxming.cn

[T33] Lua：表（数组）
来源：http://kcr.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://tha.yueranfly.top

[T34] Lua：遍历表
来源：http://ohp.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lgl.snrcjt.cn

[T35] Lua：字典表
来源：http://vog.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://err.zhijiandao.cn

[T36] Lua：函数
来源：http://frd.gzhubu.top

function add(a, b) return a + b end
来源：http://vvr.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://umc.c1oappe.top

"a" .. "b"
来源：http://wco.52xcode.cn

[T38] Lua：条件
来源：http://zqo.jinqigufen.top

if x > 0 then print("正") end
来源：http://wya.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://yeb.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://ptw.guannengcc.top

[T40] Lua：元表
来源：http://llr.smart0.xyz

setmetatable({}, { __index = base })
来源：http://pjb.yj202588.top

[T41] Perl：Hello World
来源：http://wiz.vehdjk.com

print "Hello\n";
来源：http://jiq.hysaishi.cn

[T42] Perl：变量类型
来源：http://hfy.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://puf.hfpthk.cn

[T43] Perl：字符串插值
来源：http://pxd.epnwcf.com

"值: $a"
来源：http://mdy.sweek.top

[T44] Perl：条件
来源：http://sjv.pycfn.com

if ($a > 0) { print "正"; }
来源：http://wju.52xcode.cn

[T45] Perl：数组遍历
来源：http://bon.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://qbn.meibo888.top

[T46] Perl：哈希操作
来源：http://qnz.yvedp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sem.yonumen.top

[T47] Perl：正则捕获
来源：http://xao.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fqm.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://dsk.jyoumei.cn

$s =~ s/old/new/g;
来源：http://mvc.tian-w.cn

[T49] Perl：函数
来源：http://fks.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ptv.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://rke.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hra.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://zfa.jinqigufen.top

[T51] Scala：Hello World
来源：http://tsv.c1oappe.top

println("Hello")
来源：http://xif.nanxinkj.top

[T52] Scala：变量
来源：http://lok.cqqwz.cn

val a = 1;  var b = 2
来源：http://ink.yfazqb.com

[T53] Scala：字符串插值
来源：http://pev.gotoacloud.top

s"值: $b"
来源：http://mev.ctjpmb.com

[T54] Scala：集合映射
来源：http://icm.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://uns.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://hni.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://los.zdbjq.cn

[T56] Scala：样例类
来源：http://kle.daria6918.cn

case class User(name: String, age: Int)
来源：http://mls.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://ywb.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://boh.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://rpl.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vsa.hysaishi.cn

[T59] Scala：循环
来源：http://rxy.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://vnr.yvedp.cn

[T60] Scala：折叠
来源：http://obl.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://stz.zdqjudy.top

================================================================================
来源：http://mck.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kfq.sjlbkw.cn

================================================================================
来源：http://pjf.birdmap.top

[U01] Py：创建虚拟环境
来源：http://sxq.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://hez.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://cru.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://loo.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://upx.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jrf.zdbjq.cn

[U04] Py：变量调试打印
来源：http://arp.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://crc.ybcxt.top

[U05] Py：列表去重且保序
来源：http://caz.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://kxm.guowangkeji.top

[U06] Py：合并两个字典
来源：http://vlp.jianghu66.top

{**a, **b}
来源：http://lis.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://egk.xylfe.cn

{v: k for k, v in d.items()}
来源：http://cql.yj20258.top

[U08] Py：展平二维列表
来源：http://bmm.chenlongwang.top

[y for x in nested for y in x]
来源：http://qdl.yonumen.top

[U09] Py：字典取最大值的键
来源：http://tpb.pycfn.com

max(d, key=d.get)
来源：http://ich.yongpay.top

[U10] Py：按值排序字典
来源：http://wbu.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jmt.cucudq.cn

[U11] Py：生成器表达式
来源：http://mfc.9152youxi.cn

(x * 2 for x in arr)
来源：http://rtk.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://yvo.shuidangran.top

Counter(arr).most_common(3)
来源：http://nai.yfazqb.com

[U13] Py：固定长度队列
来源：http://jla.guowangkeji.top

deque(maxlen=10)
来源：http://qig.ivvv.top

[U14] Py：分组收集到列表
来源：http://mql.yuxming.cn

defaultdict(list)
来源：http://byb.dashuyun.cn

[U15] Py：高精度计时
来源：http://xtg.zhengqikj.top

t = time.perf_counter()
来源：http://mns.yj20258.top

[U16] Py：命令行参数解析
来源：http://cja.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vup.jiagoushi.top

[U17] Py：初始化日志
来源：http://xhl.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://xby.nwbrower.top

[U18] Py：预编译正则
来源：http://qod.hesvh.cn

pat = re.compile(r"\d+")
来源：http://qhf.nanxuanxn.top

[U19] Py：正则替换带回调
来源：http://gpu.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lvh.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://wkh.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://xud.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://jkv.nanxuanxn.top

@contextlib.contextmanager
来源：http://jjd.sxryk.cn

[U22] Py：矩阵转置
来源：http://zms.zhoulong.xyz

list(zip(*m))
来源：http://luk.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://xur.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://epv.haohaochexian.top

[U24] Py：路径操作
来源：http://cjd.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://exp.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://iee.yuxming.cn

csv.DictReader(f)
来源：http://wxx.hnqzz.top

[U26] Py：并发下载
来源：http://wnw.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jfc.nwbrower.top

[U27] Py：异步 HTTP
来源：http://fyt.9152youxi.cn

aiohttp.ClientSession() 配合 async with
来源：http://tvm.svipenyu.cn

[U28] Py：类型别名
来源：http://fug.fktsv.cn

UserId = int
来源：http://cxe.fehbvm.com

[U29] Py：属性校验
来源：http://gnu.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://xqe.xziqi.cn

[U30] Py：数据类
来源：http://svz.zycfv.cn

@dataclass(slots=True)
来源：http://txk.cashguo.top

[U31] Py：单测
来源：http://wfo.bjfxy.top

python -m pytest -q
来源：http://mhs.xziqi.cn

[U32] Py：代码格式化
来源：http://ize.fzhhl.top

ruff format . && ruff check --fix .
来源：http://xog.gogol.net.cn

[U33] Py：打包发布
来源：http://txj.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://nyq.jianghu66.top

[U34] Py：判断编码
来源：http://noj.wangshuangyany.cn

chardet.detect(raw)
来源：http://xkp.cqqwz.cn

[U35] Py：发送邮件
来源：http://shh.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vob.mhx1999.top

[U36] Py：定时任务
来源：http://jvf.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://rae.vehdjk.com

[U37] Py：读写 Excel
来源：http://ucw.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bru.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://uxy.guannengcc.top

Path(__file__).resolve().parent
来源：http://ysp.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://nec.quarkkingdee.top

sys.stdout.isatty()
来源：http://bjk.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://lsc.birdmap.top

print("err", file=sys.stderr)
来源：http://rjg.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://cyl.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://vfs.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://qfc.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zpp.tanke756.top

[U43] PHP：声明命名空间
来源：http://oih.jlsjyb.cn

namespace App\Http;
来源：http://yoo.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://wfd.ybcxt.top

declare(strict_types=1);
来源：http://enh.gotoacloud.top

[U45] PHP：类型声明与返回类型
来源：http://aue.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://btm.yongpay.top

[U46] PHP：可空类型
来源：http://iqx.chenjidiqi.icu

?string $name = null
来源：http://dzd.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://oqe.haohaochexian.top

int|string $id
来源：http://mid.dianchejie.cn

[U48] PHP：纯枚举
来源：http://ezc.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bjv.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://iyc.ydzc1.top

public readonly string $name
来源：http://vzs.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://red.sxryk.cn

public function __construct(private int $id) {}
来源：http://pkp.wangdashe.top

[U51] PHP：数组解构
来源：http://uwh.iojbl.cn

[$a, $b] = $arr;
来源：http://oqn.chenlongwang.top

[U52] PHP：箭头函数
来源：http://eoj.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://bkc.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://tmj.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://vvf.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://ufy.sjlbkw.cn

$obj?->method()
来源：http://pza.sufxvd.cn

[U55] PHP：match 表达式
来源：http://yoc.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xuk.hesvh.cn

[U56] PHP：命名参数
来源：http://xoc.zdqjudy.top

f(a: 1, b: 2)
来源：http://mjm.zycfv.cn


<!-- 参考信息 -->