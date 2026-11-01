代发 wailian999

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gjooibhuc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gabveqaru.sHtML

[T48] Perl：正则替换
来源：http://baike.vehdjk.com/Article/details/gnwysrkko.sHtML

$s =~ s/old/new/g;
来源：http://read.share.vehdjk.com/Article/details/gxhsrbtcs.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gnwmzkuhk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gsbixvnxp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gdxcjhilb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gczlighgl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.yfazqb.com/Article/details/ghwjwfmmh.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gmbgohrld.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/ghctsnqvt.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/grhzftyrv.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gkdmvkdzd.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gudisvkuo.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gcgwvhecl.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gvaylqics.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gbrcnipir.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gbflweupz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gadiqwtdg.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/gsrndxfnv.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gdlchvqiv.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gjcqtamos.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gvrjwsyqq.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gejpxmrst.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/gtsznqiro.sHtML

[T59] Scala：循环
来源：http://read.share.epnwcf.com/Article/details/gbslrfomn.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gknvarkrg.sHtML

[T60] Scala：折叠
来源：http://www.share.epnwcf.com/Article/details/gmrqhpevo.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.sjlbkw.cn/Article/details/gskjulrbe.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoumstgu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gmvccrkjp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gyspontsy.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gwjuduytp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gkfslegig.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gsnikditu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.tarul.cn/Article/details/gezdrvqap.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.bbcook.cn/Article/details/ggvnowjsh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.fktsv.cn/Article/details/gdfljhlvr.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gpyeowufe.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gtoutsvdm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.yfazqb.com/Article/details/gbxdtfnmk.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/guevroyud.sHtML

[U06] Py：合并两个字典
来源：http://read.share.sjlbkw.cn/Article/details/gkydhtepi.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gcwgaxpva.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/gqvgqvgqo.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gedoxetwq.sHtML

[U08] Py：展平二维列表
来源：http://read.share.bbcook.cn/Article/details/gmkqpvuow.sHtML

[y for x in nested for y in x]
来源：http://blog.tarul.cn/Article/details/gigavpjyx.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/gtgvcftup.sHtML

max(d, key=d.get)
来源：http://3g.vehdjk.com/Article/details/gawzlsurc.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gbrtmyxnx.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.yfazqb.com/Article/details/gfdtyewgz.sHtML

[U11] Py：生成器表达式
来源：http://wap.yfazqb.com/Article/details/gmgceqdkf.sHtML

(x * 2 for x in arr)
来源：http://mobile.vehdjk.com/Article/details/gxpflmxwu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.sjlbkw.cn/Article/details/gzhsuncjd.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.yfazqb.com/Article/details/guwpuraai.sHtML

[U13] Py：固定长度队列
来源：http://baike.vehdjk.com/Article/details/glgpauxpe.sHtML

deque(maxlen=10)
来源：http://blog.yfazqb.com/Article/details/gqccddiey.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.sjlbkw.cn/Article/details/gfeewhqst.sHtML

defaultdict(list)
来源：http://www.share.sjlbkw.cn/Article/details/gjfhrnjau.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/ghadovnlr.sHtML

t = time.perf_counter()
来源：http://mobile.tarul.cn/Article/details/gwtrophdc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.epnwcf.com/Article/details/gwonhwdug.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.yfazqb.com/Article/details/ghitmeadj.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gzttctjij.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.sjlbkw.cn/Article/details/gahzqvvyu.sHtML

[U18] Py：预编译正则
来源：http://wap.yfazqb.com/Article/details/gmtrhqyzb.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gonuhnkmp.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gqgyoaclb.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaxiqosd.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.vehdjk.com/Article/details/glwpofdjk.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.sjlbkw.cn/Article/details/gdxazvhjw.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.vehdjk.com/Article/details/ginryvgrg.sHtML

@contextlib.contextmanager
来源：http://m.share.epnwcf.com/Article/details/grcppkwto.sHtML

[U22] Py：矩阵转置
来源：http://read.share.vehdjk.com/Article/details/ghjgcivtd.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/gphebiund.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/geqrpgxjf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/gheqgmnpm.sHtML

[U24] Py：路径操作
来源：http://mobile.fktsv.cn/Article/details/geetjqomw.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gnemsszcu.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhkpuetd.sHtML

csv.DictReader(f)
来源：http://mobile.epnwcf.com/Article/details/glqhjcnpy.sHtML

[U26] Py：并发下载
来源：http://www.share.vehdjk.com/Article/details/gpohsvpim.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/gzfqboikz.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gzesutehv.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.yfazqb.com/Article/details/gkrysfaqe.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gcntqjnsk.sHtML

UserId = int
来源：http://www.blog.vehdjk.com/Article/details/gxwlnuzyl.sHtML

[U29] Py：属性校验
来源：http://baike.vehdjk.com/Article/details/gspbtfjnw.sHtML

@property 与 @x.setter 配合
来源：http://3g.vehdjk.com/Article/details/gpthtjzns.sHtML

[U30] Py：数据类
来源：http://read.share.epnwcf.com/Article/details/gxopuhtnn.sHtML

@dataclass(slots=True)
来源：http://m.share.fktsv.cn/Article/details/gwmxptiam.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gogygclpq.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gmuyebqka.sHtML

[U32] Py：代码格式化
来源：http://3g.yfazqb.com/Article/details/gmyqwfegl.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.fktsv.cn/Article/details/gejngvmbf.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gseitybsa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.yfazqb.com/Article/details/gfvbviubp.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/gauorxdnk.sHtML

chardet.detect(raw)
来源：http://blog.yfazqb.com/Article/details/guwqqjxng.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/gsbzdzwys.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gktdfwutb.sHtML

[U36] Py：定时任务
来源：http://baike.sjlbkw.cn/Article/details/gkhrpwrlo.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.fktsv.cn/Article/details/gttfurofo.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gtgnuowdd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/gbnealjbq.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.vehdjk.com/Article/details/geipqeyok.sHtML

Path(__file__).resolve().parent
来源：http://blog.vehdjk.com/Article/details/govfiweig.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.m.share.tarul.cn/Article/details/gwdhbxgcm.sHtML

sys.stdout.isatty()
来源：http://wap.epnwcf.com/Article/details/gejbeqgfg.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/gogogwmui.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/goyeyekxj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.vehdjk.com/Article/details/gtdtwdyja.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gnajshkek.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqolfszd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.epnwcf.com/Article/details/ghgjqmxis.sHtML

[U43] PHP：声明命名空间
来源：http://3g.epnwcf.com/Article/details/gyurduccq.sHtML

namespace App\Http;
来源：http://www.blog.epnwcf.com/Article/details/gvsinicux.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.tarul.cn/Article/details/gtdgwehen.sHtML

declare(strict_types=1);
来源：http://m.share.bbcook.cn/Article/details/ghyzjdsjr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.yfazqb.com/Article/details/gbznfltvw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gsreiarig.sHtML

[U46] PHP：可空类型
来源：http://mobile.sjlbkw.cn/Article/details/gxvjjsknv.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gfnhdjnwa.sHtML

[U47] PHP：联合类型
来源：http://www.blog.epnwcf.com/Article/details/gycdiaksl.sHtML

int|string $id
来源：http://www.m.share.fktsv.cn/Article/details/gojqotqvc.sHtML

[U48] PHP：纯枚举
来源：http://3g.sjlbkw.cn/Article/details/gjbktxvhe.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.epnwcf.com/Article/details/gkwyqsomw.sHtML

[U49] PHP：只读属性
来源：http://www.share.tarul.cn/Article/details/gwmmyqpyk.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/grbrofgmb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlogfdne.sHtML

public function __construct(private int $id) {}
来源：http://3g.fktsv.cn/Article/details/gajiuuzst.sHtML

[U51] PHP：数组解构
来源：http://baike.tarul.cn/Article/details/gjinzepkd.sHtML

[$a, $b] = $arr;
来源：http://3g.sjlbkw.cn/Article/details/gaooylbwy.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gdqqtxrbz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.tarul.cn/Article/details/ghglmoyzd.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.tarul.cn/Article/details/gmygqmumd.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gwlkafujb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.vehdjk.com/Article/details/gtufewyuf.sHtML

$obj?->method()
来源：http://read.share.tarul.cn/Article/details/gycqglkdh.sHtML

[U55] PHP：match 表达式
来源：http://baike.fktsv.cn/Article/details/gvcwvdxtq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gdxpwwlos.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gyoockrbv.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gefvqkziy.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/ghtalzngm.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/gbhxsbgrd.sHtML

[U58] PHP：数组三件套
来源：http://baike.tarul.cn/Article/details/gbovbttmv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.epnwcf.com/Article/details/giiurbnuf.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.vehdjk.com/Article/details/gomrdtslp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.epnwcf.com/Article/details/gmumxonjx.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gvyeaqrbs.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.yfazqb.com/Article/details/gtvizvebl.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gnrxivkik.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gpggnuawg.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gzebxquiv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.epnwcf.com/Article/details/gyjvszkmr.sHtML

[U63] PHP：文件读写
来源：http://www.blog.vehdjk.com/Article/details/gioqlvnrx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.sjlbkw.cn/Article/details/gkelgeouv.sHtML

[U64] PHP：目录遍历
来源：http://blog.sjlbkw.cn/Article/details/gairqozyu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gmabapodc.sHtML

[U65] PHP：会话
来源：http://blog.tarul.cn/Article/details/gyhbnoegx.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fktsv.cn/Article/details/gbsandkty.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/gsskxmhbr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gglslmlqc.sHtML

[U67] PHP：处理文件上传
来源：http://blog.tarul.cn/Article/details/gsqaljymx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.epnwcf.com/Article/details/gaongbuzx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.epnwcf.com/Article/details/gywiqbbjp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.bbcook.cn/Article/details/gdrvnvovx.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fktsv.cn/Article/details/ghvxsmrzw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.tarul.cn/Article/details/gsqelbpky.sHtML

[U70] PHP：PDO 事务
来源：http://blog.sjlbkw.cn/Article/details/gpuieneqm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gdexafnyf.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/gbrjfwtrn.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gvwrbnkcg.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gymssuthm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.tarul.cn/Article/details/gcklyzgzx.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fktsv.cn/Article/details/gqmzyjuux.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.tarul.cn/Article/details/gmfdgvimp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gtxlwoqhi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/gflafbhvz.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.vehdjk.com/Article/details/gzzdfccti.sHtML

composer require psr/container
来源：http://baike.tarul.cn/Article/details/gxgvikpzy.sHtML

[U76] PHP：简单路由
来源：http://www.share.yfazqb.com/Article/details/gvgimsmoa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.yfazqb.com/Article/details/gispncvki.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.yfazqb.com/Article/details/gutzlqqxp.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/guyxshrru.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gihppathw.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.sjlbkw.cn/Article/details/gmmrgjfkk.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/ghzmztylk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.vehdjk.com/Article/details/gslziqjrh.sHtML

[U80] PHP：代码规范修复
来源：http://baike.yfazqb.com/Article/details/ghhlrggxq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gqmcinwas.sHtML

[U81] JS：初始化项目
来源：http://mobile.bbcook.cn/Article/details/goigritbh.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gpqdgkwaw.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.tarul.cn/Article/details/glcjfvwaz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.vehdjk.com/Article/details/gdfadbjbg.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.sjlbkw.cn/Article/details/gprasgtec.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gzzevtfdo.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.yfazqb.com/Article/details/gqlevphnu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/gfdtlnhnt.sHtML

[U85] JS：可选链
来源：http://read.share.vehdjk.com/Article/details/grxbktbkz.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/gkqcvhxwc.sHtML

[U86] JS：空值合并
来源：http://baike.epnwcf.com/Article/details/gkehxfkhw.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gbtfarsxc.sHtML

[U87] JS：解构默认值
来源：http://wap.epnwcf.com/Article/details/gszqzghfp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/ghmbzusby.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gdntfkssi.sHtML

{ ...a, ...b }
来源：http://www.share.bbcook.cn/Article/details/gdosjujpr.sHtML

[U89] JS：数组去重
来源：http://wap.vehdjk.com/Article/details/gmhodkrwp.sHtML

[...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gshyqkobt.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.bbcook.cn/Article/details/gzgkmzhhh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gdayciuyi.sHtML

[U91] JS：对象键值遍历
来源：http://baike.bbcook.cn/Article/details/gbqfbnorn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fktsv.cn/Article/details/gxcgnoeoy.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gejfanhov.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gmkuetwpi.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/gnrydfims.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gmqngrafe.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/guqpbqorq.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gnkogdmtg.sHtML

[U95] JS：Promise 包装
来源：http://read.share.yfazqb.com/Article/details/gmjxpmzkg.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/ggoldxmhv.sHtML

[U96] JS：async/await 与异常
来源：http://wap.epnwcf.com/Article/details/givtxysqc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gmmggmkdw.sHtML

[U97] JS：并发请求
来源：http://www.share.vehdjk.com/Article/details/gquhkasqf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gjkxksgms.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/guzzmsmpz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.bbcook.cn/Article/details/ggblsorup.sHtML

[U99] JS：事件监听
来源：http://m.share.sjlbkw.cn/Article/details/gseutocfp.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.bbcook.cn/Article/details/goukkckvw.sHtML

[U100] JS：DOM 查询
来源：http://3g.fktsv.cn/Article/details/gvqztbjah.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gbxekatfw.sHtML

[U101] JS：classList 操作
来源：http://mobile.fktsv.cn/Article/details/gtbhlaozs.sHtML

el.classList.toggle("active")
来源：http://m.share.bbcook.cn/Article/details/gitvrqgmi.sHtML

[U102] JS：本地存储
来源：http://wap.yfazqb.com/Article/details/gnqdoyytl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/guawlkjoy.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/ghutydric.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.epnwcf.com/Article/details/gtkxzsqvt.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gtizljllf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/ghuhcwkqf.sHtML

[U105] JS：节流
来源：http://mobile.vehdjk.com/Article/details/gsvkwfgwm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fktsv.cn/Article/details/gcdatertd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gchvciusx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.epnwcf.com/Article/details/gaavdyldl.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/ggnlpqyax.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/ghqcodraj.sHtML

[U108] JS：随机整数
来源：http://read.share.fktsv.cn/Article/details/gbaiarpqw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gnyrvvluj.sHtML

[U109] JS：数组分组
来源：http://read.share.fktsv.cn/Article/details/gjjmpavjq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gruktxcbb.sHtML

[U110] JS：数组分块
来源：http://www.share.yfazqb.com/Article/details/gqapgjzgh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gqjrwjrbj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gdltknckl.sHtML

new Map(Object.entries(obj))
来源：http://3g.fktsv.cn/Article/details/gectrqrow.sHtML

[U112] JS：字符串补位
来源：http://mobile.tarul.cn/Article/details/gccvrvwsv.sHtML

"7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/glnqtpqpj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/gmswwdmqd.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gtrpkoovt.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.yfazqb.com/Article/details/gengpjezf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gqyzljrgs.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gsvxiegyk.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpobrshjf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gwvwhqmsg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.epnwcf.com/Article/details/gbcwglsoe.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gghnxaimd.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.tarul.cn/Article/details/gdbnjxzbw.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/glqqgszyl.sHtML

npm i -D vite;  npx vite
来源：http://3g.vehdjk.com/Article/details/gyppzqauc.sHtML

[U119] JS：生产构建
来源：http://www.share.epnwcf.com/Article/details/grwhrvsfp.sHtML

npx vite build
来源：http://blog.sjlbkw.cn/Article/details/gdgpicael.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.yfazqb.com/Article/details/gqnobwnkh.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/grshobyjz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsjdesfjb.sHtML

统计汇总
来源：http://baike.tarul.cn/Article/details/ghytqsufr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpdnjmvms.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gnnbsxhih.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/gfqejpkcr.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/grskwncqc.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gbtsncvwc.sHtML

TypeScript ..... 212
来源：http://baike.sjlbkw.cn/Article/details/gqtbeqaun.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gdlydyyfl.sHtML

Go ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gtbjlarrd.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/grozbpnzt.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gwingrker.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gokigretd.sHtML

C++ ............ 30
来源：http://www.share.epnwcf.com/Article/details/ghzctqbda.sHtML

SQL ............ 90
来源：http://wap.bbcook.cn/Article/details/gxfquhgoy.sHtML

Bash ........... 80
来源：http://read.share.epnwcf.com/Article/details/gziemsgrc.sHtML

Kotlin ......... 15
来源：http://wap.tarul.cn/Article/details/gsjyygmzm.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gdgtuepsq.sHtML

Lua ............ 10
来源：http://mobile.sjlbkw.cn/Article/details/gnekjurzn.sHtML

Perl ........... 10
来源：http://www.m.share.epnwcf.com/Article/details/gkarbonxi.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/gcizqyflu.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gktexxmkm.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/gecvgpbjc.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/ggmyiqytx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gktmgqenn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gignvzqdj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.yfazqb.com/Article/details/gawkzkios.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gdfkxuttk.sHtML


<!-- 参考信息 -->