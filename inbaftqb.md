代发 wailian999

[S33] C++：vector 增删
来源：http://xgz.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cep.nanxinkj.top

[S34] C++：遍历 vector
来源：http://osr.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://prf.xylfe.cn

[S35] C++：map
来源：http://ell.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pmf.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://oza.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vyj.tian-w.cn

[S37] C++：set
来源：http://gyx.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://foq.cdnleiting.top

[S38] C++：排序
来源：http://wak.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://ntg.havefunace.top

[S39] C++：自定义比较器排序
来源：http://neb.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uki.52xcode.cn

[S40] C++：查找元素
来源：http://zpc.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gtj.fengsongda.top

[S41] C++：类与构造函数
来源：http://pgy.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlw.xuanzx.com

[S42] C++：继承与虚函数
来源：http://uyd.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://yyv.gaohongyu789.top

[S43] C++：智能指针
来源：http://gqt.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://iyx.ybcxt.top

[S44] C++：引用传参
来源：http://pet.yfazqb.com

void inc(int &x) { ++x; }
来源：http://dcc.ehwqpu.com

[S45] C++：lambda
来源：http://yzz.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jlj.jinqigufen.top

[S46] C++：函数模板
来源：http://hcg.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qmc.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://ilh.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aei.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://rlp.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://rfr.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://uuy.hcnkem.com

[S49] C++：写文件
来源：http://emv.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fim.ctjpmb.com

[S50] C++：格式化数字
来源：http://psk.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vbt.yuanzhike.top

[S51] C++：显式类型转换
来源：http://jej.smart0.xyz

static_cast<double>(a) / b
来源：http://osv.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://dub.daxiang520.top

int size() const noexcept { return n_; }
来源：http://xmx.52xcode.cn

[S53] C++：移动语义
来源：http://dri.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://jca.hesvh.cn

[S54] C++：异常处理
来源：http://bwy.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yfo.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://bpo.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hpn.jianghu66.top

[S56] C++：optional
来源：http://llq.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://poy.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://tss.haohaochexian.top

constexpr int N = 10;
来源：http://hnx.ydzc1.top

[S58] C++：命名空间
来源：http://udu.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://jrl.andypj.xyz

[S59] C++：静态断言
来源：http://nrv.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gzy.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://tyo.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dwm.yueranfly.top

================================================================================
来源：http://pqk.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqn.sxryk.cn

================================================================================
来源：http://apz.yj20258.top

[T01] Kotlin：Hello World
来源：http://lno.aibaodan.cn

println("Hello")
来源：http://wia.wangdashe.top

[T02] Kotlin：变量
来源：http://edm.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qwr.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://wqk.birdmap.top

"值: $b"
来源：http://llh.yonumen.top

[T04] Kotlin：空安全
来源：http://urk.cqqwz.cn

val n: String? = null;  n?.length
来源：http://rgu.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://lka.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gyd.cashguo.top

[T06] Kotlin：集合映射
来源：http://orv.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uci.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://nxz.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://sld.52xcode.cn

[T08] Kotlin：数据类
来源：http://jeo.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://asj.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://wfb.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://bgy.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://wkj.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nbb.quarkkingdee.top

[T11] Kotlin：协程
来源：http://ohf.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://enx.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://mmy.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://gzq.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://hjj.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://hxy.vqdsnc.cn

[T14] Kotlin：循环
来源：http://adz.tanke756.top

for (i in 1..10) println(i)
来源：http://hnd.meibo888.top

[T15] Kotlin：接口
来源：http://emj.meibo888.top

interface Shape { fun area(): Double }
来源：http://yva.gaohongyu789.top

[T16] Swift：Hello World
来源：http://pxg.bbcook.cn

print("Hello")
来源：http://agv.bjfxy.top

[T17] Swift：变量与常量
来源：http://wlo.sysykeji.top

var a = 1;  let b = 2
来源：http://fer.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://kvk.shangyingyoupin.top

"值: \(b)"
来源：http://jwg.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://ccz.sweek.top

if let n = opt { print(n) }
来源：http://hax.smart0.xyz

[T20] Swift：数组操作
来源：http://rso.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nxe.zhiwuduotai.top

[T21] Swift：遍历
来源：http://cmv.shuidangran.top

for x in a { print(x) }
来源：http://arz.cdnleiting.top

[T22] Swift：字典
来源：http://qai.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kfm.tianlin.xyz

[T23] Swift：函数
来源：http://emd.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tvj.gaohongyu789.top

[T24] Swift：闭包
来源：http://wqr.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://icq.hywenlv.cn

[T25] Swift：结构体
来源：http://aga.bjfxy.top

struct P { var x: Int }
来源：http://rso.guowangkeji.top

[T26] Swift：类与重写
来源：http://ucy.sxryk.cn

class A: Base { override func f() {} }
来源：http://tye.birdmap.top

[T27] Swift：错误处理
来源：http://kuu.yj20258888.top

do { try f() } catch { print(error) }
来源：http://wqn.0kj1m.cn

[T28] Swift：枚举
来源：http://xcl.andypj.xyz

enum Color { case red, green }
来源：http://icn.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://ooc.tian-w.cn

guard let x = opt else { return }
来源：http://xcg.hammf.cn

[T30] Swift：协议
来源：http://lkr.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://mel.ivvv.top

[T31] Lua：Hello World
来源：http://mzg.zhoulong.xyz

print("Hello")
来源：http://evn.iojbl.cn

[T32] Lua：局部变量
来源：http://ths.yonumen.top

local a = 1
来源：http://wyu.cucudq.cn

[T33] Lua：表（数组）
来源：http://aaj.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://rpz.chenzaomai.com

[T34] Lua：遍历表
来源：http://fmd.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eof.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://yxn.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://aoh.zhengqikj.top

[T36] Lua：函数
来源：http://nmk.smart0.xyz

function add(a, b) return a + b end
来源：http://fqn.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://ifx.tarul.cn

"a" .. "b"
来源：http://vtq.ivvv.top

[T38] Lua：条件
来源：http://igg.gogol.net.cn

if x > 0 then print("正") end
来源：http://jhv.hysaishi.cn

[T39] Lua：模式匹配
来源：http://hkc.havefunace.top

string.find(s, "%d+")
来源：http://qpe.yueranfly.top

[T40] Lua：元表
来源：http://lfd.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://kvj.zhixingplan.top

[T41] Perl：Hello World
来源：http://ooi.andypj.xyz

print "Hello\n";
来源：http://wxw.dianchejie.cn

[T42] Perl：变量类型
来源：http://eoa.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hca.jiagoushi.top

[T43] Perl：字符串插值
来源：http://oyt.ywan-chungtsiang.top

"值: $a"
来源：http://zby.chenjidiqi.icu

[T44] Perl：条件
来源：http://esi.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://wyb.daria6918.cn

[T45] Perl：数组遍历
来源：http://vdc.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://ypy.cucudq.cn

[T46] Perl：哈希操作
来源：http://xck.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rvs.yj20258888.top

[T47] Perl：正则捕获
来源：http://oah.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vmd.andypj.xyz

[T48] Perl：正则替换
来源：http://qeu.aizwys.cn

$s =~ s/old/new/g;
来源：http://pro.sysykeji.top

[T49] Perl：函数
来源：http://zvf.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bcc.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://blm.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rsr.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://mje.uphjek.com

[T51] Scala：Hello World
来源：http://aby.316326.xyz

println("Hello")
来源：http://bch.wangshuangyany.cn

[T52] Scala：变量
来源：http://vpw.chenzaomai.com

val a = 1;  var b = 2
来源：http://rma.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://juf.wangdashe.top

s"值: $b"
来源：http://fwn.ctjpmb.com

[T54] Scala：集合映射
来源：http://ehz.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://sit.0kj1m.cn

[T55] Scala：集合过滤
来源：http://ory.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://ufo.tanke756.top

[T56] Scala：样例类
来源：http://ybx.ivvv.top

case class User(name: String, age: Int)
来源：http://nqk.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://bhe.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gaf.daxiang520.top

[T58] Scala：函数定义
来源：http://def.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gqq.tian-w.cn

[T59] Scala：循环
来源：http://qps.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://pls.nanxinkj.top

[T60] Scala：折叠
来源：http://iug.cdnleiting.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xzt.sysykeji.top

================================================================================
来源：http://pre.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kki.uphjek.com

================================================================================
来源：http://lpo.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://qsi.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mrt.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://vih.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ica.hesvh.cn

[U03] Py：加载 .env 配置
来源：http://qla.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://fqj.cqqwz.cn

[U04] Py：变量调试打印
来源：http://ghg.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rbv.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://lbw.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://fcy.birdmap.top

[U06] Py：合并两个字典
来源：http://fbg.zhixingplan.top

{**a, **b}
来源：http://zbj.zhengqikj.top

[U07] Py：反转字典键值
来源：http://elx.iojbl.cn

{v: k for k, v in d.items()}
来源：http://feq.yongpay.top

[U08] Py：展平二维列表
来源：http://pom.ctjpmb.com

[y for x in nested for y in x]
来源：http://ppt.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://myl.andypj.xyz

max(d, key=d.get)
来源：http://hau.ydzc1.top

[U10] Py：按值排序字典
来源：http://ypc.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ydm.yj202588.top

[U11] Py：生成器表达式
来源：http://dxc.fktsv.cn

(x * 2 for x in arr)
来源：http://lip.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qbv.xziqi.cn

Counter(arr).most_common(3)
来源：http://phe.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://boq.aibaodan.cn

deque(maxlen=10)
来源：http://klv.bbcook.cn

[U14] Py：分组收集到列表
来源：http://hnr.52xcode.cn

defaultdict(list)
来源：http://ink.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://prz.jinqigufen.top

t = time.perf_counter()
来源：http://yep.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://iru.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://unb.yueranfly.top

[U17] Py：初始化日志
来源：http://moe.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://yet.sysykeji.top

[U18] Py：预编译正则
来源：http://pxk.cheryme.top

pat = re.compile(r"\d+")
来源：http://bku.sysykeji.top

[U19] Py：正则替换带回调
来源：http://qja.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zjn.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://dch.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://had.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://zyy.sufxvd.cn

@contextlib.contextmanager
来源：http://lrp.hysaishi.cn

[U22] Py：矩阵转置
来源：http://zrw.shangyingyoupin.top

list(zip(*m))
来源：http://wwk.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://peu.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tai.xinyue.icu

[U24] Py：路径操作
来源：http://jtl.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rea.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://cub.zdbjq.cn

csv.DictReader(f)
来源：http://jwg.pycfn.com

[U26] Py：并发下载
来源：http://ngz.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lkm.hnqzz.top

[U27] Py：异步 HTTP
来源：http://edo.ydjk.org.cn

aiohttp.ClientSession() 配合 async with
来源：http://wah.c1oappe.top

[U28] Py：类型别名
来源：http://cyh.yuxming.cn

UserId = int
来源：http://dyg.fktsv.cn

[U29] Py：属性校验
来源：http://tro.gogol.net.cn

@property 与 @x.setter 配合
来源：http://tyi.hammf.cn

[U30] Py：数据类
来源：http://yir.shzxlz.cn

@dataclass(slots=True)
来源：http://lib.nwbrower.top

[U31] Py：单测
来源：http://ppj.yuanzhike.top

python -m pytest -q
来源：http://ihf.svipenyu.cn

[U32] Py：代码格式化
来源：http://fhs.yuxming.cn

ruff format . && ruff check --fix .
来源：http://eaj.haohaochexian.top

[U33] Py：打包发布
来源：http://phe.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://vdg.jqgfzy.top

[U34] Py：判断编码
来源：http://lnq.ydjk.org.cn

chardet.detect(raw)
来源：http://xyq.gzhubu.top

[U35] Py：发送邮件
来源：http://ehz.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bnq.hesvh.cn

[U36] Py：定时任务
来源：http://mug.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://gss.redwolf501.top

[U37] Py：读写 Excel
来源：http://mka.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://qpe.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://biy.jianghu66.top

Path(__file__).resolve().parent
来源：http://iyw.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://otd.yongpay.top

sys.stdout.isatty()
来源：http://ghs.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://wwh.yangfankeji.com

print("err", file=sys.stderr)
来源：http://dcf.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://jsk.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://emk.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://tvr.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hbz.sysykeji.top

[U43] PHP：声明命名空间
来源：http://xcn.yonumen.top

namespace App\Http;
来源：http://jiw.tanke756.top

[U44] PHP：开启严格类型
来源：http://aql.xylfe.cn

declare(strict_types=1);
来源：http://aos.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://byj.tian-w.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://urg.yuxming.cn

[U46] PHP：可空类型
来源：http://ilz.jlsjyb.cn

?string $name = null
来源：http://qdm.meibo888.top

[U47] PHP：联合类型
来源：http://ivq.sxryk.cn

int|string $id
来源：http://wdb.tianlin.xyz

[U48] PHP：纯枚举
来源：http://nsp.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://edm.ydjk.org.cn

[U49] PHP：只读属性
来源：http://wdw.redwolf501.top

public readonly string $name
来源：http://oli.cashguo.top

[U50] PHP：构造器属性提升
来源：http://nnd.ctjpmb.com

public function __construct(private int $id) {}
来源：http://qbv.zhoulong.xyz

[U51] PHP：数组解构
来源：http://ijb.guowangkeji.top

[$a, $b] = $arr;
来源：http://xmf.tianlin.xyz

[U52] PHP：箭头函数
来源：http://apv.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://joq.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://zfd.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://tfe.hesvh.cn

[U54] PHP：空安全调用
来源：http://gtf.zhiwuduotai.top

$obj?->method()
来源：http://uif.jinqigufen.top

[U55] PHP：match 表达式
来源：http://lvz.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jvk.uphjek.com

[U56] PHP：命名参数
来源：http://fpd.hywenlv.cn

f(a: 1, b: 2)
来源：http://gxa.fehbvm.com

[U57] PHP：字符串插值
来源：http://swb.jianghu66.top

"值: {$a}"
来源：http://cpq.meibo888.top

[U58] PHP：数组三件套
来源：http://uyr.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://caf.cdnleiting.top


<!-- 参考信息 -->