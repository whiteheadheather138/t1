代发 wailian999

[T43] Perl：字符串插值
来源：http://igt.sjlbkw.cn

"值: $a"
来源：http://fjr.sufxvd.cn

[T44] Perl：条件
来源：http://ify.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://vyu.sufxvd.cn

[T45] Perl：数组遍历
来源：http://eln.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://kak.jiagoushi.top

[T46] Perl：哈希操作
来源：http://xus.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://whp.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://esd.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dcf.gotoacloud.top

[T48] Perl：正则替换
来源：http://rjx.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://aip.gotoacloud.top

[T49] Perl：函数
来源：http://byz.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hoj.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://lvm.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xtl.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://pof.zycfv.cn

[T51] Scala：Hello World
来源：http://bai.zhengqikj.top

println("Hello")
来源：http://zok.yongpay.top

[T52] Scala：变量
来源：http://ugy.cqqwz.cn

val a = 1;  var b = 2
来源：http://vtv.aizwys.cn

[T53] Scala：字符串插值
来源：http://bzd.ydjk.org.cn

s"值: $b"
来源：http://bmj.yuanzhike.top

[T54] Scala：集合映射
来源：http://kcp.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://eew.tianlin.xyz

[T55] Scala：集合过滤
来源：http://nld.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://yvc.guowangkeji.top

[T56] Scala：样例类
来源：http://rjh.cucudq.cn

case class User(name: String, age: Int)
来源：http://ave.guowangkeji.top

[T57] Scala：模式匹配
来源：http://aig.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aed.shzxlz.cn

[T58] Scala：函数定义
来源：http://uck.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://pas.yonumen.top

[T59] Scala：循环
来源：http://iva.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://ylg.iojbl.cn

[T60] Scala：折叠
来源：http://hwl.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wyu.tianlin.xyz

================================================================================
来源：http://cft.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ext.zdbjq.cn

================================================================================
来源：http://fxk.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://yte.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://dmv.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://kxz.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wdf.yonumen.top

[U03] Py：加载 .env 配置
来源：http://gxr.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lch.andypj.xyz

[U04] Py：变量调试打印
来源：http://qfs.xingfuxueyuan.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tmk.smart0.xyz

[U05] Py：列表去重且保序
来源：http://rxf.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://otd.pycfn.com

[U06] Py：合并两个字典
来源：http://vqe.zhongyouzk.top

{**a, **b}
来源：http://nmr.yonumen.top

[U07] Py：反转字典键值
来源：http://kxt.xylfe.cn

{v: k for k, v in d.items()}
来源：http://bvx.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://hti.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://sxy.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://ezn.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://axr.316326.xyz

[U10] Py：按值排序字典
来源：http://zbn.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wag.yvedp.cn

[U11] Py：生成器表达式
来源：http://lxg.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://gni.hnxiangtu.top

[U12] Py：取出现最多的 3 个元素
来源：http://wgw.aibaodan.cn

Counter(arr).most_common(3)
来源：http://fqd.zycfv.cn

[U13] Py：固定长度队列
来源：http://eoa.gzhubu.top

deque(maxlen=10)
来源：http://mtm.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://sui.wangshuangyany.cn

defaultdict(list)
来源：http://sfz.jinyuanbaomall.cn

[U15] Py：高精度计时
来源：http://wxw.kuanghao11.cn

t = time.perf_counter()
来源：http://rry.jqgufenzy.top

[U16] Py：命令行参数解析
来源：http://jjb.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xvd.quarkkingdee.top

[U17] Py：初始化日志
来源：http://mrr.daxiang520.top

logging.basicConfig(level=logging.INFO)
来源：http://aym.cashguo.top

[U18] Py：预编译正则
来源：http://ueo.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://mwp.bbcook.cn

[U19] Py：正则替换带回调
来源：http://vbu.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uok.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://run.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://jmf.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://fpi.zycfv.cn

@contextlib.contextmanager
来源：http://myb.52xcode.cn

[U22] Py：矩阵转置
来源：http://sbn.feifeiyinyue.top

list(zip(*m))
来源：http://jpc.fehbvm.com

[U23] Py：分块读取大文件
来源：http://drk.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mqs.kuanghao11.cn

[U24] Py：路径操作
来源：http://frl.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rtg.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://kyn.52xcode.cn

csv.DictReader(f)
来源：http://fiz.ivvv.top

[U26] Py：并发下载
来源：http://kcc.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zqm.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://btq.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://scw.hesvh.cn

[U28] Py：类型别名
来源：http://wmo.nwbrower.top

UserId = int
来源：http://ivu.tian-w.cn

[U29] Py：属性校验
来源：http://hkn.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://coa.bjfxy.top

[U30] Py：数据类
来源：http://nhv.zdbjq.cn

@dataclass(slots=True)
来源：http://vvk.hnxiangtu.top

[U31] Py：单测
来源：http://cqi.sufxvd.cn

python -m pytest -q
来源：http://qid.birdmap.top

[U32] Py：代码格式化
来源：http://ovt.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://udl.daria6918.cn

[U33] Py：打包发布
来源：http://oip.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://wio.jinqigfzy.top

[U34] Py：判断编码
来源：http://oht.cheryme.top

chardet.detect(raw)
来源：http://qxx.sweek.top

[U35] Py：发送邮件
来源：http://hve.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cmf.meibo888.top

[U36] Py：定时任务
来源：http://pmt.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://mat.fehbvm.com

[U37] Py：读写 Excel
来源：http://okt.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ptj.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://nno.pycfn.com

Path(__file__).resolve().parent
来源：http://izu.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://nsc.yonumen.top

sys.stdout.isatty()
来源：http://god.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://vor.yonumen.top

print("err", file=sys.stderr)
来源：http://jgb.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://aoo.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ybh.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://pjj.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dbg.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://opx.xziqi.cn

namespace App\Http;
来源：http://cce.jlsjyb.cn

[U44] PHP：开启严格类型
来源：http://lsh.zycfv.cn

declare(strict_types=1);
来源：http://kcn.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://pia.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cgn.c1oappe.top

[U46] PHP：可空类型
来源：http://rpb.ybcxt.top

?string $name = null
来源：http://nbc.zdbjq.cn

[U47] PHP：联合类型
来源：http://hhr.zhiwuduotai.top

int|string $id
来源：http://lun.andypj.xyz

[U48] PHP：纯枚举
来源：http://vxr.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mmh.0kj1m.cn

[U49] PHP：只读属性
来源：http://tir.zhongyouzk.top

public readonly string $name
来源：http://hpk.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://lez.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://xsi.nanxuanxn.top

[U51] PHP：数组解构
来源：http://eur.ybcxt.top

[$a, $b] = $arr;
来源：http://esf.xuanzx.com

[U52] PHP：箭头函数
来源：http://lpo.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://oif.yj20258888.top

[U53] PHP：空合并运算符
来源：http://yhg.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://wnj.jiagoushi.top

[U54] PHP：空安全调用
来源：http://azj.aibaodan.cn

$obj?->method()
来源：http://jvq.yvedp.cn

[U55] PHP：match 表达式
来源：http://znd.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hli.cashguo.top

[U56] PHP：命名参数
来源：http://dhn.aibaodan.cn

f(a: 1, b: 2)
来源：http://lnd.tarul.cn

[U57] PHP：字符串插值
来源：http://jzl.ywan-chungtsiang.top

"值: {$a}"
来源：http://zsb.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://mpa.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jvu.gotoacloud.top

[U59] PHP：自定义排序
来源：http://qio.0kj1m.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nke.guannengcc.top

[U60] PHP：JSON 编解码
来源：http://gem.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://erl.guowangkeji.top

[U61] PHP：正则
来源：http://xmw.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tas.cucudq.cn

[U62] PHP：日期对象
来源：http://twi.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nui.aibaodan.cn

[U63] PHP：文件读写
来源：http://hwa.tianlin.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yfh.zhixingplan.top

[U64] PHP：目录遍历
来源：http://ypz.pengpengdd.cyou

glob("dir/*.php");  scandir("dir");
来源：http://zar.9152youxi.cn

[U65] PHP：会话
来源：http://ldv.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ndh.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://faq.andypj.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sci.yueranfly.top

[U67] PHP：处理文件上传
来源：http://qsu.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fbo.yfazqb.com

[U68] PHP：PDO 连接
来源：http://cbv.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xgg.tarul.cn

[U69] PHP：PDO 预处理
来源：http://kcz.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sss.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://jnz.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zfd.hammf.cn

[U71] PHP：抛出异常
来源：http://agg.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://wiz.yj20258.top

[U72] PHP：写错误日志
来源：http://pvf.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://uhm.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://wzj.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://uct.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://kwo.yongpay.top

getenv("APP_ENV") ?: "production"
来源：http://bgs.fehbvm.com

[U75] PHP：依赖注入
来源：http://xgr.hongshengwenyu.top

composer require psr/container
来源：http://vsh.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://dbd.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jjt.gotoacloud.top

[U77] PHP：模板渲染
来源：http://wjp.redwolf501.top

composer require twig/twig
来源：http://nho.cqqwz.cn

[U78] PHP：单元测试
来源：http://vkm.nwbrower.top

composer require --dev phpunit/phpunit
来源：http://zce.hywenlv.cn

[U79] PHP：静态分析
来源：http://wee.nanxinkj.top

composer require --dev phpstan/phpstan
来源：http://kvk.jyoumei.cn

[U80] PHP：代码规范修复
来源：http://bgt.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xtm.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://xbe.pycfn.com

npm init -y;  npm i express
来源：http://fiv.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://oin.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://arl.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://uer.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://gck.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://wco.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://qus.yanxiufei.cn

[U85] JS：可选链
来源：http://nhk.cheryme.top

a?.b?.c
来源：http://iqn.zhixingplan.top

[U86] JS：空值合并
来源：http://okm.pycfn.com

a ?? b
来源：http://mfn.guannengcc.top

[U87] JS：解构默认值
来源：http://gba.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://zmh.daria6918.cn

[U88] JS：对象展开合并
来源：http://kdi.gotoacloud.top

{ ...a, ...b }
来源：http://oen.bjfxy.top

[U89] JS：数组去重
来源：http://nag.jinghuilouyu.cn

[...new Set(arr)]
来源：http://yjr.cashguo.top

[U90] JS：数字数组排序
来源：http://mpp.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://oti.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://ljo.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ikj.yj20258888.top

[U92] JS：深拷贝
来源：http://xic.aibaodan.cn

structuredClone(obj)
来源：http://asg.yuxming.cn

[U93] JS：模板字符串
来源：http://feb.cdnleiting.top

`共 ${n} 条`
来源：http://jsq.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://pgx.cqqwz.cn

const double = x => x * 2;
来源：http://vjw.chenlongwang.top

[U95] JS：Promise 包装
来源：http://diq.wangshuangyany.cn

new Promise((resolve, reject) => {})
来源：http://cgk.aibaodan.cn

[U96] JS：async/await 与异常
来源：http://prd.hongshengwenyu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ghb.dianchejie.cn

[U97] JS：并发请求
来源：http://ydo.52xcode.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://stj.chenjidiqi.icu

[U98] JS：fetch 带 JSON
来源：http://fdt.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://woq.yonumen.top

[U99] JS：事件监听
来源：http://ecp.hysaishi.cn

el.addEventListener("click", e => {})
来源：http://ulc.pycfn.com

[U100] JS：DOM 查询
来源：http://yue.yongpay.top

document.querySelector(".item")
来源：http://bcq.zhixingplan.top

[U101] JS：classList 操作
来源：http://bxl.dashuyun.cn

el.classList.toggle("active")
来源：http://kjo.ppjwa.cn

[U102] JS：本地存储
来源：http://lzx.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://tvv.wangdashe.top

[U103] JS：定时器
来源：http://aak.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xym.dianchejie.cn

[U104] JS：防抖
来源：http://tls.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgf.jinqigufen.top

[U105] JS：节流
来源：http://bbr.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xzx.hfpthk.cn

[U106] JS：日期格式化
来源：http://wwc.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iyl.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://fms.ppjwa.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kyp.tian-w.cn

[U108] JS：随机整数
来源：http://fcm.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://poy.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://wbm.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://iuh.ydjk.org.cn

[U110] JS：数组分块
来源：http://khv.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aqj.jinghuilouyu.cn

[U111] JS：对象转 Map
来源：http://vps.ydzc1.top

new Map(Object.entries(obj))
来源：http://qrc.chenlongwang.top

[U112] JS：字符串补位
来源：http://xyf.tian-w.cn

"7".padStart(3, "0")
来源：http://ezv.redwolf501.top

[U113] JS：正则替换全部
来源：http://zat.jinyuanbaomall.cn

s.replaceAll("a", "b")
来源：http://zae.52xcode.cn

[U114] JS：JSON 深比较
来源：http://snt.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iiq.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://mdf.ydjk.org.cn

crypto.randomUUID()
来源：http://xqi.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://ajc.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://tqv.yfazqb.com

[U117] JS：单元测试
来源：http://nfy.pycfn.com

npm i -D vitest;  npx vitest
来源：http://vlk.daxiang520.top

[U118] JS：开发服务器
来源：http://wwf.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://axn.yanxiufei.cn

[U119] JS：生产构建
来源：http://phg.chenjidiqi.icu

npx vite build
来源：http://utn.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://fib.316326.xyz

import.meta.env.VITE_API_URL
来源：http://tmu.zhoulong.xyz

================================================================================
来源：http://xqy.feifeiyinyue.top

统计汇总
来源：http://mqm.wangshuangyany.cn

================================================================================
来源：http://qbw.iojbl.cn

按语言统计（条）：
来源：http://soc.epnwcf.com

Python ......... 252
来源：http://ctx.zdbjq.cn

PHP ............ 252
来源：http://hzp.nwbrower.top

JavaScript ..... 252
来源：http://ctx.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://nci.quarkkingdee.top

Java ........... 212
来源：http://pfr.cdnleiting.top

Go ............. 212
来源：http://wvm.52xcode.cn

Ruby ........... 212
来源：http://gfw.sufxvd.cn

C# ............. 212
来源：http://kmw.chenzaomai.com

C .............. 30
来源：http://vzj.chenlongwang.top

C++ ............ 30
来源：http://pke.jyoumei.cn

SQL ............ 90
来源：http://jnw.zhoulong.xyz

Bash ........... 80
来源：http://rfm.jinqigfzy.top

Kotlin ......... 15
来源：http://ybu.nanxuanxn.top

Swift .......... 15
来源：http://hts.fehbvm.com

Lua ............ 10
来源：http://evc.vehdjk.com

Perl ........... 10
来源：http://qos.jyoumei.cn


<!-- 参考信息 -->