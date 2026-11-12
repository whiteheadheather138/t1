代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pme.daxiang520.top

[S55] C++：结构化绑定
来源：http://ryj.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zbv.yvedp.cn

[S56] C++：optional
来源：http://hto.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sbm.ppjwa.cn

[S57] C++：编译期常量
来源：http://unx.c1oappe.top

constexpr int N = 10;
来源：http://coo.ybcxt.top

[S58] C++：命名空间
来源：http://njw.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://uei.0kj1m.cn

[S59] C++：静态断言
来源：http://bsk.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dwr.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://zah.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pmk.zhaomingkeji.xyz

================================================================================
来源：http://qqz.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdb.0kj1m.cn

================================================================================
来源：http://tou.meibo888.top

[T01] Kotlin：Hello World
来源：http://pys.fktsv.cn

println("Hello")
来源：http://oqy.yonumen.top

[T02] Kotlin：变量
来源：http://zmj.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://emi.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://hnm.pycfn.com

"值: $b"
来源：http://hhv.aibaodan.cn

[T04] Kotlin：空安全
来源：http://rjg.bbcook.cn

val n: String? = null;  n?.length
来源：http://fgb.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://awr.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nma.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://ccx.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vlw.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://lwi.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://juw.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://oqh.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://ixt.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://zsz.yj202588.top

fun String.exclaim() = this + "!"
来源：http://wtd.gzhubu.top

[T10] Kotlin：默认参数
来源：http://ule.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sms.hesvh.cn

[T11] Kotlin：协程
来源：http://bkg.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://apo.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://eqe.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://sdb.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://hgp.sxryk.cn

val m = mapOf("a" to 1)
来源：http://sil.316326.xyz

[T14] Kotlin：循环
来源：http://bpn.dianchejie.cn

for (i in 1..10) println(i)
来源：http://dbi.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://mqu.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://vez.vqdsnc.cn

[T16] Swift：Hello World
来源：http://wjv.iojbl.cn

print("Hello")
来源：http://yps.haohaochexian.top

[T17] Swift：变量与常量
来源：http://vkn.guannengcc.top

var a = 1;  let b = 2
来源：http://pdm.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://kij.yuxming.cn

"值: \(b)"
来源：http://ijg.jianghu66.top

[T19] Swift：可选绑定
来源：http://pmp.zdqjudy.top

if let n = opt { print(n) }
来源：http://muf.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://zsh.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://bbv.316326.xyz

[T21] Swift：遍历
来源：http://ftk.quarkkingdee.top

for x in a { print(x) }
来源：http://rax.xuetiantiany.cn

[T22] Swift：字典
来源：http://orb.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://lvo.gogol.net.cn

[T23] Swift：函数
来源：http://rph.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ker.jqgfzy.top

[T24] Swift：闭包
来源：http://uyl.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hvj.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://eai.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://wrh.sxryk.cn

[T26] Swift：类与重写
来源：http://ypd.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://ajm.daria6918.cn

[T27] Swift：错误处理
来源：http://uyk.316326.xyz

do { try f() } catch { print(error) }
来源：http://enr.jqgfzy.top

[T28] Swift：枚举
来源：http://yju.yonumen.top

enum Color { case red, green }
来源：http://ylt.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://twn.gogol.net.cn

guard let x = opt else { return }
来源：http://ugg.cdnleiting.top

[T30] Swift：协议
来源：http://dhj.cheryme.top

protocol Shape { func area() -> Double }
来源：http://ket.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://jzm.xziqi.cn

print("Hello")
来源：http://xef.cqqwz.cn

[T32] Lua：局部变量
来源：http://mfg.fktsv.cn

local a = 1
来源：http://rin.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://tln.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mvn.chenzaomai.com

[T34] Lua：遍历表
来源：http://ddx.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fwi.xinyue.icu

[T35] Lua：字典表
来源：http://rwz.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://khg.hywenlv.cn

[T36] Lua：函数
来源：http://lbq.fktsv.cn

function add(a, b) return a + b end
来源：http://ehj.yfazqb.com

[T37] Lua：字符串拼接
来源：http://tkf.zhaomingkeji.xyz

"a" .. "b"
来源：http://obn.snrcjt.cn

[T38] Lua：条件
来源：http://hav.shuidangran.top

if x > 0 then print("正") end
来源：http://zmo.yuxming.cn

[T39] Lua：模式匹配
来源：http://btu.ybcxt.top

string.find(s, "%d+")
来源：http://kjr.0kj1m.cn

[T40] Lua：元表
来源：http://rco.yj202588.top

setmetatable({}, { __index = base })
来源：http://hvv.hfpthk.cn

[T41] Perl：Hello World
来源：http://tvv.kuanghao11.cn

print "Hello\n";
来源：http://spj.xinyue.icu

[T42] Perl：变量类型
来源：http://jka.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sio.yueranfly.top

[T43] Perl：字符串插值
来源：http://xkc.gogol.net.cn

"值: $a"
来源：http://gxp.zdbjq.cn

[T44] Perl：条件
来源：http://vrg.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://bao.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://tct.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://wou.xylfe.cn

[T46] Perl：哈希操作
来源：http://pew.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://msv.jqgfzy.top

[T47] Perl：正则捕获
来源：http://gki.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://mdl.vehdjk.com

[T48] Perl：正则替换
来源：http://tjk.tarul.cn

$s =~ s/old/new/g;
来源：http://ila.pycfn.com

[T49] Perl：函数
来源：http://dcr.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hvw.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://rhv.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ssq.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://ipa.sufxvd.cn

[T51] Scala：Hello World
来源：http://nth.jqgfzy.top

println("Hello")
来源：http://kvj.tanke756.top

[T52] Scala：变量
来源：http://dtu.xziqi.cn

val a = 1;  var b = 2
来源：http://uwh.c1oappe.top

[T53] Scala：字符串插值
来源：http://ipf.zhaomingkeji.xyz

s"值: $b"
来源：http://bkq.tian-w.cn

[T54] Scala：集合映射
来源：http://uyq.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://zeg.daxiang520.top

[T55] Scala：集合过滤
来源：http://gns.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://fue.yvedp.cn

[T56] Scala：样例类
来源：http://pfd.jyoumei.cn

case class User(name: String, age: Int)
来源：http://ooc.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://tib.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ssp.quarkkingdee.top

[T58] Scala：函数定义
来源：http://tet.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://zby.vqdsnc.cn

[T59] Scala：循环
来源：http://sml.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://ece.andypj.xyz

[T60] Scala：折叠
来源：http://dcg.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://veo.yj20258888.top

================================================================================
来源：http://sch.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zgb.gotoacloud.top

================================================================================
来源：http://yyq.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://ftd.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://rdd.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://fei.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oyh.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://sox.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lnt.zhixingplan.top

[U04] Py：变量调试打印
来源：http://voh.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lpt.yonumen.top

[U05] Py：列表去重且保序
来源：http://gec.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://hds.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://kno.feifeiyinyue.top

{**a, **b}
来源：http://cki.yvedp.cn

[U07] Py：反转字典键值
来源：http://cqt.ydzc1.top

{v: k for k, v in d.items()}
来源：http://bwc.yueranfly.top

[U08] Py：展平二维列表
来源：http://jdc.dashuyun.cn

[y for x in nested for y in x]
来源：http://iza.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://zag.tarul.cn

max(d, key=d.get)
来源：http://bzo.tian-w.cn

[U10] Py：按值排序字典
来源：http://jro.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://orm.hammf.cn

[U11] Py：生成器表达式
来源：http://nea.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://wqz.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://uxg.fktsv.cn

Counter(arr).most_common(3)
来源：http://gov.xuanzx.com

[U13] Py：固定长度队列
来源：http://anr.feifeiyinyue.top

deque(maxlen=10)
来源：http://nck.iojbl.cn

[U14] Py：分组收集到列表
来源：http://zng.0kj1m.cn

defaultdict(list)
来源：http://nzn.zdbjq.cn

[U15] Py：高精度计时
来源：http://akw.andypj.xyz

t = time.perf_counter()
来源：http://ysg.fzhhl.top

[U16] Py：命令行参数解析
来源：http://wkg.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gnh.xziqi.cn

[U17] Py：初始化日志
来源：http://eiw.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://uoe.chenzaomai.com

[U18] Py：预编译正则
来源：http://zep.cheryme.top

pat = re.compile(r"\d+")
来源：http://yrx.yuxming.cn

[U19] Py：正则替换带回调
来源：http://soz.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ypq.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://lhp.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://bed.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://aby.yueranfly.top

@contextlib.contextmanager
来源：http://hjp.haohaochexian.top

[U22] Py：矩阵转置
来源：http://cij.cheryme.top

list(zip(*m))
来源：http://dls.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://tkm.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fal.cucudq.cn

[U24] Py：路径操作
来源：http://kjx.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jym.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://eby.9152youxi.cn

csv.DictReader(f)
来源：http://ujc.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://nau.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cec.bjfxy.top

[U27] Py：异步 HTTP
来源：http://jld.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://dfu.vehdjk.com

[U28] Py：类型别名
来源：http://acd.dashuyun.cn

UserId = int
来源：http://ypr.bjfxy.top

[U29] Py：属性校验
来源：http://swj.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://rjm.daria6918.cn

[U30] Py：数据类
来源：http://gjo.xziqi.cn

@dataclass(slots=True)
来源：http://feq.tian-w.cn

[U31] Py：单测
来源：http://eyx.iojbl.cn

python -m pytest -q
来源：http://etn.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://syw.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://uns.yangfankeji.com

[U33] Py：打包发布
来源：http://hsk.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://xvw.gzhubu.top

[U34] Py：判断编码
来源：http://wez.shanyushiyangtech.top

chardet.detect(raw)
来源：http://rdw.316326.xyz

[U35] Py：发送邮件
来源：http://yrw.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dtm.yanxiufei.cn

[U36] Py：定时任务
来源：http://dit.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://yxu.ehwqpu.com

[U37] Py：读写 Excel
来源：http://kiz.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pmd.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://dol.uphjek.com

Path(__file__).resolve().parent
来源：http://ahj.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://tdi.zycfv.cn

sys.stdout.isatty()
来源：http://fyb.xziqi.cn

[U40] Py：打印到标准错误
来源：http://rli.ctjpmb.com

print("err", file=sys.stderr)
来源：http://upz.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://lnm.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gzg.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://kfd.hammf.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bdi.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://hwh.birdmap.top

namespace App\Http;
来源：http://xbr.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://yzp.kuanghao11.cn

declare(strict_types=1);
来源：http://hlx.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://kgr.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://ujf.sjlbkw.cn

[U46] PHP：可空类型
来源：http://dkd.xingfuxueyuan.xyz

?string $name = null
来源：http://cel.tarul.cn

[U47] PHP：联合类型
来源：http://ulw.ydzc1.top

int|string $id
来源：http://osm.gzhubu.top

[U48] PHP：纯枚举
来源：http://esf.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sod.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://zll.zdbjq.cn

public readonly string $name
来源：http://lhc.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://rpj.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://tzb.sysykeji.top

[U51] PHP：数组解构
来源：http://vft.ctjpmb.com

[$a, $b] = $arr;
来源：http://nmf.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://wto.snrcjt.cn

$double = fn($x) => $x * 2;
来源：http://pzc.fktsv.cn

[U53] PHP：空合并运算符
来源：http://iej.uphjek.com

$v = $a ?? $b ?? "default";
来源：http://hjm.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://qap.zhixingplan.top

$obj?->method()
来源：http://aoe.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://ezt.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://crp.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://xdn.ybcxt.top

f(a: 1, b: 2)
来源：http://yfd.hnqzz.top

[U57] PHP：字符串插值
来源：http://fpo.haohaochexian.top

"值: {$a}"
来源：http://cuk.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://fra.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oup.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://rbr.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mhc.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://lwz.zycfv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nxb.yangfankeji.com

[U61] PHP：正则
来源：http://gbm.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fzc.xinyue.icu

[U62] PHP：日期对象
来源：http://wam.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jqq.bjfxy.top

[U63] PHP：文件读写
来源：http://epm.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fgw.tanke756.top

[U64] PHP：目录遍历
来源：http://xbf.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://bfa.ydjk.org.cn

[U65] PHP：会话
来源：http://evi.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://oss.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://get.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xcv.uphjek.com

[U67] PHP：处理文件上传
来源：http://nsj.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bun.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://onq.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bcm.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://aoj.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vtv.tarul.cn

[U70] PHP：PDO 事务
来源：http://bra.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lrg.daxiang520.top

[U71] PHP：抛出异常
来源：http://cuk.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://fdz.yongpay.top

[U72] PHP：写错误日志
来源：http://zhn.jianghu66.top

error_log("失败: " . $e->getMessage());
来源：http://jzr.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://qev.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://hpk.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://sij.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://tfc.chenzaomai.com

[U75] PHP：依赖注入
来源：http://fhn.pycfn.com

composer require psr/container
来源：http://osg.yongpay.top

[U76] PHP：简单路由
来源：http://dny.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wtu.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://vni.aizwys.cn

composer require twig/twig
来源：http://yjc.cdnleiting.top

[U78] PHP：单元测试
来源：http://auf.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://whg.xuanzx.com

[U79] PHP：静态分析
来源：http://uaj.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://fgh.ivvv.top

[U80] PHP：代码规范修复
来源：http://obj.zhiwuduotai.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wrr.smart0.xyz


<!-- 参考信息 -->