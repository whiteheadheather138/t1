代发 wailian999

[T29] Swift：guard 提前返回
来源：http://3g.bbcook.cn/Article/details/gxipvvqyc.sHtML

guard let x = opt else { return }
来源：http://blog.sjlbkw.cn/Article/details/gsrsvmjfs.sHtML

[T30] Swift：协议
来源：http://m.share.bbcook.cn/Article/details/gomrkvvlt.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/gquigkvgr.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gsdhuaeqe.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/gsbbmkozu.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gmkeyxgfa.sHtML

local a = 1
来源：http://www.blog.epnwcf.com/Article/details/gvehmrndl.sHtML

[T33] Lua：表（数组）
来源：http://baike.yfazqb.com/Article/details/gxyvmiuuo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gdcdlaowf.sHtML

[T34] Lua：遍历表
来源：http://www.share.bbcook.cn/Article/details/gwymzmqxa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gvkwxnbsv.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gaukujvdb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gjkfioqvf.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/gemopsyvp.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gcxymvqet.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gtimhczbs.sHtML

"a" .. "b"
来源：http://wap.vehdjk.com/Article/details/gqytalyly.sHtML

[T38] Lua：条件
来源：http://www.blog.epnwcf.com/Article/details/glcgyimyf.sHtML

if x > 0 then print("正") end
来源：http://wap.bbcook.cn/Article/details/gbyiabwxd.sHtML

[T39] Lua：模式匹配
来源：http://mobile.vehdjk.com/Article/details/gbsfymjzb.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/gubktkznq.sHtML

[T40] Lua：元表
来源：http://baike.fktsv.cn/Article/details/gyurafyab.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/gdtzbqwxk.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gycufkjly.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/ggbtymbfv.sHtML

[T42] Perl：变量类型
来源：http://baike.tarul.cn/Article/details/grvsugppy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/gqupcfujh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gcunseyix.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gdtqngmwo.sHtML

[T44] Perl：条件
来源：http://3g.vehdjk.com/Article/details/golpzwuck.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gtlrfsnyt.sHtML

[T45] Perl：数组遍历
来源：http://m.share.vehdjk.com/Article/details/gbxpjublg.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gxgmnystz.sHtML

[T46] Perl：哈希操作
来源：http://m.share.bbcook.cn/Article/details/guvhyxcmz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/gcroxydpt.sHtML

[T47] Perl：正则捕获
来源：http://3g.epnwcf.com/Article/details/gcumjslhb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gkhkeltnc.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/ggfnclxyq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.bbcook.cn/Article/details/gsevjygbd.sHtML

[T49] Perl：函数
来源：http://3g.bbcook.cn/Article/details/gbpiplwds.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gjgpsykuv.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/ggqtgshxn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gakhojkec.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/ghlsjrrwy.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gnnizqfyo.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gdzkqpbcc.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gnraekxhj.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gwlyhudqg.sHtML

[T53] Scala：字符串插值
来源：http://www.share.vehdjk.com/Article/details/guzwpzelj.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gqayiwbns.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/ggzvdbobm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gdwdonryg.sHtML

[T55] Scala：集合过滤
来源：http://baike.yfazqb.com/Article/details/gjduivzdf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.vehdjk.com/Article/details/gvchlhehb.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/gtwctfmib.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fktsv.cn/Article/details/gojadqmop.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/grpmxrdcu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gsdblneyl.sHtML

[T58] Scala：函数定义
来源：http://wap.fktsv.cn/Article/details/gmonbqcbj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fktsv.cn/Article/details/gwyqipxih.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gskjwilcn.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gpswltcua.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gyatvrkvd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gjwlpgpgm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpjckmkhd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gkeumomzr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggilpiuku.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.vehdjk.com/Article/details/gvtprkors.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.bbcook.cn/Article/details/guamhezen.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.fktsv.cn/Article/details/gqgoxjhhc.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gjthkgonb.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuiaulze.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.epnwcf.com/Article/details/gwnwzgblw.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/ggvcheovf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gybpobtht.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.tarul.cn/Article/details/gegshuzzn.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gzpspwsbu.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.bbcook.cn/Article/details/gfqvbzfvb.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/ghhmqvowv.sHtML

[U07] Py：反转字典键值
来源：http://m.share.tarul.cn/Article/details/gtjckcsap.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gxngjopal.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/gweasbhmu.sHtML

[y for x in nested for y in x]
来源：http://read.share.epnwcf.com/Article/details/gldcwryuu.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/glkbxemut.sHtML

max(d, key=d.get)
来源：http://wap.bbcook.cn/Article/details/gecyjkfop.sHtML

[U10] Py：按值排序字典
来源：http://blog.yfazqb.com/Article/details/gsxwzrbbs.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.vehdjk.com/Article/details/grbvfkiab.sHtML

[U11] Py：生成器表达式
来源：http://www.blog.tarul.cn/Article/details/gsyhskzhi.sHtML

(x * 2 for x in arr)
来源：http://read.share.sjlbkw.cn/Article/details/gzgualxmy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.sjlbkw.cn/Article/details/gkyjamqpp.sHtML

Counter(arr).most_common(3)
来源：http://m.share.yfazqb.com/Article/details/gjbsgkgmk.sHtML

[U13] Py：固定长度队列
来源：http://www.share.fktsv.cn/Article/details/gmvcbsbcf.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gxykhtctd.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.yfazqb.com/Article/details/gtdmnsavz.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gjtmxotws.sHtML

[U15] Py：高精度计时
来源：http://wap.fktsv.cn/Article/details/gvkujtvxr.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gvisuhvhd.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/glmyfdmid.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/gjnkdiesk.sHtML

[U17] Py：初始化日志
来源：http://baike.epnwcf.com/Article/details/gpfvhsmyi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.tarul.cn/Article/details/ghnheuzlj.sHtML

[U18] Py：预编译正则
来源：http://www.blog.tarul.cn/Article/details/gfdrxpnuj.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/ghbulxdub.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.yfazqb.com/Article/details/gltekblof.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gddfmsdnz.sHtML

[U20] Py：缓存函数结果
来源：http://wap.fktsv.cn/Article/details/ggcwsodbd.sHtML

@functools.lru_cache(maxsize=None)
来源：http://wap.bbcook.cn/Article/details/gaaxfsesl.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gatwofwvp.sHtML

@contextlib.contextmanager
来源：http://read.share.epnwcf.com/Article/details/gknqeqili.sHtML

[U22] Py：矩阵转置
来源：http://baike.bbcook.cn/Article/details/gdwedovwb.sHtML

list(zip(*m))
来源：http://www.blog.yfazqb.com/Article/details/goanzghoy.sHtML

[U23] Py：分块读取大文件
来源：http://wap.vehdjk.com/Article/details/gttqpbgqq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mobile.bbcook.cn/Article/details/gaajibvjs.sHtML

[U24] Py：路径操作
来源：http://mobile.epnwcf.com/Article/details/gspuyafsl.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gletbzlab.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.sjlbkw.cn/Article/details/gyznzrfab.sHtML

csv.DictReader(f)
来源：http://mobile.fktsv.cn/Article/details/gavefisqt.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/gjldlizer.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/giaprxbem.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.vehdjk.com/Article/details/ghqemnpbj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/gaqzlyvhb.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gdodvqjxw.sHtML

UserId = int
来源：http://baike.sjlbkw.cn/Article/details/gjaluhvqc.sHtML

[U29] Py：属性校验
来源：http://www.share.epnwcf.com/Article/details/gtmkpnuxz.sHtML

@property 与 @x.setter 配合
来源：http://read.share.sjlbkw.cn/Article/details/geemsisnf.sHtML

[U30] Py：数据类
来源：http://www.blog.fktsv.cn/Article/details/gyetdkiqn.sHtML

@dataclass(slots=True)
来源：http://wap.fktsv.cn/Article/details/gyxfhjcfe.sHtML

[U31] Py：单测
来源：http://www.share.vehdjk.com/Article/details/gfqeirwzu.sHtML

python -m pytest -q
来源：http://read.share.tarul.cn/Article/details/gorcechws.sHtML

[U32] Py：代码格式化
来源：http://www.share.yfazqb.com/Article/details/gqicbmhld.sHtML

ruff format . && ruff check --fix .
来源：http://baike.tarul.cn/Article/details/gkouuqmom.sHtML

[U33] Py：打包发布
来源：http://baike.yfazqb.com/Article/details/gybhxynky.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gyrnhrwsb.sHtML

[U34] Py：判断编码
来源：http://blog.yfazqb.com/Article/details/gfjzfjxek.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gvahjjmom.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gsiugvoku.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.tarul.cn/Article/details/gtyffpxdg.sHtML

[U36] Py：定时任务
来源：http://blog.tarul.cn/Article/details/gfucmcciv.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.bbcook.cn/Article/details/guvmrugxi.sHtML

[U37] Py：读写 Excel
来源：http://3g.epnwcf.com/Article/details/gwucpetzn.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.bbcook.cn/Article/details/gbgdzhylz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/gucimaryh.sHtML

Path(__file__).resolve().parent
来源：http://baike.epnwcf.com/Article/details/gqawpzlvh.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gskgssqkv.sHtML

sys.stdout.isatty()
来源：http://read.share.fktsv.cn/Article/details/grfkyfzwt.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/gjodykkea.sHtML

print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gnfdidzfn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fktsv.cn/Article/details/gpxebtdnd.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gkvkcdpkq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gexbomuhn.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gglcfjxvo.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.vehdjk.com/Article/details/gpjkrfqvk.sHtML

namespace App\Http;
来源：http://read.share.tarul.cn/Article/details/gyjsstpfz.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fktsv.cn/Article/details/ggzuownkz.sHtML

declare(strict_types=1);
来源：http://blog.sjlbkw.cn/Article/details/gzjkqpyds.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.epnwcf.com/Article/details/gmzzatjwr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gkcjtkpco.sHtML

[U46] PHP：可空类型
来源：http://3g.bbcook.cn/Article/details/gshtdyxau.sHtML

?string $name = null
来源：http://mobile.tarul.cn/Article/details/gdnsmdiwo.sHtML

[U47] PHP：联合类型
来源：http://read.share.tarul.cn/Article/details/glkkxhodh.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/gsdrorhwx.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gkebyitmx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.epnwcf.com/Article/details/gxiicgonc.sHtML

[U49] PHP：只读属性
来源：http://m.share.yfazqb.com/Article/details/gwybfxxzc.sHtML

public readonly string $name
来源：http://www.share.tarul.cn/Article/details/gmhhukehz.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/guxnxactz.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fktsv.cn/Article/details/gwcnrtkch.sHtML

[U51] PHP：数组解构
来源：http://www.blog.fktsv.cn/Article/details/getqbpmlo.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gjhqodhgb.sHtML

[U52] PHP：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gpmlqzinu.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/gsezwduqy.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gpathahor.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.tarul.cn/Article/details/gcklmtrzc.sHtML

[U54] PHP：空安全调用
来源：http://m.share.yfazqb.com/Article/details/gpnplokxx.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gmxagdwpd.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gyshwswym.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gfcgplwwp.sHtML

[U56] PHP：命名参数
来源：http://m.share.epnwcf.com/Article/details/gwkmnmrtl.sHtML

f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gfgywujgz.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.epnwcf.com/Article/details/gsqbehmyh.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/gggxatszy.sHtML

[U58] PHP：数组三件套
来源：http://wap.bbcook.cn/Article/details/gtwarvewr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.bbcook.cn/Article/details/gdzbekxub.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gvultcauc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/gxpvtiqlr.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.bbcook.cn/Article/details/gzznfddcr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.epnwcf.com/Article/details/gqkfuqnwj.sHtML

[U61] PHP：正则
来源：http://m.share.fktsv.cn/Article/details/gmqgxoreg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gjdzhncag.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/gjkxxiwup.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/giijokrjw.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gjrtbpawi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.epnwcf.com/Article/details/gohsrscrf.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/givjygsks.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.bbcook.cn/Article/details/gthpazshq.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gmprrnxaq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.bbcook.cn/Article/details/gwivaearw.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.bbcook.cn/Article/details/gejurxwui.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gitzmaaql.sHtML

[U67] PHP：处理文件上传
来源：http://3g.tarul.cn/Article/details/gmbnzzsfg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.vehdjk.com/Article/details/gcetccxtm.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.fktsv.cn/Article/details/gwbbkqfdw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.vehdjk.com/Article/details/gezeheeie.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.tarul.cn/Article/details/gydfubzwk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.bbcook.cn/Article/details/gtftacygq.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.yfazqb.com/Article/details/geadwlbma.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.epnwcf.com/Article/details/ggyanwgsl.sHtML

[U71] PHP：抛出异常
来源：http://baike.vehdjk.com/Article/details/goklwocln.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.vehdjk.com/Article/details/guptlspgo.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gsabfeavn.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.vehdjk.com/Article/details/grackwjmi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.vehdjk.com/Article/details/gbdxurdyh.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gikstxond.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gjzwzfxdy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.vehdjk.com/Article/details/gusozhiay.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.fktsv.cn/Article/details/goovarnvf.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gqhsrusmn.sHtML

[U76] PHP：简单路由
来源：http://blog.tarul.cn/Article/details/gidhhdbta.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gaxyxykzz.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.tarul.cn/Article/details/gvkamtfmu.sHtML

composer require twig/twig
来源：http://www.share.vehdjk.com/Article/details/gmtkfqzvo.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gfyzemqcu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/gxcgcejgx.sHtML

[U79] PHP：静态分析
来源：http://wap.vehdjk.com/Article/details/gdtivexmd.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.fktsv.cn/Article/details/gnhmeashp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fktsv.cn/Article/details/gpcorbdwq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gceptqzin.sHtML

[U81] JS：初始化项目
来源：http://mobile.epnwcf.com/Article/details/gjdkldbhx.sHtML

npm init -y;  npm i express
来源：http://www.share.bbcook.cn/Article/details/gqppgzixe.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fktsv.cn/Article/details/gdfvfqvad.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.sjlbkw.cn/Article/details/gyzrufura.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.yfazqb.com/Article/details/grwyjisye.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gkuhorjfn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.sjlbkw.cn/Article/details/gcxzfnukc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/ghvmprooi.sHtML

[U85] JS：可选链
来源：http://blog.sjlbkw.cn/Article/details/groyaentq.sHtML

a?.b?.c
来源：http://mobile.bbcook.cn/Article/details/garukwodw.sHtML

[U86] JS：空值合并
来源：http://read.share.epnwcf.com/Article/details/gtksjttiv.sHtML

a ?? b
来源：http://m.share.vehdjk.com/Article/details/gxqqdolwe.sHtML

[U87] JS：解构默认值
来源：http://m.share.yfazqb.com/Article/details/gvlsiluhh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gtrrozsza.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.tarul.cn/Article/details/gakdkixqk.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gmmclxjnn.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gvtkazaki.sHtML

[...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gedaicnjg.sHtML

[U90] JS：数字数组排序
来源：http://blog.yfazqb.com/Article/details/gynnnttgp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gpkwoctqm.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.sjlbkw.cn/Article/details/ghoapczwm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.sjlbkw.cn/Article/details/gfdgwsoca.sHtML

[U92] JS：深拷贝
来源：http://www.share.vehdjk.com/Article/details/geigjroyx.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gtvkicopz.sHtML

[U93] JS：模板字符串
来源：http://www.blog.yfazqb.com/Article/details/gvcjnxtuq.sHtML

`共 ${n} 条`
来源：http://www.blog.vehdjk.com/Article/details/gyvjjfrpj.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gpwtustxv.sHtML

const double = x => x * 2;
来源：http://www.blog.bbcook.cn/Article/details/gnhouqpry.sHtML

[U95] JS：Promise 包装
来源：http://wap.yfazqb.com/Article/details/gqpdddbxy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.epnwcf.com/Article/details/gnkalzmmt.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.vehdjk.com/Article/details/ghlvmvayr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gfuhubucy.sHtML

[U97] JS：并发请求
来源：http://blog.epnwcf.com/Article/details/gstwuebst.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/grdmephpo.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.tarul.cn/Article/details/ghpdxruzq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.yfazqb.com/Article/details/gtegucpfu.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/gpxlyezcc.sHtML

el.addEventListener("click", e => {})
来源：http://blog.bbcook.cn/Article/details/gxsuqjghh.sHtML

[U100] JS：DOM 查询
来源：http://read.share.epnwcf.com/Article/details/glpxzkupc.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gewdqupzf.sHtML

[U101] JS：classList 操作
来源：http://www.blog.yfazqb.com/Article/details/gzkvuhhmj.sHtML

el.classList.toggle("active")
来源：http://www.blog.vehdjk.com/Article/details/gfdbiwsct.sHtML

[U102] JS：本地存储
来源：http://read.share.tarul.cn/Article/details/gbuanxufl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.tarul.cn/Article/details/gqqytycwf.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/gllifkxel.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/gfmcuunxd.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/ghpnqslva.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gxyvqtelk.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gtwjfguao.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fktsv.cn/Article/details/grqodfocc.sHtML

[U106] JS：日期格式化
来源：http://wap.bbcook.cn/Article/details/gxpzdbfnb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.vehdjk.com/Article/details/gfaeyxhfx.sHtML

[U107] JS：数字千分位
来源：http://wap.yfazqb.com/Article/details/guzynmobz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gzjddguhx.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/glkrpexco.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.vehdjk.com/Article/details/gtpbndjka.sHtML

[U109] JS：数组分组
来源：http://wap.yfazqb.com/Article/details/gveosbwlx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gpizrzslx.sHtML

[U110] JS：数组分块
来源：http://blog.tarul.cn/Article/details/gxakhcvyj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/gzelmuitm.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gejoglall.sHtML

new Map(Object.entries(obj))
来源：http://blog.sjlbkw.cn/Article/details/gwiblgsvg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/gqghsfazp.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gltxzoivk.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/gzftsmahi.sHtML

s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gksxhjgrw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gjgiicres.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/ggocqgzdf.sHtML

[U115] JS：生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gbvistrsz.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gjmyrayxq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.epnwcf.com/Article/details/gfkkfugqi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.yfazqb.com/Article/details/glifrabtu.sHtML


<!-- 参考信息 -->