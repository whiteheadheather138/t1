代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://fgg.hcnkem.com

[S59] C++：静态断言
来源：http://rup.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://azx.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://kbe.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zho.guowangkeji.top

================================================================================
来源：http://twv.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://myt.andypj.xyz

================================================================================
来源：http://fow.iojbl.cn

[T01] Kotlin：Hello World
来源：http://rfr.ydjk.org.cn

println("Hello")
来源：http://gbb.ydjk.org.cn

[T02] Kotlin：变量
来源：http://mxv.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cku.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://pin.zhixingplan.top

"值: $b"
来源：http://yiz.ydzc1.top

[T04] Kotlin：空安全
来源：http://eth.aibaodan.cn

val n: String? = null;  n?.length
来源：http://jgg.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://ygy.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bqp.epnwcf.com

[T06] Kotlin：集合映射
来源：http://xmw.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://hva.sweek.top

[T07] Kotlin：集合过滤
来源：http://jsd.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uys.ydzc1.top

[T08] Kotlin：数据类
来源：http://upt.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://rhe.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://ebi.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://npd.hnqzz.top

[T10] Kotlin：默认参数
来源：http://old.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hqu.jlsjyb.cn

[T11] Kotlin：协程
来源：http://krw.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pwv.daxiang520.top

[T12] Kotlin：解构声明
来源：http://pxy.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://iho.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://jns.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://pyl.hesvh.cn

[T14] Kotlin：循环
来源：http://dgv.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://ios.nanxuanxn.top

[T15] Kotlin：接口
来源：http://ncr.ybcxt.top

interface Shape { fun area(): Double }
来源：http://xda.ybcxt.top

[T16] Swift：Hello World
来源：http://ijc.yj20258.top

print("Hello")
来源：http://mus.ctjpmb.com

[T17] Swift：变量与常量
来源：http://jkb.ppjwa.cn

var a = 1;  let b = 2
来源：http://efr.shuidangran.top

[T18] Swift：字符串插值
来源：http://aka.yj20258.top

"值: \(b)"
来源：http://bhr.316326.xyz

[T19] Swift：可选绑定
来源：http://cfe.hywenlv.cn

if let n = opt { print(n) }
来源：http://fdu.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://ucl.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wzz.xylfe.cn

[T21] Swift：遍历
来源：http://aje.xinyue.icu

for x in a { print(x) }
来源：http://xuw.nanxuanxn.top

[T22] Swift：字典
来源：http://wkf.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://slg.chenlongwang.top

[T23] Swift：函数
来源：http://reu.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wzo.hfpthk.cn

[T24] Swift：闭包
来源：http://ynj.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://que.hammf.cn

[T25] Swift：结构体
来源：http://smw.zycfv.cn

struct P { var x: Int }
来源：http://tur.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://ypz.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://cih.quarkkingdee.top

[T27] Swift：错误处理
来源：http://ucl.daria6918.cn

do { try f() } catch { print(error) }
来源：http://iyz.yonumen.top

[T28] Swift：枚举
来源：http://bsp.xylfe.cn

enum Color { case red, green }
来源：http://aqf.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://clq.ctjpmb.com

guard let x = opt else { return }
来源：http://dpv.vehdjk.com

[T30] Swift：协议
来源：http://swm.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://rot.gaohongyu789.top

[T31] Lua：Hello World
来源：http://wsp.gogol.net.cn

print("Hello")
来源：http://yir.cqqwz.cn

[T32] Lua：局部变量
来源：http://rht.guowangkeji.top

local a = 1
来源：http://fvm.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://pnb.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tmr.ybcxt.top

[T34] Lua：遍历表
来源：http://joc.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ind.cdnleiting.top

[T35] Lua：字典表
来源：http://qwe.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://ewi.kuanghao11.cn

[T36] Lua：函数
来源：http://lww.gaohongyu789.top

function add(a, b) return a + b end
来源：http://efs.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://mxg.zycfv.cn

"a" .. "b"
来源：http://emb.tian-w.cn

[T38] Lua：条件
来源：http://erk.xziqi.cn

if x > 0 then print("正") end
来源：http://xtm.andypj.xyz

[T39] Lua：模式匹配
来源：http://lei.yanxiufei.cn

string.find(s, "%d+")
来源：http://mpt.vqdsnc.cn

[T40] Lua：元表
来源：http://nwy.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://xbo.zdqjudy.top

[T41] Perl：Hello World
来源：http://nno.zycfv.cn

print "Hello\n";
来源：http://hgs.vehdjk.com

[T42] Perl：变量类型
来源：http://yed.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rni.cdnleiting.top

[T43] Perl：字符串插值
来源：http://zub.mhx1999.top

"值: $a"
来源：http://cal.xingfuxueyuan.xyz

[T44] Perl：条件
来源：http://mfx.hammf.cn

if ($a > 0) { print "正"; }
来源：http://bhy.hnqzz.top

[T45] Perl：数组遍历
来源：http://tpr.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://bfp.316326.xyz

[T46] Perl：哈希操作
来源：http://biv.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xvw.yuxming.cn

[T47] Perl：正则捕获
来源：http://uaa.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://fud.zhengqikj.top

[T48] Perl：正则替换
来源：http://pot.wangdashe.top

$s =~ s/old/new/g;
来源：http://ryv.xinyue.icu

[T49] Perl：函数
来源：http://uxa.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qnx.yj20258888.top

[T50] Perl：逐行读文件
来源：http://ztt.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pnh.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://ybs.gaohongyu789.top

[T51] Scala：Hello World
来源：http://nwm.yanxiufei.cn

println("Hello")
来源：http://num.ehwqpu.com

[T52] Scala：变量
来源：http://mry.daxiang520.top

val a = 1;  var b = 2
来源：http://ltt.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://iea.ywan-chungtsiang.top

s"值: $b"
来源：http://yyq.yongpay.top

[T54] Scala：集合映射
来源：http://ogt.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://aac.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://hgo.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://org.dianchejie.cn

[T56] Scala：样例类
来源：http://ujg.zhengqikj.top

case class User(name: String, age: Int)
来源：http://jyg.hysaishi.cn

[T57] Scala：模式匹配
来源：http://nto.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tmw.svipenyu.cn

[T58] Scala：函数定义
来源：http://byi.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://uqz.cqqwz.cn

[T59] Scala：循环
来源：http://mio.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://hib.yfazqb.com

[T60] Scala：折叠
来源：http://fce.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eyh.gogol.net.cn

================================================================================
来源：http://dod.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qxa.yangfankeji.com

================================================================================
来源：http://wdm.tanke756.top

[U01] Py：创建虚拟环境
来源：http://qvt.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://tiu.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://sji.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zvm.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://vdx.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oju.shzxlz.cn

[U04] Py：变量调试打印
来源：http://giw.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wtz.aizwys.cn

[U05] Py：列表去重且保序
来源：http://oya.nanxinkj.top

list(dict.fromkeys(arr))
来源：http://jfe.tarul.cn

[U06] Py：合并两个字典
来源：http://yyn.zycfv.cn

{**a, **b}
来源：http://srx.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://sln.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://ylv.nwbrower.top

[U08] Py：展平二维列表
来源：http://sot.bbcook.cn

[y for x in nested for y in x]
来源：http://rlf.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://rja.smart0.xyz

max(d, key=d.get)
来源：http://lze.vehdjk.com

[U10] Py：按值排序字典
来源：http://cfv.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://arg.tian-w.cn

[U11] Py：生成器表达式
来源：http://utu.hnxiangtu.top

(x * 2 for x in arr)
来源：http://vsd.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://egx.xinyue.icu

Counter(arr).most_common(3)
来源：http://uos.nanxinkj.top

[U13] Py：固定长度队列
来源：http://aze.fanxiaobao.xyz

deque(maxlen=10)
来源：http://rud.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://aqv.wangshuangyany.cn

defaultdict(list)
来源：http://vbr.yonumen.top

[U15] Py：高精度计时
来源：http://djr.zycfv.cn

t = time.perf_counter()
来源：http://lkc.yongpay.top

[U16] Py：命令行参数解析
来源：http://fir.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ddr.yangfankeji.com

[U17] Py：初始化日志
来源：http://gbq.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://rgn.gogol.net.cn

[U18] Py：预编译正则
来源：http://oyb.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://bpn.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://pkm.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pvk.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://zdm.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://img.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://pay.fktsv.cn

@contextlib.contextmanager
来源：http://ert.hcnkem.com

[U22] Py：矩阵转置
来源：http://hnn.yj20258.top

list(zip(*m))
来源：http://qjb.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://hpm.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://evo.vehdjk.com

[U24] Py：路径操作
来源：http://nmh.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qri.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://kuz.yongpay.top

csv.DictReader(f)
来源：http://beu.haohaochexian.top

[U26] Py：并发下载
来源：http://ibp.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yzy.hcnkem.com

[U27] Py：异步 HTTP
来源：http://rgk.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://evy.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://xes.cdnleiting.top

UserId = int
来源：http://dsi.jinqigufen.top

[U29] Py：属性校验
来源：http://lrr.svipenyu.cn

@property 与 @x.setter 配合
来源：http://zqe.nwbrower.top

[U30] Py：数据类
来源：http://fys.cdnleiting.top

@dataclass(slots=True)
来源：http://xct.yanxiufei.cn

[U31] Py：单测
来源：http://cdl.0kj1m.cn

python -m pytest -q
来源：http://rde.dashuyun.cn

[U32] Py：代码格式化
来源：http://aun.smart0.xyz

ruff format . && ruff check --fix .
来源：http://mij.bbcook.cn

[U33] Py：打包发布
来源：http://msh.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://cim.xuanzx.com

[U34] Py：判断编码
来源：http://fvt.shanyushiyangtech.top

chardet.detect(raw)
来源：http://kdh.hcnkem.com

[U35] Py：发送邮件
来源：http://yyb.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://acz.yj20258.top

[U36] Py：定时任务
来源：http://zhw.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://aba.sweek.top

[U37] Py：读写 Excel
来源：http://iqi.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sih.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://bry.bbcook.cn

Path(__file__).resolve().parent
来源：http://wzt.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://srf.kuanghao11.cn

sys.stdout.isatty()
来源：http://vql.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://cmj.zdqjudy.top

print("err", file=sys.stderr)
来源：http://gsk.yueranfly.top

[U41] PHP：初始化 Composer 项目
来源：http://uxu.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://tpk.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://jkj.nwbrower.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lws.xylfe.cn

[U43] PHP：声明命名空间
来源：http://vvl.ywan-chungtsiang.top

namespace App\Http;
来源：http://rwx.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://qmk.iojbl.cn

declare(strict_types=1);
来源：http://hsm.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://gcs.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wqz.zhixingplan.top

[U46] PHP：可空类型
来源：http://ghg.uphjek.com

?string $name = null
来源：http://xkn.cqqwz.cn

[U47] PHP：联合类型
来源：http://xqc.birdmap.top

int|string $id
来源：http://rkp.dashuyun.cn

[U48] PHP：纯枚举
来源：http://msb.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tra.yanxiufei.cn

[U49] PHP：只读属性
来源：http://adw.jiagoushi.top

public readonly string $name
来源：http://dyq.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://dhd.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://qds.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://aed.jiagoushi.top

[$a, $b] = $arr;
来源：http://qwc.redwolf501.top

[U52] PHP：箭头函数
来源：http://qok.sufxvd.cn

$double = fn($x) => $x * 2;
来源：http://vei.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://dmy.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://xwn.zhaomingkeji.xyz

[U54] PHP：空安全调用
来源：http://lhq.hnqzz.top

$obj?->method()
来源：http://vlm.zdqjudy.top

[U55] PHP：match 表达式
来源：http://jri.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gkq.zhoulong.xyz

[U56] PHP：命名参数
来源：http://fpr.quarkkingdee.top

f(a: 1, b: 2)
来源：http://qod.shuidangran.top

[U57] PHP：字符串插值
来源：http://zwc.dashuyun.cn

"值: {$a}"
来源：http://mxx.hfpthk.cn

[U58] PHP：数组三件套
来源：http://app.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iqb.yj202588.top

[U59] PHP：自定义排序
来源：http://ddq.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dra.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://mal.ywan-chungtsiang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://urb.vqdsnc.cn

[U61] PHP：正则
来源：http://wvj.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nyp.gaohongyu789.top

[U62] PHP：日期对象
来源：http://cip.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nlf.havefunace.top

[U63] PHP：文件读写
来源：http://wlu.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ady.fzhhl.top

[U64] PHP：目录遍历
来源：http://yja.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://rwo.fzhhl.top

[U65] PHP：会话
来源：http://zig.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://oxm.havefunace.top

[U66] PHP：设置 Cookie
来源：http://dyw.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://thp.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://rus.zhixingplan.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vac.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://qmr.shanyushiyangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sau.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://zxz.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tyu.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://uik.shanyushiyangtech.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zsh.yj20258888.top

[U71] PHP：抛出异常
来源：http://yci.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://fcv.svipenyu.cn

[U72] PHP：写错误日志
来源：http://hnd.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://qlt.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://axs.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://dqk.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://kum.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://dty.yuxming.cn

[U75] PHP：依赖注入
来源：http://jqo.yj202588.top

composer require psr/container
来源：http://tpv.zhixingplan.top

[U76] PHP：简单路由
来源：http://mze.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dpo.svipenyu.cn

[U77] PHP：模板渲染
来源：http://gbg.ppjwa.cn

composer require twig/twig
来源：http://tnd.yvedp.cn

[U78] PHP：单元测试
来源：http://omy.ybcxt.top

composer require --dev phpunit/phpunit
来源：http://kxh.ppjwa.cn

[U79] PHP：静态分析
来源：http://fvz.epnwcf.com

composer require --dev phpstan/phpstan
来源：http://zki.daxiang520.top

[U80] PHP：代码规范修复
来源：http://wcs.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hov.wangdashe.top

[U81] JS：初始化项目
来源：http://lcz.hammf.cn

npm init -y;  npm i express
来源：http://owc.xziqi.cn

[U82] JS：package.json 脚本
来源：http://rsu.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bwo.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://zad.svipenyu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rqi.hcnkem.com

[U84] JS：CommonJS 写法
来源：http://yzh.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sus.hnxiangtu.top


<!-- 参考信息 -->