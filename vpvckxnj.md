代发 wailian999

[T43] Perl：字符串插值
来源：http://oze.fanxiaobao.xyz

"值: $a"
来源：http://ceh.9152youxi.cn

[T44] Perl：条件
来源：http://azc.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://nzt.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://wfe.sweek.top

for my $x (@arr) { print $x; }
来源：http://tad.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://bfs.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zvj.hfpthk.cn

[T47] Perl：正则捕获
来源：http://ybj.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://paz.ybcxt.top

[T48] Perl：正则替换
来源：http://bwx.shuidangran.top

$s =~ s/old/new/g;
来源：http://txa.epnwcf.com

[T49] Perl：函数
来源：http://lcx.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rpq.yueranfly.top

[T50] Perl：逐行读文件
来源：http://pzc.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mgj.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://uai.guowangkeji.top

[T51] Scala：Hello World
来源：http://lkp.cqqwz.cn

println("Hello")
来源：http://ozo.ctjpmb.com

[T52] Scala：变量
来源：http://mfp.cucudq.cn

val a = 1;  var b = 2
来源：http://qdg.shzxlz.cn

[T53] Scala：字符串插值
来源：http://cdi.yonumen.top

s"值: $b"
来源：http://mpe.yj20258.top

[T54] Scala：集合映射
来源：http://cdb.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://zhs.sufxvd.cn

[T55] Scala：集合过滤
来源：http://rqz.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://wnu.jiagoushi.top

[T56] Scala：样例类
来源：http://xzf.sweek.top

case class User(name: String, age: Int)
来源：http://eso.zhengqikj.top

[T57] Scala：模式匹配
来源：http://tlr.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://pwv.hfpthk.cn

[T58] Scala：函数定义
来源：http://ntj.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://pmp.sjlbkw.cn

[T59] Scala：循环
来源：http://dzs.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://hnb.cqqwz.cn

[T60] Scala：折叠
来源：http://mnp.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xjt.zhijiandao.cn

================================================================================
来源：http://rhq.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dai.zhengqikj.top

================================================================================
来源：http://rhk.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://mwx.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://qbk.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://jzz.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wtd.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://tnl.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tfo.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://plk.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fnm.uphjek.com

[U05] Py：列表去重且保序
来源：http://sgg.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://agd.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://xib.jiagoushi.top

{**a, **b}
来源：http://fbv.tanke756.top

[U07] Py：反转字典键值
来源：http://wcu.yvedp.cn

{v: k for k, v in d.items()}
来源：http://zho.ybcxt.top

[U08] Py：展平二维列表
来源：http://sqm.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://vaj.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://kji.tian-w.cn

max(d, key=d.get)
来源：http://fsx.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://wnn.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mua.uphjek.com

[U11] Py：生成器表达式
来源：http://wrv.epnwcf.com

(x * 2 for x in arr)
来源：http://nqi.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ycz.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://cli.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://roc.wangshuangyany.cn

deque(maxlen=10)
来源：http://yul.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://zcx.nanxinkj.top

defaultdict(list)
来源：http://yvc.vehdjk.com

[U15] Py：高精度计时
来源：http://zsb.yuxming.cn

t = time.perf_counter()
来源：http://jht.cheryme.top

[U16] Py：命令行参数解析
来源：http://elv.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wqc.0kj1m.cn

[U17] Py：初始化日志
来源：http://uvi.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://miu.yfazqb.com

[U18] Py：预编译正则
来源：http://ydd.ivvv.top

pat = re.compile(r"\d+")
来源：http://opv.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://yne.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xye.fzhhl.top

[U20] Py：缓存函数结果
来源：http://faq.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://ent.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://pje.wangshuangyany.cn

@contextlib.contextmanager
来源：http://tvq.sysykeji.top

[U22] Py：矩阵转置
来源：http://ypg.meibo888.top

list(zip(*m))
来源：http://jcj.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://gmm.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nqu.nanxinkj.top

[U24] Py：路径操作
来源：http://bpi.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ejm.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://cvo.c1oappe.top

csv.DictReader(f)
来源：http://ctt.zdbjq.cn

[U26] Py：并发下载
来源：http://onk.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yal.yuxming.cn

[U27] Py：异步 HTTP
来源：http://ihn.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://abd.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://wat.bjfxy.top

UserId = int
来源：http://pph.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://wtb.ctjpmb.com

@property 与 @x.setter 配合
来源：http://cfi.0kj1m.cn

[U30] Py：数据类
来源：http://sux.tianlin.xyz

@dataclass(slots=True)
来源：http://eok.fehbvm.com

[U31] Py：单测
来源：http://pkj.fehbvm.com

python -m pytest -q
来源：http://yav.gogol.net.cn

[U32] Py：代码格式化
来源：http://fpx.xziqi.cn

ruff format . && ruff check --fix .
来源：http://dhb.kuanghao11.cn

[U33] Py：打包发布
来源：http://izm.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://mlh.bjfxy.top

[U34] Py：判断编码
来源：http://ljl.xuanzx.com

chardet.detect(raw)
来源：http://tzm.tianlin.xyz

[U35] Py：发送邮件
来源：http://itg.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pdm.mhx1999.top

[U36] Py：定时任务
来源：http://gdm.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://pjr.yj202588.top

[U37] Py：读写 Excel
来源：http://xia.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://kfn.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://sgj.hfpthk.cn

Path(__file__).resolve().parent
来源：http://ddd.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://qrq.mhx1999.top

sys.stdout.isatty()
来源：http://egb.shuidangran.top

[U40] Py：打印到标准错误
来源：http://hnu.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://sfo.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://qkk.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://nrr.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://ifk.ivvv.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iwa.xuanzx.com

[U43] PHP：声明命名空间
来源：http://ufv.hysaishi.cn

namespace App\Http;
来源：http://svv.zhiwuduotai.top

[U44] PHP：开启严格类型
来源：http://bft.jqgufenzy.top

declare(strict_types=1);
来源：http://ewk.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://irz.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://qts.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://vtw.xylfe.cn

?string $name = null
来源：http://pen.yvedp.cn

[U47] PHP：联合类型
来源：http://xey.zhengqikj.top

int|string $id
来源：http://gef.guowangkeji.top

[U48] PHP：纯枚举
来源：http://hhr.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://awc.xuanzx.com

[U49] PHP：只读属性
来源：http://qyu.zhaomingkeji.xyz

public readonly string $name
来源：http://pjw.yuxming.cn

[U50] PHP：构造器属性提升
来源：http://sof.yj20258888.top

public function __construct(private int $id) {}
来源：http://ctf.jqgufenzy.top

[U51] PHP：数组解构
来源：http://znw.jqgufenzy.top

[$a, $b] = $arr;
来源：http://zcq.wangdashe.top

[U52] PHP：箭头函数
来源：http://hfj.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://klk.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://bdf.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://vwv.guannengcc.top

[U54] PHP：空安全调用
来源：http://ofp.hnqzz.top

$obj?->method()
来源：http://wbn.shzxlz.cn

[U55] PHP：match 表达式
来源：http://sdi.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://czf.quarkkingdee.top

[U56] PHP：命名参数
来源：http://vbh.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://fgw.redwolf501.top

[U57] PHP：字符串插值
来源：http://epw.bbcook.cn

"值: {$a}"
来源：http://mez.havefunace.top

[U58] PHP：数组三件套
来源：http://ntz.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hxq.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://bwr.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://utr.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://eby.yonumen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iih.gzhubu.top

[U61] PHP：正则
来源：http://owr.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opw.iojbl.cn

[U62] PHP：日期对象
来源：http://eoo.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uub.haohaochexian.top

[U63] PHP：文件读写
来源：http://adw.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ooe.epnwcf.com

[U64] PHP：目录遍历
来源：http://zrx.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://hmj.yonumen.top

[U65] PHP：会话
来源：http://oyt.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ugo.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://dyk.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mty.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://wss.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wba.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://bxk.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pde.jyoumei.cn

[U69] PHP：PDO 预处理
来源：http://nzy.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vvh.yuxming.cn

[U70] PHP：PDO 事务
来源：http://sbw.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fsm.zhengqikj.top

[U71] PHP：抛出异常
来源：http://puv.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://ace.yuxming.cn

[U72] PHP：写错误日志
来源：http://pbq.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://ckj.jinqigfzy.top

[U73] PHP：读取 ini 配置
来源：http://ayx.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://zzw.zhengqikj.top

[U74] PHP：读取环境变量
来源：http://nva.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://uih.c1oappe.top

[U75] PHP：依赖注入
来源：http://wkg.shanyushiyangtech.top

composer require psr/container
来源：http://jkh.daria6918.cn

[U76] PHP：简单路由
来源：http://ups.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wtx.wangshuangyany.cn

[U77] PHP：模板渲染
来源：http://biu.zhengqikj.top

composer require twig/twig
来源：http://dyk.dashuyun.cn

[U78] PHP：单元测试
来源：http://bdb.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://rip.snrcjt.cn

[U79] PHP：静态分析
来源：http://rkk.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://tgt.cashguo.top

[U80] PHP：代码规范修复
来源：http://fiy.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xqz.hysaishi.cn

[U81] JS：初始化项目
来源：http://tnk.tarul.cn

npm init -y;  npm i express
来源：http://ipu.gotoacloud.top

[U82] JS：package.json 脚本
来源：http://pju.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rlz.nanxuanxn.top

[U83] JS：ES Module 导入导出
来源：http://omv.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://qlz.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://vut.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://zuh.zhoulong.xyz

[U85] JS：可选链
来源：http://upo.cheryme.top

a?.b?.c
来源：http://zfc.tanke756.top

[U86] JS：空值合并
来源：http://nmu.316326.xyz

a ?? b
来源：http://tsa.zhoulong.xyz

[U87] JS：解构默认值
来源：http://zqr.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://onm.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://oos.xylfe.cn

{ ...a, ...b }
来源：http://oqt.pengpengdd.cyou

[U89] JS：数组去重
来源：http://tyc.feifeiyinyue.top

[...new Set(arr)]
来源：http://gan.0kj1m.cn

[U90] JS：数字数组排序
来源：http://siq.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://pqv.yongpay.top

[U91] JS：对象键值遍历
来源：http://oki.dianchejie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zke.tianlin.xyz

[U92] JS：深拷贝
来源：http://wnt.jianghu66.top

structuredClone(obj)
来源：http://rwi.jqgufenzy.top

[U93] JS：模板字符串
来源：http://dfn.zdbjq.cn

`共 ${n} 条`
来源：http://bmu.zhoulong.xyz

[U94] JS：箭头函数
来源：http://mbn.jqgufenzy.top

const double = x => x * 2;
来源：http://bka.ctjpmb.com

[U95] JS：Promise 包装
来源：http://bvi.havefunace.top

new Promise((resolve, reject) => {})
来源：http://xet.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://kio.tianlin.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rzn.fanxiaobao.xyz

[U97] JS：并发请求
来源：http://zew.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://zsf.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://elb.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://brf.hongshengwenyu.top

[U99] JS：事件监听
来源：http://apd.tarul.cn

el.addEventListener("click", e => {})
来源：http://ivg.iojbl.cn

[U100] JS：DOM 查询
来源：http://mep.nanxinkj.top

document.querySelector(".item")
来源：http://zck.tanke756.top

[U101] JS：classList 操作
来源：http://rxx.dianchejie.cn

el.classList.toggle("active")
来源：http://lcf.ivvv.top

[U102] JS：本地存储
来源：http://hhu.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hjp.chenlongwang.top

[U103] JS：定时器
来源：http://ney.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qcm.xylfe.cn

[U104] JS：防抖
来源：http://fro.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fnh.yfazqb.com

[U105] JS：节流
来源：http://abp.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://htw.yongpay.top

[U106] JS：日期格式化
来源：http://klj.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iel.vqdsnc.cn

[U107] JS：数字千分位
来源：http://xiq.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://krq.chenlongwang.top

[U108] JS：随机整数
来源：http://kzs.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mow.jyoumei.cn

[U109] JS：数组分组
来源：http://kzi.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://xbh.hywenlv.cn

[U110] JS：数组分块
来源：http://iwe.fanxiaobao.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aad.chenlongwang.top

[U111] JS：对象转 Map
来源：http://qbl.fktsv.cn

new Map(Object.entries(obj))
来源：http://hiv.aibaodan.cn

[U112] JS：字符串补位
来源：http://emz.aibaodan.cn

"7".padStart(3, "0")
来源：http://fmj.nwbrower.top

[U113] JS：正则替换全部
来源：http://tkn.shanyushiyangtech.top

s.replaceAll("a", "b")
来源：http://hmg.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://eky.hammf.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dop.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://yfb.fehbvm.com

crypto.randomUUID()
来源：http://pzk.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://hqo.fzhhl.top

/** @param {string} name */ function f(name) {}
来源：http://lyd.cucudq.cn

[U117] JS：单元测试
来源：http://alm.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://lua.zdqjudy.top

[U118] JS：开发服务器
来源：http://gmr.svipenyu.cn

npm i -D vite;  npx vite
来源：http://rbu.guannengcc.top

[U119] JS：生产构建
来源：http://xky.ehwqpu.com

npx vite build
来源：http://dju.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://qsi.shanyushiyangtech.top

import.meta.env.VITE_API_URL
来源：http://zwd.fehbvm.com

================================================================================
来源：http://zuw.daria6918.cn

统计汇总
来源：http://hnm.redwolf501.top

================================================================================
来源：http://woo.sufxvd.cn

按语言统计（条）：
来源：http://bmb.ydzc1.top

Python ......... 252
来源：http://xpw.yueranfly.top

PHP ............ 252
来源：http://fml.wangdashe.top

JavaScript ..... 252
来源：http://brk.jinqigufen.top

TypeScript ..... 212
来源：http://tvu.zhixingplan.top

Java ........... 212
来源：http://pqz.tarul.cn

Go ............. 212
来源：http://alk.zhoulong.xyz

Ruby ........... 212
来源：http://ldi.vehdjk.com

C# ............. 212
来源：http://yza.andypj.xyz

C .............. 30
来源：http://jeu.jqgufenzy.top

C++ ............ 30
来源：http://nnu.pengpengdd.cyou

SQL ............ 90
来源：http://efe.uphjek.com

Bash ........... 80
来源：http://flw.bjfxy.top

Kotlin ......... 15
来源：http://sof.nanxuanxn.top

Swift .......... 15
来源：http://bpu.hfpthk.cn

Lua ............ 10
来源：http://vmh.kuanghao11.cn

Perl ........... 10
来源：http://lev.jqgufenzy.top


<!-- 参考信息 -->