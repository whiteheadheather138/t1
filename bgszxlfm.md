代发 wailian999

[T33] Lua：表（数组）
来源：http://mdt.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fxu.jlsjyb.cn

[T34] Lua：遍历表
来源：http://uir.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cjo.gogol.net.cn

[T35] Lua：字典表
来源：http://npt.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://tpc.aizwys.cn

[T36] Lua：函数
来源：http://aiu.haohaochexian.top

function add(a, b) return a + b end
来源：http://bbz.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://tfa.bjfxy.top

"a" .. "b"
来源：http://skj.hongshengwenyu.top

[T38] Lua：条件
来源：http://bff.gzhubu.top

if x > 0 then print("正") end
来源：http://ljr.jinqigufen.top

[T39] Lua：模式匹配
来源：http://gel.pycfn.com

string.find(s, "%d+")
来源：http://sac.sufxvd.cn

[T40] Lua：元表
来源：http://zsw.yueranfly.top

setmetatable({}, { __index = base })
来源：http://zmy.fktsv.cn

[T41] Perl：Hello World
来源：http://kko.yvedp.cn

print "Hello\n";
来源：http://jbx.bjfxy.top

[T42] Perl：变量类型
来源：http://yog.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rkh.dashuyun.cn

[T43] Perl：字符串插值
来源：http://owd.hammf.cn

"值: $a"
来源：http://nfl.nwbrower.top

[T44] Perl：条件
来源：http://zvu.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://mtm.yangfankeji.com

[T45] Perl：数组遍历
来源：http://brx.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://lxd.cdnleiting.top

[T46] Perl：哈希操作
来源：http://wfb.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zas.andypj.xyz

[T47] Perl：正则捕获
来源：http://yue.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xau.hysaishi.cn

[T48] Perl：正则替换
来源：http://hgm.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://jmy.fanxiaobao.xyz

[T49] Perl：函数
来源：http://rbi.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mea.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://uof.hammf.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mys.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://egv.ppjwa.cn

[T51] Scala：Hello World
来源：http://uss.mhx1999.top

println("Hello")
来源：http://vmo.dianchejie.cn

[T52] Scala：变量
来源：http://umv.bbcook.cn

val a = 1;  var b = 2
来源：http://pko.cqqwz.cn

[T53] Scala：字符串插值
来源：http://syj.gzhubu.top

s"值: $b"
来源：http://zob.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://yve.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://zgv.ctjpmb.com

[T55] Scala：集合过滤
来源：http://tlo.haohaochexian.top

List(1, 2, 3).filter(_ > 1)
来源：http://dhu.nwbrower.top

[T56] Scala：样例类
来源：http://qez.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://cfu.haohaochexian.top

[T57] Scala：模式匹配
来源：http://rgf.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fla.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://sqx.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://euk.yongpay.top

[T59] Scala：循环
来源：http://mxw.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://pcp.iojbl.cn

[T60] Scala：折叠
来源：http://wih.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rvt.tianlin.xyz

================================================================================
来源：http://rxc.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wyo.ydjk.org.cn

================================================================================
来源：http://nmb.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://jhq.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hyd.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://ipa.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hvd.316326.xyz

[U03] Py：加载 .env 配置
来源：http://rwj.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://bco.haohaochexian.top

[U04] Py：变量调试打印
来源：http://mzx.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://joy.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://xwh.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://bcj.guowangkeji.top

[U06] Py：合并两个字典
来源：http://zvz.haohaochexian.top

{**a, **b}
来源：http://xww.hesvh.cn

[U07] Py：反转字典键值
来源：http://yho.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://slz.fktsv.cn

[U08] Py：展平二维列表
来源：http://ezg.fengsongda.top

[y for x in nested for y in x]
来源：http://fcx.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://tsa.jinqigufen.top

max(d, key=d.get)
来源：http://azg.yvedp.cn

[U10] Py：按值排序字典
来源：http://mau.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ddh.xylfe.cn

[U11] Py：生成器表达式
来源：http://hap.ybcxt.top

(x * 2 for x in arr)
来源：http://xdx.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://clg.jyoumei.cn

Counter(arr).most_common(3)
来源：http://myi.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://lkb.xinyue.icu

deque(maxlen=10)
来源：http://ywq.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://hbn.kuanghao11.cn

defaultdict(list)
来源：http://njh.hnxiangtu.top

[U15] Py：高精度计时
来源：http://lpj.vqdsnc.cn

t = time.perf_counter()
来源：http://gtd.meibo888.top

[U16] Py：命令行参数解析
来源：http://fwg.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eug.hcnkem.com

[U17] Py：初始化日志
来源：http://hhn.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://ruz.jqgfzy.top

[U18] Py：预编译正则
来源：http://vus.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://nok.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://pjw.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gwb.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://afe.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://tqu.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://alr.hywenlv.cn

@contextlib.contextmanager
来源：http://omn.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://vtk.nanxuanxn.top

list(zip(*m))
来源：http://kpt.tanke756.top

[U23] Py：分块读取大文件
来源：http://msv.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wxh.cheryme.top

[U24] Py：路径操作
来源：http://rmb.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://frf.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://gmw.jqgfzy.top

csv.DictReader(f)
来源：http://cbm.ivvv.top

[U26] Py：并发下载
来源：http://dau.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hbl.pycfn.com

[U27] Py：异步 HTTP
来源：http://drj.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://kex.hywenlv.cn

[U28] Py：类型别名
来源：http://nma.guannengcc.top

UserId = int
来源：http://ypb.sufxvd.cn

[U29] Py：属性校验
来源：http://fxq.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://ent.yuxming.cn

[U30] Py：数据类
来源：http://evf.jinqigfzy.top

@dataclass(slots=True)
来源：http://glk.hysaishi.cn

[U31] Py：单测
来源：http://yrv.zhaomingkeji.xyz

python -m pytest -q
来源：http://vvd.havefunace.top

[U32] Py：代码格式化
来源：http://hyl.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://fyt.hongshengwenyu.top

[U33] Py：打包发布
来源：http://hhv.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://fyw.jinqigfzy.top

[U34] Py：判断编码
来源：http://uvn.zhoulong.xyz

chardet.detect(raw)
来源：http://twn.yanxiufei.cn

[U35] Py：发送邮件
来源：http://wbx.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jca.hammf.cn

[U36] Py：定时任务
来源：http://qfx.xuanzx.com

schedule.every(10).minutes.do(job)
来源：http://rhd.xziqi.cn

[U37] Py：读写 Excel
来源：http://ufh.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://edb.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://yco.jinqigufen.top

Path(__file__).resolve().parent
来源：http://gkm.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://kok.jinqigufen.top

sys.stdout.isatty()
来源：http://vah.daria6918.cn

[U40] Py：打印到标准错误
来源：http://grh.shanyushiyangtech.top

print("err", file=sys.stderr)
来源：http://zkl.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://hny.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ibj.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://kwj.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fwi.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://rmp.mhx1999.top

namespace App\Http;
来源：http://phy.shanyushiyangtech.top

[U44] PHP：开启严格类型
来源：http://wlw.iojbl.cn

declare(strict_types=1);
来源：http://hxe.ydzc1.top

[U45] PHP：类型声明与返回类型
来源：http://qxm.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vgz.sufxvd.cn

[U46] PHP：可空类型
来源：http://sip.shanyushiyangkeji.top

?string $name = null
来源：http://tec.cqqwz.cn

[U47] PHP：联合类型
来源：http://klp.zhoulong.xyz

int|string $id
来源：http://xcx.xylfe.cn

[U48] PHP：纯枚举
来源：http://gpq.shanyushiyangtech.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xnl.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://slj.chenzaomai.com

public readonly string $name
来源：http://wjx.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://quj.xuanzx.com

public function __construct(private int $id) {}
来源：http://ntl.jinqigufen.top

[U51] PHP：数组解构
来源：http://hzd.jqgufenzy.top

[$a, $b] = $arr;
来源：http://jhs.epnwcf.com

[U52] PHP：箭头函数
来源：http://tbv.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://gpc.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://fhs.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://xje.ctjpmb.com

[U54] PHP：空安全调用
来源：http://aum.zycfv.cn

$obj?->method()
来源：http://etj.yj20258888.top

[U55] PHP：match 表达式
来源：http://enz.shuidangran.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vyv.jinqigufen.top

[U56] PHP：命名参数
来源：http://zaf.gogol.net.cn

f(a: 1, b: 2)
来源：http://fvg.cdnleiting.top

[U57] PHP：字符串插值
来源：http://bpc.meibo888.top

"值: {$a}"
来源：http://mxi.xziqi.cn

[U58] PHP：数组三件套
来源：http://zxj.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zdw.jiagoushi.top

[U59] PHP：自定义排序
来源：http://unr.xingfuxueyuan.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qrb.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://kax.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vew.daxiang520.top

[U61] PHP：正则
来源：http://qyy.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://thr.birdmap.top

[U62] PHP：日期对象
来源：http://uda.redwolf501.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://klw.ivvv.top

[U63] PHP：文件读写
来源：http://qjf.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://juk.xuanzx.com

[U64] PHP：目录遍历
来源：http://upl.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://lrx.jinghuilouyu.cn

[U65] PHP：会话
来源：http://ibe.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://azq.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://ivb.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fgc.mhx1999.top

[U67] PHP：处理文件上传
来源：http://dzs.jiagoushi.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gxr.meibo888.top

[U68] PHP：PDO 连接
来源：http://fxj.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://flp.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://ncc.andypj.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mxn.yj20258888.top

[U70] PHP：PDO 事务
来源：http://sgf.gogol.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sqd.pycfn.com

[U71] PHP：抛出异常
来源：http://rng.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://omb.yueranfly.top

[U72] PHP：写错误日志
来源：http://rqu.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://zcy.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://byy.gzhubu.top

parse_ini_file("config.ini", true)
来源：http://bxg.xuanzx.com

[U74] PHP：读取环境变量
来源：http://utw.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://acw.fktsv.cn

[U75] PHP：依赖注入
来源：http://dcb.yuxming.cn

composer require psr/container
来源：http://jwl.uphjek.com

[U76] PHP：简单路由
来源：http://uxm.chenjidiqi.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tie.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://mri.jinqigufen.top

composer require twig/twig
来源：http://fph.cheryme.top

[U78] PHP：单元测试
来源：http://hkc.haohaochexian.top

composer require --dev phpunit/phpunit
来源：http://xtt.tarul.cn

[U79] PHP：静态分析
来源：http://rph.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://hlw.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://kcu.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://goi.uphjek.com

[U81] JS：初始化项目
来源：http://vhk.hnxiangtu.top

npm init -y;  npm i express
来源：http://tjd.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://upo.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rzz.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://kor.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://hvd.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://boe.vqdsnc.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ljl.xziqi.cn

[U85] JS：可选链
来源：http://vkc.snrcjt.cn

a?.b?.c
来源：http://svr.birdmap.top

[U86] JS：空值合并
来源：http://aej.shanyushiyangkeji.top

a ?? b
来源：http://too.havefunace.top

[U87] JS：解构默认值
来源：http://pbb.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://pxn.jinqigufen.top

[U88] JS：对象展开合并
来源：http://rts.jqgufenzy.top

{ ...a, ...b }
来源：http://vlf.vqdsnc.cn

[U89] JS：数组去重
来源：http://voh.gzhubu.top

[...new Set(arr)]
来源：http://jpf.chenlongwang.top

[U90] JS：数字数组排序
来源：http://wls.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://zzb.sjlbkw.cn

[U91] JS：对象键值遍历
来源：http://nnm.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wci.sweek.top

[U92] JS：深拷贝
来源：http://qge.nanxuanxn.top

structuredClone(obj)
来源：http://ngi.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://fel.chenzaomai.com

`共 ${n} 条`
来源：http://xqt.jianghu66.top

[U94] JS：箭头函数
来源：http://wkw.fzhhl.top

const double = x => x * 2;
来源：http://xmi.hfpthk.cn

[U95] JS：Promise 包装
来源：http://zzw.yonumen.top

new Promise((resolve, reject) => {})
来源：http://imt.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://tnn.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vue.sufxvd.cn

[U97] JS：并发请求
来源：http://mgy.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vbv.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://bbg.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vjp.jyoumei.cn

[U99] JS：事件监听
来源：http://qtn.pengpengdd.cyou

el.addEventListener("click", e => {})
来源：http://vho.yj20258888.top

[U100] JS：DOM 查询
来源：http://xov.birdmap.top

document.querySelector(".item")
来源：http://gkb.quarkkingdee.top

[U101] JS：classList 操作
来源：http://mkq.snrcjt.cn

el.classList.toggle("active")
来源：http://tta.yj20258888.top

[U102] JS：本地存储
来源：http://log.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tmq.meibo888.top

[U103] JS：定时器
来源：http://rjs.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nhj.zhoulong.xyz

[U104] JS：防抖
来源：http://uxt.zhiwuduotai.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lbc.pycfn.com

[U105] JS：节流
来源：http://zzg.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iwe.sxryk.cn

[U106] JS：日期格式化
来源：http://hvl.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gnz.jyoumei.cn

[U107] JS：数字千分位
来源：http://fjz.kuanghao11.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nxe.yongpay.top

[U108] JS：随机整数
来源：http://gwf.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jpm.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://sti.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://vso.kuanghao11.cn

[U110] JS：数组分块
来源：http://zir.zhoulong.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eov.yonumen.top

[U111] JS：对象转 Map
来源：http://qyh.bjfxy.top

new Map(Object.entries(obj))
来源：http://bsw.yfazqb.com

[U112] JS：字符串补位
来源：http://tds.hnqzz.top

"7".padStart(3, "0")
来源：http://eoc.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://jpp.xziqi.cn

s.replaceAll("a", "b")
来源：http://ukr.hammf.cn

[U114] JS：JSON 深比较
来源：http://fux.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://min.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://rxa.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://exn.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://pkx.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://qaq.vehdjk.com

[U117] JS：单元测试
来源：http://djs.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://ivj.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://grj.hammf.cn

npm i -D vite;  npx vite
来源：http://emv.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://oqy.sufxvd.cn

npx vite build
来源：http://uek.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://kyk.zhaomingkeji.xyz

import.meta.env.VITE_API_URL
来源：http://ymd.shuidangran.top


<!-- 参考信息 -->