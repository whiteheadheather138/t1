代发 wailian999

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gykkqqxsl.sHtML

"值: $a"
来源：http://3g.sjlbkw.cn/Article/details/ggqvspjmc.sHtML

[T44] Perl：条件
来源：http://www.share.bbcook.cn/Article/details/gbbplpvsl.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/gwnepsyjp.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gaaedleqq.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.vehdjk.com/Article/details/gwbtxubse.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gmwawnevq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/giswoflpy.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gqthvhrix.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fktsv.cn/Article/details/gzxmpghps.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gbujjvtkh.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gaqojxnud.sHtML

[T49] Perl：函数
来源：http://mobile.epnwcf.com/Article/details/ganvajaac.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gjwbuawww.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gnztpznfw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gcdayhtxi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.bbcook.cn/Article/details/gxakojqrm.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gfgghgqzo.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gbykasfjq.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gzbzwlxrq.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gijqfjfsm.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gnsoergqg.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/giainzuya.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/grxgmtfgw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gtxqyvmda.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/ggwpuaydl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gmywibjhq.sHtML

[T56] Scala：样例类
来源：http://www.blog.bbcook.cn/Article/details/goaoqohnc.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gfrexuaii.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gyedmoxbr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/ghbyhhktk.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gmewvdoue.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gobdewmwe.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gjmjvljri.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gbyknxaxt.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gqwdtrqus.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/gpaiqjpph.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gznxxzyuu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gewbtgbws.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjmitiyzo.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gouqydaqy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.yfazqb.com/Article/details/gzgvjzgfh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/giutykbek.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gdsrlnxjn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/grcizlreq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.fktsv.cn/Article/details/gpgjehdpo.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/gxxdczjeo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gzwearxzt.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/ggtmhdlzd.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gcelhomsq.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gltwgbmsf.sHtML

{**a, **b}
来源：http://m.share.fktsv.cn/Article/details/gvgnmmgxm.sHtML

[U07] Py：反转字典键值
来源：http://m.share.vehdjk.com/Article/details/gzzyrpnzk.sHtML

{v: k for k, v in d.items()}
来源：http://baike.bbcook.cn/Article/details/gtqfmyvsq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.yfazqb.com/Article/details/gdjrvseor.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gvcmanoxy.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gzuykhhoq.sHtML

max(d, key=d.get)
来源：http://mobile.fktsv.cn/Article/details/gwjcpfufw.sHtML

[U10] Py：按值排序字典
来源：http://m.share.epnwcf.com/Article/details/gwogrphpo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/grkviqxrc.sHtML

[U11] Py：生成器表达式
来源：http://m.share.tarul.cn/Article/details/gymwfgcmx.sHtML

(x * 2 for x in arr)
来源：http://www.share.bbcook.cn/Article/details/gfktoxzsv.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/guszrehow.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/grkuibgdo.sHtML

[U13] Py：固定长度队列
来源：http://read.share.epnwcf.com/Article/details/gfudxyycj.sHtML

deque(maxlen=10)
来源：http://3g.vehdjk.com/Article/details/gskfxzgnf.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/glbbnufme.sHtML

defaultdict(list)
来源：http://www.share.tarul.cn/Article/details/ggqpiauth.sHtML

[U15] Py：高精度计时
来源：http://blog.sjlbkw.cn/Article/details/gfiegsbkc.sHtML

t = time.perf_counter()
来源：http://www.m.share.fktsv.cn/Article/details/gyrvmzzxu.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gjeeplree.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.sjlbkw.cn/Article/details/gusijbtmg.sHtML

[U17] Py：初始化日志
来源：http://wap.fktsv.cn/Article/details/gnzwaaodx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbcrosea.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gijdxitbp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gjnkunnnk.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/gvessocih.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.bbcook.cn/Article/details/gllcxhiga.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gfzvlorgq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://m.share.yfazqb.com/Article/details/gvpnhkfly.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.sjlbkw.cn/Article/details/gkuowqhxi.sHtML

@contextlib.contextmanager
来源：http://wap.sjlbkw.cn/Article/details/gjzrgpghj.sHtML

[U22] Py：矩阵转置
来源：http://www.share.sjlbkw.cn/Article/details/guvqslrkp.sHtML

list(zip(*m))
来源：http://blog.fktsv.cn/Article/details/gunyfjvbv.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/ghpmqtppu.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.yfazqb.com/Article/details/garmegkrj.sHtML

[U24] Py：路径操作
来源：http://baike.vehdjk.com/Article/details/gmzbrjqqg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gexbibcab.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gudsgfwct.sHtML

csv.DictReader(f)
来源：http://baike.tarul.cn/Article/details/gihwhkyhn.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/gdwxxbqcb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gynmupigx.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/ggpdkshcl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.yfazqb.com/Article/details/gjwaqekus.sHtML

[U28] Py：类型别名
来源：http://blog.sjlbkw.cn/Article/details/gvjokekcg.sHtML

UserId = int
来源：http://wap.vehdjk.com/Article/details/gciigyfos.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/glvtchall.sHtML

@property 与 @x.setter 配合
来源：http://baike.epnwcf.com/Article/details/gahlltfqh.sHtML

[U30] Py：数据类
来源：http://baike.epnwcf.com/Article/details/gbgcmgzeo.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gsblavlhc.sHtML

[U31] Py：单测
来源：http://www.m.share.epnwcf.com/Article/details/gwifcepbm.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/gddwqkboa.sHtML

[U32] Py：代码格式化
来源：http://m.share.sjlbkw.cn/Article/details/gtpzpfqov.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.vehdjk.com/Article/details/giaukedwj.sHtML

[U33] Py：打包发布
来源：http://m.share.yfazqb.com/Article/details/gfzeimqmr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://mobile.fktsv.cn/Article/details/ghhnwmmle.sHtML

[U34] Py：判断编码
来源：http://read.share.tarul.cn/Article/details/gntlqyixs.sHtML

chardet.detect(raw)
来源：http://www.share.tarul.cn/Article/details/gsnywohid.sHtML

[U35] Py：发送邮件
来源：http://www.blog.fktsv.cn/Article/details/gdkianobh.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gpuqluaeq.sHtML

[U36] Py：定时任务
来源：http://mobile.fktsv.cn/Article/details/goedwvpko.sHtML

schedule.every(10).minutes.do(job)
来源：http://3g.sjlbkw.cn/Article/details/gqjfdbzlv.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/grlakclcm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.tarul.cn/Article/details/gnkhzbvin.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/ggbafwzsk.sHtML

Path(__file__).resolve().parent
来源：http://m.share.bbcook.cn/Article/details/gmxuvmcsb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fktsv.cn/Article/details/gsvidpjqg.sHtML

sys.stdout.isatty()
来源：http://www.m.share.epnwcf.com/Article/details/gxtojzauj.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.tarul.cn/Article/details/giaknuzpv.sHtML

print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gauknvpzh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.vehdjk.com/Article/details/gcymmtzsz.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gwfzzzsye.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.tarul.cn/Article/details/grctzjfbx.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.yfazqb.com/Article/details/gbdhkwmth.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gyyxxddhg.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gyfnszkhx.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.tarul.cn/Article/details/gnnyienck.sHtML

declare(strict_types=1);
来源：http://3g.fktsv.cn/Article/details/gtiubbnkn.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.yfazqb.com/Article/details/geolyzaew.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gqzatynzo.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gkjqjxcnw.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gfmusoplr.sHtML

[U47] PHP：联合类型
来源：http://mobile.sjlbkw.cn/Article/details/gkjhebaip.sHtML

int|string $id
来源：http://www.m.share.sjlbkw.cn/Article/details/gcreqiupi.sHtML

[U48] PHP：纯枚举
来源：http://baike.sjlbkw.cn/Article/details/gzmqlnmhz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.vehdjk.com/Article/details/gbwqpubiq.sHtML

[U49] PHP：只读属性
来源：http://baike.bbcook.cn/Article/details/gdmlljoiy.sHtML

public readonly string $name
来源：http://www.blog.sjlbkw.cn/Article/details/gszrrxyez.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/gkunfrxxg.sHtML

public function __construct(private int $id) {}
来源：http://wap.vehdjk.com/Article/details/gjdsiymhl.sHtML

[U51] PHP：数组解构
来源：http://wap.tarul.cn/Article/details/gxxjwudof.sHtML

[$a, $b] = $arr;
来源：http://wap.bbcook.cn/Article/details/gyzqydkmx.sHtML

[U52] PHP：箭头函数
来源：http://wap.fktsv.cn/Article/details/gezjvdtgn.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.yfazqb.com/Article/details/grzebdses.sHtML

[U53] PHP：空合并运算符
来源：http://blog.fktsv.cn/Article/details/gkyvvysif.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.bbcook.cn/Article/details/gxhnfgloa.sHtML

[U54] PHP：空安全调用
来源：http://baike.epnwcf.com/Article/details/ghxbokasv.sHtML

$obj?->method()
来源：http://baike.vehdjk.com/Article/details/gnkbxbbqz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gduowlort.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gstnxebqc.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gibbqwgfv.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/ggplxtlsx.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gejluvdjb.sHtML

"值: {$a}"
来源：http://baike.yfazqb.com/Article/details/gaieveioc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/gjqvanzne.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.bbcook.cn/Article/details/gioqvbocj.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/guctnjfve.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gbjhknbjo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/grxinwmch.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.yfazqb.com/Article/details/ghxqkthym.sHtML

[U61] PHP：正则
来源：http://baike.vehdjk.com/Article/details/gdgysivvp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/glcigyyvh.sHtML

[U62] PHP：日期对象
来源：http://mobile.bbcook.cn/Article/details/gcowtshyv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fktsv.cn/Article/details/gmpcbcrei.sHtML

[U63] PHP：文件读写
来源：http://baike.bbcook.cn/Article/details/gjgpeidqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.yfazqb.com/Article/details/gmqanmvnk.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/golquinbd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/ghiaezubq.sHtML

[U65] PHP：会话
来源：http://m.share.fktsv.cn/Article/details/gmndivbnu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gwcklyxuc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.epnwcf.com/Article/details/gcbdjpqzj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gwxfdpwlu.sHtML

[U67] PHP：处理文件上传
来源：http://blog.yfazqb.com/Article/details/gcxdgtabp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.bbcook.cn/Article/details/gzshqqwdb.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gaedznhlq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.tarul.cn/Article/details/gfhiqtmma.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/goisrzmco.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/gobmyomkn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/gljznnyxo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gpgoyhaiw.sHtML

[U71] PHP：抛出异常
来源：http://wap.epnwcf.com/Article/details/gwlpdvwyu.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gigbspjre.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gxlzcflqk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/guyidcwwn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.bbcook.cn/Article/details/gkdepbmgx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/gbfiyqjct.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/grmdjtxnl.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.epnwcf.com/Article/details/gytlcwgft.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fktsv.cn/Article/details/gaagmkazg.sHtML

composer require psr/container
来源：http://wap.vehdjk.com/Article/details/gechzmffw.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.yfazqb.com/Article/details/gkqqmgetw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/glpzemamv.sHtML

[U77] PHP：模板渲染
来源：http://www.share.tarul.cn/Article/details/gzhntduat.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gkmebuozo.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/gbzzoyjiy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/guqnaclpo.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gldrdxcwn.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/ghspoffvf.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.epnwcf.com/Article/details/gifzsqllb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gblobflfo.sHtML

[U81] JS：初始化项目
来源：http://baike.bbcook.cn/Article/details/gbibadjuv.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/gytiurlav.sHtML

[U82] JS：package.json 脚本
来源：http://3g.sjlbkw.cn/Article/details/gdhgvjgzp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gngywvfil.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gyjdhcsqe.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gcoedlldy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/gntvwclne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.epnwcf.com/Article/details/gcftpjung.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/glfqimdks.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/gkxacllel.sHtML

[U86] JS：空值合并
来源：http://read.share.vehdjk.com/Article/details/gfyuwctoz.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gygemsplm.sHtML

[U87] JS：解构默认值
来源：http://www.share.vehdjk.com/Article/details/gssgineet.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.epnwcf.com/Article/details/gatmwtzcv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gowuyusqk.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gncdokdmd.sHtML

[U89] JS：数组去重
来源：http://wap.fktsv.cn/Article/details/gyipwhbbe.sHtML

[...new Set(arr)]
来源：http://mobile.tarul.cn/Article/details/gvkjxuqyu.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gxhjrjooe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gmjhoyeew.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gjconovdo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.fktsv.cn/Article/details/ghrrrgdgc.sHtML

[U92] JS：深拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/ggpndptkh.sHtML

structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gutulamvy.sHtML

[U93] JS：模板字符串
来源：http://baike.yfazqb.com/Article/details/gdvcvngkv.sHtML

`共 ${n} 条`
来源：http://baike.sjlbkw.cn/Article/details/gmxaljlnn.sHtML

[U94] JS：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gqiznoaaq.sHtML

const double = x => x * 2;
来源：http://www.share.bbcook.cn/Article/details/gcxyyujbk.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gddbxspie.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gkjwneeda.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gnambihnz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gfcevfonj.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/gztykcpjw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gffrxhmck.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gwieezvlu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fktsv.cn/Article/details/gepjlznjv.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gcfraapul.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/giluryrhu.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fktsv.cn/Article/details/gxltbdtiw.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gptnrwifj.sHtML

[U101] JS：classList 操作
来源：http://m.share.sjlbkw.cn/Article/details/ghpjtysua.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gmzdyasax.sHtML

[U102] JS：本地存储
来源：http://www.blog.tarul.cn/Article/details/gqawjpnad.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fktsv.cn/Article/details/glybgpmfv.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/ghestntsr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.sjlbkw.cn/Article/details/gxrflspgi.sHtML

[U104] JS：防抖
来源：http://blog.yfazqb.com/Article/details/gldrkzcmj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gqcebjplq.sHtML

[U105] JS：节流
来源：http://m.share.bbcook.cn/Article/details/gibegrrud.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gcgxvdsxl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gizsmpkim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.sjlbkw.cn/Article/details/gkdhfozvp.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gowgnliut.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gslazrppy.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/gfzywpdvq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.vehdjk.com/Article/details/ggxylhxob.sHtML

[U109] JS：数组分组
来源：http://www.blog.sjlbkw.cn/Article/details/gqlvswtkm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gimhwjckr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fktsv.cn/Article/details/gvmgnjvmm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.bbcook.cn/Article/details/gbvdvzsgf.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gbujmrwga.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gbflvtjoh.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gcyjaqobt.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gldronaqt.sHtML

[U113] JS：正则替换全部
来源：http://baike.fktsv.cn/Article/details/gklfhupnv.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gzgcdqibg.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.bbcook.cn/Article/details/geumrehkn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gpiynokat.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gkzgrpxfs.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gzvlusxfd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.bbcook.cn/Article/details/gurijaouz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.yfazqb.com/Article/details/gdrwcsrdz.sHtML

[U117] JS：单元测试
来源：http://3g.fktsv.cn/Article/details/gkgaajyke.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.sjlbkw.cn/Article/details/gsrwzlphi.sHtML

[U118] JS：开发服务器
来源：http://3g.yfazqb.com/Article/details/gryqmavvx.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gzavhsyxu.sHtML

[U119] JS：生产构建
来源：http://3g.tarul.cn/Article/details/gexxtokep.sHtML

npx vite build
来源：http://blog.bbcook.cn/Article/details/gqdepyquv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.sjlbkw.cn/Article/details/gdymlbgqr.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gdudesoft.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnajwmqs.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gmwexzhdp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbabwxxcm.sHtML

按语言统计（条）：
来源：http://m.share.epnwcf.com/Article/details/guydmtryk.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gxvitigic.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gbggijvsj.sHtML

JavaScript ..... 252
来源：http://read.share.bbcook.cn/Article/details/grwcawamx.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/giifuirvl.sHtML

Java ........... 212
来源：http://baike.sjlbkw.cn/Article/details/gkseqtcds.sHtML

Go ............. 212
来源：http://www.m.share.bbcook.cn/Article/details/gtesrgdkj.sHtML

Ruby ........... 212
来源：http://wap.tarul.cn/Article/details/gijamxusv.sHtML

C# ............. 212
来源：http://baike.epnwcf.com/Article/details/gcroipmzi.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/gjnoiulzb.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/grwierlsf.sHtML

SQL ............ 90
来源：http://blog.vehdjk.com/Article/details/gnddjahck.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/ggfxrgdpf.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gtkcgwyup.sHtML

Swift .......... 15
来源：http://www.m.share.tarul.cn/Article/details/gumqwxwzx.sHtML

Lua ............ 10
来源：http://www.share.fktsv.cn/Article/details/ghkudsupc.sHtML

Perl ........... 10
来源：http://www.blog.fktsv.cn/Article/details/ggwsbbxjv.sHtML


<!-- 参考信息 -->