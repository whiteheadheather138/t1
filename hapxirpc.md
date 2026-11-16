代发 wailian999

[T47] Perl：正则捕获
来源：http://xhm.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tlx.yj202588.top

[T48] Perl：正则替换
来源：http://bwn.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://wly.xylfe.cn

[T49] Perl：函数
来源：http://jkv.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xgk.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://efn.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://mfh.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://pim.jqgufenzy.top

[T51] Scala：Hello World
来源：http://bfw.sjlbkw.cn

println("Hello")
来源：http://vrq.sufxvd.cn

[T52] Scala：变量
来源：http://isw.zhijiandao.cn

val a = 1;  var b = 2
来源：http://fnw.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://yww.mhx1999.top

s"值: $b"
来源：http://kzr.hywenlv.cn

[T54] Scala：集合映射
来源：http://eui.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vae.chenlongwang.top

[T55] Scala：集合过滤
来源：http://txl.uphjek.com

List(1, 2, 3).filter(_ > 1)
来源：http://fdb.hcnkem.com

[T56] Scala：样例类
来源：http://pnv.52xcode.cn

case class User(name: String, age: Int)
来源：http://lkb.fktsv.cn

[T57] Scala：模式匹配
来源：http://yjb.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gnq.fengsongda.top

[T58] Scala：函数定义
来源：http://yfp.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://nbz.fehbvm.com

[T59] Scala：循环
来源：http://jmf.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://jir.meibo888.top

[T60] Scala：折叠
来源：http://vzr.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ysv.jinqigfzy.top

================================================================================
来源：http://ezz.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yhw.yuanzhike.top

================================================================================
来源：http://zjs.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://etw.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://qxi.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://qvl.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xtx.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://zro.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://whb.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://jii.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wco.wangdashe.top

[U05] Py：列表去重且保序
来源：http://tnq.iojbl.cn

list(dict.fromkeys(arr))
来源：http://mmb.ctjpmb.com

[U06] Py：合并两个字典
来源：http://vbd.yangfankeji.com

{**a, **b}
来源：http://jop.yuxming.cn

[U07] Py：反转字典键值
来源：http://gqo.nwbrower.top

{v: k for k, v in d.items()}
来源：http://lmx.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://jcn.zdqjudy.top

[y for x in nested for y in x]
来源：http://brm.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://sww.daria6918.cn

max(d, key=d.get)
来源：http://vzm.svipenyu.cn

[U10] Py：按值排序字典
来源：http://jqa.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ofa.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://ctl.guannengcc.top

(x * 2 for x in arr)
来源：http://bru.nwbrower.top

[U12] Py：取出现最多的 3 个元素
来源：http://hwy.0kj1m.cn

Counter(arr).most_common(3)
来源：http://leq.hesvh.cn

[U13] Py：固定长度队列
来源：http://lga.yanxiufei.cn

deque(maxlen=10)
来源：http://nrk.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://wyi.jiagoushi.top

defaultdict(list)
来源：http://ptq.xylfe.cn

[U15] Py：高精度计时
来源：http://ste.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://cmb.fengsongda.top

[U16] Py：命令行参数解析
来源：http://fpa.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rwp.yfazqb.com

[U17] Py：初始化日志
来源：http://sgu.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://ine.hcnkem.com

[U18] Py：预编译正则
来源：http://geu.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://ari.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://rci.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lba.andypj.xyz

[U20] Py：缓存函数结果
来源：http://oyj.yj20258888.top

@functools.lru_cache(maxsize=None)
来源：http://skc.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://neq.fengsongda.top

@contextlib.contextmanager
来源：http://giq.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://hfa.jqgufenzy.top

list(zip(*m))
来源：http://hed.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://tjs.wangdashe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jal.havefunace.top

[U24] Py：路径操作
来源：http://cac.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rsj.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://vuq.yfazqb.com

csv.DictReader(f)
来源：http://won.quarkkingdee.top

[U26] Py：并发下载
来源：http://xmy.xingfuxueyuan.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ieq.ivvv.top

[U27] Py：异步 HTTP
来源：http://xnk.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://jng.tanke756.top

[U28] Py：类型别名
来源：http://euj.kuanghao11.cn

UserId = int
来源：http://jpy.cqqwz.cn

[U29] Py：属性校验
来源：http://les.tarul.cn

@property 与 @x.setter 配合
来源：http://gqe.shzxlz.cn

[U30] Py：数据类
来源：http://pwb.xziqi.cn

@dataclass(slots=True)
来源：http://ycu.0kj1m.cn

[U31] Py：单测
来源：http://gfe.zdbjq.cn

python -m pytest -q
来源：http://smw.jqgufenzy.top

[U32] Py：代码格式化
来源：http://ibe.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://oda.nwbrower.top

[U33] Py：打包发布
来源：http://dkt.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://xjp.dianchejie.cn

[U34] Py：判断编码
来源：http://tcp.svipenyu.cn

chardet.detect(raw)
来源：http://hox.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://wnq.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmq.sysykeji.top

[U36] Py：定时任务
来源：http://kgu.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://rqg.andypj.xyz

[U37] Py：读写 Excel
来源：http://tqt.wangshuangyany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cxq.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://yut.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://xmz.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://nfm.zhongyouzk.top

sys.stdout.isatty()
来源：http://abe.fanxiaobao.xyz

[U40] Py：打印到标准错误
来源：http://kle.yj202588.top

print("err", file=sys.stderr)
来源：http://riu.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://lut.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://unx.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://pau.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bol.yuanzhike.top

[U43] PHP：声明命名空间
来源：http://ixa.zycfv.cn

namespace App\Http;
来源：http://ldg.bjfxy.top

[U44] PHP：开启严格类型
来源：http://yst.cashguo.top

declare(strict_types=1);
来源：http://ehe.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://bmm.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://juc.bbcook.cn

[U46] PHP：可空类型
来源：http://sfz.zhixingplan.top

?string $name = null
来源：http://qub.cashguo.top

[U47] PHP：联合类型
来源：http://fsh.jqgfzy.top

int|string $id
来源：http://upm.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://huh.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvc.yj20258.top

[U49] PHP：只读属性
来源：http://bjv.zhixingplan.top

public readonly string $name
来源：http://bay.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://vyy.wangdashe.top

public function __construct(private int $id) {}
来源：http://gov.yonumen.top

[U51] PHP：数组解构
来源：http://fif.xziqi.cn

[$a, $b] = $arr;
来源：http://gnz.yueranfly.top

[U52] PHP：箭头函数
来源：http://msv.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://lho.yonumen.top

[U53] PHP：空合并运算符
来源：http://kmb.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://ydg.cashguo.top

[U54] PHP：空安全调用
来源：http://eko.zdqjudy.top

$obj?->method()
来源：http://vcb.zhongyouzk.top

[U55] PHP：match 表达式
来源：http://ags.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://omi.quarkkingdee.top

[U56] PHP：命名参数
来源：http://meh.0kj1m.cn

f(a: 1, b: 2)
来源：http://ltu.cdnleiting.top

[U57] PHP：字符串插值
来源：http://hxp.chenzaomai.com

"值: {$a}"
来源：http://sha.havefunace.top

[U58] PHP：数组三件套
来源：http://qmo.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vnc.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://piv.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsr.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://cop.hammf.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fzz.jinqigufen.top

[U61] PHP：正则
来源：http://zyg.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qqp.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://nff.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jsz.yfazqb.com

[U63] PHP：文件读写
来源：http://ppm.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sow.yongpay.top

[U64] PHP：目录遍历
来源：http://bdb.hnxiangtu.top

glob("dir/*.php");  scandir("dir");
来源：http://oif.wangdashe.top

[U65] PHP：会话
来源：http://gns.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wbx.shanyushiyangkeji.top

[U66] PHP：设置 Cookie
来源：http://zcl.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mrr.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://mfl.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vqi.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://lgv.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uyz.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://xqa.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xvc.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://rfi.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://udx.aizwys.cn

[U71] PHP：抛出异常
来源：http://jhf.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://zuh.uphjek.com

[U72] PHP：写错误日志
来源：http://gfj.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://nzm.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://hsy.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://klh.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://pqw.yj20258888.top

getenv("APP_ENV") ?: "production"
来源：http://lzy.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://kdu.9152youxi.cn

composer require psr/container
来源：http://hpg.guowangkeji.top

[U76] PHP：简单路由
来源：http://ujx.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ghj.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://ncx.zycfv.cn

composer require twig/twig
来源：http://oqq.yj20258888.top

[U78] PHP：单元测试
来源：http://nbi.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://qhl.jianghu66.top

[U79] PHP：静态分析
来源：http://quu.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://jyq.redwolf501.top

[U80] PHP：代码规范修复
来源：http://lko.xziqi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tjj.uphjek.com

[U81] JS：初始化项目
来源：http://dvv.cdnleiting.top

npm init -y;  npm i express
来源：http://ffe.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://rma.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dzd.52xcode.cn

[U83] JS：ES Module 导入导出
来源：http://tfp.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://gjd.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://hkx.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ygz.meibo888.top

[U85] JS：可选链
来源：http://mqg.0kj1m.cn

a?.b?.c
来源：http://twi.sufxvd.cn

[U86] JS：空值合并
来源：http://yuc.ydjk.org.cn

a ?? b
来源：http://pyf.fzhhl.top

[U87] JS：解构默认值
来源：http://lce.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://zko.yvedp.cn

[U88] JS：对象展开合并
来源：http://wgr.fanxiaobao.xyz

{ ...a, ...b }
来源：http://kel.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://hly.smart0.xyz

[...new Set(arr)]
来源：http://oud.wangshuangyany.cn

[U90] JS：数字数组排序
来源：http://khb.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://epv.cashguo.top

[U91] JS：对象键值遍历
来源：http://wgi.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hax.fehbvm.com

[U92] JS：深拷贝
来源：http://cac.sweek.top

structuredClone(obj)
来源：http://zad.jianghu66.top

[U93] JS：模板字符串
来源：http://zxp.meibo888.top

`共 ${n} 条`
来源：http://uru.dianchejie.cn

[U94] JS：箭头函数
来源：http://txh.zdqjudy.top

const double = x => x * 2;
来源：http://zbo.wangdashe.top

[U95] JS：Promise 包装
来源：http://nwf.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://sji.bjfxy.top

[U96] JS：async/await 与异常
来源：http://dap.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://axb.zhixingplan.top

[U97] JS：并发请求
来源：http://nmh.jqgfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tcr.andypj.xyz

[U98] JS：fetch 带 JSON
来源：http://dtz.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xsr.yj202588.top

[U99] JS：事件监听
来源：http://gol.cucudq.cn

el.addEventListener("click", e => {})
来源：http://xni.havefunace.top

[U100] JS：DOM 查询
来源：http://ilr.yvedp.cn

document.querySelector(".item")
来源：http://cls.fehbvm.com

[U101] JS：classList 操作
来源：http://ucq.zycfv.cn

el.classList.toggle("active")
来源：http://zxl.yfazqb.com

[U102] JS：本地存储
来源：http://fsf.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ljg.yj202588.top

[U103] JS：定时器
来源：http://ekk.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bli.0kj1m.cn

[U104] JS：防抖
来源：http://qxr.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ygb.xingfuxueyuan.xyz

[U105] JS：节流
来源：http://ycy.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nve.52xcode.cn

[U106] JS：日期格式化
来源：http://hna.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ihz.sweek.top

[U107] JS：数字千分位
来源：http://cej.zdbjq.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://scy.zhoulong.xyz

[U108] JS：随机整数
来源：http://iob.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wfw.xziqi.cn

[U109] JS：数组分组
来源：http://ycx.jiagoushi.top

Object.groupBy(arr, x => x.type)
来源：http://atb.sjlbkw.cn

[U110] JS：数组分块
来源：http://ovw.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xgd.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://zlm.jinyuanbaomall.cn

new Map(Object.entries(obj))
来源：http://oqj.hcnkem.com

[U112] JS：字符串补位
来源：http://gle.snrcjt.cn

"7".padStart(3, "0")
来源：http://fjf.0kj1m.cn

[U113] JS：正则替换全部
来源：http://fkf.birdmap.top

s.replaceAll("a", "b")
来源：http://ryx.mhx1999.top

[U114] JS：JSON 深比较
来源：http://iam.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uhf.yueranfly.top

[U115] JS：生成 UUID
来源：http://zvg.chenlongwang.top

crypto.randomUUID()
来源：http://zbw.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://zxu.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://fdg.sufxvd.cn

[U117] JS：单元测试
来源：http://zzs.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://beo.sysykeji.top

[U118] JS：开发服务器
来源：http://fzu.hongshengwenyu.top

npm i -D vite;  npx vite
来源：http://hez.redwolf501.top

[U119] JS：生产构建
来源：http://jqe.xingfuxueyuan.xyz

npx vite build
来源：http://pax.shuidangran.top

[U120] JS：读取环境变量（Vite）
来源：http://hyu.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://mpc.pengpengdd.cyou

================================================================================
来源：http://dir.smart0.xyz

统计汇总
来源：http://sjg.fanxiaobao.xyz

================================================================================
来源：http://iki.hongshengwenyu.top

按语言统计（条）：
来源：http://zhy.yuxming.cn

Python ......... 252
来源：http://wyy.sjlbkw.cn

PHP ............ 252
来源：http://rrj.yuanzhike.top

JavaScript ..... 252
来源：http://fvn.guowangkeji.top

TypeScript ..... 212
来源：http://zuy.shanyushiyangtech.top

Java ........... 212
来源：http://esj.xingfuxueyuan.xyz

Go ............. 212
来源：http://qbc.bjfxy.top

Ruby ........... 212
来源：http://zuj.ehwqpu.com

C# ............. 212
来源：http://sik.yueranfly.top

C .............. 30
来源：http://xqx.jinqigfzy.top

C++ ............ 30
来源：http://ins.jinyuanbaomall.cn

SQL ............ 90
来源：http://edr.zhixingplan.top

Bash ........... 80
来源：http://osh.nwbrower.top

Kotlin ......... 15
来源：http://jqn.nwbrower.top

Swift .......... 15
来源：http://ttj.yvedp.cn

Lua ............ 10
来源：http://jqr.jinyuanbaomall.cn

Perl ........... 10
来源：http://bzl.ywan-chungtsiang.top

Scala .......... 10
来源：http://ddv.fehbvm.com

------------------------------------
来源：http://zjo.hysaishi.cn

合计 ........... 2106 条
来源：http://rjn.sjlbkw.cn

按章节统计：
来源：http://lrk.hongshengwenyu.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://exf.yj202588.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://caz.hesvh.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://udl.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bej.fanxiaobao.xyz


<!-- 参考信息 -->