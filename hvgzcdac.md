代发 wailian999

[T31] Lua：Hello World
来源：http://xkq.xuanzx.com

print("Hello")
来源：http://wqa.uphjek.com

[T32] Lua：局部变量
来源：http://gcj.fehbvm.com

local a = 1
来源：http://sdi.sxryk.cn

[T33] Lua：表（数组）
来源：http://ykp.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lxr.shzxlz.cn

[T34] Lua：遍历表
来源：http://krb.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cym.sysykeji.top

[T35] Lua：字典表
来源：http://axr.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://vuk.hnxiangtu.top

[T36] Lua：函数
来源：http://msy.chenzaomai.com

function add(a, b) return a + b end
来源：http://dia.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://gvn.yj202588.top

"a" .. "b"
来源：http://dmx.chenjidiqi.icu

[T38] Lua：条件
来源：http://aid.nanxuanxn.top

if x > 0 then print("正") end
来源：http://vlh.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://dvo.zycfv.cn

string.find(s, "%d+")
来源：http://lmj.zdqjudy.top

[T40] Lua：元表
来源：http://vkm.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://kex.zycfv.cn

[T41] Perl：Hello World
来源：http://gcf.bjfxy.top

print "Hello\n";
来源：http://kgc.cashguo.top

[T42] Perl：变量类型
来源：http://sop.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qdn.yvedp.cn

[T43] Perl：字符串插值
来源：http://kok.aibaodan.cn

"值: $a"
来源：http://swk.zhoulong.xyz

[T44] Perl：条件
来源：http://mly.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://nei.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://iry.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://ida.smart0.xyz

[T46] Perl：哈希操作
来源：http://jlz.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gar.cdnleiting.top

[T47] Perl：正则捕获
来源：http://gpl.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ulk.guowangkeji.top

[T48] Perl：正则替换
来源：http://uxq.yj202588.top

$s =~ s/old/new/g;
来源：http://yyb.xuanzx.com

[T49] Perl：函数
来源：http://kig.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://txa.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://owg.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://igu.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://dag.ppjwa.cn

[T51] Scala：Hello World
来源：http://tat.snrcjt.cn

println("Hello")
来源：http://ezh.dashuyun.cn

[T52] Scala：变量
来源：http://dvb.tian-w.cn

val a = 1;  var b = 2
来源：http://fnc.chenlongwang.top

[T53] Scala：字符串插值
来源：http://noa.svipenyu.cn

s"值: $b"
来源：http://rue.wangdashe.top

[T54] Scala：集合映射
来源：http://ytj.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://jnv.ctjpmb.com

[T55] Scala：集合过滤
来源：http://qix.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://zts.xuetiantiany.cn

[T56] Scala：样例类
来源：http://tun.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://dbd.smart0.xyz

[T57] Scala：模式匹配
来源：http://vzw.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://emu.yj20258.top

[T58] Scala：函数定义
来源：http://kkd.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hap.316326.xyz

[T59] Scala：循环
来源：http://mcg.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://fzn.zhiwuduotai.top

[T60] Scala：折叠
来源：http://ecs.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lwi.c1oappe.top

================================================================================
来源：http://srn.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://msw.smart0.xyz

================================================================================
来源：http://pdj.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://vkd.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://kcj.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://rmp.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yhe.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://iaq.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dnt.zdbjq.cn

[U04] Py：变量调试打印
来源：http://rrp.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wob.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://pci.cucudq.cn

list(dict.fromkeys(arr))
来源：http://fbz.haohaochexian.top

[U06] Py：合并两个字典
来源：http://fqb.gaohongyu789.top

{**a, **b}
来源：http://wso.bjfxy.top

[U07] Py：反转字典键值
来源：http://qet.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://exz.hfpthk.cn

[U08] Py：展平二维列表
来源：http://zxh.daria6918.cn

[y for x in nested for y in x]
来源：http://xrq.52xcode.cn

[U09] Py：字典取最大值的键
来源：http://rxn.chenjidiqi.icu

max(d, key=d.get)
来源：http://pdj.ivvv.top

[U10] Py：按值排序字典
来源：http://lym.redwolf501.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://biz.fengsongda.top

[U11] Py：生成器表达式
来源：http://ekl.zhoulong.xyz

(x * 2 for x in arr)
来源：http://unc.sweek.top

[U12] Py：取出现最多的 3 个元素
来源：http://dwr.cqqwz.cn

Counter(arr).most_common(3)
来源：http://toh.xinyue.icu

[U13] Py：固定长度队列
来源：http://fra.fengsongda.top

deque(maxlen=10)
来源：http://ybu.yj20258.top

[U14] Py：分组收集到列表
来源：http://plp.haohaochexian.top

defaultdict(list)
来源：http://qhc.jlsjyb.cn

[U15] Py：高精度计时
来源：http://evy.ybcxt.top

t = time.perf_counter()
来源：http://xri.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://xvt.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://you.dashuyun.cn

[U17] Py：初始化日志
来源：http://uvm.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://nrl.jqgfzy.top

[U18] Py：预编译正则
来源：http://uzu.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://ojx.daxiang520.top

[U19] Py：正则替换带回调
来源：http://gmp.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pau.yuxming.cn

[U20] Py：缓存函数结果
来源：http://vla.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://del.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://qut.nanxinkj.top

@contextlib.contextmanager
来源：http://xkw.nanxinkj.top

[U22] Py：矩阵转置
来源：http://kui.nanxinkj.top

list(zip(*m))
来源：http://ios.yj20258888.top

[U23] Py：分块读取大文件
来源：http://omd.hysaishi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zgg.birdmap.top

[U24] Py：路径操作
来源：http://hky.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://inl.meibo888.top

[U25] Py：CSV 按字典读
来源：http://jok.ppjwa.cn

csv.DictReader(f)
来源：http://ucm.zdqjudy.top

[U26] Py：并发下载
来源：http://hhd.zhongyouzk.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wki.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://mpk.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://dwf.jinqigufen.top

[U28] Py：类型别名
来源：http://jfa.hywenlv.cn

UserId = int
来源：http://anp.shangyingyoupin.top

[U29] Py：属性校验
来源：http://bkn.tian-w.cn

@property 与 @x.setter 配合
来源：http://meh.yj20258.top

[U30] Py：数据类
来源：http://hac.nanxinkj.top

@dataclass(slots=True)
来源：http://osb.ydzc1.top

[U31] Py：单测
来源：http://utp.hongshengwenyu.top

python -m pytest -q
来源：http://rvb.guowangkeji.top

[U32] Py：代码格式化
来源：http://jxh.daxiang520.top

ruff format . && ruff check --fix .
来源：http://rcx.zhijiandao.cn

[U33] Py：打包发布
来源：http://hhs.yvedp.cn

python -m build  （依赖 pyproject.toml）
来源：http://yjl.feifeiyinyue.top

[U34] Py：判断编码
来源：http://wmh.c1oappe.top

chardet.detect(raw)
来源：http://ljv.svipenyu.cn

[U35] Py：发送邮件
来源：http://yxd.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ywj.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://kpd.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://qqq.haohaochexian.top

[U37] Py：读写 Excel
来源：http://cjs.cashguo.top

pandas.read_excel / DataFrame.to_excel
来源：http://xlt.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://fno.sufxvd.cn

Path(__file__).resolve().parent
来源：http://imr.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://dmr.fengsongda.top

sys.stdout.isatty()
来源：http://hzn.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://byo.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://lix.tarul.cn

[U41] PHP：初始化 Composer 项目
来源：http://slt.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zug.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://udi.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mmi.bjfxy.top

[U43] PHP：声明命名空间
来源：http://mfr.yj202588.top

namespace App\Http;
来源：http://ofl.havefunace.top

[U44] PHP：开启严格类型
来源：http://qsy.fzhhl.top

declare(strict_types=1);
来源：http://hdh.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://gkc.xuanzx.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://aad.yj202588.top

[U46] PHP：可空类型
来源：http://nwn.pengpengdd.cyou

?string $name = null
来源：http://yyf.yj202588.top

[U47] PHP：联合类型
来源：http://zib.cashguo.top

int|string $id
来源：http://qcp.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://yfc.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://spu.xingfuxueyuan.xyz

[U49] PHP：只读属性
来源：http://oap.jqgfzy.top

public readonly string $name
来源：http://fzg.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://pnk.xingfuxueyuan.xyz

public function __construct(private int $id) {}
来源：http://ahh.yanxiufei.cn

[U51] PHP：数组解构
来源：http://yqh.mhx1999.top

[$a, $b] = $arr;
来源：http://wsl.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://yim.zhongyouzk.top

$double = fn($x) => $x * 2;
来源：http://zfk.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://pza.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://azi.hysaishi.cn

[U54] PHP：空安全调用
来源：http://zzi.cdnleiting.top

$obj?->method()
来源：http://gvq.zycfv.cn

[U55] PHP：match 表达式
来源：http://rtg.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hfa.sysykeji.top

[U56] PHP：命名参数
来源：http://bra.gotoacloud.top

f(a: 1, b: 2)
来源：http://wrg.aibaodan.cn

[U57] PHP：字符串插值
来源：http://kwh.sjlbkw.cn

"值: {$a}"
来源：http://oyl.dashuyun.cn

[U58] PHP：数组三件套
来源：http://ujx.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://usu.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://yzn.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hkh.tarul.cn

[U60] PHP：JSON 编解码
来源：http://tgt.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jyw.dashuyun.cn

[U61] PHP：正则
来源：http://auy.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wzr.yonumen.top

[U62] PHP：日期对象
来源：http://lrx.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hdo.ctjpmb.com

[U63] PHP：文件读写
来源：http://toq.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tce.redwolf501.top

[U64] PHP：目录遍历
来源：http://onl.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://lqz.hammf.cn

[U65] PHP：会话
来源：http://nnp.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fsf.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://mxg.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qxi.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://iin.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qfm.ywan-chungtsiang.top

[U68] PHP：PDO 连接
来源：http://yam.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rpg.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://mfs.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yzu.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://ktk.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wzf.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://jlg.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://fqp.ywan-chungtsiang.top

[U72] PHP：写错误日志
来源：http://jmo.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://sst.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://qbi.xingfuxueyuan.xyz

parse_ini_file("config.ini", true)
来源：http://lmq.yvedp.cn

[U74] PHP：读取环境变量
来源：http://tcy.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://ips.yuxming.cn

[U75] PHP：依赖注入
来源：http://urn.gotoacloud.top

composer require psr/container
来源：http://mvq.meibo888.top

[U76] PHP：简单路由
来源：http://zup.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ylr.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://yxz.zhongyouzk.top

composer require twig/twig
来源：http://mlb.yvedp.cn

[U78] PHP：单元测试
来源：http://gyx.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://avd.jqgufenzy.top

[U79] PHP：静态分析
来源：http://mxr.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://kol.meibo888.top

[U80] PHP：代码规范修复
来源：http://nxx.dashuyun.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xlx.wangshuangyany.cn

[U81] JS：初始化项目
来源：http://efx.zhijiandao.cn

npm init -y;  npm i express
来源：http://llx.c1oappe.top

[U82] JS：package.json 脚本
来源：http://blm.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gks.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://wrs.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://boq.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://gdj.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ylj.xinyue.icu

[U85] JS：可选链
来源：http://ckc.yanxiufei.cn

a?.b?.c
来源：http://laa.fktsv.cn

[U86] JS：空值合并
来源：http://wqt.nanxinkj.top

a ?? b
来源：http://avi.9152youxi.cn

[U87] JS：解构默认值
来源：http://jln.ydjk.org.cn

const { a = 1, b = 2 } = obj;
来源：http://zps.fanxiaobao.xyz

[U88] JS：对象展开合并
来源：http://fcw.smart0.xyz

{ ...a, ...b }
来源：http://bto.cucudq.cn

[U89] JS：数组去重
来源：http://xzl.birdmap.top

[...new Set(arr)]
来源：http://sov.yonumen.top

[U90] JS：数字数组排序
来源：http://qwj.yfazqb.com

[...arr].sort((a, b) => a - b)
来源：http://chd.snrcjt.cn

[U91] JS：对象键值遍历
来源：http://suo.vqdsnc.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dpr.iojbl.cn

[U92] JS：深拷贝
来源：http://mqb.zhijiandao.cn

structuredClone(obj)
来源：http://jxo.hnxiangtu.top

[U93] JS：模板字符串
来源：http://vqt.gogol.net.cn

`共 ${n} 条`
来源：http://lfh.snrcjt.cn

[U94] JS：箭头函数
来源：http://hxc.nanxinkj.top

const double = x => x * 2;
来源：http://gpo.shuidangran.top

[U95] JS：Promise 包装
来源：http://rjm.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://ndw.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://osg.havefunace.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hkb.zycfv.cn

[U97] JS：并发请求
来源：http://aaa.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eoy.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://dbm.shangyingyoupin.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ddi.dashuyun.cn

[U99] JS：事件监听
来源：http://qgq.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://gdb.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://dxl.yj20258888.top

document.querySelector(".item")
来源：http://qwv.yuxming.cn

[U101] JS：classList 操作
来源：http://uwr.nanxinkj.top

el.classList.toggle("active")
来源：http://mhe.sjlbkw.cn

[U102] JS：本地存储
来源：http://dxx.jqgufenzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jrk.vehdjk.com

[U103] JS：定时器
来源：http://zac.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://une.zhiwuduotai.top

[U104] JS：防抖
来源：http://rud.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpt.sysykeji.top

[U105] JS：节流
来源：http://gzq.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtz.shuidangran.top

[U106] JS：日期格式化
来源：http://koy.xinyue.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ryj.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://iew.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://don.fktsv.cn

[U108] JS：随机整数
来源：http://vnb.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dyb.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://qrp.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://oxt.cqqwz.cn

[U110] JS：数组分块
来源：http://uxg.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhe.yuxming.cn

[U111] JS：对象转 Map
来源：http://ige.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://ewh.fktsv.cn

[U112] JS：字符串补位
来源：http://dtd.sjlbkw.cn

"7".padStart(3, "0")
来源：http://mhs.yuanzhike.top

[U113] JS：正则替换全部
来源：http://jmj.hammf.cn

s.replaceAll("a", "b")
来源：http://ffk.smart0.xyz

[U114] JS：JSON 深比较
来源：http://pal.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://cer.hywenlv.cn

[U115] JS：生成 UUID
来源：http://uqz.wangshuangyany.cn

crypto.randomUUID()
来源：http://ncd.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://mav.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://jia.fehbvm.com

[U117] JS：单元测试
来源：http://khv.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://uaf.zhongyouzk.top

[U118] JS：开发服务器
来源：http://kpx.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://ibh.zhoulong.xyz


<!-- 参考信息 -->