代发 wailian999

int size() const noexcept { return n_; }
来源：http://rer.jlsjyb.cn

[S53] C++：移动语义
来源：http://ivd.uphjek.com

std::vector<int> w = std::move(v);
来源：http://zfu.quarkkingdee.top

[S54] C++：异常处理
来源：http://kee.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gss.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://hns.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qif.ivvv.top

[S56] C++：optional
来源：http://bfg.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jyu.vqdsnc.cn

[S57] C++：编译期常量
来源：http://hme.dianchejie.cn

constexpr int N = 10;
来源：http://vee.sxryk.cn

[S58] C++：命名空间
来源：http://exp.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://cga.hnxiangtu.top

[S59] C++：静态断言
来源：http://yak.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tvi.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://mhk.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wdr.zhijiandao.cn

================================================================================
来源：http://fkr.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vbe.meibo888.top

================================================================================
来源：http://yhs.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://hog.zhiwuduotai.top

println("Hello")
来源：http://nna.zdbjq.cn

[T02] Kotlin：变量
来源：http://jhx.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ogw.tanke756.top

[T03] Kotlin：字符串模板
来源：http://jjn.pengpengdd.cyou

"值: $b"
来源：http://ygr.jiagoushi.top

[T04] Kotlin：空安全
来源：http://blw.yongpay.top

val n: String? = null;  n?.length
来源：http://ikv.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://fsb.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dhq.ivvv.top

[T06] Kotlin：集合映射
来源：http://eng.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hxv.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://egw.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://caf.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://ruj.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://nys.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://vzo.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://hal.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://upw.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://alo.bbcook.cn

[T11] Kotlin：协程
来源：http://jeo.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dva.sweek.top

[T12] Kotlin：解构声明
来源：http://yap.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://cvu.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://pep.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://fkq.vqdsnc.cn

[T14] Kotlin：循环
来源：http://bxr.dashuyun.cn

for (i in 1..10) println(i)
来源：http://nhu.epnwcf.com

[T15] Kotlin：接口
来源：http://uhb.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://jbj.zhijiandao.cn

[T16] Swift：Hello World
来源：http://gtr.pycfn.com

print("Hello")
来源：http://vua.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://lvh.yvedp.cn

var a = 1;  let b = 2
来源：http://mts.xziqi.cn

[T18] Swift：字符串插值
来源：http://xqy.zhongyouzk.top

"值: \(b)"
来源：http://foe.cashguo.top

[T19] Swift：可选绑定
来源：http://gmp.0kj1m.cn

if let n = opt { print(n) }
来源：http://awc.kuanghao11.cn

[T20] Swift：数组操作
来源：http://cus.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gpk.jianghu66.top

[T21] Swift：遍历
来源：http://wvd.xziqi.cn

for x in a { print(x) }
来源：http://cci.vqdsnc.cn

[T22] Swift：字典
来源：http://hlq.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://bke.shanyushiyangtech.top

[T23] Swift：函数
来源：http://blw.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lyk.pengpengdd.cyou

[T24] Swift：闭包
来源：http://jun.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hoc.daria6918.cn

[T25] Swift：结构体
来源：http://aig.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://fny.c1oappe.top

[T26] Swift：类与重写
来源：http://ecq.ivvv.top

class A: Base { override func f() {} }
来源：http://yfo.jyoumei.cn

[T27] Swift：错误处理
来源：http://gno.cucudq.cn

do { try f() } catch { print(error) }
来源：http://vza.aibaodan.cn

[T28] Swift：枚举
来源：http://mke.xinyue.icu

enum Color { case red, green }
来源：http://eca.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://esn.0kj1m.cn

guard let x = opt else { return }
来源：http://gyt.sweek.top

[T30] Swift：协议
来源：http://cav.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://pxf.wangdashe.top

[T31] Lua：Hello World
来源：http://lvi.andypj.xyz

print("Hello")
来源：http://iod.hysaishi.cn

[T32] Lua：局部变量
来源：http://iqa.jqgufenzy.top

local a = 1
来源：http://kgz.zycfv.cn

[T33] Lua：表（数组）
来源：http://qha.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sya.haohaochexian.top

[T34] Lua：遍历表
来源：http://qhg.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://swn.vqdsnc.cn

[T35] Lua：字典表
来源：http://lsw.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://ymh.feifeiyinyue.top

[T36] Lua：函数
来源：http://vlk.aizwys.cn

function add(a, b) return a + b end
来源：http://iuz.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://rqi.shanyushiyangtech.top

"a" .. "b"
来源：http://yex.cdnleiting.top

[T38] Lua：条件
来源：http://ide.zhixingplan.top

if x > 0 then print("正") end
来源：http://hyn.guowangkeji.top

[T39] Lua：模式匹配
来源：http://txa.dianchejie.cn

string.find(s, "%d+")
来源：http://vcf.ydjk.org.cn

[T40] Lua：元表
来源：http://bdd.xziqi.cn

setmetatable({}, { __index = base })
来源：http://jmk.jqgufenzy.top

[T41] Perl：Hello World
来源：http://vdw.fktsv.cn

print "Hello\n";
来源：http://bya.fzhhl.top

[T42] Perl：变量类型
来源：http://wqo.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://csl.cqqwz.cn

[T43] Perl：字符串插值
来源：http://stk.hongshengwenyu.top

"值: $a"
来源：http://dhl.zdqjudy.top

[T44] Perl：条件
来源：http://qhn.cashguo.top

if ($a > 0) { print "正"; }
来源：http://bvs.hesvh.cn

[T45] Perl：数组遍历
来源：http://tmq.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://qxy.tanke756.top

[T46] Perl：哈希操作
来源：http://hvk.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kur.smart0.xyz

[T47] Perl：正则捕获
来源：http://fsu.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kju.aizwys.cn

[T48] Perl：正则替换
来源：http://kkm.chenlongwang.top

$s =~ s/old/new/g;
来源：http://ysp.zhixingplan.top

[T49] Perl：函数
来源：http://qck.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vbe.yongpay.top

[T50] Perl：逐行读文件
来源：http://uca.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vhs.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://jrl.hywenlv.cn

[T51] Scala：Hello World
来源：http://akt.zhoulong.xyz

println("Hello")
来源：http://wwd.zhiwuduotai.top

[T52] Scala：变量
来源：http://xcg.zhijiandao.cn

val a = 1;  var b = 2
来源：http://qui.fktsv.cn

[T53] Scala：字符串插值
来源：http://yyt.uphjek.com

s"值: $b"
来源：http://saq.ydjk.org.cn

[T54] Scala：集合映射
来源：http://bjd.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://ewt.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://eva.zhaomingkeji.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://cyq.fktsv.cn

[T56] Scala：样例类
来源：http://dlx.zhengqikj.top

case class User(name: String, age: Int)
来源：http://jnk.cqqwz.cn

[T57] Scala：模式匹配
来源：http://geb.tianlin.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://rnq.shuidangran.top

[T58] Scala：函数定义
来源：http://kek.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://qli.bjfxy.top

[T59] Scala：循环
来源：http://vyl.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://due.hywenlv.cn

[T60] Scala：折叠
来源：http://lyd.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://urr.yj20258888.top

================================================================================
来源：http://qzb.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hnd.jqgfzy.top

================================================================================
来源：http://nyg.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://ijw.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://xjv.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://abp.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pyx.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://rfs.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://baa.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://pou.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dqt.yueranfly.top

[U05] Py：列表去重且保序
来源：http://dhl.sweek.top

list(dict.fromkeys(arr))
来源：http://nrl.redwolf501.top

[U06] Py：合并两个字典
来源：http://xvr.sweek.top

{**a, **b}
来源：http://tic.hcnkem.com

[U07] Py：反转字典键值
来源：http://jnq.yueranfly.top

{v: k for k, v in d.items()}
来源：http://zug.ehwqpu.com

[U08] Py：展平二维列表
来源：http://buh.0kj1m.cn

[y for x in nested for y in x]
来源：http://aoj.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://uog.tian-w.cn

max(d, key=d.get)
来源：http://oba.wangdashe.top

[U10] Py：按值排序字典
来源：http://dac.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rey.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://bpa.gotoacloud.top

(x * 2 for x in arr)
来源：http://cci.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://rgf.fehbvm.com

Counter(arr).most_common(3)
来源：http://kex.tianlin.xyz

[U13] Py：固定长度队列
来源：http://gny.gogol.net.cn

deque(maxlen=10)
来源：http://tyi.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://hjx.xylfe.cn

defaultdict(list)
来源：http://kuw.zhijiandao.cn

[U15] Py：高精度计时
来源：http://jgy.xinyue.icu

t = time.perf_counter()
来源：http://nnb.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://mzf.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cvg.andypj.xyz

[U17] Py：初始化日志
来源：http://vjw.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://hcl.daria6918.cn

[U18] Py：预编译正则
来源：http://emu.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://dap.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://hha.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tyb.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://inc.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://shp.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://giv.ydjk.org.cn

@contextlib.contextmanager
来源：http://lix.sufxvd.cn

[U22] Py：矩阵转置
来源：http://rtm.cdnleiting.top

list(zip(*m))
来源：http://gif.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://jur.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vou.daxiang520.top

[U24] Py：路径操作
来源：http://ngw.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://arb.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://scq.yonumen.top

csv.DictReader(f)
来源：http://wbu.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://bpm.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://psx.yuxming.cn

[U27] Py：异步 HTTP
来源：http://mmc.shuidangran.top

aiohttp.ClientSession() 配合 async with
来源：http://jyc.mhx1999.top

[U28] Py：类型别名
来源：http://bfg.jqgufenzy.top

UserId = int
来源：http://yov.pycfn.com

[U29] Py：属性校验
来源：http://ifh.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://pew.birdmap.top

[U30] Py：数据类
来源：http://qvg.jiagoushi.top

@dataclass(slots=True)
来源：http://emc.uphjek.com

[U31] Py：单测
来源：http://imv.ctjpmb.com

python -m pytest -q
来源：http://cyl.fehbvm.com

[U32] Py：代码格式化
来源：http://juo.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://etd.andypj.xyz

[U33] Py：打包发布
来源：http://gir.yonumen.top

python -m build  （依赖 pyproject.toml）
来源：http://mip.hysaishi.cn

[U34] Py：判断编码
来源：http://twm.ctjpmb.com

chardet.detect(raw)
来源：http://inh.jqgfzy.top

[U35] Py：发送邮件
来源：http://gkw.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pps.jiagoushi.top

[U36] Py：定时任务
来源：http://imi.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://frn.bjfxy.top

[U37] Py：读写 Excel
来源：http://gth.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pax.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://izi.hcnkem.com

Path(__file__).resolve().parent
来源：http://tvo.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://vza.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://lar.fengsongda.top

[U40] Py：打印到标准错误
来源：http://jjh.nwbrower.top

print("err", file=sys.stderr)
来源：http://zob.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://yoj.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://leg.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ytv.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xxa.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://dck.ivvv.top

namespace App\Http;
来源：http://vgv.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://lug.hammf.cn

declare(strict_types=1);
来源：http://mak.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://kdu.sweek.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://edc.yj20258.top

[U46] PHP：可空类型
来源：http://ngb.yvedp.cn

?string $name = null
来源：http://xii.yueranfly.top

[U47] PHP：联合类型
来源：http://fzg.tian-w.cn

int|string $id
来源：http://quk.guowangkeji.top

[U48] PHP：纯枚举
来源：http://bes.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kaw.zhongyouzk.top

[U49] PHP：只读属性
来源：http://gqe.ivvv.top

public readonly string $name
来源：http://ndo.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://chn.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://dne.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://gtk.gaohongyu789.top

[$a, $b] = $arr;
来源：http://scd.daxiang520.top

[U52] PHP：箭头函数
来源：http://sch.fanxiaobao.xyz

$double = fn($x) => $x * 2;
来源：http://rsf.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://luf.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://ecl.jinqigufen.top

[U54] PHP：空安全调用
来源：http://wuw.yuanzhike.top

$obj?->method()
来源：http://hqt.yuxming.cn

[U55] PHP：match 表达式
来源：http://dpz.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tqs.zhixingplan.top

[U56] PHP：命名参数
来源：http://fgu.svipenyu.cn

f(a: 1, b: 2)
来源：http://sgs.tian-w.cn

[U57] PHP：字符串插值
来源：http://ler.quarkkingdee.top

"值: {$a}"
来源：http://kgq.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://jcg.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xql.tian-w.cn

[U59] PHP：自定义排序
来源：http://xhq.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kej.ivvv.top

[U60] PHP：JSON 编解码
来源：http://qfd.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xai.fehbvm.com

[U61] PHP：正则
来源：http://kqp.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uwd.zycfv.cn

[U62] PHP：日期对象
来源：http://mnd.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rqt.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://sdf.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://urw.ehwqpu.com

[U64] PHP：目录遍历
来源：http://fgf.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://dex.ctjpmb.com

[U65] PHP：会话
来源：http://pjk.uphjek.com

session_start();  $_SESSION["uid"] = 1;
来源：http://mjk.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://coh.hesvh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://chz.mhx1999.top

[U67] PHP：处理文件上传
来源：http://eld.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jcg.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://kys.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rxh.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://elm.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tpa.tian-w.cn

[U70] PHP：PDO 事务
来源：http://dhj.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://itq.hesvh.cn

[U71] PHP：抛出异常
来源：http://kcc.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://fqv.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://lre.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://ckl.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://qmb.hfpthk.cn

parse_ini_file("config.ini", true)
来源：http://mfm.gzhubu.top

[U74] PHP：读取环境变量
来源：http://lrp.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://kxt.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://epl.tanke756.top

composer require psr/container
来源：http://tdn.bbcook.cn

[U76] PHP：简单路由
来源：http://bcq.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://key.meibo888.top

[U77] PHP：模板渲染
来源：http://hdf.shzxlz.cn

composer require twig/twig
来源：http://vca.haohaochexian.top

[U78] PHP：单元测试
来源：http://xle.tarul.cn

composer require --dev phpunit/phpunit
来源：http://rpy.yj20258.top


<!-- 参考信息 -->