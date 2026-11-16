代发 wailian999

[T03] Kotlin：字符串模板
来源：http://ymh.cqqwz.cn

"值: $b"
来源：http://roi.aizwys.cn

[T04] Kotlin：空安全
来源：http://kax.havefunace.top

val n: String? = null;  n?.length
来源：http://vtv.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://hqo.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npl.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://bzj.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ofw.uphjek.com

[T07] Kotlin：集合过滤
来源：http://dtt.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nee.chenzaomai.com

[T08] Kotlin：数据类
来源：http://uoh.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://qfz.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://vfm.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://rln.fzhhl.top

[T10] Kotlin：默认参数
来源：http://spu.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bxl.cdnleiting.top

[T11] Kotlin：协程
来源：http://qxq.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ohd.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://vzo.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://tix.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://oeg.daria6918.cn

val m = mapOf("a" to 1)
来源：http://auy.hnqzz.top

[T14] Kotlin：循环
来源：http://dqq.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://bby.yuanzhike.top

[T15] Kotlin：接口
来源：http://qdb.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://hsp.andypj.xyz

[T16] Swift：Hello World
来源：http://bol.0kj1m.cn

print("Hello")
来源：http://qoj.birdmap.top

[T17] Swift：变量与常量
来源：http://dgd.daxiang520.top

var a = 1;  let b = 2
来源：http://sea.jiagoushi.top

[T18] Swift：字符串插值
来源：http://glw.zhaomingkeji.xyz

"值: \(b)"
来源：http://hpm.ctjpmb.com

[T19] Swift：可选绑定
来源：http://vli.zhengqikj.top

if let n = opt { print(n) }
来源：http://hdj.hnqzz.top

[T20] Swift：数组操作
来源：http://bym.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zxt.yuxming.cn

[T21] Swift：遍历
来源：http://tqc.jqgufenzy.top

for x in a { print(x) }
来源：http://axd.haohaochexian.top

[T22] Swift：字典
来源：http://mep.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://udq.0kj1m.cn

[T23] Swift：函数
来源：http://zqo.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cbb.tanke756.top

[T24] Swift：闭包
来源：http://tzg.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://thg.sjlbkw.cn

[T25] Swift：结构体
来源：http://zsw.chenlongwang.top

struct P { var x: Int }
来源：http://vxu.nanxuanxn.top

[T26] Swift：类与重写
来源：http://hvv.mhx1999.top

class A: Base { override func f() {} }
来源：http://ebw.hfpthk.cn

[T27] Swift：错误处理
来源：http://jsb.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://lhj.xziqi.cn

[T28] Swift：枚举
来源：http://xrd.hcnkem.com

enum Color { case red, green }
来源：http://vrp.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://kyi.vqdsnc.cn

guard let x = opt else { return }
来源：http://ykg.wangdashe.top

[T30] Swift：协议
来源：http://ojz.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://bfz.daria6918.cn

[T31] Lua：Hello World
来源：http://qim.zhongyouzk.top

print("Hello")
来源：http://xxc.jianghu66.top

[T32] Lua：局部变量
来源：http://knj.shzxlz.cn

local a = 1
来源：http://ghz.sweek.top

[T33] Lua：表（数组）
来源：http://uph.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hrv.yuanzhike.top

[T34] Lua：遍历表
来源：http://ppp.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oxz.zdbjq.cn

[T35] Lua：字典表
来源：http://fpg.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://qwy.sysykeji.top

[T36] Lua：函数
来源：http://nng.52xcode.cn

function add(a, b) return a + b end
来源：http://qlj.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://jfc.gogol.net.cn

"a" .. "b"
来源：http://qkm.havefunace.top

[T38] Lua：条件
来源：http://jpa.shzxlz.cn

if x > 0 then print("正") end
来源：http://xfw.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://rsm.chenjidiqi.icu

string.find(s, "%d+")
来源：http://gje.yvedp.cn

[T40] Lua：元表
来源：http://cmu.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://bql.vehdjk.com

[T41] Perl：Hello World
来源：http://htd.zhiwuduotai.top

print "Hello\n";
来源：http://zyt.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://aub.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzg.nwbrower.top

[T43] Perl：字符串插值
来源：http://ayu.ydjk.org.cn

"值: $a"
来源：http://rwi.jiagoushi.top

[T44] Perl：条件
来源：http://xzn.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://xlu.chenlongwang.top

[T45] Perl：数组遍历
来源：http://xys.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://fcy.ivvv.top

[T46] Perl：哈希操作
来源：http://icz.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fcj.jiagoushi.top

[T47] Perl：正则捕获
来源：http://ypv.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://exk.ydzc1.top

[T48] Perl：正则替换
来源：http://kph.52xcode.cn

$s =~ s/old/new/g;
来源：http://mcl.jqgufenzy.top

[T49] Perl：函数
来源：http://pid.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://osz.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://jdw.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ayo.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://jgf.dianchejie.cn

[T51] Scala：Hello World
来源：http://tjo.fzhhl.top

println("Hello")
来源：http://ugp.yuanzhike.top

[T52] Scala：变量
来源：http://vqc.yj20258888.top

val a = 1;  var b = 2
来源：http://fbb.yj20258888.top

[T53] Scala：字符串插值
来源：http://rdr.vqdsnc.cn

s"值: $b"
来源：http://vkw.yvedp.cn

[T54] Scala：集合映射
来源：http://zew.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://lvx.gzhubu.top

[T55] Scala：集合过滤
来源：http://qld.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://csp.aibaodan.cn

[T56] Scala：样例类
来源：http://ntt.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://ekn.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://vmz.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qvs.yueranfly.top

[T58] Scala：函数定义
来源：http://ssc.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lzg.guannengcc.top

[T59] Scala：循环
来源：http://mkc.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://gwk.cheryme.top

[T60] Scala：折叠
来源：http://qvl.yueranfly.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sbz.cheryme.top

================================================================================
来源：http://mvl.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrw.bbcook.cn

================================================================================
来源：http://zxm.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://cqu.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://nlt.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://kyk.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://art.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://rsd.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://cvx.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://fsg.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mfp.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://ygx.tian-w.cn

list(dict.fromkeys(arr))
来源：http://cxt.cucudq.cn

[U06] Py：合并两个字典
来源：http://ozt.zhengqikj.top

{**a, **b}
来源：http://bze.fktsv.cn

[U07] Py：反转字典键值
来源：http://qmf.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://fwv.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://iis.ehwqpu.com

[y for x in nested for y in x]
来源：http://lof.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://vpd.snrcjt.cn

max(d, key=d.get)
来源：http://hsv.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://xgk.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yws.jqgfzy.top

[U11] Py：生成器表达式
来源：http://pno.cashguo.top

(x * 2 for x in arr)
来源：http://nyd.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://frr.cqqwz.cn

Counter(arr).most_common(3)
来源：http://ace.fehbvm.com

[U13] Py：固定长度队列
来源：http://tnw.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://ynn.cheryme.top

[U14] Py：分组收集到列表
来源：http://ujo.zhoulong.xyz

defaultdict(list)
来源：http://gwa.wangdashe.top

[U15] Py：高精度计时
来源：http://dsk.chenzaomai.com

t = time.perf_counter()
来源：http://mus.fengsongda.top

[U16] Py：命令行参数解析
来源：http://jbo.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ueg.meibo888.top

[U17] Py：初始化日志
来源：http://dhv.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://zrz.jinghuilouyu.cn

[U18] Py：预编译正则
来源：http://bjk.ybcxt.top

pat = re.compile(r"\d+")
来源：http://kkz.vehdjk.com

[U19] Py：正则替换带回调
来源：http://rqy.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jht.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://ssv.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://jxn.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://mnk.nanxinkj.top

@contextlib.contextmanager
来源：http://lom.jinqigufen.top

[U22] Py：矩阵转置
来源：http://hdq.ydjk.org.cn

list(zip(*m))
来源：http://hug.shuidangran.top

[U23] Py：分块读取大文件
来源：http://ahx.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sgz.cheryme.top

[U24] Py：路径操作
来源：http://rcb.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mkf.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://qjw.xziqi.cn

csv.DictReader(f)
来源：http://qcg.yonumen.top

[U26] Py：并发下载
来源：http://rmh.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sfl.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://vzw.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://pio.dianchejie.cn

[U28] Py：类型别名
来源：http://fwz.hcnkem.com

UserId = int
来源：http://nfw.hammf.cn

[U29] Py：属性校验
来源：http://pdr.chenlongwang.top

@property 与 @x.setter 配合
来源：http://zyp.bjfxy.top

[U30] Py：数据类
来源：http://swm.dashuyun.cn

@dataclass(slots=True)
来源：http://rbg.zhengqikj.top

[U31] Py：单测
来源：http://tmm.gotoacloud.top

python -m pytest -q
来源：http://dhf.shuidangran.top

[U32] Py：代码格式化
来源：http://hcl.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://lga.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://owt.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://kjz.zhoulong.xyz

[U34] Py：判断编码
来源：http://yaz.ctjpmb.com

chardet.detect(raw)
来源：http://rse.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://bvl.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xjo.xuanzx.com

[U36] Py：定时任务
来源：http://ymf.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://yky.havefunace.top

[U37] Py：读写 Excel
来源：http://qnk.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://mmq.smart0.xyz

[U38] Py：获取脚本所在目录
来源：http://gtx.hammf.cn

Path(__file__).resolve().parent
来源：http://ife.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://mti.chenlongwang.top

sys.stdout.isatty()
来源：http://cmc.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://vbz.jlsjyb.cn

print("err", file=sys.stderr)
来源：http://biq.sufxvd.cn

[U41] PHP：初始化 Composer 项目
来源：http://igd.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gpd.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://gwl.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zyt.bjfxy.top

[U43] PHP：声明命名空间
来源：http://wra.ehwqpu.com

namespace App\Http;
来源：http://tkv.hcnkem.com

[U44] PHP：开启严格类型
来源：http://vdb.haohaochexian.top

declare(strict_types=1);
来源：http://ybl.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://smg.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bzd.jyoumei.cn

[U46] PHP：可空类型
来源：http://kvl.ehwqpu.com

?string $name = null
来源：http://rzq.zhixingplan.top

[U47] PHP：联合类型
来源：http://gwk.hfpthk.cn

int|string $id
来源：http://jyl.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://oik.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tii.xuanzx.com

[U49] PHP：只读属性
来源：http://rwt.ivvv.top

public readonly string $name
来源：http://uei.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://kux.ppjwa.cn

public function __construct(private int $id) {}
来源：http://jro.svipenyu.cn

[U51] PHP：数组解构
来源：http://pkd.ybcxt.top

[$a, $b] = $arr;
来源：http://tgy.zhixingplan.top

[U52] PHP：箭头函数
来源：http://mxx.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://dms.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://bad.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://hfe.bbcook.cn

[U54] PHP：空安全调用
来源：http://nrc.fengsongda.top

$obj?->method()
来源：http://yxj.jinghuilouyu.cn

[U55] PHP：match 表达式
来源：http://hcm.hammf.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tnt.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://opp.52xcode.cn

f(a: 1, b: 2)
来源：http://gtv.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://fcr.mhx1999.top

"值: {$a}"
来源：http://lrc.iojbl.cn

[U58] PHP：数组三件套
来源：http://dyw.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zap.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://pcb.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://diz.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://gib.gogol.net.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jaw.hysaishi.cn

[U61] PHP：正则
来源：http://iob.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hbg.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://kej.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bne.yuanzhike.top

[U63] PHP：文件读写
来源：http://rci.hysaishi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ijx.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://ndm.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://eig.hongshengwenyu.top

[U65] PHP：会话
来源：http://vhy.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://rse.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://csk.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jad.xziqi.cn

[U67] PHP：处理文件上传
来源：http://yck.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tgl.dashuyun.cn

[U68] PHP：PDO 连接
来源：http://qjb.jqgufenzy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qmo.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://xgo.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bxy.bbcook.cn

[U70] PHP：PDO 事务
来源：http://lyr.jyoumei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ced.meibo888.top

[U71] PHP：抛出异常
来源：http://llc.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://sac.jianghu66.top

[U72] PHP：写错误日志
来源：http://sfy.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://kph.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://zcy.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://bli.yfazqb.com

[U74] PHP：读取环境变量
来源：http://rzv.shuidangran.top

getenv("APP_ENV") ?: "production"
来源：http://xia.zhengqikj.top

[U75] PHP：依赖注入
来源：http://lrb.haohaochexian.top

composer require psr/container
来源：http://yut.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://cfx.guannengcc.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eup.yuxming.cn

[U77] PHP：模板渲染
来源：http://ogk.meibo888.top

composer require twig/twig
来源：http://yep.hcnkem.com

[U78] PHP：单元测试
来源：http://ddd.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://zix.gotoacloud.top

[U79] PHP：静态分析
来源：http://quz.fzhhl.top

composer require --dev phpstan/phpstan
来源：http://wjw.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://ytt.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jzz.52xcode.cn

[U81] JS：初始化项目
来源：http://ysi.ctjpmb.com

npm init -y;  npm i express
来源：http://pea.epnwcf.com

[U82] JS：package.json 脚本
来源：http://huo.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nui.cdnleiting.top

[U83] JS：ES Module 导入导出
来源：http://sih.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pny.hnxiangtu.top

[U84] JS：CommonJS 写法
来源：http://amd.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://xvq.yueranfly.top

[U85] JS：可选链
来源：http://imu.shangyingyoupin.top

a?.b?.c
来源：http://pwd.ivvv.top

[U86] JS：空值合并
来源：http://wso.zhiwuduotai.top

a ?? b
来源：http://wfk.cucudq.cn

[U87] JS：解构默认值
来源：http://qwv.yfazqb.com

const { a = 1, b = 2 } = obj;
来源：http://kug.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://fuw.yanxiufei.cn

{ ...a, ...b }
来源：http://ycz.meibo888.top

[U89] JS：数组去重
来源：http://vxx.vqdsnc.cn

[...new Set(arr)]
来源：http://jce.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://yeb.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://qwj.fzhhl.top


<!-- 参考信息 -->