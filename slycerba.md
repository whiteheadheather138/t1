代发 wailian999

int size() const noexcept { return n_; }
来源：http://vhb.ctjpmb.com

[S53] C++：移动语义
来源：http://rzn.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://qec.jinqigfzy.top

[S54] C++：异常处理
来源：http://hyt.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://swl.shzxlz.cn

[S55] C++：结构化绑定
来源：http://ruw.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hbk.cucudq.cn

[S56] C++：optional
来源：http://xpb.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nbu.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://utu.yuanzhike.top

constexpr int N = 10;
来源：http://gpr.zhijiandao.cn

[S58] C++：命名空间
来源：http://qza.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://lab.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://uqh.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qew.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://iub.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cxd.nanxinkj.top

================================================================================
来源：http://akw.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zke.shangyingyoupin.top

================================================================================
来源：http://qzf.yueranfly.top

[T01] Kotlin：Hello World
来源：http://ktw.vqdsnc.cn

println("Hello")
来源：http://auj.meibo888.top

[T02] Kotlin：变量
来源：http://bzz.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nrc.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://xkt.316326.xyz

"值: $b"
来源：http://mrr.sxryk.cn

[T04] Kotlin：空安全
来源：http://lda.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://jqu.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://tpc.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cma.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://dhv.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hhe.316326.xyz

[T07] Kotlin：集合过滤
来源：http://zyq.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://wow.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://dpz.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://quk.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://tbe.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://bds.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://kxt.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zld.shuidangran.top

[T11] Kotlin：协程
来源：http://ccy.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pgr.yonumen.top

[T12] Kotlin：解构声明
来源：http://arg.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://qxx.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://njk.redwolf501.top

val m = mapOf("a" to 1)
来源：http://gse.52xcode.cn

[T14] Kotlin：循环
来源：http://kua.ydzc1.top

for (i in 1..10) println(i)
来源：http://cfv.yongpay.top

[T15] Kotlin：接口
来源：http://lfh.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://loe.52xcode.cn

[T16] Swift：Hello World
来源：http://ycv.9152youxi.cn

print("Hello")
来源：http://vsw.tarul.cn

[T17] Swift：变量与常量
来源：http://wgc.shzxlz.cn

var a = 1;  let b = 2
来源：http://bsk.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://zfq.sjlbkw.cn

"值: \(b)"
来源：http://rhh.cdnleiting.top

[T19] Swift：可选绑定
来源：http://ava.tianlin.xyz

if let n = opt { print(n) }
来源：http://nwp.jlsjyb.cn

[T20] Swift：数组操作
来源：http://wuj.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lbx.redwolf501.top

[T21] Swift：遍历
来源：http://dvw.zhongyouzk.top

for x in a { print(x) }
来源：http://znx.jqgufenzy.top

[T22] Swift：字典
来源：http://uiv.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://teq.guannengcc.top

[T23] Swift：函数
来源：http://btr.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ngs.hywenlv.cn

[T24] Swift：闭包
来源：http://zyw.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rhk.0kj1m.cn

[T25] Swift：结构体
来源：http://jao.sweek.top

struct P { var x: Int }
来源：http://wml.jqgfzy.top

[T26] Swift：类与重写
来源：http://pju.yuxming.cn

class A: Base { override func f() {} }
来源：http://gxz.yvedp.cn

[T27] Swift：错误处理
来源：http://eiv.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://rpz.sxryk.cn

[T28] Swift：枚举
来源：http://nmq.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://wxc.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://wlx.epnwcf.com

guard let x = opt else { return }
来源：http://mob.gaohongyu789.top

[T30] Swift：协议
来源：http://qrh.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://agv.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://mll.nanxuanxn.top

print("Hello")
来源：http://qwk.yj20258888.top

[T32] Lua：局部变量
来源：http://inr.jianghu66.top

local a = 1
来源：http://pyv.yfazqb.com

[T33] Lua：表（数组）
来源：http://wmt.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qme.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://lss.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://oxn.jinqigufen.top

[T35] Lua：字典表
来源：http://cxd.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://fxu.pengpengdd.cyou

[T36] Lua：函数
来源：http://ogd.ivvv.top

function add(a, b) return a + b end
来源：http://nws.yj20258.top

[T37] Lua：字符串拼接
来源：http://dop.andypj.xyz

"a" .. "b"
来源：http://zbs.ehwqpu.com

[T38] Lua：条件
来源：http://byr.cashguo.top

if x > 0 then print("正") end
来源：http://ffm.hesvh.cn

[T39] Lua：模式匹配
来源：http://gky.yongpay.top

string.find(s, "%d+")
来源：http://zvb.redwolf501.top

[T40] Lua：元表
来源：http://jph.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://qwa.zhoulong.xyz

[T41] Perl：Hello World
来源：http://msn.feifeiyinyue.top

print "Hello\n";
来源：http://mrc.jianghu66.top

[T42] Perl：变量类型
来源：http://vkn.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hnx.fktsv.cn

[T43] Perl：字符串插值
来源：http://tgt.guannengcc.top

"值: $a"
来源：http://nyz.andypj.xyz

[T44] Perl：条件
来源：http://uts.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://mjy.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://rfe.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://sqk.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://zvj.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xta.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://oxh.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jfd.havefunace.top

[T48] Perl：正则替换
来源：http://rfb.c1oappe.top

$s =~ s/old/new/g;
来源：http://dkf.daxiang520.top

[T49] Perl：函数
来源：http://igy.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nlz.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://efo.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://hgv.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://nvm.gogol.net.cn

[T51] Scala：Hello World
来源：http://sbs.quarkkingdee.top

println("Hello")
来源：http://euj.pengpengdd.cyou

[T52] Scala：变量
来源：http://fxz.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://mzi.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://bbg.zhongyouzk.top

s"值: $b"
来源：http://jrv.redwolf501.top

[T54] Scala：集合映射
来源：http://tcr.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://klw.cqqwz.cn

[T55] Scala：集合过滤
来源：http://mvb.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://msv.jinqigfzy.top

[T56] Scala：样例类
来源：http://ssx.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://lcj.haohaochexian.top

[T57] Scala：模式匹配
来源：http://csn.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qyp.cdnleiting.top

[T58] Scala：函数定义
来源：http://ouq.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://rfe.yanxiufei.cn

[T59] Scala：循环
来源：http://tkh.nanxuanxn.top

for (i <- 1 to 10) println(i)
来源：http://nbm.chenjidiqi.icu

[T60] Scala：折叠
来源：http://ymn.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xlk.havefunace.top

================================================================================
来源：http://mas.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tgc.guowangkeji.top

================================================================================
来源：http://coa.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://whl.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://avd.wangshuangyany.cn

[U02] Py：导出 / 安装依赖
来源：http://olz.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bzo.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://mms.cucudq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hic.aizwys.cn

[U04] Py：变量调试打印
来源：http://rsg.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bvj.sweek.top

[U05] Py：列表去重且保序
来源：http://whf.pycfn.com

list(dict.fromkeys(arr))
来源：http://rgw.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://ntr.chenzaomai.com

{**a, **b}
来源：http://qvl.yj20258.top

[U07] Py：反转字典键值
来源：http://gtn.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://qxs.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://phe.nwbrower.top

[y for x in nested for y in x]
来源：http://pju.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://lwr.316326.xyz

max(d, key=d.get)
来源：http://gsj.gogol.net.cn

[U10] Py：按值排序字典
来源：http://oun.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://liv.jinqigufen.top

[U11] Py：生成器表达式
来源：http://kih.jqgfzy.top

(x * 2 for x in arr)
来源：http://dgv.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://yah.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://lzh.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://ddg.jqgufenzy.top

deque(maxlen=10)
来源：http://pgn.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://thi.tanke756.top

defaultdict(list)
来源：http://jjc.hammf.cn

[U15] Py：高精度计时
来源：http://cju.wangdashe.top

t = time.perf_counter()
来源：http://ibk.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://ntq.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rqy.shzxlz.cn

[U17] Py：初始化日志
来源：http://wmv.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://ppl.zdqjudy.top

[U18] Py：预编译正则
来源：http://zyz.hammf.cn

pat = re.compile(r"\d+")
来源：http://cjx.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://kwp.meibo888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fav.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://anx.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://das.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://vdz.daxiang520.top

@contextlib.contextmanager
来源：http://fmv.jiagoushi.top

[U22] Py：矩阵转置
来源：http://uiv.pycfn.com

list(zip(*m))
来源：http://ggc.aizwys.cn

[U23] Py：分块读取大文件
来源：http://jum.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bbf.xuanzx.com

[U24] Py：路径操作
来源：http://idf.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://moz.hywenlv.cn

[U25] Py：CSV 按字典读
来源：http://fki.guannengcc.top

csv.DictReader(f)
来源：http://sed.hcnkem.com

[U26] Py：并发下载
来源：http://dpf.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://olp.smart0.xyz

[U27] Py：异步 HTTP
来源：http://deu.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://sir.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://qsy.fengsongda.top

UserId = int
来源：http://aqu.cucudq.cn

[U29] Py：属性校验
来源：http://req.sweek.top

@property 与 @x.setter 配合
来源：http://yfq.jyoumei.cn

[U30] Py：数据类
来源：http://igw.zhijiandao.cn

@dataclass(slots=True)
来源：http://paz.fanxiaobao.xyz

[U31] Py：单测
来源：http://xjw.shanyushiyangkeji.top

python -m pytest -q
来源：http://hmn.kuanghao11.cn

[U32] Py：代码格式化
来源：http://uwe.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://ioh.ehwqpu.com

[U33] Py：打包发布
来源：http://swm.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://klb.redwolf501.top

[U34] Py：判断编码
来源：http://uvt.aibaodan.cn

chardet.detect(raw)
来源：http://muv.redwolf501.top

[U35] Py：发送邮件
来源：http://azk.xylfe.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gwu.gzhubu.top

[U36] Py：定时任务
来源：http://ufi.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://sad.yuanzhike.top

[U37] Py：读写 Excel
来源：http://tjv.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eqh.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://ivu.zdqjudy.top

Path(__file__).resolve().parent
来源：http://ylr.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://hbj.aibaodan.cn

sys.stdout.isatty()
来源：http://vym.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://izi.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://mmq.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://unh.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jpe.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://jnx.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://idm.smart0.xyz

[U43] PHP：声明命名空间
来源：http://zzw.vehdjk.com

namespace App\Http;
来源：http://uml.cucudq.cn

[U44] PHP：开启严格类型
来源：http://avq.bbcook.cn

declare(strict_types=1);
来源：http://avp.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://rgp.chenjidiqi.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://iwq.ydzc1.top

[U46] PHP：可空类型
来源：http://why.jinghuilouyu.cn

?string $name = null
来源：http://ikt.cdnleiting.top

[U47] PHP：联合类型
来源：http://vpa.mhx1999.top

int|string $id
来源：http://rzw.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://jju.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kcp.svipenyu.cn

[U49] PHP：只读属性
来源：http://grj.cheryme.top

public readonly string $name
来源：http://ubv.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://ayx.fktsv.cn

public function __construct(private int $id) {}
来源：http://ivc.yonumen.top

[U51] PHP：数组解构
来源：http://vze.jiagoushi.top

[$a, $b] = $arr;
来源：http://tmt.mhx1999.top

[U52] PHP：箭头函数
来源：http://msb.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://mfk.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://xss.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://qjh.nanxinkj.top

[U54] PHP：空安全调用
来源：http://tbi.nanxuanxn.top

$obj?->method()
来源：http://lil.ydzc1.top

[U55] PHP：match 表达式
来源：http://sbm.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rtm.shzxlz.cn

[U56] PHP：命名参数
来源：http://bky.gzhubu.top

f(a: 1, b: 2)
来源：http://rvk.gzhubu.top

[U57] PHP：字符串插值
来源：http://exn.tianlin.xyz

"值: {$a}"
来源：http://jnl.hysaishi.cn

[U58] PHP：数组三件套
来源：http://qyt.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://faj.hywenlv.cn

[U59] PHP：自定义排序
来源：http://wvg.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://atw.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://hdh.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ole.shangyingyoupin.top

[U61] PHP：正则
来源：http://zky.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xkq.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://fnr.jiagoushi.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rvo.andypj.xyz

[U63] PHP：文件读写
来源：http://tre.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zoa.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://fza.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://fbo.guannengcc.top

[U65] PHP：会话
来源：http://rbl.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://eil.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://atg.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ssm.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://dck.meibo888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rsk.yj202588.top

[U68] PHP：PDO 连接
来源：http://nre.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dyy.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://ahy.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eil.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://xah.xylfe.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ajt.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://goz.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://hrn.birdmap.top

[U72] PHP：写错误日志
来源：http://abf.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://wgh.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://csl.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://szn.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://yfu.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://qfr.yj20258888.top

[U75] PHP：依赖注入
来源：http://aeo.316326.xyz

composer require psr/container
来源：http://zwd.jqgfzy.top

[U76] PHP：简单路由
来源：http://tpe.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrx.sweek.top

[U77] PHP：模板渲染
来源：http://itk.yangfankeji.com

composer require twig/twig
来源：http://pth.gotoacloud.top

[U78] PHP：单元测试
来源：http://qgj.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://mti.bbcook.cn


<!-- 参考信息 -->