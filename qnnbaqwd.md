代发 wailian999

[S33] C++：vector 增删
来源：http://phy.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbt.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://tvc.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://waz.jinqigufen.top

[S35] C++：map
来源：http://gjf.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vrf.yj20258.top

[S36] C++：unordered_map
来源：http://gjo.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pdm.xuetiantiany.cn

[S37] C++：set
来源：http://huo.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eoy.ehwqpu.com

[S38] C++：排序
来源：http://nug.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://sar.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://txm.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nls.yuxming.cn

[S40] C++：查找元素
来源：http://yro.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pxi.daria6918.cn

[S41] C++：类与构造函数
来源：http://wyo.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lqy.yj202588.top

[S42] C++：继承与虚函数
来源：http://nxf.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://jlb.uphjek.com

[S43] C++：智能指针
来源：http://dvm.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://iry.cucudq.cn

[S44] C++：引用传参
来源：http://jop.birdmap.top

void inc(int &x) { ++x; }
来源：http://eze.ctjpmb.com

[S45] C++：lambda
来源：http://yfr.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://qyn.xuanzx.com

[S46] C++：函数模板
来源：http://zfi.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jig.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://ser.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jjo.sweek.top

[S48] C++：逐行读文件
来源：http://tel.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://fyl.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://ayw.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://eyk.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvb.nwbrower.top

[S50] C++：格式化数字
来源：http://rhv.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://owt.daxiang520.top

[S51] C++：显式类型转换
来源：http://wef.hysaishi.cn

static_cast<double>(a) / b
来源：http://ahe.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://tqe.nwbrower.top

int size() const noexcept { return n_; }
来源：http://jik.jqgfzy.top

[S53] C++：移动语义
来源：http://dvd.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://mcb.ybcxt.top

[S54] C++：异常处理
来源：http://idi.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gti.pycfn.com

[S55] C++：结构化绑定
来源：http://xmn.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xfw.9152youxi.cn

[S56] C++：optional
来源：http://zqa.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqb.cheryme.top

[S57] C++：编译期常量
来源：http://ocj.yanxiufei.cn

constexpr int N = 10;
来源：http://onh.vqdsnc.cn

[S58] C++：命名空间
来源：http://bcg.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://pdo.yueranfly.top

[S59] C++：静态断言
来源：http://akf.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://imq.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://zci.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ics.cqqwz.cn

================================================================================
来源：http://bjx.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bfs.jlsjyb.cn

================================================================================
来源：http://ydv.ydzc1.top

[T01] Kotlin：Hello World
来源：http://vvm.xziqi.cn

println("Hello")
来源：http://xcg.xziqi.cn

[T02] Kotlin：变量
来源：http://xkq.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dwu.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://vzp.quarkkingdee.top

"值: $b"
来源：http://hmy.shzxlz.cn

[T04] Kotlin：空安全
来源：http://zys.cheryme.top

val n: String? = null;  n?.length
来源：http://zbx.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://trk.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xid.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://oxo.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://txm.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://wss.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://edn.jqgfzy.top

[T08] Kotlin：数据类
来源：http://cvs.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://hbg.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://fhv.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://bba.sxryk.cn

[T10] Kotlin：默认参数
来源：http://buk.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xyn.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://vef.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yrl.yvedp.cn

[T12] Kotlin：解构声明
来源：http://khs.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://hok.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://kfc.sysykeji.top

val m = mapOf("a" to 1)
来源：http://kop.jqgufenzy.top

[T14] Kotlin：循环
来源：http://roy.meibo888.top

for (i in 1..10) println(i)
来源：http://shb.daria6918.cn

[T15] Kotlin：接口
来源：http://bqx.tarul.cn

interface Shape { fun area(): Double }
来源：http://ptd.ybcxt.top

[T16] Swift：Hello World
来源：http://nas.hnxiangtu.top

print("Hello")
来源：http://aki.hysaishi.cn

[T17] Swift：变量与常量
来源：http://fem.jqgfzy.top

var a = 1;  let b = 2
来源：http://alo.yongpay.top

[T18] Swift：字符串插值
来源：http://vzx.ivvv.top

"值: \(b)"
来源：http://ctw.xinyue.icu

[T19] Swift：可选绑定
来源：http://oqe.tian-w.cn

if let n = opt { print(n) }
来源：http://cfv.aibaodan.cn

[T20] Swift：数组操作
来源：http://oeu.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://uqi.hongshengwenyu.top

[T21] Swift：遍历
来源：http://jmd.shuidangran.top

for x in a { print(x) }
来源：http://oaa.xziqi.cn

[T22] Swift：字典
来源：http://pwj.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://oci.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://ssg.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ioe.sjlbkw.cn

[T24] Swift：闭包
来源：http://cim.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mdm.vqdsnc.cn

[T25] Swift：结构体
来源：http://mdk.feifeiyinyue.top

struct P { var x: Int }
来源：http://fdy.tarul.cn

[T26] Swift：类与重写
来源：http://qty.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://fsl.0kj1m.cn

[T27] Swift：错误处理
来源：http://kjd.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://fsr.uphjek.com

[T28] Swift：枚举
来源：http://mzl.zdbjq.cn

enum Color { case red, green }
来源：http://pzk.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://lhx.shangyingyoupin.top

guard let x = opt else { return }
来源：http://oes.pengpengdd.cyou

[T30] Swift：协议
来源：http://adf.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://puu.hcnkem.com

[T31] Lua：Hello World
来源：http://poe.nwbrower.top

print("Hello")
来源：http://hap.ybcxt.top

[T32] Lua：局部变量
来源：http://ilh.sweek.top

local a = 1
来源：http://orn.guannengcc.top

[T33] Lua：表（数组）
来源：http://hqx.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://fzs.9152youxi.cn

[T34] Lua：遍历表
来源：http://fuh.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fhk.316326.xyz

[T35] Lua：字典表
来源：http://sux.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://knc.jinqigfzy.top

[T36] Lua：函数
来源：http://oub.hammf.cn

function add(a, b) return a + b end
来源：http://yyd.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://yme.snrcjt.cn

"a" .. "b"
来源：http://cmc.hfpthk.cn

[T38] Lua：条件
来源：http://hwi.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://pmy.sweek.top

[T39] Lua：模式匹配
来源：http://stk.jlsjyb.cn

string.find(s, "%d+")
来源：http://dvf.yongpay.top

[T40] Lua：元表
来源：http://nue.xuanzx.com

setmetatable({}, { __index = base })
来源：http://ugq.yuanzhike.top

[T41] Perl：Hello World
来源：http://lbw.hnqzz.top

print "Hello\n";
来源：http://aoo.yvedp.cn

[T42] Perl：变量类型
来源：http://lqp.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zvk.fzhhl.top

[T43] Perl：字符串插值
来源：http://rak.jyoumei.cn

"值: $a"
来源：http://mba.tarul.cn

[T44] Perl：条件
来源：http://nbi.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://kyu.cheryme.top

[T45] Perl：数组遍历
来源：http://xlg.yj202588.top

for my $x (@arr) { print $x; }
来源：http://sfn.hfpthk.cn

[T46] Perl：哈希操作
来源：http://wtt.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eyf.tarul.cn

[T47] Perl：正则捕获
来源：http://yml.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://keu.uphjek.com

[T48] Perl：正则替换
来源：http://fuh.tian-w.cn

$s =~ s/old/new/g;
来源：http://vwg.52xcode.cn

[T49] Perl：函数
来源：http://ehz.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gbr.bjfxy.top

[T50] Perl：逐行读文件
来源：http://xiy.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ipf.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://orp.bbcook.cn

[T51] Scala：Hello World
来源：http://twu.shangyingyoupin.top

println("Hello")
来源：http://hqx.fehbvm.com

[T52] Scala：变量
来源：http://yxb.ybcxt.top

val a = 1;  var b = 2
来源：http://jfm.hesvh.cn

[T53] Scala：字符串插值
来源：http://uro.shanyushiyangtech.top

s"值: $b"
来源：http://wfr.jyoumei.cn

[T54] Scala：集合映射
来源：http://owo.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://abw.wangdashe.top

[T55] Scala：集合过滤
来源：http://equ.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://ovy.guannengcc.top

[T56] Scala：样例类
来源：http://bmo.sufxvd.cn

case class User(name: String, age: Int)
来源：http://iyp.bjfxy.top

[T57] Scala：模式匹配
来源：http://gkl.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://bdm.sysykeji.top

[T58] Scala：函数定义
来源：http://qer.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://szr.hongshengwenyu.top

[T59] Scala：循环
来源：http://dir.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://jst.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://aub.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jnd.xuanzx.com

================================================================================
来源：http://efg.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hfc.zycfv.cn

================================================================================
来源：http://zqy.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://uzf.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://rwr.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://kyj.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uvl.andypj.xyz

[U03] Py：加载 .env 配置
来源：http://dvj.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://drj.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://hjg.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blx.ybcxt.top

[U05] Py：列表去重且保序
来源：http://tlt.xuanzx.com

list(dict.fromkeys(arr))
来源：http://lbz.sxryk.cn

[U06] Py：合并两个字典
来源：http://hef.cucudq.cn

{**a, **b}
来源：http://gep.yj20258888.top

[U07] Py：反转字典键值
来源：http://dyc.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://yna.0kj1m.cn

[U08] Py：展平二维列表
来源：http://chn.fktsv.cn

[y for x in nested for y in x]
来源：http://rdu.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://abk.bjfxy.top

max(d, key=d.get)
来源：http://xep.sweek.top

[U10] Py：按值排序字典
来源：http://urt.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://asj.snrcjt.cn

[U11] Py：生成器表达式
来源：http://nbs.jinqigfzy.top

(x * 2 for x in arr)
来源：http://xqf.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bnz.xziqi.cn

Counter(arr).most_common(3)
来源：http://nzx.jinqigufen.top

[U13] Py：固定长度队列
来源：http://nvm.jiagoushi.top

deque(maxlen=10)
来源：http://xsk.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://tij.zycfv.cn

defaultdict(list)
来源：http://gld.zhengqikj.top

[U15] Py：高精度计时
来源：http://izo.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://vkl.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://zav.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vty.epnwcf.com

[U17] Py：初始化日志
来源：http://dcs.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://xrr.daria6918.cn

[U18] Py：预编译正则
来源：http://iwj.cheryme.top

pat = re.compile(r"\d+")
来源：http://yma.redwolf501.top

[U19] Py：正则替换带回调
来源：http://uqg.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nch.gzhubu.top

[U20] Py：缓存函数结果
来源：http://kre.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://jej.shangyingyoupin.top

[U21] Py：自定义上下文管理器
来源：http://twa.52xcode.cn

@contextlib.contextmanager
来源：http://yev.uphjek.com

[U22] Py：矩阵转置
来源：http://ppc.quarkkingdee.top

list(zip(*m))
来源：http://nki.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://btp.aizwys.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bey.hfpthk.cn

[U24] Py：路径操作
来源：http://nds.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epf.pycfn.com

[U25] Py：CSV 按字典读
来源：http://kij.mhx1999.top

csv.DictReader(f)
来源：http://zrj.zdqjudy.top

[U26] Py：并发下载
来源：http://yqx.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bxe.tianlin.xyz

[U27] Py：异步 HTTP
来源：http://aej.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://xky.shuidangran.top

[U28] Py：类型别名
来源：http://dtk.wangshuangyany.cn

UserId = int
来源：http://cql.zycfv.cn

[U29] Py：属性校验
来源：http://eab.fzhhl.top

@property 与 @x.setter 配合
来源：http://rkt.dianchejie.cn

[U30] Py：数据类
来源：http://usu.wangdashe.top

@dataclass(slots=True)
来源：http://vdg.jlsjyb.cn

[U31] Py：单测
来源：http://moi.svipenyu.cn

python -m pytest -q
来源：http://iei.quarkkingdee.top

[U32] Py：代码格式化
来源：http://ihc.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://oix.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://ynv.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://luu.yj20258888.top

[U34] Py：判断编码
来源：http://acw.sysykeji.top

chardet.detect(raw)
来源：http://tak.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://sfm.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dng.hysaishi.cn

[U36] Py：定时任务
来源：http://anf.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://yyl.gotoacloud.top

[U37] Py：读写 Excel
来源：http://gvk.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://lnc.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://ije.ydzc1.top

Path(__file__).resolve().parent
来源：http://baq.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://rml.ydjk.org.cn

sys.stdout.isatty()
来源：http://dpq.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://rbw.xylfe.cn

print("err", file=sys.stderr)
来源：http://zwp.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://sju.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jun.sjlbkw.cn

[U42] PHP：PSR-4 自动加载
来源：http://exv.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mrz.bbcook.cn

[U43] PHP：声明命名空间
来源：http://hed.shanyushiyangtech.top

namespace App\Http;
来源：http://bwa.shuidangran.top

[U44] PHP：开启严格类型
来源：http://mao.9152youxi.cn

declare(strict_types=1);
来源：http://dcr.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://dqb.gotoacloud.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cxt.ctjpmb.com

[U46] PHP：可空类型
来源：http://dms.ppjwa.cn

?string $name = null
来源：http://wjo.gogol.net.cn

[U47] PHP：联合类型
来源：http://vpa.ywan-chungtsiang.top

int|string $id
来源：http://pwg.uphjek.com

[U48] PHP：纯枚举
来源：http://rua.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gdq.birdmap.top

[U49] PHP：只读属性
来源：http://xtc.birdmap.top

public readonly string $name
来源：http://yfa.sweek.top

[U50] PHP：构造器属性提升
来源：http://efu.gotoacloud.top

public function __construct(private int $id) {}
来源：http://wwj.hnqzz.top

[U51] PHP：数组解构
来源：http://arq.jiagoushi.top

[$a, $b] = $arr;
来源：http://xin.tarul.cn

[U52] PHP：箭头函数
来源：http://bbi.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://gzm.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://mgn.snrcjt.cn

$v = $a ?? $b ?? "default";
来源：http://uqq.guannengcc.top

[U54] PHP：空安全调用
来源：http://aco.shanyushiyangtech.top

$obj?->method()
来源：http://uye.zhengqikj.top

[U55] PHP：match 表达式
来源：http://ojl.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rzx.kuanghao11.cn

[U56] PHP：命名参数
来源：http://ivx.vqdsnc.cn

f(a: 1, b: 2)
来源：http://vvo.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://tvl.hcnkem.com

"值: {$a}"
来源：http://fcf.jinqigufen.top

[U58] PHP：数组三件套
来源：http://pmg.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aqx.guannengcc.top


<!-- 参考信息 -->