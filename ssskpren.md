代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wci.tian-w.cn

================================================================================
来源：http://xzc.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://psg.shanyushiyangkeji.top

================================================================================
来源：http://wqd.yonumen.top

[T01] Kotlin：Hello World
来源：http://veu.zhiwuduotai.top

println("Hello")
来源：http://pqf.daria6918.cn

[T02] Kotlin：变量
来源：http://plm.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ydc.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://aym.yuanzhike.top

"值: $b"
来源：http://jlq.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://ydx.dianchejie.cn

val n: String? = null;  n?.length
来源：http://kqj.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://mla.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hii.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://oiy.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mwz.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://uic.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://swk.zdbjq.cn

[T08] Kotlin：数据类
来源：http://tud.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://dvv.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://nnu.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://ztx.yuxming.cn

[T10] Kotlin：默认参数
来源：http://wrr.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nws.ydzc1.top

[T11] Kotlin：协程
来源：http://fpd.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tba.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://waz.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://ays.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://ved.yongpay.top

val m = mapOf("a" to 1)
来源：http://hpp.ydjk.org.cn

[T14] Kotlin：循环
来源：http://qnm.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://the.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://zbn.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://vlx.zhixingplan.top

[T16] Swift：Hello World
来源：http://xww.yanxiufei.cn

print("Hello")
来源：http://jqw.birdmap.top

[T17] Swift：变量与常量
来源：http://gad.hnqzz.top

var a = 1;  let b = 2
来源：http://hcl.andypj.xyz

[T18] Swift：字符串插值
来源：http://cir.ydjk.org.cn

"值: \(b)"
来源：http://uey.cheryme.top

[T19] Swift：可选绑定
来源：http://umr.ctjpmb.com

if let n = opt { print(n) }
来源：http://rvi.jqgufenzy.top

[T20] Swift：数组操作
来源：http://gku.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://hjz.nanxinkj.top

[T21] Swift：遍历
来源：http://vml.gotoacloud.top

for x in a { print(x) }
来源：http://goh.yonumen.top

[T22] Swift：字典
来源：http://ofg.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://btn.yonumen.top

[T23] Swift：函数
来源：http://ggk.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvp.xuanzx.com

[T24] Swift：闭包
来源：http://xnr.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sil.yuxming.cn

[T25] Swift：结构体
来源：http://nsa.jqgfzy.top

struct P { var x: Int }
来源：http://rqw.yanxiufei.cn

[T26] Swift：类与重写
来源：http://nsu.jqgfzy.top

class A: Base { override func f() {} }
来源：http://jwx.yj20258888.top

[T27] Swift：错误处理
来源：http://ymw.tanke756.top

do { try f() } catch { print(error) }
来源：http://nua.sweek.top

[T28] Swift：枚举
来源：http://jul.gotoacloud.top

enum Color { case red, green }
来源：http://qni.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://vlh.xziqi.cn

guard let x = opt else { return }
来源：http://cnr.zhixingplan.top

[T30] Swift：协议
来源：http://pmm.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://jkc.aibaodan.cn

[T31] Lua：Hello World
来源：http://mmm.ivvv.top

print("Hello")
来源：http://uvn.kuanghao11.cn

[T32] Lua：局部变量
来源：http://lgo.yuanzhike.top

local a = 1
来源：http://zgu.hnxiangtu.top

[T33] Lua：表（数组）
来源：http://phy.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sqw.yangfankeji.com

[T34] Lua：遍历表
来源：http://kxd.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qpu.kuanghao11.cn

[T35] Lua：字典表
来源：http://sgd.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://bff.vqdsnc.cn

[T36] Lua：函数
来源：http://enw.yvedp.cn

function add(a, b) return a + b end
来源：http://phg.zycfv.cn

[T37] Lua：字符串拼接
来源：http://hni.yongpay.top

"a" .. "b"
来源：http://myz.hysaishi.cn

[T38] Lua：条件
来源：http://syy.ivvv.top

if x > 0 then print("正") end
来源：http://jki.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://rnh.snrcjt.cn

string.find(s, "%d+")
来源：http://bfx.fzhhl.top

[T40] Lua：元表
来源：http://ngp.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://lkk.ydzc1.top

[T41] Perl：Hello World
来源：http://hvd.cqqwz.cn

print "Hello\n";
来源：http://bep.fehbvm.com

[T42] Perl：变量类型
来源：http://uad.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpo.guannengcc.top

[T43] Perl：字符串插值
来源：http://wke.zhongyouzk.top

"值: $a"
来源：http://frw.jiagoushi.top

[T44] Perl：条件
来源：http://hgz.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://hec.iojbl.cn

[T45] Perl：数组遍历
来源：http://mkt.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://icy.zdqjudy.top

[T46] Perl：哈希操作
来源：http://jfu.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lxb.cqqwz.cn

[T47] Perl：正则捕获
来源：http://bvc.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://twx.daria6918.cn

[T48] Perl：正则替换
来源：http://mol.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://fox.guowangkeji.top

[T49] Perl：函数
来源：http://fqh.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxy.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://egw.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eua.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://nvj.yongpay.top

[T51] Scala：Hello World
来源：http://vkv.hywenlv.cn

println("Hello")
来源：http://bjs.jinqigfzy.top

[T52] Scala：变量
来源：http://onl.zhengqikj.top

val a = 1;  var b = 2
来源：http://mjn.cqqwz.cn

[T53] Scala：字符串插值
来源：http://pct.guannengcc.top

s"值: $b"
来源：http://rxm.gogol.net.cn

[T54] Scala：集合映射
来源：http://qrb.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://omf.feifeiyinyue.top

[T55] Scala：集合过滤
来源：http://baj.hongshengwenyu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ktt.jqgfzy.top

[T56] Scala：样例类
来源：http://xwg.ivvv.top

case class User(name: String, age: Int)
来源：http://kty.cashguo.top

[T57] Scala：模式匹配
来源：http://kng.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dqv.jlsjyb.cn

[T58] Scala：函数定义
来源：http://zyz.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://uue.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://tui.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://plc.epnwcf.com

[T60] Scala：折叠
来源：http://kum.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ohp.sysykeji.top

================================================================================
来源：http://sto.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qqf.sweek.top

================================================================================
来源：http://jny.smart0.xyz

[U01] Py：创建虚拟环境
来源：http://mpu.jqgfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://vjo.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://ncm.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ttl.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://xfn.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tcg.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://ahw.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qyz.yongpay.top

[U05] Py：列表去重且保序
来源：http://uqx.yfazqb.com

list(dict.fromkeys(arr))
来源：http://zoi.birdmap.top

[U06] Py：合并两个字典
来源：http://jbm.xingfuxueyuan.xyz

{**a, **b}
来源：http://uop.daxiang520.top

[U07] Py：反转字典键值
来源：http://xuv.iojbl.cn

{v: k for k, v in d.items()}
来源：http://gyb.uphjek.com

[U08] Py：展平二维列表
来源：http://mqt.sysykeji.top

[y for x in nested for y in x]
来源：http://oej.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://osu.hongshengwenyu.top

max(d, key=d.get)
来源：http://dcx.nanxinkj.top

[U10] Py：按值排序字典
来源：http://bfv.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://djf.cdnleiting.top

[U11] Py：生成器表达式
来源：http://kjp.zhixingplan.top

(x * 2 for x in arr)
来源：http://qgc.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://mom.yueranfly.top

Counter(arr).most_common(3)
来源：http://htj.epnwcf.com

[U13] Py：固定长度队列
来源：http://qrb.shuidangran.top

deque(maxlen=10)
来源：http://rww.yvedp.cn

[U14] Py：分组收集到列表
来源：http://jml.shuidangran.top

defaultdict(list)
来源：http://kcf.sufxvd.cn

[U15] Py：高精度计时
来源：http://fuv.chenlongwang.top

t = time.perf_counter()
来源：http://xcm.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://cth.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yof.sysykeji.top

[U17] Py：初始化日志
来源：http://owd.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://zvr.hywenlv.cn

[U18] Py：预编译正则
来源：http://azm.ybcxt.top

pat = re.compile(r"\d+")
来源：http://kao.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://dqe.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xsj.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://eba.birdmap.top

@functools.lru_cache(maxsize=None)
来源：http://dhw.dashuyun.cn

[U21] Py：自定义上下文管理器
来源：http://rck.guowangkeji.top

@contextlib.contextmanager
来源：http://egp.ydzc1.top

[U22] Py：矩阵转置
来源：http://lug.chenzaomai.com

list(zip(*m))
来源：http://vzd.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://abx.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rmf.wangdashe.top

[U24] Py：路径操作
来源：http://ycq.yangfankeji.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vua.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://xwl.zhiwuduotai.top

csv.DictReader(f)
来源：http://gbp.zycfv.cn

[U26] Py：并发下载
来源：http://wqc.hcnkem.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ugp.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://slv.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://buv.yueranfly.top

[U28] Py：类型别名
来源：http://ado.chenjidiqi.icu

UserId = int
来源：http://yhj.jyoumei.cn

[U29] Py：属性校验
来源：http://hxz.mhx1999.top

@property 与 @x.setter 配合
来源：http://asa.cqqwz.cn

[U30] Py：数据类
来源：http://vgz.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://euj.sweek.top

[U31] Py：单测
来源：http://mfn.hfpthk.cn

python -m pytest -q
来源：http://knd.bbcook.cn

[U32] Py：代码格式化
来源：http://gio.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://hmx.hfpthk.cn

[U33] Py：打包发布
来源：http://ofi.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://xrb.tanke756.top

[U34] Py：判断编码
来源：http://wnj.vqdsnc.cn

chardet.detect(raw)
来源：http://tqy.zhixingplan.top

[U35] Py：发送邮件
来源：http://ijb.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://atl.dianchejie.cn

[U36] Py：定时任务
来源：http://qym.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://wbb.shuidangran.top

[U37] Py：读写 Excel
来源：http://lom.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://gmj.xinyue.icu

[U38] Py：获取脚本所在目录
来源：http://ysp.tanke756.top

Path(__file__).resolve().parent
来源：http://byx.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://nzb.havefunace.top

sys.stdout.isatty()
来源：http://spc.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://nie.yj20258888.top

print("err", file=sys.stderr)
来源：http://qyr.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://pyo.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://gay.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://zwq.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rzl.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://trr.sufxvd.cn

namespace App\Http;
来源：http://ceg.hammf.cn

[U44] PHP：开启严格类型
来源：http://qls.c1oappe.top

declare(strict_types=1);
来源：http://fna.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://mef.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://olp.yj202588.top

[U46] PHP：可空类型
来源：http://scs.yuanzhike.top

?string $name = null
来源：http://nwn.zdqjudy.top

[U47] PHP：联合类型
来源：http://xwg.xuanzx.com

int|string $id
来源：http://qiv.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://rwy.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xxv.sweek.top

[U49] PHP：只读属性
来源：http://eqs.yfazqb.com

public readonly string $name
来源：http://cik.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://cct.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://xeu.ctjpmb.com

[U51] PHP：数组解构
来源：http://oph.nwbrower.top

[$a, $b] = $arr;
来源：http://gsy.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://qjt.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://jrx.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://xmh.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://ero.gzhubu.top

[U54] PHP：空安全调用
来源：http://kcn.vehdjk.com

$obj?->method()
来源：http://psh.hammf.cn

[U55] PHP：match 表达式
来源：http://koi.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ynp.cdnleiting.top

[U56] PHP：命名参数
来源：http://edl.tian-w.cn

f(a: 1, b: 2)
来源：http://yix.52xcode.cn

[U57] PHP：字符串插值
来源：http://fqp.vehdjk.com

"值: {$a}"
来源：http://tbd.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://jnt.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bzi.ivvv.top

[U59] PHP：自定义排序
来源：http://ymf.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://snd.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://ofu.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rtl.xuetiantiany.cn

[U61] PHP：正则
来源：http://ksz.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kun.jyoumei.cn

[U62] PHP：日期对象
来源：http://jpk.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jqo.sxryk.cn

[U63] PHP：文件读写
来源：http://ccb.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ndr.shzxlz.cn

[U64] PHP：目录遍历
来源：http://tig.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://zgh.xuetiantiany.cn

[U65] PHP：会话
来源：http://brk.birdmap.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dgp.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://vnf.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ukh.wangdashe.top

[U67] PHP：处理文件上传
来源：http://kuq.hysaishi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ewz.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://pph.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lmn.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://gmo.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tam.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://jww.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zkj.chenzaomai.com

[U71] PHP：抛出异常
来源：http://zdq.sweek.top

throw new RuntimeException("失败", 500);
来源：http://rml.tarul.cn

[U72] PHP：写错误日志
来源：http://tmq.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://gyk.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://ujw.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://bis.sysykeji.top

[U74] PHP：读取环境变量
来源：http://usf.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://kqk.hnqzz.top

[U75] PHP：依赖注入
来源：http://gye.52xcode.cn

composer require psr/container
来源：http://own.cheryme.top

[U76] PHP：简单路由
来源：http://mgd.xingfuxueyuan.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ldr.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://xxk.jlsjyb.cn

composer require twig/twig
来源：http://hxg.hnxiangtu.top

[U78] PHP：单元测试
来源：http://gfm.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://jpi.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://rfm.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://pyq.hnqzz.top

[U80] PHP：代码规范修复
来源：http://xhd.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bft.sxryk.cn

[U81] JS：初始化项目
来源：http://hjd.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://vtz.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://bqs.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wmc.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://zvy.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://aby.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://fbl.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://orb.shangyingyoupin.top

[U85] JS：可选链
来源：http://ohj.zycfv.cn

a?.b?.c
来源：http://rjx.zhoulong.xyz

[U86] JS：空值合并
来源：http://qvb.zycfv.cn

a ?? b
来源：http://btg.bjfxy.top


<!-- 参考信息 -->