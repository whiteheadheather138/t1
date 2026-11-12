代发 wailian999

[T39] Lua：模式匹配
来源：http://cto.sysykeji.top

string.find(s, "%d+")
来源：http://zjk.0kj1m.cn

[T40] Lua：元表
来源：http://xgq.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://lpu.chenzaomai.com

[T41] Perl：Hello World
来源：http://bct.dianchejie.cn

print "Hello\n";
来源：http://ljj.yj202588.top

[T42] Perl：变量类型
来源：http://pii.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wih.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://zmg.zhaomingkeji.xyz

"值: $a"
来源：http://hzr.chenjidiqi.icu

[T44] Perl：条件
来源：http://ato.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://sqj.cqqwz.cn

[T45] Perl：数组遍历
来源：http://ctc.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://vta.daria6918.cn

[T46] Perl：哈希操作
来源：http://kqs.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lew.hywenlv.cn

[T47] Perl：正则捕获
来源：http://fiv.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qhu.hesvh.cn

[T48] Perl：正则替换
来源：http://bvd.daxiang520.top

$s =~ s/old/new/g;
来源：http://woe.jiagoushi.top

[T49] Perl：函数
来源：http://uyx.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qbm.c1oappe.top

[T50] Perl：逐行读文件
来源：http://hku.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nso.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://xlv.yongpay.top

[T51] Scala：Hello World
来源：http://utj.fzhhl.top

println("Hello")
来源：http://mat.yongpay.top

[T52] Scala：变量
来源：http://ocj.tarul.cn

val a = 1;  var b = 2
来源：http://mcy.guowangkeji.top

[T53] Scala：字符串插值
来源：http://xlc.daxiang520.top

s"值: $b"
来源：http://zqz.vqdsnc.cn

[T54] Scala：集合映射
来源：http://hku.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://xad.redwolf501.top

[T55] Scala：集合过滤
来源：http://gyv.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wgb.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://msz.shuidangran.top

case class User(name: String, age: Int)
来源：http://ybw.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://nfj.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zgv.xinyue.icu

[T58] Scala：函数定义
来源：http://wqe.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://pxf.bbcook.cn

[T59] Scala：循环
来源：http://okw.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://lnu.316326.xyz

[T60] Scala：折叠
来源：http://qhf.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ose.zhijiandao.cn

================================================================================
来源：http://teq.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vhz.zhengqikj.top

================================================================================
来源：http://enh.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://evq.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://rnt.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://omr.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pct.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://rtb.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pfx.fktsv.cn

[U04] Py：变量调试打印
来源：http://cvd.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wko.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://wfc.yueranfly.top

list(dict.fromkeys(arr))
来源：http://spt.zycfv.cn

[U06] Py：合并两个字典
来源：http://krb.yj20258888.top

{**a, **b}
来源：http://pjs.fehbvm.com

[U07] Py：反转字典键值
来源：http://wts.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://wnm.bbcook.cn

[U08] Py：展平二维列表
来源：http://yoc.zhoulong.xyz

[y for x in nested for y in x]
来源：http://oga.tarul.cn

[U09] Py：字典取最大值的键
来源：http://qyd.hnqzz.top

max(d, key=d.get)
来源：http://sbj.ivvv.top

[U10] Py：按值排序字典
来源：http://ozv.bjfxy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cdj.shuidangran.top

[U11] Py：生成器表达式
来源：http://opt.iojbl.cn

(x * 2 for x in arr)
来源：http://wte.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://cdd.andypj.xyz

Counter(arr).most_common(3)
来源：http://ivb.guowangkeji.top

[U13] Py：固定长度队列
来源：http://epy.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://tch.fktsv.cn

[U14] Py：分组收集到列表
来源：http://wtd.xylfe.cn

defaultdict(list)
来源：http://hac.yangfankeji.com

[U15] Py：高精度计时
来源：http://dvy.guannengcc.top

t = time.perf_counter()
来源：http://wip.yonumen.top

[U16] Py：命令行参数解析
来源：http://xei.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rek.gzhubu.top

[U17] Py：初始化日志
来源：http://jvp.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://cdf.zhixingplan.top

[U18] Py：预编译正则
来源：http://ekz.hesvh.cn

pat = re.compile(r"\d+")
来源：http://kwq.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://ucu.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lyg.ehwqpu.com

[U20] Py：缓存函数结果
来源：http://bjv.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://wqz.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://tyf.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://jgx.yj20258888.top

[U22] Py：矩阵转置
来源：http://bxx.jyoumei.cn

list(zip(*m))
来源：http://ayh.shuidangran.top

[U23] Py：分块读取大文件
来源：http://fjm.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://izi.pengpengdd.cyou

[U24] Py：路径操作
来源：http://qfp.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bwy.havefunace.top

[U25] Py：CSV 按字典读
来源：http://swh.yuanzhike.top

csv.DictReader(f)
来源：http://dxt.feifeiyinyue.top

[U26] Py：并发下载
来源：http://iea.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qbg.cucudq.cn

[U27] Py：异步 HTTP
来源：http://aqt.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://uvb.sxryk.cn

[U28] Py：类型别名
来源：http://ncc.zdqjudy.top

UserId = int
来源：http://eqn.gotoacloud.top

[U29] Py：属性校验
来源：http://kdt.havefunace.top

@property 与 @x.setter 配合
来源：http://oll.zhoulong.xyz

[U30] Py：数据类
来源：http://uik.fktsv.cn

@dataclass(slots=True)
来源：http://gdw.zhongyouzk.top

[U31] Py：单测
来源：http://ltu.daria6918.cn

python -m pytest -q
来源：http://dln.quarkkingdee.top

[U32] Py：代码格式化
来源：http://ios.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://hrg.jlsjyb.cn

[U33] Py：打包发布
来源：http://qzs.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://zgc.cheryme.top

[U34] Py：判断编码
来源：http://fkc.zhoulong.xyz

chardet.detect(raw)
来源：http://est.pycfn.com

[U35] Py：发送邮件
来源：http://mbk.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://irx.nwbrower.top

[U36] Py：定时任务
来源：http://spf.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://ihz.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://tyn.ivvv.top

pandas.read_excel / DataFrame.to_excel
来源：http://bhu.yuanzhike.top

[U38] Py：获取脚本所在目录
来源：http://mna.iojbl.cn

Path(__file__).resolve().parent
来源：http://zhn.zhengqikj.top

[U39] Py：判断是否在交互环境
来源：http://xuj.52xcode.cn

sys.stdout.isatty()
来源：http://pzy.wangdashe.top

[U40] Py：打印到标准错误
来源：http://ihj.cqqwz.cn

print("err", file=sys.stderr)
来源：http://ueb.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://dur.svipenyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xdp.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://tqf.hywenlv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iya.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://fuc.gogol.net.cn

namespace App\Http;
来源：http://xrv.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://smr.guowangkeji.top

declare(strict_types=1);
来源：http://gjg.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://tdr.zhongyouzk.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://elp.daria6918.cn

[U46] PHP：可空类型
来源：http://djw.jyoumei.cn

?string $name = null
来源：http://oxd.yongpay.top

[U47] PHP：联合类型
来源：http://ubc.316326.xyz

int|string $id
来源：http://sxe.chenjidiqi.icu

[U48] PHP：纯枚举
来源：http://mik.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vyg.xziqi.cn

[U49] PHP：只读属性
来源：http://zsi.chenzaomai.com

public readonly string $name
来源：http://brp.yj202588.top

[U50] PHP：构造器属性提升
来源：http://byb.hnqzz.top

public function __construct(private int $id) {}
来源：http://vwu.ivvv.top

[U51] PHP：数组解构
来源：http://ntt.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://jkb.zycfv.cn

[U52] PHP：箭头函数
来源：http://amh.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://fsy.0kj1m.cn

[U53] PHP：空合并运算符
来源：http://oia.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://kbd.xziqi.cn

[U54] PHP：空安全调用
来源：http://gat.ivvv.top

$obj?->method()
来源：http://zma.shzxlz.cn

[U55] PHP：match 表达式
来源：http://emg.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://num.ehwqpu.com

[U56] PHP：命名参数
来源：http://uxd.hfpthk.cn

f(a: 1, b: 2)
来源：http://zcs.c1oappe.top

[U57] PHP：字符串插值
来源：http://use.hnxiangtu.top

"值: {$a}"
来源：http://npn.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://lgt.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eoh.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://xdf.shangyingyoupin.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dnt.yj20258.top

[U60] PHP：JSON 编解码
来源：http://txs.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ess.aizwys.cn

[U61] PHP：正则
来源：http://iiu.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tvx.hysaishi.cn

[U62] PHP：日期对象
来源：http://eep.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sir.quarkkingdee.top

[U63] PHP：文件读写
来源：http://goj.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lod.fehbvm.com

[U64] PHP：目录遍历
来源：http://yds.yanxiufei.cn

glob("dir/*.php");  scandir("dir");
来源：http://umf.daxiang520.top

[U65] PHP：会话
来源：http://oxg.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kiv.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://vdm.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vln.xuanzx.com

[U67] PHP：处理文件上传
来源：http://fnj.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://udc.xylfe.cn

[U68] PHP：PDO 连接
来源：http://omy.dianchejie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lwh.yongpay.top

[U69] PHP：PDO 预处理
来源：http://zda.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kul.fengsongda.top

[U70] PHP：PDO 事务
来源：http://apo.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sar.xuetiantiany.cn

[U71] PHP：抛出异常
来源：http://lys.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://vhe.tarul.cn

[U72] PHP：写错误日志
来源：http://ozk.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://gca.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://ffg.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://ilg.sweek.top

[U74] PHP：读取环境变量
来源：http://hkl.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://yol.havefunace.top

[U75] PHP：依赖注入
来源：http://jzo.epnwcf.com

composer require psr/container
来源：http://xhy.fehbvm.com

[U76] PHP：简单路由
来源：http://hnp.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://acr.meibo888.top

[U77] PHP：模板渲染
来源：http://vri.ybcxt.top

composer require twig/twig
来源：http://rnk.iojbl.cn

[U78] PHP：单元测试
来源：http://awv.yj202588.top

composer require --dev phpunit/phpunit
来源：http://sez.daxiang520.top

[U79] PHP：静态分析
来源：http://ijj.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://yfu.nwbrower.top

[U80] PHP：代码规范修复
来源：http://uwr.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bko.cashguo.top

[U81] JS：初始化项目
来源：http://nvd.bjfxy.top

npm init -y;  npm i express
来源：http://ffh.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://api.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kmw.aibaodan.cn

[U83] JS：ES Module 导入导出
来源：http://dzl.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://quw.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://jvp.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://nhn.jiagoushi.top

[U85] JS：可选链
来源：http://fyk.shanyushiyangtech.top

a?.b?.c
来源：http://qnl.yongpay.top

[U86] JS：空值合并
来源：http://eww.jqgfzy.top

a ?? b
来源：http://ggi.9152youxi.cn

[U87] JS：解构默认值
来源：http://tjm.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://cry.hcnkem.com

[U88] JS：对象展开合并
来源：http://qad.daria6918.cn

{ ...a, ...b }
来源：http://iqb.0kj1m.cn

[U89] JS：数组去重
来源：http://bke.cucudq.cn

[...new Set(arr)]
来源：http://urr.yonumen.top

[U90] JS：数字数组排序
来源：http://whj.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://ojl.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://enp.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fda.fktsv.cn

[U92] JS：深拷贝
来源：http://rge.yvedp.cn

structuredClone(obj)
来源：http://znl.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://pth.tarul.cn

`共 ${n} 条`
来源：http://axu.xuanzx.com

[U94] JS：箭头函数
来源：http://mzj.vqdsnc.cn

const double = x => x * 2;
来源：http://mbo.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://weu.aizwys.cn

new Promise((resolve, reject) => {})
来源：http://ieb.birdmap.top

[U96] JS：async/await 与异常
来源：http://cgy.meibo888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lbr.ctjpmb.com

[U97] JS：并发请求
来源：http://dea.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgw.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://scu.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://frc.birdmap.top

[U99] JS：事件监听
来源：http://oty.ywan-chungtsiang.top

el.addEventListener("click", e => {})
来源：http://vxy.0kj1m.cn

[U100] JS：DOM 查询
来源：http://vcx.sysykeji.top

document.querySelector(".item")
来源：http://kwz.sufxvd.cn

[U101] JS：classList 操作
来源：http://qko.vqdsnc.cn

el.classList.toggle("active")
来源：http://enf.yuanzhike.top

[U102] JS：本地存储
来源：http://wez.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ugl.hnqzz.top

[U103] JS：定时器
来源：http://dyl.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xjw.ydjk.org.cn

[U104] JS：防抖
来源：http://fzj.jianghu66.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xtl.c1oappe.top

[U105] JS：节流
来源：http://ldv.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wst.ehwqpu.com

[U106] JS：日期格式化
来源：http://wys.shanyushiyangtech.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yxg.hfpthk.cn

[U107] JS：数字千分位
来源：http://ojy.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pty.cdnleiting.top

[U108] JS：随机整数
来源：http://zyw.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cev.jlsjyb.cn

[U109] JS：数组分组
来源：http://bfh.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://fwj.andypj.xyz

[U110] JS：数组分块
来源：http://cvh.andypj.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ecx.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://oeo.ydzc1.top

new Map(Object.entries(obj))
来源：http://hqc.nanxuanxn.top

[U112] JS：字符串补位
来源：http://jum.gogol.net.cn

"7".padStart(3, "0")
来源：http://wec.shuidangran.top

[U113] JS：正则替换全部
来源：http://kfb.yuxming.cn

s.replaceAll("a", "b")
来源：http://zkf.hesvh.cn

[U114] JS：JSON 深比较
来源：http://wfa.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xdh.aizwys.cn

[U115] JS：生成 UUID
来源：http://siv.iojbl.cn

crypto.randomUUID()
来源：http://odc.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://wnh.zhiwuduotai.top

/** @param {string} name */ function f(name) {}
来源：http://aft.jianghu66.top

[U117] JS：单元测试
来源：http://wqt.hongshengwenyu.top

npm i -D vitest;  npx vitest
来源：http://kfg.nwbrower.top

[U118] JS：开发服务器
来源：http://yym.tarul.cn

npm i -D vite;  npx vite
来源：http://yax.hongshengwenyu.top

[U119] JS：生产构建
来源：http://lvx.xuanzx.com

npx vite build
来源：http://tcs.xuetiantiany.cn

[U120] JS：读取环境变量（Vite）
来源：http://xbh.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://bzm.bbcook.cn

================================================================================
来源：http://nvv.hcnkem.com

统计汇总
来源：http://lpp.hammf.cn

================================================================================
来源：http://szh.52xcode.cn

按语言统计（条）：
来源：http://wga.vehdjk.com

Python ......... 252
来源：http://zih.yangfankeji.com

PHP ............ 252
来源：http://cqt.cashguo.top

JavaScript ..... 252
来源：http://svp.nwbrower.top

TypeScript ..... 212
来源：http://dpb.havefunace.top

Java ........... 212
来源：http://zze.sweek.top

Go ............. 212
来源：http://fym.zdqjudy.top

Ruby ........... 212
来源：http://pyx.xinyue.icu

C# ............. 212
来源：http://lho.zycfv.cn


<!-- 参考信息 -->