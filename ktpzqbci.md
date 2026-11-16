代发 wailian999

[T05] Kotlin：when 表达式
来源：http://agu.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vqm.cucudq.cn

[T06] Kotlin：集合映射
来源：http://hpg.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yvn.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://wws.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wgw.gogol.net.cn

[T08] Kotlin：数据类
来源：http://cej.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://tbn.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://mxn.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://xkx.c1oappe.top

[T10] Kotlin：默认参数
来源：http://gld.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pvf.ivvv.top

[T11] Kotlin：协程
来源：http://smi.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ulr.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://rtr.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://tgj.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://dlg.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://odj.sysykeji.top

[T14] Kotlin：循环
来源：http://zly.0kj1m.cn

for (i in 1..10) println(i)
来源：http://rzk.yvedp.cn

[T15] Kotlin：接口
来源：http://mjv.nwbrower.top

interface Shape { fun area(): Double }
来源：http://mka.xylfe.cn

[T16] Swift：Hello World
来源：http://tyo.quarkkingdee.top

print("Hello")
来源：http://con.xuanzx.com

[T17] Swift：变量与常量
来源：http://gmr.yangfankeji.com

var a = 1;  let b = 2
来源：http://mqp.wangdashe.top

[T18] Swift：字符串插值
来源：http://mnx.zhixingplan.top

"值: \(b)"
来源：http://phd.jyoumei.cn

[T19] Swift：可选绑定
来源：http://idq.hysaishi.cn

if let n = opt { print(n) }
来源：http://pag.ivvv.top

[T20] Swift：数组操作
来源：http://xyj.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://bua.snrcjt.cn

[T21] Swift：遍历
来源：http://qxe.zycfv.cn

for x in a { print(x) }
来源：http://pfc.dianchejie.cn

[T22] Swift：字典
来源：http://tum.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://fhw.redwolf501.top

[T23] Swift：函数
来源：http://cqo.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ttn.svipenyu.cn

[T24] Swift：闭包
来源：http://pzk.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lsi.hnxiangtu.top

[T25] Swift：结构体
来源：http://dcr.shuidangran.top

struct P { var x: Int }
来源：http://igz.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://zhf.chenlongwang.top

class A: Base { override func f() {} }
来源：http://oua.zycfv.cn

[T27] Swift：错误处理
来源：http://uhq.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://lpp.ybcxt.top

[T28] Swift：枚举
来源：http://pje.xylfe.cn

enum Color { case red, green }
来源：http://dmr.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://uuw.ctjpmb.com

guard let x = opt else { return }
来源：http://sei.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://kqi.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://wux.ehwqpu.com

[T31] Lua：Hello World
来源：http://unn.zhiwuduotai.top

print("Hello")
来源：http://yyu.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://wcv.pycfn.com

local a = 1
来源：http://wyu.ehwqpu.com

[T33] Lua：表（数组）
来源：http://zrb.dianchejie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jao.vqdsnc.cn

[T34] Lua：遍历表
来源：http://jdz.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xof.pengpengdd.cyou

[T35] Lua：字典表
来源：http://rag.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://iee.feifeiyinyue.top

[T36] Lua：函数
来源：http://sqd.xinyue.icu

function add(a, b) return a + b end
来源：http://gax.haohaochexian.top

[T37] Lua：字符串拼接
来源：http://qjo.aizwys.cn

"a" .. "b"
来源：http://hml.hnxiangtu.top

[T38] Lua：条件
来源：http://yfj.yj202588.top

if x > 0 then print("正") end
来源：http://ttz.cashguo.top

[T39] Lua：模式匹配
来源：http://kfs.ydzc1.top

string.find(s, "%d+")
来源：http://qts.jinqigfzy.top

[T40] Lua：元表
来源：http://wsg.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://ocn.svipenyu.cn

[T41] Perl：Hello World
来源：http://dff.kuanghao11.cn

print "Hello\n";
来源：http://tnu.chenzaomai.com

[T42] Perl：变量类型
来源：http://fvw.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gdc.ehwqpu.com

[T43] Perl：字符串插值
来源：http://wcg.cucudq.cn

"值: $a"
来源：http://lbd.sjlbkw.cn

[T44] Perl：条件
来源：http://ogs.hammf.cn

if ($a > 0) { print "正"; }
来源：http://twc.tarul.cn

[T45] Perl：数组遍历
来源：http://dtx.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://awx.haohaochexian.top

[T46] Perl：哈希操作
来源：http://qir.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rdh.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://ryy.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tdm.haohaochexian.top

[T48] Perl：正则替换
来源：http://wna.nwbrower.top

$s =~ s/old/new/g;
来源：http://ywz.vehdjk.com

[T49] Perl：函数
来源：http://umw.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxv.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://wsa.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wpq.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://fjs.jianghu66.top

[T51] Scala：Hello World
来源：http://dzj.gzhubu.top

println("Hello")
来源：http://dxh.zdbjq.cn

[T52] Scala：变量
来源：http://eie.fktsv.cn

val a = 1;  var b = 2
来源：http://ptn.xylfe.cn

[T53] Scala：字符串插值
来源：http://sla.hesvh.cn

s"值: $b"
来源：http://xsc.daxiang520.top

[T54] Scala：集合映射
来源：http://kbn.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://lnn.jianghu66.top

[T55] Scala：集合过滤
来源：http://aqm.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hca.vehdjk.com

[T56] Scala：样例类
来源：http://pbe.gotoacloud.top

case class User(name: String, age: Int)
来源：http://dqv.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://aty.shanyushiyangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gim.jlsjyb.cn

[T58] Scala：函数定义
来源：http://jhs.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ukr.havefunace.top

[T59] Scala：循环
来源：http://xda.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://egb.yvedp.cn

[T60] Scala：折叠
来源：http://udl.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hqy.xuanzx.com

================================================================================
来源：http://idw.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cne.pengpengdd.cyou

================================================================================
来源：http://ley.cheryme.top

[U01] Py：创建虚拟环境
来源：http://vtl.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://drn.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://jzj.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bbo.yueranfly.top

[U03] Py：加载 .env 配置
来源：http://qmn.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bix.aibaodan.cn

[U04] Py：变量调试打印
来源：http://pbz.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jmg.yj20258.top

[U05] Py：列表去重且保序
来源：http://qza.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://hkv.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://hvb.ydzc1.top

{**a, **b}
来源：http://bem.ybcxt.top

[U07] Py：反转字典键值
来源：http://swk.hesvh.cn

{v: k for k, v in d.items()}
来源：http://dlg.sxryk.cn

[U08] Py：展平二维列表
来源：http://zun.ydzc1.top

[y for x in nested for y in x]
来源：http://tgk.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://abi.meibo888.top

max(d, key=d.get)
来源：http://dhn.jinqigufen.top

[U10] Py：按值排序字典
来源：http://coy.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://asx.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://frg.chenlongwang.top

(x * 2 for x in arr)
来源：http://cok.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yhw.epnwcf.com

Counter(arr).most_common(3)
来源：http://gjc.9152youxi.cn

[U13] Py：固定长度队列
来源：http://jfs.aibaodan.cn

deque(maxlen=10)
来源：http://vdn.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://jho.tarul.cn

defaultdict(list)
来源：http://lla.nanxinkj.top

[U15] Py：高精度计时
来源：http://vkz.zhijiandao.cn

t = time.perf_counter()
来源：http://adi.pycfn.com

[U16] Py：命令行参数解析
来源：http://grm.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zmz.yj20258.top

[U17] Py：初始化日志
来源：http://gpt.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://oca.hysaishi.cn

[U18] Py：预编译正则
来源：http://cyi.hammf.cn

pat = re.compile(r"\d+")
来源：http://vpw.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://fvp.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mof.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://rcw.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://zdl.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://icd.yanxiufei.cn

@contextlib.contextmanager
来源：http://djs.jlsjyb.cn

[U22] Py：矩阵转置
来源：http://xfp.cucudq.cn

list(zip(*m))
来源：http://uik.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://eaz.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tcp.wangshuangyany.cn

[U24] Py：路径操作
来源：http://noz.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xmw.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://ter.chenlongwang.top

csv.DictReader(f)
来源：http://pcr.yj20258.top

[U26] Py：并发下载
来源：http://xeh.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://neh.xylfe.cn

[U27] Py：异步 HTTP
来源：http://uir.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://lgy.nanxinkj.top

[U28] Py：类型别名
来源：http://gtk.ydzc1.top

UserId = int
来源：http://lke.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://mvn.gzhubu.top

@property 与 @x.setter 配合
来源：http://uqz.shzxlz.cn

[U30] Py：数据类
来源：http://wct.yangfankeji.com

@dataclass(slots=True)
来源：http://bem.yvedp.cn

[U31] Py：单测
来源：http://xjw.sxryk.cn

python -m pytest -q
来源：http://xoo.tarul.cn

[U32] Py：代码格式化
来源：http://kat.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://gvw.sufxvd.cn

[U33] Py：打包发布
来源：http://aof.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://lur.vqdsnc.cn

[U34] Py：判断编码
来源：http://tep.aizwys.cn

chardet.detect(raw)
来源：http://vxx.zhoulong.xyz

[U35] Py：发送邮件
来源：http://dag.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vut.yj20258.top

[U36] Py：定时任务
来源：http://wfa.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://bzt.9152youxi.cn

[U37] Py：读写 Excel
来源：http://ykn.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://con.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://wfl.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://ael.ydzc1.top

[U39] Py：判断是否在交互环境
来源：http://dnw.gotoacloud.top

sys.stdout.isatty()
来源：http://onz.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://cps.tianlin.xyz

print("err", file=sys.stderr)
来源：http://ywl.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://zyz.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wzv.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://req.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://omk.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://wji.yanxiufei.cn

namespace App\Http;
来源：http://hvn.svipenyu.cn

[U44] PHP：开启严格类型
来源：http://nzw.ctjpmb.com

declare(strict_types=1);
来源：http://cxa.sweek.top

[U45] PHP：类型声明与返回类型
来源：http://gao.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cku.nwbrower.top

[U46] PHP：可空类型
来源：http://kfi.ehwqpu.com

?string $name = null
来源：http://rqx.yj20258888.top

[U47] PHP：联合类型
来源：http://jmu.9152youxi.cn

int|string $id
来源：http://xen.tian-w.cn

[U48] PHP：纯枚举
来源：http://ikh.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gar.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://zef.fzhhl.top

public readonly string $name
来源：http://stl.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://sbm.hfpthk.cn

public function __construct(private int $id) {}
来源：http://qse.jinghuilouyu.cn

[U51] PHP：数组解构
来源：http://vwa.fehbvm.com

[$a, $b] = $arr;
来源：http://ihe.yangfankeji.com

[U52] PHP：箭头函数
来源：http://sck.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://pir.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://ahp.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://hzy.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://cyb.52xcode.cn

$obj?->method()
来源：http://ezw.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://dun.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lqo.hnqzz.top

[U56] PHP：命名参数
来源：http://svf.vqdsnc.cn

f(a: 1, b: 2)
来源：http://fbu.hcnkem.com

[U57] PHP：字符串插值
来源：http://def.tianlin.xyz

"值: {$a}"
来源：http://zdu.hywenlv.cn

[U58] PHP：数组三件套
来源：http://bvk.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vcw.dianchejie.cn

[U59] PHP：自定义排序
来源：http://dtx.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgn.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://yvs.guowangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pbr.xinyue.icu

[U61] PHP：正则
来源：http://wok.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://goj.yongpay.top

[U62] PHP：日期对象
来源：http://foe.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ipt.52xcode.cn

[U63] PHP：文件读写
来源：http://ied.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://onw.52xcode.cn

[U64] PHP：目录遍历
来源：http://iuk.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://lst.chenzaomai.com

[U65] PHP：会话
来源：http://jlu.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hzf.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://sxy.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sxl.nanxinkj.top

[U67] PHP：处理文件上传
来源：http://gut.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zox.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://uvu.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://paw.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://uaa.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sof.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://umj.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://myv.cucudq.cn

[U71] PHP：抛出异常
来源：http://ckq.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://two.guannengcc.top

[U72] PHP：写错误日志
来源：http://rdj.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://arx.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://eqf.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://znj.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://lnh.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://uuw.chenlongwang.top

[U75] PHP：依赖注入
来源：http://ncv.gotoacloud.top

composer require psr/container
来源：http://ybz.gogol.net.cn

[U76] PHP：简单路由
来源：http://lix.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjo.vehdjk.com

[U77] PHP：模板渲染
来源：http://vgr.tianlin.xyz

composer require twig/twig
来源：http://ubo.svipenyu.cn

[U78] PHP：单元测试
来源：http://qxw.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://dou.fanxiaobao.xyz

[U79] PHP：静态分析
来源：http://roo.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://ghw.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://txl.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://usi.guannengcc.top

[U81] JS：初始化项目
来源：http://eda.hnqzz.top

npm init -y;  npm i express
来源：http://ugf.epnwcf.com

[U82] JS：package.json 脚本
来源：http://xpa.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aht.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://spz.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://pak.iojbl.cn

[U84] JS：CommonJS 写法
来源：http://qtx.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://nub.xuetiantiany.cn

[U85] JS：可选链
来源：http://ejq.shanyushiyangkeji.top

a?.b?.c
来源：http://sim.chenjidiqi.icu

[U86] JS：空值合并
来源：http://qiw.xuetiantiany.cn

a ?? b
来源：http://fqe.birdmap.top

[U87] JS：解构默认值
来源：http://lfm.bjfxy.top

const { a = 1, b = 2 } = obj;
来源：http://omi.zhengqikj.top

[U88] JS：对象展开合并
来源：http://ryr.cdnleiting.top

{ ...a, ...b }
来源：http://yie.hnqzz.top

[U89] JS：数组去重
来源：http://xtx.jqgfzy.top

[...new Set(arr)]
来源：http://vxy.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://dii.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://ken.c1oappe.top

[U91] JS：对象键值遍历
来源：http://dbf.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jtg.hfpthk.cn

[U92] JS：深拷贝
来源：http://qqx.nwbrower.top

structuredClone(obj)
来源：http://obx.daxiang520.top


<!-- 参考信息 -->