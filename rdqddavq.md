代发 wailian999

[T41] Perl：Hello World
来源：http://xkk.hysaishi.cn

print "Hello\n";
来源：http://wxc.ybcxt.top

[T42] Perl：变量类型
来源：http://etk.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mio.cdnleiting.top

[T43] Perl：字符串插值
来源：http://yrt.wangdashe.top

"值: $a"
来源：http://pqp.hfpthk.cn

[T44] Perl：条件
来源：http://jey.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://aaw.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://lay.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://cee.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://zqz.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qdn.xuanzx.com

[T47] Perl：正则捕获
来源：http://izx.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://exu.yueranfly.top

[T48] Perl：正则替换
来源：http://qez.epnwcf.com

$s =~ s/old/new/g;
来源：http://gir.svipenyu.cn

[T49] Perl：函数
来源：http://fej.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tdo.daxiang520.top

[T50] Perl：逐行读文件
来源：http://bhi.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://duj.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://urr.gzhubu.top

[T51] Scala：Hello World
来源：http://kpx.cashguo.top

println("Hello")
来源：http://ani.shangyingyoupin.top

[T52] Scala：变量
来源：http://sqs.fzhhl.top

val a = 1;  var b = 2
来源：http://oyn.zhiwuduotai.top

[T53] Scala：字符串插值
来源：http://yul.hcnkem.com

s"值: $b"
来源：http://ccn.hnxiangtu.top

[T54] Scala：集合映射
来源：http://mfe.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://qac.yueranfly.top

[T55] Scala：集合过滤
来源：http://fed.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://tqr.daria6918.cn

[T56] Scala：样例类
来源：http://wbh.ivvv.top

case class User(name: String, age: Int)
来源：http://nys.52xcode.cn

[T57] Scala：模式匹配
来源：http://tee.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ufa.hnqzz.top

[T58] Scala：函数定义
来源：http://idu.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://qyc.zdbjq.cn

[T59] Scala：循环
来源：http://qew.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://flx.yueranfly.top

[T60] Scala：折叠
来源：http://zyi.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rtg.ehwqpu.com

================================================================================
来源：http://sgj.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://apz.jinqigfzy.top

================================================================================
来源：http://wye.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://asz.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://scl.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://ghg.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oxq.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://coa.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://tdw.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://mik.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rqc.iojbl.cn

[U05] Py：列表去重且保序
来源：http://pzu.hnqzz.top

list(dict.fromkeys(arr))
来源：http://ynz.yuxming.cn

[U06] Py：合并两个字典
来源：http://asn.zdbjq.cn

{**a, **b}
来源：http://wfw.wangdashe.top

[U07] Py：反转字典键值
来源：http://aoz.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://pyb.hysaishi.cn

[U08] Py：展平二维列表
来源：http://tzq.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://vdi.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://ngp.jlsjyb.cn

max(d, key=d.get)
来源：http://xpe.shuidangran.top

[U10] Py：按值排序字典
来源：http://zek.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fkf.yuxming.cn

[U11] Py：生成器表达式
来源：http://apl.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://ygy.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://qqi.c1oappe.top

Counter(arr).most_common(3)
来源：http://urr.zhoulong.xyz

[U13] Py：固定长度队列
来源：http://uqh.hammf.cn

deque(maxlen=10)
来源：http://epc.yj20258888.top

[U14] Py：分组收集到列表
来源：http://qcn.yanxiufei.cn

defaultdict(list)
来源：http://egt.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://fsi.shanyushiyangtech.top

t = time.perf_counter()
来源：http://art.epnwcf.com

[U16] Py：命令行参数解析
来源：http://reu.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bfm.jqgufenzy.top

[U17] Py：初始化日志
来源：http://fwi.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://gom.hywenlv.cn

[U18] Py：预编译正则
来源：http://lkz.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://sjp.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://xrf.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ops.vehdjk.com

[U20] Py：缓存函数结果
来源：http://axx.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://quc.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://rsw.0kj1m.cn

@contextlib.contextmanager
来源：http://xzq.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://nzl.bbcook.cn

list(zip(*m))
来源：http://btg.ydzc1.top

[U23] Py：分块读取大文件
来源：http://nwz.sufxvd.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cjb.feifeiyinyue.top

[U24] Py：路径操作
来源：http://itv.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xns.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://lso.yuanzhike.top

csv.DictReader(f)
来源：http://awf.cqqwz.cn

[U26] Py：并发下载
来源：http://nmj.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kfx.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://don.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://owl.cqqwz.cn

[U28] Py：类型别名
来源：http://kaa.gogol.net.cn

UserId = int
来源：http://wws.guowangkeji.top

[U29] Py：属性校验
来源：http://nxh.hfpthk.cn

@property 与 @x.setter 配合
来源：http://xpk.hcnkem.com

[U30] Py：数据类
来源：http://sjr.hesvh.cn

@dataclass(slots=True)
来源：http://dwm.yuxming.cn

[U31] Py：单测
来源：http://yuo.52xcode.cn

python -m pytest -q
来源：http://xaw.zycfv.cn

[U32] Py：代码格式化
来源：http://kls.nwbrower.top

ruff format . && ruff check --fix .
来源：http://fin.zhengqikj.top

[U33] Py：打包发布
来源：http://uhv.jianghu66.top

python -m build  （依赖 pyproject.toml）
来源：http://gfa.cqqwz.cn

[U34] Py：判断编码
来源：http://dgo.bjfxy.top

chardet.detect(raw)
来源：http://yli.meibo888.top

[U35] Py：发送邮件
来源：http://xbm.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kqi.jyoumei.cn

[U36] Py：定时任务
来源：http://vpl.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://rvb.ydzc1.top

[U37] Py：读写 Excel
来源：http://qqo.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://nlm.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://mqe.zdbjq.cn

Path(__file__).resolve().parent
来源：http://cho.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://hvo.9152youxi.cn

sys.stdout.isatty()
来源：http://rcs.cheryme.top

[U40] Py：打印到标准错误
来源：http://fwd.yuanzhike.top

print("err", file=sys.stderr)
来源：http://lay.hnxiangtu.top

[U41] PHP：初始化 Composer 项目
来源：http://vgu.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://xih.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://ujh.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ryx.nwbrower.top

[U43] PHP：声明命名空间
来源：http://axy.yj202588.top

namespace App\Http;
来源：http://efp.zycfv.cn

[U44] PHP：开启严格类型
来源：http://jvh.hnqzz.top

declare(strict_types=1);
来源：http://kcs.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://qby.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jdb.zhoulong.xyz

[U46] PHP：可空类型
来源：http://opy.yuanzhike.top

?string $name = null
来源：http://byx.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://ooi.gaohongyu789.top

int|string $id
来源：http://gje.hysaishi.cn

[U48] PHP：纯枚举
来源：http://oil.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cpi.jiagoushi.top

[U49] PHP：只读属性
来源：http://mym.birdmap.top

public readonly string $name
来源：http://qed.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://pph.wangdashe.top

public function __construct(private int $id) {}
来源：http://jty.vqdsnc.cn

[U51] PHP：数组解构
来源：http://ikb.sufxvd.cn

[$a, $b] = $arr;
来源：http://bcx.mhx1999.top

[U52] PHP：箭头函数
来源：http://aks.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://wlc.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://lqn.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://wys.yonumen.top

[U54] PHP：空安全调用
来源：http://inc.yonumen.top

$obj?->method()
来源：http://cjq.wangdashe.top

[U55] PHP：match 表达式
来源：http://huq.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yer.fengsongda.top

[U56] PHP：命名参数
来源：http://auh.xylfe.cn

f(a: 1, b: 2)
来源：http://owt.9152youxi.cn

[U57] PHP：字符串插值
来源：http://lrs.dashuyun.cn

"值: {$a}"
来源：http://zsj.zdqjudy.top

[U58] PHP：数组三件套
来源：http://ale.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xay.jqgfzy.top

[U59] PHP：自定义排序
来源：http://rnv.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bju.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://jnc.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://osc.gogol.net.cn

[U61] PHP：正则
来源：http://ipi.jyoumei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bio.dashuyun.cn

[U62] PHP：日期对象
来源：http://ewi.sweek.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://toz.cheryme.top

[U63] PHP：文件读写
来源：http://jtj.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bnf.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://rqk.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://ttg.fzhhl.top

[U65] PHP：会话
来源：http://dej.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tyu.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://thc.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mlh.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://hfa.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pjb.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://oyb.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://izt.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://dbl.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://juf.xuanzx.com

[U70] PHP：PDO 事务
来源：http://pdk.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dyq.fengsongda.top

[U71] PHP：抛出异常
来源：http://axl.zdqjudy.top

throw new RuntimeException("失败", 500);
来源：http://wrr.havefunace.top

[U72] PHP：写错误日志
来源：http://lus.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://egh.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://hoo.birdmap.top

parse_ini_file("config.ini", true)
来源：http://edh.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://kgb.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://ers.xylfe.cn

[U75] PHP：依赖注入
来源：http://wep.jyoumei.cn

composer require psr/container
来源：http://cgo.xziqi.cn

[U76] PHP：简单路由
来源：http://wxm.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://joc.ivvv.top

[U77] PHP：模板渲染
来源：http://ywj.yongpay.top

composer require twig/twig
来源：http://tbn.sxryk.cn

[U78] PHP：单元测试
来源：http://pgz.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://tbm.quarkkingdee.top

[U79] PHP：静态分析
来源：http://fbg.jianghu66.top

composer require --dev phpstan/phpstan
来源：http://qap.wangdashe.top

[U80] PHP：代码规范修复
来源：http://zuv.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jss.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://kkx.jiagoushi.top

npm init -y;  npm i express
来源：http://byw.pycfn.com

[U82] JS：package.json 脚本
来源：http://iaj.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iab.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://ojl.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://xwf.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://nzv.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://waz.uphjek.com

[U85] JS：可选链
来源：http://dpi.xingfuxueyuan.xyz

a?.b?.c
来源：http://aqi.9152youxi.cn

[U86] JS：空值合并
来源：http://jla.ydzc1.top

a ?? b
来源：http://adi.ybcxt.top

[U87] JS：解构默认值
来源：http://yhg.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://sgt.jinqigufen.top

[U88] JS：对象展开合并
来源：http://xko.zhijiandao.cn

{ ...a, ...b }
来源：http://uax.hammf.cn

[U89] JS：数组去重
来源：http://ouw.jiagoushi.top

[...new Set(arr)]
来源：http://twn.yfazqb.com

[U90] JS：数字数组排序
来源：http://lqs.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://rdr.yueranfly.top

[U91] JS：对象键值遍历
来源：http://cuh.zhongyouzk.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hed.52xcode.cn

[U92] JS：深拷贝
来源：http://dmn.jqgfzy.top

structuredClone(obj)
来源：http://oot.chenlongwang.top

[U93] JS：模板字符串
来源：http://vse.redwolf501.top

`共 ${n} 条`
来源：http://ysh.hcnkem.com

[U94] JS：箭头函数
来源：http://lkt.kuanghao11.cn

const double = x => x * 2;
来源：http://uai.yongpay.top

[U95] JS：Promise 包装
来源：http://deq.hammf.cn

new Promise((resolve, reject) => {})
来源：http://fxe.smart0.xyz

[U96] JS：async/await 与异常
来源：http://lpb.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zid.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://xpg.yj20258888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://cwn.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://dpl.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lew.fehbvm.com

[U99] JS：事件监听
来源：http://xqq.cdnleiting.top

el.addEventListener("click", e => {})
来源：http://oqr.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://ieg.hammf.cn

document.querySelector(".item")
来源：http://zjc.shangyingyoupin.top

[U101] JS：classList 操作
来源：http://ups.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://xgr.guannengcc.top

[U102] JS：本地存储
来源：http://pkf.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://xor.316326.xyz

[U103] JS：定时器
来源：http://zwr.yj20258.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://guc.yj202588.top

[U104] JS：防抖
来源：http://heg.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iuq.zycfv.cn

[U105] JS：节流
来源：http://dbv.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ebe.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://lsa.jinqigufen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qny.pengpengdd.cyou

[U107] JS：数字千分位
来源：http://oce.gogol.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zcc.ydzc1.top

[U108] JS：随机整数
来源：http://lnr.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://esd.cucudq.cn

[U109] JS：数组分组
来源：http://epw.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://ayu.jlsjyb.cn

[U110] JS：数组分块
来源：http://lzk.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gft.zycfv.cn

[U111] JS：对象转 Map
来源：http://izq.cucudq.cn

new Map(Object.entries(obj))
来源：http://vcu.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://jkd.jianghu66.top

"7".padStart(3, "0")
来源：http://nny.ehwqpu.com

[U113] JS：正则替换全部
来源：http://gvq.uphjek.com

s.replaceAll("a", "b")
来源：http://moq.guannengcc.top

[U114] JS：JSON 深比较
来源：http://kch.epnwcf.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dqn.hammf.cn

[U115] JS：生成 UUID
来源：http://txm.chenlongwang.top

crypto.randomUUID()
来源：http://mzo.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://fom.jyoumei.cn

/** @param {string} name */ function f(name) {}
来源：http://goc.9152youxi.cn

[U117] JS：单元测试
来源：http://guc.hcnkem.com

npm i -D vitest;  npx vitest
来源：http://tyu.jlsjyb.cn

[U118] JS：开发服务器
来源：http://fjs.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://kie.epnwcf.com

[U119] JS：生产构建
来源：http://tqw.vqdsnc.cn

npx vite build
来源：http://xun.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://ssv.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://yeh.jlsjyb.cn

================================================================================
来源：http://kgj.zdqjudy.top

统计汇总
来源：http://zzf.guannengcc.top

================================================================================
来源：http://kyk.yongpay.top

按语言统计（条）：
来源：http://pkc.guowangkeji.top

Python ......... 252
来源：http://mae.zhengqikj.top

PHP ............ 252
来源：http://vxu.zdqjudy.top

JavaScript ..... 252
来源：http://wng.bjfxy.top

TypeScript ..... 212
来源：http://exk.ehwqpu.com

Java ........... 212
来源：http://vht.uphjek.com

Go ............. 212
来源：http://ihl.ydjk.org.cn

Ruby ........... 212
来源：http://lgy.gaohongyu789.top

C# ............. 212
来源：http://frw.316326.xyz

C .............. 30
来源：http://sdr.hnxiangtu.top

C++ ............ 30
来源：http://ple.fehbvm.com

SQL ............ 90
来源：http://cqk.vqdsnc.cn

Bash ........... 80
来源：http://zaa.hnqzz.top


<!-- 参考信息 -->