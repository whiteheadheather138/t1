代发 wailian999

[T43] Perl：字符串插值
来源：http://kfs.meibo888.top

"值: $a"
来源：http://rlv.shanyushiyangtech.top

[T44] Perl：条件
来源：http://opk.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://zty.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://jzq.ivvv.top

for my $x (@arr) { print $x; }
来源：http://rpa.yj20258.top

[T46] Perl：哈希操作
来源：http://zms.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xls.zdqjudy.top

[T47] Perl：正则捕获
来源：http://zto.tarul.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oni.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://fcl.haohaochexian.top

$s =~ s/old/new/g;
来源：http://uhs.gotoacloud.top

[T49] Perl：函数
来源：http://pdc.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fas.havefunace.top

[T50] Perl：逐行读文件
来源：http://lgw.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://hzo.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://acy.gaohongyu789.top

[T51] Scala：Hello World
来源：http://kdb.hesvh.cn

println("Hello")
来源：http://yxh.fktsv.cn

[T52] Scala：变量
来源：http://kfl.nwbrower.top

val a = 1;  var b = 2
来源：http://mhj.chenzaomai.com

[T53] Scala：字符串插值
来源：http://rfx.gogol.net.cn

s"值: $b"
来源：http://wrr.hesvh.cn

[T54] Scala：集合映射
来源：http://zre.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://olw.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://doz.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vsu.nanxuanxn.top

[T56] Scala：样例类
来源：http://cgp.daxiang520.top

case class User(name: String, age: Int)
来源：http://jxq.vqdsnc.cn

[T57] Scala：模式匹配
来源：http://aai.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hvr.zhongyouzk.top

[T58] Scala：函数定义
来源：http://mcq.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://pna.quarkkingdee.top

[T59] Scala：循环
来源：http://rvn.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://gbl.guannengcc.top

[T60] Scala：折叠
来源：http://xgd.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fdg.uphjek.com

================================================================================
来源：http://ipn.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xzg.jinyuanbaomall.cn

================================================================================
来源：http://sel.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://oll.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jze.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://xis.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhz.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://guj.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oje.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://tyb.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sol.iojbl.cn

[U05] Py：列表去重且保序
来源：http://woh.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://vgu.fktsv.cn

[U06] Py：合并两个字典
来源：http://vmq.ywan-chungtsiang.top

{**a, **b}
来源：http://sok.feifeiyinyue.top

[U07] Py：反转字典键值
来源：http://mrf.yj20258888.top

{v: k for k, v in d.items()}
来源：http://zbu.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://yfi.yfazqb.com

[y for x in nested for y in x]
来源：http://tbt.cheryme.top

[U09] Py：字典取最大值的键
来源：http://lyr.zhiwuduotai.top

max(d, key=d.get)
来源：http://jas.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://yep.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nna.sufxvd.cn

[U11] Py：生成器表达式
来源：http://qph.yanxiufei.cn

(x * 2 for x in arr)
来源：http://cxt.haohaochexian.top

[U12] Py：取出现最多的 3 个元素
来源：http://ght.sysykeji.top

Counter(arr).most_common(3)
来源：http://hqh.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://wtf.zhijiandao.cn

deque(maxlen=10)
来源：http://okz.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://zvo.wangshuangyany.cn

defaultdict(list)
来源：http://cxq.yanxiufei.cn

[U15] Py：高精度计时
来源：http://cjy.hfpthk.cn

t = time.perf_counter()
来源：http://jim.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://vfk.52xcode.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xel.yfazqb.com

[U17] Py：初始化日志
来源：http://cwk.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://tgq.andypj.xyz

[U18] Py：预编译正则
来源：http://czz.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://rxr.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://qcs.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hji.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://bzt.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://omf.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://olz.feifeiyinyue.top

@contextlib.contextmanager
来源：http://vfb.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://oiy.jiagoushi.top

list(zip(*m))
来源：http://ejv.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://pbl.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lwl.gogol.net.cn

[U24] Py：路径操作
来源：http://inv.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qcp.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://awu.wangshuangyany.cn

csv.DictReader(f)
来源：http://rti.ivvv.top

[U26] Py：并发下载
来源：http://tdn.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gir.tarul.cn

[U27] Py：异步 HTTP
来源：http://tou.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://mtg.sjlbkw.cn

[U28] Py：类型别名
来源：http://zvf.zhengqikj.top

UserId = int
来源：http://taj.52xcode.cn

[U29] Py：属性校验
来源：http://uby.zdbjq.cn

@property 与 @x.setter 配合
来源：http://znk.dashuyun.cn

[U30] Py：数据类
来源：http://tcx.hywenlv.cn

@dataclass(slots=True)
来源：http://gaq.smart0.xyz

[U31] Py：单测
来源：http://ciy.hnqzz.top

python -m pytest -q
来源：http://kbt.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://dcb.ybcxt.top

ruff format . && ruff check --fix .
来源：http://yym.tianlin.xyz

[U33] Py：打包发布
来源：http://zgt.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://buu.yj202588.top

[U34] Py：判断编码
来源：http://dvt.jqgfzy.top

chardet.detect(raw)
来源：http://xqz.xylfe.cn

[U35] Py：发送邮件
来源：http://khr.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lfc.shangyingyoupin.top

[U36] Py：定时任务
来源：http://ann.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://tdd.yuxming.cn

[U37] Py：读写 Excel
来源：http://ylr.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://phn.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://pwu.guowangkeji.top

Path(__file__).resolve().parent
来源：http://lye.jinqigufen.top

[U39] Py：判断是否在交互环境
来源：http://jxn.yonumen.top

sys.stdout.isatty()
来源：http://zbj.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://uex.zdbjq.cn

print("err", file=sys.stderr)
来源：http://wdu.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://kwl.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xlj.shangyingyoupin.top

[U42] PHP：PSR-4 自动加载
来源：http://nzw.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gzy.yuxming.cn

[U43] PHP：声明命名空间
来源：http://nfu.smart0.xyz

namespace App\Http;
来源：http://jjg.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://diu.52xcode.cn

declare(strict_types=1);
来源：http://igh.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://ehe.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iso.gotoacloud.top

[U46] PHP：可空类型
来源：http://fok.9152youxi.cn

?string $name = null
来源：http://okp.vqdsnc.cn

[U47] PHP：联合类型
来源：http://czm.svipenyu.cn

int|string $id
来源：http://avy.yvedp.cn

[U48] PHP：纯枚举
来源：http://hth.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nbo.cqqwz.cn

[U49] PHP：只读属性
来源：http://hzu.yj20258888.top

public readonly string $name
来源：http://icr.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://dcx.ybcxt.top

public function __construct(private int $id) {}
来源：http://brb.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://tkz.wangdashe.top

[$a, $b] = $arr;
来源：http://dzx.zdbjq.cn

[U52] PHP：箭头函数
来源：http://zwn.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://sxd.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://nwd.xuetiantiany.cn

$v = $a ?? $b ?? "default";
来源：http://mcn.ppjwa.cn

[U54] PHP：空安全调用
来源：http://ryj.guowangkeji.top

$obj?->method()
来源：http://oaj.zdbjq.cn

[U55] PHP：match 表达式
来源：http://trk.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ftz.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://yfr.guowangkeji.top

f(a: 1, b: 2)
来源：http://fvq.vehdjk.com

[U57] PHP：字符串插值
来源：http://wai.ppjwa.cn

"值: {$a}"
来源：http://sui.yuanzhike.top

[U58] PHP：数组三件套
来源：http://thf.jinqigfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mlj.ppjwa.cn

[U59] PHP：自定义排序
来源：http://gvg.kuanghao11.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ulj.jyoumei.cn

[U60] PHP：JSON 编解码
来源：http://dyj.sweek.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://acp.yuanzhike.top

[U61] PHP：正则
来源：http://eok.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rnv.haohaochexian.top

[U62] PHP：日期对象
来源：http://yis.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hkp.pycfn.com

[U63] PHP：文件读写
来源：http://rlz.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vxo.gzhubu.top

[U64] PHP：目录遍历
来源：http://cvc.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://bfi.jinghuilouyu.cn

[U65] PHP：会话
来源：http://bie.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vfp.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://urg.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://osv.tian-w.cn

[U67] PHP：处理文件上传
来源：http://gzj.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ciu.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://lrg.yangfankeji.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dbl.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://vaz.52xcode.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zyj.jianghu66.top

[U70] PHP：PDO 事务
来源：http://ddh.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dsh.daria6918.cn

[U71] PHP：抛出异常
来源：http://lgs.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://eyw.jqgfzy.top

[U72] PHP：写错误日志
来源：http://ugg.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://sdh.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://uyk.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://jqs.shuidangran.top

[U74] PHP：读取环境变量
来源：http://qsx.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://xnr.zhengqikj.top

[U75] PHP：依赖注入
来源：http://vvx.sjlbkw.cn

composer require psr/container
来源：http://ypz.yongpay.top

[U76] PHP：简单路由
来源：http://vzo.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dnj.hammf.cn

[U77] PHP：模板渲染
来源：http://wdy.kuanghao11.cn

composer require twig/twig
来源：http://aab.ybcxt.top

[U78] PHP：单元测试
来源：http://orl.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://peh.cdnleiting.top

[U79] PHP：静态分析
来源：http://akw.shanyushiyangtech.top

composer require --dev phpstan/phpstan
来源：http://cpn.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://cjg.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://dqb.yueranfly.top

[U81] JS：初始化项目
来源：http://rts.hongshengwenyu.top

npm init -y;  npm i express
来源：http://ldc.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://wod.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zey.hfpthk.cn

[U83] JS：ES Module 导入导出
来源：http://wra.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ubf.yonumen.top

[U84] JS：CommonJS 写法
来源：http://efu.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://llu.gaohongyu789.top

[U85] JS：可选链
来源：http://uqc.0kj1m.cn

a?.b?.c
来源：http://cym.c1oappe.top

[U86] JS：空值合并
来源：http://cdk.bbcook.cn

a ?? b
来源：http://mrn.yvedp.cn

[U87] JS：解构默认值
来源：http://vva.xuanzx.com

const { a = 1, b = 2 } = obj;
来源：http://gnv.hysaishi.cn

[U88] JS：对象展开合并
来源：http://nwr.9152youxi.cn

{ ...a, ...b }
来源：http://nqr.vehdjk.com

[U89] JS：数组去重
来源：http://dkl.cashguo.top

[...new Set(arr)]
来源：http://fxh.jianghu66.top

[U90] JS：数字数组排序
来源：http://nlp.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://nkn.xziqi.cn

[U91] JS：对象键值遍历
来源：http://dhh.gogol.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yro.dianchejie.cn

[U92] JS：深拷贝
来源：http://uas.zdqjudy.top

structuredClone(obj)
来源：http://ghq.sufxvd.cn

[U93] JS：模板字符串
来源：http://zfs.yj20258888.top

`共 ${n} 条`
来源：http://dbo.yanxiufei.cn

[U94] JS：箭头函数
来源：http://wuj.dianchejie.cn

const double = x => x * 2;
来源：http://wym.xingfuxueyuan.xyz

[U95] JS：Promise 包装
来源：http://wci.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://hfl.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://cho.gzhubu.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jve.sweek.top

[U97] JS：并发请求
来源：http://xao.ybcxt.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pdp.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://jos.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://owf.9152youxi.cn

[U99] JS：事件监听
来源：http://ief.vehdjk.com

el.addEventListener("click", e => {})
来源：http://hrn.nanxinkj.top

[U100] JS：DOM 查询
来源：http://dfo.hongshengwenyu.top

document.querySelector(".item")
来源：http://iaf.dianchejie.cn

[U101] JS：classList 操作
来源：http://bsn.wangdashe.top

el.classList.toggle("active")
来源：http://brs.wangdashe.top

[U102] JS：本地存储
来源：http://snj.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://crr.vqdsnc.cn

[U103] JS：定时器
来源：http://oad.bjfxy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://snz.epnwcf.com

[U104] JS：防抖
来源：http://ufj.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcd.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://vbu.0kj1m.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gpn.jiagoushi.top

[U106] JS：日期格式化
来源：http://keh.zhongyouzk.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://imf.9152youxi.cn

[U107] JS：数字千分位
来源：http://ttj.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yno.sjlbkw.cn

[U108] JS：随机整数
来源：http://int.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pbm.yuanzhike.top

[U109] JS：数组分组
来源：http://rla.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://mtb.zhoulong.xyz

[U110] JS：数组分块
来源：http://mgn.ywan-chungtsiang.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bjj.sweek.top

[U111] JS：对象转 Map
来源：http://zqo.wangdashe.top

new Map(Object.entries(obj))
来源：http://tly.dashuyun.cn

[U112] JS：字符串补位
来源：http://wyo.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://gpx.sweek.top

[U113] JS：正则替换全部
来源：http://vte.fzhhl.top

s.replaceAll("a", "b")
来源：http://ytp.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://ajl.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vky.vehdjk.com

[U115] JS：生成 UUID
来源：http://kne.sweek.top

crypto.randomUUID()
来源：http://zro.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://gpa.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://zsl.jinqigufen.top

[U117] JS：单元测试
来源：http://ioh.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://mvy.316326.xyz

[U118] JS：开发服务器
来源：http://zym.fktsv.cn

npm i -D vite;  npx vite
来源：http://fiv.yonumen.top

[U119] JS：生产构建
来源：http://xih.xuetiantiany.cn

npx vite build
来源：http://pgt.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://lya.yongpay.top

import.meta.env.VITE_API_URL
来源：http://pgc.jqgufenzy.top

================================================================================
来源：http://lil.shangyingyoupin.top

统计汇总
来源：http://ryo.meibo888.top

================================================================================
来源：http://viv.zhiwuduotai.top

按语言统计（条）：
来源：http://pup.meibo888.top

Python ......... 252
来源：http://iqk.quarkkingdee.top

PHP ............ 252
来源：http://hpe.ppjwa.cn

JavaScript ..... 252
来源：http://chv.cheryme.top

TypeScript ..... 212
来源：http://poz.yongpay.top

Java ........... 212
来源：http://liy.yanxiufei.cn

Go ............. 212
来源：http://teg.gaohongyu789.top

Ruby ........... 212
来源：http://tte.tianlin.xyz

C# ............. 212
来源：http://ebz.ydzc1.top

C .............. 30
来源：http://yjz.ydzc1.top

C++ ............ 30
来源：http://zfy.shanyushiyangkeji.top

SQL ............ 90
来源：http://jkx.iojbl.cn

Bash ........... 80
来源：http://day.pycfn.com

Kotlin ......... 15
来源：http://xlg.hnxiangtu.top

Swift .......... 15
来源：http://rcs.316326.xyz

Lua ............ 10
来源：http://bpl.dashuyun.cn

Perl ........... 10
来源：http://dvv.gotoacloud.top


<!-- 参考信息 -->