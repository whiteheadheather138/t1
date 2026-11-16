代发 wailian999

[S33] C++：vector 增删
来源：http://rsn.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://amj.yj20258.top

[S34] C++：遍历 vector
来源：http://tqv.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://rag.gogol.net.cn

[S35] C++：map
来源：http://kpf.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lvm.316326.xyz

[S36] C++：unordered_map
来源：http://rab.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlu.hcnkem.com

[S37] C++：set
来源：http://pyb.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tcp.0kj1m.cn

[S38] C++：排序
来源：http://byq.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://ovz.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://sef.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://spc.zhiwuduotai.top

[S40] C++：查找元素
来源：http://bon.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://adm.zdbjq.cn

[S41] C++：类与构造函数
来源：http://gwm.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ycu.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://oce.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://jxu.tarul.cn

[S43] C++：智能指针
来源：http://gct.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://kff.meibo888.top

[S44] C++：引用传参
来源：http://ycq.zhiwuduotai.top

void inc(int &x) { ++x; }
来源：http://xzn.hongshengwenyu.top

[S45] C++：lambda
来源：http://dco.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://urx.ybcxt.top

[S46] C++：函数模板
来源：http://qdn.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vsr.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://wdk.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jwf.zhixingplan.top

[S48] C++：逐行读文件
来源：http://wya.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://vns.mhx1999.top

while (std::getline(in, line)) { }
来源：http://ixg.fzhhl.top

[S49] C++：写文件
来源：http://vqd.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ikz.jinqigfzy.top

[S50] C++：格式化数字
来源：http://yyc.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kfm.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://kom.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://ueh.birdmap.top

[S52] C++：const 与 noexcept
来源：http://xbu.epnwcf.com

int size() const noexcept { return n_; }
来源：http://umn.smart0.xyz

[S53] C++：移动语义
来源：http://sww.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://vsz.bbcook.cn

[S54] C++：异常处理
来源：http://dqn.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xpm.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://jza.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pxv.xinyue.icu

[S56] C++：optional
来源：http://yxi.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gvw.daria6918.cn

[S57] C++：编译期常量
来源：http://dwt.havefunace.top

constexpr int N = 10;
来源：http://nkn.dianchejie.cn

[S58] C++：命名空间
来源：http://ujx.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://ifh.smart0.xyz

[S59] C++：静态断言
来源：http://xuw.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lrt.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://aph.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aml.guannengcc.top

================================================================================
来源：http://dxh.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://shx.haohaochexian.top

================================================================================
来源：http://itf.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://bet.ybcxt.top

println("Hello")
来源：http://yej.yj202588.top

[T02] Kotlin：变量
来源：http://ogu.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://guq.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://bnz.zhengqikj.top

"值: $b"
来源：http://ubz.aizwys.cn

[T04] Kotlin：空安全
来源：http://kno.316326.xyz

val n: String? = null;  n?.length
来源：http://bra.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://rqt.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dqr.sweek.top

[T06] Kotlin：集合映射
来源：http://cfm.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gsm.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://eof.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nmx.fehbvm.com

[T08] Kotlin：数据类
来源：http://cjd.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://ppq.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://xsa.birdmap.top

fun String.exclaim() = this + "!"
来源：http://giw.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://lwl.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tap.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://bwk.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jqj.fktsv.cn

[T12] Kotlin：解构声明
来源：http://tzs.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://lle.yonumen.top

[T13] Kotlin：只读 Map
来源：http://ccj.wangdashe.top

val m = mapOf("a" to 1)
来源：http://vxc.52xcode.cn

[T14] Kotlin：循环
来源：http://bue.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://qln.yongpay.top

[T15] Kotlin：接口
来源：http://ral.fengsongda.top

interface Shape { fun area(): Double }
来源：http://abp.yj20258.top

[T16] Swift：Hello World
来源：http://bho.zdqjudy.top

print("Hello")
来源：http://ums.birdmap.top

[T17] Swift：变量与常量
来源：http://riq.aibaodan.cn

var a = 1;  let b = 2
来源：http://zci.tarul.cn

[T18] Swift：字符串插值
来源：http://bfj.birdmap.top

"值: \(b)"
来源：http://vhk.yj20258888.top

[T19] Swift：可选绑定
来源：http://ozs.ybcxt.top

if let n = opt { print(n) }
来源：http://jad.gogol.net.cn

[T20] Swift：数组操作
来源：http://zkk.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://ebd.snrcjt.cn

[T21] Swift：遍历
来源：http://ila.c1oappe.top

for x in a { print(x) }
来源：http://kfx.c1oappe.top

[T22] Swift：字典
来源：http://aqt.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vrp.feifeiyinyue.top

[T23] Swift：函数
来源：http://zxo.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ygo.jiagoushi.top

[T24] Swift：闭包
来源：http://kdq.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://zum.fzhhl.top

[T25] Swift：结构体
来源：http://xvg.feifeiyinyue.top

struct P { var x: Int }
来源：http://vli.chenlongwang.top

[T26] Swift：类与重写
来源：http://pzk.yj20258888.top

class A: Base { override func f() {} }
来源：http://uis.zycfv.cn

[T27] Swift：错误处理
来源：http://jmu.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://qws.tarul.cn

[T28] Swift：枚举
来源：http://sfg.0kj1m.cn

enum Color { case red, green }
来源：http://tvl.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://lyn.shzxlz.cn

guard let x = opt else { return }
来源：http://vgl.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://dii.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://bxr.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://wut.redwolf501.top

print("Hello")
来源：http://zjh.guowangkeji.top

[T32] Lua：局部变量
来源：http://jky.yj20258.top

local a = 1
来源：http://dys.birdmap.top

[T33] Lua：表（数组）
来源：http://nbe.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sjz.yuanzhike.top

[T34] Lua：遍历表
来源：http://vac.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eod.jlsjyb.cn

[T35] Lua：字典表
来源：http://eoe.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://yxr.redwolf501.top

[T36] Lua：函数
来源：http://ncz.meibo888.top

function add(a, b) return a + b end
来源：http://dmz.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://bbm.cashguo.top

"a" .. "b"
来源：http://qkm.haohaochexian.top

[T38] Lua：条件
来源：http://vaf.birdmap.top

if x > 0 then print("正") end
来源：http://uyq.tian-w.cn

[T39] Lua：模式匹配
来源：http://zgv.yfazqb.com

string.find(s, "%d+")
来源：http://ylx.jinghuilouyu.cn

[T40] Lua：元表
来源：http://dni.hcnkem.com

setmetatable({}, { __index = base })
来源：http://lsa.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://iit.jinghuilouyu.cn

print "Hello\n";
来源：http://ofh.tarul.cn

[T42] Perl：变量类型
来源：http://fsb.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oyz.fktsv.cn

[T43] Perl：字符串插值
来源：http://fsp.hnqzz.top

"值: $a"
来源：http://njv.tianlin.xyz

[T44] Perl：条件
来源：http://lzu.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://ebr.nanxinkj.top

[T45] Perl：数组遍历
来源：http://vmq.meibo888.top

for my $x (@arr) { print $x; }
来源：http://mjk.guowangkeji.top

[T46] Perl：哈希操作
来源：http://ula.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://woo.hammf.cn

[T47] Perl：正则捕获
来源：http://dck.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nmg.chenlongwang.top

[T48] Perl：正则替换
来源：http://eud.jyoumei.cn

$s =~ s/old/new/g;
来源：http://dah.jqgfzy.top

[T49] Perl：函数
来源：http://xqu.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ldh.yonumen.top

[T50] Perl：逐行读文件
来源：http://ouh.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qqm.jinyuanbaomall.cn

while (my $line = <$fh>) { print $line; }
来源：http://bqs.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://lzw.havefunace.top

println("Hello")
来源：http://wbz.gaohongyu789.top

[T52] Scala：变量
来源：http://yml.ehwqpu.com

val a = 1;  var b = 2
来源：http://zwd.yangfankeji.com

[T53] Scala：字符串插值
来源：http://mtw.xingfuxueyuan.xyz

s"值: $b"
来源：http://flz.cdnleiting.top

[T54] Scala：集合映射
来源：http://qvo.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vwy.daxiang520.top

[T55] Scala：集合过滤
来源：http://xje.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://qab.birdmap.top

[T56] Scala：样例类
来源：http://nlo.redwolf501.top

case class User(name: String, age: Int)
来源：http://ctt.havefunace.top

[T57] Scala：模式匹配
来源：http://vud.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uxm.zhijiandao.cn

[T58] Scala：函数定义
来源：http://rgj.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://hff.ppjwa.cn

[T59] Scala：循环
来源：http://wbk.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://vtq.havefunace.top

[T60] Scala：折叠
来源：http://bmc.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xwu.epnwcf.com

================================================================================
来源：http://omn.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zfy.zhixingplan.top

================================================================================
来源：http://vog.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://gno.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://vjr.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://usr.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zgn.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://bgl.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xqp.jinqigufen.top

[U04] Py：变量调试打印
来源：http://exe.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kab.ivvv.top

[U05] Py：列表去重且保序
来源：http://phu.yvedp.cn

list(dict.fromkeys(arr))
来源：http://vte.ybcxt.top

[U06] Py：合并两个字典
来源：http://wwz.yueranfly.top

{**a, **b}
来源：http://uru.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://cow.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://xzf.yj20258888.top

[U08] Py：展平二维列表
来源：http://ttu.redwolf501.top

[y for x in nested for y in x]
来源：http://lkg.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://krq.zhoulong.xyz

max(d, key=d.get)
来源：http://ads.uphjek.com

[U10] Py：按值排序字典
来源：http://wjx.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mdc.yanxiufei.cn

[U11] Py：生成器表达式
来源：http://pcp.yonumen.top

(x * 2 for x in arr)
来源：http://faq.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kaq.tarul.cn

Counter(arr).most_common(3)
来源：http://aka.yuxming.cn

[U13] Py：固定长度队列
来源：http://ley.haohaochexian.top

deque(maxlen=10)
来源：http://xut.yonumen.top

[U14] Py：分组收集到列表
来源：http://nut.yonumen.top

defaultdict(list)
来源：http://kql.yj20258888.top

[U15] Py：高精度计时
来源：http://obf.hammf.cn

t = time.perf_counter()
来源：http://bxw.cashguo.top

[U16] Py：命令行参数解析
来源：http://uhd.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ccb.vehdjk.com

[U17] Py：初始化日志
来源：http://ige.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://oht.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://swh.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://cbs.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://chb.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yvs.fehbvm.com

[U20] Py：缓存函数结果
来源：http://dlu.cashguo.top

@functools.lru_cache(maxsize=None)
来源：http://jux.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://spa.zhoulong.xyz

@contextlib.contextmanager
来源：http://lnv.andypj.xyz

[U22] Py：矩阵转置
来源：http://tbn.epnwcf.com

list(zip(*m))
来源：http://sci.yueranfly.top

[U23] Py：分块读取大文件
来源：http://lcl.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yet.0kj1m.cn

[U24] Py：路径操作
来源：http://fsq.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mhm.yongpay.top

[U25] Py：CSV 按字典读
来源：http://dwe.yonumen.top

csv.DictReader(f)
来源：http://dbp.jiagoushi.top

[U26] Py：并发下载
来源：http://bvg.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yop.daxiang520.top

[U27] Py：异步 HTTP
来源：http://mdx.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://lgm.jianghu66.top

[U28] Py：类型别名
来源：http://xqz.aizwys.cn

UserId = int
来源：http://ghb.zhongyouzk.top

[U29] Py：属性校验
来源：http://rem.fehbvm.com

@property 与 @x.setter 配合
来源：http://idl.zhongyouzk.top

[U30] Py：数据类
来源：http://bsj.hongshengwenyu.top

@dataclass(slots=True)
来源：http://glk.xuanzx.com

[U31] Py：单测
来源：http://irs.wangshuangyany.cn

python -m pytest -q
来源：http://dbj.nanxinkj.top

[U32] Py：代码格式化
来源：http://ipr.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://vaj.hnqzz.top

[U33] Py：打包发布
来源：http://xtm.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://jfu.jinqigufen.top

[U34] Py：判断编码
来源：http://bzx.xziqi.cn

chardet.detect(raw)
来源：http://jyr.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://vce.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jed.yanxiufei.cn

[U36] Py：定时任务
来源：http://kyi.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://fgi.andypj.xyz

[U37] Py：读写 Excel
来源：http://urn.hysaishi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hqb.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://bcy.shuidangran.top

Path(__file__).resolve().parent
来源：http://efy.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://onk.andypj.xyz

sys.stdout.isatty()
来源：http://txr.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://zid.0kj1m.cn

print("err", file=sys.stderr)
来源：http://uyc.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://kfu.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fga.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://nwl.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bws.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://yrn.tianlin.xyz

namespace App\Http;
来源：http://zaj.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://nby.nanxinkj.top

declare(strict_types=1);
来源：http://szc.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://bqy.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://col.hesvh.cn

[U46] PHP：可空类型
来源：http://hev.fengsongda.top

?string $name = null
来源：http://cng.c1oappe.top

[U47] PHP：联合类型
来源：http://dac.wangshuangyany.cn

int|string $id
来源：http://lcm.shuidangran.top

[U48] PHP：纯枚举
来源：http://yye.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kvp.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://yev.yj20258.top

public readonly string $name
来源：http://mmn.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://kzy.mhx1999.top

public function __construct(private int $id) {}
来源：http://dkd.hesvh.cn

[U51] PHP：数组解构
来源：http://ymg.jlsjyb.cn

[$a, $b] = $arr;
来源：http://dov.gaohongyu789.top

[U52] PHP：箭头函数
来源：http://zqv.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://nyw.hcnkem.com

[U53] PHP：空合并运算符
来源：http://mfz.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://yey.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://jsz.hcnkem.com

$obj?->method()
来源：http://ehz.shuidangran.top

[U55] PHP：match 表达式
来源：http://cyr.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wbv.yj20258888.top

[U56] PHP：命名参数
来源：http://txx.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://nvv.ybcxt.top

[U57] PHP：字符串插值
来源：http://hag.yuanzhike.top

"值: {$a}"
来源：http://qao.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://wyt.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gqj.316326.xyz


<!-- 参考信息 -->