代发 wailian999

[T09] Kotlin：扩展函数
来源：http://vgd.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://cjv.xylfe.cn

[T10] Kotlin：默认参数
来源：http://gof.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fsf.zhoulong.xyz

[T11] Kotlin：协程
来源：http://prz.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kgb.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://bxn.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://eum.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://bmd.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://hfe.jianghu66.top

[T14] Kotlin：循环
来源：http://vzp.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://wnz.sjlbkw.cn

[T15] Kotlin：接口
来源：http://wkv.fengsongda.top

interface Shape { fun area(): Double }
来源：http://xbb.epnwcf.com

[T16] Swift：Hello World
来源：http://pvz.gogol.net.cn

print("Hello")
来源：http://xqe.xinyue.icu

[T17] Swift：变量与常量
来源：http://rww.cqqwz.cn

var a = 1;  let b = 2
来源：http://nnd.snrcjt.cn

[T18] Swift：字符串插值
来源：http://wwx.chenjidiqi.icu

"值: \(b)"
来源：http://cmu.haohaochexian.top

[T19] Swift：可选绑定
来源：http://uor.xuanzx.com

if let n = opt { print(n) }
来源：http://qmq.jinqigfzy.top

[T20] Swift：数组操作
来源：http://gvr.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://kkh.xinyue.icu

[T21] Swift：遍历
来源：http://zqv.jinqigfzy.top

for x in a { print(x) }
来源：http://evu.sjlbkw.cn

[T22] Swift：字典
来源：http://mex.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://brp.sjlbkw.cn

[T23] Swift：函数
来源：http://sjd.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kwp.sxryk.cn

[T24] Swift：闭包
来源：http://ren.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://pfb.shzxlz.cn

[T25] Swift：结构体
来源：http://cnj.jinghuilouyu.cn

struct P { var x: Int }
来源：http://lnd.ehwqpu.com

[T26] Swift：类与重写
来源：http://hyz.tanke756.top

class A: Base { override func f() {} }
来源：http://vgq.shzxlz.cn

[T27] Swift：错误处理
来源：http://xfq.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://qzr.tianlin.xyz

[T28] Swift：枚举
来源：http://qgs.snrcjt.cn

enum Color { case red, green }
来源：http://ahr.yj20258.top

[T29] Swift：guard 提前返回
来源：http://wja.gotoacloud.top

guard let x = opt else { return }
来源：http://jeo.aibaodan.cn

[T30] Swift：协议
来源：http://qaj.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://tif.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://ymq.yueranfly.top

print("Hello")
来源：http://sxk.yuanzhike.top

[T32] Lua：局部变量
来源：http://qln.bbcook.cn

local a = 1
来源：http://tmo.shzxlz.cn

[T33] Lua：表（数组）
来源：http://ork.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://foe.yfazqb.com

[T34] Lua：遍历表
来源：http://kwb.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://guc.cdnleiting.top

[T35] Lua：字典表
来源：http://jtn.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://gtt.fktsv.cn

[T36] Lua：函数
来源：http://swx.hnqzz.top

function add(a, b) return a + b end
来源：http://wgj.redwolf501.top

[T37] Lua：字符串拼接
来源：http://cbr.daxiang520.top

"a" .. "b"
来源：http://lvo.yonumen.top

[T38] Lua：条件
来源：http://xgk.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://uhd.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://rzs.tian-w.cn

string.find(s, "%d+")
来源：http://spp.yuanzhike.top

[T40] Lua：元表
来源：http://ijz.jqgfzy.top

setmetatable({}, { __index = base })
来源：http://cqj.hammf.cn

[T41] Perl：Hello World
来源：http://uqe.jinghuilouyu.cn

print "Hello\n";
来源：http://jon.yfazqb.com

[T42] Perl：变量类型
来源：http://raj.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://abt.ehwqpu.com

[T43] Perl：字符串插值
来源：http://ahp.bjfxy.top

"值: $a"
来源：http://jan.snrcjt.cn

[T44] Perl：条件
来源：http://jii.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://afa.ybcxt.top

[T45] Perl：数组遍历
来源：http://prl.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://dgh.zycfv.cn

[T46] Perl：哈希操作
来源：http://lww.hfpthk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mnq.vehdjk.com

[T47] Perl：正则捕获
来源：http://lac.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qzr.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://vho.xinyue.icu

$s =~ s/old/new/g;
来源：http://hsw.shzxlz.cn

[T49] Perl：函数
来源：http://bky.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ser.yfazqb.com

[T50] Perl：逐行读文件
来源：http://ymp.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lmr.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://rbf.jyoumei.cn

[T51] Scala：Hello World
来源：http://dde.ybcxt.top

println("Hello")
来源：http://tfs.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://svd.zhixingplan.top

val a = 1;  var b = 2
来源：http://zxg.0kj1m.cn

[T53] Scala：字符串插值
来源：http://tfx.aizwys.cn

s"值: $b"
来源：http://fxl.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://wld.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://hal.xinyue.icu

[T55] Scala：集合过滤
来源：http://tky.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://tqw.sxryk.cn

[T56] Scala：样例类
来源：http://pli.gotoacloud.top

case class User(name: String, age: Int)
来源：http://zza.ybcxt.top

[T57] Scala：模式匹配
来源：http://rxa.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sim.yfazqb.com

[T58] Scala：函数定义
来源：http://sur.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://mys.ivvv.top

[T59] Scala：循环
来源：http://rxv.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://zjf.tian-w.cn

[T60] Scala：折叠
来源：http://wam.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ktf.tanke756.top

================================================================================
来源：http://agc.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://toi.xylfe.cn

================================================================================
来源：http://clb.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://jan.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://xxi.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://pnp.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ukr.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://dfm.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yhc.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://umh.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ggs.tanke756.top

[U05] Py：列表去重且保序
来源：http://raz.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://okr.sufxvd.cn

[U06] Py：合并两个字典
来源：http://nuq.yj202588.top

{**a, **b}
来源：http://vik.jiagoushi.top

[U07] Py：反转字典键值
来源：http://rdk.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://hgo.chenzaomai.com

[U08] Py：展平二维列表
来源：http://yyo.jlsjyb.cn

[y for x in nested for y in x]
来源：http://scl.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://etn.hywenlv.cn

max(d, key=d.get)
来源：http://kxy.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://bnv.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uia.svipenyu.cn

[U11] Py：生成器表达式
来源：http://iov.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://vij.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://ati.shangyingyoupin.top

Counter(arr).most_common(3)
来源：http://ytt.yueranfly.top

[U13] Py：固定长度队列
来源：http://utr.jiagoushi.top

deque(maxlen=10)
来源：http://dbs.yueranfly.top

[U14] Py：分组收集到列表
来源：http://snj.sweek.top

defaultdict(list)
来源：http://bsj.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://wrd.hnxiangtu.top

t = time.perf_counter()
来源：http://prd.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://gxq.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zpn.52xcode.cn

[U17] Py：初始化日志
来源：http://app.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://aqr.haohaochexian.top

[U18] Py：预编译正则
来源：http://efu.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://wfd.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://umy.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ylz.aizwys.cn

[U20] Py：缓存函数结果
来源：http://cqn.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://zmd.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://nar.jinqigufen.top

@contextlib.contextmanager
来源：http://jqh.sxryk.cn

[U22] Py：矩阵转置
来源：http://kys.daria6918.cn

list(zip(*m))
来源：http://lgc.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://dze.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yro.meibo888.top

[U24] Py：路径操作
来源：http://txu.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cyx.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://zag.jinghuilouyu.cn

csv.DictReader(f)
来源：http://dod.sjlbkw.cn

[U26] Py：并发下载
来源：http://xxt.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fhr.havefunace.top

[U27] Py：异步 HTTP
来源：http://yia.shanyushiyangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://hhd.fzhhl.top

[U28] Py：类型别名
来源：http://fgq.cucudq.cn

UserId = int
来源：http://vop.jyoumei.cn

[U29] Py：属性校验
来源：http://nok.yuxming.cn

@property 与 @x.setter 配合
来源：http://hsh.havefunace.top

[U30] Py：数据类
来源：http://lhd.shuidangran.top

@dataclass(slots=True)
来源：http://xsm.zhiwuduotai.top

[U31] Py：单测
来源：http://vry.yuanzhike.top

python -m pytest -q
来源：http://dhq.mhx1999.top

[U32] Py：代码格式化
来源：http://qti.epnwcf.com

ruff format . && ruff check --fix .
来源：http://hgc.yvedp.cn

[U33] Py：打包发布
来源：http://bkx.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://qhf.birdmap.top

[U34] Py：判断编码
来源：http://aav.fanxiaobao.xyz

chardet.detect(raw)
来源：http://uwh.sjlbkw.cn

[U35] Py：发送邮件
来源：http://sow.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qxk.zhijiandao.cn

[U36] Py：定时任务
来源：http://iqm.nanxuanxn.top

schedule.every(10).minutes.do(job)
来源：http://hmb.sxryk.cn

[U37] Py：读写 Excel
来源：http://ufj.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://rgd.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://vol.ybcxt.top

Path(__file__).resolve().parent
来源：http://uyq.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://bym.yj20258.top

sys.stdout.isatty()
来源：http://kbe.cashguo.top

[U40] Py：打印到标准错误
来源：http://kni.dianchejie.cn

print("err", file=sys.stderr)
来源：http://qsh.jqgfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://umy.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://csr.yanxiufei.cn

[U42] PHP：PSR-4 自动加载
来源：http://vpz.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lhn.nwbrower.top

[U43] PHP：声明命名空间
来源：http://odg.daxiang520.top

namespace App\Http;
来源：http://bel.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://jvl.zhoulong.xyz

declare(strict_types=1);
来源：http://srj.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://hom.c1oappe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rmq.fengsongda.top

[U46] PHP：可空类型
来源：http://dor.0kj1m.cn

?string $name = null
来源：http://onv.xylfe.cn

[U47] PHP：联合类型
来源：http://kjz.vqdsnc.cn

int|string $id
来源：http://aau.birdmap.top

[U48] PHP：纯枚举
来源：http://snt.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xeq.zhixingplan.top

[U49] PHP：只读属性
来源：http://fhx.jqgfzy.top

public readonly string $name
来源：http://thi.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://tog.zdbjq.cn

public function __construct(private int $id) {}
来源：http://idh.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://bip.zdqjudy.top

[$a, $b] = $arr;
来源：http://qsm.hysaishi.cn

[U52] PHP：箭头函数
来源：http://ijh.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://agt.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://grg.hongshengwenyu.top

$v = $a ?? $b ?? "default";
来源：http://szv.dianchejie.cn

[U54] PHP：空安全调用
来源：http://eha.yj202588.top

$obj?->method()
来源：http://exv.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://rfa.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lic.jinyuanbaomall.cn

[U56] PHP：命名参数
来源：http://okm.redwolf501.top

f(a: 1, b: 2)
来源：http://wrm.jianghu66.top

[U57] PHP：字符串插值
来源：http://dnj.zhaomingkeji.xyz

"值: {$a}"
来源：http://slz.sysykeji.top

[U58] PHP：数组三件套
来源：http://zme.uphjek.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ulc.tianlin.xyz

[U59] PHP：自定义排序
来源：http://fpq.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrs.pycfn.com

[U60] PHP：JSON 编解码
来源：http://wcj.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fuf.jyoumei.cn

[U61] PHP：正则
来源：http://ryp.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xol.zhoulong.xyz

[U62] PHP：日期对象
来源：http://uyh.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://swj.9152youxi.cn

[U63] PHP：文件读写
来源：http://cvu.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vig.jianghu66.top

[U64] PHP：目录遍历
来源：http://nma.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://rfm.gogol.net.cn

[U65] PHP：会话
来源：http://fus.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nds.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://oxk.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hjj.hammf.cn

[U67] PHP：处理文件上传
来源：http://sjw.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qoe.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://vay.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://typ.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://tps.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cve.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://bvj.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kca.xinyue.icu

[U71] PHP：抛出异常
来源：http://cbq.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://erw.vqdsnc.cn

[U72] PHP：写错误日志
来源：http://zvl.hcnkem.com

error_log("失败: " . $e->getMessage());
来源：http://eva.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://hac.yueranfly.top

parse_ini_file("config.ini", true)
来源：http://alf.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://sdg.cucudq.cn

getenv("APP_ENV") ?: "production"
来源：http://gya.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://cgi.zdbjq.cn

composer require psr/container
来源：http://bel.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://dbz.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eln.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://kur.shanyushiyangkeji.top

composer require twig/twig
来源：http://zul.yj20258888.top

[U78] PHP：单元测试
来源：http://cfz.sweek.top

composer require --dev phpunit/phpunit
来源：http://eix.jinqigfzy.top

[U79] PHP：静态分析
来源：http://krb.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://hrd.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://uwd.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://swl.mhx1999.top

[U81] JS：初始化项目
来源：http://uwc.snrcjt.cn

npm init -y;  npm i express
来源：http://jzj.vehdjk.com

[U82] JS：package.json 脚本
来源：http://cso.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qca.redwolf501.top

[U83] JS：ES Module 导入导出
来源：http://gsf.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://lyj.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://efe.daria6918.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vvn.guowangkeji.top

[U85] JS：可选链
来源：http://yrf.cheryme.top

a?.b?.c
来源：http://guh.yongpay.top

[U86] JS：空值合并
来源：http://nns.kuanghao11.cn

a ?? b
来源：http://rfq.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://jtv.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://avj.jiagoushi.top

[U88] JS：对象展开合并
来源：http://teu.xziqi.cn

{ ...a, ...b }
来源：http://rgj.xuetiantiany.cn

[U89] JS：数组去重
来源：http://ucl.tian-w.cn

[...new Set(arr)]
来源：http://yzn.daria6918.cn

[U90] JS：数字数组排序
来源：http://wpj.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://slm.andypj.xyz

[U91] JS：对象键值遍历
来源：http://ook.jiagoushi.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://awy.shanyushiyangkeji.top

[U92] JS：深拷贝
来源：http://yta.mhx1999.top

structuredClone(obj)
来源：http://yxk.aizwys.cn

[U93] JS：模板字符串
来源：http://zge.jianghu66.top

`共 ${n} 条`
来源：http://mvf.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://bfr.fanxiaobao.xyz

const double = x => x * 2;
来源：http://enm.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://hfa.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://goy.vehdjk.com

[U96] JS：async/await 与异常
来源：http://akz.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xra.smart0.xyz


<!-- 参考信息 -->