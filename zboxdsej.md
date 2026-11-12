代发 wailian999

[T43] Perl：字符串插值
来源：http://sdy.guannengcc.top

"值: $a"
来源：http://azb.wangshuangyany.cn

[T44] Perl：条件
来源：http://bgn.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://hgm.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://eri.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://qgo.cdnleiting.top

[T46] Perl：哈希操作
来源：http://yyu.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rok.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://qcg.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://otq.meibo888.top

[T48] Perl：正则替换
来源：http://wip.andypj.xyz

$s =~ s/old/new/g;
来源：http://fey.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://vor.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lhi.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://iyf.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pzs.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://pod.jqgufenzy.top

[T51] Scala：Hello World
来源：http://jqr.jinyuanbaomall.cn

println("Hello")
来源：http://ddj.gzhubu.top

[T52] Scala：变量
来源：http://buh.kuanghao11.cn

val a = 1;  var b = 2
来源：http://lwd.ehwqpu.com

[T53] Scala：字符串插值
来源：http://mhm.xylfe.cn

s"值: $b"
来源：http://igf.yongpay.top

[T54] Scala：集合映射
来源：http://agl.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://yqk.fengsongda.top

[T55] Scala：集合过滤
来源：http://qvc.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fia.mhx1999.top

[T56] Scala：样例类
来源：http://kpc.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://vyn.wangdashe.top

[T57] Scala：模式匹配
来源：http://znr.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://upz.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://snl.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pie.fengsongda.top

[T59] Scala：循环
来源：http://bqh.mhx1999.top

for (i <- 1 to 10) println(i)
来源：http://gbn.zdqjudy.top

[T60] Scala：折叠
来源：http://ust.daria6918.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kzq.feifeiyinyue.top

================================================================================
来源：http://gvk.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://idz.iojbl.cn

================================================================================
来源：http://eix.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://xxu.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vpm.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://mka.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qkc.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://pzq.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vtr.ivvv.top

[U04] Py：变量调试打印
来源：http://krv.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aek.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://odm.hcnkem.com

list(dict.fromkeys(arr))
来源：http://sgh.svipenyu.cn

[U06] Py：合并两个字典
来源：http://gwl.316326.xyz

{**a, **b}
来源：http://pux.hysaishi.cn

[U07] Py：反转字典键值
来源：http://yrc.jianghu66.top

{v: k for k, v in d.items()}
来源：http://ysx.shzxlz.cn

[U08] Py：展平二维列表
来源：http://eze.tianlin.xyz

[y for x in nested for y in x]
来源：http://zyi.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://fat.sufxvd.cn

max(d, key=d.get)
来源：http://idu.ctjpmb.com

[U10] Py：按值排序字典
来源：http://ueu.cucudq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zdb.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://ffw.gzhubu.top

(x * 2 for x in arr)
来源：http://ltr.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://iws.yj202588.top

Counter(arr).most_common(3)
来源：http://lgt.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://pkz.cashguo.top

deque(maxlen=10)
来源：http://rgg.52xcode.cn

[U14] Py：分组收集到列表
来源：http://pzk.zhiwuduotai.top

defaultdict(list)
来源：http://jkq.jiagoushi.top

[U15] Py：高精度计时
来源：http://coa.cdnleiting.top

t = time.perf_counter()
来源：http://mbj.redwolf501.top

[U16] Py：命令行参数解析
来源：http://ylk.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lfg.hywenlv.cn

[U17] Py：初始化日志
来源：http://xwq.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://wxp.fengsongda.top

[U18] Py：预编译正则
来源：http://hxj.hammf.cn

pat = re.compile(r"\d+")
来源：http://yxp.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://fbi.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rke.cashguo.top

[U20] Py：缓存函数结果
来源：http://wog.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://ucx.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://rgv.zhengqikj.top

@contextlib.contextmanager
来源：http://xtd.xylfe.cn

[U22] Py：矩阵转置
来源：http://qcq.kuanghao11.cn

list(zip(*m))
来源：http://uxh.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://fyn.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://egf.ybcxt.top

[U24] Py：路径操作
来源：http://ukg.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kzk.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://rye.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://prt.daria6918.cn

[U26] Py：并发下载
来源：http://umq.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jzc.shuidangran.top

[U27] Py：异步 HTTP
来源：http://trk.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://jgu.hesvh.cn

[U28] Py：类型别名
来源：http://myx.zhijiandao.cn

UserId = int
来源：http://aob.sysykeji.top

[U29] Py：属性校验
来源：http://qhp.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://lul.quarkkingdee.top

[U30] Py：数据类
来源：http://hwb.haohaochexian.top

@dataclass(slots=True)
来源：http://qej.hfpthk.cn

[U31] Py：单测
来源：http://phq.yj20258888.top

python -m pytest -q
来源：http://fgm.sjlbkw.cn

[U32] Py：代码格式化
来源：http://nbn.ppjwa.cn

ruff format . && ruff check --fix .
来源：http://rpp.ctjpmb.com

[U33] Py：打包发布
来源：http://zeb.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://puj.bbcook.cn

[U34] Py：判断编码
来源：http://zaz.sysykeji.top

chardet.detect(raw)
来源：http://gwt.yonumen.top

[U35] Py：发送邮件
来源：http://ltb.ivvv.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yua.yj202588.top

[U36] Py：定时任务
来源：http://jfl.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://ajv.bbcook.cn

[U37] Py：读写 Excel
来源：http://ase.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://brs.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://ykh.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://zly.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://zpt.0kj1m.cn

sys.stdout.isatty()
来源：http://jvr.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://bll.hywenlv.cn

print("err", file=sys.stderr)
来源：http://hmq.xuanzx.com

[U41] PHP：初始化 Composer 项目
来源：http://owe.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://reu.hysaishi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ocw.hongshengwenyu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zqj.birdmap.top

[U43] PHP：声明命名空间
来源：http://nbn.jqgufenzy.top

namespace App\Http;
来源：http://tci.xinyue.icu

[U44] PHP：开启严格类型
来源：http://omy.c1oappe.top

declare(strict_types=1);
来源：http://vsd.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://pcq.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lnr.gzhubu.top

[U46] PHP：可空类型
来源：http://bcx.yueranfly.top

?string $name = null
来源：http://isk.jiagoushi.top

[U47] PHP：联合类型
来源：http://xsg.xinyue.icu

int|string $id
来源：http://gmx.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://yhc.shzxlz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gzl.xinyue.icu

[U49] PHP：只读属性
来源：http://qzb.bjfxy.top

public readonly string $name
来源：http://epv.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://qby.yuxming.cn

public function __construct(private int $id) {}
来源：http://chl.yvedp.cn

[U51] PHP：数组解构
来源：http://rjt.yfazqb.com

[$a, $b] = $arr;
来源：http://zqr.jinqigufen.top

[U52] PHP：箭头函数
来源：http://kqp.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://jga.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://jtw.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://wml.hnxiangtu.top

[U54] PHP：空安全调用
来源：http://aaa.bbcook.cn

$obj?->method()
来源：http://jrm.tanke756.top

[U55] PHP：match 表达式
来源：http://ddp.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zsk.hesvh.cn

[U56] PHP：命名参数
来源：http://qap.hcnkem.com

f(a: 1, b: 2)
来源：http://cyr.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://etb.andypj.xyz

"值: {$a}"
来源：http://tnj.yfazqb.com

[U58] PHP：数组三件套
来源：http://hbx.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zoc.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://yqj.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mig.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://enp.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vdh.guannengcc.top

[U61] PHP：正则
来源：http://dxd.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ryf.yangfankeji.com

[U62] PHP：日期对象
来源：http://brf.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wfs.yfazqb.com

[U63] PHP：文件读写
来源：http://ycr.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qjz.yongpay.top

[U64] PHP：目录遍历
来源：http://gus.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://mgg.fengsongda.top

[U65] PHP：会话
来源：http://etc.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://acr.tarul.cn

[U66] PHP：设置 Cookie
来源：http://oto.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vbq.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://tct.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qxo.nwbrower.top

[U68] PHP：PDO 连接
来源：http://smp.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qvy.aibaodan.cn

[U69] PHP：PDO 预处理
来源：http://ili.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ssu.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://mev.fzhhl.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ifp.xuanzx.com

[U71] PHP：抛出异常
来源：http://rrv.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://kkk.yuxming.cn

[U72] PHP：写错误日志
来源：http://sxx.hongshengwenyu.top

error_log("失败: " . $e->getMessage());
来源：http://rlo.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://phy.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://rgy.andypj.xyz

[U74] PHP：读取环境变量
来源：http://vfy.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://vtv.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://gav.jinyuanbaomall.cn

composer require psr/container
来源：http://xze.iojbl.cn

[U76] PHP：简单路由
来源：http://wbw.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nmo.birdmap.top

[U77] PHP：模板渲染
来源：http://apu.dianchejie.cn

composer require twig/twig
来源：http://cpc.vehdjk.com

[U78] PHP：单元测试
来源：http://dmc.havefunace.top

composer require --dev phpunit/phpunit
来源：http://bjr.tian-w.cn

[U79] PHP：静态分析
来源：http://dbf.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://ovz.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://igk.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fmb.fktsv.cn

[U81] JS：初始化项目
来源：http://xiz.yanxiufei.cn

npm init -y;  npm i express
来源：http://hsp.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://hil.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vnr.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://qvf.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://vze.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://pes.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://teh.jianghu66.top

[U85] JS：可选链
来源：http://yji.snrcjt.cn

a?.b?.c
来源：http://aox.yj20258888.top

[U86] JS：空值合并
来源：http://smb.ctjpmb.com

a ?? b
来源：http://mfv.fktsv.cn

[U87] JS：解构默认值
来源：http://hwp.xylfe.cn

const { a = 1, b = 2 } = obj;
来源：http://shf.wangdashe.top

[U88] JS：对象展开合并
来源：http://juy.quarkkingdee.top

{ ...a, ...b }
来源：http://kab.zhengqikj.top

[U89] JS：数组去重
来源：http://tut.mhx1999.top

[...new Set(arr)]
来源：http://hsd.svipenyu.cn

[U90] JS：数字数组排序
来源：http://cex.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://byh.guannengcc.top

[U91] JS：对象键值遍历
来源：http://djd.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ede.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://pjn.guowangkeji.top

structuredClone(obj)
来源：http://vgr.mhx1999.top

[U93] JS：模板字符串
来源：http://bbu.ppjwa.cn

`共 ${n} 条`
来源：http://zac.jyoumei.cn

[U94] JS：箭头函数
来源：http://ckq.jiagoushi.top

const double = x => x * 2;
来源：http://ldz.ybcxt.top

[U95] JS：Promise 包装
来源：http://cev.tarul.cn

new Promise((resolve, reject) => {})
来源：http://gfs.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://pww.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rym.guowangkeji.top

[U97] JS：并发请求
来源：http://ezh.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eoz.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://mlm.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lnm.hcnkem.com

[U99] JS：事件监听
来源：http://els.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://ehu.bbcook.cn

[U100] JS：DOM 查询
来源：http://jvz.52xcode.cn

document.querySelector(".item")
来源：http://doe.daria6918.cn

[U101] JS：classList 操作
来源：http://dxa.hesvh.cn

el.classList.toggle("active")
来源：http://hon.xuetiantiany.cn

[U102] JS：本地存储
来源：http://vcc.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jgg.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://rna.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://okm.ydzc1.top

[U104] JS：防抖
来源：http://gdg.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://diu.yfazqb.com

[U105] JS：节流
来源：http://ivg.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://udy.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://gbj.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nan.nwbrower.top

[U107] JS：数字千分位
来源：http://arp.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wud.jinghuilouyu.cn

[U108] JS：随机整数
来源：http://eoj.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rzi.shangyingyoupin.top

[U109] JS：数组分组
来源：http://qca.hywenlv.cn

Object.groupBy(arr, x => x.type)
来源：http://bba.meibo888.top

[U110] JS：数组分块
来源：http://bbo.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bxn.hfpthk.cn

[U111] JS：对象转 Map
来源：http://ioc.tanke756.top

new Map(Object.entries(obj))
来源：http://trc.sjlbkw.cn

[U112] JS：字符串补位
来源：http://arb.jyoumei.cn

"7".padStart(3, "0")
来源：http://rzv.xziqi.cn

[U113] JS：正则替换全部
来源：http://qsb.gotoacloud.top

s.replaceAll("a", "b")
来源：http://ohm.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://fnh.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://gzp.vehdjk.com

[U115] JS：生成 UUID
来源：http://rkt.aizwys.cn

crypto.randomUUID()
来源：http://rln.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://wca.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://cgx.epnwcf.com

[U117] JS：单元测试
来源：http://mbi.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://ate.smart0.xyz

[U118] JS：开发服务器
来源：http://osd.fengsongda.top

npm i -D vite;  npx vite
来源：http://waz.sufxvd.cn

[U119] JS：生产构建
来源：http://jqq.ctjpmb.com

npx vite build
来源：http://wnl.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://vpi.epnwcf.com

import.meta.env.VITE_API_URL
来源：http://ogf.zhongyouzk.top

================================================================================
来源：http://dsa.haohaochexian.top

统计汇总
来源：http://aec.xuanzx.com

================================================================================
来源：http://pjq.cqqwz.cn

按语言统计（条）：
来源：http://zcf.meibo888.top

Python ......... 252
来源：http://uyw.jinghuilouyu.cn

PHP ............ 252
来源：http://ciy.xuanzx.com

JavaScript ..... 252
来源：http://sbo.yongpay.top

TypeScript ..... 212
来源：http://hho.yvedp.cn

Java ........... 212
来源：http://ihl.yvedp.cn

Go ............. 212
来源：http://gbc.daxiang520.top

Ruby ........... 212
来源：http://vsz.xylfe.cn

C# ............. 212
来源：http://lcj.gzhubu.top

C .............. 30
来源：http://vjv.epnwcf.com

C++ ............ 30
来源：http://pun.svipenyu.cn

SQL ............ 90
来源：http://hvd.cashguo.top

Bash ........... 80
来源：http://qyt.wangdashe.top

Kotlin ......... 15
来源：http://jgm.yvedp.cn

Swift .......... 15
来源：http://ity.uphjek.com

Lua ............ 10
来源：http://uil.mhx1999.top

Perl ........... 10
来源：http://hsj.hcnkem.com


<!-- 参考信息 -->