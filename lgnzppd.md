代发 wailian999

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gqrkbzfjy.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gasglfkgu.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gvsrcouaa.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.bbcook.cn/Article/details/gtyllayae.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gltnxmcch.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.vehdjk.com/Article/details/gaqkydqls.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gwzzhlfpe.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.epnwcf.com/Article/details/gfcvrmrzj.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gmciwrzca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/gcaykktox.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/gclfanrzw.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.vehdjk.com/Article/details/gjzdxbqiq.sHtML

[T49] Perl：函数
来源：http://blog.sjlbkw.cn/Article/details/gntihizsz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.vehdjk.com/Article/details/gjwadkfqe.sHtML

[T50] Perl：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gccewofbr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gyodiswxf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gdplcoxro.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gpzkyrrvx.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gfvnsmfwi.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/ghlggpttj.sHtML

val a = 1;  var b = 2
来源：http://blog.vehdjk.com/Article/details/gvqgqdzrm.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gnyiefhgm.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/grmpjggou.sHtML

[T54] Scala：集合映射
来源：http://3g.tarul.cn/Article/details/geqcsaxju.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gofsozzbm.sHtML

[T55] Scala：集合过滤
来源：http://blog.yfazqb.com/Article/details/gbfrsnjcl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.sjlbkw.cn/Article/details/gjzcwmfnd.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gtybsbacp.sHtML

case class User(name: String, age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gddzyhhrk.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gazbokeoc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gmjadikfy.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gbeiynwme.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gaemkroos.sHtML

[T59] Scala：循环
来源：http://www.share.vehdjk.com/Article/details/gplmqikiw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.tarul.cn/Article/details/gzxgtypjw.sHtML

[T60] Scala：折叠
来源：http://3g.epnwcf.com/Article/details/goxjtsfnz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.sjlbkw.cn/Article/details/gzoetidhp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbgiailrl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.sjlbkw.cn/Article/details/gkrkottrd.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdogfpxza.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gvdsuyhvo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/glwhpcaba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.tarul.cn/Article/details/gxfvamjwc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.vehdjk.com/Article/details/goljjvgql.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.bbcook.cn/Article/details/gaivdupod.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gxhvvrsqm.sHtML

[U04] Py：变量调试打印
来源：http://www.share.yfazqb.com/Article/details/grbmglfao.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gcbzlwtzq.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gjxkgrhif.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/givfyihen.sHtML

[U06] Py：合并两个字典
来源：http://blog.sjlbkw.cn/Article/details/gkljzgrsb.sHtML

{**a, **b}
来源：http://blog.sjlbkw.cn/Article/details/gmzgbuang.sHtML

[U07] Py：反转字典键值
来源：http://wap.sjlbkw.cn/Article/details/gyjxsnaqg.sHtML

{v: k for k, v in d.items()}
来源：http://baike.yfazqb.com/Article/details/gamlnnehj.sHtML

[U08] Py：展平二维列表
来源：http://read.share.tarul.cn/Article/details/gmspljkvc.sHtML

[y for x in nested for y in x]
来源：http://www.blog.epnwcf.com/Article/details/gopjpvyrq.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.tarul.cn/Article/details/gkudyskul.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gbulhwccn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.bbcook.cn/Article/details/gpgbjccdc.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gvhmsnhzd.sHtML

[U11] Py：生成器表达式
来源：http://mobile.tarul.cn/Article/details/gunjezlyn.sHtML

(x * 2 for x in arr)
来源：http://wap.tarul.cn/Article/details/gxjuoafvx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.vehdjk.com/Article/details/gqzwutdrc.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhsbuhym.sHtML

[U13] Py：固定长度队列
来源：http://baike.bbcook.cn/Article/details/gnnwnjyqx.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gqkrolbuo.sHtML

[U14] Py：分组收集到列表
来源：http://baike.sjlbkw.cn/Article/details/gcealssff.sHtML

defaultdict(list)
来源：http://wap.sjlbkw.cn/Article/details/glaxhvfau.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/guwkruzgw.sHtML

t = time.perf_counter()
来源：http://www.share.epnwcf.com/Article/details/gzruwreag.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.sjlbkw.cn/Article/details/gpwxajeeq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.yfazqb.com/Article/details/gauqexbwr.sHtML

[U17] Py：初始化日志
来源：http://3g.epnwcf.com/Article/details/gjybthvtc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.yfazqb.com/Article/details/gxbrzhmfv.sHtML

[U18] Py：预编译正则
来源：http://wap.sjlbkw.cn/Article/details/gpxpupnsg.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.bbcook.cn/Article/details/gqklrykkl.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.vehdjk.com/Article/details/gitbnbinc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mobile.tarul.cn/Article/details/gxrfpdpkt.sHtML

[U20] Py：缓存函数结果
来源：http://wap.vehdjk.com/Article/details/gjpojwswh.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.sjlbkw.cn/Article/details/ghhvrknuo.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.vehdjk.com/Article/details/gvcdaqpeg.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gwmrrcusm.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/gczpwyhiv.sHtML

list(zip(*m))
来源：http://baike.tarul.cn/Article/details/gjbqaonro.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/gqnahncbc.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.tarul.cn/Article/details/gdxcfdaha.sHtML

[U24] Py：路径操作
来源：http://baike.tarul.cn/Article/details/gbbgvdimi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gfncbhuzs.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.bbcook.cn/Article/details/gpapqooek.sHtML

csv.DictReader(f)
来源：http://3g.vehdjk.com/Article/details/gnlqfopbb.sHtML

[U26] Py：并发下载
来源：http://mobile.yfazqb.com/Article/details/ggmtgijjt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.vehdjk.com/Article/details/gukeglelf.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gxfldobgo.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.vehdjk.com/Article/details/gonxgwdlu.sHtML

[U28] Py：类型别名
来源：http://read.share.fktsv.cn/Article/details/gdzjchcxe.sHtML

UserId = int
来源：http://blog.bbcook.cn/Article/details/gcvexdrkr.sHtML

[U29] Py：属性校验
来源：http://www.share.yfazqb.com/Article/details/gekjbxkbw.sHtML

@property 与 @x.setter 配合
来源：http://baike.vehdjk.com/Article/details/gwzimnrei.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/gvtfxdcvh.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/glxvapqaa.sHtML

[U31] Py：单测
来源：http://m.share.sjlbkw.cn/Article/details/gdevrvhxs.sHtML

python -m pytest -q
来源：http://www.m.share.yfazqb.com/Article/details/golcijcuv.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/goxsbwlvy.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/givjpwgyo.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gatzgtjsy.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.vehdjk.com/Article/details/gxpzivtmy.sHtML

[U34] Py：判断编码
来源：http://baike.sjlbkw.cn/Article/details/gieuzlwzj.sHtML

chardet.detect(raw)
来源：http://m.share.sjlbkw.cn/Article/details/gwkxovnxg.sHtML

[U35] Py：发送邮件
来源：http://baike.yfazqb.com/Article/details/gevanmljq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.tarul.cn/Article/details/gwgxzgchr.sHtML

[U36] Py：定时任务
来源：http://www.share.epnwcf.com/Article/details/ggcskukdu.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.vehdjk.com/Article/details/gvnqpfgjq.sHtML

[U37] Py：读写 Excel
来源：http://blog.vehdjk.com/Article/details/gppulpkew.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.tarul.cn/Article/details/gcdcukeuw.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/guhnrhnnw.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.fktsv.cn/Article/details/gcvpowpzl.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.sjlbkw.cn/Article/details/ghvptracj.sHtML

sys.stdout.isatty()
来源：http://blog.bbcook.cn/Article/details/gwvsciokw.sHtML

[U40] Py：打印到标准错误
来源：http://wap.tarul.cn/Article/details/gfnoyxzbc.sHtML

print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/geexnnekx.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.bbcook.cn/Article/details/gptgkajpa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gfdkhkziu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.share.fktsv.cn/Article/details/gqbzmtgyu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.sjlbkw.cn/Article/details/gnvnxnmui.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.epnwcf.com/Article/details/gpkuhgxkf.sHtML

namespace App\Http;
来源：http://blog.vehdjk.com/Article/details/gutbvowhe.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/ggzojdvvr.sHtML

declare(strict_types=1);
来源：http://m.share.sjlbkw.cn/Article/details/gjxtpuhdb.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.fktsv.cn/Article/details/gvbpybeyn.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gdaqxirvx.sHtML

[U46] PHP：可空类型
来源：http://www.share.yfazqb.com/Article/details/ggrtaogbq.sHtML

?string $name = null
来源：http://m.share.fktsv.cn/Article/details/gylxglbtk.sHtML

[U47] PHP：联合类型
来源：http://www.blog.fktsv.cn/Article/details/gwwqqxdli.sHtML

int|string $id
来源：http://blog.vehdjk.com/Article/details/gteysffht.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/gixjpsmrg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.yfazqb.com/Article/details/gymjzhxeo.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gekywmfzu.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/ggfbkumzw.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/gbqwhdxol.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.tarul.cn/Article/details/ghiiywdbr.sHtML

[U51] PHP：数组解构
来源：http://mobile.vehdjk.com/Article/details/gabmfjaya.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gtcntdpib.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gprhvgvvs.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.tarul.cn/Article/details/gmlfijbaj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.fktsv.cn/Article/details/gyljahboe.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.vehdjk.com/Article/details/gpoocqaco.sHtML

[U54] PHP：空安全调用
来源：http://blog.tarul.cn/Article/details/gxvcufxta.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gsufrcsqj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gbxrmgnoh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.yfazqb.com/Article/details/glmrgfkrr.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.vehdjk.com/Article/details/grygdzprc.sHtML

f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gqfbzwijb.sHtML

[U57] PHP：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gddjnuzjd.sHtML

"值: {$a}"
来源：http://m.share.vehdjk.com/Article/details/gbzstaqjz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/ghxyzrzdi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fktsv.cn/Article/details/gbyxjekaj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/grkaqfkmd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.sjlbkw.cn/Article/details/gumiamckr.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gjwwzyazv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.bbcook.cn/Article/details/gpvcojxev.sHtML

[U61] PHP：正则
来源：http://www.m.share.bbcook.cn/Article/details/ggxkbhcrd.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/ghrzwbavf.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gjoxvzrct.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fktsv.cn/Article/details/ggoxmeewl.sHtML

[U63] PHP：文件读写
来源：http://www.blog.yfazqb.com/Article/details/gelfrndao.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.yfazqb.com/Article/details/gdmfihsiq.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gwdelbnoa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.tarul.cn/Article/details/gtosoiucg.sHtML

[U65] PHP：会话
来源：http://wap.epnwcf.com/Article/details/goajnjfmr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.tarul.cn/Article/details/gmbhqfxjs.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fktsv.cn/Article/details/gytnfverw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.yfazqb.com/Article/details/gekkupqcv.sHtML

[U67] PHP：处理文件上传
来源：http://3g.epnwcf.com/Article/details/gstadsayp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.tarul.cn/Article/details/gzjhhzbdq.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.vehdjk.com/Article/details/gnbngxndv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gyizqzktz.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gaxyttbed.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gnqbjbmld.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gukvhswzo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gvucjfwri.sHtML

[U71] PHP：抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gewsbgjwd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gxqmpwfdf.sHtML

[U72] PHP：写错误日志
来源：http://baike.bbcook.cn/Article/details/gmfrqrwwy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/ggdgvmeqq.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.yfazqb.com/Article/details/gwvvrqfpn.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gfveeqlzg.sHtML

[U74] PHP：读取环境变量
来源：http://blog.vehdjk.com/Article/details/gsbvvmgat.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/gkkznttpy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.epnwcf.com/Article/details/gxelazoxs.sHtML

composer require psr/container
来源：http://mobile.bbcook.cn/Article/details/gyzuuwhyi.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/geqfakjai.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.bbcook.cn/Article/details/gfewjwbpf.sHtML

[U77] PHP：模板渲染
来源：http://baike.fktsv.cn/Article/details/gtuedfqlc.sHtML

composer require twig/twig
来源：http://baike.epnwcf.com/Article/details/gbpmpnsag.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/ghctzvtwk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/gdgqjgrmn.sHtML

[U79] PHP：静态分析
来源：http://read.share.vehdjk.com/Article/details/ghuodppza.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.yfazqb.com/Article/details/gtshpktow.sHtML

[U80] PHP：代码规范修复
来源：http://blog.tarul.cn/Article/details/gejuatcui.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.bbcook.cn/Article/details/gexumkgzh.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/geymlefrn.sHtML

npm init -y;  npm i express
来源：http://wap.vehdjk.com/Article/details/gaetuzrjv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.vehdjk.com/Article/details/gxslnwwnz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.sjlbkw.cn/Article/details/gtmjmrfmo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gixtpqqll.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gplfxcujv.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.epnwcf.com/Article/details/gkrymuukd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gzfppyroj.sHtML

[U85] JS：可选链
来源：http://mobile.yfazqb.com/Article/details/ggbvizjnp.sHtML

a?.b?.c
来源：http://www.blog.bbcook.cn/Article/details/gpmkvnihu.sHtML

[U86] JS：空值合并
来源：http://3g.yfazqb.com/Article/details/ggguaxfam.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/gzxaufjss.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/gwkfafyoe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.tarul.cn/Article/details/gvdjfiqtf.sHtML

[U88] JS：对象展开合并
来源：http://3g.tarul.cn/Article/details/gsthfouwn.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/gonflexxq.sHtML

[U89] JS：数组去重
来源：http://wap.yfazqb.com/Article/details/gwrnutuqq.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gsbfzdcmb.sHtML

[U90] JS：数字数组排序
来源：http://wap.yfazqb.com/Article/details/grkblfdcm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gjabizrsy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.yfazqb.com/Article/details/gjutugfph.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gjcepyvbe.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gzpyjbfns.sHtML

structuredClone(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gqtskubpk.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fktsv.cn/Article/details/gqmodwbvo.sHtML

`共 ${n} 条`
来源：http://3g.epnwcf.com/Article/details/gvpywqeyj.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gslwnpufs.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gbybzqlrj.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/gnsctiowj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/gddakwsuw.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gawlecykq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/ggrzuwtul.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gtuxibjae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gbnvibywk.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.sjlbkw.cn/Article/details/gyimjosui.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/gmtrcbvwh.sHtML

[U99] JS：事件监听
来源：http://3g.fktsv.cn/Article/details/gfgiuxzeh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/gpavruxto.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/gzfzeugoa.sHtML

document.querySelector(".item")
来源：http://mobile.fktsv.cn/Article/details/gmrfmjmrn.sHtML

[U101] JS：classList 操作
来源：http://m.share.epnwcf.com/Article/details/gdyojwdvb.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gffbazknp.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/gmjuxvvav.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/gkluqpiuc.sHtML

[U103] JS：定时器
来源：http://mobile.fktsv.cn/Article/details/gtqittbcf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.vehdjk.com/Article/details/gmwyaefux.sHtML

[U104] JS：防抖
来源：http://mobile.tarul.cn/Article/details/gmcrkbict.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gguinlcov.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gawadkudl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/ghobabjuu.sHtML

[U106] JS：日期格式化
来源：http://baike.epnwcf.com/Article/details/glqjirzgt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.vehdjk.com/Article/details/gsoyhsydw.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gyqhueexx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gkcshgmdi.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gvxakxyqv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.sjlbkw.cn/Article/details/grqdvhtfy.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gvetuvfja.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gbthammhm.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/gtefreycr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.vehdjk.com/Article/details/ghvlzhzbq.sHtML

[U111] JS：对象转 Map
来源：http://wap.yfazqb.com/Article/details/gtveiicey.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gfwytgrvj.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gjbrahklm.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gpqizbmpm.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzqwpwtj.sHtML

s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gyuenoidy.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fktsv.cn/Article/details/gaafgybfd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gernuccos.sHtML

[U115] JS：生成 UUID
来源：http://baike.sjlbkw.cn/Article/details/gpgytfmtn.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gyjnqadvg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.bbcook.cn/Article/details/gbexwqxmi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkyzsqlxy.sHtML

[U117] JS：单元测试
来源：http://3g.fktsv.cn/Article/details/goqonvlfh.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.yfazqb.com/Article/details/gtdpaaogu.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gduvambvo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fktsv.cn/Article/details/ggsiysziq.sHtML

[U119] JS：生产构建
来源：http://read.share.fktsv.cn/Article/details/ggovgpcvu.sHtML

npx vite build
来源：http://wap.fktsv.cn/Article/details/gampmjnzi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/gmcomxskw.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/gszrzqrrh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/giuokvtnn.sHtML

统计汇总
来源：http://blog.sjlbkw.cn/Article/details/grqxalgsy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdagfkbeg.sHtML

按语言统计（条）：
来源：http://read.share.vehdjk.com/Article/details/gvdyoftap.sHtML

Python ......... 252
来源：http://blog.bbcook.cn/Article/details/gtfubbzwd.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gxcyyvquq.sHtML

JavaScript ..... 252
来源：http://www.share.fktsv.cn/Article/details/gfxlzqirp.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/gomrwvfch.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/ggehramtt.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gxzdhgdbo.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gtlqkdmva.sHtML

C# ............. 212
来源：http://mobile.fktsv.cn/Article/details/gvutvdbei.sHtML

C .............. 30
来源：http://www.m.share.yfazqb.com/Article/details/gvxtldjxp.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gueoxvvyk.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gbpehvpet.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/gkplmaiaa.sHtML

Kotlin ......... 15
来源：http://baike.fktsv.cn/Article/details/gtxihhwht.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/ghisakvmp.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/gmljntcym.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gpyezztsc.sHtML


<!-- 参考信息 -->