代发 wailian999

[T05] Kotlin：when 表达式
来源：http://yey.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lac.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://uac.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rdm.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://dpr.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwz.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://woh.316326.xyz

data class User(val name: String, val age: Int)
来源：http://ztd.birdmap.top

[T09] Kotlin：扩展函数
来源：http://mdg.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://qzd.316326.xyz

[T10] Kotlin：默认参数
来源：http://lub.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://deh.nanxuanxn.top

[T11] Kotlin：协程
来源：http://qul.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ltu.xinyue.icu

[T12] Kotlin：解构声明
来源：http://xgh.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://xmh.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://csb.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://ape.mhx1999.top

[T14] Kotlin：循环
来源：http://olq.smart0.xyz

for (i in 1..10) println(i)
来源：http://ydn.sjlbkw.cn

[T15] Kotlin：接口
来源：http://ttb.yj20258.top

interface Shape { fun area(): Double }
来源：http://eax.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://abg.jinyuanbaomall.cn

print("Hello")
来源：http://sxo.chenzaomai.com

[T17] Swift：变量与常量
来源：http://omf.bbcook.cn

var a = 1;  let b = 2
来源：http://wkd.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://aba.vqdsnc.cn

"值: \(b)"
来源：http://rnp.tian-w.cn

[T19] Swift：可选绑定
来源：http://cbe.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://usn.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://rfz.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://pme.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://qtz.hcnkem.com

for x in a { print(x) }
来源：http://wyr.epnwcf.com

[T22] Swift：字典
来源：http://cds.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aji.pengpengdd.cyou

[T23] Swift：函数
来源：http://djq.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hkz.nanxuanxn.top

[T24] Swift：闭包
来源：http://bsq.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mid.fzhhl.top

[T25] Swift：结构体
来源：http://upo.smart0.xyz

struct P { var x: Int }
来源：http://kcx.meibo888.top

[T26] Swift：类与重写
来源：http://rsa.yongpay.top

class A: Base { override func f() {} }
来源：http://lyy.andypj.xyz

[T27] Swift：错误处理
来源：http://xjb.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://scj.hammf.cn

[T28] Swift：枚举
来源：http://gdi.svipenyu.cn

enum Color { case red, green }
来源：http://qqn.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://hak.sufxvd.cn

guard let x = opt else { return }
来源：http://ita.316326.xyz

[T30] Swift：协议
来源：http://xho.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://bic.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://tda.fktsv.cn

print("Hello")
来源：http://mwb.c1oappe.top

[T32] Lua：局部变量
来源：http://wxv.nanxuanxn.top

local a = 1
来源：http://rew.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://szc.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wqf.hysaishi.cn

[T34] Lua：遍历表
来源：http://jrz.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mxx.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://trr.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://nrr.yongpay.top

[T36] Lua：函数
来源：http://jgu.yuxming.cn

function add(a, b) return a + b end
来源：http://psa.guannengcc.top

[T37] Lua：字符串拼接
来源：http://weh.zhoulong.xyz

"a" .. "b"
来源：http://ujg.zdqjudy.top

[T38] Lua：条件
来源：http://kuf.meibo888.top

if x > 0 then print("正") end
来源：http://uvo.cashguo.top

[T39] Lua：模式匹配
来源：http://adk.yj202588.top

string.find(s, "%d+")
来源：http://gqi.c1oappe.top

[T40] Lua：元表
来源：http://ikq.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://oov.guannengcc.top

[T41] Perl：Hello World
来源：http://fxi.jinghuilouyu.cn

print "Hello\n";
来源：http://voc.snrcjt.cn

[T42] Perl：变量类型
来源：http://tbk.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://roc.hysaishi.cn

[T43] Perl：字符串插值
来源：http://rsx.fanxiaobao.xyz

"值: $a"
来源：http://vlh.cdnleiting.top

[T44] Perl：条件
来源：http://goa.birdmap.top

if ($a > 0) { print "正"; }
来源：http://ssj.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://qii.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://xti.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://tsf.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tut.guannengcc.top

[T47] Perl：正则捕获
来源：http://xte.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jss.guannengcc.top

[T48] Perl：正则替换
来源：http://izv.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://bmg.jiagoushi.top

[T49] Perl：函数
来源：http://wvp.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ima.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://mgg.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://edu.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://paf.uphjek.com

[T51] Scala：Hello World
来源：http://uap.pycfn.com

println("Hello")
来源：http://atx.zhijiandao.cn

[T52] Scala：变量
来源：http://mvr.yuanzhike.top

val a = 1;  var b = 2
来源：http://cta.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://bzn.yongpay.top

s"值: $b"
来源：http://edu.iojbl.cn

[T54] Scala：集合映射
来源：http://rje.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://yvx.redwolf501.top

[T55] Scala：集合过滤
来源：http://hjp.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zmd.bjfxy.top

[T56] Scala：样例类
来源：http://mhl.zycfv.cn

case class User(name: String, age: Int)
来源：http://amp.cucudq.cn

[T57] Scala：模式匹配
来源：http://nnl.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fpj.9152youxi.cn

[T58] Scala：函数定义
来源：http://rql.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://quo.epnwcf.com

[T59] Scala：循环
来源：http://wbn.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://dsy.yuanzhike.top

[T60] Scala：折叠
来源：http://ull.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kbm.yfazqb.com

================================================================================
来源：http://eiy.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zly.jqgufenzy.top

================================================================================
来源：http://oan.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://svv.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://vbg.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://myy.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://quk.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://hdc.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wdf.shzxlz.cn

[U04] Py：变量调试打印
来源：http://shk.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zuz.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://tpj.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://tib.zhijiandao.cn

[U06] Py：合并两个字典
来源：http://cxb.cheryme.top

{**a, **b}
来源：http://ybk.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://zvg.52xcode.cn

{v: k for k, v in d.items()}
来源：http://mni.fzhhl.top

[U08] Py：展平二维列表
来源：http://tfl.hcnkem.com

[y for x in nested for y in x]
来源：http://ixh.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://rep.wangdashe.top

max(d, key=d.get)
来源：http://xbp.uphjek.com

[U10] Py：按值排序字典
来源：http://ibh.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pnm.jqgfzy.top

[U11] Py：生成器表达式
来源：http://iyo.zycfv.cn

(x * 2 for x in arr)
来源：http://mhs.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://edp.uphjek.com

Counter(arr).most_common(3)
来源：http://hhz.ppjwa.cn

[U13] Py：固定长度队列
来源：http://wdx.snrcjt.cn

deque(maxlen=10)
来源：http://myy.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://ybo.hnxiangtu.top

defaultdict(list)
来源：http://hoz.smart0.xyz

[U15] Py：高精度计时
来源：http://olx.vehdjk.com

t = time.perf_counter()
来源：http://vzp.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://aom.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xyt.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://huv.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://hlf.uphjek.com

[U18] Py：预编译正则
来源：http://rcz.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://tvq.316326.xyz

[U19] Py：正则替换带回调
来源：http://rcn.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://llh.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://ksc.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://mpv.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://tqb.nwbrower.top

@contextlib.contextmanager
来源：http://bqx.tanke756.top

[U22] Py：矩阵转置
来源：http://ghe.ivvv.top

list(zip(*m))
来源：http://lis.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://nyq.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zvy.tian-w.cn

[U24] Py：路径操作
来源：http://wmz.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ivu.shuidangran.top

[U25] Py：CSV 按字典读
来源：http://hsv.ctjpmb.com

csv.DictReader(f)
来源：http://qtd.xuanzx.com

[U26] Py：并发下载
来源：http://xnv.shanyushiyangtech.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://krz.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://sjg.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://qad.havefunace.top

[U28] Py：类型别名
来源：http://yjw.gzhubu.top

UserId = int
来源：http://zwc.vehdjk.com

[U29] Py：属性校验
来源：http://pte.birdmap.top

@property 与 @x.setter 配合
来源：http://orn.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://ree.sufxvd.cn

@dataclass(slots=True)
来源：http://pfd.havefunace.top

[U31] Py：单测
来源：http://umo.yonumen.top

python -m pytest -q
来源：http://flo.meibo888.top

[U32] Py：代码格式化
来源：http://tnf.hnqzz.top

ruff format . && ruff check --fix .
来源：http://tgk.yongpay.top

[U33] Py：打包发布
来源：http://ldk.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://rcx.cucudq.cn

[U34] Py：判断编码
来源：http://zmx.hesvh.cn

chardet.detect(raw)
来源：http://sds.zhoulong.xyz

[U35] Py：发送邮件
来源：http://nzf.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ddb.jqgufenzy.top

[U36] Py：定时任务
来源：http://aee.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://oep.hnqzz.top

[U37] Py：读写 Excel
来源：http://foi.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://tvp.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://udq.tian-w.cn

Path(__file__).resolve().parent
来源：http://boa.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://qcj.zhixingplan.top

sys.stdout.isatty()
来源：http://ryi.shuidangran.top

[U40] Py：打印到标准错误
来源：http://xhf.bjfxy.top

print("err", file=sys.stderr)
来源：http://ckl.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://mmr.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ahm.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://vus.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dlt.yfazqb.com

[U43] PHP：声明命名空间
来源：http://gaw.havefunace.top

namespace App\Http;
来源：http://rnl.hcnkem.com

[U44] PHP：开启严格类型
来源：http://gsk.yongpay.top

declare(strict_types=1);
来源：http://ybn.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://mut.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tgp.hywenlv.cn

[U46] PHP：可空类型
来源：http://xyz.jyoumei.cn

?string $name = null
来源：http://rxo.ivvv.top

[U47] PHP：联合类型
来源：http://uln.daxiang520.top

int|string $id
来源：http://cqi.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://uvy.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hho.xziqi.cn

[U49] PHP：只读属性
来源：http://wlj.havefunace.top

public readonly string $name
来源：http://laa.sweek.top

[U50] PHP：构造器属性提升
来源：http://lim.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://kgq.mhx1999.top

[U51] PHP：数组解构
来源：http://brg.jianghu66.top

[$a, $b] = $arr;
来源：http://lba.nanxinkj.top

[U52] PHP：箭头函数
来源：http://sxi.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://mxf.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://sjt.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://rci.hywenlv.cn

[U54] PHP：空安全调用
来源：http://glx.fanxiaobao.xyz

$obj?->method()
来源：http://yyu.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://xdx.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://glr.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://frm.jqgfzy.top

f(a: 1, b: 2)
来源：http://pxx.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://mug.cdnleiting.top

"值: {$a}"
来源：http://ume.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://zrq.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kry.xziqi.cn

[U59] PHP：自定义排序
来源：http://dna.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dri.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://vng.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rkg.chenzaomai.com

[U61] PHP：正则
来源：http://pdx.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ria.yvedp.cn

[U62] PHP：日期对象
来源：http://kci.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://map.yj20258.top

[U63] PHP：文件读写
来源：http://wgo.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ipi.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://yev.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://htf.yanxiufei.cn

[U65] PHP：会话
来源：http://xec.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://itr.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://pej.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ccn.hesvh.cn

[U67] PHP：处理文件上传
来源：http://enn.daria6918.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dtt.jinyuanbaomall.cn

[U68] PHP：PDO 连接
来源：http://ypo.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pbe.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://mra.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nmw.yj20258888.top

[U70] PHP：PDO 事务
来源：http://uat.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fxf.aizwys.cn

[U71] PHP：抛出异常
来源：http://yzt.xinyue.icu

throw new RuntimeException("失败", 500);
来源：http://tor.zhixingplan.top

[U72] PHP：写错误日志
来源：http://izu.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://rrc.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://nyu.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://zwp.yongpay.top

[U74] PHP：读取环境变量
来源：http://ike.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://kbd.xylfe.cn

[U75] PHP：依赖注入
来源：http://adm.fengsongda.top

composer require psr/container
来源：http://drg.yongpay.top

[U76] PHP：简单路由
来源：http://xro.cucudq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hzi.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://wcp.yuxming.cn

composer require twig/twig
来源：http://xth.yvedp.cn

[U78] PHP：单元测试
来源：http://mpk.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://qur.aizwys.cn

[U79] PHP：静态分析
来源：http://exu.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://tnv.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://cqh.yueranfly.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://brp.zycfv.cn

[U81] JS：初始化项目
来源：http://wxo.yfazqb.com

npm init -y;  npm i express
来源：http://puh.redwolf501.top

[U82] JS：package.json 脚本
来源：http://gtr.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rdg.birdmap.top

[U83] JS：ES Module 导入导出
来源：http://bfr.fehbvm.com

export const a = 1;  import { a } from "./m.js";
来源：http://qtv.zycfv.cn

[U84] JS：CommonJS 写法
来源：http://qia.jlsjyb.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pnm.316326.xyz

[U85] JS：可选链
来源：http://tfn.sxryk.cn

a?.b?.c
来源：http://hyr.cheryme.top

[U86] JS：空值合并
来源：http://zsp.redwolf501.top

a ?? b
来源：http://rrg.smart0.xyz

[U87] JS：解构默认值
来源：http://kst.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://wqv.zycfv.cn

[U88] JS：对象展开合并
来源：http://auj.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://cgo.dianchejie.cn

[U89] JS：数组去重
来源：http://drd.kuanghao11.cn

[...new Set(arr)]
来源：http://fmv.hysaishi.cn

[U90] JS：数字数组排序
来源：http://oyo.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://rbl.jinghuilouyu.cn

[U91] JS：对象键值遍历
来源：http://xxe.chenlongwang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xax.bjfxy.top

[U92] JS：深拷贝
来源：http://wpe.yueranfly.top

structuredClone(obj)
来源：http://sjh.smart0.xyz


<!-- 参考信息 -->