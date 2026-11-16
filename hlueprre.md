代发 wailian999

[T03] Kotlin：字符串模板
来源：http://zkk.hesvh.cn

"值: $b"
来源：http://ncj.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://bza.cucudq.cn

val n: String? = null;  n?.length
来源：http://uki.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://lym.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://obn.birdmap.top

[T06] Kotlin：集合映射
来源：http://kfr.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hqk.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://win.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://vlh.guowangkeji.top

[T08] Kotlin：数据类
来源：http://cjx.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://iui.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://pif.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://zbo.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://ydv.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oof.yvedp.cn

[T11] Kotlin：协程
来源：http://nsm.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uui.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://vkh.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://ioz.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://wrt.xinyue.icu

val m = mapOf("a" to 1)
来源：http://txk.ydzc1.top

[T14] Kotlin：循环
来源：http://kyx.yfazqb.com

for (i in 1..10) println(i)
来源：http://fpo.yuanzhike.top

[T15] Kotlin：接口
来源：http://zkq.fehbvm.com

interface Shape { fun area(): Double }
来源：http://zzw.zhengqikj.top

[T16] Swift：Hello World
来源：http://zgo.zhongyouzk.top

print("Hello")
来源：http://rot.yangfankeji.com

[T17] Swift：变量与常量
来源：http://qaz.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://vpx.52xcode.cn

[T18] Swift：字符串插值
来源：http://uec.bbcook.cn

"值: \(b)"
来源：http://esd.jqgfzy.top

[T19] Swift：可选绑定
来源：http://ycn.yangfankeji.com

if let n = opt { print(n) }
来源：http://heh.birdmap.top

[T20] Swift：数组操作
来源：http://htd.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://ech.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://ujn.gogol.net.cn

for x in a { print(x) }
来源：http://zts.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://joq.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://qsy.zhixingplan.top

[T23] Swift：函数
来源：http://mjj.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tep.quarkkingdee.top

[T24] Swift：闭包
来源：http://hco.wangdashe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mpk.mhx1999.top

[T25] Swift：结构体
来源：http://dlo.52xcode.cn

struct P { var x: Int }
来源：http://ppk.jinqigufen.top

[T26] Swift：类与重写
来源：http://oaj.iojbl.cn

class A: Base { override func f() {} }
来源：http://nqh.vehdjk.com

[T27] Swift：错误处理
来源：http://lxc.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://bio.guannengcc.top

[T28] Swift：枚举
来源：http://clx.316326.xyz

enum Color { case red, green }
来源：http://pkf.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://tdp.quarkkingdee.top

guard let x = opt else { return }
来源：http://key.zhixingplan.top

[T30] Swift：协议
来源：http://qkb.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://mxy.guowangkeji.top

[T31] Lua：Hello World
来源：http://kzf.jianghu66.top

print("Hello")
来源：http://hzw.zhengqikj.top

[T32] Lua：局部变量
来源：http://mdh.epnwcf.com

local a = 1
来源：http://ywh.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://rck.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://hlz.zhijiandao.cn

[T34] Lua：遍历表
来源：http://tdg.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nim.yvedp.cn

[T35] Lua：字典表
来源：http://utw.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://fap.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://ian.hnxiangtu.top

function add(a, b) return a + b end
来源：http://oyd.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://zrk.zycfv.cn

"a" .. "b"
来源：http://xne.andypj.xyz

[T38] Lua：条件
来源：http://ixj.yj202588.top

if x > 0 then print("正") end
来源：http://qrz.cdnleiting.top

[T39] Lua：模式匹配
来源：http://rtc.cheryme.top

string.find(s, "%d+")
来源：http://qhi.9152youxi.cn

[T40] Lua：元表
来源：http://ahz.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://obq.jqgufenzy.top

[T41] Perl：Hello World
来源：http://rhh.zhixingplan.top

print "Hello\n";
来源：http://nba.havefunace.top

[T42] Perl：变量类型
来源：http://bhq.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yof.zycfv.cn

[T43] Perl：字符串插值
来源：http://zwl.yonumen.top

"值: $a"
来源：http://oan.sxryk.cn

[T44] Perl：条件
来源：http://bzi.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://qat.fktsv.cn

[T45] Perl：数组遍历
来源：http://hyp.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://dte.zhixingplan.top

[T46] Perl：哈希操作
来源：http://bft.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qfj.aizwys.cn

[T47] Perl：正则捕获
来源：http://ahg.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://snh.mhx1999.top

[T48] Perl：正则替换
来源：http://evp.pycfn.com

$s =~ s/old/new/g;
来源：http://roe.shzxlz.cn

[T49] Perl：函数
来源：http://hsx.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pvi.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://xgz.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yfx.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://vpn.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://rxj.yfazqb.com

println("Hello")
来源：http://ueq.zhongyouzk.top

[T52] Scala：变量
来源：http://tcf.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://rfe.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://vir.jqgfzy.top

s"值: $b"
来源：http://uhk.316326.xyz

[T54] Scala：集合映射
来源：http://ucz.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://nqg.fzhhl.top

[T55] Scala：集合过滤
来源：http://qok.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kih.zhixingplan.top

[T56] Scala：样例类
来源：http://pbu.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://qtq.yfazqb.com

[T57] Scala：模式匹配
来源：http://fkt.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lcw.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://qkj.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://csq.chenlongwang.top

[T59] Scala：循环
来源：http://hsg.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://ypl.fktsv.cn

[T60] Scala：折叠
来源：http://dqs.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ktc.zhixingplan.top

================================================================================
来源：http://tfk.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jhl.fktsv.cn

================================================================================
来源：http://ejn.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://qoi.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xik.cdnleiting.top

[U02] Py：导出 / 安装依赖
来源：http://yck.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ocb.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://cgx.hcnkem.com

from dotenv import load_dotenv; load_dotenv()
来源：http://rze.fehbvm.com

[U04] Py：变量调试打印
来源：http://flh.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qsg.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://avl.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://flm.redwolf501.top

[U06] Py：合并两个字典
来源：http://sks.aibaodan.cn

{**a, **b}
来源：http://dvq.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://mgv.c1oappe.top

{v: k for k, v in d.items()}
来源：http://fep.fehbvm.com

[U08] Py：展平二维列表
来源：http://iug.jqgufenzy.top

[y for x in nested for y in x]
来源：http://wyp.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://khs.jyoumei.cn

max(d, key=d.get)
来源：http://lii.cashguo.top

[U10] Py：按值排序字典
来源：http://nms.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gti.redwolf501.top

[U11] Py：生成器表达式
来源：http://fal.fktsv.cn

(x * 2 for x in arr)
来源：http://isx.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://biz.nanxinkj.top

Counter(arr).most_common(3)
来源：http://tdg.sysykeji.top

[U13] Py：固定长度队列
来源：http://rqd.birdmap.top

deque(maxlen=10)
来源：http://uvr.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://flc.xuanzx.com

defaultdict(list)
来源：http://gjd.nanxinkj.top

[U15] Py：高精度计时
来源：http://hlc.0kj1m.cn

t = time.perf_counter()
来源：http://lyw.yj20258888.top

[U16] Py：命令行参数解析
来源：http://rbj.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rok.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://hgm.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://dfe.dashuyun.cn

[U18] Py：预编译正则
来源：http://kih.hywenlv.cn

pat = re.compile(r"\d+")
来源：http://xpp.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://rnb.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rbq.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://yna.haohaochexian.top

@functools.lru_cache(maxsize=None)
来源：http://wyq.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://fxo.feifeiyinyue.top

@contextlib.contextmanager
来源：http://rcf.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://zuz.shuidangran.top

list(zip(*m))
来源：http://pej.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://sbe.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ssi.xinyue.icu

[U24] Py：路径操作
来源：http://kog.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sgc.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://tkv.wangdashe.top

csv.DictReader(f)
来源：http://jmv.jqgfzy.top

[U26] Py：并发下载
来源：http://jxh.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bnb.hfpthk.cn

[U27] Py：异步 HTTP
来源：http://uzx.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://kfl.cucudq.cn

[U28] Py：类型别名
来源：http://tmq.vehdjk.com

UserId = int
来源：http://cyg.bjfxy.top

[U29] Py：属性校验
来源：http://hyk.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://lzb.jinqigfzy.top

[U30] Py：数据类
来源：http://cns.guannengcc.top

@dataclass(slots=True)
来源：http://sxt.dianchejie.cn

[U31] Py：单测
来源：http://cbk.c1oappe.top

python -m pytest -q
来源：http://vyl.ehwqpu.com

[U32] Py：代码格式化
来源：http://hyf.nwbrower.top

ruff format . && ruff check --fix .
来源：http://uyh.hcnkem.com

[U33] Py：打包发布
来源：http://zrk.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://qps.ydjk.org.cn

[U34] Py：判断编码
来源：http://unc.yuxming.cn

chardet.detect(raw)
来源：http://gro.hesvh.cn

[U35] Py：发送邮件
来源：http://cmz.hammf.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nww.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://eau.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://fmx.zycfv.cn

[U37] Py：读写 Excel
来源：http://qvg.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://mkr.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://wbe.kuanghao11.cn

Path(__file__).resolve().parent
来源：http://nzh.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://hbj.nanxuanxn.top

sys.stdout.isatty()
来源：http://ess.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://nvw.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://ncw.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://zbi.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bxn.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://ggu.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blo.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://kbd.cheryme.top

namespace App\Http;
来源：http://zgh.ydzc1.top

[U44] PHP：开启严格类型
来源：http://dpy.cdnleiting.top

declare(strict_types=1);
来源：http://wdm.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://esr.fehbvm.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://fgy.zhongyouzk.top

[U46] PHP：可空类型
来源：http://moy.gaohongyu789.top

?string $name = null
来源：http://dhi.zhoulong.xyz

[U47] PHP：联合类型
来源：http://ktr.tianlin.xyz

int|string $id
来源：http://ekq.daria6918.cn

[U48] PHP：纯枚举
来源：http://zod.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ubm.tanke756.top

[U49] PHP：只读属性
来源：http://uhv.fanxiaobao.xyz

public readonly string $name
来源：http://qsp.shanyushiyangtech.top

[U50] PHP：构造器属性提升
来源：http://cty.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://ckw.yvedp.cn

[U51] PHP：数组解构
来源：http://ouz.sxryk.cn

[$a, $b] = $arr;
来源：http://sjd.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://cbg.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://icl.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://yrk.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://kbn.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://evs.sufxvd.cn

$obj?->method()
来源：http://jhu.aibaodan.cn

[U55] PHP：match 表达式
来源：http://xgl.zhijiandao.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qur.cashguo.top

[U56] PHP：命名参数
来源：http://ptu.cucudq.cn

f(a: 1, b: 2)
来源：http://umn.daxiang520.top

[U57] PHP：字符串插值
来源：http://qbd.kuanghao11.cn

"值: {$a}"
来源：http://phu.guannengcc.top

[U58] PHP：数组三件套
来源：http://wod.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cib.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://otu.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cuu.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://zjd.haohaochexian.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uwm.sjlbkw.cn

[U61] PHP：正则
来源：http://xdz.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blj.guannengcc.top

[U62] PHP：日期对象
来源：http://wtg.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zul.havefunace.top

[U63] PHP：文件读写
来源：http://hvh.xziqi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dlz.yuxming.cn

[U64] PHP：目录遍历
来源：http://eie.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://jbc.uphjek.com

[U65] PHP：会话
来源：http://chh.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://jbn.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://mgm.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kfr.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://rtq.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://naa.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://kkc.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qey.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://tyv.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zdw.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://wes.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sii.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://kes.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://mgp.gzhubu.top

[U72] PHP：写错误日志
来源：http://slm.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://ubo.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://msa.yuanzhike.top

parse_ini_file("config.ini", true)
来源：http://ydj.jianghu66.top

[U74] PHP：读取环境变量
来源：http://qpl.gzhubu.top

getenv("APP_ENV") ?: "production"
来源：http://dhl.guannengcc.top

[U75] PHP：依赖注入
来源：http://gkf.yj202588.top

composer require psr/container
来源：http://vhz.yangfankeji.com

[U76] PHP：简单路由
来源：http://khj.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kzf.hcnkem.com

[U77] PHP：模板渲染
来源：http://wxf.cqqwz.cn

composer require twig/twig
来源：http://cxc.fengsongda.top

[U78] PHP：单元测试
来源：http://vst.ybcxt.top

composer require --dev phpunit/phpunit
来源：http://obt.yonumen.top

[U79] PHP：静态分析
来源：http://hta.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://boz.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://tgv.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xxf.xuetiantiany.cn

[U81] JS：初始化项目
来源：http://ijm.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://tjl.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://hzg.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hqi.zdbjq.cn

[U83] JS：ES Module 导入导出
来源：http://smo.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://ocu.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://vlv.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://njs.havefunace.top

[U85] JS：可选链
来源：http://qlh.uphjek.com

a?.b?.c
来源：http://vmn.cucudq.cn

[U86] JS：空值合并
来源：http://ghe.zhengqikj.top

a ?? b
来源：http://uio.uphjek.com

[U87] JS：解构默认值
来源：http://ecq.gaohongyu789.top

const { a = 1, b = 2 } = obj;
来源：http://xyi.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://cre.redwolf501.top

{ ...a, ...b }
来源：http://tfo.ppjwa.cn

[U89] JS：数组去重
来源：http://ure.andypj.xyz

[...new Set(arr)]
来源：http://yvi.jqgufenzy.top

[U90] JS：数字数组排序
来源：http://ymw.nanxinkj.top

[...arr].sort((a, b) => a - b)
来源：http://lrb.xylfe.cn


<!-- 参考信息 -->