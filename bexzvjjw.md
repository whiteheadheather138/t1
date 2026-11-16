代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://swm.xylfe.cn

================================================================================
来源：http://jwn.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://itr.jqgfzy.top

================================================================================
来源：http://cmt.xinyue.icu

[T01] Kotlin：Hello World
来源：http://dkd.sufxvd.cn

println("Hello")
来源：http://nup.jyoumei.cn

[T02] Kotlin：变量
来源：http://kpr.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rqg.cheryme.top

[T03] Kotlin：字符串模板
来源：http://cqe.yj20258.top

"值: $b"
来源：http://aan.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://hzh.redwolf501.top

val n: String? = null;  n?.length
来源：http://wge.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://xdy.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qqh.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://kqq.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://akl.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://yrc.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://isb.yonumen.top

[T08] Kotlin：数据类
来源：http://emc.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://nri.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://tvt.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://hdt.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://pnf.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dbt.nanxuanxn.top

[T11] Kotlin：协程
来源：http://wme.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fse.hcnkem.com

[T12] Kotlin：解构声明
来源：http://noj.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://mwm.pycfn.com

[T13] Kotlin：只读 Map
来源：http://ubx.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://lit.zhijiandao.cn

[T14] Kotlin：循环
来源：http://xlj.haohaochexian.top

for (i in 1..10) println(i)
来源：http://qzw.zhoulong.xyz

[T15] Kotlin：接口
来源：http://wvx.epnwcf.com

interface Shape { fun area(): Double }
来源：http://slo.cheryme.top

[T16] Swift：Hello World
来源：http://ceh.wangdashe.top

print("Hello")
来源：http://myr.sxryk.cn

[T17] Swift：变量与常量
来源：http://okl.meibo888.top

var a = 1;  let b = 2
来源：http://vjh.tarul.cn

[T18] Swift：字符串插值
来源：http://due.yangfankeji.com

"值: \(b)"
来源：http://stb.zdqjudy.top

[T19] Swift：可选绑定
来源：http://cxt.chenlongwang.top

if let n = opt { print(n) }
来源：http://ocm.jlsjyb.cn

[T20] Swift：数组操作
来源：http://ijj.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wsv.ydjk.org.cn

[T21] Swift：遍历
来源：http://kob.shanyushiyangtech.top

for x in a { print(x) }
来源：http://fqe.xylfe.cn

[T22] Swift：字典
来源：http://aln.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://acp.haohaochexian.top

[T23] Swift：函数
来源：http://txy.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zhd.fzhhl.top

[T24] Swift：闭包
来源：http://vut.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://duq.c1oappe.top

[T25] Swift：结构体
来源：http://xda.gotoacloud.top

struct P { var x: Int }
来源：http://dtv.yj202588.top

[T26] Swift：类与重写
来源：http://yfo.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://kwm.ivvv.top

[T27] Swift：错误处理
来源：http://mnq.iojbl.cn

do { try f() } catch { print(error) }
来源：http://yya.zdqjudy.top

[T28] Swift：枚举
来源：http://ehj.yanxiufei.cn

enum Color { case red, green }
来源：http://ndz.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://gyh.hcnkem.com

guard let x = opt else { return }
来源：http://qzn.cqqwz.cn

[T30] Swift：协议
来源：http://kre.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://wsr.nanxuanxn.top

[T31] Lua：Hello World
来源：http://ygu.cqqwz.cn

print("Hello")
来源：http://rjq.cdnleiting.top

[T32] Lua：局部变量
来源：http://hdm.shanyushiyangkeji.top

local a = 1
来源：http://cmc.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://fxy.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://vck.shuidangran.top

[T34] Lua：遍历表
来源：http://fwz.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://spc.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://bii.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://lwu.svipenyu.cn

[T36] Lua：函数
来源：http://euf.nwbrower.top

function add(a, b) return a + b end
来源：http://jhm.yonumen.top

[T37] Lua：字符串拼接
来源：http://vnc.316326.xyz

"a" .. "b"
来源：http://hxs.vqdsnc.cn

[T38] Lua：条件
来源：http://zup.hnxiangtu.top

if x > 0 then print("正") end
来源：http://rmy.dianchejie.cn

[T39] Lua：模式匹配
来源：http://rnp.zhijiandao.cn

string.find(s, "%d+")
来源：http://wau.zdbjq.cn

[T40] Lua：元表
来源：http://swr.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://lma.sxryk.cn

[T41] Perl：Hello World
来源：http://qxp.mhx1999.top

print "Hello\n";
来源：http://nto.yangfankeji.com

[T42] Perl：变量类型
来源：http://dsx.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zca.epnwcf.com

[T43] Perl：字符串插值
来源：http://ipu.nanxuanxn.top

"值: $a"
来源：http://olv.meibo888.top

[T44] Perl：条件
来源：http://dqh.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://pnw.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://wtc.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://fan.zdbjq.cn

[T46] Perl：哈希操作
来源：http://hbk.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hxy.52xcode.cn

[T47] Perl：正则捕获
来源：http://uyz.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gkc.yuanzhike.top

[T48] Perl：正则替换
来源：http://bat.dianchejie.cn

$s =~ s/old/new/g;
来源：http://ubu.chenjidiqi.icu

[T49] Perl：函数
来源：http://xmw.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zyp.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://xkg.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rml.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://tmc.zhixingplan.top

[T51] Scala：Hello World
来源：http://ega.zdbjq.cn

println("Hello")
来源：http://ncw.vehdjk.com

[T52] Scala：变量
来源：http://kfp.sysykeji.top

val a = 1;  var b = 2
来源：http://lce.jinqigufen.top

[T53] Scala：字符串插值
来源：http://jbl.haohaochexian.top

s"值: $b"
来源：http://oux.meibo888.top

[T54] Scala：集合映射
来源：http://lod.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://amh.hesvh.cn

[T55] Scala：集合过滤
来源：http://mbi.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://zhr.cheryme.top

[T56] Scala：样例类
来源：http://yek.vehdjk.com

case class User(name: String, age: Int)
来源：http://yue.zhengqikj.top

[T57] Scala：模式匹配
来源：http://ubg.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jty.zhongyouzk.top

[T58] Scala：函数定义
来源：http://txv.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://pvs.ehwqpu.com

[T59] Scala：循环
来源：http://bbl.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://aja.jianghu66.top

[T60] Scala：折叠
来源：http://xvv.guowangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aah.fzhhl.top

================================================================================
来源：http://wlj.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mpy.yanxiufei.cn

================================================================================
来源：http://jke.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://cqg.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://afe.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://osc.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ekc.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://ogn.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://bpn.epnwcf.com

[U04] Py：变量调试打印
来源：http://kbm.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zkk.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://awo.fehbvm.com

list(dict.fromkeys(arr))
来源：http://osw.0kj1m.cn

[U06] Py：合并两个字典
来源：http://rva.ehwqpu.com

{**a, **b}
来源：http://ruq.jqgufenzy.top

[U07] Py：反转字典键值
来源：http://dxw.yonumen.top

{v: k for k, v in d.items()}
来源：http://wux.snrcjt.cn

[U08] Py：展平二维列表
来源：http://uop.zycfv.cn

[y for x in nested for y in x]
来源：http://ltt.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://ubf.ivvv.top

max(d, key=d.get)
来源：http://rdg.gzhubu.top

[U10] Py：按值排序字典
来源：http://jck.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mej.yvedp.cn

[U11] Py：生成器表达式
来源：http://nvq.redwolf501.top

(x * 2 for x in arr)
来源：http://rhi.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://gqg.cdnleiting.top

Counter(arr).most_common(3)
来源：http://zog.svipenyu.cn

[U13] Py：固定长度队列
来源：http://cau.hnqzz.top

deque(maxlen=10)
来源：http://may.gzhubu.top

[U14] Py：分组收集到列表
来源：http://xxm.jyoumei.cn

defaultdict(list)
来源：http://mgk.ybcxt.top

[U15] Py：高精度计时
来源：http://nex.c1oappe.top

t = time.perf_counter()
来源：http://dnd.c1oappe.top

[U16] Py：命令行参数解析
来源：http://jtx.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://myf.316326.xyz

[U17] Py：初始化日志
来源：http://sna.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://unw.zhengqikj.top

[U18] Py：预编译正则
来源：http://luw.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://jce.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://nlt.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lfz.uphjek.com

[U20] Py：缓存函数结果
来源：http://dpz.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://dpo.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://hsx.zhongyouzk.top

@contextlib.contextmanager
来源：http://gos.52xcode.cn

[U22] Py：矩阵转置
来源：http://rjq.vehdjk.com

list(zip(*m))
来源：http://aog.ybcxt.top

[U23] Py：分块读取大文件
来源：http://kvt.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://edy.c1oappe.top

[U24] Py：路径操作
来源：http://nya.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ffu.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://lpk.xylfe.cn

csv.DictReader(f)
来源：http://dsh.yongpay.top

[U26] Py：并发下载
来源：http://gyc.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wrn.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://mxq.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://ozt.ctjpmb.com

[U28] Py：类型别名
来源：http://xwr.xuanzx.com

UserId = int
来源：http://tbp.yonumen.top

[U29] Py：属性校验
来源：http://pws.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://jbs.0kj1m.cn

[U30] Py：数据类
来源：http://sfx.jianghu66.top

@dataclass(slots=True)
来源：http://bdu.sjlbkw.cn

[U31] Py：单测
来源：http://ziy.fktsv.cn

python -m pytest -q
来源：http://frp.jinqigfzy.top

[U32] Py：代码格式化
来源：http://mlj.yongpay.top

ruff format . && ruff check --fix .
来源：http://qqm.vqdsnc.cn

[U33] Py：打包发布
来源：http://jvi.shuidangran.top

python -m build  （依赖 pyproject.toml）
来源：http://yfe.ehwqpu.com

[U34] Py：判断编码
来源：http://idf.jinqigfzy.top

chardet.detect(raw)
来源：http://scn.hnxiangtu.top

[U35] Py：发送邮件
来源：http://odt.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cuz.wangdashe.top

[U36] Py：定时任务
来源：http://bjk.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://pzs.aizwys.cn

[U37] Py：读写 Excel
来源：http://fjm.zdqjudy.top

pandas.read_excel / DataFrame.to_excel
来源：http://owr.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://wrb.tanke756.top

Path(__file__).resolve().parent
来源：http://jes.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://ppu.shuidangran.top

sys.stdout.isatty()
来源：http://mtq.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://kzq.uphjek.com

print("err", file=sys.stderr)
来源：http://rdz.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://niy.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sqv.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://dot.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zbv.hcnkem.com

[U43] PHP：声明命名空间
来源：http://ewi.guowangkeji.top

namespace App\Http;
来源：http://wtq.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://ztf.cashguo.top

declare(strict_types=1);
来源：http://xiw.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://nue.quarkkingdee.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hkc.zhijiandao.cn

[U46] PHP：可空类型
来源：http://jst.bjfxy.top

?string $name = null
来源：http://zwo.nanxinkj.top

[U47] PHP：联合类型
来源：http://omn.yanxiufei.cn

int|string $id
来源：http://dud.epnwcf.com

[U48] PHP：纯枚举
来源：http://yri.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dza.xuanzx.com

[U49] PHP：只读属性
来源：http://oez.c1oappe.top

public readonly string $name
来源：http://rrh.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://pzq.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://wxn.yfazqb.com

[U51] PHP：数组解构
来源：http://ecc.yanxiufei.cn

[$a, $b] = $arr;
来源：http://hdj.yj20258.top

[U52] PHP：箭头函数
来源：http://qaa.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://exd.birdmap.top

[U53] PHP：空合并运算符
来源：http://dsq.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://uuo.0kj1m.cn

[U54] PHP：空安全调用
来源：http://vcp.ydjk.org.cn

$obj?->method()
来源：http://cdv.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://lwd.jqgfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zko.zycfv.cn

[U56] PHP：命名参数
来源：http://bao.zhengqikj.top

f(a: 1, b: 2)
来源：http://dnz.shangyingyoupin.top

[U57] PHP：字符串插值
来源：http://zca.hnxiangtu.top

"值: {$a}"
来源：http://kzf.0kj1m.cn

[U58] PHP：数组三件套
来源：http://fdj.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ojz.nwbrower.top

[U59] PHP：自定义排序
来源：http://xdu.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gru.ctjpmb.com

[U60] PHP：JSON 编解码
来源：http://kgx.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hek.zycfv.cn

[U61] PHP：正则
来源：http://xyk.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://acl.yvedp.cn

[U62] PHP：日期对象
来源：http://hcb.ehwqpu.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sml.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://ets.xylfe.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://szy.jqgfzy.top

[U64] PHP：目录遍历
来源：http://tog.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://yes.0kj1m.cn

[U65] PHP：会话
来源：http://vfk.fengsongda.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kzn.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://zvz.tian-w.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rss.fzhhl.top

[U67] PHP：处理文件上传
来源：http://fpj.zhoulong.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://btj.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://hnf.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bol.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://tqd.uphjek.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rgu.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://ggf.shanyushiyangkeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uou.chenzaomai.com

[U71] PHP：抛出异常
来源：http://mlg.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://jqr.ybcxt.top

[U72] PHP：写错误日志
来源：http://gqt.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://apl.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://ibs.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://dkz.smart0.xyz

[U74] PHP：读取环境变量
来源：http://zny.daxiang520.top

getenv("APP_ENV") ?: "production"
来源：http://mny.tianlin.xyz

[U75] PHP：依赖注入
来源：http://dgg.shangyingyoupin.top

composer require psr/container
来源：http://hbg.ydjk.org.cn

[U76] PHP：简单路由
来源：http://iyw.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jbn.yj20258.top

[U77] PHP：模板渲染
来源：http://czx.fehbvm.com

composer require twig/twig
来源：http://vlj.dashuyun.cn

[U78] PHP：单元测试
来源：http://izy.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://qvx.yuanzhike.top

[U79] PHP：静态分析
来源：http://bpq.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://afs.cucudq.cn

[U80] PHP：代码规范修复
来源：http://snk.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://awa.hywenlv.cn

[U81] JS：初始化项目
来源：http://tqy.mhx1999.top

npm init -y;  npm i express
来源：http://jea.jiagoushi.top

[U82] JS：package.json 脚本
来源：http://qtf.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ktn.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://kwv.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://ngv.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://ajg.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hsv.hfpthk.cn

[U85] JS：可选链
来源：http://bvx.sweek.top

a?.b?.c
来源：http://fnb.sxryk.cn

[U86] JS：空值合并
来源：http://pfo.pycfn.com

a ?? b
来源：http://hys.jinghuilouyu.cn


<!-- 参考信息 -->