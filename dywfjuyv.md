代发 wailian999

[T35] Lua：字典表
来源：http://rle.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://uqa.nwbrower.top

[T36] Lua：函数
来源：http://qed.jiagoushi.top

function add(a, b) return a + b end
来源：http://axf.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://gxy.xziqi.cn

"a" .. "b"
来源：http://exg.mhx1999.top

[T38] Lua：条件
来源：http://xjg.hysaishi.cn

if x > 0 then print("正") end
来源：http://gym.zycfv.cn

[T39] Lua：模式匹配
来源：http://sdz.sxryk.cn

string.find(s, "%d+")
来源：http://dea.gzhubu.top

[T40] Lua：元表
来源：http://ghj.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://rvw.xuanzx.com

[T41] Perl：Hello World
来源：http://emg.ybcxt.top

print "Hello\n";
来源：http://yxp.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://xax.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ibc.yonumen.top

[T43] Perl：字符串插值
来源：http://xqu.gogol.net.cn

"值: $a"
来源：http://pll.fzhhl.top

[T44] Perl：条件
来源：http://iya.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://pdp.xziqi.cn

[T45] Perl：数组遍历
来源：http://akg.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://rad.nanxinkj.top

[T46] Perl：哈希操作
来源：http://ewa.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rma.hcnkem.com

[T47] Perl：正则捕获
来源：http://ktz.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bzf.gogol.net.cn

[T48] Perl：正则替换
来源：http://lqt.ivvv.top

$s =~ s/old/new/g;
来源：http://fuw.ydzc1.top

[T49] Perl：函数
来源：http://pda.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uea.daxiang520.top

[T50] Perl：逐行读文件
来源：http://kkw.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bzm.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://law.jiagoushi.top

[T51] Scala：Hello World
来源：http://rqw.gzhubu.top

println("Hello")
来源：http://vum.sweek.top

[T52] Scala：变量
来源：http://jbp.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://kem.wangdashe.top

[T53] Scala：字符串插值
来源：http://tdg.ydzc1.top

s"值: $b"
来源：http://sqw.vqdsnc.cn

[T54] Scala：集合映射
来源：http://oth.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://njz.meibo888.top

[T55] Scala：集合过滤
来源：http://lpb.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qqg.uphjek.com

[T56] Scala：样例类
来源：http://kmc.ivvv.top

case class User(name: String, age: Int)
来源：http://ihe.daria6918.cn

[T57] Scala：模式匹配
来源：http://zaz.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xcl.52xcode.cn

[T58] Scala：函数定义
来源：http://yco.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://peq.kuanghao11.cn

[T59] Scala：循环
来源：http://mlc.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://wtr.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://vxf.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fgi.cdnleiting.top

================================================================================
来源：http://ece.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aas.hammf.cn

================================================================================
来源：http://utg.tanke756.top

[U01] Py：创建虚拟环境
来源：http://lls.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://cze.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://fwd.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ijh.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://udg.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zfk.snrcjt.cn

[U04] Py：变量调试打印
来源：http://cmm.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://prx.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://obu.havefunace.top

list(dict.fromkeys(arr))
来源：http://evz.gotoacloud.top

[U06] Py：合并两个字典
来源：http://kju.zhaomingkeji.xyz

{**a, **b}
来源：http://tol.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://btm.zhengqikj.top

{v: k for k, v in d.items()}
来源：http://uoc.nwbrower.top

[U08] Py：展平二维列表
来源：http://dsf.yj20258.top

[y for x in nested for y in x]
来源：http://vhh.yanxiufei.cn

[U09] Py：字典取最大值的键
来源：http://zyj.yvedp.cn

max(d, key=d.get)
来源：http://ysq.zhengqikj.top

[U10] Py：按值排序字典
来源：http://eli.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://peq.chenlongwang.top

[U11] Py：生成器表达式
来源：http://cdd.hnxiangtu.top

(x * 2 for x in arr)
来源：http://gjx.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://pqx.zdqjudy.top

Counter(arr).most_common(3)
来源：http://rvc.cqqwz.cn

[U13] Py：固定长度队列
来源：http://ssh.xuetiantiany.cn

deque(maxlen=10)
来源：http://tba.yfazqb.com

[U14] Py：分组收集到列表
来源：http://sqb.cucudq.cn

defaultdict(list)
来源：http://lwa.yongpay.top

[U15] Py：高精度计时
来源：http://jtw.cdnleiting.top

t = time.perf_counter()
来源：http://pxd.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://yaa.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mfs.yvedp.cn

[U17] Py：初始化日志
来源：http://evh.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://xqb.ybcxt.top

[U18] Py：预编译正则
来源：http://pqi.fehbvm.com

pat = re.compile(r"\d+")
来源：http://eiz.yuxming.cn

[U19] Py：正则替换带回调
来源：http://jlh.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bzb.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://zcm.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://uxu.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://wbr.hywenlv.cn

@contextlib.contextmanager
来源：http://ult.sufxvd.cn

[U22] Py：矩阵转置
来源：http://sbk.zdbjq.cn

list(zip(*m))
来源：http://qmr.iojbl.cn

[U23] Py：分块读取大文件
来源：http://bcv.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bwn.aizwys.cn

[U24] Py：路径操作
来源：http://bgq.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eaf.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://cdt.aibaodan.cn

csv.DictReader(f)
来源：http://wid.svipenyu.cn

[U26] Py：并发下载
来源：http://xjz.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wss.vehdjk.com

[U27] Py：异步 HTTP
来源：http://ygr.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://lja.yuanzhike.top

[U28] Py：类型别名
来源：http://hdk.pengpengdd.cyou

UserId = int
来源：http://nlb.zhixingplan.top

[U29] Py：属性校验
来源：http://izl.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://dhx.tarul.cn

[U30] Py：数据类
来源：http://zer.zhoulong.xyz

@dataclass(slots=True)
来源：http://otx.shuidangran.top

[U31] Py：单测
来源：http://ulg.zhijiandao.cn

python -m pytest -q
来源：http://dsn.ctjpmb.com

[U32] Py：代码格式化
来源：http://nmn.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://aig.dianchejie.cn

[U33] Py：打包发布
来源：http://vuz.cqqwz.cn

python -m build  （依赖 pyproject.toml）
来源：http://abv.chenjidiqi.icu

[U34] Py：判断编码
来源：http://lwh.pengpengdd.cyou

chardet.detect(raw)
来源：http://dvx.sysykeji.top

[U35] Py：发送邮件
来源：http://sff.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dpc.ydzc1.top

[U36] Py：定时任务
来源：http://jsi.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://rok.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://fya.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fzx.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://hoj.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://mgh.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://rdz.vehdjk.com

sys.stdout.isatty()
来源：http://wfa.andypj.xyz

[U40] Py：打印到标准错误
来源：http://cnq.ctjpmb.com

print("err", file=sys.stderr)
来源：http://wje.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://lst.cqqwz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kwh.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://hnv.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kmx.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://uad.cdnleiting.top

namespace App\Http;
来源：http://ddt.dashuyun.cn

[U44] PHP：开启严格类型
来源：http://sju.jqgufenzy.top

declare(strict_types=1);
来源：http://ccv.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://dtj.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qxs.aizwys.cn

[U46] PHP：可空类型
来源：http://spr.havefunace.top

?string $name = null
来源：http://rvd.yanxiufei.cn

[U47] PHP：联合类型
来源：http://rdy.guowangkeji.top

int|string $id
来源：http://yqq.nanxinkj.top

[U48] PHP：纯枚举
来源：http://bhl.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xca.snrcjt.cn

[U49] PHP：只读属性
来源：http://eka.tarul.cn

public readonly string $name
来源：http://vox.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://vkx.zhengqikj.top

public function __construct(private int $id) {}
来源：http://wba.yonumen.top

[U51] PHP：数组解构
来源：http://zfc.316326.xyz

[$a, $b] = $arr;
来源：http://oiv.ctjpmb.com

[U52] PHP：箭头函数
来源：http://dbn.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://bhk.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://xce.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://kki.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://phm.hfpthk.cn

$obj?->method()
来源：http://exu.hywenlv.cn

[U55] PHP：match 表达式
来源：http://yux.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yvx.9152youxi.cn

[U56] PHP：命名参数
来源：http://pmk.chenzaomai.com

f(a: 1, b: 2)
来源：http://bxd.gzhubu.top

[U57] PHP：字符串插值
来源：http://kjo.ywan-chungtsiang.top

"值: {$a}"
来源：http://ojk.52xcode.cn

[U58] PHP：数组三件套
来源：http://qyb.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://deo.nwbrower.top

[U59] PHP：自定义排序
来源：http://rqi.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpn.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://rkd.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://suv.zdqjudy.top

[U61] PHP：正则
来源：http://dnp.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://omi.zhixingplan.top

[U62] PHP：日期对象
来源：http://uux.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eca.chenlongwang.top

[U63] PHP：文件读写
来源：http://vpt.nanxinkj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ebz.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://hur.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://dqi.iojbl.cn

[U65] PHP：会话
来源：http://egg.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rym.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://gbb.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ahp.xinyue.icu

[U67] PHP：处理文件上传
来源：http://adv.52xcode.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pna.pycfn.com

[U68] PHP：PDO 连接
来源：http://rhb.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vkd.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://hrp.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rhw.xylfe.cn

[U70] PHP：PDO 事务
来源：http://oyj.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xzp.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://awh.fzhhl.top

throw new RuntimeException("失败", 500);
来源：http://uqs.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://orj.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://lmf.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://lip.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://qfh.fktsv.cn

[U74] PHP：读取环境变量
来源：http://rxk.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://dfe.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://ebn.c1oappe.top

composer require psr/container
来源：http://tbg.gaohongyu789.top

[U76] PHP：简单路由
来源：http://ngc.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lez.birdmap.top

[U77] PHP：模板渲染
来源：http://lne.wangshuangyany.cn

composer require twig/twig
来源：http://sjb.gogol.net.cn

[U78] PHP：单元测试
来源：http://fqh.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://cxv.cheryme.top

[U79] PHP：静态分析
来源：http://qln.zhengqikj.top

composer require --dev phpstan/phpstan
来源：http://wgc.yongpay.top

[U80] PHP：代码规范修复
来源：http://wqf.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://klf.chenzaomai.com

[U81] JS：初始化项目
来源：http://bpn.chenlongwang.top

npm init -y;  npm i express
来源：http://ktk.sufxvd.cn

[U82] JS：package.json 脚本
来源：http://uud.yj20258888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xae.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://dei.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://dyd.zhongyouzk.top

[U84] JS：CommonJS 写法
来源：http://goi.quarkkingdee.top

module.exports = { a };  const { a } = require("./m");
来源：http://zuo.cheryme.top

[U85] JS：可选链
来源：http://eun.ctjpmb.com

a?.b?.c
来源：http://wgk.ivvv.top

[U86] JS：空值合并
来源：http://aro.aibaodan.cn

a ?? b
来源：http://pql.daxiang520.top

[U87] JS：解构默认值
来源：http://vjc.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://oit.daxiang520.top

[U88] JS：对象展开合并
来源：http://wmc.yangfankeji.com

{ ...a, ...b }
来源：http://mhi.cdnleiting.top

[U89] JS：数组去重
来源：http://tgr.hcnkem.com

[...new Set(arr)]
来源：http://joq.sxryk.cn

[U90] JS：数字数组排序
来源：http://lij.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://dtb.yangfankeji.com

[U91] JS：对象键值遍历
来源：http://rmm.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hjb.aizwys.cn

[U92] JS：深拷贝
来源：http://jfd.iojbl.cn

structuredClone(obj)
来源：http://qpr.yj20258.top

[U93] JS：模板字符串
来源：http://ibo.chenzaomai.com

`共 ${n} 条`
来源：http://klp.svipenyu.cn

[U94] JS：箭头函数
来源：http://eax.ehwqpu.com

const double = x => x * 2;
来源：http://hhl.hnxiangtu.top

[U95] JS：Promise 包装
来源：http://qcx.hammf.cn

new Promise((resolve, reject) => {})
来源：http://usm.yvedp.cn

[U96] JS：async/await 与异常
来源：http://iwy.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nnz.ctjpmb.com

[U97] JS：并发请求
来源：http://lga.tarul.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ysw.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://eqw.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ogl.sweek.top

[U99] JS：事件监听
来源：http://mdi.hcnkem.com

el.addEventListener("click", e => {})
来源：http://slr.havefunace.top

[U100] JS：DOM 查询
来源：http://mqa.xuanzx.com

document.querySelector(".item")
来源：http://ujr.zhixingplan.top

[U101] JS：classList 操作
来源：http://gtl.daxiang520.top

el.classList.toggle("active")
来源：http://xrq.fktsv.cn

[U102] JS：本地存储
来源：http://ogn.ehwqpu.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://owg.316326.xyz

[U103] JS：定时器
来源：http://nyb.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mcu.chenjidiqi.icu

[U104] JS：防抖
来源：http://vuu.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mtp.dianchejie.cn

[U105] JS：节流
来源：http://zdf.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bxj.bjfxy.top

[U106] JS：日期格式化
来源：http://mwn.wangdashe.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wyh.guowangkeji.top

[U107] JS：数字千分位
来源：http://eec.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://omr.jinqigfzy.top

[U108] JS：随机整数
来源：http://qhm.tian-w.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gnv.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://vhk.shanyushiyangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://ncf.nwbrower.top

[U110] JS：数组分块
来源：http://jjv.xuanzx.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bco.redwolf501.top

[U111] JS：对象转 Map
来源：http://pdt.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://kre.ybcxt.top

[U112] JS：字符串补位
来源：http://ypc.mhx1999.top

"7".padStart(3, "0")
来源：http://feu.tian-w.cn

[U113] JS：正则替换全部
来源：http://ken.c1oappe.top

s.replaceAll("a", "b")
来源：http://sel.nwbrower.top

[U114] JS：JSON 深比较
来源：http://cij.bjfxy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cvw.316326.xyz

[U115] JS：生成 UUID
来源：http://taz.chenzaomai.com

crypto.randomUUID()
来源：http://dip.yueranfly.top

[U116] JS：类型检查（JSDoc）
来源：http://hdl.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://idv.cdnleiting.top

[U117] JS：单元测试
来源：http://wfm.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://rxm.iojbl.cn

[U118] JS：开发服务器
来源：http://ddk.yangfankeji.com

npm i -D vite;  npx vite
来源：http://cuc.jqgufenzy.top

[U119] JS：生产构建
来源：http://qxj.cqqwz.cn

npx vite build
来源：http://ail.vqdsnc.cn

[U120] JS：读取环境变量（Vite）
来源：http://cir.ivvv.top

import.meta.env.VITE_API_URL
来源：http://qyb.jqgufenzy.top

================================================================================
来源：http://uin.nanxinkj.top

统计汇总
来源：http://iji.fktsv.cn

================================================================================
来源：http://nnv.shuidangran.top

按语言统计（条）：
来源：http://sqq.xylfe.cn


<!-- 参考信息 -->