代发 wailian999

[T45] Perl：数组遍历
来源：http://www.blog.fktsv.cn/Article/details/gabwmthhi.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gfvrtispb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gqlelbwpm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzkvswoxu.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gajcpkshh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gibhmntdd.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gkhqisqay.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gxixksgow.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gtbwtitqq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gfqotjqqf.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gnttmilwz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gmzwchfus.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gwirsnbig.sHtML

[T51] Scala：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gfdcrondq.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/glwxklgig.sHtML

[T52] Scala：变量
来源：http://www.blog.fktsv.cn/Article/details/gzhohbdlg.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/gmdxdgxdh.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gppfobwqm.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gfntiycbo.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gszimapbz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/ghgrrbmin.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/gccenkwsg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fktsv.cn/Article/details/gfzkdgwtp.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gavlbzftj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gbututaae.sHtML

[T57] Scala：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gdkctxkzd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gspffhdxw.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fktsv.cn/Article/details/gabwjofyx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/glnxvxzgb.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gnkfcjdjg.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/ggxoirbqf.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gcqjhoxzn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gebnosiha.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gjsgqxvnd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gpjclifcz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/goavthvbi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gxdposvmw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.epnwcf.com/Article/details/gqlcyockl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.bbcook.cn/Article/details/giqjnmxnd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.epnwcf.com/Article/details/gtwqomtaf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.vehdjk.com/Article/details/gyripmvuw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gunmvuhne.sHtML

[U04] Py：变量调试打印
来源：http://mobile.fktsv.cn/Article/details/gggmruvge.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gwaxglzak.sHtML

[U05] Py：列表去重且保序
来源：http://baike.sjlbkw.cn/Article/details/gqaimjajb.sHtML

list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gochcxdpc.sHtML

[U06] Py：合并两个字典
来源：http://3g.yfazqb.com/Article/details/ghhiwktrn.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/grgjmjzhh.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gnamgsfeu.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.bbcook.cn/Article/details/guhtsdlxq.sHtML

[U08] Py：展平二维列表
来源：http://baike.fktsv.cn/Article/details/ghqzfisxf.sHtML

[y for x in nested for y in x]
来源：http://mobile.vehdjk.com/Article/details/gmcrhwqim.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.sjlbkw.cn/Article/details/gycpgzfnk.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoezawej.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/glveplxvk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gqtvhcnba.sHtML

[U11] Py：生成器表达式
来源：http://m.share.vehdjk.com/Article/details/gadpilybg.sHtML

(x * 2 for x in arr)
来源：http://www.share.sjlbkw.cn/Article/details/gdrdxhsnm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/giildfiez.sHtML

Counter(arr).most_common(3)
来源：http://baike.vehdjk.com/Article/details/gdbpsutnb.sHtML

[U13] Py：固定长度队列
来源：http://blog.vehdjk.com/Article/details/grfxpxace.sHtML

deque(maxlen=10)
来源：http://read.share.yfazqb.com/Article/details/gnlnqokmk.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gjhstqthp.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/ghwlpydtn.sHtML

[U15] Py：高精度计时
来源：http://m.share.sjlbkw.cn/Article/details/gvvvbhngc.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gzmgbilcr.sHtML

[U16] Py：命令行参数解析
来源：http://baike.bbcook.cn/Article/details/gthhewenf.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.sjlbkw.cn/Article/details/gtadjfcbv.sHtML

[U17] Py：初始化日志
来源：http://blog.vehdjk.com/Article/details/gfnvssaxt.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.vehdjk.com/Article/details/gsbtmbije.sHtML

[U18] Py：预编译正则
来源：http://mobile.sjlbkw.cn/Article/details/gpdmqhyob.sHtML

pat = re.compile(r"\d+")
来源：http://blog.yfazqb.com/Article/details/gambpskkm.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.vehdjk.com/Article/details/ggpmikymy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/ggizergst.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.yfazqb.com/Article/details/gzgupdehu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.yfazqb.com/Article/details/gainpyssm.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.epnwcf.com/Article/details/gbeswockw.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/grnnixrjv.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gqxzdjoom.sHtML

list(zip(*m))
来源：http://m.share.epnwcf.com/Article/details/gnimzadxv.sHtML

[U23] Py：分块读取大文件
来源：http://3g.yfazqb.com/Article/details/gttzknuwk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.yfazqb.com/Article/details/gvphynzln.sHtML

[U24] Py：路径操作
来源：http://www.m.share.yfazqb.com/Article/details/gfajkuzys.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.vehdjk.com/Article/details/gqegoiios.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.sjlbkw.cn/Article/details/grsjibtej.sHtML

csv.DictReader(f)
来源：http://m.share.fktsv.cn/Article/details/gyynvlusv.sHtML

[U26] Py：并发下载
来源：http://blog.fktsv.cn/Article/details/gkvuxlyns.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gerwmxdrs.sHtML

[U27] Py：异步 HTTP
来源：http://www.m.share.yfazqb.com/Article/details/gqzqybmrz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gdlqguero.sHtML

[U28] Py：类型别名
来源：http://mobile.epnwcf.com/Article/details/gkoeymnlq.sHtML

UserId = int
来源：http://www.share.fktsv.cn/Article/details/guhsratcm.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/gmanqbfgf.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/gvqsgyyng.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gkszsinek.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gukaimnfk.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/ghvndidgh.sHtML

python -m pytest -q
来源：http://m.share.yfazqb.com/Article/details/gfyuzlfzu.sHtML

[U32] Py：代码格式化
来源：http://www.share.fktsv.cn/Article/details/gzjbiuwnq.sHtML

ruff format . && ruff check --fix .
来源：http://baike.fktsv.cn/Article/details/ggikccmoq.sHtML

[U33] Py：打包发布
来源：http://wap.bbcook.cn/Article/details/gbyjzalwk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.bbcook.cn/Article/details/gbqsudytq.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gdkspswpf.sHtML

chardet.detect(raw)
来源：http://m.share.epnwcf.com/Article/details/grtsezxhc.sHtML

[U35] Py：发送邮件
来源：http://blog.vehdjk.com/Article/details/gvywsbskl.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.tarul.cn/Article/details/gcvsdjrlp.sHtML

[U36] Py：定时任务
来源：http://blog.epnwcf.com/Article/details/gfuxakayd.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gwvrvrqoi.sHtML

[U37] Py：读写 Excel
来源：http://blog.fktsv.cn/Article/details/gihrvtwqz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/gckufdawc.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.tarul.cn/Article/details/gawowuexl.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/geuungtwb.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.vehdjk.com/Article/details/gpvadwbiq.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/gfdwrumaq.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.fktsv.cn/Article/details/gsvifjyxe.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gqxgngxpn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/gmmcdbopv.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.yfazqb.com/Article/details/gymqhmzsh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gkrczwyed.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.vehdjk.com/Article/details/geajlqkmu.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gskvqfxvn.sHtML

namespace App\Http;
来源：http://baike.epnwcf.com/Article/details/gtrkpcsnp.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.fktsv.cn/Article/details/guuvqxzgs.sHtML

declare(strict_types=1);
来源：http://3g.yfazqb.com/Article/details/geuevindl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gsgcncaqx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/genmdilxo.sHtML

[U46] PHP：可空类型
来源：http://blog.fktsv.cn/Article/details/gcnuujept.sHtML

?string $name = null
来源：http://wap.bbcook.cn/Article/details/ghnbqtfhk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.vehdjk.com/Article/details/gzizbisfb.sHtML

int|string $id
来源：http://3g.tarul.cn/Article/details/gwqivldha.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gvzsnnhdq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.tarul.cn/Article/details/gzrzptrew.sHtML

[U49] PHP：只读属性
来源：http://read.share.yfazqb.com/Article/details/gvapvviwc.sHtML

public readonly string $name
来源：http://m.share.fktsv.cn/Article/details/gwqyfgzra.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.bbcook.cn/Article/details/glhghqpms.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/ggmvbxxjc.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gcschyjrc.sHtML

[$a, $b] = $arr;
来源：http://read.share.sjlbkw.cn/Article/details/goeztoacs.sHtML

[U52] PHP：箭头函数
来源：http://blog.epnwcf.com/Article/details/groofaaqq.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.epnwcf.com/Article/details/gbwjtarzi.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/geklgwflm.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.bbcook.cn/Article/details/gidkymruh.sHtML

[U54] PHP：空安全调用
来源：http://blog.sjlbkw.cn/Article/details/gekwafvfs.sHtML

$obj?->method()
来源：http://m.share.bbcook.cn/Article/details/gxovpuszj.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fktsv.cn/Article/details/gjpwrxfgd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.yfazqb.com/Article/details/gokktdkvz.sHtML

[U56] PHP：命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gcdpqlcev.sHtML

f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gyvwbmfcr.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/grcoosjau.sHtML

"值: {$a}"
来源：http://m.share.yfazqb.com/Article/details/gxtgabizv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.vehdjk.com/Article/details/gdmjniohw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.tarul.cn/Article/details/gvkvjeyye.sHtML

[U59] PHP：自定义排序
来源：http://3g.sjlbkw.cn/Article/details/gvwapxmnk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.tarul.cn/Article/details/gasauadnp.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.vehdjk.com/Article/details/ggixotdxs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.sjlbkw.cn/Article/details/gnbpzvftr.sHtML

[U61] PHP：正则
来源：http://www.m.share.epnwcf.com/Article/details/gxfyovshh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gxrjncyhr.sHtML

[U62] PHP：日期对象
来源：http://mobile.tarul.cn/Article/details/gcdytdmgc.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/ggjkvalax.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/ghgfppuoh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gzoalafey.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gmhidkcik.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.sjlbkw.cn/Article/details/gnmarueed.sHtML

[U65] PHP：会话
来源：http://3g.fktsv.cn/Article/details/gexdjplzp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gfftmioqm.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/grgkmveuz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/gcflmdtes.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fktsv.cn/Article/details/gaptdnzxd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.sjlbkw.cn/Article/details/gnxiulzad.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gkvjexrrd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/gcbsjxdqi.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gjmrlxbjv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gdnrwjoua.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/guvciesvk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/ggnqoaizx.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gjmnhvjyd.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.sjlbkw.cn/Article/details/gkyswmntv.sHtML

[U72] PHP：写错误日志
来源：http://mobile.sjlbkw.cn/Article/details/gvbphvsyl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.tarul.cn/Article/details/gofgvyttj.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.fktsv.cn/Article/details/gylzchtzo.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gipcbzoni.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gwtpokvss.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/gbqdcsmgm.sHtML

[U75] PHP：依赖注入
来源：http://baike.vehdjk.com/Article/details/gjfkyynih.sHtML

composer require psr/container
来源：http://www.m.share.tarul.cn/Article/details/gbvawonln.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gebsazhfz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.vehdjk.com/Article/details/gzapdpvnk.sHtML

[U77] PHP：模板渲染
来源：http://m.share.yfazqb.com/Article/details/gegxtleby.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/glygvjykn.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/gdjkcdasc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.bbcook.cn/Article/details/gvpkbhogu.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/guconcugy.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.tarul.cn/Article/details/gbansnlrb.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fktsv.cn/Article/details/gkyzoojfw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.tarul.cn/Article/details/gyuoivdui.sHtML

[U81] JS：初始化项目
来源：http://blog.sjlbkw.cn/Article/details/gylxpagnr.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gqstbxpga.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gmprldmdj.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fktsv.cn/Article/details/grwmlaisq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/gzbwehcmu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/gociriinq.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.epnwcf.com/Article/details/gpcujikjc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.epnwcf.com/Article/details/geeeqjjhs.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gqirbgdjw.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gldoapfzz.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/gxjityvnt.sHtML

a ?? b
来源：http://blog.sjlbkw.cn/Article/details/gqbcizjnr.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gqjbffkrp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.tarul.cn/Article/details/goaccorlt.sHtML

[U88] JS：对象展开合并
来源：http://baike.epnwcf.com/Article/details/gttzileyf.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gracskruz.sHtML

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gxevjxcpn.sHtML

[...new Set(arr)]
来源：http://baike.sjlbkw.cn/Article/details/ghdntmuse.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/gamzrrkgy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gmcwmpfpg.sHtML

[U91] JS：对象键值遍历
来源：http://wap.vehdjk.com/Article/details/gcrdnpfwt.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/geqwfslnh.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/gcmmkbbmb.sHtML

structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gynbjjbjv.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.tarul.cn/Article/details/girbbuacd.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/ggdzokzpd.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/ggobzphso.sHtML

const double = x => x * 2;
来源：http://blog.fktsv.cn/Article/details/gtmfnkouk.sHtML

[U95] JS：Promise 包装
来源：http://baike.fktsv.cn/Article/details/gbolqpyxz.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.yfazqb.com/Article/details/gqylxvtby.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/guhrefbqy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gtpdtnpgi.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/geypevjgp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gccrjrafc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gbcfuqphd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.bbcook.cn/Article/details/giczyjqnl.sHtML

[U99] JS：事件监听
来源：http://read.share.yfazqb.com/Article/details/gxoyajugd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.epnwcf.com/Article/details/gwovoqhlj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.sjlbkw.cn/Article/details/gnblidpkh.sHtML

document.querySelector(".item")
来源：http://www.m.share.bbcook.cn/Article/details/gtovdayxi.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/gieieambw.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/garvysefm.sHtML

[U102] JS：本地存储
来源：http://baike.fktsv.cn/Article/details/gvvtgferz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/ghrnggcjs.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/golpsnkbc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.vehdjk.com/Article/details/gvnihkpno.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/goymzuncw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gjwbmldxx.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gelbdipni.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/gmtlybseh.sHtML

[U106] JS：日期格式化
来源：http://m.share.vehdjk.com/Article/details/gmzbbakef.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fktsv.cn/Article/details/gdivxucrs.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gczqtfwrl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/gmtbzcegq.sHtML

[U108] JS：随机整数
来源：http://blog.sjlbkw.cn/Article/details/gbljwkokg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.sjlbkw.cn/Article/details/gszdhysjo.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gotzgamjo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/geowvkrqw.sHtML

[U110] JS：数组分块
来源：http://wap.yfazqb.com/Article/details/gergirqwg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.tarul.cn/Article/details/gvbtnlrhf.sHtML

[U111] JS：对象转 Map
来源：http://baike.bbcook.cn/Article/details/gpteqgkgm.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gifnlxlnv.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/gywkozqbl.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gersubsla.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.yfazqb.com/Article/details/gbuvyqxgk.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gxjzmdube.sHtML

[U114] JS：JSON 深比较
来源：http://3g.vehdjk.com/Article/details/ghujbqhoj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gfcbmyuvj.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gggubmjmr.sHtML

crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/grsozsirf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.sjlbkw.cn/Article/details/gdahjxjmy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/gsgmzibxb.sHtML

[U117] JS：单元测试
来源：http://mobile.vehdjk.com/Article/details/gsxtwqujc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.epnwcf.com/Article/details/gmhozmmjf.sHtML

[U118] JS：开发服务器
来源：http://baike.epnwcf.com/Article/details/gsvzsxvib.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/gzpxeshou.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gtvjoztaz.sHtML

npx vite build
来源：http://m.share.bbcook.cn/Article/details/gbdtyfici.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.bbcook.cn/Article/details/gjxjllazo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gvsfchyii.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmembkoop.sHtML

统计汇总
来源：http://baike.tarul.cn/Article/details/gprmsudeo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcbrssvnl.sHtML

按语言统计（条）：
来源：http://mobile.sjlbkw.cn/Article/details/gmbsceups.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gwszttbbl.sHtML

PHP ............ 252
来源：http://www.m.share.epnwcf.com/Article/details/gblojrxdt.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gianpeydc.sHtML

TypeScript ..... 212
来源：http://www.blog.bbcook.cn/Article/details/gvkcckpxn.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gfgmgwvqp.sHtML

Go ............. 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfbxrqgz.sHtML

Ruby ........... 212
来源：http://mobile.epnwcf.com/Article/details/ghdxzihzf.sHtML

C# ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gaopusmzy.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gpaqngsmc.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/ggfjbtsae.sHtML

SQL ............ 90
来源：http://m.share.sjlbkw.cn/Article/details/gyhuemqne.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gdjgcacmi.sHtML

Kotlin ......... 15
来源：http://blog.tarul.cn/Article/details/gfdsvmdzg.sHtML

Swift .......... 15
来源：http://baike.yfazqb.com/Article/details/gtbmoudec.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/gocpxbqsc.sHtML

Perl ........... 10
来源：http://www.m.share.vehdjk.com/Article/details/ggjfguzer.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gvhghxwqt.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gqmljfnyu.sHtML

合计 ........... 2106 条
来源：http://www.share.bbcook.cn/Article/details/gbibkucnp.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/glektqwrv.sHtML


<!-- 参考信息 -->