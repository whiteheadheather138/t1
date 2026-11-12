代发 wailian999

[S41] C++：类与构造函数
来源：http://pml.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dbb.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://gym.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://khh.sjlbkw.cn

[S43] C++：智能指针
来源：http://dvy.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://fkf.vqdsnc.cn

[S44] C++：引用传参
来源：http://qka.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://mbo.hywenlv.cn

[S45] C++：lambda
来源：http://kot.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://atc.wangdashe.top

[S46] C++：函数模板
来源：http://mjd.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kuo.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://pki.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mlh.smart0.xyz

[S48] C++：逐行读文件
来源：http://xil.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://ojm.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://mal.shuidangran.top

[S49] C++：写文件
来源：http://dfw.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dmb.yj20258.top

[S50] C++：格式化数字
来源：http://jcp.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tzn.zhengqikj.top

[S51] C++：显式类型转换
来源：http://ojd.hammf.cn

static_cast<double>(a) / b
来源：http://rey.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://eaq.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://ryj.gogol.net.cn

[S53] C++：移动语义
来源：http://cim.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://wvf.zhoulong.xyz

[S54] C++：异常处理
来源：http://cey.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrx.tanke756.top

[S55] C++：结构化绑定
来源：http://lkm.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vef.hnqzz.top

[S56] C++：optional
来源：http://buw.xuanzx.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yqh.9152youxi.cn

[S57] C++：编译期常量
来源：http://ynh.gaohongyu789.top

constexpr int N = 10;
来源：http://eth.316326.xyz

[S58] C++：命名空间
来源：http://ric.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://erc.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://dvm.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cbb.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://nsc.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hah.nwbrower.top

================================================================================
来源：http://bis.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mfx.ywan-chungtsiang.top

================================================================================
来源：http://vrl.xuanzx.com

[T01] Kotlin：Hello World
来源：http://bwd.epnwcf.com

println("Hello")
来源：http://obc.yangfankeji.com

[T02] Kotlin：变量
来源：http://zhv.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lrv.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://tkg.hfpthk.cn

"值: $b"
来源：http://nnf.hnqzz.top

[T04] Kotlin：空安全
来源：http://cmn.aibaodan.cn

val n: String? = null;  n?.length
来源：http://vme.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://gxh.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xxc.bbcook.cn

[T06] Kotlin：集合映射
来源：http://ipa.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ssc.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://ccc.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hxv.hywenlv.cn

[T08] Kotlin：数据类
来源：http://uzi.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://dfm.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://deh.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://jhn.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://dxe.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rby.hnqzz.top

[T11] Kotlin：协程
来源：http://jxu.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fhh.sweek.top

[T12] Kotlin：解构声明
来源：http://emm.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://rlb.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://zbs.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://kym.ydzc1.top

[T14] Kotlin：循环
来源：http://ffh.hysaishi.cn

for (i in 1..10) println(i)
来源：http://iej.52xcode.cn

[T15] Kotlin：接口
来源：http://xww.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://vkj.zhongyouzk.top

[T16] Swift：Hello World
来源：http://njm.0kj1m.cn

print("Hello")
来源：http://wjg.cucudq.cn

[T17] Swift：变量与常量
来源：http://ubf.gogol.net.cn

var a = 1;  let b = 2
来源：http://peo.c1oappe.top

[T18] Swift：字符串插值
来源：http://bvs.tarul.cn

"值: \(b)"
来源：http://xoh.wangdashe.top

[T19] Swift：可选绑定
来源：http://ljg.jqgfzy.top

if let n = opt { print(n) }
来源：http://vnp.zdqjudy.top

[T20] Swift：数组操作
来源：http://lri.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://flm.tanke756.top

[T21] Swift：遍历
来源：http://dsb.zycfv.cn

for x in a { print(x) }
来源：http://fkb.yfazqb.com

[T22] Swift：字典
来源：http://nye.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://hpr.smart0.xyz

[T23] Swift：函数
来源：http://zob.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zwy.yuxming.cn

[T24] Swift：闭包
来源：http://heu.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qqi.jyoumei.cn

[T25] Swift：结构体
来源：http://rcw.chenzaomai.com

struct P { var x: Int }
来源：http://aes.yj20258888.top

[T26] Swift：类与重写
来源：http://tik.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://pnx.yangfankeji.com

[T27] Swift：错误处理
来源：http://ctl.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://prt.cqqwz.cn

[T28] Swift：枚举
来源：http://kif.zhongyouzk.top

enum Color { case red, green }
来源：http://ydg.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://tja.xinyue.icu

guard let x = opt else { return }
来源：http://fyv.yuxming.cn

[T30] Swift：协议
来源：http://xfn.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://djw.yj20258.top

[T31] Lua：Hello World
来源：http://vho.yangfankeji.com

print("Hello")
来源：http://abt.ydjk.org.cn

[T32] Lua：局部变量
来源：http://lrv.jqgufenzy.top

local a = 1
来源：http://dlw.yfazqb.com

[T33] Lua：表（数组）
来源：http://qxa.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://whj.ctjpmb.com

[T34] Lua：遍历表
来源：http://ojp.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cha.yangfankeji.com

[T35] Lua：字典表
来源：http://xsp.dashuyun.cn

local d = { a = 1 };  d.b = 2
来源：http://czj.yvedp.cn

[T36] Lua：函数
来源：http://phb.jianghu66.top

function add(a, b) return a + b end
来源：http://sib.yonumen.top

[T37] Lua：字符串拼接
来源：http://vwu.fehbvm.com

"a" .. "b"
来源：http://ues.yanxiufei.cn

[T38] Lua：条件
来源：http://sqv.yfazqb.com

if x > 0 then print("正") end
来源：http://qfh.dashuyun.cn

[T39] Lua：模式匹配
来源：http://jbh.yanxiufei.cn

string.find(s, "%d+")
来源：http://efi.vqdsnc.cn

[T40] Lua：元表
来源：http://hic.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://gru.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://nmk.tanke756.top

print "Hello\n";
来源：http://wui.jyoumei.cn

[T42] Perl：变量类型
来源：http://dud.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yts.redwolf501.top

[T43] Perl：字符串插值
来源：http://luu.zhongyouzk.top

"值: $a"
来源：http://tkj.sjlbkw.cn

[T44] Perl：条件
来源：http://vcx.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://xaw.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://njt.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://xon.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://mrs.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cob.yongpay.top

[T47] Perl：正则捕获
来源：http://kvt.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dhe.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://uwd.sweek.top

$s =~ s/old/new/g;
来源：http://ucy.zhijiandao.cn

[T49] Perl：函数
来源：http://erw.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ykm.havefunace.top

[T50] Perl：逐行读文件
来源：http://zzh.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bdt.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://qky.tianlin.xyz

[T51] Scala：Hello World
来源：http://use.yj20258888.top

println("Hello")
来源：http://agu.kuanghao11.cn

[T52] Scala：变量
来源：http://kgv.shzxlz.cn

val a = 1;  var b = 2
来源：http://bnd.fehbvm.com

[T53] Scala：字符串插值
来源：http://cfd.epnwcf.com

s"值: $b"
来源：http://dur.yuanzhike.top

[T54] Scala：集合映射
来源：http://uvn.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://rfl.epnwcf.com

[T55] Scala：集合过滤
来源：http://myn.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iql.aizwys.cn

[T56] Scala：样例类
来源：http://mjk.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://yds.wangdashe.top

[T57] Scala：模式匹配
来源：http://nij.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://txs.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://oxw.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nlw.chenlongwang.top

[T59] Scala：循环
来源：http://mhn.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://sjo.52xcode.cn

[T60] Scala：折叠
来源：http://cxt.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lrf.fengsongda.top

================================================================================
来源：http://uku.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kxs.sysykeji.top

================================================================================
来源：http://gpi.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://aar.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://phn.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://vyp.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fim.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://atz.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://syr.xuanzx.com

[U04] Py：变量调试打印
来源：http://yqx.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vuj.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://uwn.daxiang520.top

list(dict.fromkeys(arr))
来源：http://jwl.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://zxz.quarkkingdee.top

{**a, **b}
来源：http://rfb.gaohongyu789.top

[U07] Py：反转字典键值
来源：http://zdp.wangshuangyany.cn

{v: k for k, v in d.items()}
来源：http://pql.yuxming.cn

[U08] Py：展平二维列表
来源：http://xtn.aizwys.cn

[y for x in nested for y in x]
来源：http://dtn.yj20258.top

[U09] Py：字典取最大值的键
来源：http://ufx.jlsjyb.cn

max(d, key=d.get)
来源：http://oeb.bjfxy.top

[U10] Py：按值排序字典
来源：http://kxq.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jha.yj20258888.top

[U11] Py：生成器表达式
来源：http://xpb.vqdsnc.cn

(x * 2 for x in arr)
来源：http://lpl.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://rsp.yongpay.top

Counter(arr).most_common(3)
来源：http://atk.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://idq.smart0.xyz

deque(maxlen=10)
来源：http://wnp.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://afb.xylfe.cn

defaultdict(list)
来源：http://pzx.mhx1999.top

[U15] Py：高精度计时
来源：http://hnq.cheryme.top

t = time.perf_counter()
来源：http://urt.tanke756.top

[U16] Py：命令行参数解析
来源：http://idf.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aci.jqgfzy.top

[U17] Py：初始化日志
来源：http://mfb.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://bqx.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://blv.yuxming.cn

pat = re.compile(r"\d+")
来源：http://cdj.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://mcx.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pal.havefunace.top

[U20] Py：缓存函数结果
来源：http://bev.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://phy.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://jbz.vehdjk.com

@contextlib.contextmanager
来源：http://fab.ybcxt.top

[U22] Py：矩阵转置
来源：http://sga.zhixingplan.top

list(zip(*m))
来源：http://dtj.sweek.top

[U23] Py：分块读取大文件
来源：http://rhu.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ike.zhiwuduotai.top

[U24] Py：路径操作
来源：http://lxq.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eon.yj20258.top

[U25] Py：CSV 按字典读
来源：http://lds.andypj.xyz

csv.DictReader(f)
来源：http://uhk.yongpay.top

[U26] Py：并发下载
来源：http://tsp.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oel.birdmap.top

[U27] Py：异步 HTTP
来源：http://tim.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://gcr.mhx1999.top

[U28] Py：类型别名
来源：http://nla.gogol.net.cn

UserId = int
来源：http://zda.ydzc1.top

[U29] Py：属性校验
来源：http://thf.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://viz.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://uou.birdmap.top

@dataclass(slots=True)
来源：http://fcr.redwolf501.top

[U31] Py：单测
来源：http://bod.jyoumei.cn

python -m pytest -q
来源：http://utb.sjlbkw.cn

[U32] Py：代码格式化
来源：http://ysj.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://dal.yvedp.cn

[U33] Py：打包发布
来源：http://sqg.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://wmy.guowangkeji.top

[U34] Py：判断编码
来源：http://ary.fanxiaobao.xyz

chardet.detect(raw)
来源：http://jom.vehdjk.com

[U35] Py：发送邮件
来源：http://jkq.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wwf.bjfxy.top

[U36] Py：定时任务
来源：http://qki.gotoacloud.top

schedule.every(10).minutes.do(job)
来源：http://kcp.andypj.xyz

[U37] Py：读写 Excel
来源：http://dlb.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://rxf.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://ooh.epnwcf.com

Path(__file__).resolve().parent
来源：http://kor.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://aam.nanxinkj.top

sys.stdout.isatty()
来源：http://bwn.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://nzv.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://ook.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://nza.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://hbe.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://pku.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mze.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://nhz.fengsongda.top

namespace App\Http;
来源：http://ohk.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://guo.jqgufenzy.top

declare(strict_types=1);
来源：http://rwd.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://wrv.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pqz.hammf.cn

[U46] PHP：可空类型
来源：http://mob.jinghuilouyu.cn

?string $name = null
来源：http://bik.aibaodan.cn

[U47] PHP：联合类型
来源：http://cgy.fktsv.cn

int|string $id
来源：http://cvt.chenlongwang.top

[U48] PHP：纯枚举
来源：http://rli.sweek.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sfs.tian-w.cn

[U49] PHP：只读属性
来源：http://swh.tanke756.top

public readonly string $name
来源：http://vhm.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://vju.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://yoj.birdmap.top

[U51] PHP：数组解构
来源：http://pzi.andypj.xyz

[$a, $b] = $arr;
来源：http://pcr.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://tri.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://xmk.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://lbg.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://dvs.fehbvm.com

[U54] PHP：空安全调用
来源：http://gep.yanxiufei.cn

$obj?->method()
来源：http://jsn.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://buq.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fmq.316326.xyz

[U56] PHP：命名参数
来源：http://tyb.hcnkem.com

f(a: 1, b: 2)
来源：http://czq.yvedp.cn

[U57] PHP：字符串插值
来源：http://ozl.sweek.top

"值: {$a}"
来源：http://qiv.sjlbkw.cn

[U58] PHP：数组三件套
来源：http://awy.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dru.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://dgi.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kwv.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://avm.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fxp.sweek.top

[U61] PHP：正则
来源：http://dcf.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kdt.ydzc1.top

[U62] PHP：日期对象
来源：http://ufv.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://had.nanxuanxn.top

[U63] PHP：文件读写
来源：http://liu.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vyj.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://lug.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://ssw.fehbvm.com

[U65] PHP：会话
来源：http://vok.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lde.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://xsq.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tcc.shanyushiyangtech.top


<!-- 参考信息 -->