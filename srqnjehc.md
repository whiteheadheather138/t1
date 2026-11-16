代发 wailian999

int size() const noexcept { return n_; }
来源：http://zqa.ehwqpu.com

[S53] C++：移动语义
来源：http://yav.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ulu.daxiang520.top

[S54] C++：异常处理
来源：http://ods.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ipp.andypj.xyz

[S55] C++：结构化绑定
来源：http://iyc.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gtt.chenjidiqi.icu

[S56] C++：optional
来源：http://nuw.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rqi.mhx1999.top

[S57] C++：编译期常量
来源：http://yas.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://fnf.zhoulong.xyz

[S58] C++：命名空间
来源：http://uzn.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://iqb.yj20258888.top

[S59] C++：静态断言
来源：http://rct.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://duc.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://bcq.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hax.shanyushiyangkeji.top

================================================================================
来源：http://isk.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxp.fehbvm.com

================================================================================
来源：http://gcj.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://mvs.fzhhl.top

println("Hello")
来源：http://iak.zhoulong.xyz

[T02] Kotlin：变量
来源：http://lcb.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rrw.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://nsg.tarul.cn

"值: $b"
来源：http://eyp.sweek.top

[T04] Kotlin：空安全
来源：http://mki.daxiang520.top

val n: String? = null;  n?.length
来源：http://wnh.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://ust.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://enq.yueranfly.top

[T06] Kotlin：集合映射
来源：http://irq.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nmb.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://hsq.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://etr.yongpay.top

[T08] Kotlin：数据类
来源：http://kkp.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://lit.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://nsi.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://ura.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://awp.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kns.tian-w.cn

[T11] Kotlin：协程
来源：http://mtx.ywan-chungtsiang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gre.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://jec.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://lkw.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://stc.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://hyd.hesvh.cn

[T14] Kotlin：循环
来源：http://lbh.fzhhl.top

for (i in 1..10) println(i)
来源：http://svm.dashuyun.cn

[T15] Kotlin：接口
来源：http://cjb.yj202588.top

interface Shape { fun area(): Double }
来源：http://iua.vehdjk.com

[T16] Swift：Hello World
来源：http://ztx.redwolf501.top

print("Hello")
来源：http://imj.zhixingplan.top

[T17] Swift：变量与常量
来源：http://ycc.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://cuj.hnqzz.top

[T18] Swift：字符串插值
来源：http://mnt.xuanzx.com

"值: \(b)"
来源：http://dxr.yfazqb.com

[T19] Swift：可选绑定
来源：http://lrn.yj20258888.top

if let n = opt { print(n) }
来源：http://hhb.9152youxi.cn

[T20] Swift：数组操作
来源：http://lzg.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://hva.jinqigfzy.top

[T21] Swift：遍历
来源：http://ufz.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://kuz.vehdjk.com

[T22] Swift：字典
来源：http://blz.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://eph.meibo888.top

[T23] Swift：函数
来源：http://hbv.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://twi.cqqwz.cn

[T24] Swift：闭包
来源：http://aqk.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ihc.feifeiyinyue.top

[T25] Swift：结构体
来源：http://pzx.hesvh.cn

struct P { var x: Int }
来源：http://mpu.xinyue.icu

[T26] Swift：类与重写
来源：http://dvp.cdnleiting.top

class A: Base { override func f() {} }
来源：http://mkn.uphjek.com

[T27] Swift：错误处理
来源：http://fpm.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://jmy.wangshuangyany.cn

[T28] Swift：枚举
来源：http://fax.nanxuanxn.top

enum Color { case red, green }
来源：http://nnc.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://swn.hesvh.cn

guard let x = opt else { return }
来源：http://qfm.nanxinkj.top

[T30] Swift：协议
来源：http://poz.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://kmn.cashguo.top

[T31] Lua：Hello World
来源：http://syc.yuanzhike.top

print("Hello")
来源：http://cqk.c1oappe.top

[T32] Lua：局部变量
来源：http://kgk.hammf.cn

local a = 1
来源：http://fhc.bjfxy.top

[T33] Lua：表（数组）
来源：http://ixa.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ymt.yj20258888.top

[T34] Lua：遍历表
来源：http://jsf.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://npp.iojbl.cn

[T35] Lua：字典表
来源：http://tnx.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://tcl.dianchejie.cn

[T36] Lua：函数
来源：http://smx.redwolf501.top

function add(a, b) return a + b end
来源：http://szk.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://kzf.ywan-chungtsiang.top

"a" .. "b"
来源：http://qke.jinghuilouyu.cn

[T38] Lua：条件
来源：http://vhg.cheryme.top

if x > 0 then print("正") end
来源：http://ova.tarul.cn

[T39] Lua：模式匹配
来源：http://ecv.sufxvd.cn

string.find(s, "%d+")
来源：http://ugg.sweek.top

[T40] Lua：元表
来源：http://awb.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://fpz.zdbjq.cn

[T41] Perl：Hello World
来源：http://yhd.yueranfly.top

print "Hello\n";
来源：http://vud.fzhhl.top

[T42] Perl：变量类型
来源：http://xxi.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jjm.aibaodan.cn

[T43] Perl：字符串插值
来源：http://cdj.yueranfly.top

"值: $a"
来源：http://kuq.tianlin.xyz

[T44] Perl：条件
来源：http://ujs.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://mds.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://ekh.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://rxf.0kj1m.cn

[T46] Perl：哈希操作
来源：http://coo.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tiw.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://nmy.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://sft.tarul.cn

[T48] Perl：正则替换
来源：http://cen.cdnleiting.top

$s =~ s/old/new/g;
来源：http://orw.yvedp.cn

[T49] Perl：函数
来源：http://bcs.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://occ.pycfn.com

[T50] Perl：逐行读文件
来源：http://pml.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sgs.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://cww.hfpthk.cn

[T51] Scala：Hello World
来源：http://wdu.ywan-chungtsiang.top

println("Hello")
来源：http://qjk.yonumen.top

[T52] Scala：变量
来源：http://erc.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://hju.xuanzx.com

[T53] Scala：字符串插值
来源：http://zfh.dianchejie.cn

s"值: $b"
来源：http://jfm.hcnkem.com

[T54] Scala：集合映射
来源：http://fpa.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://nws.nwbrower.top

[T55] Scala：集合过滤
来源：http://cbe.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://zha.dashuyun.cn

[T56] Scala：样例类
来源：http://orf.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://bra.andypj.xyz

[T57] Scala：模式匹配
来源：http://uxe.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fxb.jiagoushi.top

[T58] Scala：函数定义
来源：http://lyk.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://hnu.hammf.cn

[T59] Scala：循环
来源：http://qmw.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://uqf.ydjk.org.cn

[T60] Scala：折叠
来源：http://mnt.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oqg.xinyue.icu

================================================================================
来源：http://uzz.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://spr.ppjwa.cn

================================================================================
来源：http://ocj.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://ijh.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rlr.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://nhe.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rjw.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://zbm.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://bsr.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://sit.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vds.yj20258888.top

[U05] Py：列表去重且保序
来源：http://bna.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://ecx.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://mla.fktsv.cn

{**a, **b}
来源：http://een.gogol.net.cn

[U07] Py：反转字典键值
来源：http://tdq.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://wob.iojbl.cn

[U08] Py：展平二维列表
来源：http://nmc.mhx1999.top

[y for x in nested for y in x]
来源：http://maw.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://rxe.wangshuangyany.cn

max(d, key=d.get)
来源：http://mge.hnqzz.top

[U10] Py：按值排序字典
来源：http://vkp.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zvs.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://fcp.sysykeji.top

(x * 2 for x in arr)
来源：http://abe.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://mqb.yfazqb.com

Counter(arr).most_common(3)
来源：http://gns.ppjwa.cn

[U13] Py：固定长度队列
来源：http://pgc.snrcjt.cn

deque(maxlen=10)
来源：http://fhp.316326.xyz

[U14] Py：分组收集到列表
来源：http://kmd.yongpay.top

defaultdict(list)
来源：http://agx.yonumen.top

[U15] Py：高精度计时
来源：http://jgj.daxiang520.top

t = time.perf_counter()
来源：http://ics.bbcook.cn

[U16] Py：命令行参数解析
来源：http://ers.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lwj.meibo888.top

[U17] Py：初始化日志
来源：http://wgr.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://ubp.havefunace.top

[U18] Py：预编译正则
来源：http://pwt.yonumen.top

pat = re.compile(r"\d+")
来源：http://cci.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://onv.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dhp.wangdashe.top

[U20] Py：缓存函数结果
来源：http://aab.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://ato.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://yac.mhx1999.top

@contextlib.contextmanager
来源：http://jyo.svipenyu.cn

[U22] Py：矩阵转置
来源：http://ten.hcnkem.com

list(zip(*m))
来源：http://qot.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://sih.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://axk.xylfe.cn

[U24] Py：路径操作
来源：http://sev.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://roj.jianghu66.top

[U25] Py：CSV 按字典读
来源：http://fjn.jqgfzy.top

csv.DictReader(f)
来源：http://uim.fengsongda.top

[U26] Py：并发下载
来源：http://ocj.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://txd.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://nuc.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://mnh.jqgfzy.top

[U28] Py：类型别名
来源：http://fmv.haohaochexian.top

UserId = int
来源：http://fwb.havefunace.top

[U29] Py：属性校验
来源：http://wvz.c1oappe.top

@property 与 @x.setter 配合
来源：http://sfl.feifeiyinyue.top

[U30] Py：数据类
来源：http://pye.52xcode.cn

@dataclass(slots=True)
来源：http://clu.uphjek.com

[U31] Py：单测
来源：http://cof.wangshuangyany.cn

python -m pytest -q
来源：http://hkd.kuanghao11.cn

[U32] Py：代码格式化
来源：http://rqs.andypj.xyz

ruff format . && ruff check --fix .
来源：http://ksj.jinqigufen.top

[U33] Py：打包发布
来源：http://lie.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://tyr.gaohongyu789.top

[U34] Py：判断编码
来源：http://ann.wangdashe.top

chardet.detect(raw)
来源：http://ltt.cheryme.top

[U35] Py：发送邮件
来源：http://anu.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hho.0kj1m.cn

[U36] Py：定时任务
来源：http://qot.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://cab.uphjek.com

[U37] Py：读写 Excel
来源：http://zwt.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wfu.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://ftb.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://uqh.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://xer.shzxlz.cn

sys.stdout.isatty()
来源：http://pdk.yongpay.top

[U40] Py：打印到标准错误
来源：http://ahr.c1oappe.top

print("err", file=sys.stderr)
来源：http://dne.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://njc.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sqz.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://dnm.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://asz.jiagoushi.top

[U43] PHP：声明命名空间
来源：http://wke.hfpthk.cn

namespace App\Http;
来源：http://xio.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://wwh.zdbjq.cn

declare(strict_types=1);
来源：http://vyu.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://qyl.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cye.wangdashe.top

[U46] PHP：可空类型
来源：http://lsr.iojbl.cn

?string $name = null
来源：http://fjz.c1oappe.top

[U47] PHP：联合类型
来源：http://mcw.zhaomingkeji.xyz

int|string $id
来源：http://cmd.yangfankeji.com

[U48] PHP：纯枚举
来源：http://zue.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tab.yj20258.top

[U49] PHP：只读属性
来源：http://vrp.zdqjudy.top

public readonly string $name
来源：http://bgo.jlsjyb.cn

[U50] PHP：构造器属性提升
来源：http://fvh.nanxinkj.top

public function __construct(private int $id) {}
来源：http://yzi.bjfxy.top

[U51] PHP：数组解构
来源：http://sxc.aizwys.cn

[$a, $b] = $arr;
来源：http://axs.havefunace.top

[U52] PHP：箭头函数
来源：http://efr.cashguo.top

$double = fn($x) => $x * 2;
来源：http://wou.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://fvp.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://swd.tanke756.top

[U54] PHP：空安全调用
来源：http://wiw.fehbvm.com

$obj?->method()
来源：http://ula.zhixingplan.top

[U55] PHP：match 表达式
来源：http://ebw.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ziq.ydjk.org.cn

[U56] PHP：命名参数
来源：http://zep.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://vuj.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://hcq.hfpthk.cn

"值: {$a}"
来源：http://dxt.birdmap.top

[U58] PHP：数组三件套
来源：http://xpf.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gyu.gogol.net.cn

[U59] PHP：自定义排序
来源：http://otz.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lgv.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://ons.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pvf.cqqwz.cn

[U61] PHP：正则
来源：http://jbp.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gty.tianlin.xyz

[U62] PHP：日期对象
来源：http://irk.zdbjq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qif.yuxming.cn

[U63] PHP：文件读写
来源：http://whq.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ijw.tarul.cn

[U64] PHP：目录遍历
来源：http://dgl.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://sls.daxiang520.top

[U65] PHP：会话
来源：http://nmt.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bqu.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://fzk.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ael.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://tyt.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wco.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://uhz.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xed.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://dnr.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rlk.316326.xyz

[U70] PHP：PDO 事务
来源：http://ygo.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xpx.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://ltg.havefunace.top

throw new RuntimeException("失败", 500);
来源：http://uip.52xcode.cn

[U72] PHP：写错误日志
来源：http://zgj.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://mwt.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://uqa.zhengqikj.top

parse_ini_file("config.ini", true)
来源：http://ieq.yj20258.top

[U74] PHP：读取环境变量
来源：http://zvy.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://vjv.c1oappe.top

[U75] PHP：依赖注入
来源：http://qyq.hesvh.cn

composer require psr/container
来源：http://ecc.tianlin.xyz

[U76] PHP：简单路由
来源：http://qpt.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kxc.sxryk.cn

[U77] PHP：模板渲染
来源：http://sll.epnwcf.com

composer require twig/twig
来源：http://foq.aibaodan.cn

[U78] PHP：单元测试
来源：http://cfg.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://srp.52xcode.cn


<!-- 参考信息 -->