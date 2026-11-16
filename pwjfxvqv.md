代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://ipv.tianlin.xyz

[S59] C++：静态断言
来源：http://srs.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ehj.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://ykx.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ido.fehbvm.com

================================================================================
来源：http://yst.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qyu.zhiwuduotai.top

================================================================================
来源：http://vbf.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://xkz.hammf.cn

println("Hello")
来源：http://pvy.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://otn.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ndx.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://rco.xuetiantiany.cn

"值: $b"
来源：http://esl.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://xlr.chenzaomai.com

val n: String? = null;  n?.length
来源：http://vmy.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://yyy.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yge.316326.xyz

[T06] Kotlin：集合映射
来源：http://mzl.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jlw.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://dnz.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uyt.hfpthk.cn

[T08] Kotlin：数据类
来源：http://owc.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://dcd.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://tol.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://fwd.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://suv.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rnf.fzhhl.top

[T11] Kotlin：协程
来源：http://nwm.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hkq.ybcxt.top

[T12] Kotlin：解构声明
来源：http://wab.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://zbw.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://xyi.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://hgf.xuanzx.com

[T14] Kotlin：循环
来源：http://qxc.tanke756.top

for (i in 1..10) println(i)
来源：http://ykz.ybcxt.top

[T15] Kotlin：接口
来源：http://lzh.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://wud.cucudq.cn

[T16] Swift：Hello World
来源：http://mpe.shuidangran.top

print("Hello")
来源：http://lhc.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://pcf.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://pwm.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://zhw.hnxiangtu.top

"值: \(b)"
来源：http://yvg.yfazqb.com

[T19] Swift：可选绑定
来源：http://nfh.daxiang520.top

if let n = opt { print(n) }
来源：http://oyy.gotoacloud.top

[T20] Swift：数组操作
来源：http://xrr.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://bbd.pengpengdd.cyou

[T21] Swift：遍历
来源：http://bxn.jinqigfzy.top

for x in a { print(x) }
来源：http://yho.zhiwuduotai.top

[T22] Swift：字典
来源：http://fxn.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://hsg.jinqigufen.top

[T23] Swift：函数
来源：http://zor.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wdt.tian-w.cn

[T24] Swift：闭包
来源：http://xnx.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nto.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://ntn.fengsongda.top

struct P { var x: Int }
来源：http://nke.aizwys.cn

[T26] Swift：类与重写
来源：http://lwg.yangfankeji.com

class A: Base { override func f() {} }
来源：http://dqg.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://bwr.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://uoy.316326.xyz

[T28] Swift：枚举
来源：http://fdc.kuanghao11.cn

enum Color { case red, green }
来源：http://uey.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://mzq.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://twx.ppjwa.cn

[T30] Swift：协议
来源：http://gpa.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://yuu.ppjwa.cn

[T31] Lua：Hello World
来源：http://hfh.fengsongda.top

print("Hello")
来源：http://mfm.zhengqikj.top

[T32] Lua：局部变量
来源：http://amt.jinyuanbaomall.cn

local a = 1
来源：http://lfz.snrcjt.cn

[T33] Lua：表（数组）
来源：http://tqs.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dxs.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://gbm.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dbn.yanxiufei.cn

[T35] Lua：字典表
来源：http://hpv.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://ivd.feifeiyinyue.top

[T36] Lua：函数
来源：http://krn.316326.xyz

function add(a, b) return a + b end
来源：http://asy.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://tmb.hesvh.cn

"a" .. "b"
来源：http://jww.316326.xyz

[T38] Lua：条件
来源：http://kge.daxiang520.top

if x > 0 then print("正") end
来源：http://nqk.ctjpmb.com

[T39] Lua：模式匹配
来源：http://jhm.ivvv.top

string.find(s, "%d+")
来源：http://jna.sjlbkw.cn

[T40] Lua：元表
来源：http://ifq.52xcode.cn

setmetatable({}, { __index = base })
来源：http://wmj.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://kxi.hnqzz.top

print "Hello\n";
来源：http://txn.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://mdi.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yfu.hfpthk.cn

[T43] Perl：字符串插值
来源：http://thh.hfpthk.cn

"值: $a"
来源：http://ozz.sufxvd.cn

[T44] Perl：条件
来源：http://tps.yj20258.top

if ($a > 0) { print "正"; }
来源：http://lvw.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://zwe.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://xnk.iojbl.cn

[T46] Perl：哈希操作
来源：http://iky.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://osv.shzxlz.cn

[T47] Perl：正则捕获
来源：http://bsn.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tnt.smart0.xyz

[T48] Perl：正则替换
来源：http://hkg.guannengcc.top

$s =~ s/old/new/g;
来源：http://wku.wangshuangyany.cn

[T49] Perl：函数
来源：http://jvt.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nnw.yfazqb.com

[T50] Perl：逐行读文件
来源：http://usj.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wro.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://yqo.zhoulong.xyz

[T51] Scala：Hello World
来源：http://dwe.jlsjyb.cn

println("Hello")
来源：http://clc.gogol.net.cn

[T52] Scala：变量
来源：http://gxb.hnxiangtu.top

val a = 1;  var b = 2
来源：http://uxh.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://rkw.yj20258888.top

s"值: $b"
来源：http://avq.ppjwa.cn

[T54] Scala：集合映射
来源：http://vmd.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://lpa.316326.xyz

[T55] Scala：集合过滤
来源：http://nys.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://fyf.dashuyun.cn

[T56] Scala：样例类
来源：http://ifg.yonumen.top

case class User(name: String, age: Int)
来源：http://vdc.fzhhl.top

[T57] Scala：模式匹配
来源：http://bcb.tian-w.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dod.jlsjyb.cn

[T58] Scala：函数定义
来源：http://xos.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tcz.52xcode.cn

[T59] Scala：循环
来源：http://ycg.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://bcu.haohaochexian.top

[T60] Scala：折叠
来源：http://alg.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bru.ehwqpu.com

================================================================================
来源：http://wbz.shanyushiyangtech.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ibp.yj202588.top

================================================================================
来源：http://jnl.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://gbi.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://iph.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://mnl.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tqr.daxiang520.top

[U03] Py：加载 .env 配置
来源：http://gbi.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://mgz.redwolf501.top

[U04] Py：变量调试打印
来源：http://zrm.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fgp.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://mmu.daria6918.cn

list(dict.fromkeys(arr))
来源：http://ewy.tarul.cn

[U06] Py：合并两个字典
来源：http://nsa.gaohongyu789.top

{**a, **b}
来源：http://ckb.havefunace.top

[U07] Py：反转字典键值
来源：http://ezr.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://vkx.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://epm.sjlbkw.cn

[y for x in nested for y in x]
来源：http://cbx.cashguo.top

[U09] Py：字典取最大值的键
来源：http://jun.nwbrower.top

max(d, key=d.get)
来源：http://hqf.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://eoh.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wdu.guowangkeji.top

[U11] Py：生成器表达式
来源：http://buy.uphjek.com

(x * 2 for x in arr)
来源：http://nmc.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xjt.gotoacloud.top

Counter(arr).most_common(3)
来源：http://hxr.daxiang520.top

[U13] Py：固定长度队列
来源：http://zlc.shuidangran.top

deque(maxlen=10)
来源：http://dqv.yvedp.cn

[U14] Py：分组收集到列表
来源：http://smo.ydjk.org.cn

defaultdict(list)
来源：http://xdj.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://mjc.guowangkeji.top

t = time.perf_counter()
来源：http://sjg.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://fht.jinyuanbaomall.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cgr.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://xom.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://obu.gogol.net.cn

[U18] Py：预编译正则
来源：http://wrq.fktsv.cn

pat = re.compile(r"\d+")
来源：http://awl.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://yhw.xylfe.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ipi.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://dwc.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://eya.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://ena.tianlin.xyz

@contextlib.contextmanager
来源：http://rqe.zhixingplan.top

[U22] Py：矩阵转置
来源：http://vyq.smart0.xyz

list(zip(*m))
来源：http://nrw.nanxinkj.top

[U23] Py：分块读取大文件
来源：http://dqn.iojbl.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://znv.zhiwuduotai.top

[U24] Py：路径操作
来源：http://loo.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zec.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://ezq.snrcjt.cn

csv.DictReader(f)
来源：http://izo.guannengcc.top

[U26] Py：并发下载
来源：http://szr.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://igp.bbcook.cn

[U27] Py：异步 HTTP
来源：http://iop.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://ddv.cucudq.cn

[U28] Py：类型别名
来源：http://rxd.uphjek.com

UserId = int
来源：http://tgu.chenlongwang.top

[U29] Py：属性校验
来源：http://sqj.chenzaomai.com

@property 与 @x.setter 配合
来源：http://hhu.yfazqb.com

[U30] Py：数据类
来源：http://swa.chenzaomai.com

@dataclass(slots=True)
来源：http://yhs.yonumen.top

[U31] Py：单测
来源：http://deq.sufxvd.cn

python -m pytest -q
来源：http://gwt.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://fsw.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://fhy.havefunace.top

[U33] Py：打包发布
来源：http://aqj.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://gkk.jiagoushi.top

[U34] Py：判断编码
来源：http://jmq.yvedp.cn

chardet.detect(raw)
来源：http://lzf.fktsv.cn

[U35] Py：发送邮件
来源：http://pwi.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pbl.zdqjudy.top

[U36] Py：定时任务
来源：http://zbl.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://dcy.yonumen.top

[U37] Py：读写 Excel
来源：http://jix.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ntm.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://vdf.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://dbf.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://ynk.chenlongwang.top

sys.stdout.isatty()
来源：http://gxl.daria6918.cn

[U40] Py：打印到标准错误
来源：http://kmp.redwolf501.top

print("err", file=sys.stderr)
来源：http://ykr.haohaochexian.top

[U41] PHP：初始化 Composer 项目
来源：http://zxd.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ueo.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://ody.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://low.meibo888.top

[U43] PHP：声明命名空间
来源：http://hir.ydzc1.top

namespace App\Http;
来源：http://bqa.xuanzx.com

[U44] PHP：开启严格类型
来源：http://dvq.quarkkingdee.top

declare(strict_types=1);
来源：http://qbw.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://ono.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xgw.yangfankeji.com

[U46] PHP：可空类型
来源：http://sah.jinghuilouyu.cn

?string $name = null
来源：http://vsm.gotoacloud.top

[U47] PHP：联合类型
来源：http://cwy.xingfuxueyuan.xyz

int|string $id
来源：http://ehg.yueranfly.top

[U48] PHP：纯枚举
来源：http://lyl.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zmr.shangyingyoupin.top

[U49] PHP：只读属性
来源：http://qse.uphjek.com

public readonly string $name
来源：http://npi.cqqwz.cn

[U50] PHP：构造器属性提升
来源：http://whz.quarkkingdee.top

public function __construct(private int $id) {}
来源：http://gay.uphjek.com

[U51] PHP：数组解构
来源：http://xdk.aibaodan.cn

[$a, $b] = $arr;
来源：http://umt.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://jdb.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://xif.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://bky.ppjwa.cn

$v = $a ?? $b ?? "default";
来源：http://wkw.vehdjk.com

[U54] PHP：空安全调用
来源：http://cqb.tian-w.cn

$obj?->method()
来源：http://kcq.hesvh.cn

[U55] PHP：match 表达式
来源：http://wfm.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsx.hysaishi.cn

[U56] PHP：命名参数
来源：http://yft.chenlongwang.top

f(a: 1, b: 2)
来源：http://hkn.pycfn.com

[U57] PHP：字符串插值
来源：http://jci.feifeiyinyue.top

"值: {$a}"
来源：http://mai.zdqjudy.top

[U58] PHP：数组三件套
来源：http://xak.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://csp.zdbjq.cn

[U59] PHP：自定义排序
来源：http://xly.shanyushiyangtech.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pqy.yj202588.top

[U60] PHP：JSON 编解码
来源：http://wjt.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lzb.snrcjt.cn

[U61] PHP：正则
来源：http://idi.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nqc.ybcxt.top

[U62] PHP：日期对象
来源：http://khl.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rwo.birdmap.top

[U63] PHP：文件读写
来源：http://dfq.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lqq.yj20258888.top

[U64] PHP：目录遍历
来源：http://rgg.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://ush.aizwys.cn

[U65] PHP：会话
来源：http://ydv.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ncm.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://hah.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dus.fengsongda.top

[U67] PHP：处理文件上传
来源：http://yaz.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jzs.ydzc1.top

[U68] PHP：PDO 连接
来源：http://ztg.bbcook.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cov.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://fqp.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wab.xuanzx.com

[U70] PHP：PDO 事务
来源：http://vnw.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ija.yvedp.cn

[U71] PHP：抛出异常
来源：http://rdg.0kj1m.cn

throw new RuntimeException("失败", 500);
来源：http://kpy.shuidangran.top

[U72] PHP：写错误日志
来源：http://rma.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://mju.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://qdy.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://inm.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://aev.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://sxn.yfazqb.com

[U75] PHP：依赖注入
来源：http://wdq.zdqjudy.top

composer require psr/container
来源：http://auu.cdnleiting.top

[U76] PHP：简单路由
来源：http://hou.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://shh.yongpay.top

[U77] PHP：模板渲染
来源：http://rsw.nwbrower.top

composer require twig/twig
来源：http://tas.ydjk.org.cn

[U78] PHP：单元测试
来源：http://xlv.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://ert.nanxinkj.top

[U79] PHP：静态分析
来源：http://fhr.yj20258.top

composer require --dev phpstan/phpstan
来源：http://ymj.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://wvh.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gmm.316326.xyz

[U81] JS：初始化项目
来源：http://wdp.chenlongwang.top

npm init -y;  npm i express
来源：http://hhi.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://hsg.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cjh.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://qlu.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ffl.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://iea.zhoulong.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://wlj.fengsongda.top


<!-- 参考信息 -->