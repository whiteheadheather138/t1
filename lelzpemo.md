代发 wailian999

[T05] Kotlin：when 表达式
来源：http://gvi.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cwp.xylfe.cn

[T06] Kotlin：集合映射
来源：http://sci.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ynx.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://brm.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://wph.zycfv.cn

[T08] Kotlin：数据类
来源：http://cyc.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://blq.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://lkc.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://edw.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://pss.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sfm.bjfxy.top

[T11] Kotlin：协程
来源：http://hsr.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ywx.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://klp.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://mop.yj20258.top

[T13] Kotlin：只读 Map
来源：http://tpw.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://eer.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://njl.jianghu66.top

for (i in 1..10) println(i)
来源：http://iaz.ppjwa.cn

[T15] Kotlin：接口
来源：http://qar.sysykeji.top

interface Shape { fun area(): Double }
来源：http://unj.snrcjt.cn

[T16] Swift：Hello World
来源：http://jms.jqgfzy.top

print("Hello")
来源：http://vxs.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://qdi.52xcode.cn

var a = 1;  let b = 2
来源：http://zzh.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://gsg.pycfn.com

"值: \(b)"
来源：http://fhg.fktsv.cn

[T19] Swift：可选绑定
来源：http://bxf.sjlbkw.cn

if let n = opt { print(n) }
来源：http://hft.fktsv.cn

[T20] Swift：数组操作
来源：http://tbk.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://pco.jiagoushi.top

[T21] Swift：遍历
来源：http://fqg.sysykeji.top

for x in a { print(x) }
来源：http://icf.aibaodan.cn

[T22] Swift：字典
来源：http://rto.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://yyl.hnxiangtu.top

[T23] Swift：函数
来源：http://wjx.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ftt.jianghu66.top

[T24] Swift：闭包
来源：http://vxm.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zdg.uphjek.com

[T25] Swift：结构体
来源：http://mvm.hysaishi.cn

struct P { var x: Int }
来源：http://ptc.hywenlv.cn

[T26] Swift：类与重写
来源：http://pdy.dashuyun.cn

class A: Base { override func f() {} }
来源：http://qly.yongpay.top

[T27] Swift：错误处理
来源：http://dqu.iojbl.cn

do { try f() } catch { print(error) }
来源：http://llq.jyoumei.cn

[T28] Swift：枚举
来源：http://tht.tianlin.xyz

enum Color { case red, green }
来源：http://vhp.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://scy.yuxming.cn

guard let x = opt else { return }
来源：http://ggs.hnxiangtu.top

[T30] Swift：协议
来源：http://jth.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://pbn.ehwqpu.com

[T31] Lua：Hello World
来源：http://wvt.vehdjk.com

print("Hello")
来源：http://qgn.cheryme.top

[T32] Lua：局部变量
来源：http://yue.fanxiaobao.xyz

local a = 1
来源：http://pik.yongpay.top

[T33] Lua：表（数组）
来源：http://nbi.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://imj.xuanzx.com

[T34] Lua：遍历表
来源：http://fhy.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://veb.ppjwa.cn

[T35] Lua：字典表
来源：http://khn.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://mlh.birdmap.top

[T36] Lua：函数
来源：http://wda.ppjwa.cn

function add(a, b) return a + b end
来源：http://sxw.jianghu66.top

[T37] Lua：字符串拼接
来源：http://ilm.kuanghao11.cn

"a" .. "b"
来源：http://btw.nanxuanxn.top

[T38] Lua：条件
来源：http://dpj.pycfn.com

if x > 0 then print("正") end
来源：http://cbm.hfpthk.cn

[T39] Lua：模式匹配
来源：http://aji.svipenyu.cn

string.find(s, "%d+")
来源：http://mwo.daria6918.cn

[T40] Lua：元表
来源：http://oxm.yonumen.top

setmetatable({}, { __index = base })
来源：http://lav.bjfxy.top

[T41] Perl：Hello World
来源：http://ipv.hnqzz.top

print "Hello\n";
来源：http://obb.cqqwz.cn

[T42] Perl：变量类型
来源：http://gaz.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nsd.fktsv.cn

[T43] Perl：字符串插值
来源：http://hni.tian-w.cn

"值: $a"
来源：http://guv.yj20258.top

[T44] Perl：条件
来源：http://bba.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://eby.fzhhl.top

[T45] Perl：数组遍历
来源：http://lfi.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://nzc.hcnkem.com

[T46] Perl：哈希操作
来源：http://ssm.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oxm.jyoumei.cn

[T47] Perl：正则捕获
来源：http://khx.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://abl.gaohongyu789.top

[T48] Perl：正则替换
来源：http://ezm.fehbvm.com

$s =~ s/old/new/g;
来源：http://uvc.gaohongyu789.top

[T49] Perl：函数
来源：http://jff.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jiw.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://pyz.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jer.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://vqp.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://yhq.xuetiantiany.cn

println("Hello")
来源：http://gcs.0kj1m.cn

[T52] Scala：变量
来源：http://nfi.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://kdl.uphjek.com

[T53] Scala：字符串插值
来源：http://hts.cqqwz.cn

s"值: $b"
来源：http://vpe.ydjk.org.cn

[T54] Scala：集合映射
来源：http://vep.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://rcy.hammf.cn

[T55] Scala：集合过滤
来源：http://lts.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://sut.c1oappe.top

[T56] Scala：样例类
来源：http://rgo.ivvv.top

case class User(name: String, age: Int)
来源：http://vws.fzhhl.top

[T57] Scala：模式匹配
来源：http://lbn.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lfi.fehbvm.com

[T58] Scala：函数定义
来源：http://rwe.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://kwm.xuanzx.com

[T59] Scala：循环
来源：http://ifn.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://foz.birdmap.top

[T60] Scala：折叠
来源：http://sws.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rna.chenlongwang.top

================================================================================
来源：http://ztz.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xcy.nwbrower.top

================================================================================
来源：http://bdp.yuxming.cn

[U01] Py：创建虚拟环境
来源：http://iib.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vkx.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://ulv.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://efa.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://kli.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bta.guowangkeji.top

[U04] Py：变量调试打印
来源：http://jlp.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://biz.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://zer.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://vae.sysykeji.top

[U06] Py：合并两个字典
来源：http://kuy.wangshuangyany.cn

{**a, **b}
来源：http://fui.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://wax.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://ixe.xziqi.cn

[U08] Py：展平二维列表
来源：http://enw.vqdsnc.cn

[y for x in nested for y in x]
来源：http://rpn.nanxinkj.top

[U09] Py：字典取最大值的键
来源：http://jvi.havefunace.top

max(d, key=d.get)
来源：http://znv.aizwys.cn

[U10] Py：按值排序字典
来源：http://buw.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fro.hysaishi.cn

[U11] Py：生成器表达式
来源：http://uoe.0kj1m.cn

(x * 2 for x in arr)
来源：http://luq.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://opk.bbcook.cn

Counter(arr).most_common(3)
来源：http://frs.mhx1999.top

[U13] Py：固定长度队列
来源：http://cid.hysaishi.cn

deque(maxlen=10)
来源：http://ric.ivvv.top

[U14] Py：分组收集到列表
来源：http://eca.zhiwuduotai.top

defaultdict(list)
来源：http://dyp.andypj.xyz

[U15] Py：高精度计时
来源：http://lmi.hesvh.cn

t = time.perf_counter()
来源：http://man.jianghu66.top

[U16] Py：命令行参数解析
来源：http://tyc.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ybe.ydjk.org.cn

[U17] Py：初始化日志
来源：http://lkn.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://qsd.iojbl.cn

[U18] Py：预编译正则
来源：http://rwz.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://eir.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://epm.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wzq.xylfe.cn

[U20] Py：缓存函数结果
来源：http://ssd.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://agt.mhx1999.top

[U21] Py：自定义上下文管理器
来源：http://ala.yj202588.top

@contextlib.contextmanager
来源：http://zga.yj20258888.top

[U22] Py：矩阵转置
来源：http://vsh.dashuyun.cn

list(zip(*m))
来源：http://grf.ybcxt.top

[U23] Py：分块读取大文件
来源：http://ilm.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkz.xinyue.icu

[U24] Py：路径操作
来源：http://bjz.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mqw.birdmap.top

[U25] Py：CSV 按字典读
来源：http://jea.ppjwa.cn

csv.DictReader(f)
来源：http://elz.zhixingplan.top

[U26] Py：并发下载
来源：http://aib.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tud.smart0.xyz

[U27] Py：异步 HTTP
来源：http://rru.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://eat.vqdsnc.cn

[U28] Py：类型别名
来源：http://nzo.hesvh.cn

UserId = int
来源：http://key.feifeiyinyue.top

[U29] Py：属性校验
来源：http://iqo.fzhhl.top

@property 与 @x.setter 配合
来源：http://sfx.meibo888.top

[U30] Py：数据类
来源：http://jvm.c1oappe.top

@dataclass(slots=True)
来源：http://frg.jinyuanbaomall.cn

[U31] Py：单测
来源：http://vzt.andypj.xyz

python -m pytest -q
来源：http://jim.hfpthk.cn

[U32] Py：代码格式化
来源：http://pwh.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://kbj.jqgfzy.top

[U33] Py：打包发布
来源：http://hnx.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://swj.xuetiantiany.cn

[U34] Py：判断编码
来源：http://ehp.jinghuilouyu.cn

chardet.detect(raw)
来源：http://dbx.jinqigfzy.top

[U35] Py：发送邮件
来源：http://tyf.yj202588.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://non.andypj.xyz

[U36] Py：定时任务
来源：http://yuh.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://agb.chenlongwang.top

[U37] Py：读写 Excel
来源：http://dck.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://esh.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://xqv.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://mjn.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://bqj.vehdjk.com

sys.stdout.isatty()
来源：http://qzo.cheryme.top

[U40] Py：打印到标准错误
来源：http://rjv.gotoacloud.top

print("err", file=sys.stderr)
来源：http://qvm.ybcxt.top

[U41] PHP：初始化 Composer 项目
来源：http://qzt.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vbs.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://dkl.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgs.fktsv.cn

[U43] PHP：声明命名空间
来源：http://hmj.tian-w.cn

namespace App\Http;
来源：http://waq.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://asw.havefunace.top

declare(strict_types=1);
来源：http://srt.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://aka.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hgn.tianlin.xyz

[U46] PHP：可空类型
来源：http://ljq.vehdjk.com

?string $name = null
来源：http://czu.daxiang520.top

[U47] PHP：联合类型
来源：http://gbc.sxryk.cn

int|string $id
来源：http://zbz.jiagoushi.top

[U48] PHP：纯枚举
来源：http://rtx.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zjm.kuanghao11.cn

[U49] PHP：只读属性
来源：http://agm.cqqwz.cn

public readonly string $name
来源：http://okd.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://ayc.aibaodan.cn

public function __construct(private int $id) {}
来源：http://lcp.yanxiufei.cn

[U51] PHP：数组解构
来源：http://jze.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://akt.yfazqb.com

[U52] PHP：箭头函数
来源：http://sre.hammf.cn

$double = fn($x) => $x * 2;
来源：http://ijl.fehbvm.com

[U53] PHP：空合并运算符
来源：http://tee.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://fah.yueranfly.top

[U54] PHP：空安全调用
来源：http://car.hammf.cn

$obj?->method()
来源：http://bzo.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://gvv.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iep.yuanzhike.top

[U56] PHP：命名参数
来源：http://lps.epnwcf.com

f(a: 1, b: 2)
来源：http://iku.haohaochexian.top

[U57] PHP：字符串插值
来源：http://bkf.xuetiantiany.cn

"值: {$a}"
来源：http://wfc.ydjk.org.cn

[U58] PHP：数组三件套
来源：http://owp.chenjidiqi.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xxi.c1oappe.top

[U59] PHP：自定义排序
来源：http://dth.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eir.svipenyu.cn

[U60] PHP：JSON 编解码
来源：http://sdd.c1oappe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mhj.52xcode.cn

[U61] PHP：正则
来源：http://yjp.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xyh.vehdjk.com

[U62] PHP：日期对象
来源：http://ucm.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mcv.gogol.net.cn

[U63] PHP：文件读写
来源：http://jfo.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hxb.haohaochexian.top

[U64] PHP：目录遍历
来源：http://mrg.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://kdm.zycfv.cn

[U65] PHP：会话
来源：http://jjn.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wds.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://djr.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tpx.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://aoi.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jxz.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://lum.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mhk.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://bcx.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qqt.hfpthk.cn

[U70] PHP：PDO 事务
来源：http://adw.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twg.iojbl.cn

[U71] PHP：抛出异常
来源：http://gdz.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://hly.epnwcf.com

[U72] PHP：写错误日志
来源：http://mel.gotoacloud.top

error_log("失败: " . $e->getMessage());
来源：http://gbp.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://ypf.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://oqy.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://wnl.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://rvg.yangfankeji.com

[U75] PHP：依赖注入
来源：http://lmg.9152youxi.cn

composer require psr/container
来源：http://bhf.fengsongda.top

[U76] PHP：简单路由
来源：http://rbv.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aid.zycfv.cn

[U77] PHP：模板渲染
来源：http://fmr.xingfuxueyuan.xyz

composer require twig/twig
来源：http://sxc.gzhubu.top

[U78] PHP：单元测试
来源：http://rbc.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://naz.yuxming.cn

[U79] PHP：静态分析
来源：http://efm.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://zhn.fktsv.cn

[U80] PHP：代码规范修复
来源：http://xwm.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hcr.hfpthk.cn

[U81] JS：初始化项目
来源：http://ucz.ydjk.org.cn

npm init -y;  npm i express
来源：http://duu.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://rdh.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hre.zhaomingkeji.xyz

[U83] JS：ES Module 导入导出
来源：http://qso.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://wci.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://crf.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://usd.zhijiandao.cn

[U85] JS：可选链
来源：http://ghi.shzxlz.cn

a?.b?.c
来源：http://xuw.dianchejie.cn

[U86] JS：空值合并
来源：http://otq.hammf.cn

a ?? b
来源：http://fxz.yj202588.top

[U87] JS：解构默认值
来源：http://vax.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://rad.nwbrower.top

[U88] JS：对象展开合并
来源：http://wwc.nanxinkj.top

{ ...a, ...b }
来源：http://psz.aizwys.cn

[U89] JS：数组去重
来源：http://ypn.hongshengwenyu.top

[...new Set(arr)]
来源：http://ovq.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://cyx.yangfankeji.com

[...arr].sort((a, b) => a - b)
来源：http://xnp.svipenyu.cn

[U91] JS：对象键值遍历
来源：http://uqn.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iwy.jianghu66.top

[U92] JS：深拷贝
来源：http://pxm.cdnleiting.top

structuredClone(obj)
来源：http://sjq.ppjwa.cn


<!-- 参考信息 -->