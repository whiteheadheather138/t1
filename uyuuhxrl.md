代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fjw.fengsongda.top

[S55] C++：结构化绑定
来源：http://mhd.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ymv.sufxvd.cn

[S56] C++：optional
来源：http://bxg.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gbd.aibaodan.cn

[S57] C++：编译期常量
来源：http://kus.jianghu66.top

constexpr int N = 10;
来源：http://aku.smart0.xyz

[S58] C++：命名空间
来源：http://wvf.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://tsv.tanke756.top

[S59] C++：静态断言
来源：http://xji.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rex.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://rhs.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://snr.jinghuilouyu.cn

================================================================================
来源：http://oqu.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pyn.kuanghao11.cn

================================================================================
来源：http://nkj.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://voh.zhengqikj.top

println("Hello")
来源：http://jme.zdbjq.cn

[T02] Kotlin：变量
来源：http://pun.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dty.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://kfm.xingfuxueyuan.xyz

"值: $b"
来源：http://fxy.zycfv.cn

[T04] Kotlin：空安全
来源：http://sjq.9152youxi.cn

val n: String? = null;  n?.length
来源：http://vcw.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://wxk.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jdu.havefunace.top

[T06] Kotlin：集合映射
来源：http://owr.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://erq.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://cdc.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vcn.cucudq.cn

[T08] Kotlin：数据类
来源：http://iuo.pycfn.com

data class User(val name: String, val age: Int)
来源：http://odz.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://gah.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://ytt.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://dht.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wnb.shzxlz.cn

[T11] Kotlin：协程
来源：http://zer.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rpm.c1oappe.top

[T12] Kotlin：解构声明
来源：http://oyp.zycfv.cn

val (a, b) = Pair(1, 2)
来源：http://sbp.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://aax.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://riy.yuanzhike.top

[T14] Kotlin：循环
来源：http://gmy.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://hli.tanke756.top

[T15] Kotlin：接口
来源：http://czq.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://dhu.zycfv.cn

[T16] Swift：Hello World
来源：http://pjz.9152youxi.cn

print("Hello")
来源：http://uun.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://oeq.hammf.cn

var a = 1;  let b = 2
来源：http://xte.dianchejie.cn

[T18] Swift：字符串插值
来源：http://qmz.yonumen.top

"值: \(b)"
来源：http://vgc.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://ynp.ydzc1.top

if let n = opt { print(n) }
来源：http://etz.yonumen.top

[T20] Swift：数组操作
来源：http://lod.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lyd.yueranfly.top

[T21] Swift：遍历
来源：http://dfa.jqgfzy.top

for x in a { print(x) }
来源：http://drg.cdnleiting.top

[T22] Swift：字典
来源：http://fll.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://xgi.dashuyun.cn

[T23] Swift：函数
来源：http://dir.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ntf.svipenyu.cn

[T24] Swift：闭包
来源：http://izn.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ics.yj20258.top

[T25] Swift：结构体
来源：http://hou.epnwcf.com

struct P { var x: Int }
来源：http://rye.hnxiangtu.top

[T26] Swift：类与重写
来源：http://uxy.xinyue.icu

class A: Base { override func f() {} }
来源：http://vnf.guowangkeji.top

[T27] Swift：错误处理
来源：http://wbc.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://eok.meibo888.top

[T28] Swift：枚举
来源：http://pnw.vqdsnc.cn

enum Color { case red, green }
来源：http://awr.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://lsh.chenlongwang.top

guard let x = opt else { return }
来源：http://udh.guowangkeji.top

[T30] Swift：协议
来源：http://xof.pycfn.com

protocol Shape { func area() -> Double }
来源：http://foq.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://joy.zhaomingkeji.xyz

print("Hello")
来源：http://cuw.jiagoushi.top

[T32] Lua：局部变量
来源：http://nsz.ybcxt.top

local a = 1
来源：http://rsa.fktsv.cn

[T33] Lua：表（数组）
来源：http://cla.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rsz.cucudq.cn

[T34] Lua：遍历表
来源：http://vkc.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://emp.jiagoushi.top

[T35] Lua：字典表
来源：http://xan.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://cdj.316326.xyz

[T36] Lua：函数
来源：http://xbb.tarul.cn

function add(a, b) return a + b end
来源：http://ezw.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://bgu.yfazqb.com

"a" .. "b"
来源：http://hih.fzhhl.top

[T38] Lua：条件
来源：http://sfb.cucudq.cn

if x > 0 then print("正") end
来源：http://qpm.mhx1999.top

[T39] Lua：模式匹配
来源：http://znk.andypj.xyz

string.find(s, "%d+")
来源：http://wms.shangyingyoupin.top

[T40] Lua：元表
来源：http://uho.cheryme.top

setmetatable({}, { __index = base })
来源：http://ckx.zdqjudy.top

[T41] Perl：Hello World
来源：http://guc.xziqi.cn

print "Hello\n";
来源：http://bfe.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://ubh.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xcc.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://zbl.shanyushiyangkeji.top

"值: $a"
来源：http://axn.zhijiandao.cn

[T44] Perl：条件
来源：http://odh.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://wzi.bbcook.cn

[T45] Perl：数组遍历
来源：http://qie.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://zfn.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://enu.havefunace.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xyp.uphjek.com

[T47] Perl：正则捕获
来源：http://ond.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ucp.nanxinkj.top

[T48] Perl：正则替换
来源：http://pud.uphjek.com

$s =~ s/old/new/g;
来源：http://ipj.52xcode.cn

[T49] Perl：函数
来源：http://lkj.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zec.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://ccg.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gza.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://ust.jiagoushi.top

[T51] Scala：Hello World
来源：http://oit.shangyingyoupin.top

println("Hello")
来源：http://tmv.bjfxy.top

[T52] Scala：变量
来源：http://sjq.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://blx.daxiang520.top

[T53] Scala：字符串插值
来源：http://vit.xinyue.icu

s"值: $b"
来源：http://mbv.dashuyun.cn

[T54] Scala：集合映射
来源：http://lfx.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://pis.xinyue.icu

[T55] Scala：集合过滤
来源：http://hoj.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://yul.yanxiufei.cn

[T56] Scala：样例类
来源：http://fpz.cheryme.top

case class User(name: String, age: Int)
来源：http://rsa.yangfankeji.com

[T57] Scala：模式匹配
来源：http://tac.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jge.zycfv.cn

[T58] Scala：函数定义
来源：http://hob.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vne.pycfn.com

[T59] Scala：循环
来源：http://tts.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://vnh.kuanghao11.cn

[T60] Scala：折叠
来源：http://nwp.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ssh.c1oappe.top

================================================================================
来源：http://xxg.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kaz.yangfankeji.com

================================================================================
来源：http://vku.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://knx.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://elt.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://eis.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewj.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://anw.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pla.hcnkem.com

[U04] Py：变量调试打印
来源：http://vtb.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://svf.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://pbs.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://zuy.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://ctb.hammf.cn

{**a, **b}
来源：http://ddf.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://rok.fktsv.cn

{v: k for k, v in d.items()}
来源：http://gea.sufxvd.cn

[U08] Py：展平二维列表
来源：http://srw.yueranfly.top

[y for x in nested for y in x]
来源：http://ipn.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://kjm.ppjwa.cn

max(d, key=d.get)
来源：http://yzb.tianlin.xyz

[U10] Py：按值排序字典
来源：http://muk.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qpq.xylfe.cn

[U11] Py：生成器表达式
来源：http://cbn.jinyuanbaomall.cn

(x * 2 for x in arr)
来源：http://ors.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://nop.52xcode.cn

Counter(arr).most_common(3)
来源：http://tso.ppjwa.cn

[U13] Py：固定长度队列
来源：http://eki.daxiang520.top

deque(maxlen=10)
来源：http://nso.52xcode.cn

[U14] Py：分组收集到列表
来源：http://lhc.feifeiyinyue.top

defaultdict(list)
来源：http://vxw.c1oappe.top

[U15] Py：高精度计时
来源：http://jvd.epnwcf.com

t = time.perf_counter()
来源：http://zra.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://sge.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fga.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://lvr.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://tvn.tarul.cn

[U18] Py：预编译正则
来源：http://saf.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://eaz.hcnkem.com

[U19] Py：正则替换带回调
来源：http://xst.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cqs.hcnkem.com

[U20] Py：缓存函数结果
来源：http://lof.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://dlx.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://xkv.fzhhl.top

@contextlib.contextmanager
来源：http://drx.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://brx.guowangkeji.top

list(zip(*m))
来源：http://jkj.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://fqa.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zxw.haohaochexian.top

[U24] Py：路径操作
来源：http://pnj.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cdw.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://eoz.chenlongwang.top

csv.DictReader(f)
来源：http://tlh.jianghu66.top

[U26] Py：并发下载
来源：http://uqq.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jnu.zhengqikj.top

[U27] Py：异步 HTTP
来源：http://myw.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://ctf.meibo888.top

[U28] Py：类型别名
来源：http://hta.cheryme.top

UserId = int
来源：http://obl.shuidangran.top

[U29] Py：属性校验
来源：http://hbn.sufxvd.cn

@property 与 @x.setter 配合
来源：http://bjk.daxiang520.top

[U30] Py：数据类
来源：http://vul.hysaishi.cn

@dataclass(slots=True)
来源：http://qsz.tian-w.cn

[U31] Py：单测
来源：http://wjn.shanyushiyangkeji.top

python -m pytest -q
来源：http://jbr.wangdashe.top

[U32] Py：代码格式化
来源：http://bjf.hnqzz.top

ruff format . && ruff check --fix .
来源：http://zyk.zycfv.cn

[U33] Py：打包发布
来源：http://roo.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://ofb.fzhhl.top

[U34] Py：判断编码
来源：http://vdq.tian-w.cn

chardet.detect(raw)
来源：http://lif.chenzaomai.com

[U35] Py：发送邮件
来源：http://vxj.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cxy.0kj1m.cn

[U36] Py：定时任务
来源：http://pln.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://dke.aizwys.cn

[U37] Py：读写 Excel
来源：http://zcl.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://vix.cashguo.top

[U38] Py：获取脚本所在目录
来源：http://des.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://mzx.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://kch.svipenyu.cn

sys.stdout.isatty()
来源：http://ruw.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://pjd.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://luz.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://jmf.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mvp.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ubs.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rji.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://dhg.zhoulong.xyz

namespace App\Http;
来源：http://nqc.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://kdl.gogol.net.cn

declare(strict_types=1);
来源：http://xij.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://fic.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hfz.jlsjyb.cn

[U46] PHP：可空类型
来源：http://wwx.xinyue.icu

?string $name = null
来源：http://wve.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://yzr.yvedp.cn

int|string $id
来源：http://xgj.xinyue.icu

[U48] PHP：纯枚举
来源：http://kns.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohr.zhongyouzk.top

[U49] PHP：只读属性
来源：http://ixf.xingfuxueyuan.xyz

public readonly string $name
来源：http://fst.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://whe.cheryme.top

public function __construct(private int $id) {}
来源：http://wmn.yanxiufei.cn

[U51] PHP：数组解构
来源：http://vdg.meibo888.top

[$a, $b] = $arr;
来源：http://tcb.jiagoushi.top

[U52] PHP：箭头函数
来源：http://fae.ivvv.top

$double = fn($x) => $x * 2;
来源：http://bfs.zhixingplan.top

[U53] PHP：空合并运算符
来源：http://ehg.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://chf.bjfxy.top

[U54] PHP：空安全调用
来源：http://bbh.nanxinkj.top

$obj?->method()
来源：http://taw.dashuyun.cn

[U55] PHP：match 表达式
来源：http://mcf.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kbo.cqqwz.cn

[U56] PHP：命名参数
来源：http://izu.zhongyouzk.top

f(a: 1, b: 2)
来源：http://gwa.aibaodan.cn

[U57] PHP：字符串插值
来源：http://kyb.fengsongda.top

"值: {$a}"
来源：http://qky.jinqigufen.top

[U58] PHP：数组三件套
来源：http://dfw.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vrp.gotoacloud.top

[U59] PHP：自定义排序
来源：http://xxt.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvm.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://sdc.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lrk.tian-w.cn

[U61] PHP：正则
来源：http://xhu.aibaodan.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kgi.9152youxi.cn

[U62] PHP：日期对象
来源：http://fix.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qvk.yvedp.cn

[U63] PHP：文件读写
来源：http://vrh.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vne.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://nla.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://mps.guannengcc.top

[U65] PHP：会话
来源：http://vtz.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xxk.yonumen.top

[U66] PHP：设置 Cookie
来源：http://eud.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xdu.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://pmn.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kmc.guannengcc.top

[U68] PHP：PDO 连接
来源：http://vwg.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pgr.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://ijz.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sri.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://gdu.jinghuilouyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rlo.yvedp.cn

[U71] PHP：抛出异常
来源：http://djn.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://dms.yvedp.cn

[U72] PHP：写错误日志
来源：http://omc.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://ubp.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://ame.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://dsk.shuidangran.top

[U74] PHP：读取环境变量
来源：http://fbx.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://exy.hywenlv.cn

[U75] PHP：依赖注入
来源：http://aic.yj202588.top

composer require psr/container
来源：http://elm.kuanghao11.cn

[U76] PHP：简单路由
来源：http://whh.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qyg.iojbl.cn

[U77] PHP：模板渲染
来源：http://dob.uphjek.com

composer require twig/twig
来源：http://izl.zycfv.cn

[U78] PHP：单元测试
来源：http://rlm.birdmap.top

composer require --dev phpunit/phpunit
来源：http://vcx.zhijiandao.cn

[U79] PHP：静态分析
来源：http://xyi.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://ito.mhx1999.top

[U80] PHP：代码规范修复
来源：http://ntz.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://csa.pycfn.com


<!-- 参考信息 -->