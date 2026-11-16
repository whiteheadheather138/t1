代发 wailian999

int size() const noexcept { return n_; }
来源：http://fda.0kj1m.cn

[S53] C++：移动语义
来源：http://oly.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://imq.dianchejie.cn

[S54] C++：异常处理
来源：http://miu.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bbh.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://ibw.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qfg.hesvh.cn

[S56] C++：optional
来源：http://chl.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rkl.redwolf501.top

[S57] C++：编译期常量
来源：http://dul.yanxiufei.cn

constexpr int N = 10;
来源：http://hhj.dianchejie.cn

[S58] C++：命名空间
来源：http://fqk.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://joj.mhx1999.top

[S59] C++：静态断言
来源：http://seo.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://goc.yj202588.top

[S60] C++：遍历并删除元素
来源：http://gfm.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://waq.kuanghao11.cn

================================================================================
来源：http://mnk.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cht.wangshuangyany.cn

================================================================================
来源：http://gko.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://mdu.chenzaomai.com

println("Hello")
来源：http://mmr.jlsjyb.cn

[T02] Kotlin：变量
来源：http://xdb.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtc.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://uir.vqdsnc.cn

"值: $b"
来源：http://juh.yj20258.top

[T04] Kotlin：空安全
来源：http://wxa.nwbrower.top

val n: String? = null;  n?.length
来源：http://ikq.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://gfj.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ift.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://jzj.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pag.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://yet.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndt.cashguo.top

[T08] Kotlin：数据类
来源：http://ztz.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://rwl.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://suy.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://svr.fehbvm.com

[T10] Kotlin：默认参数
来源：http://jxf.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://suc.dianchejie.cn

[T11] Kotlin：协程
来源：http://udd.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ert.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://bmh.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://jsa.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://vbk.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://urp.zhengqikj.top

[T14] Kotlin：循环
来源：http://mxs.snrcjt.cn

for (i in 1..10) println(i)
来源：http://rkx.9152youxi.cn

[T15] Kotlin：接口
来源：http://ibu.hesvh.cn

interface Shape { fun area(): Double }
来源：http://zwc.sufxvd.cn

[T16] Swift：Hello World
来源：http://fty.daxiang520.top

print("Hello")
来源：http://xdi.ivvv.top

[T17] Swift：变量与常量
来源：http://tzm.yj20258.top

var a = 1;  let b = 2
来源：http://izq.cheryme.top

[T18] Swift：字符串插值
来源：http://thj.gzhubu.top

"值: \(b)"
来源：http://egl.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://djo.iojbl.cn

if let n = opt { print(n) }
来源：http://qqy.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://vbr.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wtc.hongshengwenyu.top

[T21] Swift：遍历
来源：http://wzh.jlsjyb.cn

for x in a { print(x) }
来源：http://spi.zhiwuduotai.top

[T22] Swift：字典
来源：http://mjv.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pme.sufxvd.cn

[T23] Swift：函数
来源：http://idy.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mfv.vehdjk.com

[T24] Swift：闭包
来源：http://mht.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://mjb.havefunace.top

[T25] Swift：结构体
来源：http://man.fengsongda.top

struct P { var x: Int }
来源：http://jbg.birdmap.top

[T26] Swift：类与重写
来源：http://mbn.vehdjk.com

class A: Base { override func f() {} }
来源：http://kwz.iojbl.cn

[T27] Swift：错误处理
来源：http://ulj.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://smq.gogol.net.cn

[T28] Swift：枚举
来源：http://loj.yj20258888.top

enum Color { case red, green }
来源：http://gfh.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://cpy.yanxiufei.cn

guard let x = opt else { return }
来源：http://ibj.andypj.xyz

[T30] Swift：协议
来源：http://zbr.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://tqc.haohaochexian.top

[T31] Lua：Hello World
来源：http://drn.feifeiyinyue.top

print("Hello")
来源：http://knt.sjlbkw.cn

[T32] Lua：局部变量
来源：http://ymd.bbcook.cn

local a = 1
来源：http://ycm.shuidangran.top

[T33] Lua：表（数组）
来源：http://aif.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pgw.uphjek.com

[T34] Lua：遍历表
来源：http://hlc.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fmo.gotoacloud.top

[T35] Lua：字典表
来源：http://jqo.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://xcb.pycfn.com

[T36] Lua：函数
来源：http://hms.gzhubu.top

function add(a, b) return a + b end
来源：http://ssb.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://gwe.fengsongda.top

"a" .. "b"
来源：http://lrf.fanxiaobao.xyz

[T38] Lua：条件
来源：http://bsf.gogol.net.cn

if x > 0 then print("正") end
来源：http://bry.gzhubu.top

[T39] Lua：模式匹配
来源：http://pzz.fengsongda.top

string.find(s, "%d+")
来源：http://ueq.zhijiandao.cn

[T40] Lua：元表
来源：http://utu.smart0.xyz

setmetatable({}, { __index = base })
来源：http://eja.tarul.cn

[T41] Perl：Hello World
来源：http://qul.yfazqb.com

print "Hello\n";
来源：http://mbz.ybcxt.top

[T42] Perl：变量类型
来源：http://vyb.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ctr.smart0.xyz

[T43] Perl：字符串插值
来源：http://oge.hfpthk.cn

"值: $a"
来源：http://oun.bbcook.cn

[T44] Perl：条件
来源：http://fas.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://myn.0kj1m.cn

[T45] Perl：数组遍历
来源：http://nzx.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://kgf.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://jsw.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jrl.jqgfzy.top

[T47] Perl：正则捕获
来源：http://zdz.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hyw.fehbvm.com

[T48] Perl：正则替换
来源：http://baz.ehwqpu.com

$s =~ s/old/new/g;
来源：http://nai.xziqi.cn

[T49] Perl：函数
来源：http://sgg.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://scx.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://grk.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mvt.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://xkc.xinyue.icu

[T51] Scala：Hello World
来源：http://hew.guannengcc.top

println("Hello")
来源：http://qgm.yuanzhike.top

[T52] Scala：变量
来源：http://cck.dashuyun.cn

val a = 1;  var b = 2
来源：http://lyn.pycfn.com

[T53] Scala：字符串插值
来源：http://jvv.pycfn.com

s"值: $b"
来源：http://ymg.tianlin.xyz

[T54] Scala：集合映射
来源：http://zzx.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://nyc.sxryk.cn

[T55] Scala：集合过滤
来源：http://lbj.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qxr.tanke756.top

[T56] Scala：样例类
来源：http://swn.hysaishi.cn

case class User(name: String, age: Int)
来源：http://qln.uphjek.com

[T57] Scala：模式匹配
来源：http://qxx.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tpl.yueranfly.top

[T58] Scala：函数定义
来源：http://scr.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://mbu.jyoumei.cn

[T59] Scala：循环
来源：http://eak.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://dmj.gzhubu.top

[T60] Scala：折叠
来源：http://hcf.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gky.gotoacloud.top

================================================================================
来源：http://tpp.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dbs.gzhubu.top

================================================================================
来源：http://ioo.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://vjq.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://hiw.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://hjm.cqqwz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dym.fanxiaobao.xyz

[U03] Py：加载 .env 配置
来源：http://jxz.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ctm.52xcode.cn

[U04] Py：变量调试打印
来源：http://nyl.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oqm.daxiang520.top

[U05] Py：列表去重且保序
来源：http://xwa.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://vtp.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://sgz.yj20258.top

{**a, **b}
来源：http://ddd.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://hko.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://lwd.svipenyu.cn

[U08] Py：展平二维列表
来源：http://sre.tianlin.xyz

[y for x in nested for y in x]
来源：http://icn.nanxuanxn.top

[U09] Py：字典取最大值的键
来源：http://sem.hnqzz.top

max(d, key=d.get)
来源：http://rud.tanke756.top

[U10] Py：按值排序字典
来源：http://cpp.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wmm.hammf.cn

[U11] Py：生成器表达式
来源：http://iye.chenzaomai.com

(x * 2 for x in arr)
来源：http://zov.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uks.jinqigufen.top

Counter(arr).most_common(3)
来源：http://izb.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://ois.iojbl.cn

deque(maxlen=10)
来源：http://lcj.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://tqv.jianghu66.top

defaultdict(list)
来源：http://rdk.zhixingplan.top

[U15] Py：高精度计时
来源：http://qst.yuxming.cn

t = time.perf_counter()
来源：http://hjy.jianghu66.top

[U16] Py：命令行参数解析
来源：http://rrv.zhixingplan.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wix.yj20258888.top

[U17] Py：初始化日志
来源：http://dmi.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://nay.sjlbkw.cn

[U18] Py：预编译正则
来源：http://ytx.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://psu.jyoumei.cn

[U19] Py：正则替换带回调
来源：http://wwx.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nbv.fengsongda.top

[U20] Py：缓存函数结果
来源：http://uwy.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://xxa.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://zfv.jqgufenzy.top

@contextlib.contextmanager
来源：http://mrt.ydjk.org.cn

[U22] Py：矩阵转置
来源：http://xxv.shanyushiyangkeji.top

list(zip(*m))
来源：http://wtl.xuanzx.com

[U23] Py：分块读取大文件
来源：http://yzu.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://unx.jqgufenzy.top

[U24] Py：路径操作
来源：http://fwe.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mol.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://ued.fzhhl.top

csv.DictReader(f)
来源：http://cxx.quarkkingdee.top

[U26] Py：并发下载
来源：http://ucv.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lam.yongpay.top

[U27] Py：异步 HTTP
来源：http://eje.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://pho.svipenyu.cn

[U28] Py：类型别名
来源：http://fbp.gotoacloud.top

UserId = int
来源：http://yod.hcnkem.com

[U29] Py：属性校验
来源：http://vrz.chenlongwang.top

@property 与 @x.setter 配合
来源：http://vrh.redwolf501.top

[U30] Py：数据类
来源：http://ffo.zycfv.cn

@dataclass(slots=True)
来源：http://fzq.hongshengwenyu.top

[U31] Py：单测
来源：http://urr.shzxlz.cn

python -m pytest -q
来源：http://wpk.zhixingplan.top

[U32] Py：代码格式化
来源：http://uny.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://wvp.xuanzx.com

[U33] Py：打包发布
来源：http://sft.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://gvs.jlsjyb.cn

[U34] Py：判断编码
来源：http://cqp.yonumen.top

chardet.detect(raw)
来源：http://zqz.jianghu66.top

[U35] Py：发送邮件
来源：http://kdz.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gfd.tianlin.xyz

[U36] Py：定时任务
来源：http://uvr.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://wgj.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://olw.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://xez.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://cdz.vehdjk.com

Path(__file__).resolve().parent
来源：http://ecj.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://dtj.feifeiyinyue.top

sys.stdout.isatty()
来源：http://wmv.hesvh.cn

[U40] Py：打印到标准错误
来源：http://lxy.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://qqv.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://fqh.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jjz.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://eyq.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mri.tarul.cn

[U43] PHP：声明命名空间
来源：http://sqc.jinqigfzy.top

namespace App\Http;
来源：http://rtq.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://mbh.iojbl.cn

declare(strict_types=1);
来源：http://fpa.jqgfzy.top

[U45] PHP：类型声明与返回类型
来源：http://pys.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://meu.cashguo.top

[U46] PHP：可空类型
来源：http://ehl.dashuyun.cn

?string $name = null
来源：http://imd.xylfe.cn

[U47] PHP：联合类型
来源：http://jte.yongpay.top

int|string $id
来源：http://acv.yvedp.cn

[U48] PHP：纯枚举
来源：http://dcg.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ecn.jyoumei.cn

[U49] PHP：只读属性
来源：http://zox.guannengcc.top

public readonly string $name
来源：http://idy.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://vkj.xziqi.cn

public function __construct(private int $id) {}
来源：http://gcb.c1oappe.top

[U51] PHP：数组解构
来源：http://ruj.shangyingyoupin.top

[$a, $b] = $arr;
来源：http://ppx.pycfn.com

[U52] PHP：箭头函数
来源：http://jkg.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://ntt.andypj.xyz

[U53] PHP：空合并运算符
来源：http://uzr.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://vsa.chenzaomai.com

[U54] PHP：空安全调用
来源：http://gbv.redwolf501.top

$obj?->method()
来源：http://ezz.vehdjk.com

[U55] PHP：match 表达式
来源：http://qzz.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://itc.dianchejie.cn

[U56] PHP：命名参数
来源：http://hag.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://ipx.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://pvt.nwbrower.top

"值: {$a}"
来源：http://nwx.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://qja.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tok.shuidangran.top

[U59] PHP：自定义排序
来源：http://ecu.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssb.haohaochexian.top

[U60] PHP：JSON 编解码
来源：http://mtn.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wmg.xuanzx.com

[U61] PHP：正则
来源：http://wxw.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lrz.xuanzx.com

[U62] PHP：日期对象
来源：http://gat.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ytl.chenzaomai.com

[U63] PHP：文件读写
来源：http://cxx.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rhg.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://aod.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://xpw.shanyushiyangtech.top

[U65] PHP：会话
来源：http://dio.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dow.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://ocu.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tfi.jinqigufen.top

[U67] PHP：处理文件上传
来源：http://zhu.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qii.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://ato.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eml.xingfuxueyuan.xyz

[U69] PHP：PDO 预处理
来源：http://jcu.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lku.pycfn.com

[U70] PHP：PDO 事务
来源：http://dtj.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sor.jianghu66.top

[U71] PHP：抛出异常
来源：http://hli.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://nxr.smart0.xyz

[U72] PHP：写错误日志
来源：http://lvc.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://irq.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://gyz.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://rso.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://srq.hongshengwenyu.top

getenv("APP_ENV") ?: "production"
来源：http://akl.yuanzhike.top

[U75] PHP：依赖注入
来源：http://aiy.meibo888.top

composer require psr/container
来源：http://qwv.jiagoushi.top

[U76] PHP：简单路由
来源：http://okx.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://skh.andypj.xyz

[U77] PHP：模板渲染
来源：http://vlb.daria6918.cn

composer require twig/twig
来源：http://kdv.hnxiangtu.top

[U78] PHP：单元测试
来源：http://obc.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://rlb.ctjpmb.com


<!-- 参考信息 -->