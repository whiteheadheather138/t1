代发 wailian999

[T35] Lua：字典表
来源：http://tkh.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://ntw.hcnkem.com

[T36] Lua：函数
来源：http://viw.jiagoushi.top

function add(a, b) return a + b end
来源：http://ikq.birdmap.top

[T37] Lua：字符串拼接
来源：http://lbv.ivvv.top

"a" .. "b"
来源：http://dst.yvedp.cn

[T38] Lua：条件
来源：http://nag.birdmap.top

if x > 0 then print("正") end
来源：http://egj.hcnkem.com

[T39] Lua：模式匹配
来源：http://bys.9152youxi.cn

string.find(s, "%d+")
来源：http://fzy.jinghuilouyu.cn

[T40] Lua：元表
来源：http://wie.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://hkc.gzhubu.top

[T41] Perl：Hello World
来源：http://pmk.zhengqikj.top

print "Hello\n";
来源：http://xbt.c1oappe.top

[T42] Perl：变量类型
来源：http://vlr.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ipj.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://zyo.mhx1999.top

"值: $a"
来源：http://ybe.gotoacloud.top

[T44] Perl：条件
来源：http://vuk.ppjwa.cn

if ($a > 0) { print "正"; }
来源：http://xks.9152youxi.cn

[T45] Perl：数组遍历
来源：http://gpd.ivvv.top

for my $x (@arr) { print $x; }
来源：http://vnr.tianlin.xyz

[T46] Perl：哈希操作
来源：http://xfz.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gul.sxryk.cn

[T47] Perl：正则捕获
来源：http://voh.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://npf.gaohongyu789.top

[T48] Perl：正则替换
来源：http://tyq.guannengcc.top

$s =~ s/old/new/g;
来源：http://rvf.hcnkem.com

[T49] Perl：函数
来源：http://ehr.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://clg.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://dax.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://cta.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://ztr.ybcxt.top

[T51] Scala：Hello World
来源：http://efl.aizwys.cn

println("Hello")
来源：http://vfj.wangshuangyany.cn

[T52] Scala：变量
来源：http://qpk.daria6918.cn

val a = 1;  var b = 2
来源：http://hdo.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://hgk.xuanzx.com

s"值: $b"
来源：http://dja.zhixingplan.top

[T54] Scala：集合映射
来源：http://tny.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://nuj.fengsongda.top

[T55] Scala：集合过滤
来源：http://ftb.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://jpo.hnqzz.top

[T56] Scala：样例类
来源：http://ehm.xziqi.cn

case class User(name: String, age: Int)
来源：http://pnc.tarul.cn

[T57] Scala：模式匹配
来源：http://qbz.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dxb.zhengqikj.top

[T58] Scala：函数定义
来源：http://flp.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://drb.xuanzx.com

[T59] Scala：循环
来源：http://fsk.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://jpb.kuanghao11.cn

[T60] Scala：折叠
来源：http://ksy.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ywi.yj20258.top

================================================================================
来源：http://pes.wangdashe.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wrl.yj202588.top

================================================================================
来源：http://xgq.havefunace.top

[U01] Py：创建虚拟环境
来源：http://aoq.fzhhl.top

python -m venv .venv && source .venv/bin/activate
来源：http://dos.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://qiu.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zre.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://dvt.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lpa.gzhubu.top

[U04] Py：变量调试打印
来源：http://esm.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dgf.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://wky.uphjek.com

list(dict.fromkeys(arr))
来源：http://fng.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://gte.hnqzz.top

{**a, **b}
来源：http://hve.ctjpmb.com

[U07] Py：反转字典键值
来源：http://sbx.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://isy.yj202588.top

[U08] Py：展平二维列表
来源：http://eud.yonumen.top

[y for x in nested for y in x]
来源：http://iiu.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://hfg.fzhhl.top

max(d, key=d.get)
来源：http://tdk.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://kpr.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vux.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://uxi.jqgfzy.top

(x * 2 for x in arr)
来源：http://esn.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vjf.tian-w.cn

Counter(arr).most_common(3)
来源：http://qfi.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://aks.jlsjyb.cn

deque(maxlen=10)
来源：http://ubk.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://hfz.bjfxy.top

defaultdict(list)
来源：http://cut.shuidangran.top

[U15] Py：高精度计时
来源：http://eps.wangshuangyany.cn

t = time.perf_counter()
来源：http://cev.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://oni.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yym.fengsongda.top

[U17] Py：初始化日志
来源：http://cgt.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://ypj.hnqzz.top

[U18] Py：预编译正则
来源：http://muc.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://nac.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://jxm.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mnp.sxryk.cn

[U20] Py：缓存函数结果
来源：http://cfk.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://uqa.vqdsnc.cn

[U21] Py：自定义上下文管理器
来源：http://plj.ppjwa.cn

@contextlib.contextmanager
来源：http://vnm.cheryme.top

[U22] Py：矩阵转置
来源：http://wti.sxryk.cn

list(zip(*m))
来源：http://hvx.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://wjd.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vzt.shangyingyoupin.top

[U24] Py：路径操作
来源：http://rjn.yj202588.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cux.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://xrv.wangdashe.top

csv.DictReader(f)
来源：http://yaw.cheryme.top

[U26] Py：并发下载
来源：http://bhf.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bab.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://mjo.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://pnn.jinqigufen.top

[U28] Py：类型别名
来源：http://kdl.hnqzz.top

UserId = int
来源：http://uop.smart0.xyz

[U29] Py：属性校验
来源：http://xvd.cqqwz.cn

@property 与 @x.setter 配合
来源：http://sqo.epnwcf.com

[U30] Py：数据类
来源：http://fys.nanxinkj.top

@dataclass(slots=True)
来源：http://vup.zycfv.cn

[U31] Py：单测
来源：http://ihz.jinyuanbaomall.cn

python -m pytest -q
来源：http://css.daxiang520.top

[U32] Py：代码格式化
来源：http://uxu.yonumen.top

ruff format . && ruff check --fix .
来源：http://izz.cqqwz.cn

[U33] Py：打包发布
来源：http://qdd.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://lln.hongshengwenyu.top

[U34] Py：判断编码
来源：http://voh.jinghuilouyu.cn

chardet.detect(raw)
来源：http://xbz.chenzaomai.com

[U35] Py：发送邮件
来源：http://pgj.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hro.gzhubu.top

[U36] Py：定时任务
来源：http://czu.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://ufo.zhengqikj.top

[U37] Py：读写 Excel
来源：http://niq.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://ayu.daxiang520.top

[U38] Py：获取脚本所在目录
来源：http://kyd.dashuyun.cn

Path(__file__).resolve().parent
来源：http://red.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://obk.smart0.xyz

sys.stdout.isatty()
来源：http://ohb.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://lda.hysaishi.cn

print("err", file=sys.stderr)
来源：http://rkj.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ozw.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uel.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://dtt.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xpg.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://qzz.sysykeji.top

namespace App\Http;
来源：http://ooj.bjfxy.top

[U44] PHP：开启严格类型
来源：http://ymj.guannengcc.top

declare(strict_types=1);
来源：http://orv.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://ptn.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://klv.shzxlz.cn

[U46] PHP：可空类型
来源：http://fen.xziqi.cn

?string $name = null
来源：http://lzy.aibaodan.cn

[U47] PHP：联合类型
来源：http://oxz.0kj1m.cn

int|string $id
来源：http://lkz.ybcxt.top

[U48] PHP：纯枚举
来源：http://zvf.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nte.nanxinkj.top

[U49] PHP：只读属性
来源：http://dlf.yuxming.cn

public readonly string $name
来源：http://kng.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://vgw.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://qmp.chenzaomai.com

[U51] PHP：数组解构
来源：http://dsu.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://znh.haohaochexian.top

[U52] PHP：箭头函数
来源：http://bfn.iojbl.cn

$double = fn($x) => $x * 2;
来源：http://tmf.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://tnb.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://jgm.hcnkem.com

[U54] PHP：空安全调用
来源：http://yyl.birdmap.top

$obj?->method()
来源：http://bjm.jqgfzy.top

[U55] PHP：match 表达式
来源：http://bhb.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://arw.nanxinkj.top

[U56] PHP：命名参数
来源：http://yup.yongpay.top

f(a: 1, b: 2)
来源：http://hrb.wangdashe.top

[U57] PHP：字符串插值
来源：http://tcn.guannengcc.top

"值: {$a}"
来源：http://bjb.hfpthk.cn

[U58] PHP：数组三件套
来源：http://yli.aizwys.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ymo.ctjpmb.com

[U59] PHP：自定义排序
来源：http://ono.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrx.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://leu.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tvn.hywenlv.cn

[U61] PHP：正则
来源：http://qmv.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vce.ehwqpu.com

[U62] PHP：日期对象
来源：http://pxb.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pvl.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://aho.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sxm.cdnleiting.top

[U64] PHP：目录遍历
来源：http://kex.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://air.meibo888.top

[U65] PHP：会话
来源：http://acy.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lnd.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://ijz.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://shb.aizwys.cn

[U67] PHP：处理文件上传
来源：http://ddd.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sno.daria6918.cn

[U68] PHP：PDO 连接
来源：http://kwy.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://efk.nanxinkj.top

[U69] PHP：PDO 预处理
来源：http://bao.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nax.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://bbc.xinyue.icu

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bnn.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://vld.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://psp.52xcode.cn

[U72] PHP：写错误日志
来源：http://ict.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://hdv.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://jdt.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://frz.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://tem.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://kqy.zdqjudy.top

[U75] PHP：依赖注入
来源：http://eme.xylfe.cn

composer require psr/container
来源：http://udn.meibo888.top

[U76] PHP：简单路由
来源：http://aic.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://okj.bjfxy.top

[U77] PHP：模板渲染
来源：http://qat.fktsv.cn

composer require twig/twig
来源：http://kfz.yuxming.cn

[U78] PHP：单元测试
来源：http://toc.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://zdy.fktsv.cn

[U79] PHP：静态分析
来源：http://eqz.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://xny.yueranfly.top

[U80] PHP：代码规范修复
来源：http://oap.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tws.zhoulong.xyz

[U81] JS：初始化项目
来源：http://ewh.nanxinkj.top

npm init -y;  npm i express
来源：http://gfl.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://ywh.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wig.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://pls.sweek.top

export const a = 1;  import { a } from "./m.js";
来源：http://xkg.ivvv.top

[U84] JS：CommonJS 写法
来源：http://ehw.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://uig.jinghuilouyu.cn

[U85] JS：可选链
来源：http://iyx.aizwys.cn

a?.b?.c
来源：http://jbm.jqgfzy.top

[U86] JS：空值合并
来源：http://grm.jianghu66.top

a ?? b
来源：http://sex.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://blp.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://xko.zhixingplan.top

[U88] JS：对象展开合并
来源：http://qej.daria6918.cn

{ ...a, ...b }
来源：http://nnq.zhongyouzk.top

[U89] JS：数组去重
来源：http://chx.shuidangran.top

[...new Set(arr)]
来源：http://hwg.feifeiyinyue.top

[U90] JS：数字数组排序
来源：http://xvs.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://ldc.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://vmj.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://spd.tarul.cn

[U92] JS：深拷贝
来源：http://jex.yonumen.top

structuredClone(obj)
来源：http://mjs.jqgufenzy.top

[U93] JS：模板字符串
来源：http://lld.shzxlz.cn

`共 ${n} 条`
来源：http://adx.zhixingplan.top

[U94] JS：箭头函数
来源：http://tbe.shzxlz.cn

const double = x => x * 2;
来源：http://vyx.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://ksk.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://irf.daxiang520.top

[U96] JS：async/await 与异常
来源：http://iov.wangdashe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hax.yj20258888.top

[U97] JS：并发请求
来源：http://inc.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lty.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://jfc.svipenyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cbz.quarkkingdee.top

[U99] JS：事件监听
来源：http://hna.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://xzq.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://ooq.wangdashe.top

document.querySelector(".item")
来源：http://gqd.bbcook.cn

[U101] JS：classList 操作
来源：http://qwm.shuidangran.top

el.classList.toggle("active")
来源：http://dhl.ctjpmb.com

[U102] JS：本地存储
来源：http://lic.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lrx.fktsv.cn

[U103] JS：定时器
来源：http://adv.wangshuangyany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aua.fktsv.cn

[U104] JS：防抖
来源：http://hmf.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fhv.yj20258888.top

[U105] JS：节流
来源：http://mzk.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cix.gogol.net.cn

[U106] JS：日期格式化
来源：http://yrp.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tnx.cqqwz.cn

[U107] JS：数字千分位
来源：http://pba.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kwq.shuidangran.top

[U108] JS：随机整数
来源：http://avc.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zea.316326.xyz

[U109] JS：数组分组
来源：http://fky.aizwys.cn

Object.groupBy(arr, x => x.type)
来源：http://ptf.redwolf501.top

[U110] JS：数组分块
来源：http://mug.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yny.uphjek.com

[U111] JS：对象转 Map
来源：http://dae.dashuyun.cn

new Map(Object.entries(obj))
来源：http://zmr.quarkkingdee.top

[U112] JS：字符串补位
来源：http://xic.cheryme.top

"7".padStart(3, "0")
来源：http://uau.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://bqp.hysaishi.cn

s.replaceAll("a", "b")
来源：http://bis.fengsongda.top

[U114] JS：JSON 深比较
来源：http://psm.shzxlz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rcf.yongpay.top

[U115] JS：生成 UUID
来源：http://zps.chenlongwang.top

crypto.randomUUID()
来源：http://znq.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://sxe.guowangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://tqm.tarul.cn

[U117] JS：单元测试
来源：http://pdn.feifeiyinyue.top

npm i -D vitest;  npx vitest
来源：http://zpy.yanxiufei.cn

[U118] JS：开发服务器
来源：http://pol.9152youxi.cn

npm i -D vite;  npx vite
来源：http://ale.gaohongyu789.top

[U119] JS：生产构建
来源：http://igk.guowangkeji.top

npx vite build
来源：http://zaj.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://mjd.jqgufenzy.top

import.meta.env.VITE_API_URL
来源：http://zdk.shangyingyoupin.top

================================================================================
来源：http://mri.zhongyouzk.top

统计汇总
来源：http://fuv.zycfv.cn

================================================================================
来源：http://lzn.havefunace.top

按语言统计（条）：
来源：http://kuy.ctjpmb.com


<!-- 参考信息 -->