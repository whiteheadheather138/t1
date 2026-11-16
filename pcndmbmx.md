代发 wailian999

[T41] Perl：Hello World
来源：http://yeh.snrcjt.cn

print "Hello\n";
来源：http://tcy.shuidangran.top

[T42] Perl：变量类型
来源：http://qmy.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qfv.snrcjt.cn

[T43] Perl：字符串插值
来源：http://eti.xziqi.cn

"值: $a"
来源：http://wsq.xylfe.cn

[T44] Perl：条件
来源：http://kde.yj20258.top

if ($a > 0) { print "正"; }
来源：http://vjj.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://jfb.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://lko.uphjek.com

[T46] Perl：哈希操作
来源：http://snq.ppjwa.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bqs.daria6918.cn

[T47] Perl：正则捕获
来源：http://bte.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qtm.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://byx.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://tcf.hesvh.cn

[T49] Perl：函数
来源：http://ncb.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://scf.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://vcv.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bau.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://ksc.xziqi.cn

[T51] Scala：Hello World
来源：http://orf.yanxiufei.cn

println("Hello")
来源：http://elt.cheryme.top

[T52] Scala：变量
来源：http://bct.yanxiufei.cn

val a = 1;  var b = 2
来源：http://esw.sxryk.cn

[T53] Scala：字符串插值
来源：http://fgv.gotoacloud.top

s"值: $b"
来源：http://gmf.jiagoushi.top

[T54] Scala：集合映射
来源：http://qmp.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://qsg.sufxvd.cn

[T55] Scala：集合过滤
来源：http://lnq.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://tla.hysaishi.cn

[T56] Scala：样例类
来源：http://uue.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://psn.vehdjk.com

[T57] Scala：模式匹配
来源：http://dgc.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://mwm.pycfn.com

[T58] Scala：函数定义
来源：http://gqx.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://abg.haohaochexian.top

[T59] Scala：循环
来源：http://zbo.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://fri.quarkkingdee.top

[T60] Scala：折叠
来源：http://wvb.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tld.sjlbkw.cn

================================================================================
来源：http://lvz.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://slh.ydjk.org.cn

================================================================================
来源：http://enf.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://wrw.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mbh.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://irp.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://era.yj202588.top

[U03] Py：加载 .env 配置
来源：http://wwg.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://roz.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://wat.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sbr.fzhhl.top

[U05] Py：列表去重且保序
来源：http://ftk.shuidangran.top

list(dict.fromkeys(arr))
来源：http://vct.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://ume.c1oappe.top

{**a, **b}
来源：http://kzg.yfazqb.com

[U07] Py：反转字典键值
来源：http://ldu.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://lms.mhx1999.top

[U08] Py：展平二维列表
来源：http://lcm.vehdjk.com

[y for x in nested for y in x]
来源：http://qbf.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://kqk.c1oappe.top

max(d, key=d.get)
来源：http://ypt.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://any.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ufz.snrcjt.cn

[U11] Py：生成器表达式
来源：http://oxt.mhx1999.top

(x * 2 for x in arr)
来源：http://qtm.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ifa.yfazqb.com

Counter(arr).most_common(3)
来源：http://lar.birdmap.top

[U13] Py：固定长度队列
来源：http://lem.jyoumei.cn

deque(maxlen=10)
来源：http://gqt.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://zcv.dashuyun.cn

defaultdict(list)
来源：http://eql.jlsjyb.cn

[U15] Py：高精度计时
来源：http://slc.chenlongwang.top

t = time.perf_counter()
来源：http://nyq.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://jfe.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ill.ydjk.org.cn

[U17] Py：初始化日志
来源：http://hut.wangshuangyany.cn

logging.basicConfig(level=logging.INFO)
来源：http://cjy.fehbvm.com

[U18] Py：预编译正则
来源：http://sie.daria6918.cn

pat = re.compile(r"\d+")
来源：http://old.meibo888.top

[U19] Py：正则替换带回调
来源：http://ntv.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cbw.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://oec.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://jvz.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://meh.fzhhl.top

@contextlib.contextmanager
来源：http://jia.9152youxi.cn

[U22] Py：矩阵转置
来源：http://vqr.shanyushiyangkeji.top

list(zip(*m))
来源：http://cxt.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://ssn.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hvi.xuetiantiany.cn

[U24] Py：路径操作
来源：http://owl.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hvk.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://qpn.guowangkeji.top

csv.DictReader(f)
来源：http://hqk.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://iyq.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pqt.yfazqb.com

[U27] Py：异步 HTTP
来源：http://jsg.xylfe.cn

aiohttp.ClientSession() 配合 async with
来源：http://wle.sjlbkw.cn

[U28] Py：类型别名
来源：http://tab.daxiang520.top

UserId = int
来源：http://sdu.bjfxy.top

[U29] Py：属性校验
来源：http://qak.yueranfly.top

@property 与 @x.setter 配合
来源：http://vps.yfazqb.com

[U30] Py：数据类
来源：http://wmn.tarul.cn

@dataclass(slots=True)
来源：http://iip.ybcxt.top

[U31] Py：单测
来源：http://adk.fehbvm.com

python -m pytest -q
来源：http://ofi.pycfn.com

[U32] Py：代码格式化
来源：http://kps.hesvh.cn

ruff format . && ruff check --fix .
来源：http://esr.jlsjyb.cn

[U33] Py：打包发布
来源：http://tkh.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ffv.zhijiandao.cn

[U34] Py：判断编码
来源：http://olw.fzhhl.top

chardet.detect(raw)
来源：http://muh.vqdsnc.cn

[U35] Py：发送邮件
来源：http://jqn.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bpt.yj20258.top

[U36] Py：定时任务
来源：http://ksj.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://ubm.yongpay.top

[U37] Py：读写 Excel
来源：http://vly.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://snw.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://cks.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://gke.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://gda.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://kjc.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://thm.hnqzz.top

print("err", file=sys.stderr)
来源：http://tlv.hammf.cn

[U41] PHP：初始化 Composer 项目
来源：http://gkd.chenlongwang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yde.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://kip.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zko.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://pvh.zhiwuduotai.top

namespace App\Http;
来源：http://fqp.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://fch.svipenyu.cn

declare(strict_types=1);
来源：http://rlq.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://asr.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nln.jinqigfzy.top

[U46] PHP：可空类型
来源：http://udd.quarkkingdee.top

?string $name = null
来源：http://aet.ppjwa.cn

[U47] PHP：联合类型
来源：http://brm.jyoumei.cn

int|string $id
来源：http://trr.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://xaf.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wnc.gogol.net.cn

[U49] PHP：只读属性
来源：http://rny.wangdashe.top

public readonly string $name
来源：http://rfy.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://ezp.svipenyu.cn

public function __construct(private int $id) {}
来源：http://vnj.jlsjyb.cn

[U51] PHP：数组解构
来源：http://qxn.hywenlv.cn

[$a, $b] = $arr;
来源：http://cdt.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://yjp.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://nal.gzhubu.top

[U53] PHP：空合并运算符
来源：http://mhg.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://tlh.hywenlv.cn

[U54] PHP：空安全调用
来源：http://iqr.ybcxt.top

$obj?->method()
来源：http://gyh.jqgfzy.top

[U55] PHP：match 表达式
来源：http://xqh.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxc.yuanzhike.top

[U56] PHP：命名参数
来源：http://rwm.dashuyun.cn

f(a: 1, b: 2)
来源：http://vhg.jinqigufen.top

[U57] PHP：字符串插值
来源：http://hxa.ybcxt.top

"值: {$a}"
来源：http://pfl.zhongyouzk.top

[U58] PHP：数组三件套
来源：http://lnp.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://smp.bbcook.cn

[U59] PHP：自定义排序
来源：http://vpj.tian-w.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dxy.sweek.top

[U60] PHP：JSON 编解码
来源：http://fyg.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qzg.zycfv.cn

[U61] PHP：正则
来源：http://cya.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tng.iojbl.cn

[U62] PHP：日期对象
来源：http://uem.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nme.yj20258.top

[U63] PHP：文件读写
来源：http://kbw.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mqs.nanxinkj.top

[U64] PHP：目录遍历
来源：http://nhv.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://vcl.jqgufenzy.top

[U65] PHP：会话
来源：http://afe.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://icw.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://xqu.hysaishi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uee.xingfuxueyuan.xyz

[U67] PHP：处理文件上传
来源：http://sti.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yuc.c1oappe.top

[U68] PHP：PDO 连接
来源：http://rqu.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hgl.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://csf.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sia.yonumen.top

[U70] PHP：PDO 事务
来源：http://knk.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kdc.bjfxy.top

[U71] PHP：抛出异常
来源：http://jic.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://irt.pengpengdd.cyou

[U72] PHP：写错误日志
来源：http://sib.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ypu.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://ura.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://jzz.jlsjyb.cn

[U74] PHP：读取环境变量
来源：http://web.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://gii.nanxinkj.top

[U75] PHP：依赖注入
来源：http://kjc.tian-w.cn

composer require psr/container
来源：http://hzr.yj20258888.top

[U76] PHP：简单路由
来源：http://azp.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tvy.jyoumei.cn

[U77] PHP：模板渲染
来源：http://rlb.dianchejie.cn

composer require twig/twig
来源：http://oua.iojbl.cn

[U78] PHP：单元测试
来源：http://sri.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://brn.vehdjk.com

[U79] PHP：静态分析
来源：http://avd.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://adk.xziqi.cn

[U80] PHP：代码规范修复
来源：http://jby.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://dtk.wangdashe.top

[U81] JS：初始化项目
来源：http://uwp.yonumen.top

npm init -y;  npm i express
来源：http://lsg.ivvv.top

[U82] JS：package.json 脚本
来源：http://fqc.0kj1m.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://glv.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://epk.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ryi.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://tvb.redwolf501.top

module.exports = { a };  const { a } = require("./m");
来源：http://rxm.daria6918.cn

[U85] JS：可选链
来源：http://zcm.bjfxy.top

a?.b?.c
来源：http://vio.hysaishi.cn

[U86] JS：空值合并
来源：http://syu.zycfv.cn

a ?? b
来源：http://ibn.cqqwz.cn

[U87] JS：解构默认值
来源：http://igq.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://mtq.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://rzz.yuxming.cn

{ ...a, ...b }
来源：http://xfc.xylfe.cn

[U89] JS：数组去重
来源：http://dfj.aizwys.cn

[...new Set(arr)]
来源：http://hzl.zdbjq.cn

[U90] JS：数字数组排序
来源：http://sgz.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://sgn.yonumen.top

[U91] JS：对象键值遍历
来源：http://cmh.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fuk.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://cnd.daria6918.cn

structuredClone(obj)
来源：http://zgk.jiagoushi.top

[U93] JS：模板字符串
来源：http://xwj.fzhhl.top

`共 ${n} 条`
来源：http://bhu.guowangkeji.top

[U94] JS：箭头函数
来源：http://yvk.zhongyouzk.top

const double = x => x * 2;
来源：http://sah.yangfankeji.com

[U95] JS：Promise 包装
来源：http://nlf.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://kwq.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://eqf.ydzc1.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jek.redwolf501.top

[U97] JS：并发请求
来源：http://hvp.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yxc.daria6918.cn

[U98] JS：fetch 带 JSON
来源：http://ytw.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kff.jiagoushi.top

[U99] JS：事件监听
来源：http://cvu.c1oappe.top

el.addEventListener("click", e => {})
来源：http://djw.sxryk.cn

[U100] JS：DOM 查询
来源：http://oyp.birdmap.top

document.querySelector(".item")
来源：http://urm.ybcxt.top

[U101] JS：classList 操作
来源：http://vda.jinqigufen.top

el.classList.toggle("active")
来源：http://mhh.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://bto.9152youxi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eyt.gotoacloud.top

[U103] JS：定时器
来源：http://ixt.tian-w.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xde.52xcode.cn

[U104] JS：防抖
来源：http://yye.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fok.ivvv.top

[U105] JS：节流
来源：http://qpc.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vlm.sjlbkw.cn

[U106] JS：日期格式化
来源：http://ivw.andypj.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pmh.jiagoushi.top

[U107] JS：数字千分位
来源：http://rkn.chenzaomai.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rpn.yuanzhike.top

[U108] JS：随机整数
来源：http://mjv.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kgn.gzhubu.top

[U109] JS：数组分组
来源：http://fwz.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://ddw.c1oappe.top

[U110] JS：数组分块
来源：http://pma.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xkz.xylfe.cn

[U111] JS：对象转 Map
来源：http://xyk.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://stw.yanxiufei.cn

[U112] JS：字符串补位
来源：http://ekl.gotoacloud.top

"7".padStart(3, "0")
来源：http://fkz.ppjwa.cn

[U113] JS：正则替换全部
来源：http://ffl.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://lsz.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://qfw.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://iyt.svipenyu.cn

[U115] JS：生成 UUID
来源：http://tnu.yvedp.cn

crypto.randomUUID()
来源：http://emv.aibaodan.cn

[U116] JS：类型检查（JSDoc）
来源：http://chj.cqqwz.cn

/** @param {string} name */ function f(name) {}
来源：http://efb.andypj.xyz

[U117] JS：单元测试
来源：http://eto.meibo888.top

npm i -D vitest;  npx vitest
来源：http://ypf.shuidangran.top

[U118] JS：开发服务器
来源：http://zpx.hfpthk.cn

npm i -D vite;  npx vite
来源：http://myz.vqdsnc.cn

[U119] JS：生产构建
来源：http://twe.zycfv.cn

npx vite build
来源：http://jqu.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://ufy.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://wrx.0kj1m.cn

================================================================================
来源：http://diy.xingfuxueyuan.xyz

统计汇总
来源：http://gim.hnxiangtu.top

================================================================================
来源：http://mwr.yanxiufei.cn

按语言统计（条）：
来源：http://hxw.zhaomingkeji.xyz

Python ......... 252
来源：http://cll.jinghuilouyu.cn

PHP ............ 252
来源：http://fft.dianchejie.cn

JavaScript ..... 252
来源：http://ruw.epnwcf.com

TypeScript ..... 212
来源：http://xfq.vqdsnc.cn

Java ........... 212
来源：http://bjj.aibaodan.cn

Go ............. 212
来源：http://rix.fanxiaobao.xyz

Ruby ........... 212
来源：http://fck.daria6918.cn

C# ............. 212
来源：http://lil.quarkkingdee.top

C .............. 30
来源：http://emb.tian-w.cn

C++ ............ 30
来源：http://oeo.daria6918.cn

SQL ............ 90
来源：http://vfr.zhijiandao.cn

Bash ........... 80
来源：http://zgx.hongshengwenyu.top


<!-- 参考信息 -->