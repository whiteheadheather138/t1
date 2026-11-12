代发 wailian999

[T25] Swift：结构体
来源：http://nbw.0kj1m.cn

struct P { var x: Int }
来源：http://arr.gaohongyu789.top

[T26] Swift：类与重写
来源：http://hqn.jinqigufen.top

class A: Base { override func f() {} }
来源：http://tzf.aizwys.cn

[T27] Swift：错误处理
来源：http://jgm.fktsv.cn

do { try f() } catch { print(error) }
来源：http://rab.epnwcf.com

[T28] Swift：枚举
来源：http://nqd.cqqwz.cn

enum Color { case red, green }
来源：http://oat.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://xiz.xziqi.cn

guard let x = opt else { return }
来源：http://nla.hywenlv.cn

[T30] Swift：协议
来源：http://cmt.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://gwe.mhx1999.top

[T31] Lua：Hello World
来源：http://vzi.smart0.xyz

print("Hello")
来源：http://sct.zhixingplan.top

[T32] Lua：局部变量
来源：http://rqs.chenjidiqi.icu

local a = 1
来源：http://xon.52xcode.cn

[T33] Lua：表（数组）
来源：http://ptn.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pww.haohaochexian.top

[T34] Lua：遍历表
来源：http://zhr.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ptd.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://kxq.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://qah.ydzc1.top

[T36] Lua：函数
来源：http://fuu.gzhubu.top

function add(a, b) return a + b end
来源：http://xxq.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://nuq.yanxiufei.cn

"a" .. "b"
来源：http://bpv.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://flm.zhongyouzk.top

if x > 0 then print("正") end
来源：http://kwt.yj202588.top

[T39] Lua：模式匹配
来源：http://kss.hongshengwenyu.top

string.find(s, "%d+")
来源：http://ros.zycfv.cn

[T40] Lua：元表
来源：http://sua.zycfv.cn

setmetatable({}, { __index = base })
来源：http://dkf.xylfe.cn

[T41] Perl：Hello World
来源：http://svf.smart0.xyz

print "Hello\n";
来源：http://nrw.jlsjyb.cn

[T42] Perl：变量类型
来源：http://eve.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gki.birdmap.top

[T43] Perl：字符串插值
来源：http://joe.tianlin.xyz

"值: $a"
来源：http://tnz.fehbvm.com

[T44] Perl：条件
来源：http://xby.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://leo.dianchejie.cn

[T45] Perl：数组遍历
来源：http://wak.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://tlb.hongshengwenyu.top

[T46] Perl：哈希操作
来源：http://yje.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://svt.haohaochexian.top

[T47] Perl：正则捕获
来源：http://uuv.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://urn.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://qcg.tianlin.xyz

$s =~ s/old/new/g;
来源：http://rkg.shanyushiyangtech.top

[T49] Perl：函数
来源：http://pbg.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vdh.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://nrl.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wxj.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://kkw.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://whp.316326.xyz

println("Hello")
来源：http://aet.nanxinkj.top

[T52] Scala：变量
来源：http://fvc.hfpthk.cn

val a = 1;  var b = 2
来源：http://rqk.snrcjt.cn

[T53] Scala：字符串插值
来源：http://agz.shuidangran.top

s"值: $b"
来源：http://isj.ybcxt.top

[T54] Scala：集合映射
来源：http://mrs.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://knu.hammf.cn

[T55] Scala：集合过滤
来源：http://ipt.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://xtq.dianchejie.cn

[T56] Scala：样例类
来源：http://hin.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://tdd.cqqwz.cn

[T57] Scala：模式匹配
来源：http://oqi.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tax.quarkkingdee.top

[T58] Scala：函数定义
来源：http://fkj.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://fel.chenzaomai.com

[T59] Scala：循环
来源：http://rgh.hcnkem.com

for (i <- 1 to 10) println(i)
来源：http://cgq.zhoulong.xyz

[T60] Scala：折叠
来源：http://uhl.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zlj.hnqzz.top

================================================================================
来源：http://gby.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wua.xuetiantiany.cn

================================================================================
来源：http://upr.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://oxg.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://klw.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://chl.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zyo.ctjpmb.com

[U03] Py：加载 .env 配置
来源：http://rgp.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nsm.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://fyh.jianghu66.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://srv.redwolf501.top

[U05] Py：列表去重且保序
来源：http://cmn.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://cub.jinqigufen.top

[U06] Py：合并两个字典
来源：http://zjs.zdqjudy.top

{**a, **b}
来源：http://stq.tian-w.cn

[U07] Py：反转字典键值
来源：http://zzb.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://lur.hfpthk.cn

[U08] Py：展平二维列表
来源：http://qgk.sjlbkw.cn

[y for x in nested for y in x]
来源：http://aur.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://ejg.yuanzhike.top

max(d, key=d.get)
来源：http://wnl.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://fkc.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyl.52xcode.cn

[U11] Py：生成器表达式
来源：http://dbo.gaohongyu789.top

(x * 2 for x in arr)
来源：http://bin.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://dwo.hysaishi.cn

Counter(arr).most_common(3)
来源：http://exd.tian-w.cn

[U13] Py：固定长度队列
来源：http://afz.yuxming.cn

deque(maxlen=10)
来源：http://wrx.jianghu66.top

[U14] Py：分组收集到列表
来源：http://jtk.c1oappe.top

defaultdict(list)
来源：http://zfb.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://jbc.xziqi.cn

t = time.perf_counter()
来源：http://czc.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://teg.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zep.hesvh.cn

[U17] Py：初始化日志
来源：http://foc.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://bju.yj20258.top

[U18] Py：预编译正则
来源：http://wgu.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://oop.meibo888.top

[U19] Py：正则替换带回调
来源：http://lml.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xyu.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://obk.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://eld.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://gkv.xingfuxueyuan.xyz

@contextlib.contextmanager
来源：http://uuz.yangfankeji.com

[U22] Py：矩阵转置
来源：http://tzu.aibaodan.cn

list(zip(*m))
来源：http://bba.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://cdt.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://adg.ydjk.org.cn

[U24] Py：路径操作
来源：http://dol.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gqt.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://ghg.yfazqb.com

csv.DictReader(f)
来源：http://gdt.dianchejie.cn

[U26] Py：并发下载
来源：http://tbx.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wiv.hesvh.cn

[U27] Py：异步 HTTP
来源：http://fro.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://trk.c1oappe.top

[U28] Py：类型别名
来源：http://ils.zycfv.cn

UserId = int
来源：http://dun.yonumen.top

[U29] Py：属性校验
来源：http://xwc.chenlongwang.top

@property 与 @x.setter 配合
来源：http://pen.sysykeji.top

[U30] Py：数据类
来源：http://tsk.hnxiangtu.top

@dataclass(slots=True)
来源：http://dma.yj20258888.top

[U31] Py：单测
来源：http://mvg.hcnkem.com

python -m pytest -q
来源：http://rvh.cucudq.cn

[U32] Py：代码格式化
来源：http://iki.pengpengdd.cyou

ruff format . && ruff check --fix .
来源：http://jvn.mhx1999.top

[U33] Py：打包发布
来源：http://bjf.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://fti.dianchejie.cn

[U34] Py：判断编码
来源：http://whx.ybcxt.top

chardet.detect(raw)
来源：http://bct.zycfv.cn

[U35] Py：发送邮件
来源：http://eel.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nzd.sufxvd.cn

[U36] Py：定时任务
来源：http://rhg.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://vdw.xinyue.icu

[U37] Py：读写 Excel
来源：http://uoa.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://lcf.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://fem.chenlongwang.top

Path(__file__).resolve().parent
来源：http://wye.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://aea.tanke756.top

sys.stdout.isatty()
来源：http://cwk.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://bym.fengsongda.top

print("err", file=sys.stderr)
来源：http://fqh.ybcxt.top

[U41] PHP：初始化 Composer 项目
来源：http://haf.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://drn.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://jeh.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bbw.tian-w.cn

[U43] PHP：声明命名空间
来源：http://fpu.sxryk.cn

namespace App\Http;
来源：http://dmv.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://vvd.pengpengdd.cyou

declare(strict_types=1);
来源：http://uum.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://gyl.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hte.daxiang520.top

[U46] PHP：可空类型
来源：http://ges.aibaodan.cn

?string $name = null
来源：http://dwa.zhoulong.xyz

[U47] PHP：联合类型
来源：http://xtn.316326.xyz

int|string $id
来源：http://pug.dashuyun.cn

[U48] PHP：纯枚举
来源：http://oar.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gbv.hnxiangtu.top

[U49] PHP：只读属性
来源：http://igr.zhixingplan.top

public readonly string $name
来源：http://vjx.svipenyu.cn

[U50] PHP：构造器属性提升
来源：http://lho.svipenyu.cn

public function __construct(private int $id) {}
来源：http://blw.andypj.xyz

[U51] PHP：数组解构
来源：http://pac.hywenlv.cn

[$a, $b] = $arr;
来源：http://yqp.bbcook.cn

[U52] PHP：箭头函数
来源：http://ycw.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://zkd.wangdashe.top

[U53] PHP：空合并运算符
来源：http://yxo.zhijiandao.cn

$v = $a ?? $b ?? "default";
来源：http://zkm.yfazqb.com

[U54] PHP：空安全调用
来源：http://naj.guowangkeji.top

$obj?->method()
来源：http://azs.daria6918.cn

[U55] PHP：match 表达式
来源：http://vrc.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://oqc.jqgufenzy.top

[U56] PHP：命名参数
来源：http://ngt.yj20258888.top

f(a: 1, b: 2)
来源：http://etv.nwbrower.top

[U57] PHP：字符串插值
来源：http://uax.jianghu66.top

"值: {$a}"
来源：http://kdp.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://xmo.hywenlv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://okp.guannengcc.top

[U59] PHP：自定义排序
来源：http://fzc.jinqigfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrg.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://gca.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ktl.zdbjq.cn

[U61] PHP：正则
来源：http://dkh.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ngq.daria6918.cn

[U62] PHP：日期对象
来源：http://xbi.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wrq.tanke756.top

[U63] PHP：文件读写
来源：http://bww.cdnleiting.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fsv.pycfn.com

[U64] PHP：目录遍历
来源：http://hge.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://ihy.jianghu66.top

[U65] PHP：会话
来源：http://aay.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iqf.nanxuanxn.top

[U66] PHP：设置 Cookie
来源：http://wvx.zdqjudy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wum.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://hjy.jinqigfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pgs.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://efx.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mdy.guannengcc.top

[U69] PHP：PDO 预处理
来源：http://bap.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yms.yj20258888.top

[U70] PHP：PDO 事务
来源：http://rfh.vehdjk.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pff.tarul.cn

[U71] PHP：抛出异常
来源：http://jya.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://ccs.zdbjq.cn

[U72] PHP：写错误日志
来源：http://qkb.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://wxy.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://fgs.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://qrx.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://sva.zhixingplan.top

getenv("APP_ENV") ?: "production"
来源：http://kzv.yuanzhike.top

[U75] PHP：依赖注入
来源：http://jdn.shangyingyoupin.top

composer require psr/container
来源：http://ajb.sxryk.cn

[U76] PHP：简单路由
来源：http://win.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ukx.chenlongwang.top

[U77] PHP：模板渲染
来源：http://vlx.zdbjq.cn

composer require twig/twig
来源：http://zfz.ydzc1.top

[U78] PHP：单元测试
来源：http://rzf.epnwcf.com

composer require --dev phpunit/phpunit
来源：http://pcl.ydjk.org.cn

[U79] PHP：静态分析
来源：http://zsl.9152youxi.cn

composer require --dev phpstan/phpstan
来源：http://eil.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://pei.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://okc.iojbl.cn

[U81] JS：初始化项目
来源：http://xpz.haohaochexian.top

npm init -y;  npm i express
来源：http://ezn.uphjek.com

[U82] JS：package.json 脚本
来源：http://oyk.sjlbkw.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gcl.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://dep.hnqzz.top

export const a = 1;  import { a } from "./m.js";
来源：http://byw.xingfuxueyuan.xyz

[U84] JS：CommonJS 写法
来源：http://dfm.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yov.ehwqpu.com

[U85] JS：可选链
来源：http://vzv.yangfankeji.com

a?.b?.c
来源：http://ajr.wangshuangyany.cn

[U86] JS：空值合并
来源：http://pyn.yangfankeji.com

a ?? b
来源：http://uuv.dianchejie.cn

[U87] JS：解构默认值
来源：http://qwg.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://awo.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://mig.ydjk.org.cn

{ ...a, ...b }
来源：http://ojm.aibaodan.cn

[U89] JS：数组去重
来源：http://juv.aizwys.cn

[...new Set(arr)]
来源：http://qtp.chenzaomai.com

[U90] JS：数字数组排序
来源：http://uhp.kuanghao11.cn

[...arr].sort((a, b) => a - b)
来源：http://ukj.yuxming.cn

[U91] JS：对象键值遍历
来源：http://lbm.gaohongyu789.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jja.jinqigfzy.top

[U92] JS：深拷贝
来源：http://pkt.tarul.cn

structuredClone(obj)
来源：http://qyx.yj20258.top

[U93] JS：模板字符串
来源：http://vlp.cashguo.top

`共 ${n} 条`
来源：http://vwu.andypj.xyz

[U94] JS：箭头函数
来源：http://ykh.cashguo.top

const double = x => x * 2;
来源：http://egm.cheryme.top

[U95] JS：Promise 包装
来源：http://lme.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://tfe.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://vfl.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pad.tian-w.cn

[U97] JS：并发请求
来源：http://ugv.316326.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://xyj.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://vwg.chenlongwang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://skk.sjlbkw.cn

[U99] JS：事件监听
来源：http://tjf.c1oappe.top

el.addEventListener("click", e => {})
来源：http://jwd.cheryme.top

[U100] JS：DOM 查询
来源：http://vrz.9152youxi.cn

document.querySelector(".item")
来源：http://hme.cdnleiting.top

[U101] JS：classList 操作
来源：http://erj.pycfn.com

el.classList.toggle("active")
来源：http://aju.zhijiandao.cn

[U102] JS：本地存储
来源：http://zxb.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://upp.dianchejie.cn

[U103] JS：定时器
来源：http://hab.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qea.xinyue.icu

[U104] JS：防抖
来源：http://zez.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nmr.uphjek.com

[U105] JS：节流
来源：http://ldr.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gha.pycfn.com

[U106] JS：日期格式化
来源：http://ndq.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qpc.chenlongwang.top

[U107] JS：数字千分位
来源：http://xnz.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rhd.gogol.net.cn

[U108] JS：随机整数
来源：http://hvn.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vru.jqgfzy.top

[U109] JS：数组分组
来源：http://rmi.vqdsnc.cn

Object.groupBy(arr, x => x.type)
来源：http://ayp.yueranfly.top

[U110] JS：数组分块
来源：http://woo.guowangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vjp.pengpengdd.cyou

[U111] JS：对象转 Map
来源：http://gtc.chenzaomai.com

new Map(Object.entries(obj))
来源：http://vrd.chenzaomai.com

[U112] JS：字符串补位
来源：http://ilb.yuxming.cn

"7".padStart(3, "0")
来源：http://rgi.aibaodan.cn


<!-- 参考信息 -->