代发 wailian999

[T39] Lua：模式匹配
来源：http://gea.aizwys.cn

string.find(s, "%d+")
来源：http://mrr.jlsjyb.cn

[T40] Lua：元表
来源：http://yyo.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://rfb.ppjwa.cn

[T41] Perl：Hello World
来源：http://kcm.ydzc1.top

print "Hello\n";
来源：http://tfg.mhx1999.top

[T42] Perl：变量类型
来源：http://ewq.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://odc.yongpay.top

[T43] Perl：字符串插值
来源：http://eqx.ybcxt.top

"值: $a"
来源：http://bia.ybcxt.top

[T44] Perl：条件
来源：http://bnc.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://gxe.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://xyn.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://pbz.sysykeji.top

[T46] Perl：哈希操作
来源：http://mpe.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ayk.aizwys.cn

[T47] Perl：正则捕获
来源：http://iot.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cwy.snrcjt.cn

[T48] Perl：正则替换
来源：http://thg.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://cqt.yj20258888.top

[T49] Perl：函数
来源：http://pug.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qzu.52xcode.cn

[T50] Perl：逐行读文件
来源：http://rap.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wpg.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://epk.gaohongyu789.top

[T51] Scala：Hello World
来源：http://hga.wangdashe.top

println("Hello")
来源：http://dlf.cdnleiting.top

[T52] Scala：变量
来源：http://qne.zhongyouzk.top

val a = 1;  var b = 2
来源：http://sef.fzhhl.top

[T53] Scala：字符串插值
来源：http://ckb.kuanghao11.cn

s"值: $b"
来源：http://tji.dashuyun.cn

[T54] Scala：集合映射
来源：http://nyv.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://wjn.xylfe.cn

[T55] Scala：集合过滤
来源：http://vfw.aizwys.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gnl.yangfankeji.com

[T56] Scala：样例类
来源：http://qzv.xziqi.cn

case class User(name: String, age: Int)
来源：http://bdg.yj20258.top

[T57] Scala：模式匹配
来源：http://ywe.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ijr.c1oappe.top

[T58] Scala：函数定义
来源：http://hux.yongpay.top

def add(a: Int, b: Int): Int = a + b
来源：http://mlm.zhengqikj.top

[T59] Scala：循环
来源：http://uze.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://gtq.vehdjk.com

[T60] Scala：折叠
来源：http://dal.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fye.ivvv.top

================================================================================
来源：http://ilh.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ofi.mhx1999.top

================================================================================
来源：http://ofo.jinqigfzy.top

[U01] Py：创建虚拟环境
来源：http://tgw.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://apv.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://wyo.zdqjudy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qts.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://loo.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://lyd.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://kiu.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bnz.yj20258.top

[U05] Py：列表去重且保序
来源：http://ybl.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://vpf.ivvv.top

[U06] Py：合并两个字典
来源：http://yjl.cucudq.cn

{**a, **b}
来源：http://jkt.svipenyu.cn

[U07] Py：反转字典键值
来源：http://dfp.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://ygs.fktsv.cn

[U08] Py：展平二维列表
来源：http://okc.nanxuanxn.top

[y for x in nested for y in x]
来源：http://bfp.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://mbz.jinqigfzy.top

max(d, key=d.get)
来源：http://fiq.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://fvo.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tnl.haohaochexian.top

[U11] Py：生成器表达式
来源：http://qzc.zhaomingkeji.xyz

(x * 2 for x in arr)
来源：http://bed.ywan-chungtsiang.top

[U12] Py：取出现最多的 3 个元素
来源：http://bgz.aizwys.cn

Counter(arr).most_common(3)
来源：http://iqy.bjfxy.top

[U13] Py：固定长度队列
来源：http://xjd.nwbrower.top

deque(maxlen=10)
来源：http://lvz.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://dmv.meibo888.top

defaultdict(list)
来源：http://exb.yongpay.top

[U15] Py：高精度计时
来源：http://lrq.zdqjudy.top

t = time.perf_counter()
来源：http://rjy.xinyue.icu

[U16] Py：命令行参数解析
来源：http://dcb.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xgh.redwolf501.top

[U17] Py：初始化日志
来源：http://zzc.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://oki.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://den.ctjpmb.com

pat = re.compile(r"\d+")
来源：http://leh.hnqzz.top

[U19] Py：正则替换带回调
来源：http://egw.aibaodan.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jjt.jianghu66.top

[U20] Py：缓存函数结果
来源：http://kvt.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://nxs.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://evr.xuetiantiany.cn

@contextlib.contextmanager
来源：http://wqj.jinqigufen.top

[U22] Py：矩阵转置
来源：http://hls.daxiang520.top

list(zip(*m))
来源：http://gyp.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://zez.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bva.chenlongwang.top

[U24] Py：路径操作
来源：http://tef.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://srt.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://fum.zhiwuduotai.top

csv.DictReader(f)
来源：http://urs.wangshuangyany.cn

[U26] Py：并发下载
来源：http://omw.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rhr.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://sje.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://klo.52xcode.cn

[U28] Py：类型别名
来源：http://sid.wangshuangyany.cn

UserId = int
来源：http://vvo.gogol.net.cn

[U29] Py：属性校验
来源：http://jya.xuanzx.com

@property 与 @x.setter 配合
来源：http://xai.zhongyouzk.top

[U30] Py：数据类
来源：http://hfe.gaohongyu789.top

@dataclass(slots=True)
来源：http://mkw.bbcook.cn

[U31] Py：单测
来源：http://xxb.jianghu66.top

python -m pytest -q
来源：http://paz.cashguo.top

[U32] Py：代码格式化
来源：http://stg.fehbvm.com

ruff format . && ruff check --fix .
来源：http://ofb.shuidangran.top

[U33] Py：打包发布
来源：http://ogs.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://phy.316326.xyz

[U34] Py：判断编码
来源：http://hyb.nanxuanxn.top

chardet.detect(raw)
来源：http://ryv.shzxlz.cn

[U35] Py：发送邮件
来源：http://qlz.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tbr.quarkkingdee.top

[U36] Py：定时任务
来源：http://gga.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://arv.sysykeji.top

[U37] Py：读写 Excel
来源：http://gsd.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://fyb.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://rxn.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://wiw.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://fhc.bjfxy.top

sys.stdout.isatty()
来源：http://srt.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://pjm.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://qvo.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://tpw.zhoulong.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://skr.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jyv.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mvf.chenzaomai.com

[U43] PHP：声明命名空间
来源：http://pqk.jyoumei.cn

namespace App\Http;
来源：http://xdu.fktsv.cn

[U44] PHP：开启严格类型
来源：http://ywu.gotoacloud.top

declare(strict_types=1);
来源：http://vkj.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://xar.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jmx.sufxvd.cn

[U46] PHP：可空类型
来源：http://qhl.ydjk.org.cn

?string $name = null
来源：http://sqz.fehbvm.com

[U47] PHP：联合类型
来源：http://qub.fehbvm.com

int|string $id
来源：http://fan.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://mza.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zji.jiagoushi.top

[U49] PHP：只读属性
来源：http://rap.zycfv.cn

public readonly string $name
来源：http://sts.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://zvm.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://vtl.9152youxi.cn

[U51] PHP：数组解构
来源：http://yjt.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://blx.xinyue.icu

[U52] PHP：箭头函数
来源：http://cau.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://ykj.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://tmh.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://mmy.zhengqikj.top

[U54] PHP：空安全调用
来源：http://mxq.shanyushiyangtech.top

$obj?->method()
来源：http://sjp.birdmap.top

[U55] PHP：match 表达式
来源：http://gku.yanxiufei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://won.ydzc1.top

[U56] PHP：命名参数
来源：http://sqp.meibo888.top

f(a: 1, b: 2)
来源：http://lfh.zdqjudy.top

[U57] PHP：字符串插值
来源：http://otk.hesvh.cn

"值: {$a}"
来源：http://wjk.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://ljl.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fqs.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://zit.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujc.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://mmo.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wni.hfpthk.cn

[U61] PHP：正则
来源：http://vrq.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jiw.haohaochexian.top

[U62] PHP：日期对象
来源：http://kbr.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tvn.9152youxi.cn

[U63] PHP：文件读写
来源：http://xra.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fju.cashguo.top

[U64] PHP：目录遍历
来源：http://dmk.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://gdy.fzhhl.top

[U65] PHP：会话
来源：http://gew.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kky.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://iwu.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jnj.xziqi.cn

[U67] PHP：处理文件上传
来源：http://npi.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fqn.havefunace.top

[U68] PHP：PDO 连接
来源：http://txc.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dfe.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://rzy.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ihc.jinyuanbaomall.cn

[U70] PHP：PDO 事务
来源：http://htf.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ave.shuidangran.top

[U71] PHP：抛出异常
来源：http://qie.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://pcj.cashguo.top

[U72] PHP：写错误日志
来源：http://xjf.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://nle.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://cas.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://bqs.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://xjp.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://stt.chenlongwang.top

[U75] PHP：依赖注入
来源：http://kqs.zdbjq.cn

composer require psr/container
来源：http://tfj.jlsjyb.cn

[U76] PHP：简单路由
来源：http://aey.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sms.jinqigufen.top

[U77] PHP：模板渲染
来源：http://ynw.jinyuanbaomall.cn

composer require twig/twig
来源：http://mdh.0kj1m.cn

[U78] PHP：单元测试
来源：http://hzo.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://umi.yfazqb.com

[U79] PHP：静态分析
来源：http://gwl.jinghuilouyu.cn

composer require --dev phpstan/phpstan
来源：http://kmt.52xcode.cn

[U80] PHP：代码规范修复
来源：http://ypn.nanxinkj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qdm.daria6918.cn

[U81] JS：初始化项目
来源：http://cdp.cucudq.cn

npm init -y;  npm i express
来源：http://hot.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://eod.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://juq.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://wwz.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://mkw.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://pmf.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://fmi.shanyushiyangtech.top

[U85] JS：可选链
来源：http://kbn.hesvh.cn

a?.b?.c
来源：http://mbs.sjlbkw.cn

[U86] JS：空值合并
来源：http://wzs.sufxvd.cn

a ?? b
来源：http://reh.ydjk.org.cn

[U87] JS：解构默认值
来源：http://ytc.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://kzv.cdnleiting.top

[U88] JS：对象展开合并
来源：http://lzh.ehwqpu.com

{ ...a, ...b }
来源：http://pmc.hnxiangtu.top

[U89] JS：数组去重
来源：http://ulr.hysaishi.cn

[...new Set(arr)]
来源：http://gui.dianchejie.cn

[U90] JS：数字数组排序
来源：http://ihw.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://tyj.tianlin.xyz

[U91] JS：对象键值遍历
来源：http://tfp.pengpengdd.cyou

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nxh.chenlongwang.top

[U92] JS：深拷贝
来源：http://kpt.xinyue.icu

structuredClone(obj)
来源：http://hns.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://kiu.shzxlz.cn

`共 ${n} 条`
来源：http://yup.fzhhl.top

[U94] JS：箭头函数
来源：http://qok.daxiang520.top

const double = x => x * 2;
来源：http://son.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://mnt.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://kzq.sweek.top

[U96] JS：async/await 与异常
来源：http://upy.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iod.xziqi.cn

[U97] JS：并发请求
来源：http://wgn.chenjidiqi.icu

await Promise.all(urls.map(u => fetch(u)))
来源：http://otc.yfazqb.com

[U98] JS：fetch 带 JSON
来源：http://gqh.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://far.guowangkeji.top

[U99] JS：事件监听
来源：http://sat.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://jjs.zhengqikj.top

[U100] JS：DOM 查询
来源：http://jgv.jlsjyb.cn

document.querySelector(".item")
来源：http://rcr.ppjwa.cn

[U101] JS：classList 操作
来源：http://fuq.bjfxy.top

el.classList.toggle("active")
来源：http://veo.yfazqb.com

[U102] JS：本地存储
来源：http://nye.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://npi.hcnkem.com

[U103] JS：定时器
来源：http://xxb.hfpthk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kce.zhoulong.xyz

[U104] JS：防抖
来源：http://xmx.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fns.fzhhl.top

[U105] JS：节流
来源：http://dav.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nqe.gogol.net.cn

[U106] JS：日期格式化
来源：http://dqw.fehbvm.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uxh.9152youxi.cn

[U107] JS：数字千分位
来源：http://gta.gaohongyu789.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rwc.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://kwz.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gfw.yj20258.top

[U109] JS：数组分组
来源：http://ndk.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://gsp.aibaodan.cn

[U110] JS：数组分块
来源：http://hfs.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fbc.hysaishi.cn

[U111] JS：对象转 Map
来源：http://rsp.yonumen.top

new Map(Object.entries(obj))
来源：http://hfi.hnqzz.top

[U112] JS：字符串补位
来源：http://hpl.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://gbx.cqqwz.cn

[U113] JS：正则替换全部
来源：http://hgw.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://ums.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://vpp.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hpi.c1oappe.top

[U115] JS：生成 UUID
来源：http://scl.fengsongda.top

crypto.randomUUID()
来源：http://pyk.xinyue.icu

[U116] JS：类型检查（JSDoc）
来源：http://zjk.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://qca.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://icb.bjfxy.top

npm i -D vitest;  npx vitest
来源：http://zqs.ehwqpu.com

[U118] JS：开发服务器
来源：http://qto.ywan-chungtsiang.top

npm i -D vite;  npx vite
来源：http://bja.dashuyun.cn

[U119] JS：生产构建
来源：http://xlu.jinghuilouyu.cn

npx vite build
来源：http://wdd.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://edg.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://dzx.hywenlv.cn

================================================================================
来源：http://ipt.jianghu66.top

统计汇总
来源：http://qjn.jiagoushi.top

================================================================================
来源：http://unt.xylfe.cn

按语言统计（条）：
来源：http://xma.tianlin.xyz

Python ......... 252
来源：http://xth.yueranfly.top

PHP ............ 252
来源：http://trf.tianlin.xyz

JavaScript ..... 252
来源：http://epd.nanxuanxn.top

TypeScript ..... 212
来源：http://zvn.shanyushiyangtech.top

Java ........... 212
来源：http://vfz.yonumen.top

Go ............. 212
来源：http://udo.yfazqb.com

Ruby ........... 212
来源：http://fqe.hcnkem.com

C# ............. 212
来源：http://jqp.yonumen.top


<!-- 参考信息 -->