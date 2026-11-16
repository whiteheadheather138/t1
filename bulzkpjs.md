代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bbh.sweek.top

================================================================================
来源：http://vrx.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ama.hysaishi.cn

================================================================================
来源：http://mhf.mhx1999.top

[T01] Kotlin：Hello World
来源：http://tig.fktsv.cn

println("Hello")
来源：http://imc.pycfn.com

[T02] Kotlin：变量
来源：http://jbl.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gws.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://fmg.shangyingyoupin.top

"值: $b"
来源：http://jhc.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://zvi.iojbl.cn

val n: String? = null;  n?.length
来源：http://mvl.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://lec.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hgi.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://lgu.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ial.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://gus.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ews.jqgfzy.top

[T08] Kotlin：数据类
来源：http://nkv.sweek.top

data class User(val name: String, val age: Int)
来源：http://ouv.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://ntv.sweek.top

fun String.exclaim() = this + "!"
来源：http://zfa.iojbl.cn

[T10] Kotlin：默认参数
来源：http://mni.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ydt.hammf.cn

[T11] Kotlin：协程
来源：http://zuy.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://shi.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://kwk.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://zhd.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://fvl.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://zzi.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://rwm.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://jsb.sysykeji.top

[T15] Kotlin：接口
来源：http://icl.zycfv.cn

interface Shape { fun area(): Double }
来源：http://vif.bbcook.cn

[T16] Swift：Hello World
来源：http://jfw.feifeiyinyue.top

print("Hello")
来源：http://igs.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://qmj.jlsjyb.cn

var a = 1;  let b = 2
来源：http://lgy.bjfxy.top

[T18] Swift：字符串插值
来源：http://nfz.shanyushiyangtech.top

"值: \(b)"
来源：http://ahv.dianchejie.cn

[T19] Swift：可选绑定
来源：http://blj.ydjk.org.cn

if let n = opt { print(n) }
来源：http://nqn.yonumen.top

[T20] Swift：数组操作
来源：http://swx.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wrr.xuanzx.com

[T21] Swift：遍历
来源：http://pep.epnwcf.com

for x in a { print(x) }
来源：http://xfz.shzxlz.cn

[T22] Swift：字典
来源：http://gcu.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fsw.hywenlv.cn

[T23] Swift：函数
来源：http://zoy.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dav.yonumen.top

[T24] Swift：闭包
来源：http://ozl.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ozw.dianchejie.cn

[T25] Swift：结构体
来源：http://uzr.ydzc1.top

struct P { var x: Int }
来源：http://imo.yonumen.top

[T26] Swift：类与重写
来源：http://ija.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://fzg.yj20258.top

[T27] Swift：错误处理
来源：http://euw.yongpay.top

do { try f() } catch { print(error) }
来源：http://yfv.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://fny.sweek.top

enum Color { case red, green }
来源：http://hzm.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://nzx.gaohongyu789.top

guard let x = opt else { return }
来源：http://epv.aizwys.cn

[T30] Swift：协议
来源：http://oee.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://bde.chenzaomai.com

[T31] Lua：Hello World
来源：http://vfn.uphjek.com

print("Hello")
来源：http://tic.pycfn.com

[T32] Lua：局部变量
来源：http://itx.hysaishi.cn

local a = 1
来源：http://wns.fengsongda.top

[T33] Lua：表（数组）
来源：http://fdr.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gdy.uphjek.com

[T34] Lua：遍历表
来源：http://cjd.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://meg.zdbjq.cn

[T35] Lua：字典表
来源：http://xqf.zhijiandao.cn

local d = { a = 1 };  d.b = 2
来源：http://aas.hammf.cn

[T36] Lua：函数
来源：http://log.52xcode.cn

function add(a, b) return a + b end
来源：http://dek.xinyue.icu

[T37] Lua：字符串拼接
来源：http://lmt.iojbl.cn

"a" .. "b"
来源：http://eot.zhengqikj.top

[T38] Lua：条件
来源：http://tbt.yj202588.top

if x > 0 then print("正") end
来源：http://pbw.epnwcf.com

[T39] Lua：模式匹配
来源：http://zuc.yuanzhike.top

string.find(s, "%d+")
来源：http://vqq.ivvv.top

[T40] Lua：元表
来源：http://zpd.epnwcf.com

setmetatable({}, { __index = base })
来源：http://czy.uphjek.com

[T41] Perl：Hello World
来源：http://xzv.zhongyouzk.top

print "Hello\n";
来源：http://idq.tian-w.cn

[T42] Perl：变量类型
来源：http://nci.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lhg.yfazqb.com

[T43] Perl：字符串插值
来源：http://ajg.haohaochexian.top

"值: $a"
来源：http://wej.shanyushiyangtech.top

[T44] Perl：条件
来源：http://rof.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://ozp.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://qpk.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://pel.redwolf501.top

[T46] Perl：哈希操作
来源：http://cav.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eru.yuxming.cn

[T47] Perl：正则捕获
来源：http://zrp.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tuo.fehbvm.com

[T48] Perl：正则替换
来源：http://dbx.aizwys.cn

$s =~ s/old/new/g;
来源：http://mwv.shanyushiyangtech.top

[T49] Perl：函数
来源：http://jew.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mdh.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://rzq.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://czl.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://nox.yfazqb.com

[T51] Scala：Hello World
来源：http://ick.iojbl.cn

println("Hello")
来源：http://hst.dashuyun.cn

[T52] Scala：变量
来源：http://xwh.fengsongda.top

val a = 1;  var b = 2
来源：http://sas.pycfn.com

[T53] Scala：字符串插值
来源：http://wod.smart0.xyz

s"值: $b"
来源：http://vsy.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://ost.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://uuj.xylfe.cn

[T55] Scala：集合过滤
来源：http://hbh.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://crs.sweek.top

[T56] Scala：样例类
来源：http://gfh.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://wub.ehwqpu.com

[T57] Scala：模式匹配
来源：http://uhw.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://euw.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://swc.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://upo.fktsv.cn

[T59] Scala：循环
来源：http://xxf.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://xpd.zdbjq.cn

[T60] Scala：折叠
来源：http://bcz.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aak.c1oappe.top

================================================================================
来源：http://vbq.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://chl.gzhubu.top

================================================================================
来源：http://bqy.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://vfp.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ymy.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://svm.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xdp.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://ker.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://igz.havefunace.top

[U04] Py：变量调试打印
来源：http://tro.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bww.birdmap.top

[U05] Py：列表去重且保序
来源：http://fbf.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://iwt.gzhubu.top

[U06] Py：合并两个字典
来源：http://gny.smart0.xyz

{**a, **b}
来源：http://uej.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://sts.meibo888.top

{v: k for k, v in d.items()}
来源：http://fer.jyoumei.cn

[U08] Py：展平二维列表
来源：http://nfh.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://ysz.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://owp.guowangkeji.top

max(d, key=d.get)
来源：http://cwa.cashguo.top

[U10] Py：按值排序字典
来源：http://pfn.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pfv.chenlongwang.top

[U11] Py：生成器表达式
来源：http://afr.zdqjudy.top

(x * 2 for x in arr)
来源：http://lup.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://keh.jlsjyb.cn

Counter(arr).most_common(3)
来源：http://gzt.jianghu66.top

[U13] Py：固定长度队列
来源：http://bjg.fengsongda.top

deque(maxlen=10)
来源：http://gpy.tanke756.top

[U14] Py：分组收集到列表
来源：http://abj.jinqigfzy.top

defaultdict(list)
来源：http://vtn.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://qbu.shuidangran.top

t = time.perf_counter()
来源：http://bkj.ybcxt.top

[U16] Py：命令行参数解析
来源：http://deb.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ayh.hammf.cn

[U17] Py：初始化日志
来源：http://bjw.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://lll.zycfv.cn

[U18] Py：预编译正则
来源：http://pzt.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://axv.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://swf.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lxi.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://sax.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://pqu.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://rft.uphjek.com

@contextlib.contextmanager
来源：http://lgx.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://gcz.ydzc1.top

list(zip(*m))
来源：http://rfw.zycfv.cn

[U23] Py：分块读取大文件
来源：http://swt.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://psa.ydzc1.top

[U24] Py：路径操作
来源：http://rba.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tvi.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://hpr.birdmap.top

csv.DictReader(f)
来源：http://opr.uphjek.com

[U26] Py：并发下载
来源：http://mrx.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xdy.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://ivz.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://xuo.zhoulong.xyz

[U28] Py：类型别名
来源：http://vlg.daria6918.cn

UserId = int
来源：http://gmt.jianghu66.top

[U29] Py：属性校验
来源：http://bzv.andypj.xyz

@property 与 @x.setter 配合
来源：http://rzy.ppjwa.cn

[U30] Py：数据类
来源：http://jtl.gogol.net.cn

@dataclass(slots=True)
来源：http://ckc.feifeiyinyue.top

[U31] Py：单测
来源：http://npy.yuanzhike.top

python -m pytest -q
来源：http://xaz.fehbvm.com

[U32] Py：代码格式化
来源：http://ezg.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://fia.jlsjyb.cn

[U33] Py：打包发布
来源：http://gef.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://bjd.yuxming.cn

[U34] Py：判断编码
来源：http://dhi.chenlongwang.top

chardet.detect(raw)
来源：http://mvy.smart0.xyz

[U35] Py：发送邮件
来源：http://adg.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uig.snrcjt.cn

[U36] Py：定时任务
来源：http://vmp.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://nne.aizwys.cn

[U37] Py：读写 Excel
来源：http://cfm.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://gck.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://ina.jyoumei.cn

Path(__file__).resolve().parent
来源：http://mnc.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://arp.bbcook.cn

sys.stdout.isatty()
来源：http://edm.ydzc1.top

[U40] Py：打印到标准错误
来源：http://stm.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://nqr.snrcjt.cn

[U41] PHP：初始化 Composer 项目
来源：http://khs.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://ize.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://rfi.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wmr.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://zka.jlsjyb.cn

namespace App\Http;
来源：http://vmj.ydzc1.top

[U44] PHP：开启严格类型
来源：http://mtc.feifeiyinyue.top

declare(strict_types=1);
来源：http://vco.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://tiy.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yjq.zhongyouzk.top

[U46] PHP：可空类型
来源：http://ije.zhoulong.xyz

?string $name = null
来源：http://qnt.zhixingplan.top

[U47] PHP：联合类型
来源：http://aur.vehdjk.com

int|string $id
来源：http://mvn.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://tuv.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aur.hesvh.cn

[U49] PHP：只读属性
来源：http://sai.shangyingyoupin.top

public readonly string $name
来源：http://azv.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://ydu.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://tfa.hysaishi.cn

[U51] PHP：数组解构
来源：http://ktq.ctjpmb.com

[$a, $b] = $arr;
来源：http://iqq.sweek.top

[U52] PHP：箭头函数
来源：http://qhb.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://ztl.yonumen.top

[U53] PHP：空合并运算符
来源：http://kaj.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://anr.ydzc1.top

[U54] PHP：空安全调用
来源：http://tbp.zhengqikj.top

$obj?->method()
来源：http://ezc.hnqzz.top

[U55] PHP：match 表达式
来源：http://rif.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hgy.aizwys.cn

[U56] PHP：命名参数
来源：http://keh.sufxvd.cn

f(a: 1, b: 2)
来源：http://zty.yj20258.top

[U57] PHP：字符串插值
来源：http://wdc.svipenyu.cn

"值: {$a}"
来源：http://whm.yvedp.cn

[U58] PHP：数组三件套
来源：http://eru.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xum.yonumen.top

[U59] PHP：自定义排序
来源：http://mwa.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rje.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://sko.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fmz.yj20258.top

[U61] PHP：正则
来源：http://idu.sxryk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jyj.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://krs.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ipr.zdbjq.cn

[U63] PHP：文件读写
来源：http://dth.hywenlv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://les.aizwys.cn

[U64] PHP：目录遍历
来源：http://gkb.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://vcd.jlsjyb.cn

[U65] PHP：会话
来源：http://fgu.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://xoy.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://ddf.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qfa.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://iaf.yfazqb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dct.ehwqpu.com

[U68] PHP：PDO 连接
来源：http://jpv.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jjv.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://olb.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wxz.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://crc.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.yj20258888.top

[U71] PHP：抛出异常
来源：http://jbg.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://kfc.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://cia.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://vho.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://hsz.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://tpz.daria6918.cn

[U74] PHP：读取环境变量
来源：http://izj.hcnkem.com

getenv("APP_ENV") ?: "production"
来源：http://utd.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://vgr.zhaomingkeji.xyz

composer require psr/container
来源：http://nee.ydzc1.top

[U76] PHP：简单路由
来源：http://ryx.aizwys.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://brw.sxryk.cn

[U77] PHP：模板渲染
来源：http://jsw.cheryme.top

composer require twig/twig
来源：http://olb.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://tkm.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://mdl.jqgufenzy.top

[U79] PHP：静态分析
来源：http://idu.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://yyr.9152youxi.cn

[U80] PHP：代码规范修复
来源：http://xeq.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xsv.c1oappe.top

[U81] JS：初始化项目
来源：http://qzl.cdnleiting.top

npm init -y;  npm i express
来源：http://ldn.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://lrx.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ubg.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://uqx.shanyushiyangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://lnb.meibo888.top

[U84] JS：CommonJS 写法
来源：http://tez.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fqw.kuanghao11.cn

[U85] JS：可选链
来源：http://yvd.quarkkingdee.top

a?.b?.c
来源：http://jlk.hysaishi.cn

[U86] JS：空值合并
来源：http://yxp.dianchejie.cn

a ?? b
来源：http://sou.guowangkeji.top


<!-- 参考信息 -->