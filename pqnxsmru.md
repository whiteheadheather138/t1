代发 wailian999

[S33] C++：vector 增删
来源：http://bii.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qrp.gotoacloud.top

[S34] C++：遍历 vector
来源：http://hfq.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://wxc.shuidangran.top

[S35] C++：map
来源：http://klr.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bfv.hesvh.cn

[S36] C++：unordered_map
来源：http://vsf.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jpq.quarkkingdee.top

[S37] C++：set
来源：http://skh.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vnw.cucudq.cn

[S38] C++：排序
来源：http://lmq.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://ykv.yj20258.top

[S39] C++：自定义比较器排序
来源：http://vei.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jcw.jiagoushi.top

[S40] C++：查找元素
来源：http://icc.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nlp.cheryme.top

[S41] C++：类与构造函数
来源：http://gey.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://axd.andypj.xyz

[S42] C++：继承与虚函数
来源：http://fik.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://bqi.hammf.cn

[S43] C++：智能指针
来源：http://qvy.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://emu.bbcook.cn

[S44] C++：引用传参
来源：http://eqm.yueranfly.top

void inc(int &x) { ++x; }
来源：http://iht.jqgfzy.top

[S45] C++：lambda
来源：http://vbn.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://odt.52xcode.cn

[S46] C++：函数模板
来源：http://xwu.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jlj.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://osp.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nff.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://eei.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oxw.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://wvl.yanxiufei.cn

[S49] C++：写文件
来源：http://dyv.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eya.chenzaomai.com

[S50] C++：格式化数字
来源：http://tmp.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tus.ydzc1.top

[S51] C++：显式类型转换
来源：http://vvl.c1oappe.top

static_cast<double>(a) / b
来源：http://eds.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://qqo.vehdjk.com

int size() const noexcept { return n_; }
来源：http://iwg.shuidangran.top

[S53] C++：移动语义
来源：http://yrk.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://xma.yueranfly.top

[S54] C++：异常处理
来源：http://gwz.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jid.gotoacloud.top

[S55] C++：结构化绑定
来源：http://ywg.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zuj.snrcjt.cn

[S56] C++：optional
来源：http://jrp.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://scs.yuxming.cn

[S57] C++：编译期常量
来源：http://qhk.aizwys.cn

constexpr int N = 10;
来源：http://yyz.yj20258.top

[S58] C++：命名空间
来源：http://ygu.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://gtd.xinyue.icu

[S59] C++：静态断言
来源：http://xlq.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tjx.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://lye.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://epl.tarul.cn

================================================================================
来源：http://fpn.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nzk.tarul.cn

================================================================================
来源：http://vtu.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://qkm.fehbvm.com

println("Hello")
来源：http://ctz.yj20258888.top

[T02] Kotlin：变量
来源：http://mwo.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obm.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://klh.guowangkeji.top

"值: $b"
来源：http://wme.andypj.xyz

[T04] Kotlin：空安全
来源：http://khs.9152youxi.cn

val n: String? = null;  n?.length
来源：http://fqy.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://uqt.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xbi.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://tug.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ekr.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://tee.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tyw.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://gjw.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://rqc.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://kfl.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://cvu.iojbl.cn

[T10] Kotlin：默认参数
来源：http://xai.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qlj.yueranfly.top

[T11] Kotlin：协程
来源：http://rgf.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xft.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://tdj.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://fup.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://sem.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://tdi.zhengqikj.top

[T14] Kotlin：循环
来源：http://owr.fengsongda.top

for (i in 1..10) println(i)
来源：http://gzc.yfazqb.com

[T15] Kotlin：接口
来源：http://zbe.shuidangran.top

interface Shape { fun area(): Double }
来源：http://cam.sweek.top

[T16] Swift：Hello World
来源：http://cdj.cqqwz.cn

print("Hello")
来源：http://eqy.yongpay.top

[T17] Swift：变量与常量
来源：http://lpb.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://dje.hcnkem.com

[T18] Swift：字符串插值
来源：http://wxa.shzxlz.cn

"值: \(b)"
来源：http://mml.vehdjk.com

[T19] Swift：可选绑定
来源：http://vov.zhoulong.xyz

if let n = opt { print(n) }
来源：http://smd.nwbrower.top

[T20] Swift：数组操作
来源：http://tvd.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mze.jqgfzy.top

[T21] Swift：遍历
来源：http://xnn.iojbl.cn

for x in a { print(x) }
来源：http://afo.9152youxi.cn

[T22] Swift：字典
来源：http://kkc.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://law.zhoulong.xyz

[T23] Swift：函数
来源：http://csu.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dpv.hesvh.cn

[T24] Swift：闭包
来源：http://fgu.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dcb.fehbvm.com

[T25] Swift：结构体
来源：http://esw.hnqzz.top

struct P { var x: Int }
来源：http://izr.52xcode.cn

[T26] Swift：类与重写
来源：http://inx.xuanzx.com

class A: Base { override func f() {} }
来源：http://irj.jinqigfzy.top

[T27] Swift：错误处理
来源：http://jog.yuxming.cn

do { try f() } catch { print(error) }
来源：http://eyc.snrcjt.cn

[T28] Swift：枚举
来源：http://nll.yvedp.cn

enum Color { case red, green }
来源：http://dps.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://vfu.xuanzx.com

guard let x = opt else { return }
来源：http://uhq.yvedp.cn

[T30] Swift：协议
来源：http://cvp.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://rdf.yuanzhike.top

[T31] Lua：Hello World
来源：http://wqv.svipenyu.cn

print("Hello")
来源：http://tlw.ivvv.top

[T32] Lua：局部变量
来源：http://aps.daxiang520.top

local a = 1
来源：http://map.chenlongwang.top

[T33] Lua：表（数组）
来源：http://rhr.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ztc.yj20258888.top

[T34] Lua：遍历表
来源：http://wtp.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gjb.hcnkem.com

[T35] Lua：字典表
来源：http://snf.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://nsr.bbcook.cn

[T36] Lua：函数
来源：http://cnb.yuxming.cn

function add(a, b) return a + b end
来源：http://vuv.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://zic.sufxvd.cn

"a" .. "b"
来源：http://fqw.hywenlv.cn

[T38] Lua：条件
来源：http://wbh.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://arb.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://bgm.tian-w.cn

string.find(s, "%d+")
来源：http://zmb.haohaochexian.top

[T40] Lua：元表
来源：http://nyr.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://ntu.9152youxi.cn

[T41] Perl：Hello World
来源：http://upe.tanke756.top

print "Hello\n";
来源：http://fkg.yongpay.top

[T42] Perl：变量类型
来源：http://nfj.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hbl.uphjek.com

[T43] Perl：字符串插值
来源：http://lzg.tianlin.xyz

"值: $a"
来源：http://woo.yanxiufei.cn

[T44] Perl：条件
来源：http://cuu.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://obt.tian-w.cn

[T45] Perl：数组遍历
来源：http://fnw.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://mwk.yuanzhike.top

[T46] Perl：哈希操作
来源：http://gxh.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jfm.hfpthk.cn

[T47] Perl：正则捕获
来源：http://edh.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fgy.yj20258.top

[T48] Perl：正则替换
来源：http://tsc.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://ont.sysykeji.top

[T49] Perl：函数
来源：http://hwl.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hfq.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://fob.ywan-chungtsiang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bhu.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://ofg.zycfv.cn

[T51] Scala：Hello World
来源：http://huy.dianchejie.cn

println("Hello")
来源：http://mph.dianchejie.cn

[T52] Scala：变量
来源：http://zxm.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://fsu.gotoacloud.top

[T53] Scala：字符串插值
来源：http://zea.xingfuxueyuan.xyz

s"值: $b"
来源：http://jlw.zdbjq.cn

[T54] Scala：集合映射
来源：http://eel.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://jin.ivvv.top

[T55] Scala：集合过滤
来源：http://got.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bnq.tianlin.xyz

[T56] Scala：样例类
来源：http://iik.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://nui.chenzaomai.com

[T57] Scala：模式匹配
来源：http://yqd.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ouu.9152youxi.cn

[T58] Scala：函数定义
来源：http://mpl.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://idg.xuanzx.com

[T59] Scala：循环
来源：http://ria.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://rvi.bbcook.cn

[T60] Scala：折叠
来源：http://bnd.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ozs.yanxiufei.cn

================================================================================
来源：http://gmy.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cma.yj20258888.top

================================================================================
来源：http://nxf.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://aky.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://apr.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://htq.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mid.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://iot.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://igz.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://cfp.ydzc1.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://egg.fzhhl.top

[U05] Py：列表去重且保序
来源：http://mad.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://mli.yvedp.cn

[U06] Py：合并两个字典
来源：http://txc.yanxiufei.cn

{**a, **b}
来源：http://gra.dashuyun.cn

[U07] Py：反转字典键值
来源：http://wzm.redwolf501.top

{v: k for k, v in d.items()}
来源：http://mlq.zdbjq.cn

[U08] Py：展平二维列表
来源：http://une.gogol.net.cn

[y for x in nested for y in x]
来源：http://mad.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://cms.svipenyu.cn

max(d, key=d.get)
来源：http://tzm.hywenlv.cn

[U10] Py：按值排序字典
来源：http://rrs.ctjpmb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qmz.yangfankeji.com

[U11] Py：生成器表达式
来源：http://ews.fehbvm.com

(x * 2 for x in arr)
来源：http://jnu.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://wlq.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://ahx.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://yar.hfpthk.cn

deque(maxlen=10)
来源：http://jzf.yuxming.cn

[U14] Py：分组收集到列表
来源：http://omz.chenlongwang.top

defaultdict(list)
来源：http://zum.gaohongyu789.top

[U15] Py：高精度计时
来源：http://gwv.smart0.xyz

t = time.perf_counter()
来源：http://fhq.hesvh.cn

[U16] Py：命令行参数解析
来源：http://jya.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bcg.tianlin.xyz

[U17] Py：初始化日志
来源：http://kfe.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://mia.svipenyu.cn

[U18] Py：预编译正则
来源：http://kob.andypj.xyz

pat = re.compile(r"\d+")
来源：http://bul.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://uvu.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zlj.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://ctx.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://yai.jqgufenzy.top

[U21] Py：自定义上下文管理器
来源：http://shf.svipenyu.cn

@contextlib.contextmanager
来源：http://zwp.cashguo.top

[U22] Py：矩阵转置
来源：http://smp.dashuyun.cn

list(zip(*m))
来源：http://eyf.aizwys.cn

[U23] Py：分块读取大文件
来源：http://vsp.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ueh.fengsongda.top

[U24] Py：路径操作
来源：http://kun.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://slj.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://abf.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://bqi.tanke756.top

[U26] Py：并发下载
来源：http://kzz.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qso.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://not.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://lbp.tian-w.cn

[U28] Py：类型别名
来源：http://sgq.guannengcc.top

UserId = int
来源：http://syv.hammf.cn

[U29] Py：属性校验
来源：http://pit.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://kfq.xziqi.cn

[U30] Py：数据类
来源：http://oyf.redwolf501.top

@dataclass(slots=True)
来源：http://sbx.cdnleiting.top

[U31] Py：单测
来源：http://fsg.svipenyu.cn

python -m pytest -q
来源：http://tgf.smart0.xyz

[U32] Py：代码格式化
来源：http://vun.wangshuangyany.cn

ruff format . && ruff check --fix .
来源：http://gju.dashuyun.cn

[U33] Py：打包发布
来源：http://lrf.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://xxe.yfazqb.com

[U34] Py：判断编码
来源：http://zrg.aibaodan.cn

chardet.detect(raw)
来源：http://rrc.aibaodan.cn

[U35] Py：发送邮件
来源：http://llj.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qrr.fktsv.cn

[U36] Py：定时任务
来源：http://uif.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://tde.havefunace.top

[U37] Py：读写 Excel
来源：http://liy.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lbe.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://uxj.redwolf501.top

Path(__file__).resolve().parent
来源：http://gmh.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://uys.tarul.cn

sys.stdout.isatty()
来源：http://vjl.wangdashe.top

[U40] Py：打印到标准错误
来源：http://ozn.ivvv.top

print("err", file=sys.stderr)
来源：http://nrv.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://sif.xinyue.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://jgm.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://qmf.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qno.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://mlf.zdbjq.cn

namespace App\Http;
来源：http://huj.ydzc1.top

[U44] PHP：开启严格类型
来源：http://lrx.yj202588.top

declare(strict_types=1);
来源：http://pyq.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://dhw.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://joq.daxiang520.top

[U46] PHP：可空类型
来源：http://dyw.gzhubu.top

?string $name = null
来源：http://euc.fehbvm.com

[U47] PHP：联合类型
来源：http://upk.nanxuanxn.top

int|string $id
来源：http://jbj.yfazqb.com

[U48] PHP：纯枚举
来源：http://hny.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zes.yj202588.top

[U49] PHP：只读属性
来源：http://inm.zhengqikj.top

public readonly string $name
来源：http://ftu.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://hfm.jiagoushi.top

public function __construct(private int $id) {}
来源：http://tpc.yueranfly.top

[U51] PHP：数组解构
来源：http://qdh.jianghu66.top

[$a, $b] = $arr;
来源：http://thj.ivvv.top

[U52] PHP：箭头函数
来源：http://xew.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://xuq.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://mxx.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://mtr.sysykeji.top

[U54] PHP：空安全调用
来源：http://ypq.chenjidiqi.icu

$obj?->method()
来源：http://yeb.cdnleiting.top

[U55] PHP：match 表达式
来源：http://nel.fengsongda.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vzy.tianlin.xyz

[U56] PHP：命名参数
来源：http://ypj.nanxinkj.top

f(a: 1, b: 2)
来源：http://gys.ivvv.top

[U57] PHP：字符串插值
来源：http://fou.xinyue.icu

"值: {$a}"
来源：http://gce.jianghu66.top

[U58] PHP：数组三件套
来源：http://zvs.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pvl.jinyuanbaomall.cn


<!-- 参考信息 -->