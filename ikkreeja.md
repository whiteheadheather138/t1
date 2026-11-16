代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yku.yanxiufei.cn

================================================================================
来源：http://tft.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdq.9152youxi.cn

================================================================================
来源：http://lxk.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://oor.xziqi.cn

println("Hello")
来源：http://xfa.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://krz.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgp.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://rah.316326.xyz

"值: $b"
来源：http://zva.316326.xyz

[T04] Kotlin：空安全
来源：http://jna.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://yck.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://owr.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ppf.sweek.top

[T06] Kotlin：集合映射
来源：http://bsb.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xid.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://ybw.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mmm.xziqi.cn

[T08] Kotlin：数据类
来源：http://tdn.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://has.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://rli.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://ksc.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://xlv.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tfw.haohaochexian.top

[T11] Kotlin：协程
来源：http://cmw.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rsx.uphjek.com

[T12] Kotlin：解构声明
来源：http://elc.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://ogx.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://ise.birdmap.top

val m = mapOf("a" to 1)
来源：http://kop.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://bfq.uphjek.com

for (i in 1..10) println(i)
来源：http://wpu.cashguo.top

[T15] Kotlin：接口
来源：http://gor.yj20258.top

interface Shape { fun area(): Double }
来源：http://wkc.yanxiufei.cn

[T16] Swift：Hello World
来源：http://plb.yuxming.cn

print("Hello")
来源：http://uax.9152youxi.cn

[T17] Swift：变量与常量
来源：http://pyw.hfpthk.cn

var a = 1;  let b = 2
来源：http://hps.epnwcf.com

[T18] Swift：字符串插值
来源：http://jao.zhijiandao.cn

"值: \(b)"
来源：http://hjr.shzxlz.cn

[T19] Swift：可选绑定
来源：http://qzw.cheryme.top

if let n = opt { print(n) }
来源：http://zle.snrcjt.cn

[T20] Swift：数组操作
来源：http://aje.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://djs.uphjek.com

[T21] Swift：遍历
来源：http://vcs.hfpthk.cn

for x in a { print(x) }
来源：http://zjm.daria6918.cn

[T22] Swift：字典
来源：http://zrq.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rgf.jqgfzy.top

[T23] Swift：函数
来源：http://lwt.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lce.mhx1999.top

[T24] Swift：闭包
来源：http://bbl.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://avp.smart0.xyz

[T25] Swift：结构体
来源：http://zat.vehdjk.com

struct P { var x: Int }
来源：http://jxg.sufxvd.cn

[T26] Swift：类与重写
来源：http://nrn.fehbvm.com

class A: Base { override func f() {} }
来源：http://qpp.yuxming.cn

[T27] Swift：错误处理
来源：http://kda.redwolf501.top

do { try f() } catch { print(error) }
来源：http://okv.smart0.xyz

[T28] Swift：枚举
来源：http://ime.guowangkeji.top

enum Color { case red, green }
来源：http://xdu.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://jmw.gogol.net.cn

guard let x = opt else { return }
来源：http://pgb.wangshuangyany.cn

[T30] Swift：协议
来源：http://euf.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://uge.9152youxi.cn

[T31] Lua：Hello World
来源：http://wam.uphjek.com

print("Hello")
来源：http://lrz.sysykeji.top

[T32] Lua：局部变量
来源：http://aiv.ywan-chungtsiang.top

local a = 1
来源：http://ftg.fzhhl.top

[T33] Lua：表（数组）
来源：http://ows.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xxg.ivvv.top

[T34] Lua：遍历表
来源：http://ycf.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xjb.cheryme.top

[T35] Lua：字典表
来源：http://sej.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://qap.guowangkeji.top

[T36] Lua：函数
来源：http://ndh.ydzc1.top

function add(a, b) return a + b end
来源：http://yhh.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://jve.ywan-chungtsiang.top

"a" .. "b"
来源：http://dkp.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://mew.jlsjyb.cn

if x > 0 then print("正") end
来源：http://pib.shzxlz.cn

[T39] Lua：模式匹配
来源：http://gbk.yj202588.top

string.find(s, "%d+")
来源：http://jcs.pycfn.com

[T40] Lua：元表
来源：http://gzj.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://cqe.wangdashe.top

[T41] Perl：Hello World
来源：http://zci.ehwqpu.com

print "Hello\n";
来源：http://zmm.epnwcf.com

[T42] Perl：变量类型
来源：http://uof.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sme.jyoumei.cn

[T43] Perl：字符串插值
来源：http://tjo.shanyushiyangtech.top

"值: $a"
来源：http://fim.sysykeji.top

[T44] Perl：条件
来源：http://enh.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://yni.snrcjt.cn

[T45] Perl：数组遍历
来源：http://ilf.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://bod.zdqjudy.top

[T46] Perl：哈希操作
来源：http://fsm.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uzf.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://nsx.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xwr.yj202588.top

[T48] Perl：正则替换
来源：http://vat.redwolf501.top

$s =~ s/old/new/g;
来源：http://kkr.jqgfzy.top

[T49] Perl：函数
来源：http://anu.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vnu.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://lgh.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fgt.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://gvp.redwolf501.top

[T51] Scala：Hello World
来源：http://gyv.cheryme.top

println("Hello")
来源：http://wmn.ydzc1.top

[T52] Scala：变量
来源：http://ier.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://luz.yvedp.cn

[T53] Scala：字符串插值
来源：http://tgx.hysaishi.cn

s"值: $b"
来源：http://vjn.hcnkem.com

[T54] Scala：集合映射
来源：http://fgk.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://zdx.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://pjq.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://yhl.tanke756.top

[T56] Scala：样例类
来源：http://hsh.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://fhz.yj20258888.top

[T57] Scala：模式匹配
来源：http://ggd.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vqj.zhengqikj.top

[T58] Scala：函数定义
来源：http://ihe.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://bxv.fehbvm.com

[T59] Scala：循环
来源：http://ywa.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://rgj.hnxiangtu.top

[T60] Scala：折叠
来源：http://gtc.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pqv.smart0.xyz

================================================================================
来源：http://jyt.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wka.gotoacloud.top

================================================================================
来源：http://bwe.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://hzs.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://dfw.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://ynj.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xun.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://cyk.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pvs.bbcook.cn

[U04] Py：变量调试打印
来源：http://rxi.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://soz.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://yxz.nwbrower.top

list(dict.fromkeys(arr))
来源：http://sqo.smart0.xyz

[U06] Py：合并两个字典
来源：http://pqg.hongshengwenyu.top

{**a, **b}
来源：http://ash.gzhubu.top

[U07] Py：反转字典键值
来源：http://jyj.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://yup.zhengqikj.top

[U08] Py：展平二维列表
来源：http://ozv.kuanghao11.cn

[y for x in nested for y in x]
来源：http://jvr.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://kob.zhixingplan.top

max(d, key=d.get)
来源：http://scf.ehwqpu.com

[U10] Py：按值排序字典
来源：http://zvd.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oey.cheryme.top

[U11] Py：生成器表达式
来源：http://gfp.jianghu66.top

(x * 2 for x in arr)
来源：http://htx.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://cpu.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://qdg.ybcxt.top

[U13] Py：固定长度队列
来源：http://bsm.shangyingyoupin.top

deque(maxlen=10)
来源：http://qne.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://wax.smart0.xyz

defaultdict(list)
来源：http://irr.andypj.xyz

[U15] Py：高精度计时
来源：http://cpr.chenlongwang.top

t = time.perf_counter()
来源：http://wai.yueranfly.top

[U16] Py：命令行参数解析
来源：http://quh.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://juy.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://inl.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://syd.shzxlz.cn

[U18] Py：预编译正则
来源：http://gjh.sxryk.cn

pat = re.compile(r"\d+")
来源：http://ogz.xuanzx.com

[U19] Py：正则替换带回调
来源：http://pzl.gotoacloud.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zup.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://cuu.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://uhk.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://gxb.vqdsnc.cn

@contextlib.contextmanager
来源：http://ayu.yvedp.cn

[U22] Py：矩阵转置
来源：http://fsk.guannengcc.top

list(zip(*m))
来源：http://vvu.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://vwt.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wut.cashguo.top

[U24] Py：路径操作
来源：http://agu.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qwy.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://aps.vehdjk.com

csv.DictReader(f)
来源：http://hrp.hammf.cn

[U26] Py：并发下载
来源：http://lvf.snrcjt.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yjx.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://utu.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://hye.ydjk.org.cn

[U28] Py：类型别名
来源：http://vdt.wangdashe.top

UserId = int
来源：http://tfx.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://aod.guannengcc.top

@property 与 @x.setter 配合
来源：http://duk.hongshengwenyu.top

[U30] Py：数据类
来源：http://lup.mhx1999.top

@dataclass(slots=True)
来源：http://eyq.sysykeji.top

[U31] Py：单测
来源：http://dqc.jinqigufen.top

python -m pytest -q
来源：http://yhd.cucudq.cn

[U32] Py：代码格式化
来源：http://iuo.xuanzx.com

ruff format . && ruff check --fix .
来源：http://blf.sxryk.cn

[U33] Py：打包发布
来源：http://uyb.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://ftn.xuetiantiany.cn

[U34] Py：判断编码
来源：http://dyk.yueranfly.top

chardet.detect(raw)
来源：http://nmx.hysaishi.cn

[U35] Py：发送邮件
来源：http://kfw.yongpay.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tzw.wangshuangyany.cn

[U36] Py：定时任务
来源：http://gqc.redwolf501.top

schedule.every(10).minutes.do(job)
来源：http://lkn.aibaodan.cn

[U37] Py：读写 Excel
来源：http://wqh.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://msk.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://uqz.sweek.top

Path(__file__).resolve().parent
来源：http://dkt.yonumen.top

[U39] Py：判断是否在交互环境
来源：http://cyj.vqdsnc.cn

sys.stdout.isatty()
来源：http://bkd.ivvv.top

[U40] Py：打印到标准错误
来源：http://ezy.snrcjt.cn

print("err", file=sys.stderr)
来源：http://pun.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://efx.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pji.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://gdq.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qwv.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://ieh.vqdsnc.cn

namespace App\Http;
来源：http://wdg.bbcook.cn

[U44] PHP：开启严格类型
来源：http://yfz.ppjwa.cn

declare(strict_types=1);
来源：http://lbe.wangdashe.top

[U45] PHP：类型声明与返回类型
来源：http://yho.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://syl.yanxiufei.cn

[U46] PHP：可空类型
来源：http://ain.sweek.top

?string $name = null
来源：http://twb.zhixingplan.top

[U47] PHP：联合类型
来源：http://ank.nanxinkj.top

int|string $id
来源：http://eyn.wangdashe.top

[U48] PHP：纯枚举
来源：http://rrs.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wjn.bbcook.cn

[U49] PHP：只读属性
来源：http://rdm.shangyingyoupin.top

public readonly string $name
来源：http://nzt.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://hxc.jinyuanbaomall.cn

public function __construct(private int $id) {}
来源：http://gpf.fktsv.cn

[U51] PHP：数组解构
来源：http://yhy.ydzc1.top

[$a, $b] = $arr;
来源：http://avu.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://iyw.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://vbe.yangfankeji.com

[U53] PHP：空合并运算符
来源：http://qlz.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://rdw.cheryme.top

[U54] PHP：空安全调用
来源：http://kyw.316326.xyz

$obj?->method()
来源：http://thq.yongpay.top

[U55] PHP：match 表达式
来源：http://mky.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eub.jinqigufen.top

[U56] PHP：命名参数
来源：http://hew.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://wgx.ybcxt.top

[U57] PHP：字符串插值
来源：http://wrs.ydzc1.top

"值: {$a}"
来源：http://zid.birdmap.top

[U58] PHP：数组三件套
来源：http://qpr.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yeh.ehwqpu.com

[U59] PHP：自定义排序
来源：http://psm.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mre.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://qbv.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eno.uphjek.com

[U61] PHP：正则
来源：http://ool.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opo.tianlin.xyz

[U62] PHP：日期对象
来源：http://nxs.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iig.zhixingplan.top

[U63] PHP：文件读写
来源：http://qes.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffk.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://xjw.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://hft.jinqigufen.top

[U65] PHP：会话
来源：http://gcz.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://erp.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://bhe.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wvu.hcnkem.com

[U67] PHP：处理文件上传
来源：http://bia.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://can.yongpay.top

[U68] PHP：PDO 连接
来源：http://seo.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rue.yonumen.top

[U69] PHP：PDO 预处理
来源：http://koa.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qjf.quarkkingdee.top

[U70] PHP：PDO 事务
来源：http://jgm.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://axz.sweek.top

[U71] PHP：抛出异常
来源：http://lsi.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://czm.tianlin.xyz

[U72] PHP：写错误日志
来源：http://isa.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://bvq.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://cop.tarul.cn

parse_ini_file("config.ini", true)
来源：http://oba.yueranfly.top

[U74] PHP：读取环境变量
来源：http://qnm.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://clu.pycfn.com

[U75] PHP：依赖注入
来源：http://qtu.cdnleiting.top

composer require psr/container
来源：http://bcj.sufxvd.cn

[U76] PHP：简单路由
来源：http://wrj.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oyu.wangdashe.top

[U77] PHP：模板渲染
来源：http://zls.hnqzz.top

composer require twig/twig
来源：http://ydy.hesvh.cn

[U78] PHP：单元测试
来源：http://fcn.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://dow.haohaochexian.top

[U79] PHP：静态分析
来源：http://qec.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://skf.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://mme.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mmx.cqqwz.cn

[U81] JS：初始化项目
来源：http://xoy.zhengqikj.top

npm init -y;  npm i express
来源：http://vtu.birdmap.top

[U82] JS：package.json 脚本
来源：http://ufm.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hpd.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://bor.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://tvc.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://swx.cucudq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xgy.wangdashe.top

[U85] JS：可选链
来源：http://udb.havefunace.top

a?.b?.c
来源：http://luw.zhixingplan.top

[U86] JS：空值合并
来源：http://ndv.jinqigufen.top

a ?? b
来源：http://xyv.gzhubu.top


<!-- 参考信息 -->