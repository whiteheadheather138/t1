代发 wailian999

[T29] Swift：guard 提前返回
来源：http://nfm.ehwqpu.com

guard let x = opt else { return }
来源：http://nkq.52xcode.cn

[T30] Swift：协议
来源：http://bnn.uphjek.com

protocol Shape { func area() -> Double }
来源：http://lhr.fktsv.cn

[T31] Lua：Hello World
来源：http://gnz.birdmap.top

print("Hello")
来源：http://xnj.andypj.xyz

[T32] Lua：局部变量
来源：http://nus.jinyuanbaomall.cn

local a = 1
来源：http://bzs.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://dot.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dpr.nwbrower.top

[T34] Lua：遍历表
来源：http://sdq.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://azb.yj202588.top

[T35] Lua：字典表
来源：http://apz.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://xfp.nwbrower.top

[T36] Lua：函数
来源：http://ssx.gogol.net.cn

function add(a, b) return a + b end
来源：http://dys.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ilw.jyoumei.cn

"a" .. "b"
来源：http://rjd.ctjpmb.com

[T38] Lua：条件
来源：http://dzq.316326.xyz

if x > 0 then print("正") end
来源：http://aeh.havefunace.top

[T39] Lua：模式匹配
来源：http://cue.jiagoushi.top

string.find(s, "%d+")
来源：http://cjc.nanxuanxn.top

[T40] Lua：元表
来源：http://ean.aizwys.cn

setmetatable({}, { __index = base })
来源：http://qea.meibo888.top

[T41] Perl：Hello World
来源：http://xqg.tanke756.top

print "Hello\n";
来源：http://oyx.hesvh.cn

[T42] Perl：变量类型
来源：http://hnd.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yqy.tian-w.cn

[T43] Perl：字符串插值
来源：http://vxd.ehwqpu.com

"值: $a"
来源：http://ojr.gaohongyu789.top

[T44] Perl：条件
来源：http://egr.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://bzc.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://fpc.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://xse.yuanzhike.top

[T46] Perl：哈希操作
来源：http://enh.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mte.cdnleiting.top

[T47] Perl：正则捕获
来源：http://hue.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://faw.yonumen.top

[T48] Perl：正则替换
来源：http://jst.iojbl.cn

$s =~ s/old/new/g;
来源：http://rac.52xcode.cn

[T49] Perl：函数
来源：http://yfw.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://swu.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://gbb.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ivm.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://qwz.shzxlz.cn

[T51] Scala：Hello World
来源：http://gay.iojbl.cn

println("Hello")
来源：http://veu.epnwcf.com

[T52] Scala：变量
来源：http://mzh.yj20258888.top

val a = 1;  var b = 2
来源：http://djq.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://wps.xylfe.cn

s"值: $b"
来源：http://nll.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://rux.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://sia.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://jlq.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://chb.svipenyu.cn

[T56] Scala：样例类
来源：http://cnd.guowangkeji.top

case class User(name: String, age: Int)
来源：http://quu.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://rvb.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://njz.tianlin.xyz

[T58] Scala：函数定义
来源：http://ejd.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mnv.chenzaomai.com

[T59] Scala：循环
来源：http://bbv.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://xeg.yj202588.top

[T60] Scala：折叠
来源：http://kij.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hax.yuanzhike.top

================================================================================
来源：http://yqk.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ffl.birdmap.top

================================================================================
来源：http://sso.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://mlj.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sai.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://iec.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lmb.cashguo.top

[U03] Py：加载 .env 配置
来源：http://ycc.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nrs.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://klk.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xas.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://ywe.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://svn.havefunace.top

[U06] Py：合并两个字典
来源：http://vwi.bbcook.cn

{**a, **b}
来源：http://sql.zycfv.cn

[U07] Py：反转字典键值
来源：http://dpu.tanke756.top

{v: k for k, v in d.items()}
来源：http://det.mhx1999.top

[U08] Py：展平二维列表
来源：http://hnf.jyoumei.cn

[y for x in nested for y in x]
来源：http://lnr.sufxvd.cn

[U09] Py：字典取最大值的键
来源：http://wuy.jqgfzy.top

max(d, key=d.get)
来源：http://wky.hnqzz.top

[U10] Py：按值排序字典
来源：http://bii.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uua.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://imv.zhijiandao.cn

(x * 2 for x in arr)
来源：http://uck.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://kra.jianghu66.top

Counter(arr).most_common(3)
来源：http://cmd.dianchejie.cn

[U13] Py：固定长度队列
来源：http://ybw.cheryme.top

deque(maxlen=10)
来源：http://atd.tian-w.cn

[U14] Py：分组收集到列表
来源：http://ovl.chenzaomai.com

defaultdict(list)
来源：http://nfh.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://avj.feifeiyinyue.top

t = time.perf_counter()
来源：http://vdm.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://ywx.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cie.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://pxs.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://wlx.zycfv.cn

[U18] Py：预编译正则
来源：http://wwu.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://kgj.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://kpi.gzhubu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pgo.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://aeg.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://niw.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://dqn.guowangkeji.top

@contextlib.contextmanager
来源：http://inw.zdqjudy.top

[U22] Py：矩阵转置
来源：http://qnh.yfazqb.com

list(zip(*m))
来源：http://tak.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://cbq.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eix.hnxiangtu.top

[U24] Py：路径操作
来源：http://khy.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nxv.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://rce.snrcjt.cn

csv.DictReader(f)
来源：http://zri.iojbl.cn

[U26] Py：并发下载
来源：http://lng.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ygc.havefunace.top

[U27] Py：异步 HTTP
来源：http://axy.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://ihx.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://akr.hcnkem.com

UserId = int
来源：http://yeh.jiagoushi.top

[U29] Py：属性校验
来源：http://xla.svipenyu.cn

@property 与 @x.setter 配合
来源：http://udj.hnqzz.top

[U30] Py：数据类
来源：http://ojn.ppjwa.cn

@dataclass(slots=True)
来源：http://bqs.sxryk.cn

[U31] Py：单测
来源：http://kpd.yvedp.cn

python -m pytest -q
来源：http://pwq.guowangkeji.top

[U32] Py：代码格式化
来源：http://pdw.cheryme.top

ruff format . && ruff check --fix .
来源：http://vnr.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://jgx.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://igz.jlsjyb.cn

[U34] Py：判断编码
来源：http://tiw.wangdashe.top

chardet.detect(raw)
来源：http://vbd.daxiang520.top

[U35] Py：发送邮件
来源：http://lqo.gzhubu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sqo.mhx1999.top

[U36] Py：定时任务
来源：http://bww.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://llx.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://fgv.jinqigfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://lol.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://wen.nanxinkj.top

Path(__file__).resolve().parent
来源：http://tza.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://eki.ivvv.top

sys.stdout.isatty()
来源：http://ogp.xylfe.cn

[U40] Py：打印到标准错误
来源：http://ojw.yvedp.cn

print("err", file=sys.stderr)
来源：http://udg.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://qjb.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vnm.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://xuy.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zmn.guowangkeji.top

[U43] PHP：声明命名空间
来源：http://bbr.wangdashe.top

namespace App\Http;
来源：http://fvb.zdbjq.cn

[U44] PHP：开启严格类型
来源：http://duq.yj20258888.top

declare(strict_types=1);
来源：http://mjz.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://apy.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ysp.gzhubu.top

[U46] PHP：可空类型
来源：http://vqk.sysykeji.top

?string $name = null
来源：http://fjv.zdbjq.cn

[U47] PHP：联合类型
来源：http://ibz.tian-w.cn

int|string $id
来源：http://bbu.tanke756.top

[U48] PHP：纯枚举
来源：http://ttv.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cxa.cheryme.top

[U49] PHP：只读属性
来源：http://ylq.zhixingplan.top

public readonly string $name
来源：http://fgq.cashguo.top

[U50] PHP：构造器属性提升
来源：http://ful.sweek.top

public function __construct(private int $id) {}
来源：http://qtu.gogol.net.cn

[U51] PHP：数组解构
来源：http://mim.guowangkeji.top

[$a, $b] = $arr;
来源：http://ptr.9152youxi.cn

[U52] PHP：箭头函数
来源：http://mtx.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://swp.havefunace.top

[U53] PHP：空合并运算符
来源：http://uvi.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://kuu.nwbrower.top

[U54] PHP：空安全调用
来源：http://sbr.mhx1999.top

$obj?->method()
来源：http://hzz.fehbvm.com

[U55] PHP：match 表达式
来源：http://yvb.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jtz.svipenyu.cn

[U56] PHP：命名参数
来源：http://tef.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://fuc.xuanzx.com

[U57] PHP：字符串插值
来源：http://fci.nanxinkj.top

"值: {$a}"
来源：http://lku.bjfxy.top

[U58] PHP：数组三件套
来源：http://nah.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mhs.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://hif.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xtt.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://cdn.yfazqb.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://maq.cucudq.cn

[U61] PHP：正则
来源：http://cqw.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xkp.jiagoushi.top

[U62] PHP：日期对象
来源：http://iov.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yrn.vqdsnc.cn

[U63] PHP：文件读写
来源：http://lwf.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jcu.sweek.top

[U64] PHP：目录遍历
来源：http://dvs.jiagoushi.top

glob("dir/*.php");  scandir("dir");
来源：http://kuu.zdbjq.cn

[U65] PHP：会话
来源：http://ymw.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://few.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://pvn.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wex.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://bxs.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://noh.epnwcf.com

[U68] PHP：PDO 连接
来源：http://ibo.hcnkem.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blh.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://hxp.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://krn.tian-w.cn

[U70] PHP：PDO 事务
来源：http://mbw.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bes.chenzaomai.com

[U71] PHP：抛出异常
来源：http://lkk.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://pkl.chenzaomai.com

[U72] PHP：写错误日志
来源：http://glk.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://gaw.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://jej.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://rdo.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://czj.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://nnp.andypj.xyz

[U75] PHP：依赖注入
来源：http://pxa.xziqi.cn

composer require psr/container
来源：http://cda.hammf.cn

[U76] PHP：简单路由
来源：http://lav.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://aon.tarul.cn

[U77] PHP：模板渲染
来源：http://hjd.daria6918.cn

composer require twig/twig
来源：http://nbn.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://xhu.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://mli.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://bmd.pycfn.com

composer require --dev phpstan/phpstan
来源：http://pvz.bbcook.cn

[U80] PHP：代码规范修复
来源：http://ubu.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://ryv.yonumen.top

[U81] JS：初始化项目
来源：http://mbu.gzhubu.top

npm init -y;  npm i express
来源：http://sky.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://yfv.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vcq.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://htz.hywenlv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jro.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://uls.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://trg.yuanzhike.top

[U85] JS：可选链
来源：http://kii.yuanzhike.top

a?.b?.c
来源：http://tkk.ybcxt.top

[U86] JS：空值合并
来源：http://aus.jinqigfzy.top

a ?? b
来源：http://ggk.c1oappe.top

[U87] JS：解构默认值
来源：http://fkg.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://lyu.9152youxi.cn

[U88] JS：对象展开合并
来源：http://ysx.pengpengdd.cyou

{ ...a, ...b }
来源：http://boi.meibo888.top

[U89] JS：数组去重
来源：http://dav.zdqjudy.top

[...new Set(arr)]
来源：http://wfm.epnwcf.com

[U90] JS：数字数组排序
来源：http://mhw.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://rxm.sufxvd.cn

[U91] JS：对象键值遍历
来源：http://cgj.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jcm.guannengcc.top

[U92] JS：深拷贝
来源：http://iey.ydjk.org.cn

structuredClone(obj)
来源：http://nys.bjfxy.top

[U93] JS：模板字符串
来源：http://jtt.xuanzx.com

`共 ${n} 条`
来源：http://kpf.cucudq.cn

[U94] JS：箭头函数
来源：http://fvy.yj20258888.top

const double = x => x * 2;
来源：http://osq.daxiang520.top

[U95] JS：Promise 包装
来源：http://skr.gaohongyu789.top

new Promise((resolve, reject) => {})
来源：http://ats.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://lal.ivvv.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kaf.xuetiantiany.cn

[U97] JS：并发请求
来源：http://mjm.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ewh.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://los.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://csg.redwolf501.top

[U99] JS：事件监听
来源：http://zle.vehdjk.com

el.addEventListener("click", e => {})
来源：http://xkb.yuxming.cn

[U100] JS：DOM 查询
来源：http://jfy.bbcook.cn

document.querySelector(".item")
来源：http://kps.cqqwz.cn

[U101] JS：classList 操作
来源：http://erp.yanxiufei.cn

el.classList.toggle("active")
来源：http://dlg.chenlongwang.top

[U102] JS：本地存储
来源：http://foj.birdmap.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nfe.yuanzhike.top

[U103] JS：定时器
来源：http://kgh.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bub.xuanzx.com

[U104] JS：防抖
来源：http://tnt.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpi.yj202588.top

[U105] JS：节流
来源：http://wuu.nwbrower.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wuc.feifeiyinyue.top

[U106] JS：日期格式化
来源：http://szp.bjfxy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qmv.pycfn.com

[U107] JS：数字千分位
来源：http://xbg.yvedp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ucp.xuanzx.com

[U108] JS：随机整数
来源：http://yes.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bml.sjlbkw.cn

[U109] JS：数组分组
来源：http://fyx.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://oby.nanxuanxn.top

[U110] JS：数组分块
来源：http://kkp.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://obv.hnqzz.top

[U111] JS：对象转 Map
来源：http://qos.ybcxt.top

new Map(Object.entries(obj))
来源：http://tyd.epnwcf.com

[U112] JS：字符串补位
来源：http://cpz.hammf.cn

"7".padStart(3, "0")
来源：http://fue.shuidangran.top

[U113] JS：正则替换全部
来源：http://cox.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://khr.ywan-chungtsiang.top

[U114] JS：JSON 深比较
来源：http://wjw.nanxuanxn.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hej.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://yxh.cashguo.top

crypto.randomUUID()
来源：http://prk.ywan-chungtsiang.top

[U116] JS：类型检查（JSDoc）
来源：http://ncy.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://dbc.bjfxy.top


<!-- 参考信息 -->