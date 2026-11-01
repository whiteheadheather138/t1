代发 wailian999

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gvutzsgoq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.tarul.cn/Article/details/gfvidpubd.sHtML

[T36] Lua：函数
来源：http://3g.tarul.cn/Article/details/grovggzxa.sHtML

function add(a, b) return a + b end
来源：http://www.blog.vehdjk.com/Article/details/gbmjkexpk.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gejsbnldb.sHtML

"a" .. "b"
来源：http://www.share.sjlbkw.cn/Article/details/gdbuqrzwz.sHtML

[T38] Lua：条件
来源：http://baike.fktsv.cn/Article/details/gzyjcaoat.sHtML

if x > 0 then print("正") end
来源：http://wap.tarul.cn/Article/details/ggdubhtau.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gfmqygfcv.sHtML

string.find(s, "%d+")
来源：http://www.m.share.tarul.cn/Article/details/glrnfukga.sHtML

[T40] Lua：元表
来源：http://read.share.epnwcf.com/Article/details/gtnmlokcx.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gdergwstl.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gcmalqsqp.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gmzuboshr.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gfyvjisti.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gzijchnzv.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gqrcxgnaq.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrxhmyty.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/gjrdqolvz.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gsfreszwr.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gvpmjmqkg.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.epnwcf.com/Article/details/gtplvdaba.sHtML

[T46] Perl：哈希操作
来源：http://read.share.sjlbkw.cn/Article/details/gxldzzjrj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzjndxgre.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/gusvhymie.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/grmtlbind.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gqjibmqbt.sHtML

$s =~ s/old/new/g;
来源：http://mobile.sjlbkw.cn/Article/details/gcidldfua.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/gwridphmt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/goyocutfo.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gwxegihse.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/gmdixddcf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gjiuipbmv.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gqrwjzyui.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/gopicwckv.sHtML

[T52] Scala：变量
来源：http://mobile.sjlbkw.cn/Article/details/gaxqccexx.sHtML

val a = 1;  var b = 2
来源：http://www.share.fktsv.cn/Article/details/gjvptrfch.sHtML

[T53] Scala：字符串插值
来源：http://blog.vehdjk.com/Article/details/gugyeoujy.sHtML

s"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/gqazjakuq.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gcwmpuwwv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gdmgqhqux.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gjodukxzd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.yfazqb.com/Article/details/geigjmuqm.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/glfcimeqe.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/ghiujhtib.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/gmamjhwoa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gkgmnjjnb.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/garkekjjg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.yfazqb.com/Article/details/gyyuwtheu.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gtonowgwh.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gejnxipib.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gyipwbxlr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzplqfpi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghlrzvgjv.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/giulbpymo.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzucgiqjb.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gigrdrktn.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gxwoquihx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/ggtswqkep.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gbhyuuumo.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.fktsv.cn/Article/details/gfbuzypzh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/ggmatxhrk.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/geuoacecq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/gfqukwkzp.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.vehdjk.com/Article/details/gimfphtce.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gbctgqezb.sHtML

[U06] Py：合并两个字典
来源：http://read.share.epnwcf.com/Article/details/glhdxllxd.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gkhrnasmp.sHtML

[U07] Py：反转字典键值
来源：http://3g.tarul.cn/Article/details/ggzuveutk.sHtML

{v: k for k, v in d.items()}
来源：http://blog.vehdjk.com/Article/details/gnjxymsbq.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.vehdjk.com/Article/details/gbtybydmu.sHtML

[y for x in nested for y in x]
来源：http://wap.tarul.cn/Article/details/gzsbtnrae.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.vehdjk.com/Article/details/glbhxvseo.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/gnopaztdg.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/ggvxtavsg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gsbmaoith.sHtML

[U11] Py：生成器表达式
来源：http://wap.vehdjk.com/Article/details/gncexrlmb.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gzdrayzvx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.yfazqb.com/Article/details/getlqlgxk.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.fktsv.cn/Article/details/gbvlwzxjz.sHtML

[U13] Py：固定长度队列
来源：http://mobile.epnwcf.com/Article/details/gjxvdgpfa.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/golgrktzg.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.tarul.cn/Article/details/gdwagimlb.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gmjxqkqps.sHtML

[U15] Py：高精度计时
来源：http://www.share.fktsv.cn/Article/details/grvgqngzu.sHtML

t = time.perf_counter()
来源：http://blog.tarul.cn/Article/details/gjarpxjmy.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gpdhvtmiq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.bbcook.cn/Article/details/gsqttsxpq.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.yfazqb.com/Article/details/grwwpjdxu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gxzkvyvkf.sHtML

[U18] Py：预编译正则
来源：http://3g.tarul.cn/Article/details/gixibcdvc.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.epnwcf.com/Article/details/gtakfypbu.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.tarul.cn/Article/details/gulfabqtz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.sjlbkw.cn/Article/details/gqkjxdvvn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.tarul.cn/Article/details/gmecxptdm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.yfazqb.com/Article/details/gugbpoldk.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gwgniroly.sHtML

@contextlib.contextmanager
来源：http://www.m.share.fktsv.cn/Article/details/gtaezmrih.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gkapkopbx.sHtML

list(zip(*m))
来源：http://www.blog.bbcook.cn/Article/details/gqryejlze.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.sjlbkw.cn/Article/details/gvluzyuuj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.sjlbkw.cn/Article/details/ggxhiaglk.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/gnyemagvi.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gfjdxmmjz.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.vehdjk.com/Article/details/gzksgqvvr.sHtML

csv.DictReader(f)
来源：http://blog.vehdjk.com/Article/details/gmsenswua.sHtML

[U26] Py：并发下载
来源：http://www.m.share.bbcook.cn/Article/details/gcxhxykap.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.epnwcf.com/Article/details/gzgvivzom.sHtML

[U27] Py：异步 HTTP
来源：http://3g.fktsv.cn/Article/details/gpncbmfkt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gfbppuygc.sHtML

[U28] Py：类型别名
来源：http://www.share.tarul.cn/Article/details/gwoorgxby.sHtML

UserId = int
来源：http://www.blog.fktsv.cn/Article/details/gdmidnypo.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gnwyaxzan.sHtML

@property 与 @x.setter 配合
来源：http://mobile.tarul.cn/Article/details/gvmvaqffn.sHtML

[U30] Py：数据类
来源：http://m.share.vehdjk.com/Article/details/gxvffxelo.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gxnvdluik.sHtML

[U31] Py：单测
来源：http://m.share.tarul.cn/Article/details/gvcupkauo.sHtML

python -m pytest -q
来源：http://mobile.bbcook.cn/Article/details/gqclsyjkl.sHtML

[U32] Py：代码格式化
来源：http://www.blog.vehdjk.com/Article/details/gmeqjrzra.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gpfqkkmqp.sHtML

[U33] Py：打包发布
来源：http://3g.bbcook.cn/Article/details/gtwrmcirz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.sjlbkw.cn/Article/details/gsidwwowt.sHtML

[U34] Py：判断编码
来源：http://wap.epnwcf.com/Article/details/gtvkcgtjf.sHtML

chardet.detect(raw)
来源：http://wap.vehdjk.com/Article/details/gisahyges.sHtML

[U35] Py：发送邮件
来源：http://3g.fktsv.cn/Article/details/geqhhjbuj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gnfhkizds.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gvdiezkvh.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.bbcook.cn/Article/details/gtapnahpg.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/gibdhqwzg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.epnwcf.com/Article/details/gvtcxqxbl.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.fktsv.cn/Article/details/gtmmrfalk.sHtML

Path(__file__).resolve().parent
来源：http://3g.yfazqb.com/Article/details/gwarffwal.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/gaixsmmtd.sHtML

sys.stdout.isatty()
来源：http://wap.vehdjk.com/Article/details/gwgpmvvqs.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/giwwkrihw.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gehmfrzns.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.vehdjk.com/Article/details/gifzadkyp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gbfygkbyu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.tarul.cn/Article/details/gnxdidsvh.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fktsv.cn/Article/details/gcwkdsfjl.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/ggkuecflm.sHtML

namespace App\Http;
来源：http://blog.fktsv.cn/Article/details/gwoyjuagv.sHtML

[U44] PHP：开启严格类型
来源：http://baike.tarul.cn/Article/details/gkgeuvexf.sHtML

declare(strict_types=1);
来源：http://read.share.vehdjk.com/Article/details/gjbpayhbm.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.bbcook.cn/Article/details/gtcjhbmqi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gvcxsrgcm.sHtML

[U46] PHP：可空类型
来源：http://read.share.yfazqb.com/Article/details/gqmujllzc.sHtML

?string $name = null
来源：http://blog.yfazqb.com/Article/details/gqshbwsao.sHtML

[U47] PHP：联合类型
来源：http://blog.yfazqb.com/Article/details/gojsiqpbo.sHtML

int|string $id
来源：http://blog.fktsv.cn/Article/details/ggkgjwtrd.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fktsv.cn/Article/details/gskimqqaz.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/grtekyikf.sHtML

[U49] PHP：只读属性
来源：http://www.blog.tarul.cn/Article/details/goedhovuo.sHtML

public readonly string $name
来源：http://3g.epnwcf.com/Article/details/gptabffjp.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/ggbcwliiw.sHtML

public function __construct(private int $id) {}
来源：http://read.share.yfazqb.com/Article/details/gbifdsmzl.sHtML

[U51] PHP：数组解构
来源：http://blog.fktsv.cn/Article/details/gxpwtoczp.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/ghvxprovd.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gbgeiffmt.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/gntfzpimz.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.epnwcf.com/Article/details/gxpgradki.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.m.share.epnwcf.com/Article/details/gaqbbjmkf.sHtML

[U54] PHP：空安全调用
来源：http://blog.epnwcf.com/Article/details/gqvjxeuew.sHtML

$obj?->method()
来源：http://3g.tarul.cn/Article/details/gjhzacpkt.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fktsv.cn/Article/details/ghuuwmeni.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/gagxpfzls.sHtML

[U56] PHP：命名参数
来源：http://blog.fktsv.cn/Article/details/gnrbhsmzs.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gwogirmeq.sHtML

[U57] PHP：字符串插值
来源：http://wap.yfazqb.com/Article/details/gvzdigxmj.sHtML

"值: {$a}"
来源：http://3g.epnwcf.com/Article/details/gnuvfbxdl.sHtML

[U58] PHP：数组三件套
来源：http://3g.yfazqb.com/Article/details/gbifvywxv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gqaxtlzmm.sHtML

[U59] PHP：自定义排序
来源：http://baike.fktsv.cn/Article/details/gkhgroefk.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gxggwqawu.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.tarul.cn/Article/details/gfyycmhni.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.tarul.cn/Article/details/gzueumvmk.sHtML

[U61] PHP：正则
来源：http://3g.fktsv.cn/Article/details/gusdhpdwz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gwnhkfxgd.sHtML

[U62] PHP：日期对象
来源：http://baike.fktsv.cn/Article/details/gomvinvrv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.tarul.cn/Article/details/gwkuzznxk.sHtML

[U63] PHP：文件读写
来源：http://mobile.tarul.cn/Article/details/gdcmykqwt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.sjlbkw.cn/Article/details/gjtiokror.sHtML

[U64] PHP：目录遍历
来源：http://www.share.sjlbkw.cn/Article/details/ghxfkmlfy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/grquecwvp.sHtML

[U65] PHP：会话
来源：http://read.share.yfazqb.com/Article/details/gmdnmabbk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gfoygkate.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gjssubznh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.epnwcf.com/Article/details/grffkdfmi.sHtML

[U67] PHP：处理文件上传
来源：http://wap.epnwcf.com/Article/details/gfxztahng.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.fktsv.cn/Article/details/gjqfrtnaj.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.tarul.cn/Article/details/gmyxevayp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.vehdjk.com/Article/details/gqueabzmd.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/geiklnzaq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/grkfalpmx.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/grqoahawf.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/gsifftigx.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/gdwgullyq.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gcnfeepuo.sHtML

[U72] PHP：写错误日志
来源：http://wap.vehdjk.com/Article/details/gpntikrqf.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/gyhdwmwtb.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gixuykgxx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.epnwcf.com/Article/details/geyruxqzg.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/ghwlfpfch.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/gayeaevyn.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.tarul.cn/Article/details/ghtcujuzq.sHtML

composer require psr/container
来源：http://mobile.fktsv.cn/Article/details/gjmqjyxjk.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/giepvgczz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fktsv.cn/Article/details/gkumvofwl.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/gvefzgptj.sHtML

composer require twig/twig
来源：http://mobile.tarul.cn/Article/details/gzqobalct.sHtML

[U78] PHP：单元测试
来源：http://www.share.sjlbkw.cn/Article/details/gybymczdp.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.yfazqb.com/Article/details/gmnrgdrim.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gveyqmkwc.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.epnwcf.com/Article/details/gompbhlng.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gnymydbuf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gctdvqmou.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gcxogcttx.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/goexocvzg.sHtML

[U82] JS：package.json 脚本
来源：http://3g.epnwcf.com/Article/details/ghnoelvkt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.bbcook.cn/Article/details/gqwwcwlsp.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.tarul.cn/Article/details/gjfiehgvx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gjzcjmkjm.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.bbcook.cn/Article/details/gtzjoucqp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/guvrhmayj.sHtML

[U85] JS：可选链
来源：http://www.blog.vehdjk.com/Article/details/gxcstxsjn.sHtML

a?.b?.c
来源：http://read.share.yfazqb.com/Article/details/gbkyxdgjm.sHtML

[U86] JS：空值合并
来源：http://www.blog.yfazqb.com/Article/details/gxlbmqeec.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gazxxthaf.sHtML

[U87] JS：解构默认值
来源：http://blog.fktsv.cn/Article/details/gyoxygofw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/gqavhstau.sHtML

[U88] JS：对象展开合并
来源：http://wap.fktsv.cn/Article/details/gulurxjjv.sHtML

{ ...a, ...b }
来源：http://mobile.yfazqb.com/Article/details/gtyduytcu.sHtML

[U89] JS：数组去重
来源：http://3g.vehdjk.com/Article/details/gmatxnbkn.sHtML

[...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gdpwoxcyn.sHtML

[U90] JS：数字数组排序
来源：http://mobile.tarul.cn/Article/details/gongsjamm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gykwkflqf.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.epnwcf.com/Article/details/gksorccng.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/gtzswejvt.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fktsv.cn/Article/details/ggqlhelpy.sHtML

structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaycozxql.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/gzjnioqnv.sHtML

`共 ${n} 条`
来源：http://3g.sjlbkw.cn/Article/details/gwlkgluqa.sHtML

[U94] JS：箭头函数
来源：http://baike.yfazqb.com/Article/details/gxplxtsud.sHtML

const double = x => x * 2;
来源：http://blog.bbcook.cn/Article/details/geoyxprwz.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/gwsdknlmd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gimotdbvl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/gigmaunut.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gmsdtgrnt.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gktcsdsrw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/grtyqnazb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gktspvmas.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.epnwcf.com/Article/details/gehbamyaz.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/gywpcvwzw.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.tarul.cn/Article/details/ghvlznjqd.sHtML

[U100] JS：DOM 查询
来源：http://baike.tarul.cn/Article/details/gwiilsgsm.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/glcdiveso.sHtML

[U101] JS：classList 操作
来源：http://blog.tarul.cn/Article/details/gzwgtavlt.sHtML

el.classList.toggle("active")
来源：http://www.share.epnwcf.com/Article/details/gbujieqka.sHtML

[U102] JS：本地存储
来源：http://www.share.tarul.cn/Article/details/gvfsqzkrl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.vehdjk.com/Article/details/gczlodxaq.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/gboakqvkm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gpxnvlgnk.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gleojifgq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gzhrjbplp.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gathysmaq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.epnwcf.com/Article/details/gievomjkt.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/gskhjqdqi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gzzswkrxu.sHtML

[U107] JS：数字千分位
来源：http://3g.vehdjk.com/Article/details/gngwawqae.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gieazucfz.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gjtlgrbch.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.bbcook.cn/Article/details/gzwnfljzv.sHtML

[U109] JS：数组分组
来源：http://mobile.tarul.cn/Article/details/gkbjalwwo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/guufffurb.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/gvxhaujfy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.epnwcf.com/Article/details/gvirdibba.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gjpbzpyyf.sHtML

new Map(Object.entries(obj))
来源：http://baike.sjlbkw.cn/Article/details/gxdemxomw.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gqpkwmtyg.sHtML

"7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gtfdxzngw.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gmgcxjrdt.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gmnmvqecm.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gfmztxzvs.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gpauyqrit.sHtML

[U115] JS：生成 UUID
来源：http://3g.yfazqb.com/Article/details/ghefciupb.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/ghfpkbaoy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/gxpzybasu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gpvlltngt.sHtML

[U117] JS：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gzoyxmtuz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.sjlbkw.cn/Article/details/gziqtkbwf.sHtML

[U118] JS：开发服务器
来源：http://m.share.bbcook.cn/Article/details/gzgljbgtf.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fktsv.cn/Article/details/ggrjozfqf.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gdjaopuha.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/gpdtsqqua.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.bbcook.cn/Article/details/grdzfwann.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fktsv.cn/Article/details/gzmvdufnc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/getkpdhmx.sHtML

统计汇总
来源：http://wap.vehdjk.com/Article/details/gopveqwxd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gynpppoiy.sHtML

按语言统计（条）：
来源：http://read.share.tarul.cn/Article/details/gojzvzgvs.sHtML


<!-- 参考信息 -->