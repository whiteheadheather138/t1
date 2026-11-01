代发 wailian999

[T43] Perl：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gdztitknw.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gqcwpwkuj.sHtML

[T44] Perl：条件
来源：http://m.share.sjlbkw.cn/Article/details/gmmtemani.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gbslkhtxu.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gsyrqiuuf.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.tarul.cn/Article/details/gdxcowfij.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/goddzpqaa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/grgltpsgl.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gsuchjooo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gfkzqzgqq.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/ghiocmfge.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gvlydkucl.sHtML

[T49] Perl：函数
来源：http://blog.tarul.cn/Article/details/grjqpjhwv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gggdzubbg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.epnwcf.com/Article/details/glgstrlop.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gcfimxxpc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.tarul.cn/Article/details/gkluzossh.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/ghkknywvw.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/growrqauq.sHtML

[T52] Scala：变量
来源：http://read.share.vehdjk.com/Article/details/gywlolasc.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gahdpzzmh.sHtML

[T53] Scala：字符串插值
来源：http://3g.epnwcf.com/Article/details/gajcmqzoq.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gcjkesgwd.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gsnnztbpr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.tarul.cn/Article/details/gidylsngd.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/gaxspjnpo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/gnmrrcdfd.sHtML

[T56] Scala：样例类
来源：http://www.m.share.epnwcf.com/Article/details/gtholsxfm.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gudksdwgu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdnsvjxa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fktsv.cn/Article/details/gdfvarjir.sHtML

[T58] Scala：函数定义
来源：http://mobile.fktsv.cn/Article/details/gvtexjfxh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/gglwoxffj.sHtML

[T59] Scala：循环
来源：http://m.share.sjlbkw.cn/Article/details/gjdngziji.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gseffmdkj.sHtML

[T60] Scala：折叠
来源：http://wap.epnwcf.com/Article/details/gcbbrquso.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.epnwcf.com/Article/details/gaajyejvf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfvygdjvk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/guitygfuf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gejxlfaqh.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.yfazqb.com/Article/details/gybltxkmf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gcuisgpzj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.yfazqb.com/Article/details/gahiremnf.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/grmtaceuu.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.epnwcf.com/Article/details/gjswdkrmz.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/gmdvgetpx.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/ghwoajiqk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gkjuzqipk.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.vehdjk.com/Article/details/gkrivpgyx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gkycocghw.sHtML

[U06] Py：合并两个字典
来源：http://mobile.yfazqb.com/Article/details/gjldxhcaa.sHtML

{**a, **b}
来源：http://blog.tarul.cn/Article/details/ginenbuhr.sHtML

[U07] Py：反转字典键值
来源：http://mobile.epnwcf.com/Article/details/gskbagbrp.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gcarymqxi.sHtML

[U08] Py：展平二维列表
来源：http://blog.fktsv.cn/Article/details/ggcjtkdpt.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gryqrtdje.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/ghmtidxwo.sHtML

max(d, key=d.get)
来源：http://www.blog.vehdjk.com/Article/details/gwtfacshs.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.epnwcf.com/Article/details/gyagkbfyl.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.epnwcf.com/Article/details/gkrbghgnv.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/ggxmorsbg.sHtML

(x * 2 for x in arr)
来源：http://mobile.yfazqb.com/Article/details/gpiokfmaw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.epnwcf.com/Article/details/ggvgvgnht.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gzwbkxlbz.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.bbcook.cn/Article/details/gwwqrgpch.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gszbwgbnh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.vehdjk.com/Article/details/ghbcqagcf.sHtML

defaultdict(list)
来源：http://www.blog.bbcook.cn/Article/details/gqpuryzml.sHtML

[U15] Py：高精度计时
来源：http://read.share.epnwcf.com/Article/details/gevuubfll.sHtML

t = time.perf_counter()
来源：http://m.share.fktsv.cn/Article/details/grkapotda.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/gdtnlwqzx.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.tarul.cn/Article/details/gijsiupzf.sHtML

[U17] Py：初始化日志
来源：http://blog.epnwcf.com/Article/details/geqtiaucr.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gslihlyma.sHtML

[U18] Py：预编译正则
来源：http://m.share.yfazqb.com/Article/details/gigiglcoi.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.bbcook.cn/Article/details/gzbqklfzs.sHtML

[U19] Py：正则替换带回调
来源：http://wap.epnwcf.com/Article/details/ghdcjejoz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.yfazqb.com/Article/details/gsdfhktpm.sHtML

[U20] Py：缓存函数结果
来源：http://3g.fktsv.cn/Article/details/gngbrbori.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.fktsv.cn/Article/details/gtsikpgdt.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.sjlbkw.cn/Article/details/gookscfto.sHtML

@contextlib.contextmanager
来源：http://www.share.vehdjk.com/Article/details/ggyhjgwzl.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.epnwcf.com/Article/details/gsfndhwau.sHtML

list(zip(*m))
来源：http://baike.yfazqb.com/Article/details/gjxojopda.sHtML

[U23] Py：分块读取大文件
来源：http://3g.epnwcf.com/Article/details/gkzvmhijw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/grfjkjeph.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/gjlbhcwgw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.tarul.cn/Article/details/glkovzlfu.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.vehdjk.com/Article/details/gkisxfvhq.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/gdnetqsut.sHtML

[U26] Py：并发下载
来源：http://read.share.epnwcf.com/Article/details/gvgdcffyq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/ghmocrqpy.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.tarul.cn/Article/details/gnhkxcysw.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/gxlznerqx.sHtML

[U28] Py：类型别名
来源：http://www.blog.vehdjk.com/Article/details/guctpaebq.sHtML

UserId = int
来源：http://www.share.fktsv.cn/Article/details/gtflwxrfh.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gprzknidc.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.bbcook.cn/Article/details/gsnykngyr.sHtML

[U30] Py：数据类
来源：http://www.blog.yfazqb.com/Article/details/gkvmkzjro.sHtML

@dataclass(slots=True)
来源：http://blog.epnwcf.com/Article/details/gcnrjidny.sHtML

[U31] Py：单测
来源：http://blog.sjlbkw.cn/Article/details/geqklsxyx.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gyjkbwldn.sHtML

[U32] Py：代码格式化
来源：http://wap.tarul.cn/Article/details/gzdtdcmhr.sHtML

ruff format . && ruff check --fix .
来源：http://wap.sjlbkw.cn/Article/details/gsbjekbrr.sHtML

[U33] Py：打包发布
来源：http://blog.tarul.cn/Article/details/gxrhelsuo.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gcnyvhzge.sHtML

[U34] Py：判断编码
来源：http://m.share.tarul.cn/Article/details/gnqkvsqyd.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gpjwphxct.sHtML

[U35] Py：发送邮件
来源：http://www.blog.yfazqb.com/Article/details/gsprtuukt.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gnhqbesym.sHtML

[U36] Py：定时任务
来源：http://wap.sjlbkw.cn/Article/details/gkngpmbbe.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gibfnwwuy.sHtML

[U37] Py：读写 Excel
来源：http://www.share.vehdjk.com/Article/details/gwkbwokvf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.vehdjk.com/Article/details/grscwarfn.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.fktsv.cn/Article/details/gygoujyuu.sHtML

Path(__file__).resolve().parent
来源：http://www.share.epnwcf.com/Article/details/gfksefcxa.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.epnwcf.com/Article/details/gubtqompn.sHtML

sys.stdout.isatty()
来源：http://blog.yfazqb.com/Article/details/gfdxdofpl.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/gsemhlgbf.sHtML

print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gjbwcrxqs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://3g.epnwcf.com/Article/details/gakcklixm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.sjlbkw.cn/Article/details/gyglharwy.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.sjlbkw.cn/Article/details/gyjoiwssk.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.sjlbkw.cn/Article/details/gykbimony.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gyopaduvy.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gpsvjsfco.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gfbgtrvpa.sHtML

declare(strict_types=1);
来源：http://www.blog.sjlbkw.cn/Article/details/gwbmruseb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.vehdjk.com/Article/details/gprusqngy.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gpcqvcuzr.sHtML

[U46] PHP：可空类型
来源：http://m.share.vehdjk.com/Article/details/gtvmewukb.sHtML

?string $name = null
来源：http://wap.sjlbkw.cn/Article/details/gsndjljdf.sHtML

[U47] PHP：联合类型
来源：http://wap.yfazqb.com/Article/details/gymilbmfp.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gobrwmjnv.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.tarul.cn/Article/details/giepzmtai.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gioicawdg.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/gubrlmbdh.sHtML

public readonly string $name
来源：http://www.share.bbcook.cn/Article/details/gugrobsaq.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.bbcook.cn/Article/details/gpwrqznjh.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gzqfonupx.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/ggqtiqdfi.sHtML

[$a, $b] = $arr;
来源：http://mobile.sjlbkw.cn/Article/details/gbekoqrld.sHtML

[U52] PHP：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gzrldyvbs.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gttfkkapv.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.sjlbkw.cn/Article/details/gyhmizhaf.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.tarul.cn/Article/details/ghrswbwgu.sHtML

[U54] PHP：空安全调用
来源：http://3g.tarul.cn/Article/details/gybxznwve.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/gyotdzxhn.sHtML

[U55] PHP：match 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gobjjbkmr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gkglxvbru.sHtML

[U56] PHP：命名参数
来源：http://3g.fktsv.cn/Article/details/gnfeigokf.sHtML

f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gzimsykuj.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gvxsgvikg.sHtML

"值: {$a}"
来源：http://blog.fktsv.cn/Article/details/ggeypzpwm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.yfazqb.com/Article/details/grmiqkwvj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gqkozohzm.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gmwzsqkoz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gioyqprsh.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.bbcook.cn/Article/details/grztqfmpi.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gpunbzduq.sHtML

[U61] PHP：正则
来源：http://read.share.fktsv.cn/Article/details/gqwzlourt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/gyzxzcbhm.sHtML

[U62] PHP：日期对象
来源：http://wap.epnwcf.com/Article/details/gvbkjmoom.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/gjjgqywvn.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/golbwnhtx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.epnwcf.com/Article/details/gkwubwqan.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/glduufzgn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.sjlbkw.cn/Article/details/gcghlvaos.sHtML

[U65] PHP：会话
来源：http://read.share.fktsv.cn/Article/details/gbzdezhlj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/ggxoaheet.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gexlkjedu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.epnwcf.com/Article/details/gvjoumcev.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/glaizkeeu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gwvkzutnw.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.tarul.cn/Article/details/gcphnnern.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gwmqnkyds.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gjqlfveol.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gqstpwjsj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gherfzyru.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.yfazqb.com/Article/details/ghapbzibm.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/gngmpokos.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gjqaugypm.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/gcowkahyi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.epnwcf.com/Article/details/gtinzoupg.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/gsrsdtkwf.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.yfazqb.com/Article/details/gztkklneq.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gldjkuyim.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.vehdjk.com/Article/details/gudaqhvxp.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/gmijyyyzx.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/gprjfbvhi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gprukzssh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/gicxezjhf.sHtML

[U77] PHP：模板渲染
来源：http://read.share.bbcook.cn/Article/details/gcynlfeov.sHtML

composer require twig/twig
来源：http://mobile.yfazqb.com/Article/details/gfmlduahd.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gjfngoikb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gdnmosjdj.sHtML

[U79] PHP：静态分析
来源：http://m.share.tarul.cn/Article/details/gskqambvz.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/goypbgddt.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.epnwcf.com/Article/details/gdaxghldl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gengdvfra.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gtcvsmhbr.sHtML

npm init -y;  npm i express
来源：http://baike.sjlbkw.cn/Article/details/gcbnoakhl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.vehdjk.com/Article/details/grsstiuww.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.sjlbkw.cn/Article/details/gskgqxqum.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.bbcook.cn/Article/details/ggfoodhxr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/gfixjnqdm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.epnwcf.com/Article/details/gujibsylu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fktsv.cn/Article/details/gooieqoef.sHtML

[U85] JS：可选链
来源：http://www.share.vehdjk.com/Article/details/glerabgvu.sHtML

a?.b?.c
来源：http://www.m.share.yfazqb.com/Article/details/gigttyayc.sHtML

[U86] JS：空值合并
来源：http://m.share.vehdjk.com/Article/details/gvzpajtwz.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/gurzpgmzo.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/gmxwhtyay.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gdxwiobio.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.tarul.cn/Article/details/gthczfhfl.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gzslcfavl.sHtML

[U89] JS：数组去重
来源：http://m.share.fktsv.cn/Article/details/gvpkmdfcn.sHtML

[...new Set(arr)]
来源：http://read.share.yfazqb.com/Article/details/grkicennf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gulpkqraa.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gqoorrxdh.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gbiuzobtr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.bbcook.cn/Article/details/ghxzrznxb.sHtML

[U92] JS：深拷贝
来源：http://wap.sjlbkw.cn/Article/details/gevplhmro.sHtML

structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gubhxwjxl.sHtML

[U93] JS：模板字符串
来源：http://mobile.bbcook.cn/Article/details/gcsfiluhf.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gtyfedwyv.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gwzaokaex.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gobwwvmfq.sHtML

[U95] JS：Promise 包装
来源：http://read.share.epnwcf.com/Article/details/gsgrxrfwa.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fktsv.cn/Article/details/gwommwrgl.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gpdjhgcdq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gtmvldswa.sHtML

[U97] JS：并发请求
来源：http://m.share.tarul.cn/Article/details/gihtsqyvq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gejgplpav.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.vehdjk.com/Article/details/gqpmviwtu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.epnwcf.com/Article/details/gwmrltkuj.sHtML

[U99] JS：事件监听
来源：http://blog.fktsv.cn/Article/details/glxzwsllm.sHtML

el.addEventListener("click", e => {})
来源：http://blog.vehdjk.com/Article/details/gxtmumxmv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.epnwcf.com/Article/details/gwwvzdegb.sHtML

document.querySelector(".item")
来源：http://blog.vehdjk.com/Article/details/gexwzdxam.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/ggfyunrtn.sHtML

el.classList.toggle("active")
来源：http://read.share.sjlbkw.cn/Article/details/glsszhtik.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/gsqyaigih.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/guxdbhhqa.sHtML

[U103] JS：定时器
来源：http://www.share.fktsv.cn/Article/details/gkqptabhb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.sjlbkw.cn/Article/details/gkwzysdia.sHtML

[U104] JS：防抖
来源：http://wap.vehdjk.com/Article/details/gzagnvotl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/guahimiqa.sHtML

[U105] JS：节流
来源：http://read.share.bbcook.cn/Article/details/gagminzee.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.bbcook.cn/Article/details/gxrdmvlcx.sHtML

[U106] JS：日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gercxivcv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/gmpwxvjqv.sHtML

[U107] JS：数字千分位
来源：http://3g.tarul.cn/Article/details/gzbsijmfz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gzokmjmnz.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/gqhdbtaqy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.tarul.cn/Article/details/gjjqdskwz.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/geugkmwbz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gqnvsiiqg.sHtML

[U110] JS：数组分块
来源：http://read.share.vehdjk.com/Article/details/gnhignvzv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.sjlbkw.cn/Article/details/gkmnicwmz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/gzetuneng.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.yfazqb.com/Article/details/gytagmkzv.sHtML

[U112] JS：字符串补位
来源：http://blog.sjlbkw.cn/Article/details/gptftujev.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gthkndfzl.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gfztwhgmd.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gwbrtwtwr.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/glzucshts.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gosmsbsyw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.vehdjk.com/Article/details/grqlgwjtd.sHtML

crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gwilchsqy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/gexbqduuw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/gstxpgxvo.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gjspizwwm.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.vehdjk.com/Article/details/gnqlugynm.sHtML

[U118] JS：开发服务器
来源：http://m.share.tarul.cn/Article/details/gjitzeogm.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/gnkagaypc.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gbipagvqc.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gngubnsey.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.sjlbkw.cn/Article/details/grjkglmcu.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.vehdjk.com/Article/details/gvjlenoca.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnpyyvjab.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gxmrbudyo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfpnlgquw.sHtML

按语言统计（条）：
来源：http://mobile.tarul.cn/Article/details/gbtrzmupm.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gbqytgsvi.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gagjzvpkw.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/guuygrbzn.sHtML

TypeScript ..... 212
来源：http://read.share.yfazqb.com/Article/details/gwzhnkddp.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gcqdndcqy.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gbpslsbxx.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gpnbbubxc.sHtML

C# ............. 212
来源：http://baike.vehdjk.com/Article/details/ggvvgrnwv.sHtML

C .............. 30
来源：http://www.m.share.sjlbkw.cn/Article/details/grhjvyunl.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gptbonmbs.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gcxvmcmgi.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gulmeplqw.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gkazsyvmx.sHtML

Swift .......... 15
来源：http://wap.sjlbkw.cn/Article/details/gyyawkasp.sHtML

Lua ............ 10
来源：http://m.share.fktsv.cn/Article/details/geotgongl.sHtML

Perl ........... 10
来源：http://www.m.share.vehdjk.com/Article/details/gcqbijxyf.sHtML


<!-- 参考信息 -->