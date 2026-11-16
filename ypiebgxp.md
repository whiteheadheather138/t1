代发 wailian999

[S35] C++：map
来源：http://ecu.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mvj.dashuyun.cn

[S36] C++：unordered_map
来源：http://iju.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://whe.cqqwz.cn

[S37] C++：set
来源：http://dbj.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://muk.ydzc1.top

[S38] C++：排序
来源：http://pwn.sweek.top

std::sort(v.begin(), v.end());
来源：http://ygu.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://kor.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://acf.feifeiyinyue.top

[S40] C++：查找元素
来源：http://gph.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jbf.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://vwx.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://plk.fzhhl.top

[S42] C++：继承与虚函数
来源：http://lfw.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://yhm.daxiang520.top

[S43] C++：智能指针
来源：http://apf.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://nxn.jqgfzy.top

[S44] C++：引用传参
来源：http://iap.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://ytx.nwbrower.top

[S45] C++：lambda
来源：http://wrm.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://lou.xuanzx.com

[S46] C++：函数模板
来源：http://obc.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vyf.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://kbz.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yeh.xinyue.icu

[S48] C++：逐行读文件
来源：http://pmq.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://bpa.meibo888.top

while (std::getline(in, line)) { }
来源：http://wfz.fanxiaobao.xyz

[S49] C++：写文件
来源：http://tcq.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vjm.aibaodan.cn

[S50] C++：格式化数字
来源：http://fdj.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rkf.yj20258.top

[S51] C++：显式类型转换
来源：http://dnw.kuanghao11.cn

static_cast<double>(a) / b
来源：http://shr.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://lhr.andypj.xyz

int size() const noexcept { return n_; }
来源：http://dfl.gogol.net.cn

[S53] C++：移动语义
来源：http://yca.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://llx.hysaishi.cn

[S54] C++：异常处理
来源：http://igy.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vzk.gzhubu.top

[S55] C++：结构化绑定
来源：http://lmr.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://idu.gzhubu.top

[S56] C++：optional
来源：http://syd.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hss.svipenyu.cn

[S57] C++：编译期常量
来源：http://pnz.ybcxt.top

constexpr int N = 10;
来源：http://fkv.jiagoushi.top

[S58] C++：命名空间
来源：http://glq.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://vnc.zhoulong.xyz

[S59] C++：静态断言
来源：http://hto.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xzs.uphjek.com

[S60] C++：遍历并删除元素
来源：http://pnj.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yzn.c1oappe.top

================================================================================
来源：http://sxz.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tok.ydjk.org.cn

================================================================================
来源：http://xsp.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://pgp.yangfankeji.com

println("Hello")
来源：http://waf.tianlin.xyz

[T02] Kotlin：变量
来源：http://sgg.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xka.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://isc.fzhhl.top

"值: $b"
来源：http://ary.epnwcf.com

[T04] Kotlin：空安全
来源：http://kap.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://nga.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://gwx.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://joz.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://jxt.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://anh.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://ngu.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tie.ivvv.top

[T08] Kotlin：数据类
来源：http://upx.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://vnp.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://ybm.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://lcy.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://kyz.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nue.jqgfzy.top

[T11] Kotlin：协程
来源：http://gqs.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tbf.sxryk.cn

[T12] Kotlin：解构声明
来源：http://nyo.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://dku.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://wsq.yongpay.top

val m = mapOf("a" to 1)
来源：http://vhp.sweek.top

[T14] Kotlin：循环
来源：http://ywq.yuanzhike.top

for (i in 1..10) println(i)
来源：http://sqx.ctjpmb.com

[T15] Kotlin：接口
来源：http://iqh.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://fuk.zhijiandao.cn

[T16] Swift：Hello World
来源：http://udi.vqdsnc.cn

print("Hello")
来源：http://ona.tarul.cn

[T17] Swift：变量与常量
来源：http://akz.sxryk.cn

var a = 1;  let b = 2
来源：http://klz.tian-w.cn

[T18] Swift：字符串插值
来源：http://klr.yfazqb.com

"值: \(b)"
来源：http://xnc.yvedp.cn

[T19] Swift：可选绑定
来源：http://cla.jlsjyb.cn

if let n = opt { print(n) }
来源：http://xit.cqqwz.cn

[T20] Swift：数组操作
来源：http://mvw.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://wdc.zycfv.cn

[T21] Swift：遍历
来源：http://pzq.ydjk.org.cn

for x in a { print(x) }
来源：http://myq.vqdsnc.cn

[T22] Swift：字典
来源：http://uuw.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lnf.yueranfly.top

[T23] Swift：函数
来源：http://kdf.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jxn.xziqi.cn

[T24] Swift：闭包
来源：http://dso.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://dsn.tianlin.xyz

[T25] Swift：结构体
来源：http://bow.guowangkeji.top

struct P { var x: Int }
来源：http://yfv.yuanzhike.top

[T26] Swift：类与重写
来源：http://saa.hammf.cn

class A: Base { override func f() {} }
来源：http://qyp.jiagoushi.top

[T27] Swift：错误处理
来源：http://yjz.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://dom.meibo888.top

[T28] Swift：枚举
来源：http://uhw.yonumen.top

enum Color { case red, green }
来源：http://jvs.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://geo.jinqigfzy.top

guard let x = opt else { return }
来源：http://kwf.hesvh.cn

[T30] Swift：协议
来源：http://lcj.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://jmi.hesvh.cn

[T31] Lua：Hello World
来源：http://zwq.meibo888.top

print("Hello")
来源：http://hvv.yj202588.top

[T32] Lua：局部变量
来源：http://gxx.zdbjq.cn

local a = 1
来源：http://zew.sysykeji.top

[T33] Lua：表（数组）
来源：http://nwg.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gft.yvedp.cn

[T34] Lua：遍历表
来源：http://lmz.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://amt.gotoacloud.top

[T35] Lua：字典表
来源：http://joa.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://boo.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://suw.fktsv.cn

function add(a, b) return a + b end
来源：http://jgh.yfazqb.com

[T37] Lua：字符串拼接
来源：http://mfb.nanxuanxn.top

"a" .. "b"
来源：http://ofm.yj20258888.top

[T38] Lua：条件
来源：http://haq.yanxiufei.cn

if x > 0 then print("正") end
来源：http://cxg.yfazqb.com

[T39] Lua：模式匹配
来源：http://abh.cheryme.top

string.find(s, "%d+")
来源：http://bom.zdqjudy.top

[T40] Lua：元表
来源：http://ggw.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://nne.hfpthk.cn

[T41] Perl：Hello World
来源：http://gvg.yj20258888.top

print "Hello\n";
来源：http://sgj.xuanzx.com

[T42] Perl：变量类型
来源：http://jux.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zhf.zdqjudy.top

[T43] Perl：字符串插值
来源：http://xww.vqdsnc.cn

"值: $a"
来源：http://ntr.yueranfly.top

[T44] Perl：条件
来源：http://mxa.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://phm.smart0.xyz

[T45] Perl：数组遍历
来源：http://wdw.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://dga.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://bse.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://idf.gzhubu.top

[T47] Perl：正则捕获
来源：http://bfc.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bvj.redwolf501.top

[T48] Perl：正则替换
来源：http://tde.yj20258.top

$s =~ s/old/new/g;
来源：http://suc.feifeiyinyue.top

[T49] Perl：函数
来源：http://lsk.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ppi.tian-w.cn

[T50] Perl：逐行读文件
来源：http://kxz.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jao.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://cbi.chenlongwang.top

[T51] Scala：Hello World
来源：http://ytg.guannengcc.top

println("Hello")
来源：http://kdn.hongshengwenyu.top

[T52] Scala：变量
来源：http://zxu.bbcook.cn

val a = 1;  var b = 2
来源：http://hjw.tanke756.top

[T53] Scala：字符串插值
来源：http://hzd.aibaodan.cn

s"值: $b"
来源：http://grx.iojbl.cn

[T54] Scala：集合映射
来源：http://uxf.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://nhj.cucudq.cn

[T55] Scala：集合过滤
来源：http://lkm.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://dke.ctjpmb.com

[T56] Scala：样例类
来源：http://wdn.0kj1m.cn

case class User(name: String, age: Int)
来源：http://sfc.cheryme.top

[T57] Scala：模式匹配
来源：http://jgl.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://utk.tianlin.xyz

[T58] Scala：函数定义
来源：http://ijt.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://zrz.haohaochexian.top

[T59] Scala：循环
来源：http://hqe.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://ttg.dashuyun.cn

[T60] Scala：折叠
来源：http://rdm.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zkj.yj202588.top

================================================================================
来源：http://xto.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dpy.jqgufenzy.top

================================================================================
来源：http://foc.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://xca.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://bzj.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://tkd.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tkl.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://kvm.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sho.pycfn.com

[U04] Py：变量调试打印
来源：http://qbs.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ssd.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://kue.hnqzz.top

list(dict.fromkeys(arr))
来源：http://fym.bjfxy.top

[U06] Py：合并两个字典
来源：http://lyp.xylfe.cn

{**a, **b}
来源：http://rem.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://icu.yueranfly.top

{v: k for k, v in d.items()}
来源：http://sev.snrcjt.cn

[U08] Py：展平二维列表
来源：http://pzw.yvedp.cn

[y for x in nested for y in x]
来源：http://fsn.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://pfu.fengsongda.top

max(d, key=d.get)
来源：http://uyd.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://hve.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://euu.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://syb.redwolf501.top

(x * 2 for x in arr)
来源：http://igs.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://kxq.fktsv.cn

Counter(arr).most_common(3)
来源：http://xvy.fehbvm.com

[U13] Py：固定长度队列
来源：http://tfe.guannengcc.top

deque(maxlen=10)
来源：http://zer.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://mzp.ywan-chungtsiang.top

defaultdict(list)
来源：http://ytj.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://bfs.jyoumei.cn

t = time.perf_counter()
来源：http://mnm.xinyue.icu

[U16] Py：命令行参数解析
来源：http://edv.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dzi.jyoumei.cn

[U17] Py：初始化日志
来源：http://qac.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://yrb.jqgufenzy.top

[U18] Py：预编译正则
来源：http://ybm.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://rhx.redwolf501.top

[U19] Py：正则替换带回调
来源：http://alt.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qag.fehbvm.com

[U20] Py：缓存函数结果
来源：http://vhk.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://ebm.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://nrv.yj20258888.top

@contextlib.contextmanager
来源：http://kyw.fehbvm.com

[U22] Py：矩阵转置
来源：http://ebf.shanyushiyangtech.top

list(zip(*m))
来源：http://ngg.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://iin.zhengqikj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eeo.tianlin.xyz

[U24] Py：路径操作
来源：http://yuu.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pvl.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://vyg.feifeiyinyue.top

csv.DictReader(f)
来源：http://ieu.epnwcf.com

[U26] Py：并发下载
来源：http://put.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vvg.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://nob.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://pnk.haohaochexian.top

[U28] Py：类型别名
来源：http://mug.cqqwz.cn

UserId = int
来源：http://ukj.jqgufenzy.top

[U29] Py：属性校验
来源：http://enr.mhx1999.top

@property 与 @x.setter 配合
来源：http://uyh.tanke756.top

[U30] Py：数据类
来源：http://byo.sxryk.cn

@dataclass(slots=True)
来源：http://zaf.hammf.cn

[U31] Py：单测
来源：http://yhn.vehdjk.com

python -m pytest -q
来源：http://osa.pycfn.com

[U32] Py：代码格式化
来源：http://dik.jianghu66.top

ruff format . && ruff check --fix .
来源：http://pil.jyoumei.cn

[U33] Py：打包发布
来源：http://txo.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://jdp.sjlbkw.cn

[U34] Py：判断编码
来源：http://mzs.fengsongda.top

chardet.detect(raw)
来源：http://rem.ehwqpu.com

[U35] Py：发送邮件
来源：http://axk.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://djt.hesvh.cn

[U36] Py：定时任务
来源：http://mbb.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://sux.shuidangran.top

[U37] Py：读写 Excel
来源：http://lpk.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://ntc.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://exd.hnqzz.top

Path(__file__).resolve().parent
来源：http://ahb.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://fjy.yanxiufei.cn

sys.stdout.isatty()
来源：http://zno.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://dex.svipenyu.cn

print("err", file=sys.stderr)
来源：http://tzm.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://npz.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qpn.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://jmd.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uck.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://uah.0kj1m.cn

namespace App\Http;
来源：http://imh.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://uyb.zycfv.cn

declare(strict_types=1);
来源：http://rlq.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://tgr.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://ewf.ehwqpu.com

[U46] PHP：可空类型
来源：http://ota.gotoacloud.top

?string $name = null
来源：http://eop.jinqigufen.top

[U47] PHP：联合类型
来源：http://wzn.xinyue.icu

int|string $id
来源：http://qfv.yueranfly.top

[U48] PHP：纯枚举
来源：http://aqq.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rag.nwbrower.top

[U49] PHP：只读属性
来源：http://rvt.shanyushiyangtech.top

public readonly string $name
来源：http://ezk.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://cjw.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://ojj.yj20258888.top

[U51] PHP：数组解构
来源：http://gpo.guannengcc.top

[$a, $b] = $arr;
来源：http://tvw.pycfn.com

[U52] PHP：箭头函数
来源：http://chh.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://tdq.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://xzg.havefunace.top

$v = $a ?? $b ?? "default";
来源：http://rue.tanke756.top

[U54] PHP：空安全调用
来源：http://wan.sufxvd.cn

$obj?->method()
来源：http://djm.iojbl.cn

[U55] PHP：match 表达式
来源：http://tjj.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eau.zhoulong.xyz

[U56] PHP：命名参数
来源：http://ctu.uphjek.com

f(a: 1, b: 2)
来源：http://gfj.ppjwa.cn

[U57] PHP：字符串插值
来源：http://emg.xuetiantiany.cn

"值: {$a}"
来源：http://gns.hesvh.cn

[U58] PHP：数组三件套
来源：http://nzr.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cwd.yj20258888.top

[U59] PHP：自定义排序
来源：http://mwg.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kgb.316326.xyz

[U60] PHP：JSON 编解码
来源：http://tjs.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://adm.ctjpmb.com


<!-- 参考信息 -->