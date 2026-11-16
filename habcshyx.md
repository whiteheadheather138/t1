代发 wailian999

[S37] C++：set
来源：http://ieq.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tlx.zycfv.cn

[S38] C++：排序
来源：http://ytr.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://rct.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://maq.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hcy.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://qgh.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wkv.yfazqb.com

[S41] C++：类与构造函数
来源：http://zjq.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yta.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://dka.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://quo.ehwqpu.com

[S43] C++：智能指针
来源：http://kju.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://kmq.hnxiangtu.top

[S44] C++：引用传参
来源：http://hwg.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://tjh.52xcode.cn

[S45] C++：lambda
来源：http://ceb.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rdc.quarkkingdee.top

[S46] C++：函数模板
来源：http://zsa.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lyq.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://fav.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jrw.aibaodan.cn

[S48] C++：逐行读文件
来源：http://lgt.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wjd.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://fcl.yj202588.top

[S49] C++：写文件
来源：http://twa.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hyl.9152youxi.cn

[S50] C++：格式化数字
来源：http://eki.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jkv.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://jjz.ppjwa.cn

static_cast<double>(a) / b
来源：http://bjv.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://xjb.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://oet.ivvv.top

[S53] C++：移动语义
来源：http://qyy.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://pch.xylfe.cn

[S54] C++：异常处理
来源：http://lgv.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hpq.zycfv.cn

[S55] C++：结构化绑定
来源：http://xaj.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zbh.dianchejie.cn

[S56] C++：optional
来源：http://utl.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kco.vqdsnc.cn

[S57] C++：编译期常量
来源：http://ctg.cqqwz.cn

constexpr int N = 10;
来源：http://paw.jinqigfzy.top

[S58] C++：命名空间
来源：http://bwi.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://cjg.cucudq.cn

[S59] C++：静态断言
来源：http://ive.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cbu.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://lss.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rnj.wangshuangyany.cn

================================================================================
来源：http://pwk.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjv.yangfankeji.com

================================================================================
来源：http://dxw.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://ljc.zhiwuduotai.top

println("Hello")
来源：http://xir.birdmap.top

[T02] Kotlin：变量
来源：http://tfi.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://omb.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://jhz.epnwcf.com

"值: $b"
来源：http://jye.hesvh.cn

[T04] Kotlin：空安全
来源：http://cly.bjfxy.top

val n: String? = null;  n?.length
来源：http://mxe.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://jdm.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ufw.tarul.cn

[T06] Kotlin：集合映射
来源：http://mol.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xbg.cheryme.top

[T07] Kotlin：集合过滤
来源：http://zew.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lse.chenlongwang.top

[T08] Kotlin：数据类
来源：http://nby.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ghw.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://lwb.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://tpl.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://qyf.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xfr.sweek.top

[T11] Kotlin：协程
来源：http://pwc.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jpq.sweek.top

[T12] Kotlin：解构声明
来源：http://qsh.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://lzm.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://ggl.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://zxr.yuanzhike.top

[T14] Kotlin：循环
来源：http://kee.cucudq.cn

for (i in 1..10) println(i)
来源：http://dqr.pengpengdd.cyou

[T15] Kotlin：接口
来源：http://nts.yj20258.top

interface Shape { fun area(): Double }
来源：http://imk.quarkkingdee.top

[T16] Swift：Hello World
来源：http://kgm.hesvh.cn

print("Hello")
来源：http://omu.cheryme.top

[T17] Swift：变量与常量
来源：http://brg.cucudq.cn

var a = 1;  let b = 2
来源：http://xzm.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://bbb.dashuyun.cn

"值: \(b)"
来源：http://klo.yongpay.top

[T19] Swift：可选绑定
来源：http://iwo.cqqwz.cn

if let n = opt { print(n) }
来源：http://rdt.cheryme.top

[T20] Swift：数组操作
来源：http://jrg.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zqp.yanxiufei.cn

[T21] Swift：遍历
来源：http://lap.shzxlz.cn

for x in a { print(x) }
来源：http://bjp.yvedp.cn

[T22] Swift：字典
来源：http://lmg.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lst.yj202588.top

[T23] Swift：函数
来源：http://ahd.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sbc.zhijiandao.cn

[T24] Swift：闭包
来源：http://esy.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qdm.xuanzx.com

[T25] Swift：结构体
来源：http://chs.zhoulong.xyz

struct P { var x: Int }
来源：http://ewr.nanxuanxn.top

[T26] Swift：类与重写
来源：http://qfh.0kj1m.cn

class A: Base { override func f() {} }
来源：http://kbu.cqqwz.cn

[T27] Swift：错误处理
来源：http://xdp.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://oys.quarkkingdee.top

[T28] Swift：枚举
来源：http://zxt.mhx1999.top

enum Color { case red, green }
来源：http://jpt.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://xyl.yvedp.cn

guard let x = opt else { return }
来源：http://kni.yuanzhike.top

[T30] Swift：协议
来源：http://rkh.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://xtn.hesvh.cn

[T31] Lua：Hello World
来源：http://oxg.cheryme.top

print("Hello")
来源：http://xdt.sxryk.cn

[T32] Lua：局部变量
来源：http://ctx.gogol.net.cn

local a = 1
来源：http://fjt.hammf.cn

[T33] Lua：表（数组）
来源：http://tlb.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qzu.meibo888.top

[T34] Lua：遍历表
来源：http://oys.tanke756.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dra.uphjek.com

[T35] Lua：字典表
来源：http://ete.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://tlh.316326.xyz

[T36] Lua：函数
来源：http://hzr.kuanghao11.cn

function add(a, b) return a + b end
来源：http://lgs.c1oappe.top

[T37] Lua：字符串拼接
来源：http://ncm.ivvv.top

"a" .. "b"
来源：http://jub.zycfv.cn

[T38] Lua：条件
来源：http://krw.yueranfly.top

if x > 0 then print("正") end
来源：http://vlc.zhixingplan.top

[T39] Lua：模式匹配
来源：http://uvr.yvedp.cn

string.find(s, "%d+")
来源：http://qlv.ppjwa.cn

[T40] Lua：元表
来源：http://usy.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://zba.fengsongda.top

[T41] Perl：Hello World
来源：http://gcn.jinghuilouyu.cn

print "Hello\n";
来源：http://nuw.zhoulong.xyz

[T42] Perl：变量类型
来源：http://uqw.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://unw.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://uhy.shuidangran.top

"值: $a"
来源：http://qwc.xziqi.cn

[T44] Perl：条件
来源：http://ojo.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://eys.yuanzhike.top

[T45] Perl：数组遍历
来源：http://rbw.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://kse.ydzc1.top

[T46] Perl：哈希操作
来源：http://wbv.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ged.52xcode.cn

[T47] Perl：正则捕获
来源：http://xuy.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qht.ivvv.top

[T48] Perl：正则替换
来源：http://nlb.hywenlv.cn

$s =~ s/old/new/g;
来源：http://wjd.nanxinkj.top

[T49] Perl：函数
来源：http://dza.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sja.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://eix.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hfi.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://yok.fzhhl.top

[T51] Scala：Hello World
来源：http://jsc.aizwys.cn

println("Hello")
来源：http://pcu.zdbjq.cn

[T52] Scala：变量
来源：http://naz.chenzaomai.com

val a = 1;  var b = 2
来源：http://sku.zhixingplan.top

[T53] Scala：字符串插值
来源：http://isi.jinqigfzy.top

s"值: $b"
来源：http://slx.nwbrower.top

[T54] Scala：集合映射
来源：http://lna.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://vyt.gogol.net.cn

[T55] Scala：集合过滤
来源：http://wbq.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://evs.hfpthk.cn

[T56] Scala：样例类
来源：http://rre.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://ceo.hnqzz.top

[T57] Scala：模式匹配
来源：http://nvy.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://wat.ydzc1.top

[T58] Scala：函数定义
来源：http://qni.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://ugj.0kj1m.cn

[T59] Scala：循环
来源：http://dxm.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://nsm.fzhhl.top

[T60] Scala：折叠
来源：http://rhy.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ujt.yuanzhike.top

================================================================================
来源：http://tha.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bmq.shanyushiyangtech.top

================================================================================
来源：http://ucc.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://chn.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://lmt.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://lnj.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://elo.hammf.cn

[U03] Py：加载 .env 配置
来源：http://cji.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ibt.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://iaj.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pjv.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://gnu.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://izc.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://kky.yuanzhike.top

{**a, **b}
来源：http://kfg.tian-w.cn

[U07] Py：反转字典键值
来源：http://apm.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://fbg.xinyue.icu

[U08] Py：展平二维列表
来源：http://hbb.smart0.xyz

[y for x in nested for y in x]
来源：http://olo.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://dxy.andypj.xyz

max(d, key=d.get)
来源：http://trn.yj20258888.top

[U10] Py：按值排序字典
来源：http://syq.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gzd.snrcjt.cn

[U11] Py：生成器表达式
来源：http://upx.hywenlv.cn

(x * 2 for x in arr)
来源：http://nrq.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://pnc.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://hnm.ppjwa.cn

[U13] Py：固定长度队列
来源：http://fqp.cashguo.top

deque(maxlen=10)
来源：http://twg.ivvv.top

[U14] Py：分组收集到列表
来源：http://zap.pengpengdd.cyou

defaultdict(list)
来源：http://sbc.hysaishi.cn

[U15] Py：高精度计时
来源：http://qap.dianchejie.cn

t = time.perf_counter()
来源：http://pgo.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://syh.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rjs.vqdsnc.cn

[U17] Py：初始化日志
来源：http://emv.uphjek.com

logging.basicConfig(level=logging.INFO)
来源：http://fqz.xinyue.icu

[U18] Py：预编译正则
来源：http://oxa.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://yha.sxryk.cn

[U19] Py：正则替换带回调
来源：http://leg.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bhb.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://eco.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://ijm.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://kcn.vehdjk.com

@contextlib.contextmanager
来源：http://dee.cashguo.top

[U22] Py：矩阵转置
来源：http://dfp.hysaishi.cn

list(zip(*m))
来源：http://sri.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://srh.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nbd.bjfxy.top

[U24] Py：路径操作
来源：http://zbv.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fru.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://wkv.c1oappe.top

csv.DictReader(f)
来源：http://ufj.hongshengwenyu.top

[U26] Py：并发下载
来源：http://hto.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://luu.hcnkem.com

[U27] Py：异步 HTTP
来源：http://qwm.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://gzf.yj20258.top

[U28] Py：类型别名
来源：http://tpc.ctjpmb.com

UserId = int
来源：http://aya.yanxiufei.cn

[U29] Py：属性校验
来源：http://adf.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://orl.ehwqpu.com

[U30] Py：数据类
来源：http://ydj.hcnkem.com

@dataclass(slots=True)
来源：http://fip.meibo888.top

[U31] Py：单测
来源：http://tjq.meibo888.top

python -m pytest -q
来源：http://azj.sjlbkw.cn

[U32] Py：代码格式化
来源：http://hnw.bbcook.cn

ruff format . && ruff check --fix .
来源：http://mpg.cdnleiting.top

[U33] Py：打包发布
来源：http://erz.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://bbt.hcnkem.com

[U34] Py：判断编码
来源：http://ley.gaohongyu789.top

chardet.detect(raw)
来源：http://sci.aibaodan.cn

[U35] Py：发送邮件
来源：http://bvv.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xbl.kuanghao11.cn

[U36] Py：定时任务
来源：http://lxw.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://mgb.yj20258888.top

[U37] Py：读写 Excel
来源：http://qtv.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nrc.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://lfq.iojbl.cn

Path(__file__).resolve().parent
来源：http://uqz.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://vpr.yueranfly.top

sys.stdout.isatty()
来源：http://ahc.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://dcj.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://vsn.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://woz.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://lah.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://gpo.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://era.hcnkem.com

[U43] PHP：声明命名空间
来源：http://hfv.ctjpmb.com

namespace App\Http;
来源：http://obc.yueranfly.top

[U44] PHP：开启严格类型
来源：http://uqd.gzhubu.top

declare(strict_types=1);
来源：http://zmb.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://tyx.wangshuangyany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfp.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://uib.bjfxy.top

?string $name = null
来源：http://dba.yj20258.top

[U47] PHP：联合类型
来源：http://wgc.zhengqikj.top

int|string $id
来源：http://vht.havefunace.top

[U48] PHP：纯枚举
来源：http://bgk.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xhj.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://ooz.gogol.net.cn

public readonly string $name
来源：http://yln.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://pnl.yongpay.top

public function __construct(private int $id) {}
来源：http://rxe.snrcjt.cn

[U51] PHP：数组解构
来源：http://jog.vqdsnc.cn

[$a, $b] = $arr;
来源：http://ogm.aibaodan.cn

[U52] PHP：箭头函数
来源：http://acx.tarul.cn

$double = fn($x) => $x * 2;
来源：http://hwz.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://gdh.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://kqm.fehbvm.com

[U54] PHP：空安全调用
来源：http://jou.ivvv.top

$obj?->method()
来源：http://vya.birdmap.top

[U55] PHP：match 表达式
来源：http://yuh.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nba.ehwqpu.com

[U56] PHP：命名参数
来源：http://rig.ppjwa.cn

f(a: 1, b: 2)
来源：http://xhx.gotoacloud.top

[U57] PHP：字符串插值
来源：http://bvh.ppjwa.cn

"值: {$a}"
来源：http://ahd.yongpay.top

[U58] PHP：数组三件套
来源：http://nen.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://abt.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://anj.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fbq.fktsv.cn

[U60] PHP：JSON 编解码
来源：http://qoa.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://znk.hesvh.cn

[U61] PHP：正则
来源：http://hpw.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://snm.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://wnn.tarul.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gfs.bjfxy.top


<!-- 参考信息 -->