代发 wailian999

[T39] Lua：模式匹配
来源：http://bdf.shuidangran.top

string.find(s, "%d+")
来源：http://yqf.hfpthk.cn

[T40] Lua：元表
来源：http://lhr.yvedp.cn

setmetatable({}, { __index = base })
来源：http://ccf.shzxlz.cn

[T41] Perl：Hello World
来源：http://dsu.xuetiantiany.cn

print "Hello\n";
来源：http://vqh.yvedp.cn

[T42] Perl：变量类型
来源：http://fjg.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uvf.tian-w.cn

[T43] Perl：字符串插值
来源：http://qzd.zhaomingkeji.xyz

"值: $a"
来源：http://ukc.wangshuangyany.cn

[T44] Perl：条件
来源：http://ppk.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://wqe.ppjwa.cn

[T45] Perl：数组遍历
来源：http://ofo.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://pdk.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://cmg.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tkn.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://dfx.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jzn.yj202588.top

[T48] Perl：正则替换
来源：http://agn.hywenlv.cn

$s =~ s/old/new/g;
来源：http://qff.hnqzz.top

[T49] Perl：函数
来源：http://ufq.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qqj.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://csg.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nst.jyoumei.cn

while (my $line = <$fh>) { print $line; }
来源：http://jms.hesvh.cn

[T51] Scala：Hello World
来源：http://wka.chenjidiqi.icu

println("Hello")
来源：http://alo.yueranfly.top

[T52] Scala：变量
来源：http://hew.tarul.cn

val a = 1;  var b = 2
来源：http://cqp.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://ubi.meibo888.top

s"值: $b"
来源：http://yas.zycfv.cn

[T54] Scala：集合映射
来源：http://gho.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://lpb.nanxinkj.top

[T55] Scala：集合过滤
来源：http://pen.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fbd.bjfxy.top

[T56] Scala：样例类
来源：http://aau.fehbvm.com

case class User(name: String, age: Int)
来源：http://osz.chenlongwang.top

[T57] Scala：模式匹配
来源：http://kod.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://icj.sysykeji.top

[T58] Scala：函数定义
来源：http://izh.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://waj.yonumen.top

[T59] Scala：循环
来源：http://wti.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://tjf.smart0.xyz

[T60] Scala：折叠
来源：http://ers.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zlv.shzxlz.cn

================================================================================
来源：http://tth.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mog.guowangkeji.top

================================================================================
来源：http://xil.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://mfk.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://uxq.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://wtt.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cvf.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://fbx.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://itf.jiagoushi.top

[U04] Py：变量调试打印
来源：http://iqk.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hgo.yuxming.cn

[U05] Py：列表去重且保序
来源：http://sql.fzhhl.top

list(dict.fromkeys(arr))
来源：http://agz.hywenlv.cn

[U06] Py：合并两个字典
来源：http://ghe.ybcxt.top

{**a, **b}
来源：http://fwq.tianlin.xyz

[U07] Py：反转字典键值
来源：http://zob.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://rnb.nanxinkj.top

[U08] Py：展平二维列表
来源：http://nru.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://nau.tarul.cn

[U09] Py：字典取最大值的键
来源：http://wcx.jinqigfzy.top

max(d, key=d.get)
来源：http://eas.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://zgu.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rov.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://yzs.yuxming.cn

(x * 2 for x in arr)
来源：http://xkw.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://rmf.vehdjk.com

Counter(arr).most_common(3)
来源：http://yjf.vehdjk.com

[U13] Py：固定长度队列
来源：http://qbx.daxiang520.top

deque(maxlen=10)
来源：http://owz.yj20258.top

[U14] Py：分组收集到列表
来源：http://yho.jyoumei.cn

defaultdict(list)
来源：http://isi.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://dfx.vehdjk.com

t = time.perf_counter()
来源：http://kmj.ybcxt.top

[U16] Py：命令行参数解析
来源：http://vvv.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nam.sysykeji.top

[U17] Py：初始化日志
来源：http://eeq.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://xst.jqgfzy.top

[U18] Py：预编译正则
来源：http://vya.hesvh.cn

pat = re.compile(r"\d+")
来源：http://gus.yfazqb.com

[U19] Py：正则替换带回调
来源：http://zjx.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://acb.bjfxy.top

[U20] Py：缓存函数结果
来源：http://qts.uphjek.com

@functools.lru_cache(maxsize=None)
来源：http://qdf.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://hjg.sufxvd.cn

@contextlib.contextmanager
来源：http://ioe.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://mqr.daxiang520.top

list(zip(*m))
来源：http://zaa.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://xyl.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ysi.zhixingplan.top

[U24] Py：路径操作
来源：http://jsm.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vmr.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://kbm.tian-w.cn

csv.DictReader(f)
来源：http://fpm.xinyue.icu

[U26] Py：并发下载
来源：http://lmw.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jpd.shuidangran.top

[U27] Py：异步 HTTP
来源：http://mwn.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://jly.aibaodan.cn

[U28] Py：类型别名
来源：http://jse.zycfv.cn

UserId = int
来源：http://tqg.yonumen.top

[U29] Py：属性校验
来源：http://mge.wangdashe.top

@property 与 @x.setter 配合
来源：http://gvg.xylfe.cn

[U30] Py：数据类
来源：http://tgd.yangfankeji.com

@dataclass(slots=True)
来源：http://knx.sweek.top

[U31] Py：单测
来源：http://yxb.sxryk.cn

python -m pytest -q
来源：http://xpo.jlsjyb.cn

[U32] Py：代码格式化
来源：http://zpu.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://alg.hysaishi.cn

[U33] Py：打包发布
来源：http://eja.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://iqs.kuanghao11.cn

[U34] Py：判断编码
来源：http://nmc.dashuyun.cn

chardet.detect(raw)
来源：http://jmi.epnwcf.com

[U35] Py：发送邮件
来源：http://yfu.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://huh.9152youxi.cn

[U36] Py：定时任务
来源：http://dhz.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://kmh.jinghuilouyu.cn

[U37] Py：读写 Excel
来源：http://xxi.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://cap.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://qzi.aizwys.cn

Path(__file__).resolve().parent
来源：http://oyo.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://uxq.jinqigufen.top

sys.stdout.isatty()
来源：http://ueu.guannengcc.top

[U40] Py：打印到标准错误
来源：http://kqh.gzhubu.top

print("err", file=sys.stderr)
来源：http://gmj.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://sqr.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://mps.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://jfk.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvb.uphjek.com

[U43] PHP：声明命名空间
来源：http://oyj.zdbjq.cn

namespace App\Http;
来源：http://com.gzhubu.top

[U44] PHP：开启严格类型
来源：http://kpt.ctjpmb.com

declare(strict_types=1);
来源：http://bjh.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://ees.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yqs.0kj1m.cn

[U46] PHP：可空类型
来源：http://fvt.snrcjt.cn

?string $name = null
来源：http://vlk.xylfe.cn

[U47] PHP：联合类型
来源：http://oeq.ppjwa.cn

int|string $id
来源：http://qgo.chenzaomai.com

[U48] PHP：纯枚举
来源：http://dod.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lfi.ydzc1.top

[U49] PHP：只读属性
来源：http://wgo.yanxiufei.cn

public readonly string $name
来源：http://avf.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://rqo.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://zjm.zycfv.cn

[U51] PHP：数组解构
来源：http://sfi.sufxvd.cn

[$a, $b] = $arr;
来源：http://las.bbcook.cn

[U52] PHP：箭头函数
来源：http://uao.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://xvf.cdnleiting.top

[U53] PHP：空合并运算符
来源：http://ndd.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://lbb.daxiang520.top

[U54] PHP：空安全调用
来源：http://uef.yuxming.cn

$obj?->method()
来源：http://rrd.yfazqb.com

[U55] PHP：match 表达式
来源：http://llx.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pxy.c1oappe.top

[U56] PHP：命名参数
来源：http://duu.yj20258.top

f(a: 1, b: 2)
来源：http://ifp.hywenlv.cn

[U57] PHP：字符串插值
来源：http://umu.jinyuanbaomall.cn

"值: {$a}"
来源：http://cnv.bbcook.cn

[U58] PHP：数组三件套
来源：http://kpb.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://koq.yj202588.top

[U59] PHP：自定义排序
来源：http://cxg.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ncs.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://dho.yvedp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://usv.iojbl.cn

[U61] PHP：正则
来源：http://xdj.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ltb.xziqi.cn

[U62] PHP：日期对象
来源：http://rwx.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yfa.yangfankeji.com

[U63] PHP：文件读写
来源：http://atf.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wql.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://obj.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://bcu.zycfv.cn

[U65] PHP：会话
来源：http://vdd.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://sii.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://olx.9152youxi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tok.ivvv.top

[U67] PHP：处理文件上传
来源：http://wun.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fzu.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://xmb.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fpg.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://txy.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iaf.fktsv.cn

[U70] PHP：PDO 事务
来源：http://zjh.c1oappe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dpv.hysaishi.cn

[U71] PHP：抛出异常
来源：http://fmc.jqgfzy.top

throw new RuntimeException("失败", 500);
来源：http://nfs.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://dun.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://eex.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://gad.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://ywe.yuxming.cn

[U74] PHP：读取环境变量
来源：http://oby.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://nbo.zdbjq.cn

[U75] PHP：依赖注入
来源：http://fmf.ywan-chungtsiang.top

composer require psr/container
来源：http://ctq.daxiang520.top

[U76] PHP：简单路由
来源：http://rsq.yongpay.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qrr.fehbvm.com

[U77] PHP：模板渲染
来源：http://zev.jinqigfzy.top

composer require twig/twig
来源：http://cvj.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://zxw.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://atb.xuetiantiany.cn

[U79] PHP：静态分析
来源：http://ynp.hongshengwenyu.top

composer require --dev phpstan/phpstan
来源：http://mgr.yj202588.top

[U80] PHP：代码规范修复
来源：http://nbj.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lhx.shzxlz.cn

[U81] JS：初始化项目
来源：http://uhl.wangdashe.top

npm init -y;  npm i express
来源：http://tsp.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://fjy.jinqigufen.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wno.shuidangran.top

[U83] JS：ES Module 导入导出
来源：http://xzh.jianghu66.top

export const a = 1;  import { a } from "./m.js";
来源：http://ydl.aibaodan.cn

[U84] JS：CommonJS 写法
来源：http://kqz.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gxj.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://obj.ivvv.top

a?.b?.c
来源：http://rhj.tanke756.top

[U86] JS：空值合并
来源：http://zoe.sufxvd.cn

a ?? b
来源：http://lnp.vehdjk.com

[U87] JS：解构默认值
来源：http://yji.jqgufenzy.top

const { a = 1, b = 2 } = obj;
来源：http://yfq.yuanzhike.top

[U88] JS：对象展开合并
来源：http://fbu.iojbl.cn

{ ...a, ...b }
来源：http://nhb.pengpengdd.cyou

[U89] JS：数组去重
来源：http://byj.gogol.net.cn

[...new Set(arr)]
来源：http://kpg.yangfankeji.com

[U90] JS：数字数组排序
来源：http://kxe.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://kgu.daxiang520.top

[U91] JS：对象键值遍历
来源：http://cbi.fktsv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sxe.nwbrower.top

[U92] JS：深拷贝
来源：http://ejn.daria6918.cn

structuredClone(obj)
来源：http://cuq.birdmap.top

[U93] JS：模板字符串
来源：http://ktk.xuanzx.com

`共 ${n} 条`
来源：http://ypy.9152youxi.cn

[U94] JS：箭头函数
来源：http://vrv.bjfxy.top

const double = x => x * 2;
来源：http://zew.andypj.xyz

[U95] JS：Promise 包装
来源：http://twq.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://puu.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://tfx.guowangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sce.bjfxy.top

[U97] JS：并发请求
来源：http://qlc.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yvv.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://hdx.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yqe.ppjwa.cn

[U99] JS：事件监听
来源：http://nrh.meibo888.top

el.addEventListener("click", e => {})
来源：http://agz.redwolf501.top

[U100] JS：DOM 查询
来源：http://jxy.tanke756.top

document.querySelector(".item")
来源：http://fto.ydjk.org.cn

[U101] JS：classList 操作
来源：http://xfs.cheryme.top

el.classList.toggle("active")
来源：http://fnx.guowangkeji.top

[U102] JS：本地存储
来源：http://yyd.jianghu66.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gfe.tianlin.xyz

[U103] JS：定时器
来源：http://ovr.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lnk.52xcode.cn

[U104] JS：防抖
来源：http://qat.zycfv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eoz.9152youxi.cn

[U105] JS：节流
来源：http://ueo.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xyl.dianchejie.cn

[U106] JS：日期格式化
来源：http://ehf.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vdv.bbcook.cn

[U107] JS：数字千分位
来源：http://bua.gzhubu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://grq.aibaodan.cn

[U108] JS：随机整数
来源：http://woo.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tfc.chenlongwang.top

[U109] JS：数组分组
来源：http://ale.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://pdi.cheryme.top

[U110] JS：数组分块
来源：http://kpd.aizwys.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jij.cdnleiting.top

[U111] JS：对象转 Map
来源：http://jic.cucudq.cn

new Map(Object.entries(obj))
来源：http://jxm.aizwys.cn

[U112] JS：字符串补位
来源：http://oun.ydzc1.top

"7".padStart(3, "0")
来源：http://jmb.sysykeji.top

[U113] JS：正则替换全部
来源：http://ugi.dashuyun.cn

s.replaceAll("a", "b")
来源：http://qmm.aibaodan.cn

[U114] JS：JSON 深比较
来源：http://hpd.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://smm.shanyushiyangkeji.top

[U115] JS：生成 UUID
来源：http://zfv.pengpengdd.cyou

crypto.randomUUID()
来源：http://cue.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://kfa.jianghu66.top

/** @param {string} name */ function f(name) {}
来源：http://hts.jinqigfzy.top

[U117] JS：单元测试
来源：http://bwr.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://gss.mhx1999.top

[U118] JS：开发服务器
来源：http://igz.ctjpmb.com

npm i -D vite;  npx vite
来源：http://nqe.zhijiandao.cn

[U119] JS：生产构建
来源：http://zvo.nanxinkj.top

npx vite build
来源：http://pef.ywan-chungtsiang.top

[U120] JS：读取环境变量（Vite）
来源：http://swe.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://ntr.ywan-chungtsiang.top

================================================================================
来源：http://ska.svipenyu.cn

统计汇总
来源：http://ptm.nanxuanxn.top

================================================================================
来源：http://krd.daria6918.cn

按语言统计（条）：
来源：http://oaj.chenzaomai.com

Python ......... 252
来源：http://qzb.jinyuanbaomall.cn

PHP ............ 252
来源：http://ppw.9152youxi.cn

JavaScript ..... 252
来源：http://muc.tianlin.xyz

TypeScript ..... 212
来源：http://juh.shzxlz.cn

Java ........... 212
来源：http://ekr.redwolf501.top

Go ............. 212
来源：http://auf.hcnkem.com

Ruby ........... 212
来源：http://fgd.jinghuilouyu.cn

C# ............. 212
来源：http://ehk.xziqi.cn


<!-- 参考信息 -->