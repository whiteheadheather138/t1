代发 wailian999

[S33] C++：vector 增删
来源：http://fvm.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uyj.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://uhm.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://qbh.zhijiandao.cn

[S35] C++：map
来源：http://guq.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://frb.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://bmp.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aow.sufxvd.cn

[S37] C++：set
来源：http://sof.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ecq.c1oappe.top

[S38] C++：排序
来源：http://uqn.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://wpr.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://itv.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nza.yj202588.top

[S40] C++：查找元素
来源：http://iys.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vey.hfpthk.cn

[S41] C++：类与构造函数
来源：http://aji.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jcz.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://elp.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://rkl.haohaochexian.top

[S43] C++：智能指针
来源：http://byu.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://ojj.fengsongda.top

[S44] C++：引用传参
来源：http://ffl.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://rgr.zhoulong.xyz

[S45] C++：lambda
来源：http://nqr.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://pmi.daxiang520.top

[S46] C++：函数模板
来源：http://lbo.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://egc.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://zoo.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zvc.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://qxu.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://fww.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://qds.chenlongwang.top

[S49] C++：写文件
来源：http://wvp.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zxz.yj20258.top

[S50] C++：格式化数字
来源：http://ixc.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xvs.tian-w.cn

[S51] C++：显式类型转换
来源：http://vtq.yfazqb.com

static_cast<double>(a) / b
来源：http://gxo.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://zdi.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://mcn.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://fvx.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://xol.yonumen.top

[S54] C++：异常处理
来源：http://bfz.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uwr.nwbrower.top

[S55] C++：结构化绑定
来源：http://wcz.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gyr.fanxiaobao.xyz

[S56] C++：optional
来源：http://vhz.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sfl.hcnkem.com

[S57] C++：编译期常量
来源：http://zvp.redwolf501.top

constexpr int N = 10;
来源：http://fki.yuanzhike.top

[S58] C++：命名空间
来源：http://scd.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://una.xziqi.cn

[S59] C++：静态断言
来源：http://tcy.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://myg.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://kij.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhf.zycfv.cn

================================================================================
来源：http://ryt.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kvr.yj20258888.top

================================================================================
来源：http://mcc.yj202588.top

[T01] Kotlin：Hello World
来源：http://rni.shzxlz.cn

println("Hello")
来源：http://qrn.yongpay.top

[T02] Kotlin：变量
来源：http://cfz.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ejo.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://zcx.sufxvd.cn

"值: $b"
来源：http://kri.yuxming.cn

[T04] Kotlin：空安全
来源：http://dov.cqqwz.cn

val n: String? = null;  n?.length
来源：http://rih.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://oun.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oyf.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://kkt.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bqa.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://xeh.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://amr.zhengqikj.top

[T08] Kotlin：数据类
来源：http://ayz.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://aht.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://jhg.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://txp.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://sqa.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iwj.jlsjyb.cn

[T11] Kotlin：协程
来源：http://ywt.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kik.ybcxt.top

[T12] Kotlin：解构声明
来源：http://usd.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://hro.uphjek.com

[T13] Kotlin：只读 Map
来源：http://vmj.aizwys.cn

val m = mapOf("a" to 1)
来源：http://fsi.xylfe.cn

[T14] Kotlin：循环
来源：http://dzq.yj202588.top

for (i in 1..10) println(i)
来源：http://oqx.fktsv.cn

[T15] Kotlin：接口
来源：http://xkd.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://tse.yj20258.top

[T16] Swift：Hello World
来源：http://xeh.pycfn.com

print("Hello")
来源：http://fku.yuanzhike.top

[T17] Swift：变量与常量
来源：http://bkc.hywenlv.cn

var a = 1;  let b = 2
来源：http://otq.gotoacloud.top

[T18] Swift：字符串插值
来源：http://mib.xinyue.icu

"值: \(b)"
来源：http://zue.jyoumei.cn

[T19] Swift：可选绑定
来源：http://xfy.fktsv.cn

if let n = opt { print(n) }
来源：http://bfp.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://gjv.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://qdg.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://xul.bbcook.cn

for x in a { print(x) }
来源：http://jbd.zhixingplan.top

[T22] Swift：字典
来源：http://snp.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://wfg.316326.xyz

[T23] Swift：函数
来源：http://jna.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cpb.fengsongda.top

[T24] Swift：闭包
来源：http://msc.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ywp.chenlongwang.top

[T25] Swift：结构体
来源：http://edf.9152youxi.cn

struct P { var x: Int }
来源：http://vpw.hysaishi.cn

[T26] Swift：类与重写
来源：http://xgz.yongpay.top

class A: Base { override func f() {} }
来源：http://fro.jinqigufen.top

[T27] Swift：错误处理
来源：http://dsy.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://rls.sjlbkw.cn

[T28] Swift：枚举
来源：http://ihz.hnqzz.top

enum Color { case red, green }
来源：http://pkj.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://yss.yj202588.top

guard let x = opt else { return }
来源：http://twa.aizwys.cn

[T30] Swift：协议
来源：http://gjh.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://ymx.bbcook.cn

[T31] Lua：Hello World
来源：http://djb.cdnleiting.top

print("Hello")
来源：http://keb.yueranfly.top

[T32] Lua：局部变量
来源：http://nrw.tanke756.top

local a = 1
来源：http://qyp.chenlongwang.top

[T33] Lua：表（数组）
来源：http://yzi.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://omh.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://doq.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wmt.aibaodan.cn

[T35] Lua：字典表
来源：http://dps.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://utf.nanxuanxn.top

[T36] Lua：函数
来源：http://rlu.svipenyu.cn

function add(a, b) return a + b end
来源：http://xze.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://sqe.cdnleiting.top

"a" .. "b"
来源：http://xmp.wangshuangyany.cn

[T38] Lua：条件
来源：http://afi.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://bmz.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://lpr.yuxming.cn

string.find(s, "%d+")
来源：http://enq.sysykeji.top

[T40] Lua：元表
来源：http://xir.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://xqj.cdnleiting.top

[T41] Perl：Hello World
来源：http://pwn.52xcode.cn

print "Hello\n";
来源：http://kow.fengsongda.top

[T42] Perl：变量类型
来源：http://ufn.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rom.xinyue.icu

[T43] Perl：字符串插值
来源：http://ooj.ctjpmb.com

"值: $a"
来源：http://var.dashuyun.cn

[T44] Perl：条件
来源：http://hlc.svipenyu.cn

if ($a > 0) { print "正"; }
来源：http://hsa.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://wvx.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://wme.redwolf501.top

[T46] Perl：哈希操作
来源：http://dpr.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tie.316326.xyz

[T47] Perl：正则捕获
来源：http://jfh.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://hkt.ydjk.org.cn

[T48] Perl：正则替换
来源：http://hks.snrcjt.cn

$s =~ s/old/new/g;
来源：http://trx.xuetiantiany.cn

[T49] Perl：函数
来源：http://mcv.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://smm.316326.xyz

[T50] Perl：逐行读文件
来源：http://gni.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://mjm.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://jss.svipenyu.cn

[T51] Scala：Hello World
来源：http://ezz.yanxiufei.cn

println("Hello")
来源：http://nim.sufxvd.cn

[T52] Scala：变量
来源：http://qwa.wangdashe.top

val a = 1;  var b = 2
来源：http://ghk.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://icj.yvedp.cn

s"值: $b"
来源：http://zxp.gaohongyu789.top

[T54] Scala：集合映射
来源：http://eld.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://vap.smart0.xyz

[T55] Scala：集合过滤
来源：http://qup.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://aks.sysykeji.top

[T56] Scala：样例类
来源：http://hsg.xylfe.cn

case class User(name: String, age: Int)
来源：http://cmk.chenzaomai.com

[T57] Scala：模式匹配
来源：http://zek.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kpr.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://nkj.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://msw.zhoulong.xyz

[T59] Scala：循环
来源：http://ljh.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://oua.xuanzx.com

[T60] Scala：折叠
来源：http://qeb.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fbq.jyoumei.cn

================================================================================
来源：http://ckv.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zib.gotoacloud.top

================================================================================
来源：http://msg.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://pbj.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://fzq.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://qge.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ees.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://pip.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://adt.zdqjudy.top

[U04] Py：变量调试打印
来源：http://dbe.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aix.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://fvu.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://dav.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://yot.nwbrower.top

{**a, **b}
来源：http://dfd.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://bsg.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://qln.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://bvr.yj20258.top

[y for x in nested for y in x]
来源：http://pqn.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://bll.yfazqb.com

max(d, key=d.get)
来源：http://rzc.bjfxy.top

[U10] Py：按值排序字典
来源：http://fmk.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xdb.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://yyd.uphjek.com

(x * 2 for x in arr)
来源：http://kmy.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://xfi.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://azs.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://idi.zdqjudy.top

deque(maxlen=10)
来源：http://fkt.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://iaf.yj202588.top

defaultdict(list)
来源：http://kza.fengsongda.top

[U15] Py：高精度计时
来源：http://brv.sjlbkw.cn

t = time.perf_counter()
来源：http://ybt.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://twh.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mug.sweek.top

[U17] Py：初始化日志
来源：http://yrp.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://gls.xuanzx.com

[U18] Py：预编译正则
来源：http://vsj.xylfe.cn

pat = re.compile(r"\d+")
来源：http://oit.gzhubu.top

[U19] Py：正则替换带回调
来源：http://pvm.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://guj.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://ofm.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://jcy.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://dgj.jinqigfzy.top

@contextlib.contextmanager
来源：http://zdz.uphjek.com

[U22] Py：矩阵转置
来源：http://fsd.epnwcf.com

list(zip(*m))
来源：http://thu.yj202588.top

[U23] Py：分块读取大文件
来源：http://wla.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esl.aizwys.cn

[U24] Py：路径操作
来源：http://mwy.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uwk.birdmap.top

[U25] Py：CSV 按字典读
来源：http://erv.yonumen.top

csv.DictReader(f)
来源：http://sei.xinyue.icu

[U26] Py：并发下载
来源：http://lin.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eqz.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://eal.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://vrw.smart0.xyz

[U28] Py：类型别名
来源：http://ash.hnxiangtu.top

UserId = int
来源：http://wiy.smart0.xyz

[U29] Py：属性校验
来源：http://ysh.uphjek.com

@property 与 @x.setter 配合
来源：http://lvf.nanxuanxn.top

[U30] Py：数据类
来源：http://qem.ppjwa.cn

@dataclass(slots=True)
来源：http://slb.hnxiangtu.top

[U31] Py：单测
来源：http://wvj.sjlbkw.cn

python -m pytest -q
来源：http://eqt.cdnleiting.top

[U32] Py：代码格式化
来源：http://szz.sxryk.cn

ruff format . && ruff check --fix .
来源：http://seu.zhiwuduotai.top

[U33] Py：打包发布
来源：http://umw.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://sub.hongshengwenyu.top

[U34] Py：判断编码
来源：http://zzg.yonumen.top

chardet.detect(raw)
来源：http://tpw.fktsv.cn

[U35] Py：发送邮件
来源：http://wwk.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iaq.daxiang520.top

[U36] Py：定时任务
来源：http://tam.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://fxm.yvedp.cn

[U37] Py：读写 Excel
来源：http://urf.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://sdx.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://ezl.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://nzo.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://fgh.birdmap.top

sys.stdout.isatty()
来源：http://sek.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://kpj.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://kqs.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://wqa.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cyf.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://tmf.jyoumei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://drv.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://kap.9152youxi.cn

namespace App\Http;
来源：http://yku.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://amq.guowangkeji.top

declare(strict_types=1);
来源：http://edd.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://alg.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://azu.0kj1m.cn

[U46] PHP：可空类型
来源：http://gla.yj20258888.top

?string $name = null
来源：http://ptc.zhiwuduotai.top

[U47] PHP：联合类型
来源：http://yie.hongshengwenyu.top

int|string $id
来源：http://nga.sysykeji.top

[U48] PHP：纯枚举
来源：http://mcp.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://iwo.xziqi.cn

[U49] PHP：只读属性
来源：http://mcp.shanyushiyangkeji.top

public readonly string $name
来源：http://nwr.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://upf.cheryme.top

public function __construct(private int $id) {}
来源：http://gzh.sufxvd.cn

[U51] PHP：数组解构
来源：http://pdg.dianchejie.cn

[$a, $b] = $arr;
来源：http://zko.chenzaomai.com

[U52] PHP：箭头函数
来源：http://zrn.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://axm.havefunace.top

[U53] PHP：空合并运算符
来源：http://jvx.ehwqpu.com

$v = $a ?? $b ?? "default";
来源：http://isi.cqqwz.cn

[U54] PHP：空安全调用
来源：http://atq.ivvv.top

$obj?->method()
来源：http://jnn.daria6918.cn

[U55] PHP：match 表达式
来源：http://lgg.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ehu.yuxming.cn

[U56] PHP：命名参数
来源：http://byv.shuidangran.top

f(a: 1, b: 2)
来源：http://wur.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://zko.haohaochexian.top

"值: {$a}"
来源：http://ckq.tianlin.xyz

[U58] PHP：数组三件套
来源：http://rsp.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ffr.xuanzx.com


<!-- 参考信息 -->