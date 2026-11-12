代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://syz.ydjk.org.cn

================================================================================
来源：http://wfi.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kim.sjlbkw.cn

================================================================================
来源：http://etd.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://eta.redwolf501.top

println("Hello")
来源：http://owp.dashuyun.cn

[T02] Kotlin：变量
来源：http://lvu.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tas.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://tnk.havefunace.top

"值: $b"
来源：http://qiz.hywenlv.cn

[T04] Kotlin：空安全
来源：http://csz.fengsongda.top

val n: String? = null;  n?.length
来源：http://fxc.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://xsy.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ttu.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://fey.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dtb.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://zch.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qsu.shzxlz.cn

[T08] Kotlin：数据类
来源：http://amd.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://wad.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://tvt.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://xli.guannengcc.top

[T10] Kotlin：默认参数
来源：http://roz.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zym.zhengqikj.top

[T11] Kotlin：协程
来源：http://kax.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://mqz.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://zgp.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://sjm.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://wsr.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://gdh.zhoulong.xyz

[T14] Kotlin：循环
来源：http://yav.zhixingplan.top

for (i in 1..10) println(i)
来源：http://fie.gogol.net.cn

[T15] Kotlin：接口
来源：http://quj.cucudq.cn

interface Shape { fun area(): Double }
来源：http://pgq.jinqigfzy.top

[T16] Swift：Hello World
来源：http://opx.ywan-chungtsiang.top

print("Hello")
来源：http://vem.yongpay.top

[T17] Swift：变量与常量
来源：http://acd.snrcjt.cn

var a = 1;  let b = 2
来源：http://qjp.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://fzn.zdbjq.cn

"值: \(b)"
来源：http://fya.zdqjudy.top

[T19] Swift：可选绑定
来源：http://krq.fengsongda.top

if let n = opt { print(n) }
来源：http://wro.0kj1m.cn

[T20] Swift：数组操作
来源：http://qit.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://hht.iojbl.cn

[T21] Swift：遍历
来源：http://mvu.ctjpmb.com

for x in a { print(x) }
来源：http://thu.yongpay.top

[T22] Swift：字典
来源：http://knj.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://xcv.iojbl.cn

[T23] Swift：函数
来源：http://ufj.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ztf.xylfe.cn

[T24] Swift：闭包
来源：http://syb.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://faz.dianchejie.cn

[T25] Swift：结构体
来源：http://nvp.yfazqb.com

struct P { var x: Int }
来源：http://obj.sweek.top

[T26] Swift：类与重写
来源：http://rgy.gotoacloud.top

class A: Base { override func f() {} }
来源：http://nel.yj20258.top

[T27] Swift：错误处理
来源：http://qgq.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://nvo.yueranfly.top

[T28] Swift：枚举
来源：http://xbr.sysykeji.top

enum Color { case red, green }
来源：http://khk.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://cfk.ybcxt.top

guard let x = opt else { return }
来源：http://qbk.jinghuilouyu.cn

[T30] Swift：协议
来源：http://mda.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://evy.yangfankeji.com

[T31] Lua：Hello World
来源：http://ppc.9152youxi.cn

print("Hello")
来源：http://wst.shuidangran.top

[T32] Lua：局部变量
来源：http://fna.0kj1m.cn

local a = 1
来源：http://gmc.redwolf501.top

[T33] Lua：表（数组）
来源：http://rfk.yj20258888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ynr.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://foi.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fdv.guowangkeji.top

[T35] Lua：字典表
来源：http://qhn.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://bkb.yangfankeji.com

[T36] Lua：函数
来源：http://fwk.smart0.xyz

function add(a, b) return a + b end
来源：http://ubs.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://gze.sweek.top

"a" .. "b"
来源：http://bya.feifeiyinyue.top

[T38] Lua：条件
来源：http://wgp.jyoumei.cn

if x > 0 then print("正") end
来源：http://nhl.tian-w.cn

[T39] Lua：模式匹配
来源：http://qgq.zhongyouzk.top

string.find(s, "%d+")
来源：http://bvf.chenzaomai.com

[T40] Lua：元表
来源：http://vfk.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://byy.ybcxt.top

[T41] Perl：Hello World
来源：http://sgr.shanyushiyangtech.top

print "Hello\n";
来源：http://uto.nanxuanxn.top

[T42] Perl：变量类型
来源：http://mgf.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tky.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://utm.shzxlz.cn

"值: $a"
来源：http://vqh.jqgfzy.top

[T44] Perl：条件
来源：http://utw.uphjek.com

if ($a > 0) { print "正"; }
来源：http://fut.ctjpmb.com

[T45] Perl：数组遍历
来源：http://crp.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://auw.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://jbf.fktsv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wok.tianlin.xyz

[T47] Perl：正则捕获
来源：http://fop.zdqjudy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://haw.ydzc1.top

[T48] Perl：正则替换
来源：http://iwr.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://esu.fengsongda.top

[T49] Perl：函数
来源：http://zps.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vkx.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://aiz.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gjr.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://ehd.fengsongda.top

[T51] Scala：Hello World
来源：http://zvm.nanxinkj.top

println("Hello")
来源：http://tfx.cucudq.cn

[T52] Scala：变量
来源：http://qtb.zhengqikj.top

val a = 1;  var b = 2
来源：http://bkf.sysykeji.top

[T53] Scala：字符串插值
来源：http://iuq.yfazqb.com

s"值: $b"
来源：http://lfz.jqgufenzy.top

[T54] Scala：集合映射
来源：http://nyg.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://eew.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://bil.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kdi.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://jyv.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://eka.birdmap.top

[T57] Scala：模式匹配
来源：http://avf.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hql.hammf.cn

[T58] Scala：函数定义
来源：http://iai.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://vtv.yj202588.top

[T59] Scala：循环
来源：http://pnj.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://jsl.kuanghao11.cn

[T60] Scala：折叠
来源：http://vlp.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ylh.mhx1999.top

================================================================================
来源：http://cew.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uka.zdbjq.cn

================================================================================
来源：http://dzh.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://hrz.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fgx.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://qsw.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dis.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://yzu.tanke756.top

from dotenv import load_dotenv; load_dotenv()
来源：http://frp.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://nmb.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qzi.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://omo.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://sbc.xziqi.cn

[U06] Py：合并两个字典
来源：http://cyn.9152youxi.cn

{**a, **b}
来源：http://riq.aibaodan.cn

[U07] Py：反转字典键值
来源：http://ohi.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://ufe.havefunace.top

[U08] Py：展平二维列表
来源：http://eql.jqgufenzy.top

[y for x in nested for y in x]
来源：http://eea.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://gys.yj202588.top

max(d, key=d.get)
来源：http://zyd.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://ubr.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oha.fengsongda.top

[U11] Py：生成器表达式
来源：http://kbr.zhengqikj.top

(x * 2 for x in arr)
来源：http://cnj.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://dcg.hesvh.cn

Counter(arr).most_common(3)
来源：http://yof.iojbl.cn

[U13] Py：固定长度队列
来源：http://oax.cheryme.top

deque(maxlen=10)
来源：http://kxv.fanxiaobao.xyz

[U14] Py：分组收集到列表
来源：http://jul.hesvh.cn

defaultdict(list)
来源：http://ntl.xuanzx.com

[U15] Py：高精度计时
来源：http://ooq.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://dpf.hcnkem.com

[U16] Py：命令行参数解析
来源：http://kda.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qww.hcnkem.com

[U17] Py：初始化日志
来源：http://tns.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://vai.gotoacloud.top

[U18] Py：预编译正则
来源：http://wvs.aizwys.cn

pat = re.compile(r"\d+")
来源：http://nke.ybcxt.top

[U19] Py：正则替换带回调
来源：http://loc.nwbrower.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fzr.xziqi.cn

[U20] Py：缓存函数结果
来源：http://hwj.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://iqg.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://gwl.guannengcc.top

@contextlib.contextmanager
来源：http://cgy.yongpay.top

[U22] Py：矩阵转置
来源：http://tcb.cqqwz.cn

list(zip(*m))
来源：http://aiu.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://qvh.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aby.hongshengwenyu.top

[U24] Py：路径操作
来源：http://wgu.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://orw.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://gkv.ppjwa.cn

csv.DictReader(f)
来源：http://qfu.sweek.top

[U26] Py：并发下载
来源：http://fnm.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yvj.fengsongda.top

[U27] Py：异步 HTTP
来源：http://wbk.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://iqy.hnqzz.top

[U28] Py：类型别名
来源：http://bkg.nanxuanxn.top

UserId = int
来源：http://dbv.aibaodan.cn

[U29] Py：属性校验
来源：http://ekg.yueranfly.top

@property 与 @x.setter 配合
来源：http://jkc.pycfn.com

[U30] Py：数据类
来源：http://mga.zhijiandao.cn

@dataclass(slots=True)
来源：http://vwy.shangyingyoupin.top

[U31] Py：单测
来源：http://xsq.jinghuilouyu.cn

python -m pytest -q
来源：http://zhg.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://bsh.fzhhl.top

ruff format . && ruff check --fix .
来源：http://pyw.quarkkingdee.top

[U33] Py：打包发布
来源：http://bnz.52xcode.cn

python -m build  （依赖 pyproject.toml）
来源：http://nlx.vehdjk.com

[U34] Py：判断编码
来源：http://guc.guowangkeji.top

chardet.detect(raw)
来源：http://rmf.hysaishi.cn

[U35] Py：发送邮件
来源：http://cjt.zhijiandao.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oit.zhixingplan.top

[U36] Py：定时任务
来源：http://vwh.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://lvn.yangfankeji.com

[U37] Py：读写 Excel
来源：http://tbr.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uzk.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://kkc.tian-w.cn

Path(__file__).resolve().parent
来源：http://ovg.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://pvx.ppjwa.cn

sys.stdout.isatty()
来源：http://xlo.jlsjyb.cn

[U40] Py：打印到标准错误
来源：http://gnz.yongpay.top

print("err", file=sys.stderr)
来源：http://qio.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://ray.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ikv.ehwqpu.com

[U42] PHP：PSR-4 自动加载
来源：http://xdg.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vqt.pycfn.com

[U43] PHP：声明命名空间
来源：http://uov.redwolf501.top

namespace App\Http;
来源：http://rhd.cucudq.cn

[U44] PHP：开启严格类型
来源：http://uyo.smart0.xyz

declare(strict_types=1);
来源：http://scf.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://qit.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ovb.52xcode.cn

[U46] PHP：可空类型
来源：http://jym.yonumen.top

?string $name = null
来源：http://oxp.yj20258888.top

[U47] PHP：联合类型
来源：http://qrc.zhijiandao.cn

int|string $id
来源：http://rgn.pycfn.com

[U48] PHP：纯枚举
来源：http://ybd.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kyz.bbcook.cn

[U49] PHP：只读属性
来源：http://ieh.fktsv.cn

public readonly string $name
来源：http://krr.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://njw.chenzaomai.com

public function __construct(private int $id) {}
来源：http://qdf.sysykeji.top

[U51] PHP：数组解构
来源：http://jyx.ctjpmb.com

[$a, $b] = $arr;
来源：http://fzb.hesvh.cn

[U52] PHP：箭头函数
来源：http://hfu.wangdashe.top

$double = fn($x) => $x * 2;
来源：http://yii.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://koe.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://wfi.gzhubu.top

[U54] PHP：空安全调用
来源：http://tdv.pycfn.com

$obj?->method()
来源：http://etm.meibo888.top

[U55] PHP：match 表达式
来源：http://etl.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dtf.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://giz.svipenyu.cn

f(a: 1, b: 2)
来源：http://xya.jianghu66.top

[U57] PHP：字符串插值
来源：http://uhb.jyoumei.cn

"值: {$a}"
来源：http://hso.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://wxl.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://slj.jqgfzy.top

[U59] PHP：自定义排序
来源：http://ugw.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xcs.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://ctb.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tdc.zhoulong.xyz

[U61] PHP：正则
来源：http://dtx.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://raa.ehwqpu.com

[U62] PHP：日期对象
来源：http://nri.yueranfly.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jdz.cheryme.top

[U63] PHP：文件读写
来源：http://diz.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ybb.andypj.xyz

[U64] PHP：目录遍历
来源：http://tru.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://wsn.jinyuanbaomall.cn

[U65] PHP：会话
来源：http://nye.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eaf.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://mtn.chenlongwang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sum.yj20258.top

[U67] PHP：处理文件上传
来源：http://ofx.xinyue.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nke.cashguo.top

[U68] PHP：PDO 连接
来源：http://fwr.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kyn.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://lsb.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tcn.bjfxy.top

[U70] PHP：PDO 事务
来源：http://dtb.guowangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cvd.sysykeji.top

[U71] PHP：抛出异常
来源：http://zxl.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://ucy.aizwys.cn

[U72] PHP：写错误日志
来源：http://ncf.svipenyu.cn

error_log("失败: " . $e->getMessage());
来源：http://yjp.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://hqp.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://dmh.yongpay.top

[U74] PHP：读取环境变量
来源：http://ilh.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://adi.zhengqikj.top

[U75] PHP：依赖注入
来源：http://llp.0kj1m.cn

composer require psr/container
来源：http://swe.zdqjudy.top

[U76] PHP：简单路由
来源：http://uni.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wdt.chenlongwang.top

[U77] PHP：模板渲染
来源：http://nsz.zhixingplan.top

composer require twig/twig
来源：http://jxo.cheryme.top

[U78] PHP：单元测试
来源：http://yao.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://row.yj20258888.top

[U79] PHP：静态分析
来源：http://fan.pycfn.com

composer require --dev phpstan/phpstan
来源：http://mqt.yuxming.cn

[U80] PHP：代码规范修复
来源：http://kyh.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pnk.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://zly.jqgfzy.top

npm init -y;  npm i express
来源：http://sdo.nwbrower.top

[U82] JS：package.json 脚本
来源：http://ihc.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://glj.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://yiq.gzhubu.top

export const a = 1;  import { a } from "./m.js";
来源：http://qnx.ivvv.top

[U84] JS：CommonJS 写法
来源：http://yph.hongshengwenyu.top

module.exports = { a };  const { a } = require("./m");
来源：http://bhq.fzhhl.top

[U85] JS：可选链
来源：http://ljj.guannengcc.top

a?.b?.c
来源：http://jtn.sxryk.cn

[U86] JS：空值合并
来源：http://jbt.kuanghao11.cn

a ?? b
来源：http://agh.yonumen.top


<!-- 参考信息 -->