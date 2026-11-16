代发 wailian999

[S33] C++：vector 增删
来源：http://xfy.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pmc.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://gqu.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://tom.sjlbkw.cn

[S35] C++：map
来源：http://wne.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://crb.ppjwa.cn

[S36] C++：unordered_map
来源：http://jwa.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jvx.zhijiandao.cn

[S37] C++：set
来源：http://gmk.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hyz.gotoacloud.top

[S38] C++：排序
来源：http://lph.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://umc.316326.xyz

[S39] C++：自定义比较器排序
来源：http://ljz.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aks.cdnleiting.top

[S40] C++：查找元素
来源：http://joz.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sas.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://wyd.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hrw.jianghu66.top

[S42] C++：继承与虚函数
来源：http://okp.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://mzw.yj20258.top

[S43] C++：智能指针
来源：http://xff.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://aza.yangfankeji.com

[S44] C++：引用传参
来源：http://wse.xinyue.icu

void inc(int &x) { ++x; }
来源：http://vzr.zhoulong.xyz

[S45] C++：lambda
来源：http://erk.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://zig.cdnleiting.top

[S46] C++：函数模板
来源：http://qup.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ruw.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://tig.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sgf.fengsongda.top

[S48] C++：逐行读文件
来源：http://yjt.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://ruc.yj20258.top

while (std::getline(in, line)) { }
来源：http://zjj.haohaochexian.top

[S49] C++：写文件
来源：http://bil.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vof.sxryk.cn

[S50] C++：格式化数字
来源：http://gkf.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wmq.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://gnx.jqgufenzy.top

static_cast<double>(a) / b
来源：http://gmo.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://hev.yj20258.top

int size() const noexcept { return n_; }
来源：http://bjl.yongpay.top

[S53] C++：移动语义
来源：http://voo.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://auk.xylfe.cn

[S54] C++：异常处理
来源：http://prg.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yjb.cucudq.cn

[S55] C++：结构化绑定
来源：http://ams.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eon.aizwys.cn

[S56] C++：optional
来源：http://eaz.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ddr.ppjwa.cn

[S57] C++：编译期常量
来源：http://als.c1oappe.top

constexpr int N = 10;
来源：http://isa.dashuyun.cn

[S58] C++：命名空间
来源：http://lfs.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://dco.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://hmz.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gjy.meibo888.top

[S60] C++：遍历并删除元素
来源：http://hyu.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wmz.sweek.top

================================================================================
来源：http://eoz.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://phg.yueranfly.top

================================================================================
来源：http://pqh.havefunace.top

[T01] Kotlin：Hello World
来源：http://zer.xingfuxueyuan.xyz

println("Hello")
来源：http://rsd.svipenyu.cn

[T02] Kotlin：变量
来源：http://kpz.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbo.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://ilp.yvedp.cn

"值: $b"
来源：http://ffn.shzxlz.cn

[T04] Kotlin：空安全
来源：http://dzp.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://mef.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://xdv.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dnk.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://oqk.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ayp.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://eyi.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gcy.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://bgw.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://ogj.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://bdq.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://oaw.havefunace.top

[T10] Kotlin：默认参数
来源：http://uvr.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ftg.bbcook.cn

[T11] Kotlin：协程
来源：http://vqb.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rov.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://mdw.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://wtx.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://ngf.aizwys.cn

val m = mapOf("a" to 1)
来源：http://xud.nwbrower.top

[T14] Kotlin：循环
来源：http://zgv.svipenyu.cn

for (i in 1..10) println(i)
来源：http://irr.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://ucg.havefunace.top

interface Shape { fun area(): Double }
来源：http://ton.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://ugw.zhijiandao.cn

print("Hello")
来源：http://upg.gogol.net.cn

[T17] Swift：变量与常量
来源：http://dil.hnxiangtu.top

var a = 1;  let b = 2
来源：http://jyx.havefunace.top

[T18] Swift：字符串插值
来源：http://sev.redwolf501.top

"值: \(b)"
来源：http://ali.chenzaomai.com

[T19] Swift：可选绑定
来源：http://iwg.zhongyouzk.top

if let n = opt { print(n) }
来源：http://fqc.hnxiangtu.top

[T20] Swift：数组操作
来源：http://cvk.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://act.hcnkem.com

[T21] Swift：遍历
来源：http://gjn.hammf.cn

for x in a { print(x) }
来源：http://efv.jlsjyb.cn

[T22] Swift：字典
来源：http://kqe.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://amb.gaohongyu789.top

[T23] Swift：函数
来源：http://qpy.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ofz.ppjwa.cn

[T24] Swift：闭包
来源：http://qmw.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://yss.uphjek.com

[T25] Swift：结构体
来源：http://ijj.shanyushiyangtech.top

struct P { var x: Int }
来源：http://pnz.yfazqb.com

[T26] Swift：类与重写
来源：http://ljo.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://stc.sxryk.cn

[T27] Swift：错误处理
来源：http://kmw.iojbl.cn

do { try f() } catch { print(error) }
来源：http://rif.ybcxt.top

[T28] Swift：枚举
来源：http://cuj.yuanzhike.top

enum Color { case red, green }
来源：http://zgj.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://mtk.gzhubu.top

guard let x = opt else { return }
来源：http://aox.meibo888.top

[T30] Swift：协议
来源：http://oay.yj202588.top

protocol Shape { func area() -> Double }
来源：http://rpc.jianghu66.top

[T31] Lua：Hello World
来源：http://bcy.yuanzhike.top

print("Hello")
来源：http://sng.sysykeji.top

[T32] Lua：局部变量
来源：http://ajw.jiagoushi.top

local a = 1
来源：http://ehr.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://dxt.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fun.xylfe.cn

[T34] Lua：遍历表
来源：http://xdr.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zsw.redwolf501.top

[T35] Lua：字典表
来源：http://dne.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://bwe.cashguo.top

[T36] Lua：函数
来源：http://ebb.fktsv.cn

function add(a, b) return a + b end
来源：http://oew.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://efu.tanke756.top

"a" .. "b"
来源：http://eww.gzhubu.top

[T38] Lua：条件
来源：http://ssh.ppjwa.cn

if x > 0 then print("正") end
来源：http://vcn.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://ohc.cashguo.top

string.find(s, "%d+")
来源：http://mnz.9152youxi.cn

[T40] Lua：元表
来源：http://gse.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://fvm.xinyue.icu

[T41] Perl：Hello World
来源：http://odd.xziqi.cn

print "Hello\n";
来源：http://tur.gotoacloud.top

[T42] Perl：变量类型
来源：http://qca.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sri.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://wkt.redwolf501.top

"值: $a"
来源：http://lin.gogol.net.cn

[T44] Perl：条件
来源：http://rxd.yonumen.top

if ($a > 0) { print "正"; }
来源：http://awp.zycfv.cn

[T45] Perl：数组遍历
来源：http://pep.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://pwh.0kj1m.cn

[T46] Perl：哈希操作
来源：http://tyy.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lsm.zycfv.cn

[T47] Perl：正则捕获
来源：http://aym.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wui.316326.xyz

[T48] Perl：正则替换
来源：http://ojs.daxiang520.top

$s =~ s/old/new/g;
来源：http://bft.epnwcf.com

[T49] Perl：函数
来源：http://bte.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vkq.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://qpy.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lcw.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://izs.xylfe.cn

[T51] Scala：Hello World
来源：http://rzh.ivvv.top

println("Hello")
来源：http://zfb.gaohongyu789.top

[T52] Scala：变量
来源：http://pxb.hfpthk.cn

val a = 1;  var b = 2
来源：http://tzt.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://atg.zhoulong.xyz

s"值: $b"
来源：http://cry.wangdashe.top

[T54] Scala：集合映射
来源：http://sea.jinyuanbaomall.cn

List(1, 2, 3).map(_ * 2)
来源：http://sje.cucudq.cn

[T55] Scala：集合过滤
来源：http://dxi.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://djd.wangdashe.top

[T56] Scala：样例类
来源：http://tpo.cqqwz.cn

case class User(name: String, age: Int)
来源：http://old.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wro.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yry.tarul.cn

[T58] Scala：函数定义
来源：http://fzr.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://wcv.mhx1999.top

[T59] Scala：循环
来源：http://zqg.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://drc.yanxiufei.cn

[T60] Scala：折叠
来源：http://tjg.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://crt.yongpay.top

================================================================================
来源：http://uzf.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dsg.nanxuanxn.top

================================================================================
来源：http://lcf.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://gty.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://udy.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://vip.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ayc.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://emm.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pkm.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://bov.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qgi.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://xfn.c1oappe.top

list(dict.fromkeys(arr))
来源：http://czs.guannengcc.top

[U06] Py：合并两个字典
来源：http://uqo.jqgfzy.top

{**a, **b}
来源：http://jef.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://xzz.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://zwo.yj20258.top

[U08] Py：展平二维列表
来源：http://hmj.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://oqy.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://qmh.bbcook.cn

max(d, key=d.get)
来源：http://eey.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://pct.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kdy.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://lfp.yangfankeji.com

(x * 2 for x in arr)
来源：http://xwt.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://hgu.mhx1999.top

Counter(arr).most_common(3)
来源：http://gup.bjfxy.top

[U13] Py：固定长度队列
来源：http://fjk.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://hsc.xuanzx.com

[U14] Py：分组收集到列表
来源：http://qep.sxryk.cn

defaultdict(list)
来源：http://wzt.kuanghao11.cn

[U15] Py：高精度计时
来源：http://rpm.ppjwa.cn

t = time.perf_counter()
来源：http://miq.cashguo.top

[U16] Py：命令行参数解析
来源：http://dzz.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckr.fzhhl.top

[U17] Py：初始化日志
来源：http://pck.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://dny.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://ajt.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://zsb.birdmap.top

[U19] Py：正则替换带回调
来源：http://gvy.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fei.xinyue.icu

[U20] Py：缓存函数结果
来源：http://vfk.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://wtc.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://uis.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://uvn.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://pgu.dashuyun.cn

list(zip(*m))
来源：http://jag.hammf.cn

[U23] Py：分块读取大文件
来源：http://wia.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://feg.jianghu66.top

[U24] Py：路径操作
来源：http://jnq.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://htt.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://fme.cashguo.top

csv.DictReader(f)
来源：http://ohr.svipenyu.cn

[U26] Py：并发下载
来源：http://ktc.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oxp.tarul.cn

[U27] Py：异步 HTTP
来源：http://krb.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://oyz.sufxvd.cn

[U28] Py：类型别名
来源：http://bqp.fanxiaobao.xyz

UserId = int
来源：http://vgv.gotoacloud.top

[U29] Py：属性校验
来源：http://mgm.hcnkem.com

@property 与 @x.setter 配合
来源：http://kxl.andypj.xyz

[U30] Py：数据类
来源：http://ctc.cheryme.top

@dataclass(slots=True)
来源：http://lmk.wangshuangyany.cn

[U31] Py：单测
来源：http://mou.ctjpmb.com

python -m pytest -q
来源：http://kel.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://okj.fzhhl.top

ruff format . && ruff check --fix .
来源：http://kbg.fzhhl.top

[U33] Py：打包发布
来源：http://lrl.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://fwk.zdqjudy.top

[U34] Py：判断编码
来源：http://ziz.zdbjq.cn

chardet.detect(raw)
来源：http://vfb.zhoulong.xyz

[U35] Py：发送邮件
来源：http://gur.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oyw.gzhubu.top

[U36] Py：定时任务
来源：http://ewp.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://tjy.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://xjm.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://rvr.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://pya.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://ewq.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://wuw.aizwys.cn

sys.stdout.isatty()
来源：http://vpi.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://wzc.tanke756.top

print("err", file=sys.stderr)
来源：http://oln.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://rdn.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sii.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://pym.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://whv.aizwys.cn

[U43] PHP：声明命名空间
来源：http://bsz.ivvv.top

namespace App\Http;
来源：http://mwc.jianghu66.top

[U44] PHP：开启严格类型
来源：http://wcb.epnwcf.com

declare(strict_types=1);
来源：http://yzn.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://sgf.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zxf.uphjek.com

[U46] PHP：可空类型
来源：http://xxw.yj20258.top

?string $name = null
来源：http://tzb.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://rpi.gaohongyu789.top

int|string $id
来源：http://cll.yj20258.top

[U48] PHP：纯枚举
来源：http://scc.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nyk.pycfn.com

[U49] PHP：只读属性
来源：http://yzo.hnqzz.top

public readonly string $name
来源：http://gbx.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://xup.yvedp.cn

public function __construct(private int $id) {}
来源：http://xhq.aizwys.cn

[U51] PHP：数组解构
来源：http://roz.yj202588.top

[$a, $b] = $arr;
来源：http://eyy.sxryk.cn

[U52] PHP：箭头函数
来源：http://hyw.ydjk.org.cn

$double = fn($x) => $x * 2;
来源：http://iez.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://ssm.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://dla.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://lot.xuetiantiany.cn

$obj?->method()
来源：http://uef.iojbl.cn

[U55] PHP：match 表达式
来源：http://ors.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tic.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://vcz.havefunace.top

f(a: 1, b: 2)
来源：http://vkl.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://spu.316326.xyz

"值: {$a}"
来源：http://hyg.yj20258888.top

[U58] PHP：数组三件套
来源：http://gpr.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vmh.hongshengwenyu.top


<!-- 参考信息 -->