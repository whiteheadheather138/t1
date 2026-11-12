代发 wailian999

[T41] Perl：Hello World
来源：http://uwi.gotoacloud.top

print "Hello\n";
来源：http://hhu.zhoulong.xyz

[T42] Perl：变量类型
来源：http://fht.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://znj.bjfxy.top

[T43] Perl：字符串插值
来源：http://gyc.sxryk.cn

"值: $a"
来源：http://bfa.zhijiandao.cn

[T44] Perl：条件
来源：http://qot.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://aiz.havefunace.top

[T45] Perl：数组遍历
来源：http://azc.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://xjt.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://guh.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ndu.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://lxe.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://cca.yueranfly.top

[T48] Perl：正则替换
来源：http://ase.yfazqb.com

$s =~ s/old/new/g;
来源：http://vxu.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://lgu.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ohu.shuidangran.top

[T50] Perl：逐行读文件
来源：http://jfz.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ekd.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://urv.daria6918.cn

[T51] Scala：Hello World
来源：http://tko.zycfv.cn

println("Hello")
来源：http://zuj.chenzaomai.com

[T52] Scala：变量
来源：http://aod.yueranfly.top

val a = 1;  var b = 2
来源：http://bzj.ehwqpu.com

[T53] Scala：字符串插值
来源：http://ngp.ydzc1.top

s"值: $b"
来源：http://arp.ydzc1.top

[T54] Scala：集合映射
来源：http://pbu.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://ptd.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://mqr.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://vfl.yuanzhike.top

[T56] Scala：样例类
来源：http://igm.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://tvu.ydzc1.top

[T57] Scala：模式匹配
来源：http://rxg.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zhe.tarul.cn

[T58] Scala：函数定义
来源：http://xqy.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://ezl.ehwqpu.com

[T59] Scala：循环
来源：http://hwc.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://pdi.yonumen.top

[T60] Scala：折叠
来源：http://kmn.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eqg.wangshuangyany.cn

================================================================================
来源：http://uls.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fjy.hongshengwenyu.top

================================================================================
来源：http://mro.birdmap.top

[U01] Py：创建虚拟环境
来源：http://khm.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sfw.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://rwn.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dmr.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://tpd.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yoi.ybcxt.top

[U04] Py：变量调试打印
来源：http://qin.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zui.yj20258.top

[U05] Py：列表去重且保序
来源：http://wvx.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://bbx.dianchejie.cn

[U06] Py：合并两个字典
来源：http://sxv.chenjidiqi.icu

{**a, **b}
来源：http://rbb.yangfankeji.com

[U07] Py：反转字典键值
来源：http://oyr.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://qrt.xuanzx.com

[U08] Py：展平二维列表
来源：http://bhb.fktsv.cn

[y for x in nested for y in x]
来源：http://seg.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://lub.kuanghao11.cn

max(d, key=d.get)
来源：http://kam.iojbl.cn

[U10] Py：按值排序字典
来源：http://cvo.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oek.bjfxy.top

[U11] Py：生成器表达式
来源：http://muj.guannengcc.top

(x * 2 for x in arr)
来源：http://dcy.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://hku.jinqigufen.top

Counter(arr).most_common(3)
来源：http://kin.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://bcx.feifeiyinyue.top

deque(maxlen=10)
来源：http://out.xylfe.cn

[U14] Py：分组收集到列表
来源：http://rfi.sweek.top

defaultdict(list)
来源：http://cpd.guowangkeji.top

[U15] Py：高精度计时
来源：http://rzl.bbcook.cn

t = time.perf_counter()
来源：http://zzm.316326.xyz

[U16] Py：命令行参数解析
来源：http://pgn.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xol.yj20258.top

[U17] Py：初始化日志
来源：http://hui.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://uvt.ywan-chungtsiang.top

[U18] Py：预编译正则
来源：http://gaq.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://tno.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://ohc.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pah.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://zps.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://kdg.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://oue.ivvv.top

@contextlib.contextmanager
来源：http://mqz.tianlin.xyz

[U22] Py：矩阵转置
来源：http://rnl.bjfxy.top

list(zip(*m))
来源：http://kyj.nwbrower.top

[U23] Py：分块读取大文件
来源：http://luw.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mec.yongpay.top

[U24] Py：路径操作
来源：http://cal.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qai.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://qwn.cucudq.cn

csv.DictReader(f)
来源：http://jjj.yangfankeji.com

[U26] Py：并发下载
来源：http://sib.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hzp.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://uqw.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://nhn.yvedp.cn

[U28] Py：类型别名
来源：http://liu.fehbvm.com

UserId = int
来源：http://bod.vqdsnc.cn

[U29] Py：属性校验
来源：http://bkr.c1oappe.top

@property 与 @x.setter 配合
来源：http://vcd.guannengcc.top

[U30] Py：数据类
来源：http://mlu.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://ymd.yonumen.top

[U31] Py：单测
来源：http://cpy.0kj1m.cn

python -m pytest -q
来源：http://vlp.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://vwk.tanke756.top

ruff format . && ruff check --fix .
来源：http://urc.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://kat.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://efs.hammf.cn

[U34] Py：判断编码
来源：http://mdq.ywan-chungtsiang.top

chardet.detect(raw)
来源：http://moo.tianlin.xyz

[U35] Py：发送邮件
来源：http://sjp.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://inl.ppjwa.cn

[U36] Py：定时任务
来源：http://fom.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://neg.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://ljz.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://umf.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://ahs.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://qhv.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://zmi.zycfv.cn

sys.stdout.isatty()
来源：http://dus.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://smg.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://mge.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://fcb.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rlo.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://itt.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ldm.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://zhx.xuanzx.com

namespace App\Http;
来源：http://pcf.andypj.xyz

[U44] PHP：开启严格类型
来源：http://gfx.gaohongyu789.top

declare(strict_types=1);
来源：http://zct.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://zwx.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://niq.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://mdg.jlsjyb.cn

?string $name = null
来源：http://qbo.yvedp.cn

[U47] PHP：联合类型
来源：http://bpj.9152youxi.cn

int|string $id
来源：http://gwh.52xcode.cn

[U48] PHP：纯枚举
来源：http://rqm.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qfj.sweek.top

[U49] PHP：只读属性
来源：http://tby.yj20258.top

public readonly string $name
来源：http://oua.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://fmv.hammf.cn

public function __construct(private int $id) {}
来源：http://ctv.shuidangran.top

[U51] PHP：数组解构
来源：http://bvh.cdnleiting.top

[$a, $b] = $arr;
来源：http://kga.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://erp.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://vfu.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://lhn.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://tsc.cashguo.top

[U54] PHP：空安全调用
来源：http://ncd.jinqigufen.top

$obj?->method()
来源：http://fge.nanxinkj.top

[U55] PHP：match 表达式
来源：http://bcw.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://piw.redwolf501.top

[U56] PHP：命名参数
来源：http://vrz.gaohongyu789.top

f(a: 1, b: 2)
来源：http://uov.hesvh.cn

[U57] PHP：字符串插值
来源：http://ryy.jiagoushi.top

"值: {$a}"
来源：http://epf.yfazqb.com

[U58] PHP：数组三件套
来源：http://fly.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rdh.guowangkeji.top

[U59] PHP：自定义排序
来源：http://qze.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbt.kuanghao11.cn

[U60] PHP：JSON 编解码
来源：http://qvd.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hzk.yanxiufei.cn

[U61] PHP：正则
来源：http://xlu.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ata.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://gaz.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nim.nwbrower.top

[U63] PHP：文件读写
来源：http://zcd.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xkw.sufxvd.cn

[U64] PHP：目录遍历
来源：http://lho.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://fsp.jyoumei.cn

[U65] PHP：会话
来源：http://rbn.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dwu.havefunace.top

[U66] PHP：设置 Cookie
来源：http://emj.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vxa.ybcxt.top

[U67] PHP：处理文件上传
来源：http://ihx.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wpc.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://tgg.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mmy.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://tni.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qol.cucudq.cn

[U70] PHP：PDO 事务
来源：http://umf.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://evn.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://fdz.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://ebf.ctjpmb.com

[U72] PHP：写错误日志
来源：http://yea.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://fze.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://acn.aizwys.cn

parse_ini_file("config.ini", true)
来源：http://exz.shuidangran.top

[U74] PHP：读取环境变量
来源：http://dnd.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://rme.daria6918.cn

[U75] PHP：依赖注入
来源：http://tmk.zdbjq.cn

composer require psr/container
来源：http://dnm.yj20258888.top

[U76] PHP：简单路由
来源：http://iwc.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://icg.smart0.xyz

[U77] PHP：模板渲染
来源：http://kfd.ydjk.org.cn

composer require twig/twig
来源：http://woa.fanxiaobao.xyz

[U78] PHP：单元测试
来源：http://wcp.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://lof.gogol.net.cn

[U79] PHP：静态分析
来源：http://qmk.vqdsnc.cn

composer require --dev phpstan/phpstan
来源：http://srf.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://xkx.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://sfm.pycfn.com

[U81] JS：初始化项目
来源：http://gmt.svipenyu.cn

npm init -y;  npm i express
来源：http://qwq.xziqi.cn

[U82] JS：package.json 脚本
来源：http://qee.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lxy.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://dtw.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://xgr.xinyue.icu

[U84] JS：CommonJS 写法
来源：http://dak.hnqzz.top

module.exports = { a };  const { a } = require("./m");
来源：http://pnh.aizwys.cn

[U85] JS：可选链
来源：http://hiy.xylfe.cn

a?.b?.c
来源：http://vxk.hesvh.cn

[U86] JS：空值合并
来源：http://gvp.jlsjyb.cn

a ?? b
来源：http://tqi.yfazqb.com

[U87] JS：解构默认值
来源：http://wpp.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://jfg.chenzaomai.com

[U88] JS：对象展开合并
来源：http://imo.xuetiantiany.cn

{ ...a, ...b }
来源：http://xoj.ydjk.org.cn

[U89] JS：数组去重
来源：http://ppi.birdmap.top

[...new Set(arr)]
来源：http://tul.xingfuxueyuan.xyz

[U90] JS：数字数组排序
来源：http://pbz.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://daw.cashguo.top

[U91] JS：对象键值遍历
来源：http://ohy.ywan-chungtsiang.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://okq.fzhhl.top

[U92] JS：深拷贝
来源：http://swe.cheryme.top

structuredClone(obj)
来源：http://qds.jqgufenzy.top

[U93] JS：模板字符串
来源：http://oac.aibaodan.cn

`共 ${n} 条`
来源：http://mro.yvedp.cn

[U94] JS：箭头函数
来源：http://smc.uphjek.com

const double = x => x * 2;
来源：http://kws.nwbrower.top

[U95] JS：Promise 包装
来源：http://uvy.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://ngx.havefunace.top

[U96] JS：async/await 与异常
来源：http://ewj.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xnp.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://mbn.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://iea.52xcode.cn

[U98] JS：fetch 带 JSON
来源：http://cvt.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cuw.cucudq.cn

[U99] JS：事件监听
来源：http://sdp.meibo888.top

el.addEventListener("click", e => {})
来源：http://thl.tarul.cn

[U100] JS：DOM 查询
来源：http://iql.ppjwa.cn

document.querySelector(".item")
来源：http://egq.bjfxy.top

[U101] JS：classList 操作
来源：http://mwp.cashguo.top

el.classList.toggle("active")
来源：http://xcw.hysaishi.cn

[U102] JS：本地存储
来源：http://mjv.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dlw.chenjidiqi.icu

[U103] JS：定时器
来源：http://eif.tanke756.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ehc.pengpengdd.cyou

[U104] JS：防抖
来源：http://foc.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uah.gaohongyu789.top

[U105] JS：节流
来源：http://asx.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hyl.ydjk.org.cn

[U106] JS：日期格式化
来源：http://iur.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mdf.zdbjq.cn

[U107] JS：数字千分位
来源：http://ljc.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jch.xuanzx.com

[U108] JS：随机整数
来源：http://eya.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xfl.jinqigfzy.top

[U109] JS：数组分组
来源：http://twv.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://jnu.uphjek.com

[U110] JS：数组分块
来源：http://uto.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eiw.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://kuh.smart0.xyz

new Map(Object.entries(obj))
来源：http://emw.zdqjudy.top

[U112] JS：字符串补位
来源：http://atr.yuxming.cn

"7".padStart(3, "0")
来源：http://zvv.yueranfly.top

[U113] JS：正则替换全部
来源：http://wtv.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://duj.sxryk.cn

[U114] JS：JSON 深比较
来源：http://hgj.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lma.hfpthk.cn

[U115] JS：生成 UUID
来源：http://nrn.cucudq.cn

crypto.randomUUID()
来源：http://xvg.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://qpr.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://swc.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://pex.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://wsi.hysaishi.cn

[U118] JS：开发服务器
来源：http://dfo.hfpthk.cn

npm i -D vite;  npx vite
来源：http://tmc.cqqwz.cn

[U119] JS：生产构建
来源：http://sln.jinyuanbaomall.cn

npx vite build
来源：http://zzs.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://wvo.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://giu.nwbrower.top

================================================================================
来源：http://pei.52xcode.cn

统计汇总
来源：http://eps.0kj1m.cn

================================================================================
来源：http://oob.yfazqb.com

按语言统计（条）：
来源：http://qnn.jqgfzy.top

Python ......... 252
来源：http://lhi.jyoumei.cn

PHP ............ 252
来源：http://fda.vehdjk.com

JavaScript ..... 252
来源：http://pju.mhx1999.top

TypeScript ..... 212
来源：http://anu.yangfankeji.com

Java ........... 212
来源：http://lqs.tanke756.top

Go ............. 212
来源：http://oir.jinyuanbaomall.cn

Ruby ........... 212
来源：http://yao.shanyushiyangtech.top

C# ............. 212
来源：http://dml.fehbvm.com

C .............. 30
来源：http://omx.ywan-chungtsiang.top

C++ ............ 30
来源：http://bsj.zycfv.cn

SQL ............ 90
来源：http://eay.xingfuxueyuan.xyz

Bash ........... 80
来源：http://fcr.epnwcf.com


<!-- 参考信息 -->