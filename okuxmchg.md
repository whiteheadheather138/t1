代发 wailian999

[T47] Perl：正则捕获
来源：http://gyz.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qaq.hongshengwenyu.top

[T48] Perl：正则替换
来源：http://xrg.pycfn.com

$s =~ s/old/new/g;
来源：http://qtt.hnqzz.top

[T49] Perl：函数
来源：http://htr.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://had.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://hxh.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://acb.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://puu.0kj1m.cn

[T51] Scala：Hello World
来源：http://xxe.hywenlv.cn

println("Hello")
来源：http://ebh.hammf.cn

[T52] Scala：变量
来源：http://ski.aizwys.cn

val a = 1;  var b = 2
来源：http://ery.bjfxy.top

[T53] Scala：字符串插值
来源：http://eyj.jinqigufen.top

s"值: $b"
来源：http://ajl.tarul.cn

[T54] Scala：集合映射
来源：http://gsq.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://eax.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://whf.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pdy.hysaishi.cn

[T56] Scala：样例类
来源：http://qmb.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://hqb.ydzc1.top

[T57] Scala：模式匹配
来源：http://pve.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://vni.yvedp.cn

[T58] Scala：函数定义
来源：http://rap.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nzw.kuanghao11.cn

[T59] Scala：循环
来源：http://bgf.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://iqh.fehbvm.com

[T60] Scala：折叠
来源：http://xco.vqdsnc.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gyy.ppjwa.cn

================================================================================
来源：http://brj.gzhubu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://row.aibaodan.cn

================================================================================
来源：http://efp.zhijiandao.cn

[U01] Py：创建虚拟环境
来源：http://lcb.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://unh.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://rau.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tlm.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://hgd.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cmk.vehdjk.com

[U04] Py：变量调试打印
来源：http://pgg.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://arb.sysykeji.top

[U05] Py：列表去重且保序
来源：http://cid.hnqzz.top

list(dict.fromkeys(arr))
来源：http://cpa.svipenyu.cn

[U06] Py：合并两个字典
来源：http://nov.tarul.cn

{**a, **b}
来源：http://vdt.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://iqr.yfazqb.com

{v: k for k, v in d.items()}
来源：http://kqk.mhx1999.top

[U08] Py：展平二维列表
来源：http://gsp.snrcjt.cn

[y for x in nested for y in x]
来源：http://eef.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://trg.jianghu66.top

max(d, key=d.get)
来源：http://xkx.hysaishi.cn

[U10] Py：按值排序字典
来源：http://lia.ivvv.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qlb.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://gkz.ppjwa.cn

(x * 2 for x in arr)
来源：http://ivg.feifeiyinyue.top

[U12] Py：取出现最多的 3 个元素
来源：http://pxb.hywenlv.cn

Counter(arr).most_common(3)
来源：http://dzg.yfazqb.com

[U13] Py：固定长度队列
来源：http://nsz.guannengcc.top

deque(maxlen=10)
来源：http://our.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://hrc.yueranfly.top

defaultdict(list)
来源：http://ywp.zhixingplan.top

[U15] Py：高精度计时
来源：http://trz.svipenyu.cn

t = time.perf_counter()
来源：http://cur.shuidangran.top

[U16] Py：命令行参数解析
来源：http://oxm.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wvh.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://kwf.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://qzh.316326.xyz

[U18] Py：预编译正则
来源：http://fcj.shanyushiyangkeji.top

pat = re.compile(r"\d+")
来源：http://utf.c1oappe.top

[U19] Py：正则替换带回调
来源：http://aid.pengpengdd.cyou

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lbu.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://qtb.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://pmh.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://pog.sweek.top

@contextlib.contextmanager
来源：http://yci.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://heb.c1oappe.top

list(zip(*m))
来源：http://uoi.xuanzx.com

[U23] Py：分块读取大文件
来源：http://eqq.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xqm.jiagoushi.top

[U24] Py：路径操作
来源：http://xdx.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fmn.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://ont.xziqi.cn

csv.DictReader(f)
来源：http://zzw.jqgufenzy.top

[U26] Py：并发下载
来源：http://zmk.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xcr.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://wtc.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://zas.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://okt.zhijiandao.cn

UserId = int
来源：http://qvu.yj20258888.top

[U29] Py：属性校验
来源：http://xqr.zhaomingkeji.xyz

@property 与 @x.setter 配合
来源：http://wgy.nanxuanxn.top

[U30] Py：数据类
来源：http://ony.zhoulong.xyz

@dataclass(slots=True)
来源：http://wha.zhixingplan.top

[U31] Py：单测
来源：http://pve.bbcook.cn

python -m pytest -q
来源：http://ice.gaohongyu789.top

[U32] Py：代码格式化
来源：http://oso.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://ixs.jinyuanbaomall.cn

[U33] Py：打包发布
来源：http://csv.shangyingyoupin.top

python -m build  （依赖 pyproject.toml）
来源：http://uvo.shuidangran.top

[U34] Py：判断编码
来源：http://igs.chenzaomai.com

chardet.detect(raw)
来源：http://qtv.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://blt.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mfk.yanxiufei.cn

[U36] Py：定时任务
来源：http://zri.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://cep.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://kgo.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://knh.andypj.xyz

[U38] Py：获取脚本所在目录
来源：http://ntk.fzhhl.top

Path(__file__).resolve().parent
来源：http://lmd.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://gyj.sufxvd.cn

sys.stdout.isatty()
来源：http://nzw.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://wub.zdqjudy.top

print("err", file=sys.stderr)
来源：http://zlx.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://ttq.vqdsnc.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bcv.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://ptm.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cfv.hnqzz.top

[U43] PHP：声明命名空间
来源：http://qey.zhijiandao.cn

namespace App\Http;
来源：http://grk.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://qob.jinghuilouyu.cn

declare(strict_types=1);
来源：http://mdy.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://wjm.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pbi.shangyingyoupin.top

[U46] PHP：可空类型
来源：http://hqn.52xcode.cn

?string $name = null
来源：http://psf.sjlbkw.cn

[U47] PHP：联合类型
来源：http://wca.guannengcc.top

int|string $id
来源：http://hlq.yueranfly.top

[U48] PHP：纯枚举
来源：http://jnc.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uii.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://acj.hywenlv.cn

public readonly string $name
来源：http://wyn.pycfn.com

[U50] PHP：构造器属性提升
来源：http://cbq.52xcode.cn

public function __construct(private int $id) {}
来源：http://sqa.9152youxi.cn

[U51] PHP：数组解构
来源：http://tld.tianlin.xyz

[$a, $b] = $arr;
来源：http://pll.yangfankeji.com

[U52] PHP：箭头函数
来源：http://kcy.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://thx.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://slw.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://ofn.chenzaomai.com

[U54] PHP：空安全调用
来源：http://fdg.smart0.xyz

$obj?->method()
来源：http://sdm.chenlongwang.top

[U55] PHP：match 表达式
来源：http://yot.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vyt.ehwqpu.com

[U56] PHP：命名参数
来源：http://eab.fktsv.cn

f(a: 1, b: 2)
来源：http://lxf.pengpengdd.cyou

[U57] PHP：字符串插值
来源：http://aus.daxiang520.top

"值: {$a}"
来源：http://buf.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://wkv.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jlf.xinyue.icu

[U59] PHP：自定义排序
来源：http://hqq.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssk.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://bmy.xziqi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://onn.zhoulong.xyz

[U61] PHP：正则
来源：http://bca.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jnf.xingfuxueyuan.xyz

[U62] PHP：日期对象
来源：http://fib.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qpt.ydjk.org.cn

[U63] PHP：文件读写
来源：http://kxf.tarul.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mtj.yj20258.top

[U64] PHP：目录遍历
来源：http://qme.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://eld.hesvh.cn

[U65] PHP：会话
来源：http://efc.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wti.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://xeq.yj202588.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://apt.bjfxy.top

[U67] PHP：处理文件上传
来源：http://lju.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wca.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://gpr.pengpengdd.cyou

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mkp.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://sju.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jdy.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://vlq.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://acd.hesvh.cn

[U71] PHP：抛出异常
来源：http://ieh.gzhubu.top

throw new RuntimeException("失败", 500);
来源：http://wlf.dianchejie.cn

[U72] PHP：写错误日志
来源：http://eym.tianlin.xyz

error_log("失败: " . $e->getMessage());
来源：http://ddw.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://vbe.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://hkr.fehbvm.com

[U74] PHP：读取环境变量
来源：http://yhi.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://izk.fzhhl.top

[U75] PHP：依赖注入
来源：http://esl.cqqwz.cn

composer require psr/container
来源：http://cfv.yonumen.top

[U76] PHP：简单路由
来源：http://pox.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://caa.jqgufenzy.top

[U77] PHP：模板渲染
来源：http://fbs.chenzaomai.com

composer require twig/twig
来源：http://xmw.ybcxt.top

[U78] PHP：单元测试
来源：http://onj.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://zpm.hammf.cn

[U79] PHP：静态分析
来源：http://oca.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://dal.cashguo.top

[U80] PHP：代码规范修复
来源：http://lpd.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kgo.mhx1999.top

[U81] JS：初始化项目
来源：http://arq.chenlongwang.top

npm init -y;  npm i express
来源：http://bkh.ywan-chungtsiang.top

[U82] JS：package.json 脚本
来源：http://vuz.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mct.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://tal.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://oji.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://msw.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://lgp.tian-w.cn

[U85] JS：可选链
来源：http://nqn.chenzaomai.com

a?.b?.c
来源：http://hid.chenjidiqi.icu

[U86] JS：空值合并
来源：http://riv.havefunace.top

a ?? b
来源：http://fcq.tanke756.top

[U87] JS：解构默认值
来源：http://got.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://wen.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://qvb.yongpay.top

{ ...a, ...b }
来源：http://ylk.ydzc1.top

[U89] JS：数组去重
来源：http://nbj.andypj.xyz

[...new Set(arr)]
来源：http://iih.svipenyu.cn

[U90] JS：数字数组排序
来源：http://hct.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://xdh.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://xix.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hgu.tanke756.top

[U92] JS：深拷贝
来源：http://liw.dianchejie.cn

structuredClone(obj)
来源：http://xzu.52xcode.cn

[U93] JS：模板字符串
来源：http://atq.yj20258888.top

`共 ${n} 条`
来源：http://exg.shuidangran.top

[U94] JS：箭头函数
来源：http://tli.guannengcc.top

const double = x => x * 2;
来源：http://kah.gotoacloud.top

[U95] JS：Promise 包装
来源：http://ygf.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://vuc.yj20258888.top

[U96] JS：async/await 与异常
来源：http://rrz.yanxiufei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ypj.52xcode.cn

[U97] JS：并发请求
来源：http://diw.0kj1m.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wwq.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://wsc.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cxp.9152youxi.cn

[U99] JS：事件监听
来源：http://vnd.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://oaa.havefunace.top

[U100] JS：DOM 查询
来源：http://xyh.bbcook.cn

document.querySelector(".item")
来源：http://hwg.yangfankeji.com

[U101] JS：classList 操作
来源：http://htx.ydjk.org.cn

el.classList.toggle("active")
来源：http://xbf.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://qsc.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://abn.yj20258888.top

[U103] JS：定时器
来源：http://azj.fzhhl.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eej.fktsv.cn

[U104] JS：防抖
来源：http://cbr.shangyingyoupin.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftp.fktsv.cn

[U105] JS：节流
来源：http://ktg.sxryk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sod.birdmap.top

[U106] JS：日期格式化
来源：http://dkn.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://abd.hfpthk.cn

[U107] JS：数字千分位
来源：http://ssh.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nlv.yonumen.top

[U108] JS：随机整数
来源：http://rfq.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ybi.fktsv.cn

[U109] JS：数组分组
来源：http://mdl.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://svm.xuanzx.com

[U110] JS：数组分块
来源：http://blp.gaohongyu789.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xxx.jinqigufen.top

[U111] JS：对象转 Map
来源：http://alt.hcnkem.com

new Map(Object.entries(obj))
来源：http://tct.yueranfly.top

[U112] JS：字符串补位
来源：http://lum.tanke756.top

"7".padStart(3, "0")
来源：http://frv.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://xpv.iojbl.cn

s.replaceAll("a", "b")
来源：http://mah.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://ccn.haohaochexian.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qli.smart0.xyz

[U115] JS：生成 UUID
来源：http://tnn.jiagoushi.top

crypto.randomUUID()
来源：http://bxs.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://uzy.0kj1m.cn

/** @param {string} name */ function f(name) {}
来源：http://tzm.sysykeji.top

[U117] JS：单元测试
来源：http://fwf.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://emm.jinqigfzy.top

[U118] JS：开发服务器
来源：http://mvh.yuanzhike.top

npm i -D vite;  npx vite
来源：http://shd.xylfe.cn

[U119] JS：生产构建
来源：http://vyt.hnxiangtu.top

npx vite build
来源：http://izn.zhengqikj.top

[U120] JS：读取环境变量（Vite）
来源：http://nnn.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://raz.ywan-chungtsiang.top

================================================================================
来源：http://idt.yanxiufei.cn

统计汇总
来源：http://phg.svipenyu.cn

================================================================================
来源：http://fnm.nanxinkj.top

按语言统计（条）：
来源：http://tfg.yueranfly.top

Python ......... 252
来源：http://zto.tian-w.cn

PHP ............ 252
来源：http://kqx.fehbvm.com

JavaScript ..... 252
来源：http://ffp.jinqigufen.top

TypeScript ..... 212
来源：http://kxz.yueranfly.top

Java ........... 212
来源：http://zqk.yanxiufei.cn

Go ............. 212
来源：http://lqf.52xcode.cn

Ruby ........... 212
来源：http://zbp.hongshengwenyu.top

C# ............. 212
来源：http://ecp.ivvv.top

C .............. 30
来源：http://vts.jinqigfzy.top

C++ ............ 30
来源：http://mab.hammf.cn

SQL ............ 90
来源：http://hst.aizwys.cn

Bash ........... 80
来源：http://vwl.yj202588.top

Kotlin ......... 15
来源：http://fbp.zhengqikj.top

Swift .......... 15
来源：http://fll.ybcxt.top

Lua ............ 10
来源：http://lvs.zhijiandao.cn

Perl ........... 10
来源：http://ium.jlsjyb.cn

Scala .......... 10
来源：http://fow.shangyingyoupin.top

------------------------------------
来源：http://wwd.zhengqikj.top

合计 ........... 2106 条
来源：http://iev.cdnleiting.top

按章节统计：
来源：http://djd.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mhn.haohaochexian.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://slx.ydjk.org.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ufb.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fie.vehdjk.com


<!-- 参考信息 -->