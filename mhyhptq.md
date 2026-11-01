代发 wailian999

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/gzjeqzcnb.sHtML

print "Hello\n";
来源：http://wap.bbcook.cn/Article/details/gvzaqpmgx.sHtML

[T42] Perl：变量类型
来源：http://m.share.epnwcf.com/Article/details/gwluekbwj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gckzmxcfp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gluadusno.sHtML

"值: $a"
来源：http://blog.fktsv.cn/Article/details/geefyeiuj.sHtML

[T44] Perl：条件
来源：http://www.share.fktsv.cn/Article/details/gfozmmlyp.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/grehlunxk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.tarul.cn/Article/details/gxylhpnhe.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gdmckuqmo.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/ggiysekko.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gdyxwldwa.sHtML

[T47] Perl：正则捕获
来源：http://m.share.sjlbkw.cn/Article/details/guhjedyvk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/glfnevxim.sHtML

[T48] Perl：正则替换
来源：http://read.share.yfazqb.com/Article/details/gicbgorjy.sHtML

$s =~ s/old/new/g;
来源：http://mobile.bbcook.cn/Article/details/gtgtvdbbq.sHtML

[T49] Perl：函数
来源：http://www.blog.tarul.cn/Article/details/gndjlkecw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gsgwnpxit.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/glqdyhsrg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gubengqer.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fktsv.cn/Article/details/gyzhenyzj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ghfykhzmi.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gqzbpxvuu.sHtML

[T52] Scala：变量
来源：http://blog.sjlbkw.cn/Article/details/gjsyjpaqz.sHtML

val a = 1;  var b = 2
来源：http://www.share.bbcook.cn/Article/details/gncslvxwl.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gxnpnsqwx.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gyowcawcy.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gndvnnkbp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/gjsaeahhn.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.epnwcf.com/Article/details/girbbzzea.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gmfetcnzc.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/ggvkvmwnm.sHtML

case class User(name: String, age: Int)
来源：http://read.share.tarul.cn/Article/details/gyihwngaj.sHtML

[T57] Scala：模式匹配
来源：http://m.share.vehdjk.com/Article/details/grycnzoef.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.tarul.cn/Article/details/gwdfmxavg.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/ggsidboqy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.epnwcf.com/Article/details/grxjvxwbj.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gwltqeabl.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gqlrjajsb.sHtML

[T60] Scala：折叠
来源：http://3g.fktsv.cn/Article/details/gfscznczy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/gzxjkxnut.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcpcqmcqu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fktsv.cn/Article/details/gwzjvguss.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwklouypk.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gzhhyaqkj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gymbxylej.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gzepwsybk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.epnwcf.com/Article/details/gcugydfvc.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gchwlqame.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.sjlbkw.cn/Article/details/greftjwpp.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gwxqxswlx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.sjlbkw.cn/Article/details/gbypwykdb.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gkltmjjnx.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gvtawfklg.sHtML

[U06] Py：合并两个字典
来源：http://blog.bbcook.cn/Article/details/grokaktdq.sHtML

{**a, **b}
来源：http://www.blog.bbcook.cn/Article/details/gmcmlhgch.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/gaqdohryp.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.fktsv.cn/Article/details/guustikrr.sHtML

[U08] Py：展平二维列表
来源：http://blog.yfazqb.com/Article/details/gaqcwifjy.sHtML

[y for x in nested for y in x]
来源：http://www.share.epnwcf.com/Article/details/gsovwbxlj.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.epnwcf.com/Article/details/gxpkvadps.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gtrujpjhz.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gamucrgmq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.epnwcf.com/Article/details/gugoelepl.sHtML

[U11] Py：生成器表达式
来源：http://read.share.bbcook.cn/Article/details/guytrkznp.sHtML

(x * 2 for x in arr)
来源：http://m.share.tarul.cn/Article/details/gmffsctac.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/gmndmuzqf.sHtML

Counter(arr).most_common(3)
来源：http://wap.vehdjk.com/Article/details/gjkfmnnxm.sHtML

[U13] Py：固定长度队列
来源：http://read.share.yfazqb.com/Article/details/ghxljvudr.sHtML

deque(maxlen=10)
来源：http://www.m.share.vehdjk.com/Article/details/gnoilrats.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gnwkvvejb.sHtML

defaultdict(list)
来源：http://3g.vehdjk.com/Article/details/gkssyfqtm.sHtML

[U15] Py：高精度计时
来源：http://mobile.fktsv.cn/Article/details/gduuczxlj.sHtML

t = time.perf_counter()
来源：http://baike.bbcook.cn/Article/details/gxjmxxfzr.sHtML

[U16] Py：命令行参数解析
来源：http://3g.bbcook.cn/Article/details/glryzrvzu.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.sjlbkw.cn/Article/details/gsdwlfxzy.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/gwxxpyxnl.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.yfazqb.com/Article/details/gmysvjryo.sHtML

[U18] Py：预编译正则
来源：http://wap.vehdjk.com/Article/details/gzdysqali.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gfzprpqha.sHtML

[U19] Py：正则替换带回调
来源：http://blog.vehdjk.com/Article/details/gzmhbbtgd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gbatmnzta.sHtML

[U20] Py：缓存函数结果
来源：http://3g.epnwcf.com/Article/details/gzifkdbce.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.sjlbkw.cn/Article/details/gdvpgttmw.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.epnwcf.com/Article/details/ghgyklqbl.sHtML

@contextlib.contextmanager
来源：http://3g.vehdjk.com/Article/details/giejqwqor.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gmxioncse.sHtML

list(zip(*m))
来源：http://read.share.epnwcf.com/Article/details/gkqwmyetm.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/ghncsqxha.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/gpejlhgec.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gwjmfdxjn.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.fktsv.cn/Article/details/gvxrhjzfm.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gjranoikk.sHtML

csv.DictReader(f)
来源：http://www.blog.fktsv.cn/Article/details/gxccbhkph.sHtML

[U26] Py：并发下载
来源：http://baike.epnwcf.com/Article/details/gzrtllawp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.bbcook.cn/Article/details/ghfgkdbdq.sHtML

[U27] Py：异步 HTTP
来源：http://blog.sjlbkw.cn/Article/details/gyqydqrhv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.fktsv.cn/Article/details/guessmfyv.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gmgqovkia.sHtML

UserId = int
来源：http://www.share.tarul.cn/Article/details/gwplfptmj.sHtML

[U29] Py：属性校验
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjdjqmxr.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.sjlbkw.cn/Article/details/gglfqzqkm.sHtML

[U30] Py：数据类
来源：http://wap.tarul.cn/Article/details/gffmzkbrf.sHtML

@dataclass(slots=True)
来源：http://www.share.tarul.cn/Article/details/gnhwnbcjg.sHtML

[U31] Py：单测
来源：http://read.share.tarul.cn/Article/details/gngzykotp.sHtML

python -m pytest -q
来源：http://baike.fktsv.cn/Article/details/ggsvcaysx.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/gmxsjfeso.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/goujhnrco.sHtML

[U33] Py：打包发布
来源：http://www.blog.vehdjk.com/Article/details/gqnadsikq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/ggcpowjln.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gbpbqbabr.sHtML

chardet.detect(raw)
来源：http://www.blog.yfazqb.com/Article/details/garbzumoi.sHtML

[U35] Py：发送邮件
来源：http://wap.vehdjk.com/Article/details/gcvspqoab.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.fktsv.cn/Article/details/gplxonezz.sHtML

[U36] Py：定时任务
来源：http://mobile.yfazqb.com/Article/details/gmqhkogia.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.vehdjk.com/Article/details/gnyotizkd.sHtML

[U37] Py：读写 Excel
来源：http://3g.fktsv.cn/Article/details/gdrybduqc.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://wap.fktsv.cn/Article/details/gafhecpan.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gxraorirc.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gdkhobhjp.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.tarul.cn/Article/details/gyefaxvjw.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gszcfwldv.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.epnwcf.com/Article/details/ghubsjgot.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzkzxkdl.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/gbfecaklj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gdavtotru.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gyaaflsky.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fktsv.cn/Article/details/ghexdvczv.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.fktsv.cn/Article/details/ghzampest.sHtML

namespace App\Http;
来源：http://www.share.yfazqb.com/Article/details/ggnjulfbm.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.yfazqb.com/Article/details/gbmwuwhxu.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gccdgpnav.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fktsv.cn/Article/details/gopoxabkq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.vehdjk.com/Article/details/gzfqypyum.sHtML

[U46] PHP：可空类型
来源：http://baike.vehdjk.com/Article/details/gchrezecf.sHtML

?string $name = null
来源：http://www.m.share.yfazqb.com/Article/details/gjqlyywhp.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gvpymugrr.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gvsstxwyu.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gpzwkxkeg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gneawssdr.sHtML

[U49] PHP：只读属性
来源：http://3g.sjlbkw.cn/Article/details/gamluskfo.sHtML

public readonly string $name
来源：http://mobile.yfazqb.com/Article/details/gqfkzrckg.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/glorfxscp.sHtML

public function __construct(private int $id) {}
来源：http://3g.epnwcf.com/Article/details/ggqepipgu.sHtML

[U51] PHP：数组解构
来源：http://www.share.sjlbkw.cn/Article/details/ghcilkjhn.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gpencsdcz.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gyphcjatu.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gsghcorwe.sHtML

[U53] PHP：空合并运算符
来源：http://blog.vehdjk.com/Article/details/glcitqxfn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.bbcook.cn/Article/details/gypupkmpy.sHtML

[U54] PHP：空安全调用
来源：http://mobile.yfazqb.com/Article/details/gruhtzgje.sHtML

$obj?->method()
来源：http://3g.bbcook.cn/Article/details/gcfefqmeo.sHtML

[U55] PHP：match 表达式
来源：http://baike.yfazqb.com/Article/details/gersnjdmv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.yfazqb.com/Article/details/gygidqtqp.sHtML

[U56] PHP：命名参数
来源：http://3g.sjlbkw.cn/Article/details/gqmgawqln.sHtML

f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/gjrwtyjdi.sHtML

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/gnwvjiygc.sHtML

"值: {$a}"
来源：http://blog.yfazqb.com/Article/details/guwmtdrbg.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/guathkaqn.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.epnwcf.com/Article/details/gsaowvipi.sHtML

[U59] PHP：自定义排序
来源：http://m.share.vehdjk.com/Article/details/gxxzevdqw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.tarul.cn/Article/details/gardtfmxk.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.bbcook.cn/Article/details/gqqjgjgpa.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gyiiuyjct.sHtML

[U61] PHP：正则
来源：http://www.m.share.tarul.cn/Article/details/gkavsiglb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.epnwcf.com/Article/details/gosujjmac.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gpxcmmfgt.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gsobznsve.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/gziklampu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/grhcmrpxh.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fktsv.cn/Article/details/gtgoxlydt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/gpcdoulzj.sHtML

[U65] PHP：会话
来源：http://wap.sjlbkw.cn/Article/details/gaaqbccrl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gwfoukwla.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.epnwcf.com/Article/details/gzunngksv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fktsv.cn/Article/details/gskeudqcm.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fktsv.cn/Article/details/gndkupeoq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.sjlbkw.cn/Article/details/guamnpori.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gzxsmihpo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjoitbhy.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/gevlwxpzu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/gzxwkqkxd.sHtML

[U70] PHP：PDO 事务
来源：http://3g.vehdjk.com/Article/details/geuyoooqx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.vehdjk.com/Article/details/gtjyoojab.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gteotnnlf.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fktsv.cn/Article/details/gmpqpddye.sHtML

[U72] PHP：写错误日志
来源：http://blog.epnwcf.com/Article/details/gpuxshpat.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.epnwcf.com/Article/details/gavmwhnqu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/gpqurgxct.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.sjlbkw.cn/Article/details/guptucsqi.sHtML

[U74] PHP：读取环境变量
来源：http://baike.bbcook.cn/Article/details/gybeprasa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/gqkxzrcic.sHtML

[U75] PHP：依赖注入
来源：http://wap.bbcook.cn/Article/details/gefzebvnh.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/gjhhmfqso.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/guijvwrzt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.yfazqb.com/Article/details/gmwyuaorz.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/gfaktxkwl.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/guobdnoaj.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gltsootts.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.vehdjk.com/Article/details/gkdqrdivq.sHtML

[U79] PHP：静态分析
来源：http://baike.vehdjk.com/Article/details/gahktjtod.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gkopfbess.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.yfazqb.com/Article/details/gyirtqspd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fktsv.cn/Article/details/gugjjkacj.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/grxuczelr.sHtML

npm init -y;  npm i express
来源：http://www.m.share.sjlbkw.cn/Article/details/gggpmitey.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fktsv.cn/Article/details/gflreaxfu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/greslyzkf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.sjlbkw.cn/Article/details/gdjwlhabp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gdauhbvdl.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fktsv.cn/Article/details/gxmbkgcpj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.tarul.cn/Article/details/gxfjcmzks.sHtML

[U85] JS：可选链
来源：http://www.share.vehdjk.com/Article/details/gphfvgbto.sHtML

a?.b?.c
来源：http://mobile.vehdjk.com/Article/details/grdlpoweb.sHtML

[U86] JS：空值合并
来源：http://blog.tarul.cn/Article/details/ggdgntbgk.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gekjtbtyb.sHtML

[U87] JS：解构默认值
来源：http://baike.vehdjk.com/Article/details/gtsysuqdj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.sjlbkw.cn/Article/details/ghcuidqsv.sHtML

[U88] JS：对象展开合并
来源：http://www.share.vehdjk.com/Article/details/grtoxzgja.sHtML

{ ...a, ...b }
来源：http://www.share.epnwcf.com/Article/details/ggkxzltjs.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gsjwghsgj.sHtML

[...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gatlcwymb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gkpvgtldo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gqwvskiyj.sHtML

[U91] JS：对象键值遍历
来源：http://wap.yfazqb.com/Article/details/giiujziui.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.sjlbkw.cn/Article/details/gvshtndim.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/gxprkdeaa.sHtML

structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gmiutwenl.sHtML

[U93] JS：模板字符串
来源：http://read.share.tarul.cn/Article/details/gxjddphbj.sHtML

`共 ${n} 条`
来源：http://www.blog.sjlbkw.cn/Article/details/gjummhwgi.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.epnwcf.com/Article/details/gpifrpdrm.sHtML

const double = x => x * 2;
来源：http://3g.vehdjk.com/Article/details/glhonlkme.sHtML

[U95] JS：Promise 包装
来源：http://wap.bbcook.cn/Article/details/gwkpnztzt.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gbwzgjqys.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/gbqjpqfdd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gfprrtegh.sHtML

[U97] JS：并发请求
来源：http://www.blog.sjlbkw.cn/Article/details/gnkpdfrnc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gvwncsdkv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gnhycgmtc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.epnwcf.com/Article/details/gsaehylmm.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gmxzbczwn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.vehdjk.com/Article/details/gxkmngeod.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.bbcook.cn/Article/details/gtoezljki.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/guaplhlkt.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gfdwdwcfn.sHtML

el.classList.toggle("active")
来源：http://mobile.tarul.cn/Article/details/gzdixdjva.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/ghezcaujp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gvecoofno.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gmchgqguf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.tarul.cn/Article/details/gwlmjzawt.sHtML

[U104] JS：防抖
来源：http://read.share.fktsv.cn/Article/details/glhrnwhyz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ggvwrwcyg.sHtML

[U105] JS：节流
来源：http://m.share.vehdjk.com/Article/details/gpfbwfwiz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.vehdjk.com/Article/details/gefxeoczi.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gudzzzijk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/goytpxbzn.sHtML

[U107] JS：数字千分位
来源：http://blog.epnwcf.com/Article/details/gfgbteckf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gqjmtzjou.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/galbtklfn.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/grkxhyauv.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gvddlotwu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/giqhxiozh.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gzkoserxv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gjvdikbau.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/gtiyzhznp.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gabcyjmdh.sHtML

[U112] JS：字符串补位
来源：http://3g.vehdjk.com/Article/details/gvmdowlhe.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gfidcimjq.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/gnjnmminp.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gioqfggjp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.bbcook.cn/Article/details/grqbfijmu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gnjafnpge.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gbbxqjgtp.sHtML

crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gqxxtndhx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.epnwcf.com/Article/details/gcfhdhzoc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gbaofxfab.sHtML

[U117] JS：单元测试
来源：http://www.m.share.tarul.cn/Article/details/ggabsefui.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gjwqwwowk.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gbsmnwllp.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gtxpjgddr.sHtML

[U119] JS：生产构建
来源：http://wap.yfazqb.com/Article/details/gucbkfvix.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gktmsfply.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.yfazqb.com/Article/details/ghshxzgyv.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.vehdjk.com/Article/details/gwztjgvbl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmbeeapys.sHtML

统计汇总
来源：http://mobile.fktsv.cn/Article/details/gpbvzgftj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfebdepfd.sHtML

按语言统计（条）：
来源：http://baike.epnwcf.com/Article/details/gyqypnivn.sHtML

Python ......... 252
来源：http://blog.fktsv.cn/Article/details/gcmloccia.sHtML

PHP ............ 252
来源：http://read.share.epnwcf.com/Article/details/geeigueqd.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gizzqtykc.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gqfygbsvv.sHtML

Java ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/glbeagruh.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gympaxwma.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gyjjuogmm.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/gpysflhoi.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gfnphxfft.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/ggbdkjpnl.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gngcmdpmf.sHtML

Bash ........... 80
来源：http://wap.vehdjk.com/Article/details/grmxtqcfb.sHtML


<!-- 参考信息 -->