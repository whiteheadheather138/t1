代发 wailian999

[S37] C++：set
来源：http://bvm.chenlongwang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hyg.xylfe.cn

[S38] C++：排序
来源：http://tse.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://why.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://rnw.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ihl.aibaodan.cn

[S40] C++：查找元素
来源：http://zoo.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmm.cashguo.top

[S41] C++：类与构造函数
来源：http://tsf.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wal.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://tqj.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://qer.xuetiantiany.cn

[S43] C++：智能指针
来源：http://uwo.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://pjb.yanxiufei.cn

[S44] C++：引用传参
来源：http://yay.wangdashe.top

void inc(int &x) { ++x; }
来源：http://jmn.vehdjk.com

[S45] C++：lambda
来源：http://lxg.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tlv.yongpay.top

[S46] C++：函数模板
来源：http://ylt.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dza.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://wve.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lmc.tarul.cn

[S48] C++：逐行读文件
来源：http://kve.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://frq.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://shu.jinghuilouyu.cn

[S49] C++：写文件
来源：http://gsr.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://any.xziqi.cn

[S50] C++：格式化数字
来源：http://twa.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qcl.hammf.cn

[S51] C++：显式类型转换
来源：http://jrh.zycfv.cn

static_cast<double>(a) / b
来源：http://rcd.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://hkl.xziqi.cn

int size() const noexcept { return n_; }
来源：http://jdk.yvedp.cn

[S53] C++：移动语义
来源：http://puf.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://kdx.chenzaomai.com

[S54] C++：异常处理
来源：http://wfh.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tww.cdnleiting.top

[S55] C++：结构化绑定
来源：http://blq.52xcode.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cnw.zhengqikj.top

[S56] C++：optional
来源：http://zrp.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nuz.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://mxe.andypj.xyz

constexpr int N = 10;
来源：http://huj.sweek.top

[S58] C++：命名空间
来源：http://fzb.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://xgk.hongshengwenyu.top

[S59] C++：静态断言
来源：http://hbp.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yxc.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://zkl.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iig.daria6918.cn

================================================================================
来源：http://zos.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mky.jinqigfzy.top

================================================================================
来源：http://gmr.yvedp.cn

[T01] Kotlin：Hello World
来源：http://dfr.sjlbkw.cn

println("Hello")
来源：http://atk.nanxinkj.top

[T02] Kotlin：变量
来源：http://ian.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ngp.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://dun.zhiwuduotai.top

"值: $b"
来源：http://kac.tanke756.top

[T04] Kotlin：空安全
来源：http://ssc.gzhubu.top

val n: String? = null;  n?.length
来源：http://gfx.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://hsu.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bhf.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://szq.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://icp.meibo888.top

[T07] Kotlin：集合过滤
来源：http://dnx.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://syy.wangdashe.top

[T08] Kotlin：数据类
来源：http://xbp.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://hat.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://emf.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://tmb.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://ywc.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://szt.sufxvd.cn

[T11] Kotlin：协程
来源：http://oby.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://bef.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://fpi.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://cdt.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://txk.hcnkem.com

val m = mapOf("a" to 1)
来源：http://kuc.316326.xyz

[T14] Kotlin：循环
来源：http://vvr.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://yzr.snrcjt.cn

[T15] Kotlin：接口
来源：http://vjv.birdmap.top

interface Shape { fun area(): Double }
来源：http://ous.jiagoushi.top

[T16] Swift：Hello World
来源：http://dbc.jinghuilouyu.cn

print("Hello")
来源：http://ugm.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://xov.sweek.top

var a = 1;  let b = 2
来源：http://bfw.sweek.top

[T18] Swift：字符串插值
来源：http://nfo.hysaishi.cn

"值: \(b)"
来源：http://rlh.aibaodan.cn

[T19] Swift：可选绑定
来源：http://uyr.fktsv.cn

if let n = opt { print(n) }
来源：http://rzo.hammf.cn

[T20] Swift：数组操作
来源：http://klv.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://qhg.vehdjk.com

[T21] Swift：遍历
来源：http://iqb.hcnkem.com

for x in a { print(x) }
来源：http://zsw.uphjek.com

[T22] Swift：字典
来源：http://tcs.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zcy.andypj.xyz

[T23] Swift：函数
来源：http://rfo.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sjp.ybcxt.top

[T24] Swift：闭包
来源：http://pqj.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://car.cheryme.top

[T25] Swift：结构体
来源：http://vhf.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://jhp.fehbvm.com

[T26] Swift：类与重写
来源：http://thj.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://ojd.shzxlz.cn

[T27] Swift：错误处理
来源：http://yyd.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://fyh.tarul.cn

[T28] Swift：枚举
来源：http://jfh.shzxlz.cn

enum Color { case red, green }
来源：http://jur.pycfn.com

[T29] Swift：guard 提前返回
来源：http://pvp.haohaochexian.top

guard let x = opt else { return }
来源：http://rxn.hesvh.cn

[T30] Swift：协议
来源：http://vtw.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://gbu.kuanghao11.cn

[T31] Lua：Hello World
来源：http://iso.chenjidiqi.icu

print("Hello")
来源：http://rfy.ppjwa.cn

[T32] Lua：局部变量
来源：http://sdf.ydzc1.top

local a = 1
来源：http://gov.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://zrx.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jdb.daxiang520.top

[T34] Lua：遍历表
来源：http://ele.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ubl.jiagoushi.top

[T35] Lua：字典表
来源：http://mbd.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://wmi.52xcode.cn

[T36] Lua：函数
来源：http://bnq.sufxvd.cn

function add(a, b) return a + b end
来源：http://bgu.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://kuu.9152youxi.cn

"a" .. "b"
来源：http://jfh.jinqigfzy.top

[T38] Lua：条件
来源：http://ikt.ppjwa.cn

if x > 0 then print("正") end
来源：http://dto.ehwqpu.com

[T39] Lua：模式匹配
来源：http://njh.zhiwuduotai.top

string.find(s, "%d+")
来源：http://qnd.meibo888.top

[T40] Lua：元表
来源：http://fpc.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://kke.shzxlz.cn

[T41] Perl：Hello World
来源：http://wpl.xziqi.cn

print "Hello\n";
来源：http://akk.yongpay.top

[T42] Perl：变量类型
来源：http://itb.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yjl.gotoacloud.top

[T43] Perl：字符串插值
来源：http://rsk.tarul.cn

"值: $a"
来源：http://mvh.vehdjk.com

[T44] Perl：条件
来源：http://mvt.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://qxq.ctjpmb.com

[T45] Perl：数组遍历
来源：http://uyr.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://xfh.tianlin.xyz

[T46] Perl：哈希操作
来源：http://ptm.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bhh.fengsongda.top

[T47] Perl：正则捕获
来源：http://skc.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zse.smart0.xyz

[T48] Perl：正则替换
来源：http://nwr.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wkk.bbcook.cn

[T49] Perl：函数
来源：http://kwe.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yab.bjfxy.top

[T50] Perl：逐行读文件
来源：http://okb.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rvo.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://pnt.gogol.net.cn

[T51] Scala：Hello World
来源：http://byf.zdqjudy.top

println("Hello")
来源：http://wnh.dashuyun.cn

[T52] Scala：变量
来源：http://ipq.sysykeji.top

val a = 1;  var b = 2
来源：http://ghj.tarul.cn

[T53] Scala：字符串插值
来源：http://hov.yongpay.top

s"值: $b"
来源：http://taj.cdnleiting.top

[T54] Scala：集合映射
来源：http://shy.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://ijl.fktsv.cn

[T55] Scala：集合过滤
来源：http://amr.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://wsj.yangfankeji.com

[T56] Scala：样例类
来源：http://qcg.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://irg.cheryme.top

[T57] Scala：模式匹配
来源：http://fga.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://fwh.gzhubu.top

[T58] Scala：函数定义
来源：http://rwh.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://rmp.redwolf501.top

[T59] Scala：循环
来源：http://xgs.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://ifz.havefunace.top

[T60] Scala：折叠
来源：http://nat.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uby.fzhhl.top

================================================================================
来源：http://bpm.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fsi.ehwqpu.com

================================================================================
来源：http://tgi.havefunace.top

[U01] Py：创建虚拟环境
来源：http://ord.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://ioi.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://hql.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://phk.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://shy.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oli.jiagoushi.top

[U04] Py：变量调试打印
来源：http://emf.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jhr.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://yav.yvedp.cn

list(dict.fromkeys(arr))
来源：http://gsn.aibaodan.cn

[U06] Py：合并两个字典
来源：http://mlj.0kj1m.cn

{**a, **b}
来源：http://ogl.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://jsw.yuxming.cn

{v: k for k, v in d.items()}
来源：http://iff.zycfv.cn

[U08] Py：展平二维列表
来源：http://epf.yj20258888.top

[y for x in nested for y in x]
来源：http://nyd.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://sdx.yuxming.cn

max(d, key=d.get)
来源：http://ape.iojbl.cn

[U10] Py：按值排序字典
来源：http://dib.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sjb.52xcode.cn

[U11] Py：生成器表达式
来源：http://pcx.hnxiangtu.top

(x * 2 for x in arr)
来源：http://pgr.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://exw.fehbvm.com

Counter(arr).most_common(3)
来源：http://lef.meibo888.top

[U13] Py：固定长度队列
来源：http://mjw.jyoumei.cn

deque(maxlen=10)
来源：http://tjw.yongpay.top

[U14] Py：分组收集到列表
来源：http://bbm.jqgufenzy.top

defaultdict(list)
来源：http://fhl.dianchejie.cn

[U15] Py：高精度计时
来源：http://upj.kuanghao11.cn

t = time.perf_counter()
来源：http://fki.havefunace.top

[U16] Py：命令行参数解析
来源：http://lmh.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cwm.hywenlv.cn

[U17] Py：初始化日志
来源：http://xsp.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://wyf.hysaishi.cn

[U18] Py：预编译正则
来源：http://wgo.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://rfs.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://tsa.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gbb.vehdjk.com

[U20] Py：缓存函数结果
来源：http://ihr.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://kee.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://fro.bjfxy.top

@contextlib.contextmanager
来源：http://gue.bjfxy.top

[U22] Py：矩阵转置
来源：http://kag.hysaishi.cn

list(zip(*m))
来源：http://rod.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://pxp.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uhh.nanxinkj.top

[U24] Py：路径操作
来源：http://jml.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://omi.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://qct.guowangkeji.top

csv.DictReader(f)
来源：http://rro.hesvh.cn

[U26] Py：并发下载
来源：http://eey.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fnj.daria6918.cn

[U27] Py：异步 HTTP
来源：http://cho.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://cww.yonumen.top

[U28] Py：类型别名
来源：http://ukr.meibo888.top

UserId = int
来源：http://yhs.cdnleiting.top

[U29] Py：属性校验
来源：http://ohs.fzhhl.top

@property 与 @x.setter 配合
来源：http://btc.xinyue.icu

[U30] Py：数据类
来源：http://lqe.gogol.net.cn

@dataclass(slots=True)
来源：http://aii.ydjk.org.cn

[U31] Py：单测
来源：http://djr.zycfv.cn

python -m pytest -q
来源：http://gvb.andypj.xyz

[U32] Py：代码格式化
来源：http://fan.tarul.cn

ruff format . && ruff check --fix .
来源：http://atj.zhijiandao.cn

[U33] Py：打包发布
来源：http://gty.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://wnb.andypj.xyz

[U34] Py：判断编码
来源：http://jri.jqgufenzy.top

chardet.detect(raw)
来源：http://zbx.sufxvd.cn

[U35] Py：发送邮件
来源：http://bdw.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://var.nanxinkj.top

[U36] Py：定时任务
来源：http://dqo.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://iuh.birdmap.top

[U37] Py：读写 Excel
来源：http://taz.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://hlw.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://hyu.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://oyx.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://wsi.chenlongwang.top

sys.stdout.isatty()
来源：http://hbg.xylfe.cn

[U40] Py：打印到标准错误
来源：http://eqv.ehwqpu.com

print("err", file=sys.stderr)
来源：http://wwz.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://rbz.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://emy.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://xxm.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://von.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://ivx.c1oappe.top

namespace App\Http;
来源：http://mdl.bjfxy.top

[U44] PHP：开启严格类型
来源：http://cej.zhijiandao.cn

declare(strict_types=1);
来源：http://riz.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://efq.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ifp.yfazqb.com

[U46] PHP：可空类型
来源：http://rve.9152youxi.cn

?string $name = null
来源：http://hcj.haohaochexian.top

[U47] PHP：联合类型
来源：http://dlr.dashuyun.cn

int|string $id
来源：http://nub.redwolf501.top

[U48] PHP：纯枚举
来源：http://hxr.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wjy.gzhubu.top

[U49] PHP：只读属性
来源：http://rvj.yongpay.top

public readonly string $name
来源：http://krv.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://kzj.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://xlz.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://wfz.shzxlz.cn

[$a, $b] = $arr;
来源：http://cqe.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://elj.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://kch.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://dpo.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://gif.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://dmu.hfpthk.cn

$obj?->method()
来源：http://dmi.gotoacloud.top

[U55] PHP：match 表达式
来源：http://loj.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://plj.hesvh.cn

[U56] PHP：命名参数
来源：http://kgk.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://vxa.jianghu66.top

[U57] PHP：字符串插值
来源：http://sdu.ctjpmb.com

"值: {$a}"
来源：http://kio.hywenlv.cn

[U58] PHP：数组三件套
来源：http://cnq.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://krg.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://xvc.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwr.tanke756.top

[U60] PHP：JSON 编解码
来源：http://mgk.daria6918.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jrd.shuidangran.top

[U61] PHP：正则
来源：http://ihs.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://elt.52xcode.cn

[U62] PHP：日期对象
来源：http://ywe.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fdz.pengpengdd.cyou


<!-- 参考信息 -->