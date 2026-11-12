代发 wailian999

[T41] Perl：Hello World
来源：http://lsq.fehbvm.com

print "Hello\n";
来源：http://gaa.nanxuanxn.top

[T42] Perl：变量类型
来源：http://hpw.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cke.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://khb.xylfe.cn

"值: $a"
来源：http://uig.feifeiyinyue.top

[T44] Perl：条件
来源：http://xgp.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://hbx.ybcxt.top

[T45] Perl：数组遍历
来源：http://fyr.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://xkp.xinyue.icu

[T46] Perl：哈希操作
来源：http://chc.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://woy.gogol.net.cn

[T47] Perl：正则捕获
来源：http://cso.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://krv.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://iwa.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://mxp.xylfe.cn

[T49] Perl：函数
来源：http://wlz.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggz.sxryk.cn

[T50] Perl：逐行读文件
来源：http://pfe.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://adc.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://ksm.wangdashe.top

[T51] Scala：Hello World
来源：http://jzu.aibaodan.cn

println("Hello")
来源：http://wbg.hfpthk.cn

[T52] Scala：变量
来源：http://mbe.sxryk.cn

val a = 1;  var b = 2
来源：http://ols.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://uhm.havefunace.top

s"值: $b"
来源：http://yax.hcnkem.com

[T54] Scala：集合映射
来源：http://obj.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://tfd.dashuyun.cn

[T55] Scala：集合过滤
来源：http://fqf.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://slu.jiagoushi.top

[T56] Scala：样例类
来源：http://fsn.jyoumei.cn

case class User(name: String, age: Int)
来源：http://eub.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://teb.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vsu.guowangkeji.top

[T58] Scala：函数定义
来源：http://mro.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://kzb.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://rzc.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://ena.cdnleiting.top

[T60] Scala：折叠
来源：http://qwg.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kdg.cashguo.top

================================================================================
来源：http://lwo.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pyc.daria6918.cn

================================================================================
来源：http://odi.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://pep.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://jax.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://awr.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hrf.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://gpe.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mlc.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://pkz.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lvc.cheryme.top

[U05] Py：列表去重且保序
来源：http://kna.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://nln.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://jkz.cdnleiting.top

{**a, **b}
来源：http://zjv.andypj.xyz

[U07] Py：反转字典键值
来源：http://hbf.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://yiw.yongpay.top

[U08] Py：展平二维列表
来源：http://jyw.jqgufenzy.top

[y for x in nested for y in x]
来源：http://xxd.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://ols.yuanzhike.top

max(d, key=d.get)
来源：http://gnk.cheryme.top

[U10] Py：按值排序字典
来源：http://ngp.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rct.yuanzhike.top

[U11] Py：生成器表达式
来源：http://xdp.sysykeji.top

(x * 2 for x in arr)
来源：http://lhp.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://oss.meibo888.top

Counter(arr).most_common(3)
来源：http://iak.wangdashe.top

[U13] Py：固定长度队列
来源：http://jey.gzhubu.top

deque(maxlen=10)
来源：http://yay.pycfn.com

[U14] Py：分组收集到列表
来源：http://vfd.sxryk.cn

defaultdict(list)
来源：http://rlm.ehwqpu.com

[U15] Py：高精度计时
来源：http://hhs.havefunace.top

t = time.perf_counter()
来源：http://urg.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://ubh.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hli.meibo888.top

[U17] Py：初始化日志
来源：http://gas.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://eyh.yj202588.top

[U18] Py：预编译正则
来源：http://qmi.yvedp.cn

pat = re.compile(r"\d+")
来源：http://bzd.fzhhl.top

[U19] Py：正则替换带回调
来源：http://mza.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rgd.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://qrz.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://flh.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://eft.yuanzhike.top

@contextlib.contextmanager
来源：http://pcf.shzxlz.cn

[U22] Py：矩阵转置
来源：http://hgd.yongpay.top

list(zip(*m))
来源：http://lbb.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://tkg.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jtt.gaohongyu789.top

[U24] Py：路径操作
来源：http://ckg.gotoacloud.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fbm.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://jkm.havefunace.top

csv.DictReader(f)
来源：http://bus.xuanzx.com

[U26] Py：并发下载
来源：http://ewx.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vnk.ywan-chungtsiang.top

[U27] Py：异步 HTTP
来源：http://qfv.fktsv.cn

aiohttp.ClientSession() 配合 async with
来源：http://wap.aibaodan.cn

[U28] Py：类型别名
来源：http://gdo.svipenyu.cn

UserId = int
来源：http://sem.snrcjt.cn

[U29] Py：属性校验
来源：http://ima.fengsongda.top

@property 与 @x.setter 配合
来源：http://rbb.meibo888.top

[U30] Py：数据类
来源：http://xyw.c1oappe.top

@dataclass(slots=True)
来源：http://llu.9152youxi.cn

[U31] Py：单测
来源：http://ieq.bbcook.cn

python -m pytest -q
来源：http://nde.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://hbn.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://ztc.zycfv.cn

[U33] Py：打包发布
来源：http://mgr.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://smy.ydzc1.top

[U34] Py：判断编码
来源：http://uam.shzxlz.cn

chardet.detect(raw)
来源：http://kvx.yuanzhike.top

[U35] Py：发送邮件
来源：http://wxx.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kcq.zhongyouzk.top

[U36] Py：定时任务
来源：http://fao.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://qhp.fengsongda.top

[U37] Py：读写 Excel
来源：http://xfo.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://pgc.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://icw.andypj.xyz

Path(__file__).resolve().parent
来源：http://apx.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://iaa.yvedp.cn

sys.stdout.isatty()
来源：http://fnu.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://ryx.cdnleiting.top

print("err", file=sys.stderr)
来源：http://qhi.316326.xyz

[U41] PHP：初始化 Composer 项目
来源：http://jxv.sysykeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qwg.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://nrl.fzhhl.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yiw.mhx1999.top

[U43] PHP：声明命名空间
来源：http://ibv.aizwys.cn

namespace App\Http;
来源：http://rbz.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://fkm.yuanzhike.top

declare(strict_types=1);
来源：http://nnp.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://orn.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mve.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://xiw.aizwys.cn

?string $name = null
来源：http://cqd.xziqi.cn

[U47] PHP：联合类型
来源：http://vbe.yongpay.top

int|string $id
来源：http://ygs.hywenlv.cn

[U48] PHP：纯枚举
来源：http://lfc.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://odl.fktsv.cn

[U49] PHP：只读属性
来源：http://nak.meibo888.top

public readonly string $name
来源：http://kaw.c1oappe.top

[U50] PHP：构造器属性提升
来源：http://fql.cqqwz.cn

public function __construct(private int $id) {}
来源：http://roe.redwolf501.top

[U51] PHP：数组解构
来源：http://iil.gaohongyu789.top

[$a, $b] = $arr;
来源：http://gmc.jinqigufen.top

[U52] PHP：箭头函数
来源：http://xfe.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://edf.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://iwt.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://uhw.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://uxj.chenlongwang.top

$obj?->method()
来源：http://sfk.jyoumei.cn

[U55] PHP：match 表达式
来源：http://luw.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zst.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://kky.vehdjk.com

f(a: 1, b: 2)
来源：http://ylp.hywenlv.cn

[U57] PHP：字符串插值
来源：http://aul.nanxuanxn.top

"值: {$a}"
来源：http://dla.guannengcc.top

[U58] PHP：数组三件套
来源：http://wen.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ozo.svipenyu.cn

[U59] PHP：自定义排序
来源：http://rtp.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zzg.cashguo.top

[U60] PHP：JSON 编解码
来源：http://tzh.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gum.dianchejie.cn

[U61] PHP：正则
来源：http://iij.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vrt.tanke756.top

[U62] PHP：日期对象
来源：http://vkf.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ukr.chenzaomai.com

[U63] PHP：文件读写
来源：http://srf.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hev.haohaochexian.top

[U64] PHP：目录遍历
来源：http://ncs.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://kul.ehwqpu.com

[U65] PHP：会话
来源：http://pqq.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://uuu.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://dfr.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yry.316326.xyz

[U67] PHP：处理文件上传
来源：http://ejz.fanxiaobao.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qgo.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://jlr.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wdz.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://khd.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bdr.mhx1999.top

[U70] PHP：PDO 事务
来源：http://uuu.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tay.bbcook.cn

[U71] PHP：抛出异常
来源：http://grw.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://qad.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://rgx.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://iwj.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://ury.yj20258.top

parse_ini_file("config.ini", true)
来源：http://rob.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://uwf.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://aai.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://pbg.zycfv.cn

composer require psr/container
来源：http://orm.ehwqpu.com

[U76] PHP：简单路由
来源：http://qcy.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://atm.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://ahb.c1oappe.top

composer require twig/twig
来源：http://bir.bbcook.cn

[U78] PHP：单元测试
来源：http://bjp.cdnleiting.top

composer require --dev phpunit/phpunit
来源：http://jnk.cqqwz.cn

[U79] PHP：静态分析
来源：http://ksc.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://wwg.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://zdl.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ucl.ydjk.org.cn

[U81] JS：初始化项目
来源：http://irb.vqdsnc.cn

npm init -y;  npm i express
来源：http://ydv.52xcode.cn

[U82] JS：package.json 脚本
来源：http://zze.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gav.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://vpi.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://mad.tanke756.top

[U84] JS：CommonJS 写法
来源：http://emw.feifeiyinyue.top

module.exports = { a };  const { a } = require("./m");
来源：http://pmv.redwolf501.top

[U85] JS：可选链
来源：http://ets.yongpay.top

a?.b?.c
来源：http://ckq.zhijiandao.cn

[U86] JS：空值合并
来源：http://vwg.ctjpmb.com

a ?? b
来源：http://bat.yueranfly.top

[U87] JS：解构默认值
来源：http://jpr.fehbvm.com

const { a = 1, b = 2 } = obj;
来源：http://lzo.aizwys.cn

[U88] JS：对象展开合并
来源：http://vby.yj202588.top

{ ...a, ...b }
来源：http://dat.xylfe.cn

[U89] JS：数组去重
来源：http://twb.jinqigfzy.top

[...new Set(arr)]
来源：http://hxs.fzhhl.top

[U90] JS：数字数组排序
来源：http://ilv.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://hwo.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://ryy.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://etq.yangfankeji.com

[U92] JS：深拷贝
来源：http://lmu.gaohongyu789.top

structuredClone(obj)
来源：http://yio.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://dkw.cucudq.cn

`共 ${n} 条`
来源：http://umw.zhoulong.xyz

[U94] JS：箭头函数
来源：http://gkb.yonumen.top

const double = x => x * 2;
来源：http://pvn.fzhhl.top

[U95] JS：Promise 包装
来源：http://bmx.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://weu.jianghu66.top

[U96] JS：async/await 与异常
来源：http://guw.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vro.yuanzhike.top

[U97] JS：并发请求
来源：http://jgi.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rgc.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://kvs.tarul.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://erc.shuidangran.top

[U99] JS：事件监听
来源：http://qls.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://ghn.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://tdt.jianghu66.top

document.querySelector(".item")
来源：http://usb.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://xqu.zdbjq.cn

el.classList.toggle("active")
来源：http://nyc.tanke756.top

[U102] JS：本地存储
来源：http://ycf.yfazqb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://qrn.ydjk.org.cn

[U103] JS：定时器
来源：http://sfc.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rks.gogol.net.cn

[U104] JS：防抖
来源：http://hqo.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tph.wangshuangyany.cn

[U105] JS：节流
来源：http://jyb.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ztf.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://hub.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kwy.zdbjq.cn

[U107] JS：数字千分位
来源：http://blm.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ngr.birdmap.top

[U108] JS：随机整数
来源：http://dun.dianchejie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://teg.jinqigufen.top

[U109] JS：数组分组
来源：http://sxf.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://myd.bjfxy.top

[U110] JS：数组分块
来源：http://jwl.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iry.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://mwu.jlsjyb.cn

new Map(Object.entries(obj))
来源：http://cil.yueranfly.top

[U112] JS：字符串补位
来源：http://ihi.hnxiangtu.top

"7".padStart(3, "0")
来源：http://jde.kuanghao11.cn

[U113] JS：正则替换全部
来源：http://wus.c1oappe.top

s.replaceAll("a", "b")
来源：http://ypq.daria6918.cn

[U114] JS：JSON 深比较
来源：http://qdo.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dkt.sysykeji.top

[U115] JS：生成 UUID
来源：http://lqi.hongshengwenyu.top

crypto.randomUUID()
来源：http://mxz.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://hfi.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://uud.hywenlv.cn

[U117] JS：单元测试
来源：http://vih.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://jew.shanyushiyangkeji.top

[U118] JS：开发服务器
来源：http://mnn.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://pqr.tarul.cn

[U119] JS：生产构建
来源：http://zrl.316326.xyz

npx vite build
来源：http://dsa.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://hvf.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://bbt.andypj.xyz

================================================================================
来源：http://tce.svipenyu.cn

统计汇总
来源：http://ekc.fengsongda.top

================================================================================
来源：http://uen.316326.xyz

按语言统计（条）：
来源：http://kdg.chenlongwang.top

Python ......... 252
来源：http://qww.hywenlv.cn

PHP ............ 252
来源：http://pgl.feifeiyinyue.top

JavaScript ..... 252
来源：http://mxv.chenzaomai.com

TypeScript ..... 212
来源：http://pki.gaohongyu789.top

Java ........... 212
来源：http://eyz.xuetiantiany.cn

Go ............. 212
来源：http://ybm.zhiwuduotai.top

Ruby ........... 212
来源：http://yrr.mhx1999.top

C# ............. 212
来源：http://xlm.zdbjq.cn

C .............. 30
来源：http://gsx.ydjk.org.cn

C++ ............ 30
来源：http://xaf.zdqjudy.top

SQL ............ 90
来源：http://rtb.yj20258.top

Bash ........... 80
来源：http://nbq.hysaishi.cn


<!-- 参考信息 -->