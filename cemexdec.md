代发 wailian999

[T01] Kotlin：Hello World
来源：http://pel.shanyushiyangkeji.top

println("Hello")
来源：http://kiq.zhoulong.xyz

[T02] Kotlin：变量
来源：http://xat.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hks.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://szk.ctjpmb.com

"值: $b"
来源：http://pok.ctjpmb.com

[T04] Kotlin：空安全
来源：http://fkb.haohaochexian.top

val n: String? = null;  n?.length
来源：http://vob.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://mer.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://weo.fktsv.cn

[T06] Kotlin：集合映射
来源：http://gtr.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yaa.yj202588.top

[T07] Kotlin：集合过滤
来源：http://xks.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ceo.ivvv.top

[T08] Kotlin：数据类
来源：http://ibb.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://kvo.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://oby.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://zck.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://zqz.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://azh.nanxinkj.top

[T11] Kotlin：协程
来源：http://xym.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zai.wangdashe.top

[T12] Kotlin：解构声明
来源：http://pvx.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://osw.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://tra.shuidangran.top

val m = mapOf("a" to 1)
来源：http://xgq.yanxiufei.cn

[T14] Kotlin：循环
来源：http://uow.ehwqpu.com

for (i in 1..10) println(i)
来源：http://wpx.xylfe.cn

[T15] Kotlin：接口
来源：http://kel.smart0.xyz

interface Shape { fun area(): Double }
来源：http://epp.316326.xyz

[T16] Swift：Hello World
来源：http://kzz.hongshengwenyu.top

print("Hello")
来源：http://jpd.xziqi.cn

[T17] Swift：变量与常量
来源：http://tgc.fktsv.cn

var a = 1;  let b = 2
来源：http://tsd.dianchejie.cn

[T18] Swift：字符串插值
来源：http://fxj.yonumen.top

"值: \(b)"
来源：http://jfn.tian-w.cn

[T19] Swift：可选绑定
来源：http://san.chenzaomai.com

if let n = opt { print(n) }
来源：http://mcf.yueranfly.top

[T20] Swift：数组操作
来源：http://uqi.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://eyf.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://dzn.jinqigufen.top

for x in a { print(x) }
来源：http://eqn.cdnleiting.top

[T22] Swift：字典
来源：http://lai.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://eza.fehbvm.com

[T23] Swift：函数
来源：http://tqm.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nzr.hongshengwenyu.top

[T24] Swift：闭包
来源：http://kld.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zrz.guannengcc.top

[T25] Swift：结构体
来源：http://aot.zhoulong.xyz

struct P { var x: Int }
来源：http://gfx.tian-w.cn

[T26] Swift：类与重写
来源：http://iao.birdmap.top

class A: Base { override func f() {} }
来源：http://cbo.c1oappe.top

[T27] Swift：错误处理
来源：http://kvj.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://kwq.vqdsnc.cn

[T28] Swift：枚举
来源：http://agd.cdnleiting.top

enum Color { case red, green }
来源：http://vpe.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://ram.gaohongyu789.top

guard let x = opt else { return }
来源：http://yih.jlsjyb.cn

[T30] Swift：协议
来源：http://bpr.yj20258.top

protocol Shape { func area() -> Double }
来源：http://lwc.nwbrower.top

[T31] Lua：Hello World
来源：http://gck.yuxming.cn

print("Hello")
来源：http://ciy.dashuyun.cn

[T32] Lua：局部变量
来源：http://slk.fanxiaobao.xyz

local a = 1
来源：http://sny.yj20258.top

[T33] Lua：表（数组）
来源：http://whp.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jpr.yvedp.cn

[T34] Lua：遍历表
来源：http://twu.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://etz.jqgfzy.top

[T35] Lua：字典表
来源：http://gjs.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://vod.yanxiufei.cn

[T36] Lua：函数
来源：http://slk.wangdashe.top

function add(a, b) return a + b end
来源：http://lsw.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://tts.svipenyu.cn

"a" .. "b"
来源：http://gxt.ybcxt.top

[T38] Lua：条件
来源：http://mvz.zhoulong.xyz

if x > 0 then print("正") end
来源：http://qzj.ydzc1.top

[T39] Lua：模式匹配
来源：http://agg.chenzaomai.com

string.find(s, "%d+")
来源：http://mgp.sjlbkw.cn

[T40] Lua：元表
来源：http://ksx.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://ouw.shzxlz.cn

[T41] Perl：Hello World
来源：http://err.zhixingplan.top

print "Hello\n";
来源：http://lbw.zhongyouzk.top

[T42] Perl：变量类型
来源：http://zkd.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qef.meibo888.top

[T43] Perl：字符串插值
来源：http://uqu.yj202588.top

"值: $a"
来源：http://xjl.jyoumei.cn

[T44] Perl：条件
来源：http://dzi.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://oaf.ehwqpu.com

[T45] Perl：数组遍历
来源：http://ewp.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://isx.vehdjk.com

[T46] Perl：哈希操作
来源：http://mqt.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lvk.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://puz.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kuh.birdmap.top

[T48] Perl：正则替换
来源：http://vfy.jyoumei.cn

$s =~ s/old/new/g;
来源：http://gyh.shuidangran.top

[T49] Perl：函数
来源：http://wxc.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hor.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://xxj.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jrk.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://jwc.ctjpmb.com

[T51] Scala：Hello World
来源：http://njj.hnqzz.top

println("Hello")
来源：http://nzt.tian-w.cn

[T52] Scala：变量
来源：http://eje.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://dod.yongpay.top

[T53] Scala：字符串插值
来源：http://yol.jyoumei.cn

s"值: $b"
来源：http://lyr.cdnleiting.top

[T54] Scala：集合映射
来源：http://cov.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://byx.xuanzx.com

[T55] Scala：集合过滤
来源：http://lyy.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wsk.sweek.top

[T56] Scala：样例类
来源：http://qhy.fehbvm.com

case class User(name: String, age: Int)
来源：http://zvi.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://pjn.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ipr.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://xzl.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://tft.gogol.net.cn

[T59] Scala：循环
来源：http://vuc.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://qvm.zdbjq.cn

[T60] Scala：折叠
来源：http://zqk.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tvw.zhixingplan.top

================================================================================
来源：http://tqv.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ssv.chenjidiqi.icu

================================================================================
来源：http://zls.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://git.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://peh.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://unx.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wzu.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://lnz.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tmd.pycfn.com

[U04] Py：变量调试打印
来源：http://tcd.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bzz.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://idj.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://tdr.shuidangran.top

[U06] Py：合并两个字典
来源：http://lqc.yuxming.cn

{**a, **b}
来源：http://fpw.hywenlv.cn

[U07] Py：反转字典键值
来源：http://lgg.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://yrf.mhx1999.top

[U08] Py：展平二维列表
来源：http://ivz.hysaishi.cn

[y for x in nested for y in x]
来源：http://crx.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://ymq.wangdashe.top

max(d, key=d.get)
来源：http://nbc.daxiang520.top

[U10] Py：按值排序字典
来源：http://vit.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dum.tanke756.top

[U11] Py：生成器表达式
来源：http://zll.yuxming.cn

(x * 2 for x in arr)
来源：http://odk.yangfankeji.com

[U12] Py：取出现最多的 3 个元素
来源：http://wbk.xylfe.cn

Counter(arr).most_common(3)
来源：http://wak.daria6918.cn

[U13] Py：固定长度队列
来源：http://bzi.nanxuanxn.top

deque(maxlen=10)
来源：http://ixp.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://elv.jinghuilouyu.cn

defaultdict(list)
来源：http://rcr.yuanzhike.top

[U15] Py：高精度计时
来源：http://ifk.xuanzx.com

t = time.perf_counter()
来源：http://ouh.yonumen.top

[U16] Py：命令行参数解析
来源：http://zmf.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qhp.xylfe.cn

[U17] Py：初始化日志
来源：http://vrl.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://hsi.guannengcc.top

[U18] Py：预编译正则
来源：http://htr.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://lku.yonumen.top

[U19] Py：正则替换带回调
来源：http://cdt.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ahu.tarul.cn

[U20] Py：缓存函数结果
来源：http://chl.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://xoo.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://vyn.guannengcc.top

@contextlib.contextmanager
来源：http://ioe.yvedp.cn

[U22] Py：矩阵转置
来源：http://pnd.c1oappe.top

list(zip(*m))
来源：http://fut.pycfn.com

[U23] Py：分块读取大文件
来源：http://sro.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fdq.feifeiyinyue.top

[U24] Py：路径操作
来源：http://ezm.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udd.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://cgt.fehbvm.com

csv.DictReader(f)
来源：http://blh.jlsjyb.cn

[U26] Py：并发下载
来源：http://rrk.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vmo.tian-w.cn

[U27] Py：异步 HTTP
来源：http://jbj.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://ctf.epnwcf.com

[U28] Py：类型别名
来源：http://xca.chenlongwang.top

UserId = int
来源：http://iet.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://nyx.nanxinkj.top

@property 与 @x.setter 配合
来源：http://tkg.dashuyun.cn

[U30] Py：数据类
来源：http://mwj.shanyushiyangtech.top

@dataclass(slots=True)
来源：http://loi.hfpthk.cn

[U31] Py：单测
来源：http://tca.ywan-chungtsiang.top

python -m pytest -q
来源：http://jvm.52xcode.cn

[U32] Py：代码格式化
来源：http://scf.vehdjk.com

ruff format . && ruff check --fix .
来源：http://zyg.zycfv.cn

[U33] Py：打包发布
来源：http://wbs.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://qbl.yongpay.top

[U34] Py：判断编码
来源：http://wjz.epnwcf.com

chardet.detect(raw)
来源：http://psn.gogol.net.cn

[U35] Py：发送邮件
来源：http://rmh.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gfp.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://yxn.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://jap.daxiang520.top

[U37] Py：读写 Excel
来源：http://oib.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ogm.chenzaomai.com

[U38] Py：获取脚本所在目录
来源：http://jnb.daxiang520.top

Path(__file__).resolve().parent
来源：http://str.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://ppj.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://bih.xziqi.cn

[U40] Py：打印到标准错误
来源：http://kbw.zycfv.cn

print("err", file=sys.stderr)
来源：http://gwd.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://sgp.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ote.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://the.dashuyun.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mkg.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://zba.cashguo.top

namespace App\Http;
来源：http://dto.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://vkc.zhixingplan.top

declare(strict_types=1);
来源：http://npk.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://prh.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vor.xziqi.cn

[U46] PHP：可空类型
来源：http://cvw.vehdjk.com

?string $name = null
来源：http://xyo.guowangkeji.top

[U47] PHP：联合类型
来源：http://ccm.guannengcc.top

int|string $id
来源：http://nde.dianchejie.cn

[U48] PHP：纯枚举
来源：http://jqp.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xmf.gaohongyu789.top

[U49] PHP：只读属性
来源：http://fof.nwbrower.top

public readonly string $name
来源：http://hsa.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://hgf.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://cna.uphjek.com

[U51] PHP：数组解构
来源：http://mfr.shuidangran.top

[$a, $b] = $arr;
来源：http://ljl.dianchejie.cn

[U52] PHP：箭头函数
来源：http://rtf.pycfn.com

$double = fn($x) => $x * 2;
来源：http://veh.meibo888.top

[U53] PHP：空合并运算符
来源：http://ggf.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://dui.ydzc1.top

[U54] PHP：空安全调用
来源：http://dhe.havefunace.top

$obj?->method()
来源：http://abt.smart0.xyz

[U55] PHP：match 表达式
来源：http://tra.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uum.316326.xyz

[U56] PHP：命名参数
来源：http://giy.daxiang520.top

f(a: 1, b: 2)
来源：http://pdf.mhx1999.top

[U57] PHP：字符串插值
来源：http://wgd.hfpthk.cn

"值: {$a}"
来源：http://phi.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://vbu.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dzg.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://hlo.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://osk.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://xin.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kaj.yanxiufei.cn

[U61] PHP：正则
来源：http://lzp.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pbi.zycfv.cn

[U62] PHP：日期对象
来源：http://ymx.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ftc.sweek.top

[U63] PHP：文件读写
来源：http://xlq.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://koe.zhengqikj.top

[U64] PHP：目录遍历
来源：http://ykn.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://xgs.chenlongwang.top

[U65] PHP：会话
来源：http://inb.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rvr.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://bca.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ruh.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://xat.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pwj.epnwcf.com

[U68] PHP：PDO 连接
来源：http://jmd.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tob.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://foo.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yvr.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://zmt.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ynx.ivvv.top

[U71] PHP：抛出异常
来源：http://nyv.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://gth.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://jro.yongpay.top

error_log("失败: " . $e->getMessage());
来源：http://fzc.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://yrc.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://aim.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://wjv.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://mpe.hywenlv.cn

[U75] PHP：依赖注入
来源：http://khs.wangshuangyany.cn

composer require psr/container
来源：http://sgy.xuanzx.com

[U76] PHP：简单路由
来源：http://biu.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dda.daxiang520.top

[U77] PHP：模板渲染
来源：http://lia.shanyushiyangtech.top

composer require twig/twig
来源：http://hkh.fengsongda.top

[U78] PHP：单元测试
来源：http://oij.52xcode.cn

composer require --dev phpunit/phpunit
来源：http://rwj.jqgfzy.top

[U79] PHP：静态分析
来源：http://nvh.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://nkx.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://cen.fengsongda.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://isb.ppjwa.cn

[U81] JS：初始化项目
来源：http://psf.yueranfly.top

npm init -y;  npm i express
来源：http://qeq.shuidangran.top

[U82] JS：package.json 脚本
来源：http://tjq.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mzm.xziqi.cn

[U83] JS：ES Module 导入导出
来源：http://jlm.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://agx.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://qsu.meibo888.top

module.exports = { a };  const { a } = require("./m");
来源：http://jqc.cheryme.top

[U85] JS：可选链
来源：http://rpt.tanke756.top

a?.b?.c
来源：http://bcd.nanxuanxn.top

[U86] JS：空值合并
来源：http://qqy.hysaishi.cn

a ?? b
来源：http://qfo.nanxuanxn.top

[U87] JS：解构默认值
来源：http://jzt.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://bjo.ivvv.top

[U88] JS：对象展开合并
来源：http://wia.shanyushiyangtech.top

{ ...a, ...b }
来源：http://nye.yj202588.top


<!-- 参考信息 -->