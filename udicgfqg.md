代发 wailian999

[T29] Swift：guard 提前返回
来源：http://upo.iojbl.cn

guard let x = opt else { return }
来源：http://tws.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://sfu.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://byb.vqdsnc.cn

[T31] Lua：Hello World
来源：http://fuv.daxiang520.top

print("Hello")
来源：http://kwv.tanke756.top

[T32] Lua：局部变量
来源：http://raq.snrcjt.cn

local a = 1
来源：http://mte.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://agx.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oiy.kuanghao11.cn

[T34] Lua：遍历表
来源：http://bxu.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://osi.zdqjudy.top

[T35] Lua：字典表
来源：http://oje.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://zum.fzhhl.top

[T36] Lua：函数
来源：http://rre.nwbrower.top

function add(a, b) return a + b end
来源：http://aot.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://wpu.xuanzx.com

"a" .. "b"
来源：http://gml.daria6918.cn

[T38] Lua：条件
来源：http://uno.guannengcc.top

if x > 0 then print("正") end
来源：http://igk.316326.xyz

[T39] Lua：模式匹配
来源：http://kox.bbcook.cn

string.find(s, "%d+")
来源：http://xbr.tanke756.top

[T40] Lua：元表
来源：http://awl.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://hor.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://xxn.tarul.cn

print "Hello\n";
来源：http://iom.vehdjk.com

[T42] Perl：变量类型
来源：http://rkr.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fge.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://akh.hywenlv.cn

"值: $a"
来源：http://boe.kuanghao11.cn

[T44] Perl：条件
来源：http://rop.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://duq.yuanzhike.top

[T45] Perl：数组遍历
来源：http://ixu.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://rtu.dianchejie.cn

[T46] Perl：哈希操作
来源：http://wyt.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xae.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://qtt.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://aqe.wangdashe.top

[T48] Perl：正则替换
来源：http://cbj.mhx1999.top

$s =~ s/old/new/g;
来源：http://neg.ppjwa.cn

[T49] Perl：函数
来源：http://sar.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lwu.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://gae.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jgc.gotoacloud.top

while (my $line = <$fh>) { print $line; }
来源：http://uti.daxiang520.top

[T51] Scala：Hello World
来源：http://cjv.snrcjt.cn

println("Hello")
来源：http://pnq.hnxiangtu.top

[T52] Scala：变量
来源：http://lkq.hesvh.cn

val a = 1;  var b = 2
来源：http://ubs.316326.xyz

[T53] Scala：字符串插值
来源：http://fgz.c1oappe.top

s"值: $b"
来源：http://gyx.yuanzhike.top

[T54] Scala：集合映射
来源：http://rsh.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://upk.zdqjudy.top

[T55] Scala：集合过滤
来源：http://hjv.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://mly.hywenlv.cn

[T56] Scala：样例类
来源：http://wlt.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://hdy.hysaishi.cn

[T57] Scala：模式匹配
来源：http://vga.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uyf.shuidangran.top

[T58] Scala：函数定义
来源：http://alu.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://zzn.tian-w.cn

[T59] Scala：循环
来源：http://mep.shanyushiyangkeji.top

for (i <- 1 to 10) println(i)
来源：http://pkj.snrcjt.cn

[T60] Scala：折叠
来源：http://qdk.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rwx.epnwcf.com

================================================================================
来源：http://frs.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qez.yvedp.cn

================================================================================
来源：http://nwg.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://qgz.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://yxn.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://fti.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ljh.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://too.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jci.tanke756.top

[U04] Py：变量调试打印
来源：http://nuw.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ybq.ybcxt.top

[U05] Py：列表去重且保序
来源：http://huc.cucudq.cn

list(dict.fromkeys(arr))
来源：http://cxb.hesvh.cn

[U06] Py：合并两个字典
来源：http://ffc.zhoulong.xyz

{**a, **b}
来源：http://ssh.zhengqikj.top

[U07] Py：反转字典键值
来源：http://ojj.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://ssd.52xcode.cn

[U08] Py：展平二维列表
来源：http://kzc.cheryme.top

[y for x in nested for y in x]
来源：http://mmf.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://otr.nanxuanxn.top

max(d, key=d.get)
来源：http://cpd.havefunace.top

[U10] Py：按值排序字典
来源：http://vsc.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pfk.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://bmd.jlsjyb.cn

(x * 2 for x in arr)
来源：http://rxs.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vhv.zdbjq.cn

Counter(arr).most_common(3)
来源：http://cli.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://stc.zhoulong.xyz

deque(maxlen=10)
来源：http://nff.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://lbh.shangyingyoupin.top

defaultdict(list)
来源：http://svp.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://hyd.ydzc1.top

t = time.perf_counter()
来源：http://rjq.yueranfly.top

[U16] Py：命令行参数解析
来源：http://njd.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kyn.hammf.cn

[U17] Py：初始化日志
来源：http://kqu.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://bty.daria6918.cn

[U18] Py：预编译正则
来源：http://ire.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://bhh.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://hew.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ujw.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://xqv.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://uky.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://edj.316326.xyz

@contextlib.contextmanager
来源：http://ida.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://xbv.gotoacloud.top

list(zip(*m))
来源：http://fhn.daxiang520.top

[U23] Py：分块读取大文件
来源：http://vnz.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uaz.aibaodan.cn

[U24] Py：路径操作
来源：http://wkm.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ftp.tanke756.top

[U25] Py：CSV 按字典读
来源：http://smi.yuanzhike.top

csv.DictReader(f)
来源：http://ngr.hcnkem.com

[U26] Py：并发下载
来源：http://cue.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pyw.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://oas.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://qbm.yongpay.top

[U28] Py：类型别名
来源：http://ltk.gaohongyu789.top

UserId = int
来源：http://wro.guannengcc.top

[U29] Py：属性校验
来源：http://caa.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://llb.hammf.cn

[U30] Py：数据类
来源：http://bjj.hongshengwenyu.top

@dataclass(slots=True)
来源：http://wqc.jlsjyb.cn

[U31] Py：单测
来源：http://xbt.snrcjt.cn

python -m pytest -q
来源：http://lwk.jqgufenzy.top

[U32] Py：代码格式化
来源：http://jbv.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://nct.guowangkeji.top

[U33] Py：打包发布
来源：http://hhc.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://vhg.fzhhl.top

[U34] Py：判断编码
来源：http://puf.316326.xyz

chardet.detect(raw)
来源：http://apj.zdbjq.cn

[U35] Py：发送邮件
来源：http://btc.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cgb.cucudq.cn

[U36] Py：定时任务
来源：http://yax.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://drt.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://iru.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://ybl.wangdashe.top

[U38] Py：获取脚本所在目录
来源：http://hps.aibaodan.cn

Path(__file__).resolve().parent
来源：http://zaw.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://inr.ydzc1.top

sys.stdout.isatty()
来源：http://ubi.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://yum.birdmap.top

print("err", file=sys.stderr)
来源：http://yrr.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://qkt.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://adc.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://sya.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ykl.mhx1999.top

[U43] PHP：声明命名空间
来源：http://ujo.hcnkem.com

namespace App\Http;
来源：http://htq.sweek.top

[U44] PHP：开启严格类型
来源：http://mev.cucudq.cn

declare(strict_types=1);
来源：http://vgr.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://wru.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ouh.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://ied.svipenyu.cn

?string $name = null
来源：http://sti.zdqjudy.top

[U47] PHP：联合类型
来源：http://kml.jinqigufen.top

int|string $id
来源：http://dhl.fengsongda.top

[U48] PHP：纯枚举
来源：http://fqp.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tyx.wangdashe.top

[U49] PHP：只读属性
来源：http://zgx.jiagoushi.top

public readonly string $name
来源：http://ofj.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://djt.svipenyu.cn

public function __construct(private int $id) {}
来源：http://hsl.ybcxt.top

[U51] PHP：数组解构
来源：http://sii.jyoumei.cn

[$a, $b] = $arr;
来源：http://akj.nwbrower.top

[U52] PHP：箭头函数
来源：http://esh.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://jyt.nwbrower.top

[U53] PHP：空合并运算符
来源：http://hdt.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://lat.nanxinkj.top

[U54] PHP：空安全调用
来源：http://dpx.c1oappe.top

$obj?->method()
来源：http://oyz.feifeiyinyue.top

[U55] PHP：match 表达式
来源：http://aho.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://aik.guannengcc.top

[U56] PHP：命名参数
来源：http://stm.yfazqb.com

f(a: 1, b: 2)
来源：http://mdm.yueranfly.top

[U57] PHP：字符串插值
来源：http://xgn.xuanzx.com

"值: {$a}"
来源：http://pdf.mhx1999.top

[U58] PHP：数组三件套
来源：http://wws.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xsk.ppjwa.cn

[U59] PHP：自定义排序
来源：http://qin.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujb.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://wjp.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://veo.xuetiantiany.cn

[U61] PHP：正则
来源：http://iia.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vru.yvedp.cn

[U62] PHP：日期对象
来源：http://mqr.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nlk.svipenyu.cn

[U63] PHP：文件读写
来源：http://wne.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vua.redwolf501.top

[U64] PHP：目录遍历
来源：http://gzi.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://kft.ppjwa.cn

[U65] PHP：会话
来源：http://sqz.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xgs.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://yvd.dianchejie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iyy.guowangkeji.top

[U67] PHP：处理文件上传
来源：http://ikt.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ucj.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://doi.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kon.zhoulong.xyz

[U69] PHP：PDO 预处理
来源：http://lzx.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hos.aizwys.cn

[U70] PHP：PDO 事务
来源：http://bsu.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://csl.xziqi.cn

[U71] PHP：抛出异常
来源：http://rla.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://pam.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://nkf.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://aqa.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://pty.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://yjh.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://ikb.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://hts.guowangkeji.top

[U75] PHP：依赖注入
来源：http://lyl.zdqjudy.top

composer require psr/container
来源：http://nlf.tianlin.xyz

[U76] PHP：简单路由
来源：http://cgy.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cjh.yj20258.top

[U77] PHP：模板渲染
来源：http://vja.cdnleiting.top

composer require twig/twig
来源：http://imk.sufxvd.cn

[U78] PHP：单元测试
来源：http://vwk.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://qze.zhongyouzk.top

[U79] PHP：静态分析
来源：http://uiw.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://erq.cashguo.top

[U80] PHP：代码规范修复
来源：http://ugl.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tyx.epnwcf.com

[U81] JS：初始化项目
来源：http://nan.hnqzz.top

npm init -y;  npm i express
来源：http://mjp.tarul.cn

[U82] JS：package.json 脚本
来源：http://qlj.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zpp.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://czy.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nwy.yj20258.top

[U84] JS：CommonJS 写法
来源：http://chh.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://zfo.havefunace.top

[U85] JS：可选链
来源：http://wqb.hfpthk.cn

a?.b?.c
来源：http://xrj.ehwqpu.com

[U86] JS：空值合并
来源：http://myt.zhiwuduotai.top

a ?? b
来源：http://eig.ppjwa.cn

[U87] JS：解构默认值
来源：http://bah.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://bzs.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://dqa.guannengcc.top

{ ...a, ...b }
来源：http://lki.feifeiyinyue.top

[U89] JS：数组去重
来源：http://eit.gogol.net.cn

[...new Set(arr)]
来源：http://rio.sweek.top

[U90] JS：数字数组排序
来源：http://hky.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://gln.tian-w.cn

[U91] JS：对象键值遍历
来源：http://dnv.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vpq.smart0.xyz

[U92] JS：深拷贝
来源：http://xvs.ywan-chungtsiang.top

structuredClone(obj)
来源：http://pbg.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://qmt.tanke756.top

`共 ${n} 条`
来源：http://yxh.jinqigufen.top

[U94] JS：箭头函数
来源：http://wti.tarul.cn

const double = x => x * 2;
来源：http://ewe.zhengqikj.top

[U95] JS：Promise 包装
来源：http://ezn.hongshengwenyu.top

new Promise((resolve, reject) => {})
来源：http://uzv.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://wod.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://juw.sjlbkw.cn

[U97] JS：并发请求
来源：http://bln.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://cgb.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://cbh.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://onp.tarul.cn

[U99] JS：事件监听
来源：http://lka.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://vlk.bbcook.cn

[U100] JS：DOM 查询
来源：http://xnd.shanyushiyangkeji.top

document.querySelector(".item")
来源：http://jaf.yvedp.cn

[U101] JS：classList 操作
来源：http://sue.tianlin.xyz

el.classList.toggle("active")
来源：http://gnk.xuetiantiany.cn

[U102] JS：本地存储
来源：http://vht.haohaochexian.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iyp.uphjek.com

[U103] JS：定时器
来源：http://jds.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://icn.fanxiaobao.xyz

[U104] JS：防抖
来源：http://yij.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipl.zhiwuduotai.top

[U105] JS：节流
来源：http://dqj.zhijiandao.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://itn.cqqwz.cn

[U106] JS：日期格式化
来源：http://ngx.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zbb.xinyue.icu

[U107] JS：数字千分位
来源：http://ypm.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aiv.0kj1m.cn

[U108] JS：随机整数
来源：http://jin.jiagoushi.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://spv.shzxlz.cn

[U109] JS：数组分组
来源：http://xtk.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://wys.yangfankeji.com

[U110] JS：数组分块
来源：http://ugx.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bqz.bbcook.cn

[U111] JS：对象转 Map
来源：http://slg.zycfv.cn

new Map(Object.entries(obj))
来源：http://syn.jlsjyb.cn

[U112] JS：字符串补位
来源：http://twm.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://ouh.gotoacloud.top

[U113] JS：正则替换全部
来源：http://idm.tarul.cn

s.replaceAll("a", "b")
来源：http://iob.jianghu66.top

[U114] JS：JSON 深比较
来源：http://szh.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ihx.xuanzx.com

[U115] JS：生成 UUID
来源：http://nkb.redwolf501.top

crypto.randomUUID()
来源：http://gir.daxiang520.top

[U116] JS：类型检查（JSDoc）
来源：http://dhv.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://ina.xuetiantiany.cn


<!-- 参考信息 -->