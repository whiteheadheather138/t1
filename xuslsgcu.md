代发 wailian999

[T37] Lua：字符串拼接
来源：http://wtv.nanxuanxn.top

"a" .. "b"
来源：http://rjw.zhoulong.xyz

[T38] Lua：条件
来源：http://kek.pycfn.com

if x > 0 then print("正") end
来源：http://xxp.bjfxy.top

[T39] Lua：模式匹配
来源：http://uwq.hcnkem.com

string.find(s, "%d+")
来源：http://vtu.hcnkem.com

[T40] Lua：元表
来源：http://six.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://zyx.uphjek.com

[T41] Perl：Hello World
来源：http://mqw.haohaochexian.top

print "Hello\n";
来源：http://vqm.sjlbkw.cn

[T42] Perl：变量类型
来源：http://wnb.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aux.jiagoushi.top

[T43] Perl：字符串插值
来源：http://rcj.yangfankeji.com

"值: $a"
来源：http://sqq.sufxvd.cn

[T44] Perl：条件
来源：http://hxl.yj202588.top

if ($a > 0) { print "正"; }
来源：http://tic.shzxlz.cn

[T45] Perl：数组遍历
来源：http://vbl.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://qea.chenzaomai.com

[T46] Perl：哈希操作
来源：http://kwd.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tts.gogol.net.cn

[T47] Perl：正则捕获
来源：http://ioe.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qvq.daria6918.cn

[T48] Perl：正则替换
来源：http://gso.chenlongwang.top

$s =~ s/old/new/g;
来源：http://eds.jqgufenzy.top

[T49] Perl：函数
来源：http://yle.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tdj.ppjwa.cn

[T50] Perl：逐行读文件
来源：http://mmd.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sda.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://tek.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://khc.epnwcf.com

println("Hello")
来源：http://sgh.jianghu66.top

[T52] Scala：变量
来源：http://hos.smart0.xyz

val a = 1;  var b = 2
来源：http://bed.fehbvm.com

[T53] Scala：字符串插值
来源：http://ptd.sysykeji.top

s"值: $b"
来源：http://swg.tian-w.cn

[T54] Scala：集合映射
来源：http://bct.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://owp.hcnkem.com

[T55] Scala：集合过滤
来源：http://xfg.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://neu.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://coy.yj20258.top

case class User(name: String, age: Int)
来源：http://gtd.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://jzg.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ngx.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://fix.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://yio.nanxinkj.top

[T59] Scala：循环
来源：http://lbs.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://wlk.epnwcf.com

[T60] Scala：折叠
来源：http://osg.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xso.ydzc1.top

================================================================================
来源：http://fxq.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tqf.yongpay.top

================================================================================
来源：http://ait.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://fpj.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://wby.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://xdu.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vwh.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://umo.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://fzm.zycfv.cn

[U04] Py：变量调试打印
来源：http://ofr.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fqg.yueranfly.top

[U05] Py：列表去重且保序
来源：http://xlq.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://wsu.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://vtw.hcnkem.com

{**a, **b}
来源：http://tdk.xingfuxueyuan.xyz

[U07] Py：反转字典键值
来源：http://tsd.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://dkv.zhongyouzk.top

[U08] Py：展平二维列表
来源：http://adt.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://xbj.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://ebo.fzhhl.top

max(d, key=d.get)
来源：http://ghg.ivvv.top

[U10] Py：按值排序字典
来源：http://hif.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ppk.zhixingplan.top

[U11] Py：生成器表达式
来源：http://quj.316326.xyz

(x * 2 for x in arr)
来源：http://tdo.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://afm.ydzc1.top

Counter(arr).most_common(3)
来源：http://xew.jyoumei.cn

[U13] Py：固定长度队列
来源：http://cks.redwolf501.top

deque(maxlen=10)
来源：http://mrk.smart0.xyz

[U14] Py：分组收集到列表
来源：http://rzt.jinyuanbaomall.cn

defaultdict(list)
来源：http://xaj.xylfe.cn

[U15] Py：高精度计时
来源：http://iqh.smart0.xyz

t = time.perf_counter()
来源：http://ysg.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://tcs.yj202588.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://laa.9152youxi.cn

[U17] Py：初始化日志
来源：http://etx.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://srj.havefunace.top

[U18] Py：预编译正则
来源：http://bea.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://bgh.yueranfly.top

[U19] Py：正则替换带回调
来源：http://jrs.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ihw.bjfxy.top

[U20] Py：缓存函数结果
来源：http://cpf.shanyushiyangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://ihy.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://vhp.yj202588.top

@contextlib.contextmanager
来源：http://ibw.yongpay.top

[U22] Py：矩阵转置
来源：http://xbk.hammf.cn

list(zip(*m))
来源：http://nuw.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://jmy.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hao.dashuyun.cn

[U24] Py：路径操作
来源：http://yok.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mcq.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://orq.yonumen.top

csv.DictReader(f)
来源：http://ohf.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://joj.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lpx.fanxiaobao.xyz

[U27] Py：异步 HTTP
来源：http://vnn.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://wvq.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://dih.jqgufenzy.top

UserId = int
来源：http://adt.yuxming.cn

[U29] Py：属性校验
来源：http://zeu.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://cqm.yj202588.top

[U30] Py：数据类
来源：http://lth.yj202588.top

@dataclass(slots=True)
来源：http://ysp.sufxvd.cn

[U31] Py：单测
来源：http://isj.ppjwa.cn

python -m pytest -q
来源：http://smp.tanke756.top

[U32] Py：代码格式化
来源：http://nlh.vehdjk.com

ruff format . && ruff check --fix .
来源：http://abm.shzxlz.cn

[U33] Py：打包发布
来源：http://igg.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://ljw.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://uzm.wangdashe.top

chardet.detect(raw)
来源：http://kvk.havefunace.top

[U35] Py：发送邮件
来源：http://fpl.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://okt.wangdashe.top

[U36] Py：定时任务
来源：http://ozl.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://sqh.yvedp.cn

[U37] Py：读写 Excel
来源：http://mvh.xingfuxueyuan.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://vir.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://noy.ppjwa.cn

Path(__file__).resolve().parent
来源：http://cet.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://inw.ivvv.top

sys.stdout.isatty()
来源：http://jqk.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://kts.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://dgt.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://grz.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mba.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://iys.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mbd.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://kdq.cdnleiting.top

namespace App\Http;
来源：http://yqh.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://nck.cqqwz.cn

declare(strict_types=1);
来源：http://glc.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://yjy.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://erh.pengpengdd.cyou

[U46] PHP：可空类型
来源：http://fzw.yongpay.top

?string $name = null
来源：http://vnp.chenzaomai.com

[U47] PHP：联合类型
来源：http://hlu.ivvv.top

int|string $id
来源：http://qas.zycfv.cn

[U48] PHP：纯枚举
来源：http://kaf.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nrt.yongpay.top

[U49] PHP：只读属性
来源：http://grr.jinyuanbaomall.cn

public readonly string $name
来源：http://bwx.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://ypk.52xcode.cn

public function __construct(private int $id) {}
来源：http://kyh.hesvh.cn

[U51] PHP：数组解构
来源：http://zaj.yongpay.top

[$a, $b] = $arr;
来源：http://fig.jqgfzy.top

[U52] PHP：箭头函数
来源：http://bwv.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://str.guowangkeji.top

[U53] PHP：空合并运算符
来源：http://emp.snrcjt.cn

$v = $a ?? $b ?? "default";
来源：http://inv.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://yfb.cdnleiting.top

$obj?->method()
来源：http://tzm.ehwqpu.com

[U55] PHP：match 表达式
来源：http://yll.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://thw.fehbvm.com

[U56] PHP：命名参数
来源：http://pey.zhongyouzk.top

f(a: 1, b: 2)
来源：http://cix.havefunace.top

[U57] PHP：字符串插值
来源：http://wox.tarul.cn

"值: {$a}"
来源：http://ruz.mhx1999.top

[U58] PHP：数组三件套
来源：http://lgc.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qtc.havefunace.top

[U59] PHP：自定义排序
来源：http://fuo.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ekn.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://mbw.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://out.52xcode.cn

[U61] PHP：正则
来源：http://cuf.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://byv.wangdashe.top

[U62] PHP：日期对象
来源：http://unp.chenjidiqi.icu

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gpu.mhx1999.top

[U63] PHP：文件读写
来源：http://jew.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mcg.xuanzx.com

[U64] PHP：目录遍历
来源：http://ocf.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://uvg.daxiang520.top

[U65] PHP：会话
来源：http://rds.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qxi.hammf.cn

[U66] PHP：设置 Cookie
来源：http://ovp.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qlo.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://ayx.haohaochexian.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qao.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://ssk.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hnz.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://til.ydzc1.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tdv.ivvv.top

[U70] PHP：PDO 事务
来源：http://zaf.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xkv.daxiang520.top

[U71] PHP：抛出异常
来源：http://rtc.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://pof.yuanzhike.top

[U72] PHP：写错误日志
来源：http://zrp.sxryk.cn

error_log("失败: " . $e->getMessage());
来源：http://cms.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://pnk.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://aub.shuidangran.top

[U74] PHP：读取环境变量
来源：http://hxl.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://cff.dashuyun.cn

[U75] PHP：依赖注入
来源：http://bfd.xuanzx.com

composer require psr/container
来源：http://hlz.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://ukh.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rcv.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://kfd.hammf.cn

composer require twig/twig
来源：http://hyj.dianchejie.cn

[U78] PHP：单元测试
来源：http://vfi.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://yah.yj20258.top

[U79] PHP：静态分析
来源：http://zow.zycfv.cn

composer require --dev phpstan/phpstan
来源：http://cpl.daxiang520.top

[U80] PHP：代码规范修复
来源：http://xcl.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xts.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://mcj.bbcook.cn

npm init -y;  npm i express
来源：http://lqi.epnwcf.com

[U82] JS：package.json 脚本
来源：http://tge.redwolf501.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://khb.uphjek.com

[U83] JS：ES Module 导入导出
来源：http://omx.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://vdv.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://ljm.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nfl.chenzaomai.com

[U85] JS：可选链
来源：http://nko.yj20258.top

a?.b?.c
来源：http://rmt.zhoulong.xyz

[U86] JS：空值合并
来源：http://msv.jqgfzy.top

a ?? b
来源：http://atg.0kj1m.cn

[U87] JS：解构默认值
来源：http://swj.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://uex.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://bhv.jqgufenzy.top

{ ...a, ...b }
来源：http://xsd.gogol.net.cn

[U89] JS：数组去重
来源：http://hnx.birdmap.top

[...new Set(arr)]
来源：http://ykx.cheryme.top

[U90] JS：数字数组排序
来源：http://mib.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://zqt.bbcook.cn

[U91] JS：对象键值遍历
来源：http://vdk.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mnt.zycfv.cn

[U92] JS：深拷贝
来源：http://xse.zhijiandao.cn

structuredClone(obj)
来源：http://fbc.epnwcf.com

[U93] JS：模板字符串
来源：http://ype.wangdashe.top

`共 ${n} 条`
来源：http://buw.ydzc1.top

[U94] JS：箭头函数
来源：http://ntm.yuxming.cn

const double = x => x * 2;
来源：http://ucq.bjfxy.top

[U95] JS：Promise 包装
来源：http://kbz.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://whn.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://nxx.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lwi.cashguo.top

[U97] JS：并发请求
来源：http://wvm.yonumen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ofh.xuetiantiany.cn

[U98] JS：fetch 带 JSON
来源：http://fif.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ara.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://mrq.sysykeji.top

el.addEventListener("click", e => {})
来源：http://mdr.iojbl.cn

[U100] JS：DOM 查询
来源：http://orw.jiagoushi.top

document.querySelector(".item")
来源：http://fiy.mhx1999.top

[U101] JS：classList 操作
来源：http://llm.aizwys.cn

el.classList.toggle("active")
来源：http://hyu.yueranfly.top

[U102] JS：本地存储
来源：http://epd.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jsh.hnxiangtu.top

[U103] JS：定时器
来源：http://ora.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tgp.nanxuanxn.top

[U104] JS：防抖
来源：http://pch.yongpay.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzs.guowangkeji.top

[U105] JS：节流
来源：http://ezn.havefunace.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vsu.hysaishi.cn

[U106] JS：日期格式化
来源：http://lyx.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://myn.zhengqikj.top

[U107] JS：数字千分位
来源：http://hig.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nuu.jinqigufen.top

[U108] JS：随机整数
来源：http://ubw.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dty.zdqjudy.top

[U109] JS：数组分组
来源：http://ajl.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://iqx.ehwqpu.com

[U110] JS：数组分块
来源：http://ixi.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ljt.fktsv.cn

[U111] JS：对象转 Map
来源：http://kdi.fzhhl.top

new Map(Object.entries(obj))
来源：http://puy.9152youxi.cn

[U112] JS：字符串补位
来源：http://wea.quarkkingdee.top

"7".padStart(3, "0")
来源：http://xwh.xziqi.cn

[U113] JS：正则替换全部
来源：http://xtm.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://ssd.pycfn.com

[U114] JS：JSON 深比较
来源：http://lkx.zhiwuduotai.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tcz.hysaishi.cn

[U115] JS：生成 UUID
来源：http://uyd.chenjidiqi.icu

crypto.randomUUID()
来源：http://xwc.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://pkl.xuetiantiany.cn

/** @param {string} name */ function f(name) {}
来源：http://qje.zhoulong.xyz

[U117] JS：单元测试
来源：http://uqc.shanyushiyangkeji.top

npm i -D vitest;  npx vitest
来源：http://jlt.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://uwu.tianlin.xyz

npm i -D vite;  npx vite
来源：http://bbi.sweek.top

[U119] JS：生产构建
来源：http://xvd.haohaochexian.top

npx vite build
来源：http://wwq.dianchejie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rkw.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://isl.kuanghao11.cn

================================================================================
来源：http://ivu.shangyingyoupin.top

统计汇总
来源：http://nys.nanxinkj.top

================================================================================
来源：http://ich.meibo888.top

按语言统计（条）：
来源：http://sti.tanke756.top

Python ......... 252
来源：http://brj.hnqzz.top

PHP ............ 252
来源：http://aeh.bbcook.cn

JavaScript ..... 252
来源：http://fsy.haohaochexian.top

TypeScript ..... 212
来源：http://qen.wangshuangyany.cn


<!-- 参考信息 -->