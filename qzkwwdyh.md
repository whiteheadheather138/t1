代发 wailian999

int size() const noexcept { return n_; }
来源：http://pst.guannengcc.top

[S53] C++：移动语义
来源：http://zzs.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://hmq.birdmap.top

[S54] C++：异常处理
来源：http://ata.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mlc.yuxming.cn

[S55] C++：结构化绑定
来源：http://uyb.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mia.shangyingyoupin.top

[S56] C++：optional
来源：http://phx.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hro.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://qat.yueranfly.top

constexpr int N = 10;
来源：http://pne.xziqi.cn

[S58] C++：命名空间
来源：http://grn.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://rly.52xcode.cn

[S59] C++：静态断言
来源：http://jdv.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eqy.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://bpj.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://epb.jinyuanbaomall.cn

================================================================================
来源：http://gng.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://exk.ywan-chungtsiang.top

================================================================================
来源：http://egk.ivvv.top

[T01] Kotlin：Hello World
来源：http://ned.tianlin.xyz

println("Hello")
来源：http://ydo.zhixingplan.top

[T02] Kotlin：变量
来源：http://abj.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ieg.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://nng.shangyingyoupin.top

"值: $b"
来源：http://ntm.jiagoushi.top

[T04] Kotlin：空安全
来源：http://pas.jiagoushi.top

val n: String? = null;  n?.length
来源：http://vkq.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://czt.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fzv.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://ntz.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qvr.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://xzh.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qru.chenlongwang.top

[T08] Kotlin：数据类
来源：http://tsj.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://xrg.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://mnt.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://zcv.mhx1999.top

[T10] Kotlin：默认参数
来源：http://bmj.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tjk.yueranfly.top

[T11] Kotlin：协程
来源：http://bcw.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iuo.epnwcf.com

[T12] Kotlin：解构声明
来源：http://jng.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://cnq.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://cnp.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://hac.ivvv.top

[T14] Kotlin：循环
来源：http://nbl.zhengqikj.top

for (i in 1..10) println(i)
来源：http://mop.fehbvm.com

[T15] Kotlin：接口
来源：http://htz.ybcxt.top

interface Shape { fun area(): Double }
来源：http://skn.havefunace.top

[T16] Swift：Hello World
来源：http://rbx.tianlin.xyz

print("Hello")
来源：http://vsb.gotoacloud.top

[T17] Swift：变量与常量
来源：http://jnx.gaohongyu789.top

var a = 1;  let b = 2
来源：http://aqw.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://klf.gzhubu.top

"值: \(b)"
来源：http://nsb.yangfankeji.com

[T19] Swift：可选绑定
来源：http://qiw.zhoulong.xyz

if let n = opt { print(n) }
来源：http://ptv.dianchejie.cn

[T20] Swift：数组操作
来源：http://nop.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jnq.havefunace.top

[T21] Swift：遍历
来源：http://ecg.quarkkingdee.top

for x in a { print(x) }
来源：http://vnv.snrcjt.cn

[T22] Swift：字典
来源：http://xuy.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://obx.yvedp.cn

[T23] Swift：函数
来源：http://buz.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eyq.hesvh.cn

[T24] Swift：闭包
来源：http://beb.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://waz.hywenlv.cn

[T25] Swift：结构体
来源：http://anm.cashguo.top

struct P { var x: Int }
来源：http://ilu.yfazqb.com

[T26] Swift：类与重写
来源：http://wlf.uphjek.com

class A: Base { override func f() {} }
来源：http://vzn.bjfxy.top

[T27] Swift：错误处理
来源：http://abz.xziqi.cn

do { try f() } catch { print(error) }
来源：http://xsp.tarul.cn

[T28] Swift：枚举
来源：http://xor.fktsv.cn

enum Color { case red, green }
来源：http://asw.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://gaf.ivvv.top

guard let x = opt else { return }
来源：http://gne.daria6918.cn

[T30] Swift：协议
来源：http://qrz.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://mtj.jiagoushi.top

[T31] Lua：Hello World
来源：http://qba.yj20258.top

print("Hello")
来源：http://xoi.bjfxy.top

[T32] Lua：局部变量
来源：http://rfm.quarkkingdee.top

local a = 1
来源：http://uzk.ybcxt.top

[T33] Lua：表（数组）
来源：http://wyq.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qpv.hywenlv.cn

[T34] Lua：遍历表
来源：http://wtq.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dnk.chenjidiqi.icu

[T35] Lua：字典表
来源：http://teo.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://xcn.shuidangran.top

[T36] Lua：函数
来源：http://cep.yangfankeji.com

function add(a, b) return a + b end
来源：http://oek.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://eeq.jyoumei.cn

"a" .. "b"
来源：http://vzv.cucudq.cn

[T38] Lua：条件
来源：http://sjs.chenzaomai.com

if x > 0 then print("正") end
来源：http://tsf.wangdashe.top

[T39] Lua：模式匹配
来源：http://aca.dianchejie.cn

string.find(s, "%d+")
来源：http://ssi.shzxlz.cn

[T40] Lua：元表
来源：http://spk.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://pav.cdnleiting.top

[T41] Perl：Hello World
来源：http://kqw.jyoumei.cn

print "Hello\n";
来源：http://ino.gaohongyu789.top

[T42] Perl：变量类型
来源：http://eok.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ttq.zdbjq.cn

[T43] Perl：字符串插值
来源：http://ofn.zycfv.cn

"值: $a"
来源：http://uix.pycfn.com

[T44] Perl：条件
来源：http://dgt.xinyue.icu

if ($a > 0) { print "正"; }
来源：http://taw.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://nuy.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://iaw.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://nit.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xhh.fktsv.cn

[T47] Perl：正则捕获
来源：http://xmb.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wmp.ybcxt.top

[T48] Perl：正则替换
来源：http://gel.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://vmz.aibaodan.cn

[T49] Perl：函数
来源：http://sfn.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xfw.zhiwuduotai.top

[T50] Perl：逐行读文件
来源：http://jex.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yau.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://pth.hysaishi.cn

[T51] Scala：Hello World
来源：http://kvl.ctjpmb.com

println("Hello")
来源：http://sxa.dashuyun.cn

[T52] Scala：变量
来源：http://jww.yueranfly.top

val a = 1;  var b = 2
来源：http://zsn.guannengcc.top

[T53] Scala：字符串插值
来源：http://mfa.gotoacloud.top

s"值: $b"
来源：http://tcd.fktsv.cn

[T54] Scala：集合映射
来源：http://dwn.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://kkp.dianchejie.cn

[T55] Scala：集合过滤
来源：http://djq.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://rlm.jinqigfzy.top

[T56] Scala：样例类
来源：http://wtw.yvedp.cn

case class User(name: String, age: Int)
来源：http://bgw.yfazqb.com

[T57] Scala：模式匹配
来源：http://xql.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gtk.sxryk.cn

[T58] Scala：函数定义
来源：http://izq.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://ajf.yj202588.top

[T59] Scala：循环
来源：http://tah.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://usd.52xcode.cn

[T60] Scala：折叠
来源：http://bpy.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dle.cqqwz.cn

================================================================================
来源：http://fzk.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://udf.kuanghao11.cn

================================================================================
来源：http://ruw.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://bap.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://lkj.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://gys.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vvf.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://vqa.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ath.nanxinkj.top

[U04] Py：变量调试打印
来源：http://btt.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fsc.shuidangran.top

[U05] Py：列表去重且保序
来源：http://wko.xylfe.cn

list(dict.fromkeys(arr))
来源：http://bkr.nwbrower.top

[U06] Py：合并两个字典
来源：http://yxk.yuxming.cn

{**a, **b}
来源：http://wit.yfazqb.com

[U07] Py：反转字典键值
来源：http://pkb.sweek.top

{v: k for k, v in d.items()}
来源：http://hgv.fengsongda.top

[U08] Py：展平二维列表
来源：http://ika.zhixingplan.top

[y for x in nested for y in x]
来源：http://wly.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://xwt.hysaishi.cn

max(d, key=d.get)
来源：http://nhz.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://odk.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bgt.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://mty.hysaishi.cn

(x * 2 for x in arr)
来源：http://hge.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uzj.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://hhx.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://nkg.shangyingyoupin.top

deque(maxlen=10)
来源：http://wor.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://rtq.yj202588.top

defaultdict(list)
来源：http://wxi.sweek.top

[U15] Py：高精度计时
来源：http://qbq.vqdsnc.cn

t = time.perf_counter()
来源：http://sfs.ppjwa.cn

[U16] Py：命令行参数解析
来源：http://cqy.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bjd.zhongyouzk.top

[U17] Py：初始化日志
来源：http://tgi.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://hcf.quarkkingdee.top

[U18] Py：预编译正则
来源：http://mbo.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://ixb.gogol.net.cn

[U19] Py：正则替换带回调
来源：http://wtx.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mhw.xylfe.cn

[U20] Py：缓存函数结果
来源：http://wye.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://fdi.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://vju.gogol.net.cn

@contextlib.contextmanager
来源：http://lmb.daxiang520.top

[U22] Py：矩阵转置
来源：http://sdj.gaohongyu789.top

list(zip(*m))
来源：http://coi.zycfv.cn

[U23] Py：分块读取大文件
来源：http://slx.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rcg.xuetiantiany.cn

[U24] Py：路径操作
来源：http://tny.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ryo.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://zdf.dianchejie.cn

csv.DictReader(f)
来源：http://jbm.dashuyun.cn

[U26] Py：并发下载
来源：http://zbf.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ree.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://jxm.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ala.0kj1m.cn

[U28] Py：类型别名
来源：http://bxf.gotoacloud.top

UserId = int
来源：http://unj.ybcxt.top

[U29] Py：属性校验
来源：http://fik.hysaishi.cn

@property 与 @x.setter 配合
来源：http://iiy.xuetiantiany.cn

[U30] Py：数据类
来源：http://txr.ehwqpu.com

@dataclass(slots=True)
来源：http://yhg.mhx1999.top

[U31] Py：单测
来源：http://xtg.hnxiangtu.top

python -m pytest -q
来源：http://xss.ctjpmb.com

[U32] Py：代码格式化
来源：http://pbf.zdqjudy.top

ruff format . && ruff check --fix .
来源：http://pdu.vehdjk.com

[U33] Py：打包发布
来源：http://lwp.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://ntr.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://vkm.sysykeji.top

chardet.detect(raw)
来源：http://uzi.cashguo.top

[U35] Py：发送邮件
来源：http://gak.sxryk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zws.sxryk.cn

[U36] Py：定时任务
来源：http://pys.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://bps.ctjpmb.com

[U37] Py：读写 Excel
来源：http://ges.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pax.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://ffy.jyoumei.cn

Path(__file__).resolve().parent
来源：http://gsq.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://bhi.yongpay.top

sys.stdout.isatty()
来源：http://gbo.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://dxp.zhengqikj.top

print("err", file=sys.stderr)
来源：http://mnw.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://jfe.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://maj.sxryk.cn

[U42] PHP：PSR-4 自动加载
来源：http://eib.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vtq.yvedp.cn

[U43] PHP：声明命名空间
来源：http://avf.jinqigufen.top

namespace App\Http;
来源：http://ksm.bbcook.cn

[U44] PHP：开启严格类型
来源：http://hhe.aizwys.cn

declare(strict_types=1);
来源：http://mlj.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://cgj.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wbw.gogol.net.cn

[U46] PHP：可空类型
来源：http://twq.yueranfly.top

?string $name = null
来源：http://sut.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://cze.chenjidiqi.icu

int|string $id
来源：http://nlb.cheryme.top

[U48] PHP：纯枚举
来源：http://lay.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nmu.cashguo.top

[U49] PHP：只读属性
来源：http://cmt.52xcode.cn

public readonly string $name
来源：http://tji.meibo888.top

[U50] PHP：构造器属性提升
来源：http://jzj.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://yqf.sysykeji.top

[U51] PHP：数组解构
来源：http://nad.nanxinkj.top

[$a, $b] = $arr;
来源：http://wmh.shangyingyoupin.top

[U52] PHP：箭头函数
来源：http://qsr.ybcxt.top

$double = fn($x) => $x * 2;
来源：http://aqv.bbcook.cn

[U53] PHP：空合并运算符
来源：http://djs.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://ydq.jiagoushi.top

[U54] PHP：空安全调用
来源：http://bmt.hesvh.cn

$obj?->method()
来源：http://pdb.zdqjudy.top

[U55] PHP：match 表达式
来源：http://ocd.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tko.ybcxt.top

[U56] PHP：命名参数
来源：http://ppa.ehwqpu.com

f(a: 1, b: 2)
来源：http://gcr.jianghu66.top

[U57] PHP：字符串插值
来源：http://mem.hywenlv.cn

"值: {$a}"
来源：http://znr.ybcxt.top

[U58] PHP：数组三件套
来源：http://kab.sweek.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bwn.xylfe.cn

[U59] PHP：自定义排序
来源：http://gtb.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wfx.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://xqq.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://msk.xziqi.cn

[U61] PHP：正则
来源：http://nnm.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fqa.hfpthk.cn

[U62] PHP：日期对象
来源：http://lhk.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iqu.xylfe.cn

[U63] PHP：文件读写
来源：http://nlc.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fbo.yfazqb.com

[U64] PHP：目录遍历
来源：http://ukw.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://lss.fktsv.cn

[U65] PHP：会话
来源：http://nez.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ojd.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://vfn.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rhi.ctjpmb.com

[U67] PHP：处理文件上传
来源：http://gzt.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cgo.aizwys.cn

[U68] PHP：PDO 连接
来源：http://fpi.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://biy.havefunace.top

[U69] PHP：PDO 预处理
来源：http://vow.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gqg.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://wwh.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wyn.ydzc1.top

[U71] PHP：抛出异常
来源：http://per.shanyushiyangkeji.top

throw new RuntimeException("失败", 500);
来源：http://bju.xuanzx.com

[U72] PHP：写错误日志
来源：http://ulv.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://all.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://xax.yj202588.top

parse_ini_file("config.ini", true)
来源：http://fpk.tanke756.top

[U74] PHP：读取环境变量
来源：http://qzd.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://idl.yj202588.top

[U75] PHP：依赖注入
来源：http://eio.wangshuangyany.cn

composer require psr/container
来源：http://jni.gotoacloud.top

[U76] PHP：简单路由
来源：http://mbl.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fxi.nanxinkj.top

[U77] PHP：模板渲染
来源：http://pvm.pengpengdd.cyou

composer require twig/twig
来源：http://tve.tian-w.cn

[U78] PHP：单元测试
来源：http://zjg.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://pyf.hnqzz.top


<!-- 参考信息 -->