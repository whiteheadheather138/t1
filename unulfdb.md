代发 wailian999

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gmjruxgjp.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/goliiguez.sHtML

[T42] Perl：变量类型
来源：http://mobile.yfazqb.com/Article/details/gubhblfik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gfuqaiesg.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/ggdntjssb.sHtML

"值: $a"
来源：http://blog.tarul.cn/Article/details/gxjgibczh.sHtML

[T44] Perl：条件
来源：http://m.share.fktsv.cn/Article/details/gvmeygsfb.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.yfazqb.com/Article/details/glukhvstk.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gaivazyom.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.yfazqb.com/Article/details/gyxufgdyi.sHtML

[T46] Perl：哈希操作
来源：http://mobile.vehdjk.com/Article/details/gjetxlpwv.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.tarul.cn/Article/details/gdkrhpnli.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gnvduvmji.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fktsv.cn/Article/details/gtumhkmfk.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/guejbhzye.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gpqtlfsfx.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/girsadxez.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gbiwrzaei.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/girvypose.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/giivajhcn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.epnwcf.com/Article/details/gfmfduhad.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gspgjwebf.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gyihambll.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gjbwrmdgv.sHtML

val a = 1;  var b = 2
来源：http://blog.yfazqb.com/Article/details/gnihlhqxd.sHtML

[T53] Scala：字符串插值
来源：http://wap.yfazqb.com/Article/details/gfixogund.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gvwluyjzk.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gskwuthpw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gcqxwlyoy.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gxjisrhxa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gizhtndpj.sHtML

[T56] Scala：样例类
来源：http://baike.fktsv.cn/Article/details/ghlnxxcsu.sHtML

case class User(name: String, age: Int)
来源：http://m.share.epnwcf.com/Article/details/gwctblhrc.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/ghaqlbqmy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gzihtswep.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/gfjyulrpl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gtrhfrbhr.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gyhziupsp.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gsatqxdhi.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gquiqjlyl.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gkvvqncxq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghqegujdw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.tarul.cn/Article/details/ggcowvbns.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gzoxsqwcw.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/gvvbxmfzx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gdrxnxlnp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.bbcook.cn/Article/details/gajydweks.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.epnwcf.com/Article/details/gfuqidtlv.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gaqxibqxk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.tarul.cn/Article/details/gbcxpbfay.sHtML

[U04] Py：变量调试打印
来源：http://blog.sjlbkw.cn/Article/details/ghkkvnkoa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.tarul.cn/Article/details/gbewvzghb.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gtvebogwy.sHtML

list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gkepoqyup.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gbedbhcej.sHtML

{**a, **b}
来源：http://3g.tarul.cn/Article/details/ghkytqfxz.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/gpgxvxqsm.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/ggsongfby.sHtML

[U08] Py：展平二维列表
来源：http://www.share.epnwcf.com/Article/details/gqcnzlnsc.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.fktsv.cn/Article/details/gnhhijlow.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gsfbumrtt.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkseympl.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.bbcook.cn/Article/details/ggrtqkggr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/gspnotaqp.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gbirihder.sHtML

(x * 2 for x in arr)
来源：http://read.share.fktsv.cn/Article/details/gebtmemsd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.fktsv.cn/Article/details/gwzxjlsfa.sHtML

Counter(arr).most_common(3)
来源：http://blog.vehdjk.com/Article/details/gvorjkvvj.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/grfpfejhp.sHtML

deque(maxlen=10)
来源：http://read.share.bbcook.cn/Article/details/gyrsltkar.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.vehdjk.com/Article/details/gflbcjhqs.sHtML

defaultdict(list)
来源：http://m.share.vehdjk.com/Article/details/geeliiksj.sHtML

[U15] Py：高精度计时
来源：http://3g.yfazqb.com/Article/details/gelefycfj.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/gcrttxqjt.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.epnwcf.com/Article/details/grahwtfch.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.epnwcf.com/Article/details/gzxtycdkq.sHtML

[U17] Py：初始化日志
来源：http://baike.bbcook.cn/Article/details/goocwscky.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.tarul.cn/Article/details/govtocblj.sHtML

[U18] Py：预编译正则
来源：http://m.share.fktsv.cn/Article/details/gbakhunte.sHtML

pat = re.compile(r"\d+")
来源：http://baike.epnwcf.com/Article/details/gzhkuwbph.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/grnwtjnmq.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.vehdjk.com/Article/details/gauyuiotd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.epnwcf.com/Article/details/gbygujsvh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gevwcaybh.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.yfazqb.com/Article/details/gplnsyqgr.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gxjtvyflg.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gwljjxrac.sHtML

list(zip(*m))
来源：http://read.share.vehdjk.com/Article/details/gwoxjqjwk.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.yfazqb.com/Article/details/gmvzvifzt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.sjlbkw.cn/Article/details/goqsjdzqb.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gqwiahjlr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mobile.vehdjk.com/Article/details/gbsdwqymr.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.sjlbkw.cn/Article/details/gnsznztdk.sHtML

csv.DictReader(f)
来源：http://m.share.sjlbkw.cn/Article/details/gnnmpsxeg.sHtML

[U26] Py：并发下载
来源：http://read.share.sjlbkw.cn/Article/details/gsmdiwwuz.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.m.share.epnwcf.com/Article/details/gfvaxozoj.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.bbcook.cn/Article/details/giunmoxyt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.tarul.cn/Article/details/garmuswjd.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gxfolingv.sHtML

UserId = int
来源：http://www.share.yfazqb.com/Article/details/gvosokwxu.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/grxvlfycy.sHtML

@property 与 @x.setter 配合
来源：http://baike.yfazqb.com/Article/details/gjulazmjf.sHtML

[U30] Py：数据类
来源：http://blog.tarul.cn/Article/details/gidotgcsu.sHtML

@dataclass(slots=True)
来源：http://m.share.vehdjk.com/Article/details/glcaascwe.sHtML

[U31] Py：单测
来源：http://baike.epnwcf.com/Article/details/gnphbndqs.sHtML

python -m pytest -q
来源：http://www.share.vehdjk.com/Article/details/gacysrjht.sHtML

[U32] Py：代码格式化
来源：http://mobile.tarul.cn/Article/details/ghwunmwtj.sHtML

ruff format . && ruff check --fix .
来源：http://blog.yfazqb.com/Article/details/gobhklhcu.sHtML

[U33] Py：打包发布
来源：http://m.share.tarul.cn/Article/details/ggckcojzo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.tarul.cn/Article/details/gqxgbvwvh.sHtML

[U34] Py：判断编码
来源：http://baike.epnwcf.com/Article/details/gknmlksyw.sHtML

chardet.detect(raw)
来源：http://www.blog.bbcook.cn/Article/details/ggvcesejg.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/ggvticptq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.sjlbkw.cn/Article/details/gxnvtkkrx.sHtML

[U36] Py：定时任务
来源：http://3g.sjlbkw.cn/Article/details/gsvfzcvqk.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.yfazqb.com/Article/details/gfhwwulke.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/guscclker.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/gpqajhaya.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.tarul.cn/Article/details/gnqrmyeir.sHtML

Path(__file__).resolve().parent
来源：http://3g.bbcook.cn/Article/details/goemxhpew.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.yfazqb.com/Article/details/gswrazycc.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/gdkuzkslj.sHtML

[U40] Py：打印到标准错误
来源：http://blog.sjlbkw.cn/Article/details/gfhlmjokg.sHtML

print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gpddklhxc.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpgfviga.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.yfazqb.com/Article/details/ghpzihdev.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.epnwcf.com/Article/details/ggxkbiqui.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/gzdbkufuo.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.sjlbkw.cn/Article/details/gfmxprifb.sHtML

namespace App\Http;
来源：http://mobile.sjlbkw.cn/Article/details/gujeqiwaf.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gofqcrglb.sHtML

declare(strict_types=1);
来源：http://wap.sjlbkw.cn/Article/details/gyveaeisg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/glllynciu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gvrxjytqu.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/ggfpnwnps.sHtML

?string $name = null
来源：http://mobile.fktsv.cn/Article/details/gicdchjmv.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/ggkxesdum.sHtML

int|string $id
来源：http://wap.sjlbkw.cn/Article/details/grhmueguo.sHtML

[U48] PHP：纯枚举
来源：http://read.share.epnwcf.com/Article/details/gazmppnkd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/galjourpl.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gjksscthm.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/geqilecme.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/gyuojyvlz.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gwavnxjji.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.yfazqb.com/Article/details/gohqdjdsj.sHtML

[$a, $b] = $arr;
来源：http://m.share.fktsv.cn/Article/details/gkvrqshyf.sHtML

[U52] PHP：箭头函数
来源：http://mobile.sjlbkw.cn/Article/details/gjkfbcieu.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gyampideg.sHtML

[U53] PHP：空合并运算符
来源：http://wap.epnwcf.com/Article/details/gyxweuhdw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/govpiqenb.sHtML

[U54] PHP：空安全调用
来源：http://baike.tarul.cn/Article/details/gqtdgoefj.sHtML

$obj?->method()
来源：http://mobile.yfazqb.com/Article/details/gsmrfdqdq.sHtML

[U55] PHP：match 表达式
来源：http://3g.sjlbkw.cn/Article/details/glujfcefx.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/gwbinhgpf.sHtML

[U56] PHP：命名参数
来源：http://baike.fktsv.cn/Article/details/gqschewjl.sHtML

f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gevqquvyo.sHtML

[U57] PHP：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gbunudcja.sHtML

"值: {$a}"
来源：http://3g.fktsv.cn/Article/details/gbtxnkkgn.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/geddipota.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.tarul.cn/Article/details/gagiynwkf.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gavwukftd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/glrzzntvv.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.tarul.cn/Article/details/gpjezofkp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.vehdjk.com/Article/details/gmvjpzmlb.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gxaehwjqc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/gzjvgycpk.sHtML

[U62] PHP：日期对象
来源：http://m.share.epnwcf.com/Article/details/ghbdkpshb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.tarul.cn/Article/details/gbexyndhg.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/gfjrtxljo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.epnwcf.com/Article/details/gudusznvr.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.fktsv.cn/Article/details/glrigwbkx.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.tarul.cn/Article/details/gwzlwsvyn.sHtML

[U65] PHP：会话
来源：http://blog.sjlbkw.cn/Article/details/ggdtprwlv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gmshrzulm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.sjlbkw.cn/Article/details/gwxfrqmdn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.epnwcf.com/Article/details/gaeyvhwhg.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.bbcook.cn/Article/details/ghceppjkm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gudnrysie.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fktsv.cn/Article/details/gvwkwespm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.yfazqb.com/Article/details/gruinprqe.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gpirdljom.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gjnqpucmd.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gxaofbufn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqmdvlhz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.sjlbkw.cn/Article/details/ghwbvcfbr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/goyvjavnh.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.sjlbkw.cn/Article/details/gzxojjese.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/grymrwiyv.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.yfazqb.com/Article/details/gevhimuod.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.bbcook.cn/Article/details/ghofugzlg.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.tarul.cn/Article/details/gfebbnhoa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gtgftzewn.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gqeprkehw.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/giyuhufev.sHtML

[U76] PHP：简单路由
来源：http://m.share.epnwcf.com/Article/details/gdzkpcmcy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.sjlbkw.cn/Article/details/govnuhhcp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.vehdjk.com/Article/details/gnkqwhjnq.sHtML

composer require twig/twig
来源：http://wap.sjlbkw.cn/Article/details/gmanzwhlw.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gfrvqevdl.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.tarul.cn/Article/details/gdaqwwvvv.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/gsldbercx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fktsv.cn/Article/details/guxihhese.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/gqusqerfa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.tarul.cn/Article/details/gxbyilnxs.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.tarul.cn/Article/details/gcpimvnrp.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gdogdtdho.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/ggiypytle.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/glqgdcida.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.tarul.cn/Article/details/gzrzzlgsx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gnfszdrlh.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.vehdjk.com/Article/details/gcebzagpa.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.bbcook.cn/Article/details/grayalcwc.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gkshenpdm.sHtML

a?.b?.c
来源：http://www.share.epnwcf.com/Article/details/gklygcdtj.sHtML

[U86] JS：空值合并
来源：http://mobile.epnwcf.com/Article/details/gqqkpdoev.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gpbgpcmzp.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gxokfhooq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fktsv.cn/Article/details/gxlktrhnk.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/gzhjfuwbn.sHtML

{ ...a, ...b }
来源：http://blog.yfazqb.com/Article/details/gvpvemgbg.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gedlvdxdm.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/guxwsqtpv.sHtML

[U90] JS：数字数组排序
来源：http://read.share.bbcook.cn/Article/details/gvqkkwyzt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gvtdoosrs.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/golmrrsif.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/ghougigfc.sHtML

[U92] JS：深拷贝
来源：http://read.share.vehdjk.com/Article/details/ghfodgrel.sHtML

structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gmodofedf.sHtML

[U93] JS：模板字符串
来源：http://m.share.fktsv.cn/Article/details/ggkvahsmk.sHtML

`共 ${n} 条`
来源：http://mobile.fktsv.cn/Article/details/gbotdtqho.sHtML

[U94] JS：箭头函数
来源：http://3g.vehdjk.com/Article/details/gmhplsjit.sHtML

const double = x => x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gfjafmhhy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.tarul.cn/Article/details/gismndxhd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.vehdjk.com/Article/details/gxkvxelsk.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.sjlbkw.cn/Article/details/ggxpqykjx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gbhgdrqmd.sHtML

[U97] JS：并发请求
来源：http://baike.tarul.cn/Article/details/geuppgndu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gghzkyshy.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gpegfezjn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.sjlbkw.cn/Article/details/gcxtortds.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/ghvkkcthy.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gwnktbvrf.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gxgazeuil.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gzsdfnski.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gnfbovxme.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/gvdivipdy.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/ghkmoizzb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.epnwcf.com/Article/details/gbelxanon.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/gocaortcw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fktsv.cn/Article/details/gcgaxootr.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/gposerlpd.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/glkfwixvf.sHtML

[U105] JS：节流
来源：http://blog.epnwcf.com/Article/details/gtoikogzy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.vehdjk.com/Article/details/gonpknwqe.sHtML

[U106] JS：日期格式化
来源：http://www.share.tarul.cn/Article/details/gdnglfrep.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/grzgtfnnf.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gejuiqxsj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gjvycjcer.sHtML

[U108] JS：随机整数
来源：http://m.share.yfazqb.com/Article/details/gidkbjdxd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gkuxcddmb.sHtML

[U109] JS：数组分组
来源：http://baike.epnwcf.com/Article/details/gswtxohqt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/ghbpjcium.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gpqkhzqoi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gtvjkidqd.sHtML

[U111] JS：对象转 Map
来源：http://3g.bbcook.cn/Article/details/gatdgcccq.sHtML

new Map(Object.entries(obj))
来源：http://3g.tarul.cn/Article/details/gwrnynvjr.sHtML

[U112] JS：字符串补位
来源：http://blog.bbcook.cn/Article/details/gnihlmrck.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gnrzddhak.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/gteqcouum.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gnolrvxne.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.sjlbkw.cn/Article/details/gnefzjwqr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gczevwpjr.sHtML

[U115] JS：生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gcolgxhpr.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gofbkgdix.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gzkhugdta.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.epnwcf.com/Article/details/gufujhjcr.sHtML

[U117] JS：单元测试
来源：http://blog.tarul.cn/Article/details/gzocimtyi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.vehdjk.com/Article/details/gsdmydalk.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fktsv.cn/Article/details/gbtrlxjbb.sHtML

npm i -D vite;  npx vite
来源：http://m.share.yfazqb.com/Article/details/ghnmjedho.sHtML

[U119] JS：生产构建
来源：http://read.share.epnwcf.com/Article/details/gtslywefo.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gzqyaxwvw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.vehdjk.com/Article/details/gvarlycfc.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.yfazqb.com/Article/details/gbsvshslc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghaaatbui.sHtML

统计汇总
来源：http://3g.sjlbkw.cn/Article/details/gmmebeqga.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glepyuvxw.sHtML

按语言统计（条）：
来源：http://wap.fktsv.cn/Article/details/gcuyljwyh.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gshwdedbo.sHtML

PHP ............ 252
来源：http://baike.bbcook.cn/Article/details/gcgkcgsbj.sHtML

JavaScript ..... 252
来源：http://www.m.share.tarul.cn/Article/details/gzmmtqufc.sHtML

TypeScript ..... 212
来源：http://wap.fktsv.cn/Article/details/giyjulgwj.sHtML

Java ........... 212
来源：http://read.share.epnwcf.com/Article/details/grphyesdz.sHtML

Go ............. 212
来源：http://m.share.epnwcf.com/Article/details/gmuudwioq.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gvvzyopco.sHtML

C# ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gpvgthxlv.sHtML

C .............. 30
来源：http://mobile.tarul.cn/Article/details/ghpylixal.sHtML

C++ ............ 30
来源：http://www.m.share.yfazqb.com/Article/details/gwuvldfwi.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/gntylfgmo.sHtML

Bash ........... 80
来源：http://blog.bbcook.cn/Article/details/gdzolshpy.sHtML


<!-- 参考信息 -->