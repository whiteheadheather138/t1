代发 wailian999

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/gxzshbudx.sHtML

"值: $a"
来源：http://baike.vehdjk.com/Article/details/gjvtjzhaq.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gqqmaqkpi.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gfkrwifeh.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/ggzvfyjuh.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gfwolmfrs.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gjqsxipul.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gnwewrizj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fktsv.cn/Article/details/goowtakod.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.tarul.cn/Article/details/gyoebbwwl.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gcrvkcrip.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/gymswyqos.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/ghymakqub.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gbkneqtko.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/guzsxohpb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gakajrokq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gjqvnrpzy.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gaxoortqm.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gsypitfdy.sHtML

[T52] Scala：变量
来源：http://3g.epnwcf.com/Article/details/grxdlalqq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gqiibozfh.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gjznejequ.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/grtleqoao.sHtML

[T54] Scala：集合映射
来源：http://m.share.sjlbkw.cn/Article/details/gbwqmhdjh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gjpmwqutd.sHtML

[T55] Scala：集合过滤
来源：http://blog.vehdjk.com/Article/details/gkdzcoajz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gdtcurzsm.sHtML

[T56] Scala：样例类
来源：http://www.blog.tarul.cn/Article/details/graxizebo.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gbdowhwsv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gmbrkrawz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gelvbhmiz.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gxpcodipr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/gsltqbryr.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gedsagnax.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/guikmxcau.sHtML

[T60] Scala：折叠
来源：http://3g.yfazqb.com/Article/details/gwdhwflhk.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.yfazqb.com/Article/details/gfedbjgfg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggcqjpipn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/gbywtaopu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giprvqbip.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gfyqvqzbv.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.vehdjk.com/Article/details/gbhzkaioz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gxrjvqmxg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.tarul.cn/Article/details/gmmwymeze.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.yfazqb.com/Article/details/ghmyysyjo.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.bbcook.cn/Article/details/gcadiojyb.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.epnwcf.com/Article/details/ghlxszzyr.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpviwmhf.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.vehdjk.com/Article/details/gtyovwmsk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gxkraqnxx.sHtML

[U06] Py：合并两个字典
来源：http://read.share.fktsv.cn/Article/details/gqrrtqlvo.sHtML

{**a, **b}
来源：http://3g.sjlbkw.cn/Article/details/grzjnfruc.sHtML

[U07] Py：反转字典键值
来源：http://3g.vehdjk.com/Article/details/gbpkhpoil.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gxqifhjbp.sHtML

[U08] Py：展平二维列表
来源：http://blog.tarul.cn/Article/details/gdvjugbfv.sHtML

[y for x in nested for y in x]
来源：http://3g.tarul.cn/Article/details/gpoziagsf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.vehdjk.com/Article/details/gprafeqku.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/grvulpclh.sHtML

[U10] Py：按值排序字典
来源：http://m.share.vehdjk.com/Article/details/gbczdrrdz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/ggafckzvo.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gikryztxi.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.fktsv.cn/Article/details/gymylaawp.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.tarul.cn/Article/details/gmobuxoai.sHtML

Counter(arr).most_common(3)
来源：http://wap.sjlbkw.cn/Article/details/ghroluwlm.sHtML

[U13] Py：固定长度队列
来源：http://3g.tarul.cn/Article/details/gadwtskmx.sHtML

deque(maxlen=10)
来源：http://3g.yfazqb.com/Article/details/gjwkgcfbv.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.fktsv.cn/Article/details/gnosyuwit.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/guzxsvplt.sHtML

[U15] Py：高精度计时
来源：http://m.share.yfazqb.com/Article/details/gqfafbjuy.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gycmrfxfm.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.sjlbkw.cn/Article/details/glrnnfieb.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.epnwcf.com/Article/details/ggrkzwffg.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/gbleaulmw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://wap.vehdjk.com/Article/details/gwgbljpzd.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gqlltnnxv.sHtML

pat = re.compile(r"\d+")
来源：http://3g.bbcook.cn/Article/details/gitbkhgdt.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.sjlbkw.cn/Article/details/gyoebqnmm.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.epnwcf.com/Article/details/gvtumekae.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gwhxpvabi.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.vehdjk.com/Article/details/gekqgrkkt.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.fktsv.cn/Article/details/gwrhkbqig.sHtML

@contextlib.contextmanager
来源：http://3g.epnwcf.com/Article/details/gglarhrws.sHtML

[U22] Py：矩阵转置
来源：http://www.blog.sjlbkw.cn/Article/details/gzgrkpkfs.sHtML

list(zip(*m))
来源：http://baike.epnwcf.com/Article/details/gydqxhpaq.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.fktsv.cn/Article/details/guhztiyuw.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/gxmohemro.sHtML

[U24] Py：路径操作
来源：http://blog.fktsv.cn/Article/details/goldtnggc.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gyvtpyvpq.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.sjlbkw.cn/Article/details/gvvdllpfi.sHtML

csv.DictReader(f)
来源：http://www.blog.bbcook.cn/Article/details/gvlxqgfzn.sHtML

[U26] Py：并发下载
来源：http://baike.sjlbkw.cn/Article/details/gxhwluhjh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.sjlbkw.cn/Article/details/gdhemosup.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.yfazqb.com/Article/details/giglhyxzm.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/geepryzdq.sHtML

[U28] Py：类型别名
来源：http://blog.fktsv.cn/Article/details/gfktqcbtn.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gzoghvxea.sHtML

[U29] Py：属性校验
来源：http://mobile.yfazqb.com/Article/details/gnufvrtmz.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gbdhjufbw.sHtML

[U30] Py：数据类
来源：http://www.m.share.vehdjk.com/Article/details/ghordmyjs.sHtML

@dataclass(slots=True)
来源：http://www.m.share.vehdjk.com/Article/details/gbnmvbxzd.sHtML

[U31] Py：单测
来源：http://read.share.sjlbkw.cn/Article/details/gconpaxkf.sHtML

python -m pytest -q
来源：http://www.share.fktsv.cn/Article/details/gwtquaksj.sHtML

[U32] Py：代码格式化
来源：http://wap.bbcook.cn/Article/details/gpeiumkxt.sHtML

ruff format . && ruff check --fix .
来源：http://3g.sjlbkw.cn/Article/details/gifvesaqs.sHtML

[U33] Py：打包发布
来源：http://www.m.share.epnwcf.com/Article/details/gshxnwhrl.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.vehdjk.com/Article/details/gdwhrwwwv.sHtML

[U34] Py：判断编码
来源：http://www.share.fktsv.cn/Article/details/gwaarccno.sHtML

chardet.detect(raw)
来源：http://mobile.yfazqb.com/Article/details/gawtwoaji.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gcrcyqnrb.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.fktsv.cn/Article/details/gvqaqahzq.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gnjhooupy.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.yfazqb.com/Article/details/gwydavjce.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.epnwcf.com/Article/details/gkxymqvqj.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.yfazqb.com/Article/details/gctbpkdbx.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gnytgyjyj.sHtML

Path(__file__).resolve().parent
来源：http://wap.fktsv.cn/Article/details/gnwlquych.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.tarul.cn/Article/details/gysnufnjn.sHtML

sys.stdout.isatty()
来源：http://read.share.tarul.cn/Article/details/guvhfoftx.sHtML

[U40] Py：打印到标准错误
来源：http://baike.sjlbkw.cn/Article/details/ghgkxywln.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/ghfvtssnw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.fktsv.cn/Article/details/gwlfzsjlc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.bbcook.cn/Article/details/grhcafapn.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.tarul.cn/Article/details/gcqwekvqv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://m.share.tarul.cn/Article/details/geooiiihb.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.bbcook.cn/Article/details/gomqcvilj.sHtML

namespace App\Http;
来源：http://3g.fktsv.cn/Article/details/gauquembe.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.epnwcf.com/Article/details/ghnegvsqf.sHtML

declare(strict_types=1);
来源：http://www.share.sjlbkw.cn/Article/details/gofljyyda.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.vehdjk.com/Article/details/gaycxtgds.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gkgtzeull.sHtML

[U46] PHP：可空类型
来源：http://www.blog.epnwcf.com/Article/details/gictfpbup.sHtML

?string $name = null
来源：http://baike.tarul.cn/Article/details/gotryrdfl.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fktsv.cn/Article/details/gabejoffc.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/ghszjneig.sHtML

[U48] PHP：纯枚举
来源：http://mobile.epnwcf.com/Article/details/gtlyugcrf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.vehdjk.com/Article/details/gpqdzxqmp.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpmrglcd.sHtML

public readonly string $name
来源：http://3g.yfazqb.com/Article/details/gwgndkhxu.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/gvvamyqzc.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.epnwcf.com/Article/details/gncnlkicv.sHtML

[U51] PHP：数组解构
来源：http://read.share.fktsv.cn/Article/details/gbdjfuucr.sHtML

[$a, $b] = $arr;
来源：http://www.share.vehdjk.com/Article/details/gwabtdmws.sHtML

[U52] PHP：箭头函数
来源：http://m.share.yfazqb.com/Article/details/gowegprve.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.bbcook.cn/Article/details/gxjvyidyf.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/glnhompzd.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/guzabgirk.sHtML

[U54] PHP：空安全调用
来源：http://blog.fktsv.cn/Article/details/gewffpsam.sHtML

$obj?->method()
来源：http://read.share.vehdjk.com/Article/details/ghhgdrcno.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fktsv.cn/Article/details/gbxniywax.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.bbcook.cn/Article/details/gvbuvkpsn.sHtML

[U56] PHP：命名参数
来源：http://read.share.yfazqb.com/Article/details/gvixopmpe.sHtML

f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gwoavzbkc.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gzuallmqc.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/gizzyvqou.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/gsrqphcni.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/gujrlymei.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gutohlglk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gugorbjfg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.tarul.cn/Article/details/gfnbflbta.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.vehdjk.com/Article/details/gvtcigflm.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gcnrujmrw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gbmhclpmr.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/gvcamxytv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.fktsv.cn/Article/details/gbfbbldqq.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/ggyummmmp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.yfazqb.com/Article/details/gfsywuiqo.sHtML

[U64] PHP：目录遍历
来源：http://wap.tarul.cn/Article/details/gtckubhdt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gzqmzaxvi.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gwxwobxny.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/govyrnzpl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.epnwcf.com/Article/details/gadwkphwr.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkdrlknc.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.bbcook.cn/Article/details/glphctofj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gympjobrx.sHtML

[U68] PHP：PDO 连接
来源：http://3g.vehdjk.com/Article/details/gutcvzvsn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.tarul.cn/Article/details/gpdeldlgn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.tarul.cn/Article/details/gbpvatwtd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.vehdjk.com/Article/details/gadcyoiot.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/glvjmpquv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/grybfqxbz.sHtML

[U71] PHP：抛出异常
来源：http://mobile.bbcook.cn/Article/details/gwehhiauf.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.epnwcf.com/Article/details/gybwrokoe.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.vehdjk.com/Article/details/ghodrbjwi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.epnwcf.com/Article/details/gcqocxhcn.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gogkmfwbd.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gannimjix.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gwefeqjcx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/grxuyvvpm.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.vehdjk.com/Article/details/ggytnuigk.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gicsgzlmi.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gpedfebmp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.vehdjk.com/Article/details/gzodtlrcm.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.epnwcf.com/Article/details/ggvjtdlir.sHtML

composer require twig/twig
来源：http://read.share.epnwcf.com/Article/details/glgowcuvj.sHtML

[U78] PHP：单元测试
来源：http://read.share.fktsv.cn/Article/details/gvoxysnsb.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.tarul.cn/Article/details/gcizbmjja.sHtML

[U79] PHP：静态分析
来源：http://baike.bbcook.cn/Article/details/gdhwpqwys.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/gucybepgt.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/gdrgfrnga.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gnjqpscaz.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.epnwcf.com/Article/details/gfbmrcswi.sHtML

npm init -y;  npm i express
来源：http://www.share.yfazqb.com/Article/details/gputvzgfe.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.vehdjk.com/Article/details/gkmjgkwcu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gtloeyzut.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.tarul.cn/Article/details/gophpcriv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/grwkzaekm.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.epnwcf.com/Article/details/gnxeuqrgb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.bbcook.cn/Article/details/gmqcgfpzb.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/gemxogohp.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gjcmgilwe.sHtML

[U86] JS：空值合并
来源：http://www.share.tarul.cn/Article/details/ghdjieyrx.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gqnhzxdal.sHtML

[U87] JS：解构默认值
来源：http://blog.fktsv.cn/Article/details/gefehjrzc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/goaxhvdzt.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fktsv.cn/Article/details/grbkjagfy.sHtML

{ ...a, ...b }
来源：http://read.share.epnwcf.com/Article/details/gqekhfsbf.sHtML

[U89] JS：数组去重
来源：http://blog.fktsv.cn/Article/details/gumzllnuf.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gasksjftw.sHtML

[U90] JS：数字数组排序
来源：http://mobile.yfazqb.com/Article/details/gvselivbg.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gpmmnulad.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/gjrjmtqby.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fktsv.cn/Article/details/gerynjghc.sHtML

[U92] JS：深拷贝
来源：http://mobile.yfazqb.com/Article/details/gbtwscfyb.sHtML

structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/ghkuwccwk.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gnffogjeq.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gmqurncqo.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/givqokvez.sHtML

const double = x => x * 2;
来源：http://3g.bbcook.cn/Article/details/gefktnrsk.sHtML

[U95] JS：Promise 包装
来源：http://blog.bbcook.cn/Article/details/gnhlgbfol.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.sjlbkw.cn/Article/details/gmutrnlpz.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gjmeqleek.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gizkqmdbp.sHtML

[U97] JS：并发请求
来源：http://3g.vehdjk.com/Article/details/gisbflyae.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/ggzbrrjqt.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.tarul.cn/Article/details/gmwgauoxj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.bbcook.cn/Article/details/gnbiaxaph.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/gttpxieby.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/ghcqglark.sHtML

[U100] JS：DOM 查询
来源：http://blog.tarul.cn/Article/details/glffivbxk.sHtML

document.querySelector(".item")
来源：http://www.blog.sjlbkw.cn/Article/details/gwzjjcqfi.sHtML

[U101] JS：classList 操作
来源：http://www.share.yfazqb.com/Article/details/gmplcctyt.sHtML

el.classList.toggle("active")
来源：http://mobile.yfazqb.com/Article/details/gjvzyluxb.sHtML

[U102] JS：本地存储
来源：http://read.share.epnwcf.com/Article/details/gztdtdkxx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/gpdthvbuu.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gnlyhtxpg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gqgqmfyto.sHtML

[U104] JS：防抖
来源：http://3g.sjlbkw.cn/Article/details/gpnvlzznn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/glimqblde.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/gsqsvvybh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gjmzhyllv.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gnmanhksj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.bbcook.cn/Article/details/gfzfbtyzs.sHtML

[U107] JS：数字千分位
来源：http://blog.tarul.cn/Article/details/gbxbhchoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gfieowafm.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxvxvgef.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gtavccqje.sHtML

[U109] JS：数组分组
来源：http://www.m.share.tarul.cn/Article/details/gujynuyas.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gulnvwqth.sHtML

[U110] JS：数组分块
来源：http://baike.bbcook.cn/Article/details/gzciilfxq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.epnwcf.com/Article/details/gbofjpzyi.sHtML

[U111] JS：对象转 Map
来源：http://m.share.vehdjk.com/Article/details/gawjjosjm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fktsv.cn/Article/details/gckrmrzxn.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gxebqzdgl.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gndmqgptv.sHtML

[U113] JS：正则替换全部
来源：http://www.share.sjlbkw.cn/Article/details/gribkfriv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/grzjjedmx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.yfazqb.com/Article/details/gdihxigdw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/gbfdjmjab.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gawacrclp.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gfuvwrzix.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gjkokgefb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fktsv.cn/Article/details/gikwptbkw.sHtML

[U117] JS：单元测试
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvmcmfca.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.epnwcf.com/Article/details/gzydlhnal.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gwjtkbidh.sHtML

npm i -D vite;  npx vite
来源：http://baike.vehdjk.com/Article/details/gljnokbyf.sHtML

[U119] JS：生产构建
来源：http://www.blog.bbcook.cn/Article/details/gdxvkkxdm.sHtML

npx vite build
来源：http://www.blog.epnwcf.com/Article/details/ghdnzknfd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gywccrrfi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/ggfzlfozm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggtraizvn.sHtML

统计汇总
来源：http://www.m.share.bbcook.cn/Article/details/gnrrtzaic.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjvtdegki.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/gkjntrkbf.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/gvaiqznif.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gjhyhihpg.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/gltieijio.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gkgqnyqhj.sHtML

Java ........... 212
来源：http://3g.epnwcf.com/Article/details/gsnqtncgo.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gbsbwczee.sHtML

Ruby ........... 212
来源：http://blog.sjlbkw.cn/Article/details/gcynbvjvq.sHtML

C# ............. 212
来源：http://wap.epnwcf.com/Article/details/gszidkgti.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gitknxzox.sHtML

C++ ............ 30
来源：http://www.blog.yfazqb.com/Article/details/govtfsjjv.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/gjcwrbxei.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gphhztsjk.sHtML

Kotlin ......... 15
来源：http://blog.bbcook.cn/Article/details/gpdwqwwwq.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/gtujimxpc.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gjgosgicz.sHtML

Perl ........... 10
来源：http://3g.sjlbkw.cn/Article/details/gqgyknghn.sHtML


<!-- 参考信息 -->