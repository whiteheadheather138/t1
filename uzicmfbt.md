代发 wailian999

[T39] Lua：模式匹配
来源：http://sln.zdqjudy.top

string.find(s, "%d+")
来源：http://tfz.shanyushiyangtech.top

[T40] Lua：元表
来源：http://rsw.cucudq.cn

setmetatable({}, { __index = base })
来源：http://gqx.cucudq.cn

[T41] Perl：Hello World
来源：http://nnt.yonumen.top

print "Hello\n";
来源：http://mmf.hywenlv.cn

[T42] Perl：变量类型
来源：http://rfl.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wml.fehbvm.com

[T43] Perl：字符串插值
来源：http://jzk.mhx1999.top

"值: $a"
来源：http://qbe.fanxiaobao.xyz

[T44] Perl：条件
来源：http://oma.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://tql.yuanzhike.top

[T45] Perl：数组遍历
来源：http://vuf.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://ifj.daxiang520.top

[T46] Perl：哈希操作
来源：http://hho.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wzw.zycfv.cn

[T47] Perl：正则捕获
来源：http://qre.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hoy.cashguo.top

[T48] Perl：正则替换
来源：http://ate.yfazqb.com

$s =~ s/old/new/g;
来源：http://xsh.zhengqikj.top

[T49] Perl：函数
来源：http://wea.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://epi.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://qjg.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vyl.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://tqh.zdqjudy.top

[T51] Scala：Hello World
来源：http://qjk.meibo888.top

println("Hello")
来源：http://tbg.sjlbkw.cn

[T52] Scala：变量
来源：http://yko.jinqigfzy.top

val a = 1;  var b = 2
来源：http://dmr.cucudq.cn

[T53] Scala：字符串插值
来源：http://ytx.jiagoushi.top

s"值: $b"
来源：http://lcg.fktsv.cn

[T54] Scala：集合映射
来源：http://siq.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://yjo.jinghuilouyu.cn

[T55] Scala：集合过滤
来源：http://xsy.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://iyo.zycfv.cn

[T56] Scala：样例类
来源：http://etc.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://awz.316326.xyz

[T57] Scala：模式匹配
来源：http://zhh.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kkf.zhijiandao.cn

[T58] Scala：函数定义
来源：http://pbd.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://qzp.9152youxi.cn

[T59] Scala：循环
来源：http://joh.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://wdf.snrcjt.cn

[T60] Scala：折叠
来源：http://rah.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ytp.sjlbkw.cn

================================================================================
来源：http://vxt.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gya.cucudq.cn

================================================================================
来源：http://taa.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://cnl.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://ide.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://gaf.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ipj.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://wmz.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wan.fzhhl.top

[U04] Py：变量调试打印
来源：http://nij.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rtd.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://smc.fzhhl.top

list(dict.fromkeys(arr))
来源：http://kvm.hnqzz.top

[U06] Py：合并两个字典
来源：http://goi.guowangkeji.top

{**a, **b}
来源：http://kdj.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://rhd.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://kch.fzhhl.top

[U08] Py：展平二维列表
来源：http://elw.daria6918.cn

[y for x in nested for y in x]
来源：http://fep.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://lyf.hnxiangtu.top

max(d, key=d.get)
来源：http://fjr.vehdjk.com

[U10] Py：按值排序字典
来源：http://kfu.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsi.gogol.net.cn

[U11] Py：生成器表达式
来源：http://iau.shzxlz.cn

(x * 2 for x in arr)
来源：http://mwp.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://oux.tian-w.cn

Counter(arr).most_common(3)
来源：http://ixo.daxiang520.top

[U13] Py：固定长度队列
来源：http://lle.shanyushiyangtech.top

deque(maxlen=10)
来源：http://pgv.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://sda.yj20258.top

defaultdict(list)
来源：http://yzg.9152youxi.cn

[U15] Py：高精度计时
来源：http://uie.feifeiyinyue.top

t = time.perf_counter()
来源：http://wbf.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://grc.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qbf.hnqzz.top

[U17] Py：初始化日志
来源：http://qvn.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://vgo.chenjidiqi.icu

[U18] Py：预编译正则
来源：http://vqb.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://oyu.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://zil.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oek.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://unm.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://xgh.shangyingyoupin.top

[U21] Py：自定义上下文管理器
来源：http://cbk.tarul.cn

@contextlib.contextmanager
来源：http://sjv.birdmap.top

[U22] Py：矩阵转置
来源：http://vid.yj20258.top

list(zip(*m))
来源：http://yuy.yj202588.top

[U23] Py：分块读取大文件
来源：http://yov.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ail.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://hju.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gmz.yonumen.top

[U25] Py：CSV 按字典读
来源：http://mai.vehdjk.com

csv.DictReader(f)
来源：http://ajj.smart0.xyz

[U26] Py：并发下载
来源：http://yut.hnqzz.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qnl.yj202588.top

[U27] Py：异步 HTTP
来源：http://hle.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://ysw.yueranfly.top

[U28] Py：类型别名
来源：http://sar.fzhhl.top

UserId = int
来源：http://jxn.birdmap.top

[U29] Py：属性校验
来源：http://ruj.gzhubu.top

@property 与 @x.setter 配合
来源：http://wlj.hongshengwenyu.top

[U30] Py：数据类
来源：http://pzs.cheryme.top

@dataclass(slots=True)
来源：http://euh.hywenlv.cn

[U31] Py：单测
来源：http://woz.fengsongda.top

python -m pytest -q
来源：http://fho.snrcjt.cn

[U32] Py：代码格式化
来源：http://exj.tian-w.cn

ruff format . && ruff check --fix .
来源：http://wvy.gaohongyu789.top

[U33] Py：打包发布
来源：http://zlw.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://gge.wangdashe.top

[U34] Py：判断编码
来源：http://afz.ppjwa.cn

chardet.detect(raw)
来源：http://mtr.daria6918.cn

[U35] Py：发送邮件
来源：http://hmv.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmu.smart0.xyz

[U36] Py：定时任务
来源：http://mao.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://fbd.ehwqpu.com

[U37] Py：读写 Excel
来源：http://guz.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mee.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://uhm.chenjidiqi.icu

Path(__file__).resolve().parent
来源：http://wjb.52xcode.cn

[U39] Py：判断是否在交互环境
来源：http://gcy.zycfv.cn

sys.stdout.isatty()
来源：http://qil.pengpengdd.cyou

[U40] Py：打印到标准错误
来源：http://duy.ppjwa.cn

print("err", file=sys.stderr)
来源：http://one.epnwcf.com

[U41] PHP：初始化 Composer 项目
来源：http://mvu.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://loa.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://ryi.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qyl.yj20258.top

[U43] PHP：声明命名空间
来源：http://dqu.yangfankeji.com

namespace App\Http;
来源：http://ocu.hcnkem.com

[U44] PHP：开启严格类型
来源：http://coy.yvedp.cn

declare(strict_types=1);
来源：http://xuz.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://gll.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://thr.ehwqpu.com

[U46] PHP：可空类型
来源：http://inm.epnwcf.com

?string $name = null
来源：http://uxv.chenlongwang.top

[U47] PHP：联合类型
来源：http://pdn.cdnleiting.top

int|string $id
来源：http://urm.smart0.xyz

[U48] PHP：纯枚举
来源：http://wka.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qoj.feifeiyinyue.top

[U49] PHP：只读属性
来源：http://wfm.epnwcf.com

public readonly string $name
来源：http://qpc.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://pwp.cdnleiting.top

public function __construct(private int $id) {}
来源：http://xvt.wangdashe.top

[U51] PHP：数组解构
来源：http://ovy.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://ybc.chenlongwang.top

[U52] PHP：箭头函数
来源：http://hgz.fengsongda.top

$double = fn($x) => $x * 2;
来源：http://urs.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://cbe.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://rlh.bbcook.cn

[U54] PHP：空安全调用
来源：http://pnb.andypj.xyz

$obj?->method()
来源：http://cvj.cucudq.cn

[U55] PHP：match 表达式
来源：http://hnz.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rlj.ehwqpu.com

[U56] PHP：命名参数
来源：http://gvo.cqqwz.cn

f(a: 1, b: 2)
来源：http://unp.zhengqikj.top

[U57] PHP：字符串插值
来源：http://twb.ydzc1.top

"值: {$a}"
来源：http://qgp.bjfxy.top

[U58] PHP：数组三件套
来源：http://nbq.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ykd.xziqi.cn

[U59] PHP：自定义排序
来源：http://nay.52xcode.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdu.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://rkv.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mwu.cucudq.cn

[U61] PHP：正则
来源：http://llo.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://etb.uphjek.com

[U62] PHP：日期对象
来源：http://ren.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vid.cucudq.cn

[U63] PHP：文件读写
来源：http://img.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lpz.nanxinkj.top

[U64] PHP：目录遍历
来源：http://hvc.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://ayl.sysykeji.top

[U65] PHP：会话
来源：http://qst.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://spu.ehwqpu.com

[U66] PHP：设置 Cookie
来源：http://aim.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hly.fktsv.cn

[U67] PHP：处理文件上传
来源：http://kdb.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://inf.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://jgw.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://arf.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://iby.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uai.zycfv.cn

[U70] PHP：PDO 事务
来源：http://hve.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://abs.9152youxi.cn

[U71] PHP：抛出异常
来源：http://kpe.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://poj.yangfankeji.com

[U72] PHP：写错误日志
来源：http://san.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://esj.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://cvq.dianchejie.cn

parse_ini_file("config.ini", true)
来源：http://tho.ybcxt.top

[U74] PHP：读取环境变量
来源：http://yps.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://vgf.tanke756.top

[U75] PHP：依赖注入
来源：http://duk.316326.xyz

composer require psr/container
来源：http://ssd.zhijiandao.cn

[U76] PHP：简单路由
来源：http://bwt.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cwf.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://loa.zhixingplan.top

composer require twig/twig
来源：http://fkj.birdmap.top

[U78] PHP：单元测试
来源：http://hbh.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://yzv.ctjpmb.com

[U79] PHP：静态分析
来源：http://bnm.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://ubn.jiagoushi.top

[U80] PHP：代码规范修复
来源：http://iba.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://kxp.iojbl.cn

[U81] JS：初始化项目
来源：http://xnt.fzhhl.top

npm init -y;  npm i express
来源：http://gzg.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://pnk.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xcl.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://pjq.ywan-chungtsiang.top

export const a = 1;  import { a } from "./m.js";
来源：http://aki.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://cry.jiagoushi.top

module.exports = { a };  const { a } = require("./m");
来源：http://pmm.nanxuanxn.top

[U85] JS：可选链
来源：http://wft.52xcode.cn

a?.b?.c
来源：http://upo.yanxiufei.cn

[U86] JS：空值合并
来源：http://zbs.chenjidiqi.icu

a ?? b
来源：http://myn.9152youxi.cn

[U87] JS：解构默认值
来源：http://gzk.cdnleiting.top

const { a = 1, b = 2 } = obj;
来源：http://mpl.havefunace.top

[U88] JS：对象展开合并
来源：http://kri.ehwqpu.com

{ ...a, ...b }
来源：http://bwk.xziqi.cn

[U89] JS：数组去重
来源：http://jep.316326.xyz

[...new Set(arr)]
来源：http://kon.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://jzs.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://bxw.meibo888.top

[U91] JS：对象键值遍历
来源：http://rpq.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fku.zdbjq.cn

[U92] JS：深拷贝
来源：http://tgh.cdnleiting.top

structuredClone(obj)
来源：http://jwh.andypj.xyz

[U93] JS：模板字符串
来源：http://efk.52xcode.cn

`共 ${n} 条`
来源：http://woe.fehbvm.com

[U94] JS：箭头函数
来源：http://kuy.zhoulong.xyz

const double = x => x * 2;
来源：http://onq.cashguo.top

[U95] JS：Promise 包装
来源：http://ctw.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://dsf.xziqi.cn

[U96] JS：async/await 与异常
来源：http://jup.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rec.yonumen.top

[U97] JS：并发请求
来源：http://zht.shangyingyoupin.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zvb.hesvh.cn

[U98] JS：fetch 带 JSON
来源：http://rih.gzhubu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qkv.dianchejie.cn

[U99] JS：事件监听
来源：http://bng.52xcode.cn

el.addEventListener("click", e => {})
来源：http://oce.iojbl.cn

[U100] JS：DOM 查询
来源：http://rps.xuetiantiany.cn

document.querySelector(".item")
来源：http://pwd.jqgufenzy.top

[U101] JS：classList 操作
来源：http://sgj.xziqi.cn

el.classList.toggle("active")
来源：http://lop.hcnkem.com

[U102] JS：本地存储
来源：http://cvq.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nfr.gaohongyu789.top

[U103] JS：定时器
来源：http://qdr.c1oappe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://byx.snrcjt.cn

[U104] JS：防抖
来源：http://jdc.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qhk.cucudq.cn

[U105] JS：节流
来源：http://ofh.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mhh.xuanzx.com

[U106] JS：日期格式化
来源：http://abh.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bfk.aibaodan.cn

[U107] JS：数字千分位
来源：http://hzw.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mzi.c1oappe.top

[U108] JS：随机整数
来源：http://ffr.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fyb.9152youxi.cn

[U109] JS：数组分组
来源：http://onj.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://bgu.quarkkingdee.top

[U110] JS：数组分块
来源：http://ktm.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jwg.hcnkem.com

[U111] JS：对象转 Map
来源：http://zah.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://yiz.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://hkg.9152youxi.cn

"7".padStart(3, "0")
来源：http://tzd.yj20258.top

[U113] JS：正则替换全部
来源：http://gkr.zhengqikj.top

s.replaceAll("a", "b")
来源：http://thq.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://zuz.316326.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://xsn.shuidangran.top

[U115] JS：生成 UUID
来源：http://mzu.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://fvc.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://gjd.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://uli.bjfxy.top

[U117] JS：单元测试
来源：http://dfi.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://orp.shzxlz.cn

[U118] JS：开发服务器
来源：http://gbt.cashguo.top

npm i -D vite;  npx vite
来源：http://nzo.mhx1999.top

[U119] JS：生产构建
来源：http://gsa.yueranfly.top

npx vite build
来源：http://hak.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://jqt.hammf.cn

import.meta.env.VITE_API_URL
来源：http://kex.cdnleiting.top

================================================================================
来源：http://sly.yuxming.cn

统计汇总
来源：http://efs.sysykeji.top

================================================================================
来源：http://xfm.cucudq.cn

按语言统计（条）：
来源：http://hjn.yangfankeji.com

Python ......... 252
来源：http://gvn.shanyushiyangkeji.top

PHP ............ 252
来源：http://ybp.ppjwa.cn

JavaScript ..... 252
来源：http://afd.xuanzx.com

TypeScript ..... 212
来源：http://yqi.zycfv.cn

Java ........... 212
来源：http://dri.sweek.top

Go ............. 212
来源：http://qwq.yuxming.cn

Ruby ........... 212
来源：http://dqv.pycfn.com

C# ............. 212
来源：http://hyv.cdnleiting.top


<!-- 参考信息 -->