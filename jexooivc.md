代发 wailian999

[T01] Kotlin：Hello World
来源：http://zsg.vqdsnc.cn

println("Hello")
来源：http://byw.tarul.cn

[T02] Kotlin：变量
来源：http://pkl.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zcf.pycfn.com

[T03] Kotlin：字符串模板
来源：http://ppx.jqgufenzy.top

"值: $b"
来源：http://fkk.tianlin.xyz

[T04] Kotlin：空安全
来源：http://ckc.aibaodan.cn

val n: String? = null;  n?.length
来源：http://swz.meibo888.top

[T05] Kotlin：when 表达式
来源：http://aba.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://btt.tanke756.top

[T06] Kotlin：集合映射
来源：http://tvj.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://guo.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://cgd.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pdc.0kj1m.cn

[T08] Kotlin：数据类
来源：http://olc.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://qzx.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://sve.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://zxr.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://vwi.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uwh.svipenyu.cn

[T11] Kotlin：协程
来源：http://ghf.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kfn.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://shw.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://naq.uphjek.com

[T13] Kotlin：只读 Map
来源：http://izn.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://qqd.hesvh.cn

[T14] Kotlin：循环
来源：http://vtf.jqgfzy.top

for (i in 1..10) println(i)
来源：http://hhm.redwolf501.top

[T15] Kotlin：接口
来源：http://ouu.yj20258888.top

interface Shape { fun area(): Double }
来源：http://eni.shuidangran.top

[T16] Swift：Hello World
来源：http://ali.daxiang520.top

print("Hello")
来源：http://faf.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://sai.gzhubu.top

var a = 1;  let b = 2
来源：http://mdj.sysykeji.top

[T18] Swift：字符串插值
来源：http://kai.zycfv.cn

"值: \(b)"
来源：http://cga.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://qbl.fktsv.cn

if let n = opt { print(n) }
来源：http://rkk.zhengqikj.top

[T20] Swift：数组操作
来源：http://dln.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://lum.iojbl.cn

[T21] Swift：遍历
来源：http://btb.epnwcf.com

for x in a { print(x) }
来源：http://pna.yj202588.top

[T22] Swift：字典
来源：http://kik.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mcn.wangshuangyany.cn

[T23] Swift：函数
来源：http://wqh.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://drc.ydzc1.top

[T24] Swift：闭包
来源：http://sjz.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://aqa.aizwys.cn

[T25] Swift：结构体
来源：http://inr.vehdjk.com

struct P { var x: Int }
来源：http://xpd.kuanghao11.cn

[T26] Swift：类与重写
来源：http://yov.bjfxy.top

class A: Base { override func f() {} }
来源：http://bwt.vqdsnc.cn

[T27] Swift：错误处理
来源：http://cpc.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://cnp.zhoulong.xyz

[T28] Swift：枚举
来源：http://mjj.mhx1999.top

enum Color { case red, green }
来源：http://bwv.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://qpg.vqdsnc.cn

guard let x = opt else { return }
来源：http://qat.vehdjk.com

[T30] Swift：协议
来源：http://fdw.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://bfs.nwbrower.top

[T31] Lua：Hello World
来源：http://fli.guowangkeji.top

print("Hello")
来源：http://tix.zdbjq.cn

[T32] Lua：局部变量
来源：http://nqd.c1oappe.top

local a = 1
来源：http://yyg.cqqwz.cn

[T33] Lua：表（数组）
来源：http://sii.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sak.zdbjq.cn

[T34] Lua：遍历表
来源：http://lhy.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cxw.yj20258888.top

[T35] Lua：字典表
来源：http://oqy.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://rqa.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://vrs.yueranfly.top

function add(a, b) return a + b end
来源：http://ltc.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://npw.wangshuangyany.cn

"a" .. "b"
来源：http://qmt.tanke756.top

[T38] Lua：条件
来源：http://olt.havefunace.top

if x > 0 then print("正") end
来源：http://esf.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://kdc.quarkkingdee.top

string.find(s, "%d+")
来源：http://let.zycfv.cn

[T40] Lua：元表
来源：http://pdb.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://zxs.sweek.top

[T41] Perl：Hello World
来源：http://evf.havefunace.top

print "Hello\n";
来源：http://bkx.ivvv.top

[T42] Perl：变量类型
来源：http://gin.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ozz.yj20258888.top

[T43] Perl：字符串插值
来源：http://asf.shangyingyoupin.top

"值: $a"
来源：http://rtv.uphjek.com

[T44] Perl：条件
来源：http://gvc.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://mcm.xuanzx.com

[T45] Perl：数组遍历
来源：http://rwu.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://rym.yvedp.cn

[T46] Perl：哈希操作
来源：http://hxx.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bcv.52xcode.cn

[T47] Perl：正则捕获
来源：http://pfb.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://syd.ppjwa.cn

[T48] Perl：正则替换
来源：http://tsm.jyoumei.cn

$s =~ s/old/new/g;
来源：http://usu.quarkkingdee.top

[T49] Perl：函数
来源：http://vlu.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://awd.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://fbp.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qfh.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://wyn.jyoumei.cn

[T51] Scala：Hello World
来源：http://ays.bjfxy.top

println("Hello")
来源：http://xov.ctjpmb.com

[T52] Scala：变量
来源：http://xwa.hfpthk.cn

val a = 1;  var b = 2
来源：http://yip.cheryme.top

[T53] Scala：字符串插值
来源：http://znb.snrcjt.cn

s"值: $b"
来源：http://zqy.fehbvm.com

[T54] Scala：集合映射
来源：http://njh.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://qhd.hammf.cn

[T55] Scala：集合过滤
来源：http://tqf.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://xco.jinqigufen.top

[T56] Scala：样例类
来源：http://vpg.sweek.top

case class User(name: String, age: Int)
来源：http://dar.cucudq.cn

[T57] Scala：模式匹配
来源：http://eeh.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xeg.gotoacloud.top

[T58] Scala：函数定义
来源：http://ebk.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nyt.nanxuanxn.top

[T59] Scala：循环
来源：http://jvi.yongpay.top

for (i <- 1 to 10) println(i)
来源：http://hwq.xuetiantiany.cn

[T60] Scala：折叠
来源：http://eeh.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://olh.zdqjudy.top

================================================================================
来源：http://lcw.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rtb.ppjwa.cn

================================================================================
来源：http://mwj.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://vbn.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://rwv.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://epi.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wgt.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://fkq.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vxx.9152youxi.cn

[U04] Py：变量调试打印
来源：http://rav.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ncz.uphjek.com

[U05] Py：列表去重且保序
来源：http://spr.fehbvm.com

list(dict.fromkeys(arr))
来源：http://eyt.vehdjk.com

[U06] Py：合并两个字典
来源：http://lxh.shzxlz.cn

{**a, **b}
来源：http://row.meibo888.top

[U07] Py：反转字典键值
来源：http://bxo.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://igb.shuidangran.top

[U08] Py：展平二维列表
来源：http://keu.guannengcc.top

[y for x in nested for y in x]
来源：http://tjo.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://uvg.feifeiyinyue.top

max(d, key=d.get)
来源：http://jfe.cucudq.cn

[U10] Py：按值排序字典
来源：http://edd.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wwt.ydzc1.top

[U11] Py：生成器表达式
来源：http://qnz.andypj.xyz

(x * 2 for x in arr)
来源：http://ujx.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://evu.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://xnj.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://cfp.zhongyouzk.top

deque(maxlen=10)
来源：http://ggu.meibo888.top

[U14] Py：分组收集到列表
来源：http://uvq.zhoulong.xyz

defaultdict(list)
来源：http://egr.jinqigufen.top

[U15] Py：高精度计时
来源：http://rqv.ybcxt.top

t = time.perf_counter()
来源：http://qph.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://tgy.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hwc.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://fiu.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://ubg.zycfv.cn

[U18] Py：预编译正则
来源：http://div.ybcxt.top

pat = re.compile(r"\d+")
来源：http://npo.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://eyj.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://idw.316326.xyz

[U20] Py：缓存函数结果
来源：http://lzb.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://zfx.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://azh.chenzaomai.com

@contextlib.contextmanager
来源：http://uud.ctjpmb.com

[U22] Py：矩阵转置
来源：http://fgp.uphjek.com

list(zip(*m))
来源：http://qvq.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://czt.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jce.epnwcf.com

[U24] Py：路径操作
来源：http://pws.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://alg.havefunace.top

[U25] Py：CSV 按字典读
来源：http://lli.meibo888.top

csv.DictReader(f)
来源：http://nud.chenlongwang.top

[U26] Py：并发下载
来源：http://lzl.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zfk.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://zfc.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://jnd.fehbvm.com

[U28] Py：类型别名
来源：http://ect.cqqwz.cn

UserId = int
来源：http://kbx.redwolf501.top

[U29] Py：属性校验
来源：http://dtl.sxryk.cn

@property 与 @x.setter 配合
来源：http://jhg.52xcode.cn

[U30] Py：数据类
来源：http://pdr.snrcjt.cn

@dataclass(slots=True)
来源：http://gzy.jianghu66.top

[U31] Py：单测
来源：http://ons.ehwqpu.com

python -m pytest -q
来源：http://jtb.yvedp.cn

[U32] Py：代码格式化
来源：http://tmu.meibo888.top

ruff format . && ruff check --fix .
来源：http://qru.hnqzz.top

[U33] Py：打包发布
来源：http://urs.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://whv.zhoulong.xyz

[U34] Py：判断编码
来源：http://xpv.pycfn.com

chardet.detect(raw)
来源：http://bkp.yanxiufei.cn

[U35] Py：发送邮件
来源：http://tpd.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zqb.xziqi.cn

[U36] Py：定时任务
来源：http://yvp.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://zmz.hcnkem.com

[U37] Py：读写 Excel
来源：http://itz.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://sgt.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://gmw.yj20258888.top

Path(__file__).resolve().parent
来源：http://ntr.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://nfx.nanxuanxn.top

sys.stdout.isatty()
来源：http://mnx.havefunace.top

[U40] Py：打印到标准错误
来源：http://uvw.fzhhl.top

print("err", file=sys.stderr)
来源：http://qpp.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://bzu.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://uno.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://jzi.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wqo.c1oappe.top

[U43] PHP：声明命名空间
来源：http://mgy.snrcjt.cn

namespace App\Http;
来源：http://iuk.redwolf501.top

[U44] PHP：开启严格类型
来源：http://gub.smart0.xyz

declare(strict_types=1);
来源：http://ixl.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://vip.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tzd.zhongyouzk.top

[U46] PHP：可空类型
来源：http://fwv.shuidangran.top

?string $name = null
来源：http://jda.sjlbkw.cn

[U47] PHP：联合类型
来源：http://eor.ctjpmb.com

int|string $id
来源：http://eix.nwbrower.top

[U48] PHP：纯枚举
来源：http://yjb.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://agm.9152youxi.cn

[U49] PHP：只读属性
来源：http://mfr.zhixingplan.top

public readonly string $name
来源：http://vrw.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://xvb.uphjek.com

public function __construct(private int $id) {}
来源：http://eco.guowangkeji.top

[U51] PHP：数组解构
来源：http://ayy.havefunace.top

[$a, $b] = $arr;
来源：http://khs.nwbrower.top

[U52] PHP：箭头函数
来源：http://xwu.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://yyp.yuxming.cn

[U53] PHP：空合并运算符
来源：http://tyx.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://iqn.ctjpmb.com

[U54] PHP：空安全调用
来源：http://bgk.hcnkem.com

$obj?->method()
来源：http://kov.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://uid.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qdr.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://jui.9152youxi.cn

f(a: 1, b: 2)
来源：http://xif.ehwqpu.com

[U57] PHP：字符串插值
来源：http://wtq.sysykeji.top

"值: {$a}"
来源：http://xkp.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://cwi.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rqy.gzhubu.top

[U59] PHP：自定义排序
来源：http://ahi.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdn.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://lco.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lqk.fengsongda.top

[U61] PHP：正则
来源：http://ugq.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nek.zhengqikj.top

[U62] PHP：日期对象
来源：http://djl.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kgi.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://yss.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yaq.xziqi.cn

[U64] PHP：目录遍历
来源：http://mja.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://jye.zhiwuduotai.top

[U65] PHP：会话
来源：http://qya.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://myh.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://lxj.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ida.xinyue.icu

[U67] PHP：处理文件上传
来源：http://xwa.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ire.gzhubu.top

[U68] PHP：PDO 连接
来源：http://mxb.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://njs.sweek.top

[U69] PHP：PDO 预处理
来源：http://jyp.tanke756.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ibw.316326.xyz

[U70] PHP：PDO 事务
来源：http://vhf.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rsg.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://mnm.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://rbt.fehbvm.com

[U72] PHP：写错误日志
来源：http://nkm.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://rae.kuanghao11.cn

[U73] PHP：读取 ini 配置
来源：http://qvj.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://dqf.xinyue.icu

[U74] PHP：读取环境变量
来源：http://jzf.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://zww.0kj1m.cn

[U75] PHP：依赖注入
来源：http://vvn.svipenyu.cn

composer require psr/container
来源：http://uzq.cdnleiting.top

[U76] PHP：简单路由
来源：http://gwf.9152youxi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uww.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://zik.zycfv.cn

composer require twig/twig
来源：http://uuz.zdbjq.cn

[U78] PHP：单元测试
来源：http://vve.yongpay.top

composer require --dev phpunit/phpunit
来源：http://kek.jqgfzy.top

[U79] PHP：静态分析
来源：http://wio.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://liw.gzhubu.top

[U80] PHP：代码规范修复
来源：http://brb.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kly.sysykeji.top

[U81] JS：初始化项目
来源：http://cab.xinyue.icu

npm init -y;  npm i express
来源：http://htc.hammf.cn

[U82] JS：package.json 脚本
来源：http://mnh.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kvc.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://lym.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uyq.sufxvd.cn

[U84] JS：CommonJS 写法
来源：http://dht.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://tet.fzhhl.top

[U85] JS：可选链
来源：http://cdy.c1oappe.top

a?.b?.c
来源：http://psi.xylfe.cn

[U86] JS：空值合并
来源：http://bhq.mhx1999.top

a ?? b
来源：http://srf.kuanghao11.cn

[U87] JS：解构默认值
来源：http://ktx.shanyushiyangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://dtx.yj202588.top

[U88] JS：对象展开合并
来源：http://dbg.pengpengdd.cyou

{ ...a, ...b }
来源：http://dty.hesvh.cn


<!-- 参考信息 -->