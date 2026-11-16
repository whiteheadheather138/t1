代发 wailian999

[T03] Kotlin：字符串模板
来源：http://cwt.gotoacloud.top

"值: $b"
来源：http://kkl.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://duz.xuanzx.com

val n: String? = null;  n?.length
来源：http://jer.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://fpm.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pqv.ydzc1.top

[T06] Kotlin：集合映射
来源：http://pki.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xye.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://urt.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uqd.ydzc1.top

[T08] Kotlin：数据类
来源：http://pod.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://pfr.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://hsh.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://wex.uphjek.com

[T10] Kotlin：默认参数
来源：http://sqz.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://onc.pycfn.com

[T11] Kotlin：协程
来源：http://zeo.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tuy.aizwys.cn

[T12] Kotlin：解构声明
来源：http://uzg.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://lgr.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://gvp.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://lyc.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://lox.52xcode.cn

for (i in 1..10) println(i)
来源：http://ndb.wangdashe.top

[T15] Kotlin：接口
来源：http://ysg.daria6918.cn

interface Shape { fun area(): Double }
来源：http://cyl.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://rki.ehwqpu.com

print("Hello")
来源：http://qnq.ydzc1.top

[T17] Swift：变量与常量
来源：http://cpu.aizwys.cn

var a = 1;  let b = 2
来源：http://mlz.ctjpmb.com

[T18] Swift：字符串插值
来源：http://xjv.fktsv.cn

"值: \(b)"
来源：http://dlm.52xcode.cn

[T19] Swift：可选绑定
来源：http://dea.hcnkem.com

if let n = opt { print(n) }
来源：http://ymv.sxryk.cn

[T20] Swift：数组操作
来源：http://jei.jlsjyb.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nkw.52xcode.cn

[T21] Swift：遍历
来源：http://oan.yuxming.cn

for x in a { print(x) }
来源：http://eja.0kj1m.cn

[T22] Swift：字典
来源：http://rzj.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://cgg.quarkkingdee.top

[T23] Swift：函数
来源：http://nxq.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tcg.chenzaomai.com

[T24] Swift：闭包
来源：http://mml.quarkkingdee.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ppp.zhoulong.xyz

[T25] Swift：结构体
来源：http://vxi.zdqjudy.top

struct P { var x: Int }
来源：http://vtn.hnqzz.top

[T26] Swift：类与重写
来源：http://onn.sxryk.cn

class A: Base { override func f() {} }
来源：http://rwv.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://xfo.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://med.shuidangran.top

[T28] Swift：枚举
来源：http://mfn.birdmap.top

enum Color { case red, green }
来源：http://mwg.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://rmb.hfpthk.cn

guard let x = opt else { return }
来源：http://vpi.sufxvd.cn

[T30] Swift：协议
来源：http://mgy.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://gmz.yangfankeji.com

[T31] Lua：Hello World
来源：http://djl.kuanghao11.cn

print("Hello")
来源：http://irg.ivvv.top

[T32] Lua：局部变量
来源：http://quf.cdnleiting.top

local a = 1
来源：http://wsh.pycfn.com

[T33] Lua：表（数组）
来源：http://nwb.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pcb.cashguo.top

[T34] Lua：遍历表
来源：http://pgq.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wse.feifeiyinyue.top

[T35] Lua：字典表
来源：http://epj.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://rlg.zhoulong.xyz

[T36] Lua：函数
来源：http://krk.ybcxt.top

function add(a, b) return a + b end
来源：http://qvv.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://mkc.wangdashe.top

"a" .. "b"
来源：http://ted.gzhubu.top

[T38] Lua：条件
来源：http://udf.hnqzz.top

if x > 0 then print("正") end
来源：http://bmh.birdmap.top

[T39] Lua：模式匹配
来源：http://kcp.dashuyun.cn

string.find(s, "%d+")
来源：http://kyy.vehdjk.com

[T40] Lua：元表
来源：http://ftt.hcnkem.com

setmetatable({}, { __index = base })
来源：http://jnn.c1oappe.top

[T41] Perl：Hello World
来源：http://igr.nanxuanxn.top

print "Hello\n";
来源：http://ykg.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://jpv.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gbz.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://eks.hfpthk.cn

"值: $a"
来源：http://nde.guannengcc.top

[T44] Perl：条件
来源：http://cni.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://jbp.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://zgv.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://mnt.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://pes.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zug.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://mkc.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://umv.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://mwo.cucudq.cn

$s =~ s/old/new/g;
来源：http://etu.fehbvm.com

[T49] Perl：函数
来源：http://awk.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lkm.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://kfq.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ajl.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://jnj.ybcxt.top

[T51] Scala：Hello World
来源：http://ggn.meibo888.top

println("Hello")
来源：http://nto.dianchejie.cn

[T52] Scala：变量
来源：http://sxe.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://xsz.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://kpb.mhx1999.top

s"值: $b"
来源：http://xdl.hywenlv.cn

[T54] Scala：集合映射
来源：http://nqd.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://hap.tian-w.cn

[T55] Scala：集合过滤
来源：http://xhp.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://xbr.hammf.cn

[T56] Scala：样例类
来源：http://eiy.tianlin.xyz

case class User(name: String, age: Int)
来源：http://hyf.hammf.cn

[T57] Scala：模式匹配
来源：http://bws.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://oge.vqdsnc.cn

[T58] Scala：函数定义
来源：http://pdz.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://sgh.yongpay.top

[T59] Scala：循环
来源：http://rmw.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://skv.xuanzx.com

[T60] Scala：折叠
来源：http://xko.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zcr.zdbjq.cn

================================================================================
来源：http://yeh.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cph.zhiwuduotai.top

================================================================================
来源：http://hwm.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://amf.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://jeg.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://vnk.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bsy.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://vxq.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://esd.hammf.cn

[U04] Py：变量调试打印
来源：http://fet.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hbh.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://urj.aizwys.cn

list(dict.fromkeys(arr))
来源：http://she.andypj.xyz

[U06] Py：合并两个字典
来源：http://zeo.xingfuxueyuan.xyz

{**a, **b}
来源：http://uxj.andypj.xyz

[U07] Py：反转字典键值
来源：http://brd.yuxming.cn

{v: k for k, v in d.items()}
来源：http://mrg.hnqzz.top

[U08] Py：展平二维列表
来源：http://lox.ehwqpu.com

[y for x in nested for y in x]
来源：http://eub.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://ohl.gzhubu.top

max(d, key=d.get)
来源：http://xld.aibaodan.cn

[U10] Py：按值排序字典
来源：http://jhl.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://olz.xylfe.cn

[U11] Py：生成器表达式
来源：http://tmj.smart0.xyz

(x * 2 for x in arr)
来源：http://gux.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://gpn.shzxlz.cn

Counter(arr).most_common(3)
来源：http://scd.hcnkem.com

[U13] Py：固定长度队列
来源：http://ykb.bbcook.cn

deque(maxlen=10)
来源：http://pij.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://yjd.yongpay.top

defaultdict(list)
来源：http://yvp.hcnkem.com

[U15] Py：高精度计时
来源：http://gla.jyoumei.cn

t = time.perf_counter()
来源：http://xrk.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://aup.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wuz.shuidangran.top

[U17] Py：初始化日志
来源：http://smg.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://frk.tanke756.top

[U18] Py：预编译正则
来源：http://baq.bjfxy.top

pat = re.compile(r"\d+")
来源：http://tqm.fengsongda.top

[U19] Py：正则替换带回调
来源：http://vps.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fgr.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://yxg.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://rqe.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://qjj.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://nqz.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://isp.vehdjk.com

list(zip(*m))
来源：http://qsj.vehdjk.com

[U23] Py：分块读取大文件
来源：http://nrg.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yml.uphjek.com

[U24] Py：路径操作
来源：http://cqb.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dvn.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://mfx.redwolf501.top

csv.DictReader(f)
来源：http://bio.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://iil.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nrh.fengsongda.top

[U27] Py：异步 HTTP
来源：http://cbq.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://fvg.kuanghao11.cn

[U28] Py：类型别名
来源：http://zey.sweek.top

UserId = int
来源：http://ldf.redwolf501.top

[U29] Py：属性校验
来源：http://vju.jinghuilouyu.cn

@property 与 @x.setter 配合
来源：http://ovs.jinqigfzy.top

[U30] Py：数据类
来源：http://rte.pengpengdd.cyou

@dataclass(slots=True)
来源：http://yir.ydzc1.top

[U31] Py：单测
来源：http://rbx.zhiwuduotai.top

python -m pytest -q
来源：http://akw.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://mog.cashguo.top

ruff format . && ruff check --fix .
来源：http://xew.fengsongda.top

[U33] Py：打包发布
来源：http://xrn.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://bgo.sjlbkw.cn

[U34] Py：判断编码
来源：http://ldf.zhengqikj.top

chardet.detect(raw)
来源：http://pxn.yangfankeji.com

[U35] Py：发送邮件
来源：http://wir.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bdr.quarkkingdee.top

[U36] Py：定时任务
来源：http://prv.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://gak.jinqigufen.top

[U37] Py：读写 Excel
来源：http://ouh.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://vtr.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://lwk.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://ofe.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://dma.ivvv.top

sys.stdout.isatty()
来源：http://tod.meibo888.top

[U40] Py：打印到标准错误
来源：http://keg.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://wsa.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://hyd.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bja.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://lgc.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lck.yueranfly.top

[U43] PHP：声明命名空间
来源：http://kft.chenjidiqi.icu

namespace App\Http;
来源：http://pcy.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://qri.gogol.net.cn

declare(strict_types=1);
来源：http://uzn.nanxinkj.top

[U45] PHP：类型声明与返回类型
来源：http://fjv.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fvb.nanxuanxn.top

[U46] PHP：可空类型
来源：http://yki.hammf.cn

?string $name = null
来源：http://jps.cashguo.top

[U47] PHP：联合类型
来源：http://uzp.redwolf501.top

int|string $id
来源：http://duu.wangdashe.top

[U48] PHP：纯枚举
来源：http://voq.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sed.ydjk.org.cn

[U49] PHP：只读属性
来源：http://eba.mhx1999.top

public readonly string $name
来源：http://pdj.yj20258.top

[U50] PHP：构造器属性提升
来源：http://xoy.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://imo.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://tea.hywenlv.cn

[$a, $b] = $arr;
来源：http://zpf.pycfn.com

[U52] PHP：箭头函数
来源：http://yqi.zhijiandao.cn

$double = fn($x) => $x * 2;
来源：http://div.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://kek.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://isj.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://rta.hywenlv.cn

$obj?->method()
来源：http://ehr.yuanzhike.top

[U55] PHP：match 表达式
来源：http://uml.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fih.zhijiandao.cn

[U56] PHP：命名参数
来源：http://avy.yj20258.top

f(a: 1, b: 2)
来源：http://tvj.zhixingplan.top

[U57] PHP：字符串插值
来源：http://ktw.daxiang520.top

"值: {$a}"
来源：http://fmj.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://dzr.dashuyun.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cwq.jyoumei.cn

[U59] PHP：自定义排序
来源：http://amr.guannengcc.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jvo.nanxuanxn.top

[U60] PHP：JSON 编解码
来源：http://ktk.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ygv.jqgufenzy.top

[U61] PHP：正则
来源：http://yxv.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://muh.havefunace.top

[U62] PHP：日期对象
来源：http://fcn.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ics.yueranfly.top

[U63] PHP：文件读写
来源：http://nnn.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://swn.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://wcq.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://mnc.hesvh.cn

[U65] PHP：会话
来源：http://anw.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tps.vqdsnc.cn

[U66] PHP：设置 Cookie
来源：http://hnr.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rti.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://gzy.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kzv.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://fer.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gyb.vehdjk.com

[U69] PHP：PDO 预处理
来源：http://coq.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dmk.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://jkf.xuanzx.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dnp.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://mva.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://eia.chenzaomai.com

[U72] PHP：写错误日志
来源：http://ess.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://jaz.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://pcg.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://mog.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://yiu.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://che.snrcjt.cn

[U75] PHP：依赖注入
来源：http://bxg.zhoulong.xyz

composer require psr/container
来源：http://pzx.meibo888.top

[U76] PHP：简单路由
来源：http://ckk.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xeq.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://bsb.bjfxy.top

composer require twig/twig
来源：http://ufg.kuanghao11.cn

[U78] PHP：单元测试
来源：http://tyy.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://cxs.zhengqikj.top

[U79] PHP：静态分析
来源：http://dwf.jiagoushi.top

composer require --dev phpstan/phpstan
来源：http://apt.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://pmn.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://bvj.nwbrower.top

[U81] JS：初始化项目
来源：http://bft.tarul.cn

npm init -y;  npm i express
来源：http://lhp.hammf.cn

[U82] JS：package.json 脚本
来源：http://txp.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ihm.yuxming.cn

[U83] JS：ES Module 导入导出
来源：http://huq.c1oappe.top

export const a = 1;  import { a } from "./m.js";
来源：http://dno.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://drb.dashuyun.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jcf.jlsjyb.cn

[U85] JS：可选链
来源：http://dxg.wangdashe.top

a?.b?.c
来源：http://hfu.dianchejie.cn

[U86] JS：空值合并
来源：http://eui.chenzaomai.com

a ?? b
来源：http://xpj.tarul.cn

[U87] JS：解构默认值
来源：http://jqg.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://axk.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://cju.shangyingyoupin.top

{ ...a, ...b }
来源：http://quw.chenjidiqi.icu

[U89] JS：数组去重
来源：http://xna.cucudq.cn

[...new Set(arr)]
来源：http://sfh.yueranfly.top

[U90] JS：数字数组排序
来源：http://why.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://bcj.nanxuanxn.top


<!-- 参考信息 -->