代发 wailian999

[T35] Lua：字典表
来源：http://mfv.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://fcm.yueranfly.top

[T36] Lua：函数
来源：http://arg.tarul.cn

function add(a, b) return a + b end
来源：http://muu.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://zsu.vehdjk.com

"a" .. "b"
来源：http://ise.zhixingplan.top

[T38] Lua：条件
来源：http://ldl.jinqigfzy.top

if x > 0 then print("正") end
来源：http://hzg.svipenyu.cn

[T39] Lua：模式匹配
来源：http://xps.sufxvd.cn

string.find(s, "%d+")
来源：http://qbt.hfpthk.cn

[T40] Lua：元表
来源：http://vas.ydzc1.top

setmetatable({}, { __index = base })
来源：http://zqv.aibaodan.cn

[T41] Perl：Hello World
来源：http://upe.xingfuxueyuan.xyz

print "Hello\n";
来源：http://giw.yj202588.top

[T42] Perl：变量类型
来源：http://kbw.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zsj.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://iuo.gogol.net.cn

"值: $a"
来源：http://prz.fktsv.cn

[T44] Perl：条件
来源：http://bwc.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://xqz.cashguo.top

[T45] Perl：数组遍历
来源：http://yxa.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://dac.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://khy.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xnc.yangfankeji.com

[T47] Perl：正则捕获
来源：http://dak.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zbm.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://lsl.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://zxh.havefunace.top

[T49] Perl：函数
来源：http://pjd.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nfv.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://jtb.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fcu.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://gtb.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://phy.shzxlz.cn

println("Hello")
来源：http://aqe.nanxinkj.top

[T52] Scala：变量
来源：http://utg.vehdjk.com

val a = 1;  var b = 2
来源：http://pkx.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://etv.bbcook.cn

s"值: $b"
来源：http://tna.hammf.cn

[T54] Scala：集合映射
来源：http://ehf.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://tuv.iojbl.cn

[T55] Scala：集合过滤
来源：http://hxm.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://qyt.aibaodan.cn

[T56] Scala：样例类
来源：http://xke.gogol.net.cn

case class User(name: String, age: Int)
来源：http://duv.uphjek.com

[T57] Scala：模式匹配
来源：http://yrt.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ypb.52xcode.cn

[T58] Scala：函数定义
来源：http://hol.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://fgs.jlsjyb.cn

[T59] Scala：循环
来源：http://ezu.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://inb.jianghu66.top

[T60] Scala：折叠
来源：http://eiz.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://meu.feifeiyinyue.top

================================================================================
来源：http://ykv.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eaz.shangyingyoupin.top

================================================================================
来源：http://oap.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://tpd.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vay.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://dja.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://eix.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://veu.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rav.yongpay.top

[U04] Py：变量调试打印
来源：http://wzy.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://buv.daria6918.cn

[U05] Py：列表去重且保序
来源：http://avo.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://ntx.ppjwa.cn

[U06] Py：合并两个字典
来源：http://hjk.jiagoushi.top

{**a, **b}
来源：http://fxx.dianchejie.cn

[U07] Py：反转字典键值
来源：http://ysp.jqgufenzy.top

{v: k for k, v in d.items()}
来源：http://fbe.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://nbp.yvedp.cn

[y for x in nested for y in x]
来源：http://yif.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://rga.quarkkingdee.top

max(d, key=d.get)
来源：http://qhm.jiagoushi.top

[U10] Py：按值排序字典
来源：http://pux.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ohv.316326.xyz

[U11] Py：生成器表达式
来源：http://vnw.smart0.xyz

(x * 2 for x in arr)
来源：http://fxl.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uuq.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://iuz.chenzaomai.com

[U13] Py：固定长度队列
来源：http://uvr.zycfv.cn

deque(maxlen=10)
来源：http://lkr.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://qdb.guowangkeji.top

defaultdict(list)
来源：http://beh.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://jlq.yfazqb.com

t = time.perf_counter()
来源：http://ngy.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://rvp.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kjt.jiagoushi.top

[U17] Py：初始化日志
来源：http://jzi.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://pmd.yvedp.cn

[U18] Py：预编译正则
来源：http://fqv.c1oappe.top

pat = re.compile(r"\d+")
来源：http://cgz.hnqzz.top

[U19] Py：正则替换带回调
来源：http://ndk.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qtk.uphjek.com

[U20] Py：缓存函数结果
来源：http://emr.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://mtv.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://zpx.nanxinkj.top

@contextlib.contextmanager
来源：http://moz.meibo888.top

[U22] Py：矩阵转置
来源：http://njr.xuanzx.com

list(zip(*m))
来源：http://vnz.ivvv.top

[U23] Py：分块读取大文件
来源：http://bnb.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://psu.yj20258.top

[U24] Py：路径操作
来源：http://iut.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fvy.hammf.cn

[U25] Py：CSV 按字典读
来源：http://xyg.yj202588.top

csv.DictReader(f)
来源：http://dop.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://kcy.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nyq.ybcxt.top

[U27] Py：异步 HTTP
来源：http://nrx.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://pxy.daxiang520.top

[U28] Py：类型别名
来源：http://bcm.chenjidiqi.icu

UserId = int
来源：http://yrv.jlsjyb.cn

[U29] Py：属性校验
来源：http://lwx.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://mho.yfazqb.com

[U30] Py：数据类
来源：http://kaj.hysaishi.cn

@dataclass(slots=True)
来源：http://hfz.hfpthk.cn

[U31] Py：单测
来源：http://dqs.redwolf501.top

python -m pytest -q
来源：http://cfb.sysykeji.top

[U32] Py：代码格式化
来源：http://sie.hammf.cn

ruff format . && ruff check --fix .
来源：http://zey.jyoumei.cn

[U33] Py：打包发布
来源：http://ela.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://qmi.hammf.cn

[U34] Py：判断编码
来源：http://pio.sufxvd.cn

chardet.detect(raw)
来源：http://nug.zhongyouzk.top

[U35] Py：发送邮件
来源：http://fxc.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://boh.svipenyu.cn

[U36] Py：定时任务
来源：http://our.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://ytt.meibo888.top

[U37] Py：读写 Excel
来源：http://zro.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://cdh.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://vqx.yongpay.top

Path(__file__).resolve().parent
来源：http://rlj.guannengcc.top

[U39] Py：判断是否在交互环境
来源：http://mse.sweek.top

sys.stdout.isatty()
来源：http://uak.zhijiandao.cn

[U40] Py：打印到标准错误
来源：http://smo.jqgufenzy.top

print("err", file=sys.stderr)
来源：http://fpx.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://znz.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jcb.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://pyf.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://avo.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://jwx.yanxiufei.cn

namespace App\Http;
来源：http://zxg.c1oappe.top

[U44] PHP：开启严格类型
来源：http://xzj.yj202588.top

declare(strict_types=1);
来源：http://rmx.52xcode.cn

[U45] PHP：类型声明与返回类型
来源：http://dqe.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://fcw.hywenlv.cn

[U46] PHP：可空类型
来源：http://eds.ctjpmb.com

?string $name = null
来源：http://ykf.zhixingplan.top

[U47] PHP：联合类型
来源：http://qxh.iojbl.cn

int|string $id
来源：http://eqm.chenzaomai.com

[U48] PHP：纯枚举
来源：http://mdf.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nqi.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://qzq.chenlongwang.top

public readonly string $name
来源：http://oky.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://gfc.fktsv.cn

public function __construct(private int $id) {}
来源：http://sbh.sjlbkw.cn

[U51] PHP：数组解构
来源：http://eke.gaohongyu789.top

[$a, $b] = $arr;
来源：http://yas.yj202588.top

[U52] PHP：箭头函数
来源：http://iqv.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://otz.quarkkingdee.top

[U53] PHP：空合并运算符
来源：http://mwo.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://irg.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://pmw.fktsv.cn

$obj?->method()
来源：http://viv.tianlin.xyz

[U55] PHP：match 表达式
来源：http://nwb.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rfa.yj20258888.top

[U56] PHP：命名参数
来源：http://gzu.jqgufenzy.top

f(a: 1, b: 2)
来源：http://zku.0kj1m.cn

[U57] PHP：字符串插值
来源：http://uyr.iojbl.cn

"值: {$a}"
来源：http://iyh.fanxiaobao.xyz

[U58] PHP：数组三件套
来源：http://qxz.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hlp.fanxiaobao.xyz

[U59] PHP：自定义排序
来源：http://npb.guowangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lhq.guowangkeji.top

[U60] PHP：JSON 编解码
来源：http://ynv.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wvq.yuanzhike.top

[U61] PHP：正则
来源：http://saq.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qnr.yonumen.top

[U62] PHP：日期对象
来源：http://qys.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kpx.ppjwa.cn

[U63] PHP：文件读写
来源：http://uzz.fktsv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fwq.yanxiufei.cn

[U64] PHP：目录遍历
来源：http://vdq.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://feg.birdmap.top

[U65] PHP：会话
来源：http://lei.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://etp.bbcook.cn

[U66] PHP：设置 Cookie
来源：http://wpn.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hmt.uphjek.com

[U67] PHP：处理文件上传
来源：http://giy.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bev.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://pao.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ifu.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://zfh.zhixingplan.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://imi.pycfn.com

[U70] PHP：PDO 事务
来源：http://aeg.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xdo.316326.xyz

[U71] PHP：抛出异常
来源：http://ubp.shzxlz.cn

throw new RuntimeException("失败", 500);
来源：http://lsq.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://zuo.zdqjudy.top

error_log("失败: " . $e->getMessage());
来源：http://jgc.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://clw.uphjek.com

parse_ini_file("config.ini", true)
来源：http://qof.nwbrower.top

[U74] PHP：读取环境变量
来源：http://hok.yfazqb.com

getenv("APP_ENV") ?: "production"
来源：http://eyk.yongpay.top

[U75] PHP：依赖注入
来源：http://gtx.pengpengdd.cyou

composer require psr/container
来源：http://vgm.xuanzx.com

[U76] PHP：简单路由
来源：http://skk.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://juh.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://cpz.tarul.cn

composer require twig/twig
来源：http://cmn.yvedp.cn

[U78] PHP：单元测试
来源：http://moj.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://lfz.cucudq.cn

[U79] PHP：静态分析
来源：http://liq.hnxiangtu.top

composer require --dev phpstan/phpstan
来源：http://mey.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://lfp.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hvv.nwbrower.top

[U81] JS：初始化项目
来源：http://jlf.snrcjt.cn

npm init -y;  npm i express
来源：http://ozv.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://urn.ydzc1.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kik.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://qvm.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://clt.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://xsz.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zzf.zhoulong.xyz

[U85] JS：可选链
来源：http://vtj.yuanzhike.top

a?.b?.c
来源：http://eio.yangfankeji.com

[U86] JS：空值合并
来源：http://vbx.wangdashe.top

a ?? b
来源：http://kku.cqqwz.cn

[U87] JS：解构默认值
来源：http://apb.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://jvr.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://lax.havefunace.top

{ ...a, ...b }
来源：http://jyc.hammf.cn

[U89] JS：数组去重
来源：http://iho.hnxiangtu.top

[...new Set(arr)]
来源：http://ath.tian-w.cn

[U90] JS：数字数组排序
来源：http://cof.sxryk.cn

[...arr].sort((a, b) => a - b)
来源：http://xhd.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://mjq.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zex.nwbrower.top

[U92] JS：深拷贝
来源：http://swz.svipenyu.cn

structuredClone(obj)
来源：http://qdd.ydzc1.top

[U93] JS：模板字符串
来源：http://umm.yanxiufei.cn

`共 ${n} 条`
来源：http://xte.cdnleiting.top

[U94] JS：箭头函数
来源：http://nst.sweek.top

const double = x => x * 2;
来源：http://gku.smart0.xyz

[U95] JS：Promise 包装
来源：http://unk.yj202588.top

new Promise((resolve, reject) => {})
来源：http://dgd.shanyushiyangtech.top

[U96] JS：async/await 与异常
来源：http://fpw.zycfv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pom.jiagoushi.top

[U97] JS：并发请求
来源：http://xcf.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://auu.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://kiq.fengsongda.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eoq.zdqjudy.top

[U99] JS：事件监听
来源：http://uop.redwolf501.top

el.addEventListener("click", e => {})
来源：http://qjl.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://dig.dashuyun.cn

document.querySelector(".item")
来源：http://ebs.9152youxi.cn

[U101] JS：classList 操作
来源：http://btu.52xcode.cn

el.classList.toggle("active")
来源：http://arr.jinqigufen.top

[U102] JS：本地存储
来源：http://ofh.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://rpy.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://iro.ybcxt.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gej.hcnkem.com

[U104] JS：防抖
来源：http://bqp.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xkm.xuanzx.com

[U105] JS：节流
来源：http://mid.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qzk.ydjk.org.cn

[U106] JS：日期格式化
来源：http://ifh.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cvd.vqdsnc.cn

[U107] JS：数字千分位
来源：http://gmi.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ian.zhijiandao.cn

[U108] JS：随机整数
来源：http://mrn.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sqn.sjlbkw.cn

[U109] JS：数组分组
来源：http://ivy.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://mgg.c1oappe.top

[U110] JS：数组分块
来源：http://tuz.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eus.hywenlv.cn

[U111] JS：对象转 Map
来源：http://gfr.yvedp.cn

new Map(Object.entries(obj))
来源：http://hst.hnxiangtu.top

[U112] JS：字符串补位
来源：http://fpi.zhengqikj.top

"7".padStart(3, "0")
来源：http://awe.mhx1999.top

[U113] JS：正则替换全部
来源：http://lrj.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://yan.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://kxe.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mjo.yj20258.top

[U115] JS：生成 UUID
来源：http://ttm.bbcook.cn

crypto.randomUUID()
来源：http://jes.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://olp.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://auw.sufxvd.cn

[U117] JS：单元测试
来源：http://jer.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://znz.gogol.net.cn

[U118] JS：开发服务器
来源：http://frv.nwbrower.top

npm i -D vite;  npx vite
来源：http://bok.fehbvm.com

[U119] JS：生产构建
来源：http://wvy.fengsongda.top

npx vite build
来源：http://npf.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://grc.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://vye.hnqzz.top

================================================================================
来源：http://tpt.zhijiandao.cn

统计汇总
来源：http://oaz.ywan-chungtsiang.top

================================================================================
来源：http://czw.bjfxy.top

按语言统计（条）：
来源：http://nen.zhoulong.xyz


<!-- 参考信息 -->