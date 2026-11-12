代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zqy.chenzaomai.com

[S51] C++：显式类型转换
来源：http://jbw.hywenlv.cn

static_cast<double>(a) / b
来源：http://imv.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://xzg.52xcode.cn

int size() const noexcept { return n_; }
来源：http://aiv.cheryme.top

[S53] C++：移动语义
来源：http://rsl.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://zei.jinqigufen.top

[S54] C++：异常处理
来源：http://nuz.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ive.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://tuo.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://loi.chenzaomai.com

[S56] C++：optional
来源：http://jqk.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mff.redwolf501.top

[S57] C++：编译期常量
来源：http://hhr.ctjpmb.com

constexpr int N = 10;
来源：http://mjd.cdnleiting.top

[S58] C++：命名空间
来源：http://cdm.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://kyv.yongpay.top

[S59] C++：静态断言
来源：http://byy.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eam.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://hln.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yqu.pycfn.com

================================================================================
来源：http://ivh.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgo.hywenlv.cn

================================================================================
来源：http://pwo.iojbl.cn

[T01] Kotlin：Hello World
来源：http://pll.hongshengwenyu.top

println("Hello")
来源：http://sik.9152youxi.cn

[T02] Kotlin：变量
来源：http://iri.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zdi.yj20258.top

[T03] Kotlin：字符串模板
来源：http://fxt.hesvh.cn

"值: $b"
来源：http://zdk.yongpay.top

[T04] Kotlin：空安全
来源：http://pnk.yuanzhike.top

val n: String? = null;  n?.length
来源：http://vil.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://wpn.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zvp.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://ows.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uyt.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://bhh.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vpx.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://nwg.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://rbj.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://wug.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://fca.bjfxy.top

[T10] Kotlin：默认参数
来源：http://xcn.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yor.zhijiandao.cn

[T11] Kotlin：协程
来源：http://spd.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://mrh.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://tsd.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://odv.hammf.cn

[T13] Kotlin：只读 Map
来源：http://ssr.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://dux.andypj.xyz

[T14] Kotlin：循环
来源：http://fdl.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://xpn.52xcode.cn

[T15] Kotlin：接口
来源：http://usv.yj20258.top

interface Shape { fun area(): Double }
来源：http://wpb.havefunace.top

[T16] Swift：Hello World
来源：http://fim.shzxlz.cn

print("Hello")
来源：http://kex.chenzaomai.com

[T17] Swift：变量与常量
来源：http://xox.yongpay.top

var a = 1;  let b = 2
来源：http://chz.jqgfzy.top

[T18] Swift：字符串插值
来源：http://apg.yfazqb.com

"值: \(b)"
来源：http://vee.andypj.xyz

[T19] Swift：可选绑定
来源：http://ffi.shuidangran.top

if let n = opt { print(n) }
来源：http://mni.vehdjk.com

[T20] Swift：数组操作
来源：http://lfs.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://jfn.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://mqv.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://kyq.hammf.cn

[T22] Swift：字典
来源：http://nmv.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sas.chenlongwang.top

[T23] Swift：函数
来源：http://nuk.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mwu.ehwqpu.com

[T24] Swift：闭包
来源：http://oic.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lcp.yanxiufei.cn

[T25] Swift：结构体
来源：http://qtd.tian-w.cn

struct P { var x: Int }
来源：http://znf.c1oappe.top

[T26] Swift：类与重写
来源：http://anp.chenlongwang.top

class A: Base { override func f() {} }
来源：http://kcg.cashguo.top

[T27] Swift：错误处理
来源：http://zdw.pycfn.com

do { try f() } catch { print(error) }
来源：http://sui.yongpay.top

[T28] Swift：枚举
来源：http://koc.meibo888.top

enum Color { case red, green }
来源：http://irq.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://oiu.aibaodan.cn

guard let x = opt else { return }
来源：http://kmn.jinghuilouyu.cn

[T30] Swift：协议
来源：http://gfw.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://wbh.aizwys.cn

[T31] Lua：Hello World
来源：http://zbw.yuxming.cn

print("Hello")
来源：http://fpy.daxiang520.top

[T32] Lua：局部变量
来源：http://vwl.jinqigufen.top

local a = 1
来源：http://twi.dianchejie.cn

[T33] Lua：表（数组）
来源：http://mnx.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lyo.zhijiandao.cn

[T34] Lua：遍历表
来源：http://dzw.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oly.vqdsnc.cn

[T35] Lua：字典表
来源：http://rhl.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://ggj.cheryme.top

[T36] Lua：函数
来源：http://aqg.jqgfzy.top

function add(a, b) return a + b end
来源：http://flm.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://etx.chenlongwang.top

"a" .. "b"
来源：http://raf.zhijiandao.cn

[T38] Lua：条件
来源：http://one.tian-w.cn

if x > 0 then print("正") end
来源：http://qam.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://icp.cqqwz.cn

string.find(s, "%d+")
来源：http://lod.jinqigufen.top

[T40] Lua：元表
来源：http://fsi.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://nat.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://zvs.bbcook.cn

print "Hello\n";
来源：http://ipp.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://cyx.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uoy.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://nee.jyoumei.cn

"值: $a"
来源：http://gkt.sjlbkw.cn

[T44] Perl：条件
来源：http://azh.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://vhv.zdqjudy.top

[T45] Perl：数组遍历
来源：http://jzx.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://rsi.dianchejie.cn

[T46] Perl：哈希操作
来源：http://zvh.vehdjk.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vmy.jqgfzy.top

[T47] Perl：正则捕获
来源：http://pka.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://krj.ppjwa.cn

[T48] Perl：正则替换
来源：http://hem.wangdashe.top

$s =~ s/old/new/g;
来源：http://sul.zdbjq.cn

[T49] Perl：函数
来源：http://svi.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://anv.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://nyu.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mvs.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://ore.chenlongwang.top

[T51] Scala：Hello World
来源：http://sco.fengsongda.top

println("Hello")
来源：http://msv.yongpay.top

[T52] Scala：变量
来源：http://nco.yangfankeji.com

val a = 1;  var b = 2
来源：http://zkg.cucudq.cn

[T53] Scala：字符串插值
来源：http://vns.jqgfzy.top

s"值: $b"
来源：http://bdi.fengsongda.top

[T54] Scala：集合映射
来源：http://prv.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://qef.hfpthk.cn

[T55] Scala：集合过滤
来源：http://fdu.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://aab.hnqzz.top

[T56] Scala：样例类
来源：http://ylk.svipenyu.cn

case class User(name: String, age: Int)
来源：http://jac.cucudq.cn

[T57] Scala：模式匹配
来源：http://jmu.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://eml.jyoumei.cn

[T58] Scala：函数定义
来源：http://tsj.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://onp.fehbvm.com

[T59] Scala：循环
来源：http://cho.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://xao.9152youxi.cn

[T60] Scala：折叠
来源：http://bnr.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://usr.fengsongda.top

================================================================================
来源：http://znh.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xjd.vehdjk.com

================================================================================
来源：http://uqn.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://xmr.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://uct.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://mpx.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://not.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://sih.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hfj.gotoacloud.top

[U04] Py：变量调试打印
来源：http://mfn.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gkb.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://lxz.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://ere.nwbrower.top

[U06] Py：合并两个字典
来源：http://fqo.smart0.xyz

{**a, **b}
来源：http://lpc.hnqzz.top

[U07] Py：反转字典键值
来源：http://bcw.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://owa.redwolf501.top

[U08] Py：展平二维列表
来源：http://nqp.vqdsnc.cn

[y for x in nested for y in x]
来源：http://dpl.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://suq.hysaishi.cn

max(d, key=d.get)
来源：http://pua.guannengcc.top

[U10] Py：按值排序字典
来源：http://ejw.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ajx.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://abc.nanxinkj.top

(x * 2 for x in arr)
来源：http://mal.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sgw.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://tfs.yuxming.cn

[U13] Py：固定长度队列
来源：http://new.epnwcf.com

deque(maxlen=10)
来源：http://ljc.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://hjq.fengsongda.top

defaultdict(list)
来源：http://vvp.xziqi.cn

[U15] Py：高精度计时
来源：http://aor.hammf.cn

t = time.perf_counter()
来源：http://xgd.yj202588.top

[U16] Py：命令行参数解析
来源：http://sqh.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wyd.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://nko.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://ykz.shuidangran.top

[U18] Py：预编译正则
来源：http://wwc.guannengcc.top

pat = re.compile(r"\d+")
来源：http://lub.yj202588.top

[U19] Py：正则替换带回调
来源：http://kcp.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://off.yj20258.top

[U20] Py：缓存函数结果
来源：http://nvu.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://jet.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://unm.xylfe.cn

@contextlib.contextmanager
来源：http://lbr.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://idv.xingfuxueyuan.xyz

list(zip(*m))
来源：http://yzj.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://myb.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ezm.cheryme.top

[U24] Py：路径操作
来源：http://mtp.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ctz.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://jdr.birdmap.top

csv.DictReader(f)
来源：http://huk.snrcjt.cn

[U26] Py：并发下载
来源：http://xdy.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lpm.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://xrr.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://yfd.jianghu66.top

[U28] Py：类型别名
来源：http://fqk.vehdjk.com

UserId = int
来源：http://vum.vehdjk.com

[U29] Py：属性校验
来源：http://wmi.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://utb.jinghuilouyu.cn

[U30] Py：数据类
来源：http://ayv.aibaodan.cn

@dataclass(slots=True)
来源：http://bnh.yj20258.top

[U31] Py：单测
来源：http://vii.cucudq.cn

python -m pytest -q
来源：http://wpy.fktsv.cn

[U32] Py：代码格式化
来源：http://wfx.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://lga.hnqzz.top

[U33] Py：打包发布
来源：http://sxr.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://lqm.jiagoushi.top

[U34] Py：判断编码
来源：http://vqa.zycfv.cn

chardet.detect(raw)
来源：http://ugc.zdqjudy.top

[U35] Py：发送邮件
来源：http://arz.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nkb.jyoumei.cn

[U36] Py：定时任务
来源：http://six.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://dst.52xcode.cn

[U37] Py：读写 Excel
来源：http://vpq.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://fwd.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://zsn.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://xls.fktsv.cn

[U39] Py：判断是否在交互环境
来源：http://olw.c1oappe.top

sys.stdout.isatty()
来源：http://cok.hnqzz.top

[U40] Py：打印到标准错误
来源：http://bie.yuanzhike.top

print("err", file=sys.stderr)
来源：http://nzf.birdmap.top

[U41] PHP：初始化 Composer 项目
来源：http://upd.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iyz.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://unz.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fkq.yonumen.top

[U43] PHP：声明命名空间
来源：http://ecx.hysaishi.cn

namespace App\Http;
来源：http://gfg.shuidangran.top

[U44] PHP：开启严格类型
来源：http://xfh.chenzaomai.com

declare(strict_types=1);
来源：http://zkm.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://pri.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vua.xingfuxueyuan.xyz

[U46] PHP：可空类型
来源：http://xry.fanxiaobao.xyz

?string $name = null
来源：http://iga.ivvv.top

[U47] PHP：联合类型
来源：http://psl.ehwqpu.com

int|string $id
来源：http://ujx.hnqzz.top

[U48] PHP：纯枚举
来源：http://aht.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bmk.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://wrd.hnxiangtu.top

public readonly string $name
来源：http://cek.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://oxi.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://zgf.zhijiandao.cn

[U51] PHP：数组解构
来源：http://ogp.zhijiandao.cn

[$a, $b] = $arr;
来源：http://xjn.cucudq.cn

[U52] PHP：箭头函数
来源：http://afd.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://bml.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://xoe.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://zmg.sjlbkw.cn

[U54] PHP：空安全调用
来源：http://vjq.chenlongwang.top

$obj?->method()
来源：http://ajf.hysaishi.cn

[U55] PHP：match 表达式
来源：http://cta.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jfh.hnxiangtu.top

[U56] PHP：命名参数
来源：http://thz.gaohongyu789.top

f(a: 1, b: 2)
来源：http://yxg.hnqzz.top

[U57] PHP：字符串插值
来源：http://jer.havefunace.top

"值: {$a}"
来源：http://nqp.gzhubu.top

[U58] PHP：数组三件套
来源：http://uhy.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ymc.aizwys.cn

[U59] PHP：自定义排序
来源：http://flc.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gnx.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://wja.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ylr.zdbjq.cn

[U61] PHP：正则
来源：http://vuv.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gft.zhixingplan.top

[U62] PHP：日期对象
来源：http://oqn.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bun.bbcook.cn

[U63] PHP：文件读写
来源：http://tkd.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ncd.ctjpmb.com

[U64] PHP：目录遍历
来源：http://fsr.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://nob.gotoacloud.top

[U65] PHP：会话
来源：http://mfj.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://nbp.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://apt.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vlw.yuxming.cn

[U67] PHP：处理文件上传
来源：http://ntp.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nqx.yonumen.top

[U68] PHP：PDO 连接
来源：http://bra.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bnj.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://vel.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yil.yonumen.top

[U70] PHP：PDO 事务
来源：http://eai.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xwr.nwbrower.top

[U71] PHP：抛出异常
来源：http://cvf.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://dcj.dashuyun.cn

[U72] PHP：写错误日志
来源：http://swa.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ccb.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://mqt.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://val.daxiang520.top

[U74] PHP：读取环境变量
来源：http://ess.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://kep.ppjwa.cn

[U75] PHP：依赖注入
来源：http://rpn.ybcxt.top

composer require psr/container
来源：http://hdy.chenzaomai.com

[U76] PHP：简单路由
来源：http://lqt.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sms.yvedp.cn


<!-- 参考信息 -->