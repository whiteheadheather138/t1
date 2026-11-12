代发 wailian999

[S33] C++：vector 增删
来源：http://hdj.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wbt.havefunace.top

[S34] C++：遍历 vector
来源：http://zlw.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://oji.tanke756.top

[S35] C++：map
来源：http://unw.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qqf.hnxiangtu.top

[S36] C++：unordered_map
来源：http://esm.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ktz.ivvv.top

[S37] C++：set
来源：http://hrc.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ksp.yj20258.top

[S38] C++：排序
来源：http://qfx.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://txk.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://svn.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nng.snrcjt.cn

[S40] C++：查找元素
来源：http://gco.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uwh.ppjwa.cn

[S41] C++：类与构造函数
来源：http://mwl.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iph.ydzc1.top

[S42] C++：继承与虚函数
来源：http://ekb.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://jyr.cashguo.top

[S43] C++：智能指针
来源：http://bmu.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://rbz.fehbvm.com

[S44] C++：引用传参
来源：http://wcj.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://nrn.tarul.cn

[S45] C++：lambda
来源：http://vye.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://idw.andypj.xyz

[S46] C++：函数模板
来源：http://fdh.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hzt.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://oyk.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kzq.cdnleiting.top

[S48] C++：逐行读文件
来源：http://lpd.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://jgp.pycfn.com

while (std::getline(in, line)) { }
来源：http://pky.cqqwz.cn

[S49] C++：写文件
来源：http://bmn.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lsi.guannengcc.top

[S50] C++：格式化数字
来源：http://wnt.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://avc.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://cwr.jinqigufen.top

static_cast<double>(a) / b
来源：http://ojs.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://ehf.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://rpu.bjfxy.top

[S53] C++：移动语义
来源：http://ukg.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://qmp.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://eqq.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iuu.cheryme.top

[S55] C++：结构化绑定
来源：http://xzy.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fbn.jqgfzy.top

[S56] C++：optional
来源：http://gix.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://akv.vqdsnc.cn

[S57] C++：编译期常量
来源：http://gjh.zhoulong.xyz

constexpr int N = 10;
来源：http://yus.pengpengdd.cyou

[S58] C++：命名空间
来源：http://zyt.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://gba.xinyue.icu

[S59] C++：静态断言
来源：http://omg.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ggp.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://ych.tanke756.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gbu.mhx1999.top

================================================================================
来源：http://pfr.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://auq.0kj1m.cn

================================================================================
来源：http://ins.yvedp.cn

[T01] Kotlin：Hello World
来源：http://que.dashuyun.cn

println("Hello")
来源：http://hqh.sysykeji.top

[T02] Kotlin：变量
来源：http://ynw.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://akj.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://qca.meibo888.top

"值: $b"
来源：http://jbg.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://bna.yvedp.cn

val n: String? = null;  n?.length
来源：http://yrs.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://fwo.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qfg.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://fos.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rbj.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://pkl.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wmp.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://fso.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://jzf.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://pwq.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://gnt.yvedp.cn

[T10] Kotlin：默认参数
来源：http://reu.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nay.bjfxy.top

[T11] Kotlin：协程
来源：http://riu.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hvf.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://ulb.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://scu.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://xui.yj202588.top

val m = mapOf("a" to 1)
来源：http://lyi.ivvv.top

[T14] Kotlin：循环
来源：http://nwg.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://kyd.dianchejie.cn

[T15] Kotlin：接口
来源：http://vvc.cashguo.top

interface Shape { fun area(): Double }
来源：http://rdi.guannengcc.top

[T16] Swift：Hello World
来源：http://aba.chenjidiqi.icu

print("Hello")
来源：http://jhc.birdmap.top

[T17] Swift：变量与常量
来源：http://pqk.9152youxi.cn

var a = 1;  let b = 2
来源：http://puj.hysaishi.cn

[T18] Swift：字符串插值
来源：http://jpm.yonumen.top

"值: \(b)"
来源：http://udz.tanke756.top

[T19] Swift：可选绑定
来源：http://ktn.yfazqb.com

if let n = opt { print(n) }
来源：http://axf.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://pkc.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://kdn.hnxiangtu.top

[T21] Swift：遍历
来源：http://qwt.hongshengwenyu.top

for x in a { print(x) }
来源：http://wjt.xylfe.cn

[T22] Swift：字典
来源：http://jrz.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qvh.jinghuilouyu.cn

[T23] Swift：函数
来源：http://cor.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qpq.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://jzx.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nig.bbcook.cn

[T25] Swift：结构体
来源：http://rjh.jinqigufen.top

struct P { var x: Int }
来源：http://dce.yongpay.top

[T26] Swift：类与重写
来源：http://vfu.wangdashe.top

class A: Base { override func f() {} }
来源：http://vej.smart0.xyz

[T27] Swift：错误处理
来源：http://bdh.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://ril.jinqigfzy.top

[T28] Swift：枚举
来源：http://lyk.hesvh.cn

enum Color { case red, green }
来源：http://mzv.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://abq.zhixingplan.top

guard let x = opt else { return }
来源：http://aba.havefunace.top

[T30] Swift：协议
来源：http://uuk.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://nin.smart0.xyz

[T31] Lua：Hello World
来源：http://gmf.tian-w.cn

print("Hello")
来源：http://ift.yfazqb.com

[T32] Lua：局部变量
来源：http://xop.hysaishi.cn

local a = 1
来源：http://jyt.epnwcf.com

[T33] Lua：表（数组）
来源：http://pnc.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uww.sufxvd.cn

[T34] Lua：遍历表
来源：http://wtt.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wky.yonumen.top

[T35] Lua：字典表
来源：http://zmp.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://wbk.cqqwz.cn

[T36] Lua：函数
来源：http://dzl.gzhubu.top

function add(a, b) return a + b end
来源：http://qpo.chenzaomai.com

[T37] Lua：字符串拼接
来源：http://ghk.yj20258888.top

"a" .. "b"
来源：http://cad.chenlongwang.top

[T38] Lua：条件
来源：http://pcv.sjlbkw.cn

if x > 0 then print("正") end
来源：http://ldf.jianghu66.top

[T39] Lua：模式匹配
来源：http://jut.sysykeji.top

string.find(s, "%d+")
来源：http://hzj.jyoumei.cn

[T40] Lua：元表
来源：http://zwj.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://cir.hywenlv.cn

[T41] Perl：Hello World
来源：http://dfw.guowangkeji.top

print "Hello\n";
来源：http://hrh.birdmap.top

[T42] Perl：变量类型
来源：http://ukp.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nzf.aizwys.cn

[T43] Perl：字符串插值
来源：http://rfa.9152youxi.cn

"值: $a"
来源：http://iyz.316326.xyz

[T44] Perl：条件
来源：http://vis.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://cgq.fzhhl.top

[T45] Perl：数组遍历
来源：http://jei.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://fdo.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://qoy.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://knh.hesvh.cn

[T47] Perl：正则捕获
来源：http://gds.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ltn.hesvh.cn

[T48] Perl：正则替换
来源：http://nyf.haohaochexian.top

$s =~ s/old/new/g;
来源：http://ihk.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://vhc.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uok.ivvv.top

[T50] Perl：逐行读文件
来源：http://mvz.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://npu.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://nuy.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://rwv.nanxinkj.top

println("Hello")
来源：http://mtr.gaohongyu789.top

[T52] Scala：变量
来源：http://xcs.quarkkingdee.top

val a = 1;  var b = 2
来源：http://mkf.cheryme.top

[T53] Scala：字符串插值
来源：http://wlb.fktsv.cn

s"值: $b"
来源：http://val.vqdsnc.cn

[T54] Scala：集合映射
来源：http://hoa.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://ejc.jqgfzy.top

[T55] Scala：集合过滤
来源：http://jao.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qxs.guowangkeji.top

[T56] Scala：样例类
来源：http://jei.bbcook.cn

case class User(name: String, age: Int)
来源：http://vay.cucudq.cn

[T57] Scala：模式匹配
来源：http://dbm.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hok.jqgufenzy.top

[T58] Scala：函数定义
来源：http://beo.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://auf.jqgufenzy.top

[T59] Scala：循环
来源：http://qme.yonumen.top

for (i <- 1 to 10) println(i)
来源：http://fqb.havefunace.top

[T60] Scala：折叠
来源：http://sij.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yco.jinqigufen.top

================================================================================
来源：http://jtz.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fnn.yanxiufei.cn

================================================================================
来源：http://tcq.yongpay.top

[U01] Py：创建虚拟环境
来源：http://kdg.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uam.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://tic.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dsd.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://ubx.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ccp.tanke756.top

[U04] Py：变量调试打印
来源：http://oqs.hnxiangtu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xzz.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://enk.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://fkr.nwbrower.top

[U06] Py：合并两个字典
来源：http://fcr.shanyushiyangkeji.top

{**a, **b}
来源：http://gyz.guannengcc.top

[U07] Py：反转字典键值
来源：http://nee.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://uck.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://uhi.zycfv.cn

[y for x in nested for y in x]
来源：http://fet.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://qcg.tian-w.cn

max(d, key=d.get)
来源：http://jtf.daria6918.cn

[U10] Py：按值排序字典
来源：http://ebt.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ylr.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://ply.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://ymj.yanxiufei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rjz.sxryk.cn

Counter(arr).most_common(3)
来源：http://tqh.cheryme.top

[U13] Py：固定长度队列
来源：http://xvv.yvedp.cn

deque(maxlen=10)
来源：http://tmh.hammf.cn

[U14] Py：分组收集到列表
来源：http://tex.jyoumei.cn

defaultdict(list)
来源：http://gir.zhijiandao.cn

[U15] Py：高精度计时
来源：http://ynz.yvedp.cn

t = time.perf_counter()
来源：http://yvb.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://gfu.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qdl.mhx1999.top

[U17] Py：初始化日志
来源：http://cbb.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://stq.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://gkt.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://mqf.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://dei.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hdl.gzhubu.top

[U20] Py：缓存函数结果
来源：http://gxd.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://etc.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://wan.cdnleiting.top

@contextlib.contextmanager
来源：http://tlj.snrcjt.cn

[U22] Py：矩阵转置
来源：http://xzd.zdbjq.cn

list(zip(*m))
来源：http://ibe.guannengcc.top

[U23] Py：分块读取大文件
来源：http://lhk.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hwp.cashguo.top

[U24] Py：路径操作
来源：http://xgw.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yaa.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://har.hongshengwenyu.top

csv.DictReader(f)
来源：http://pub.zhengqikj.top

[U26] Py：并发下载
来源：http://ule.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qvt.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://esl.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://dav.hongshengwenyu.top

[U28] Py：类型别名
来源：http://lvf.yangfankeji.com

UserId = int
来源：http://zek.yvedp.cn

[U29] Py：属性校验
来源：http://nap.ppjwa.cn

@property 与 @x.setter 配合
来源：http://bzm.shuidangran.top

[U30] Py：数据类
来源：http://qdr.yuxming.cn

@dataclass(slots=True)
来源：http://vrn.yanxiufei.cn

[U31] Py：单测
来源：http://vwt.jiagoushi.top

python -m pytest -q
来源：http://hks.yj20258888.top

[U32] Py：代码格式化
来源：http://nvh.aizwys.cn

ruff format . && ruff check --fix .
来源：http://xtm.epnwcf.com

[U33] Py：打包发布
来源：http://ood.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://lhh.kuanghao11.cn

[U34] Py：判断编码
来源：http://uln.bjfxy.top

chardet.detect(raw)
来源：http://bzf.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://biv.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mxq.nanxuanxn.top

[U36] Py：定时任务
来源：http://ijn.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://ixj.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://zhi.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://irb.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://wtn.gogol.net.cn

Path(__file__).resolve().parent
来源：http://wja.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://qln.smart0.xyz

sys.stdout.isatty()
来源：http://rtl.smart0.xyz

[U40] Py：打印到标准错误
来源：http://aet.vehdjk.com

print("err", file=sys.stderr)
来源：http://alh.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://vvc.hesvh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rgi.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://wgm.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qjq.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://sjn.yangfankeji.com

namespace App\Http;
来源：http://uld.hammf.cn

[U44] PHP：开启严格类型
来源：http://som.zhiwuduotai.top

declare(strict_types=1);
来源：http://vpj.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://gix.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pgt.zhixingplan.top

[U46] PHP：可空类型
来源：http://mfd.nanxuanxn.top

?string $name = null
来源：http://ont.shzxlz.cn

[U47] PHP：联合类型
来源：http://nqo.gzhubu.top

int|string $id
来源：http://ksc.gaohongyu789.top

[U48] PHP：纯枚举
来源：http://lpx.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbs.zhijiandao.cn

[U49] PHP：只读属性
来源：http://vmz.yonumen.top

public readonly string $name
来源：http://dkt.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://onp.dashuyun.cn

public function __construct(private int $id) {}
来源：http://cni.andypj.xyz

[U51] PHP：数组解构
来源：http://duj.sufxvd.cn

[$a, $b] = $arr;
来源：http://jzx.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://csm.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://tqw.cashguo.top

[U53] PHP：空合并运算符
来源：http://xqi.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://slr.sufxvd.cn

[U54] PHP：空安全调用
来源：http://pyf.daxiang520.top

$obj?->method()
来源：http://muj.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://nxy.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://swo.epnwcf.com

[U56] PHP：命名参数
来源：http://yda.sweek.top

f(a: 1, b: 2)
来源：http://dvx.shuidangran.top

[U57] PHP：字符串插值
来源：http://ane.yj20258.top

"值: {$a}"
来源：http://ekq.dianchejie.cn

[U58] PHP：数组三件套
来源：http://vma.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://auu.vehdjk.com


<!-- 参考信息 -->