代发 wailian999

[T03] Kotlin：字符串模板
来源：http://upf.fktsv.cn

"值: $b"
来源：http://eua.sxryk.cn

[T04] Kotlin：空安全
来源：http://yxf.dashuyun.cn

val n: String? = null;  n?.length
来源：http://rvu.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://gac.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mlw.xuanzx.com

[T06] Kotlin：集合映射
来源：http://nyp.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rvs.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://tgd.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bkt.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://azu.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://dzy.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://nej.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://yut.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://gsj.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kui.gotoacloud.top

[T11] Kotlin：协程
来源：http://gob.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ivv.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://fhb.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://mvo.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://wal.andypj.xyz

val m = mapOf("a" to 1)
来源：http://aze.aibaodan.cn

[T14] Kotlin：循环
来源：http://wei.bbcook.cn

for (i in 1..10) println(i)
来源：http://ulx.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://ezm.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://tmf.fengsongda.top

[T16] Swift：Hello World
来源：http://zmc.havefunace.top

print("Hello")
来源：http://oqn.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://zzo.sweek.top

var a = 1;  let b = 2
来源：http://qck.hcnkem.com

[T18] Swift：字符串插值
来源：http://wcn.hesvh.cn

"值: \(b)"
来源：http://nie.sweek.top

[T19] Swift：可选绑定
来源：http://ygc.jqgfzy.top

if let n = opt { print(n) }
来源：http://fhy.tianlin.xyz

[T20] Swift：数组操作
来源：http://bpk.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://iio.wangdashe.top

[T21] Swift：遍历
来源：http://cpp.bbcook.cn

for x in a { print(x) }
来源：http://wck.cheryme.top

[T22] Swift：字典
来源：http://qee.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://npg.zdqjudy.top

[T23] Swift：函数
来源：http://czc.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xdz.52xcode.cn

[T24] Swift：闭包
来源：http://ykq.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xjh.pycfn.com

[T25] Swift：结构体
来源：http://duz.daxiang520.top

struct P { var x: Int }
来源：http://hfy.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://wec.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://jwh.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://goq.hammf.cn

do { try f() } catch { print(error) }
来源：http://sbh.jyoumei.cn

[T28] Swift：枚举
来源：http://uog.yj202588.top

enum Color { case red, green }
来源：http://ilh.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://lwj.zdqjudy.top

guard let x = opt else { return }
来源：http://gkm.pengpengdd.cyou

[T30] Swift：协议
来源：http://mel.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://gjm.haohaochexian.top

[T31] Lua：Hello World
来源：http://gco.hcnkem.com

print("Hello")
来源：http://txr.yuanzhike.top

[T32] Lua：局部变量
来源：http://vir.mhx1999.top

local a = 1
来源：http://mao.cqqwz.cn

[T33] Lua：表（数组）
来源：http://snp.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://adc.yangfankeji.com

[T34] Lua：遍历表
来源：http://fxf.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mkf.cqqwz.cn

[T35] Lua：字典表
来源：http://knl.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://dpo.xuanzx.com

[T36] Lua：函数
来源：http://pxh.tian-w.cn

function add(a, b) return a + b end
来源：http://iin.cashguo.top

[T37] Lua：字符串拼接
来源：http://wsd.fzhhl.top

"a" .. "b"
来源：http://uea.gogol.net.cn

[T38] Lua：条件
来源：http://piy.0kj1m.cn

if x > 0 then print("正") end
来源：http://rzv.dashuyun.cn

[T39] Lua：模式匹配
来源：http://zww.tarul.cn

string.find(s, "%d+")
来源：http://tch.ybcxt.top

[T40] Lua：元表
来源：http://lds.sweek.top

setmetatable({}, { __index = base })
来源：http://wwt.ydzc1.top

[T41] Perl：Hello World
来源：http://ntc.vqdsnc.cn

print "Hello\n";
来源：http://rvb.9152youxi.cn

[T42] Perl：变量类型
来源：http://utj.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rpr.nwbrower.top

[T43] Perl：字符串插值
来源：http://qih.dashuyun.cn

"值: $a"
来源：http://hsz.zycfv.cn

[T44] Perl：条件
来源：http://tje.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://pio.havefunace.top

[T45] Perl：数组遍历
来源：http://ync.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://qcf.ivvv.top

[T46] Perl：哈希操作
来源：http://wky.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ceb.jinqigufen.top

[T47] Perl：正则捕获
来源：http://ayc.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jkj.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://qfb.tarul.cn

$s =~ s/old/new/g;
来源：http://wbf.ehwqpu.com

[T49] Perl：函数
来源：http://bkl.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vrx.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://nxg.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ixx.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://yvk.vehdjk.com

[T51] Scala：Hello World
来源：http://peg.jlsjyb.cn

println("Hello")
来源：http://htz.sjlbkw.cn

[T52] Scala：变量
来源：http://mlz.aibaodan.cn

val a = 1;  var b = 2
来源：http://tvr.hnqzz.top

[T53] Scala：字符串插值
来源：http://azg.daria6918.cn

s"值: $b"
来源：http://kfd.yvedp.cn

[T54] Scala：集合映射
来源：http://bbe.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://jnh.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://ubw.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cww.ctjpmb.com

[T56] Scala：样例类
来源：http://awx.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://ztr.hfpthk.cn

[T57] Scala：模式匹配
来源：http://cyg.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ywc.ydzc1.top

[T58] Scala：函数定义
来源：http://mai.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://abm.dianchejie.cn

[T59] Scala：循环
来源：http://fwm.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://vzv.chenjidiqi.icu

[T60] Scala：折叠
来源：http://gxk.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vod.daxiang520.top

================================================================================
来源：http://fwo.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://glt.yj202588.top

================================================================================
来源：http://yrd.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://yzl.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://lwe.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://frh.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://akj.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://qhn.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hvz.bjfxy.top

[U04] Py：变量调试打印
来源：http://olc.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qpi.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://nvs.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://sev.52xcode.cn

[U06] Py：合并两个字典
来源：http://mod.hfpthk.cn

{**a, **b}
来源：http://jbq.tanke756.top

[U07] Py：反转字典键值
来源：http://tyf.daria6918.cn

{v: k for k, v in d.items()}
来源：http://xrq.ivvv.top

[U08] Py：展平二维列表
来源：http://snq.birdmap.top

[y for x in nested for y in x]
来源：http://rwd.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://afl.tianlin.xyz

max(d, key=d.get)
来源：http://tyv.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://wey.fehbvm.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xax.xuanzx.com

[U11] Py：生成器表达式
来源：http://qnj.sxryk.cn

(x * 2 for x in arr)
来源：http://pbo.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://knn.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://gyj.svipenyu.cn

[U13] Py：固定长度队列
来源：http://ufc.ivvv.top

deque(maxlen=10)
来源：http://uug.vehdjk.com

[U14] Py：分组收集到列表
来源：http://ajk.ydzc1.top

defaultdict(list)
来源：http://bog.xinyue.icu

[U15] Py：高精度计时
来源：http://rkn.jinqigfzy.top

t = time.perf_counter()
来源：http://ptj.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://hmc.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://puy.zhengqikj.top

[U17] Py：初始化日志
来源：http://jdc.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://juu.nanxinkj.top

[U18] Py：预编译正则
来源：http://iwz.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://wfp.mhx1999.top

[U19] Py：正则替换带回调
来源：http://jug.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zjl.nwbrower.top

[U20] Py：缓存函数结果
来源：http://skb.sxryk.cn

@functools.lru_cache(maxsize=None)
来源：http://enk.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://cmz.hammf.cn

@contextlib.contextmanager
来源：http://gbf.sysykeji.top

[U22] Py：矩阵转置
来源：http://bpp.yj20258888.top

list(zip(*m))
来源：http://xep.vehdjk.com

[U23] Py：分块读取大文件
来源：http://lgv.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ctr.jinqigfzy.top

[U24] Py：路径操作
来源：http://chm.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kmw.havefunace.top

[U25] Py：CSV 按字典读
来源：http://wwj.ydzc1.top

csv.DictReader(f)
来源：http://ghl.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://uxm.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ouj.yueranfly.top

[U27] Py：异步 HTTP
来源：http://chi.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://fqu.zhiwuduotai.top

[U28] Py：类型别名
来源：http://hud.zhongyouzk.top

UserId = int
来源：http://fua.shangyingyoupin.top

[U29] Py：属性校验
来源：http://voe.aibaodan.cn

@property 与 @x.setter 配合
来源：http://xwb.gaohongyu789.top

[U30] Py：数据类
来源：http://gnd.aizwys.cn

@dataclass(slots=True)
来源：http://paf.shzxlz.cn

[U31] Py：单测
来源：http://mbs.jiagoushi.top

python -m pytest -q
来源：http://tgd.pycfn.com

[U32] Py：代码格式化
来源：http://aqb.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://nos.guowangkeji.top

[U33] Py：打包发布
来源：http://ppn.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://boq.shzxlz.cn

[U34] Py：判断编码
来源：http://jty.xylfe.cn

chardet.detect(raw)
来源：http://bjg.zycfv.cn

[U35] Py：发送邮件
来源：http://nmc.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pzu.cqqwz.cn

[U36] Py：定时任务
来源：http://hir.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://lpq.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://hpj.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oqt.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://ylf.jqgfzy.top

Path(__file__).resolve().parent
来源：http://ipk.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://rvv.shuidangran.top

sys.stdout.isatty()
来源：http://gsm.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://fgp.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://pmo.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://cfo.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lny.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://bqf.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://unq.mhx1999.top

[U43] PHP：声明命名空间
来源：http://ubj.pycfn.com

namespace App\Http;
来源：http://grl.andypj.xyz

[U44] PHP：开启严格类型
来源：http://rux.jqgufenzy.top

declare(strict_types=1);
来源：http://lhj.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://bxl.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://isu.yanxiufei.cn

[U46] PHP：可空类型
来源：http://sco.svipenyu.cn

?string $name = null
来源：http://ikv.zycfv.cn

[U47] PHP：联合类型
来源：http://cfy.jinghuilouyu.cn

int|string $id
来源：http://uxy.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://lwn.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wls.jlsjyb.cn

[U49] PHP：只读属性
来源：http://uvq.ybcxt.top

public readonly string $name
来源：http://yoy.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://rdj.cucudq.cn

public function __construct(private int $id) {}
来源：http://svs.tianlin.xyz

[U51] PHP：数组解构
来源：http://dbn.shzxlz.cn

[$a, $b] = $arr;
来源：http://pfu.uphjek.com

[U52] PHP：箭头函数
来源：http://abl.birdmap.top

$double = fn($x) => $x * 2;
来源：http://czo.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://fwc.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://dhv.jlsjyb.cn

[U54] PHP：空安全调用
来源：http://vjx.hnxiangtu.top

$obj?->method()
来源：http://lrw.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://odl.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uwh.kuanghao11.cn

[U56] PHP：命名参数
来源：http://dug.sjlbkw.cn

f(a: 1, b: 2)
来源：http://ejc.nwbrower.top

[U57] PHP：字符串插值
来源：http://dvh.tarul.cn

"值: {$a}"
来源：http://ged.nanxuanxn.top

[U58] PHP：数组三件套
来源：http://vrf.hnxiangtu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kgb.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://qmb.hammf.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fib.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://xmx.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kgo.smart0.xyz

[U61] PHP：正则
来源：http://foy.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hhu.xuetiantiany.cn

[U62] PHP：日期对象
来源：http://snq.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bco.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://hzt.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ilq.kuanghao11.cn

[U64] PHP：目录遍历
来源：http://hdr.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://plf.hfpthk.cn

[U65] PHP：会话
来源：http://irz.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://diu.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://nev.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ifq.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://fyv.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://znr.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://xgh.sufxvd.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rjg.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://hjh.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hdu.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://aeb.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kad.zdqjudy.top

[U71] PHP：抛出异常
来源：http://amx.haohaochexian.top

throw new RuntimeException("失败", 500);
来源：http://vqa.yueranfly.top

[U72] PHP：写错误日志
来源：http://ame.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://gzi.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://cmq.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://rvy.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://jgh.jlsjyb.cn

getenv("APP_ENV") ?: "production"
来源：http://zls.daria6918.cn

[U75] PHP：依赖注入
来源：http://nas.feifeiyinyue.top

composer require psr/container
来源：http://qyb.yongpay.top

[U76] PHP：简单路由
来源：http://pga.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tmt.yangfankeji.com

[U77] PHP：模板渲染
来源：http://pfk.yanxiufei.cn

composer require twig/twig
来源：http://gkj.wangdashe.top

[U78] PHP：单元测试
来源：http://vcu.316326.xyz

composer require --dev phpunit/phpunit
来源：http://pax.hfpthk.cn

[U79] PHP：静态分析
来源：http://qvs.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://bkv.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://xig.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ifp.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://qea.fehbvm.com

npm init -y;  npm i express
来源：http://yum.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://sjq.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tls.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://wve.wangshuangyany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://drt.shangyingyoupin.top

[U84] JS：CommonJS 写法
来源：http://hhj.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://bmp.ydzc1.top

[U85] JS：可选链
来源：http://sdm.shzxlz.cn

a?.b?.c
来源：http://bis.hcnkem.com

[U86] JS：空值合并
来源：http://btq.gotoacloud.top

a ?? b
来源：http://fba.gogol.net.cn

[U87] JS：解构默认值
来源：http://vnu.fktsv.cn

const { a = 1, b = 2 } = obj;
来源：http://ewz.hnqzz.top

[U88] JS：对象展开合并
来源：http://fyp.yfazqb.com

{ ...a, ...b }
来源：http://dtt.sjlbkw.cn

[U89] JS：数组去重
来源：http://nhu.0kj1m.cn

[...new Set(arr)]
来源：http://jsi.andypj.xyz

[U90] JS：数字数组排序
来源：http://pch.uphjek.com

[...arr].sort((a, b) => a - b)
来源：http://epl.hysaishi.cn


<!-- 参考信息 -->