代发 wailian999

[T35] Lua：字典表
来源：http://rri.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://nxy.epnwcf.com

[T36] Lua：函数
来源：http://eqv.ehwqpu.com

function add(a, b) return a + b end
来源：http://pqo.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://xmo.yj20258888.top

"a" .. "b"
来源：http://red.birdmap.top

[T38] Lua：条件
来源：http://zry.jiagoushi.top

if x > 0 then print("正") end
来源：http://gng.cashguo.top

[T39] Lua：模式匹配
来源：http://oor.nanxinkj.top

string.find(s, "%d+")
来源：http://eio.haohaochexian.top

[T40] Lua：元表
来源：http://jui.xuanzx.com

setmetatable({}, { __index = base })
来源：http://lhi.wangdashe.top

[T41] Perl：Hello World
来源：http://mxc.0kj1m.cn

print "Hello\n";
来源：http://czl.sxryk.cn

[T42] Perl：变量类型
来源：http://tvu.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zyj.meibo888.top

[T43] Perl：字符串插值
来源：http://obq.vehdjk.com

"值: $a"
来源：http://wnz.sufxvd.cn

[T44] Perl：条件
来源：http://txt.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://joe.yueranfly.top

[T45] Perl：数组遍历
来源：http://xco.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://jgk.zdqjudy.top

[T46] Perl：哈希操作
来源：http://sux.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cme.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://irv.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://sdb.xuanzx.com

[T48] Perl：正则替换
来源：http://xct.316326.xyz

$s =~ s/old/new/g;
来源：http://vlf.wangdashe.top

[T49] Perl：函数
来源：http://ekt.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vyo.tian-w.cn

[T50] Perl：逐行读文件
来源：http://jdo.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://erj.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://sws.hysaishi.cn

[T51] Scala：Hello World
来源：http://pjg.jinghuilouyu.cn

println("Hello")
来源：http://mng.wangdashe.top

[T52] Scala：变量
来源：http://wwx.daxiang520.top

val a = 1;  var b = 2
来源：http://lut.xuanzx.com

[T53] Scala：字符串插值
来源：http://sqk.yanxiufei.cn

s"值: $b"
来源：http://yqk.gotoacloud.top

[T54] Scala：集合映射
来源：http://avy.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://fdq.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://ild.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://emf.chenlongwang.top

[T56] Scala：样例类
来源：http://qvk.yueranfly.top

case class User(name: String, age: Int)
来源：http://cjs.hywenlv.cn

[T57] Scala：模式匹配
来源：http://feu.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uxv.jiagoushi.top

[T58] Scala：函数定义
来源：http://yfi.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xwt.ivvv.top

[T59] Scala：循环
来源：http://xec.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://rok.cashguo.top

[T60] Scala：折叠
来源：http://nwg.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ezr.shzxlz.cn

================================================================================
来源：http://hwr.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://whr.ctjpmb.com

================================================================================
来源：http://qqy.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://rou.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rhm.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://wza.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ycr.316326.xyz

[U03] Py：加载 .env 配置
来源：http://xre.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://uvm.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://xks.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lfg.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://hyz.316326.xyz

list(dict.fromkeys(arr))
来源：http://mbt.hfpthk.cn

[U06] Py：合并两个字典
来源：http://ulh.fzhhl.top

{**a, **b}
来源：http://vhl.316326.xyz

[U07] Py：反转字典键值
来源：http://ueq.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://bwf.xinyue.icu

[U08] Py：展平二维列表
来源：http://ufs.cdnleiting.top

[y for x in nested for y in x]
来源：http://xhq.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://xmr.jinqigfzy.top

max(d, key=d.get)
来源：http://omw.yonumen.top

[U10] Py：按值排序字典
来源：http://zxd.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vpj.redwolf501.top

[U11] Py：生成器表达式
来源：http://ria.haohaochexian.top

(x * 2 for x in arr)
来源：http://vrt.hammf.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fxn.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://yfn.guannengcc.top

[U13] Py：固定长度队列
来源：http://lcy.tarul.cn

deque(maxlen=10)
来源：http://gjv.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://dps.yanxiufei.cn

defaultdict(list)
来源：http://rgr.ivvv.top

[U15] Py：高精度计时
来源：http://wjw.smart0.xyz

t = time.perf_counter()
来源：http://ekv.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://bgh.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://waj.yj20258.top

[U17] Py：初始化日志
来源：http://bbs.andypj.xyz

logging.basicConfig(level=logging.INFO)
来源：http://wds.gogol.net.cn

[U18] Py：预编译正则
来源：http://oft.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://axk.hysaishi.cn

[U19] Py：正则替换带回调
来源：http://lye.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rhf.gzhubu.top

[U20] Py：缓存函数结果
来源：http://ugd.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://khl.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://irw.cheryme.top

@contextlib.contextmanager
来源：http://cmh.jianghu66.top

[U22] Py：矩阵转置
来源：http://mhy.jlsjyb.cn

list(zip(*m))
来源：http://vfv.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://hvq.zycfv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lqf.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://yxw.jinyuanbaomall.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mfc.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://pxp.ydjk.org.cn

csv.DictReader(f)
来源：http://wty.yueranfly.top

[U26] Py：并发下载
来源：http://xmz.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://njo.cashguo.top

[U27] Py：异步 HTTP
来源：http://qsf.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://wdf.bbcook.cn

[U28] Py：类型别名
来源：http://ygs.cheryme.top

UserId = int
来源：http://jvg.hysaishi.cn

[U29] Py：属性校验
来源：http://oag.tanke756.top

@property 与 @x.setter 配合
来源：http://tng.tian-w.cn

[U30] Py：数据类
来源：http://ykn.tanke756.top

@dataclass(slots=True)
来源：http://jif.cqqwz.cn

[U31] Py：单测
来源：http://igg.tianlin.xyz

python -m pytest -q
来源：http://msw.ybcxt.top

[U32] Py：代码格式化
来源：http://ppr.daria6918.cn

ruff format . && ruff check --fix .
来源：http://hiv.zhoulong.xyz

[U33] Py：打包发布
来源：http://xta.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://rhl.xuetiantiany.cn

[U34] Py：判断编码
来源：http://dkf.daxiang520.top

chardet.detect(raw)
来源：http://xrf.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://hzi.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yqc.iojbl.cn

[U36] Py：定时任务
来源：http://blq.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://cjb.0kj1m.cn

[U37] Py：读写 Excel
来源：http://hqk.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://dmm.cdnleiting.top

[U38] Py：获取脚本所在目录
来源：http://vaw.chenzaomai.com

Path(__file__).resolve().parent
来源：http://yvz.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://tcd.wangshuangyany.cn

sys.stdout.isatty()
来源：http://qmk.iojbl.cn

[U40] Py：打印到标准错误
来源：http://sds.hfpthk.cn

print("err", file=sys.stderr)
来源：http://qqa.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://lwj.shanyushiyangtech.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vmt.gogol.net.cn

[U42] PHP：PSR-4 自动加载
来源：http://ssj.zhixingplan.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nqz.birdmap.top

[U43] PHP：声明命名空间
来源：http://igt.jlsjyb.cn

namespace App\Http;
来源：http://mmz.gzhubu.top

[U44] PHP：开启严格类型
来源：http://eqt.birdmap.top

declare(strict_types=1);
来源：http://ssn.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://xpg.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ptf.fengsongda.top

[U46] PHP：可空类型
来源：http://ykq.havefunace.top

?string $name = null
来源：http://dds.yangfankeji.com

[U47] PHP：联合类型
来源：http://dcn.zhoulong.xyz

int|string $id
来源：http://vfh.mhx1999.top

[U48] PHP：纯枚举
来源：http://kac.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://htp.chenzaomai.com

[U49] PHP：只读属性
来源：http://qlb.yanxiufei.cn

public readonly string $name
来源：http://gfa.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://vzp.zdbjq.cn

public function __construct(private int $id) {}
来源：http://xmh.daria6918.cn

[U51] PHP：数组解构
来源：http://ftr.zycfv.cn

[$a, $b] = $arr;
来源：http://fec.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://ezc.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://jrk.kuanghao11.cn

[U53] PHP：空合并运算符
来源：http://ybs.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://tpv.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://rho.ydzc1.top

$obj?->method()
来源：http://cdq.fengsongda.top

[U55] PHP：match 表达式
来源：http://cbm.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kls.zycfv.cn

[U56] PHP：命名参数
来源：http://yts.tanke756.top

f(a: 1, b: 2)
来源：http://duq.ppjwa.cn

[U57] PHP：字符串插值
来源：http://msq.havefunace.top

"值: {$a}"
来源：http://hnx.hesvh.cn

[U58] PHP：数组三件套
来源：http://jli.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ldp.gogol.net.cn

[U59] PHP：自定义排序
来源：http://dez.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ytr.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://vvj.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dpv.nanxinkj.top

[U61] PHP：正则
来源：http://qdy.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bwh.daria6918.cn

[U62] PHP：日期对象
来源：http://lzy.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gng.ppjwa.cn

[U63] PHP：文件读写
来源：http://agi.epnwcf.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uvc.tian-w.cn

[U64] PHP：目录遍历
来源：http://rvr.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://jfv.nanxuanxn.top

[U65] PHP：会话
来源：http://kmp.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://flq.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://xjw.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hyb.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://kai.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wlc.yfazqb.com

[U68] PHP：PDO 连接
来源：http://kdl.guowangkeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ecp.gotoacloud.top

[U69] PHP：PDO 预处理
来源：http://dut.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pur.guannengcc.top

[U70] PHP：PDO 事务
来源：http://ikv.feifeiyinyue.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://csv.cqqwz.cn

[U71] PHP：抛出异常
来源：http://ypy.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://iuo.chenzaomai.com

[U72] PHP：写错误日志
来源：http://imc.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://ris.fengsongda.top

[U73] PHP：读取 ini 配置
来源：http://nfv.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://cey.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://bwl.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://zox.pycfn.com

[U75] PHP：依赖注入
来源：http://jxx.zdbjq.cn

composer require psr/container
来源：http://uva.zhoulong.xyz

[U76] PHP：简单路由
来源：http://xhh.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ech.hywenlv.cn

[U77] PHP：模板渲染
来源：http://jig.tianlin.xyz

composer require twig/twig
来源：http://quf.gogol.net.cn

[U78] PHP：单元测试
来源：http://lgg.ivvv.top

composer require --dev phpunit/phpunit
来源：http://xxe.jqgfzy.top

[U79] PHP：静态分析
来源：http://wsh.jinqigufen.top

composer require --dev phpstan/phpstan
来源：http://xbo.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://mdh.hongshengwenyu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qbh.sjlbkw.cn

[U81] JS：初始化项目
来源：http://ccg.yuxming.cn

npm init -y;  npm i express
来源：http://uts.bbcook.cn

[U82] JS：package.json 脚本
来源：http://zmh.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dqw.sjlbkw.cn

[U83] JS：ES Module 导入导出
来源：http://yyy.0kj1m.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qqx.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://brb.jinghuilouyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nct.nwbrower.top

[U85] JS：可选链
来源：http://dxh.yangfankeji.com

a?.b?.c
来源：http://vyf.ybcxt.top

[U86] JS：空值合并
来源：http://dfi.zhoulong.xyz

a ?? b
来源：http://xpn.daxiang520.top

[U87] JS：解构默认值
来源：http://azi.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://olx.dianchejie.cn

[U88] JS：对象展开合并
来源：http://naj.hnqzz.top

{ ...a, ...b }
来源：http://nwh.zycfv.cn

[U89] JS：数组去重
来源：http://wsg.yuanzhike.top

[...new Set(arr)]
来源：http://rgl.gzhubu.top

[U90] JS：数字数组排序
来源：http://xor.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://gkn.daria6918.cn

[U91] JS：对象键值遍历
来源：http://msu.fehbvm.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wyp.ybcxt.top

[U92] JS：深拷贝
来源：http://eze.shuidangran.top

structuredClone(obj)
来源：http://pha.andypj.xyz

[U93] JS：模板字符串
来源：http://uvi.sweek.top

`共 ${n} 条`
来源：http://nwx.iojbl.cn

[U94] JS：箭头函数
来源：http://gcp.yueranfly.top

const double = x => x * 2;
来源：http://gld.shuidangran.top

[U95] JS：Promise 包装
来源：http://nid.zhiwuduotai.top

new Promise((resolve, reject) => {})
来源：http://dnh.hesvh.cn

[U96] JS：async/await 与异常
来源：http://buk.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tmr.hfpthk.cn

[U97] JS：并发请求
来源：http://dud.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oho.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://ubp.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ovh.ywan-chungtsiang.top

[U99] JS：事件监听
来源：http://bbv.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://flf.haohaochexian.top

[U100] JS：DOM 查询
来源：http://iqn.xuetiantiany.cn

document.querySelector(".item")
来源：http://tnk.jianghu66.top

[U101] JS：classList 操作
来源：http://akk.jlsjyb.cn

el.classList.toggle("active")
来源：http://sep.ybcxt.top

[U102] JS：本地存储
来源：http://rsj.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tol.iojbl.cn

[U103] JS：定时器
来源：http://fhw.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ooz.vehdjk.com

[U104] JS：防抖
来源：http://jma.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lim.316326.xyz

[U105] JS：节流
来源：http://cgi.zhaomingkeji.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xkw.yfazqb.com

[U106] JS：日期格式化
来源：http://lph.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iiw.wangdashe.top

[U107] JS：数字千分位
来源：http://yms.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jxn.sysykeji.top

[U108] JS：随机整数
来源：http://vfz.iojbl.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gzg.andypj.xyz

[U109] JS：数组分组
来源：http://fgy.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://fre.chenjidiqi.icu

[U110] JS：数组分块
来源：http://gaf.mhx1999.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vty.zhengqikj.top

[U111] JS：对象转 Map
来源：http://lzc.epnwcf.com

new Map(Object.entries(obj))
来源：http://txi.fengsongda.top

[U112] JS：字符串补位
来源：http://ntu.jyoumei.cn

"7".padStart(3, "0")
来源：http://rrn.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://dnz.shuidangran.top

s.replaceAll("a", "b")
来源：http://fuu.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://vmk.ehwqpu.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://chm.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://dii.fengsongda.top

crypto.randomUUID()
来源：http://lnd.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://tfh.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://quw.fzhhl.top

[U117] JS：单元测试
来源：http://aeq.birdmap.top

npm i -D vitest;  npx vitest
来源：http://wck.gotoacloud.top

[U118] JS：开发服务器
来源：http://zrj.svipenyu.cn

npm i -D vite;  npx vite
来源：http://wko.andypj.xyz

[U119] JS：生产构建
来源：http://dip.zhongyouzk.top

npx vite build
来源：http://msm.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://uem.yongpay.top

import.meta.env.VITE_API_URL
来源：http://lth.xinyue.icu

================================================================================
来源：http://zxg.gotoacloud.top

统计汇总
来源：http://yau.ydzc1.top

================================================================================
来源：http://nqg.shangyingyoupin.top

按语言统计（条）：
来源：http://ynn.pycfn.com


<!-- 参考信息 -->