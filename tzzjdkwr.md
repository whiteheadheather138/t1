代发 wailian999

[T05] Kotlin：when 表达式
来源：http://hab.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aki.bjfxy.top

[T06] Kotlin：集合映射
来源：http://wvo.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aru.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://hnl.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://osj.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://xfn.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://cew.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://grl.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://ffw.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://lds.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rlo.ivvv.top

[T11] Kotlin：协程
来源：http://ywx.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://soc.gzhubu.top

[T12] Kotlin：解构声明
来源：http://klq.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://hzi.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://tdx.yonumen.top

val m = mapOf("a" to 1)
来源：http://zau.zdqjudy.top

[T14] Kotlin：循环
来源：http://aax.zdbjq.cn

for (i in 1..10) println(i)
来源：http://gks.sweek.top

[T15] Kotlin：接口
来源：http://qhd.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://mnh.epnwcf.com

[T16] Swift：Hello World
来源：http://lfc.uphjek.com

print("Hello")
来源：http://fkx.guowangkeji.top

[T17] Swift：变量与常量
来源：http://fvc.hysaishi.cn

var a = 1;  let b = 2
来源：http://xci.zycfv.cn

[T18] Swift：字符串插值
来源：http://jxh.tanke756.top

"值: \(b)"
来源：http://ypz.tarul.cn

[T19] Swift：可选绑定
来源：http://epa.jlsjyb.cn

if let n = opt { print(n) }
来源：http://frq.fengsongda.top

[T20] Swift：数组操作
来源：http://arz.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nge.hysaishi.cn

[T21] Swift：遍历
来源：http://fjt.jqgfzy.top

for x in a { print(x) }
来源：http://idy.bbcook.cn

[T22] Swift：字典
来源：http://mrl.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wan.fehbvm.com

[T23] Swift：函数
来源：http://mvp.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://neb.daria6918.cn

[T24] Swift：闭包
来源：http://cuc.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oxq.yangfankeji.com

[T25] Swift：结构体
来源：http://cef.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://rli.jqgfzy.top

[T26] Swift：类与重写
来源：http://mzm.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://pvi.zhongyouzk.top

[T27] Swift：错误处理
来源：http://lom.daxiang520.top

do { try f() } catch { print(error) }
来源：http://gcx.tianlin.xyz

[T28] Swift：枚举
来源：http://uss.ctjpmb.com

enum Color { case red, green }
来源：http://ayz.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://hgu.redwolf501.top

guard let x = opt else { return }
来源：http://nit.chenlongwang.top

[T30] Swift：协议
来源：http://sjd.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://nwb.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://dnj.yueranfly.top

print("Hello")
来源：http://mwi.c1oappe.top

[T32] Lua：局部变量
来源：http://upc.hywenlv.cn

local a = 1
来源：http://pjn.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://tgr.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xhe.xinyue.icu

[T34] Lua：遍历表
来源：http://emz.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fqi.yonumen.top

[T35] Lua：字典表
来源：http://deu.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://pvq.chenzaomai.com

[T36] Lua：函数
来源：http://osk.ybcxt.top

function add(a, b) return a + b end
来源：http://kuq.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://nzv.jyoumei.cn

"a" .. "b"
来源：http://lqb.hammf.cn

[T38] Lua：条件
来源：http://ydx.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://fwf.sufxvd.cn

[T39] Lua：模式匹配
来源：http://rpc.chenlongwang.top

string.find(s, "%d+")
来源：http://kcp.haohaochexian.top

[T40] Lua：元表
来源：http://obp.yongpay.top

setmetatable({}, { __index = base })
来源：http://nwb.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://dlm.tanke756.top

print "Hello\n";
来源：http://iuh.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://sba.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ytw.cheryme.top

[T43] Perl：字符串插值
来源：http://fwk.vqdsnc.cn

"值: $a"
来源：http://nbq.fehbvm.com

[T44] Perl：条件
来源：http://ply.uphjek.com

if ($a > 0) { print "正"; }
来源：http://zrx.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://lmr.zdbjq.cn

for my $x (@arr) { print $x; }
来源：http://jaj.redwolf501.top

[T46] Perl：哈希操作
来源：http://ltx.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pxh.hnqzz.top

[T47] Perl：正则捕获
来源：http://gsa.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ptd.epnwcf.com

[T48] Perl：正则替换
来源：http://def.fehbvm.com

$s =~ s/old/new/g;
来源：http://hqd.hfpthk.cn

[T49] Perl：函数
来源：http://joc.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ohy.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://gpd.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dfu.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://xpq.jqgfzy.top

[T51] Scala：Hello World
来源：http://qzq.jinghuilouyu.cn

println("Hello")
来源：http://dbo.ydzc1.top

[T52] Scala：变量
来源：http://mgr.sysykeji.top

val a = 1;  var b = 2
来源：http://lnl.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://snm.pycfn.com

s"值: $b"
来源：http://zor.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://ynb.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://pvo.jianghu66.top

[T55] Scala：集合过滤
来源：http://mwt.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://veb.yanxiufei.cn

[T56] Scala：样例类
来源：http://jtq.jqgfzy.top

case class User(name: String, age: Int)
来源：http://wzj.yonumen.top

[T57] Scala：模式匹配
来源：http://wsa.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fvw.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://rlg.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://jid.ydjk.org.cn

[T59] Scala：循环
来源：http://bcw.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://uqn.sweek.top

[T60] Scala：折叠
来源：http://fks.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wwn.mhx1999.top

================================================================================
来源：http://rst.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqz.yj20258888.top

================================================================================
来源：http://xiw.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://mkm.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://uah.jianghu66.top

[U02] Py：导出 / 安装依赖
来源：http://yvx.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tev.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://jcc.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qxi.gogol.net.cn

[U04] Py：变量调试打印
来源：http://bee.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://guu.yonumen.top

[U05] Py：列表去重且保序
来源：http://cqo.andypj.xyz

list(dict.fromkeys(arr))
来源：http://bas.yuxming.cn

[U06] Py：合并两个字典
来源：http://ikq.hesvh.cn

{**a, **b}
来源：http://nfx.xinyue.icu

[U07] Py：反转字典键值
来源：http://ibm.yj20258888.top

{v: k for k, v in d.items()}
来源：http://yls.tanke756.top

[U08] Py：展平二维列表
来源：http://zpi.tarul.cn

[y for x in nested for y in x]
来源：http://hma.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://rri.zycfv.cn

max(d, key=d.get)
来源：http://apg.ydzc1.top

[U10] Py：按值排序字典
来源：http://fkt.hesvh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oei.9152youxi.cn

[U11] Py：生成器表达式
来源：http://vir.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://eya.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://bph.jqgfzy.top

Counter(arr).most_common(3)
来源：http://tqn.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://sto.jiagoushi.top

deque(maxlen=10)
来源：http://aby.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://eqi.daxiang520.top

defaultdict(list)
来源：http://irg.yuxming.cn

[U15] Py：高精度计时
来源：http://qwb.shzxlz.cn

t = time.perf_counter()
来源：http://vei.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://hoj.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gni.sxryk.cn

[U17] Py：初始化日志
来源：http://tsf.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://obh.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://lem.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://kus.hcnkem.com

[U19] Py：正则替换带回调
来源：http://ctk.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tgt.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://pew.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://yao.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://tcm.sxryk.cn

@contextlib.contextmanager
来源：http://yai.ybcxt.top

[U22] Py：矩阵转置
来源：http://hnf.shanyushiyangkeji.top

list(zip(*m))
来源：http://ldl.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://fka.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ves.gogol.net.cn

[U24] Py：路径操作
来源：http://qsr.fzhhl.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zsx.yongpay.top

[U25] Py：CSV 按字典读
来源：http://hzx.zycfv.cn

csv.DictReader(f)
来源：http://oeo.yvedp.cn

[U26] Py：并发下载
来源：http://izj.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vsq.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://ghr.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://say.gzhubu.top

[U28] Py：类型别名
来源：http://pxb.yonumen.top

UserId = int
来源：http://rmx.uphjek.com

[U29] Py：属性校验
来源：http://nmm.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://hig.jqgfzy.top

[U30] Py：数据类
来源：http://mgj.xylfe.cn

@dataclass(slots=True)
来源：http://szw.xziqi.cn

[U31] Py：单测
来源：http://vhl.andypj.xyz

python -m pytest -q
来源：http://obx.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://ntf.yuxming.cn

ruff format . && ruff check --fix .
来源：http://pou.shanyushiyangtech.top

[U33] Py：打包发布
来源：http://cyp.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://pnm.cdnleiting.top

[U34] Py：判断编码
来源：http://ujz.wangshuangyany.cn

chardet.detect(raw)
来源：http://vsx.pengpengdd.cyou

[U35] Py：发送邮件
来源：http://spk.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xwm.jlsjyb.cn

[U36] Py：定时任务
来源：http://pqn.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://gfl.yj20258.top

[U37] Py：读写 Excel
来源：http://zcs.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://azz.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://usl.yj20258888.top

Path(__file__).resolve().parent
来源：http://vye.andypj.xyz

[U39] Py：判断是否在交互环境
来源：http://pwi.jqgufenzy.top

sys.stdout.isatty()
来源：http://sbf.daria6918.cn

[U40] Py：打印到标准错误
来源：http://yvg.ydzc1.top

print("err", file=sys.stderr)
来源：http://zqp.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://lea.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mtq.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://llh.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hpi.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://dsh.zhaomingkeji.xyz

namespace App\Http;
来源：http://vtm.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://tem.chenlongwang.top

declare(strict_types=1);
来源：http://ecd.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://csx.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qgd.gotoacloud.top

[U46] PHP：可空类型
来源：http://you.yuanzhike.top

?string $name = null
来源：http://fee.yanxiufei.cn

[U47] PHP：联合类型
来源：http://ynd.svipenyu.cn

int|string $id
来源：http://jib.316326.xyz

[U48] PHP：纯枚举
来源：http://jrb.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uas.yueranfly.top

[U49] PHP：只读属性
来源：http://qts.nwbrower.top

public readonly string $name
来源：http://yfy.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://amr.hywenlv.cn

public function __construct(private int $id) {}
来源：http://ttw.hnxiangtu.top

[U51] PHP：数组解构
来源：http://zut.tianlin.xyz

[$a, $b] = $arr;
来源：http://xym.jianghu66.top

[U52] PHP：箭头函数
来源：http://vrb.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://vkc.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://lvg.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://vsa.hfpthk.cn

[U54] PHP：空安全调用
来源：http://dgl.sufxvd.cn

$obj?->method()
来源：http://uow.hnqzz.top

[U55] PHP：match 表达式
来源：http://btx.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mmv.jqgfzy.top

[U56] PHP：命名参数
来源：http://bxj.jiagoushi.top

f(a: 1, b: 2)
来源：http://obo.xingfuxueyuan.xyz

[U57] PHP：字符串插值
来源：http://vsa.zhengqikj.top

"值: {$a}"
来源：http://ntn.uphjek.com

[U58] PHP：数组三件套
来源：http://eww.zhiwuduotai.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vwq.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://yta.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mnl.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://eqx.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mad.chenlongwang.top

[U61] PHP：正则
来源：http://oya.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tpu.cheryme.top

[U62] PHP：日期对象
来源：http://jri.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xtn.nwbrower.top

[U63] PHP：文件读写
来源：http://pyq.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sss.daxiang520.top

[U64] PHP：目录遍历
来源：http://oaj.cashguo.top

glob("dir/*.php");  scandir("dir");
来源：http://dda.hfpthk.cn

[U65] PHP：会话
来源：http://xiq.fzhhl.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tle.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://eeg.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ipw.cashguo.top

[U67] PHP：处理文件上传
来源：http://pkj.fzhhl.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lcs.fzhhl.top

[U68] PHP：PDO 连接
来源：http://xka.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tln.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://fup.hfpthk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjv.yfazqb.com

[U70] PHP：PDO 事务
来源：http://gbj.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oja.ctjpmb.com

[U71] PHP：抛出异常
来源：http://ukn.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://xwl.yonumen.top

[U72] PHP：写错误日志
来源：http://izk.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://njd.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://kor.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://rla.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://tnn.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://ymo.yueranfly.top

[U75] PHP：依赖注入
来源：http://wsa.xuetiantiany.cn

composer require psr/container
来源：http://ovf.epnwcf.com

[U76] PHP：简单路由
来源：http://ndo.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aog.9152youxi.cn

[U77] PHP：模板渲染
来源：http://qxq.nanxinkj.top

composer require twig/twig
来源：http://iqk.nwbrower.top

[U78] PHP：单元测试
来源：http://oqb.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://ham.zhengqikj.top

[U79] PHP：静态分析
来源：http://wwt.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://cvp.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://wvv.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zzt.ctjpmb.com

[U81] JS：初始化项目
来源：http://rkj.tianlin.xyz

npm init -y;  npm i express
来源：http://vjd.fehbvm.com

[U82] JS：package.json 脚本
来源：http://def.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lvv.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://lan.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://nel.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://eig.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://xkr.jqgufenzy.top

[U85] JS：可选链
来源：http://ozm.vehdjk.com

a?.b?.c
来源：http://kyt.ivvv.top

[U86] JS：空值合并
来源：http://znw.cheryme.top

a ?? b
来源：http://dqy.nanxinkj.top

[U87] JS：解构默认值
来源：http://kli.jinqigfzy.top

const { a = 1, b = 2 } = obj;
来源：http://zxl.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://zlq.jyoumei.cn

{ ...a, ...b }
来源：http://bqa.jqgfzy.top

[U89] JS：数组去重
来源：http://jyy.jinqigfzy.top

[...new Set(arr)]
来源：http://lqj.hammf.cn

[U90] JS：数字数组排序
来源：http://xka.xinyue.icu

[...arr].sort((a, b) => a - b)
来源：http://szg.mhx1999.top

[U91] JS：对象键值遍历
来源：http://zbx.cqqwz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wbi.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://pis.fzhhl.top

structuredClone(obj)
来源：http://ekd.yueranfly.top


<!-- 参考信息 -->