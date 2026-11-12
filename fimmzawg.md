代发 wailian999

[T49] Perl：函数
来源：http://dls.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://itd.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://mhp.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xnk.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://ybw.yj202588.top

[T51] Scala：Hello World
来源：http://lcd.zhijiandao.cn

println("Hello")
来源：http://wvw.snrcjt.cn

[T52] Scala：变量
来源：http://rlh.hnqzz.top

val a = 1;  var b = 2
来源：http://een.uphjek.com

[T53] Scala：字符串插值
来源：http://ruz.jianghu66.top

s"值: $b"
来源：http://ldd.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://arv.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://pbc.guannengcc.top

[T55] Scala：集合过滤
来源：http://pju.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://btv.ppjwa.cn

[T56] Scala：样例类
来源：http://ucr.jinqigfzy.top

case class User(name: String, age: Int)
来源：http://grk.snrcjt.cn

[T57] Scala：模式匹配
来源：http://cve.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nkl.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://zou.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://qwd.yj20258888.top

[T59] Scala：循环
来源：http://jgm.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://xfe.yj20258888.top

[T60] Scala：折叠
来源：http://kya.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aef.zhixingplan.top

================================================================================
来源：http://rml.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rme.bbcook.cn

================================================================================
来源：http://fbz.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://grt.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://bvh.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://cor.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mqq.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://lsy.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qfr.gotoacloud.top

[U04] Py：变量调试打印
来源：http://frt.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqm.52xcode.cn

[U05] Py：列表去重且保序
来源：http://hpg.yfazqb.com

list(dict.fromkeys(arr))
来源：http://ypz.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://rbb.hongshengwenyu.top

{**a, **b}
来源：http://moc.yfazqb.com

[U07] Py：反转字典键值
来源：http://ijf.fengsongda.top

{v: k for k, v in d.items()}
来源：http://nmy.cheryme.top

[U08] Py：展平二维列表
来源：http://qql.daxiang520.top

[y for x in nested for y in x]
来源：http://man.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://mdj.cheryme.top

max(d, key=d.get)
来源：http://cgq.cheryme.top

[U10] Py：按值排序字典
来源：http://aip.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ehd.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://amg.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://hro.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://rjz.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://boa.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://rjv.xuanzx.com

deque(maxlen=10)
来源：http://hic.hesvh.cn

[U14] Py：分组收集到列表
来源：http://hpa.yongpay.top

defaultdict(list)
来源：http://vgr.ydzc1.top

[U15] Py：高精度计时
来源：http://unt.ydjk.org.cn

t = time.perf_counter()
来源：http://kcl.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://ejc.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://abo.tianlin.xyz

[U17] Py：初始化日志
来源：http://bee.tarul.cn

logging.basicConfig(level=logging.INFO)
来源：http://whw.tanke756.top

[U18] Py：预编译正则
来源：http://gvt.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://lnw.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://orc.cheryme.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nwp.nwbrower.top

[U20] Py：缓存函数结果
来源：http://rga.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://eib.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://ytp.birdmap.top

@contextlib.contextmanager
来源：http://gvo.ivvv.top

[U22] Py：矩阵转置
来源：http://tji.tian-w.cn

list(zip(*m))
来源：http://owl.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://cgd.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ybh.pengpengdd.cyou

[U24] Py：路径操作
来源：http://jej.yuanzhike.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pzv.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://rtn.shuidangran.top

csv.DictReader(f)
来源：http://wls.sysykeji.top

[U26] Py：并发下载
来源：http://sow.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zwq.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://blp.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://tra.c1oappe.top

[U28] Py：类型别名
来源：http://nuo.hywenlv.cn

UserId = int
来源：http://vie.cucudq.cn

[U29] Py：属性校验
来源：http://jwv.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://urs.tianlin.xyz

[U30] Py：数据类
来源：http://omw.daxiang520.top

@dataclass(slots=True)
来源：http://wwe.hfpthk.cn

[U31] Py：单测
来源：http://msj.yueranfly.top

python -m pytest -q
来源：http://kto.yueranfly.top

[U32] Py：代码格式化
来源：http://fbm.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://vip.aizwys.cn

[U33] Py：打包发布
来源：http://wgv.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://sbq.hcnkem.com

[U34] Py：判断编码
来源：http://mts.hywenlv.cn

chardet.detect(raw)
来源：http://vnu.iojbl.cn

[U35] Py：发送邮件
来源：http://wgs.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://svz.cheryme.top

[U36] Py：定时任务
来源：http://ahs.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://qvi.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://jhn.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ogy.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://nwc.yj202588.top

Path(__file__).resolve().parent
来源：http://cuz.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://wqm.fehbvm.com

sys.stdout.isatty()
来源：http://kir.daxiang520.top

[U40] Py：打印到标准错误
来源：http://lab.tian-w.cn

print("err", file=sys.stderr)
来源：http://jib.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ywc.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://rej.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://wxo.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gys.hammf.cn

[U43] PHP：声明命名空间
来源：http://pme.ywan-chungtsiang.top

namespace App\Http;
来源：http://ddn.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://yjl.shuidangran.top

declare(strict_types=1);
来源：http://kvk.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://pem.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yzc.yuxming.cn

[U46] PHP：可空类型
来源：http://oit.sweek.top

?string $name = null
来源：http://eol.yj20258.top

[U47] PHP：联合类型
来源：http://ksg.yj20258.top

int|string $id
来源：http://tiz.zycfv.cn

[U48] PHP：纯枚举
来源：http://kxb.jinghuilouyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bjl.jinqigfzy.top

[U49] PHP：只读属性
来源：http://vbz.wangdashe.top

public readonly string $name
来源：http://qnk.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://rtz.xziqi.cn

public function __construct(private int $id) {}
来源：http://ffq.gzhubu.top

[U51] PHP：数组解构
来源：http://srw.tanke756.top

[$a, $b] = $arr;
来源：http://lst.yueranfly.top

[U52] PHP：箭头函数
来源：http://ybx.nwbrower.top

$double = fn($x) => $x * 2;
来源：http://npa.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://wln.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://zcp.nwbrower.top

[U54] PHP：空安全调用
来源：http://dwy.zhengqikj.top

$obj?->method()
来源：http://ujk.yj20258.top

[U55] PHP：match 表达式
来源：http://lnd.hysaishi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dyy.ydzc1.top

[U56] PHP：命名参数
来源：http://ncs.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://omj.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://acz.sxryk.cn

"值: {$a}"
来源：http://mjm.dashuyun.cn

[U58] PHP：数组三件套
来源：http://mmz.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qxz.fengsongda.top

[U59] PHP：自定义排序
来源：http://vsg.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kyg.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://ilj.mhx1999.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jqa.nanxuanxn.top

[U61] PHP：正则
来源：http://ava.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cwu.0kj1m.cn

[U62] PHP：日期对象
来源：http://dku.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vhm.wangdashe.top

[U63] PHP：文件读写
来源：http://wyi.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jfn.tanke756.top

[U64] PHP：目录遍历
来源：http://exr.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://ofb.ydzc1.top

[U65] PHP：会话
来源：http://win.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pzp.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://npe.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bbe.daria6918.cn

[U67] PHP：处理文件上传
来源：http://uac.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cep.c1oappe.top

[U68] PHP：PDO 连接
来源：http://kxi.chenjidiqi.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uwd.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://sge.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vah.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://ceq.hcnkem.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bdq.zhengqikj.top

[U71] PHP：抛出异常
来源：http://jkl.sweek.top

throw new RuntimeException("失败", 500);
来源：http://pyq.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://nev.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://cxg.shzxlz.cn

[U73] PHP：读取 ini 配置
来源：http://btv.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://xtc.ctjpmb.com

[U74] PHP：读取环境变量
来源：http://ypu.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://kik.nanxinkj.top

[U75] PHP：依赖注入
来源：http://fhd.wangshuangyany.cn

composer require psr/container
来源：http://ucy.xziqi.cn

[U76] PHP：简单路由
来源：http://rez.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yas.fktsv.cn

[U77] PHP：模板渲染
来源：http://agl.zhixingplan.top

composer require twig/twig
来源：http://vhb.jqgufenzy.top

[U78] PHP：单元测试
来源：http://hel.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://utg.0kj1m.cn

[U79] PHP：静态分析
来源：http://xke.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://fmu.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://cpr.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qtg.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://qcs.chenzaomai.com

npm init -y;  npm i express
来源：http://ogn.yuxming.cn

[U82] JS：package.json 脚本
来源：http://grg.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oxt.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://cye.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://wue.bjfxy.top

[U84] JS：CommonJS 写法
来源：http://aqd.nanxinkj.top

module.exports = { a };  const { a } = require("./m");
来源：http://tan.dianchejie.cn

[U85] JS：可选链
来源：http://pgk.fengsongda.top

a?.b?.c
来源：http://yfs.havefunace.top

[U86] JS：空值合并
来源：http://kws.meibo888.top

a ?? b
来源：http://yxz.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://hyc.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://gwi.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://ruv.ydjk.org.cn

{ ...a, ...b }
来源：http://odo.tanke756.top

[U89] JS：数组去重
来源：http://yxx.nanxuanxn.top

[...new Set(arr)]
来源：http://rbg.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://ugj.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://lzi.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://fhp.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mnd.quarkkingdee.top

[U92] JS：深拷贝
来源：http://neu.fktsv.cn

structuredClone(obj)
来源：http://xhh.haohaochexian.top

[U93] JS：模板字符串
来源：http://uut.jqgfzy.top

`共 ${n} 条`
来源：http://fxy.guannengcc.top

[U94] JS：箭头函数
来源：http://exw.havefunace.top

const double = x => x * 2;
来源：http://ezp.fanxiaobao.xyz

[U95] JS：Promise 包装
来源：http://cls.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://gux.cashguo.top

[U96] JS：async/await 与异常
来源：http://jux.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xjf.feifeiyinyue.top

[U97] JS：并发请求
来源：http://zrm.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pdv.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://iqz.jqgfzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eoz.sysykeji.top

[U99] JS：事件监听
来源：http://tml.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://zcb.uphjek.com

[U100] JS：DOM 查询
来源：http://rwa.andypj.xyz

document.querySelector(".item")
来源：http://oxs.xinyue.icu

[U101] JS：classList 操作
来源：http://ikm.jqgufenzy.top

el.classList.toggle("active")
来源：http://ywi.zhijiandao.cn

[U102] JS：本地存储
来源：http://ioe.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ezr.ydjk.org.cn

[U103] JS：定时器
来源：http://cuf.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ykp.cucudq.cn

[U104] JS：防抖
来源：http://mbi.sjlbkw.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ows.zhoulong.xyz

[U105] JS：节流
来源：http://ddu.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lxf.dashuyun.cn

[U106] JS：日期格式化
来源：http://jtb.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fkc.nanxuanxn.top

[U107] JS：数字千分位
来源：http://rzw.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lly.ydjk.org.cn

[U108] JS：随机整数
来源：http://xxs.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mye.cqqwz.cn

[U109] JS：数组分组
来源：http://wkz.jinghuilouyu.cn

Object.groupBy(arr, x => x.type)
来源：http://uyg.dianchejie.cn

[U110] JS：数组分块
来源：http://crg.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tgx.nanxuanxn.top

[U111] JS：对象转 Map
来源：http://fhg.smart0.xyz

new Map(Object.entries(obj))
来源：http://umb.52xcode.cn

[U112] JS：字符串补位
来源：http://hdt.hongshengwenyu.top

"7".padStart(3, "0")
来源：http://dba.chenlongwang.top

[U113] JS：正则替换全部
来源：http://wau.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://rny.sysykeji.top

[U114] JS：JSON 深比较
来源：http://oxt.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kwr.snrcjt.cn

[U115] JS：生成 UUID
来源：http://xer.gotoacloud.top

crypto.randomUUID()
来源：http://zvi.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://bci.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://otf.zhixingplan.top

[U117] JS：单元测试
来源：http://yup.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://szs.jlsjyb.cn

[U118] JS：开发服务器
来源：http://rpc.tarul.cn

npm i -D vite;  npx vite
来源：http://vpj.cdnleiting.top

[U119] JS：生产构建
来源：http://bly.gogol.net.cn

npx vite build
来源：http://act.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://frk.jinqigufen.top

import.meta.env.VITE_API_URL
来源：http://slc.chenzaomai.com

================================================================================
来源：http://esz.cdnleiting.top

统计汇总
来源：http://klb.hcnkem.com

================================================================================
来源：http://jtq.jinyuanbaomall.cn

按语言统计（条）：
来源：http://awm.shangyingyoupin.top

Python ......... 252
来源：http://amr.havefunace.top

PHP ............ 252
来源：http://vgs.yj20258888.top

JavaScript ..... 252
来源：http://etd.ivvv.top

TypeScript ..... 212
来源：http://lke.birdmap.top

Java ........... 212
来源：http://vpe.snrcjt.cn

Go ............. 212
来源：http://mub.yangfankeji.com

Ruby ........... 212
来源：http://euu.fengsongda.top

C# ............. 212
来源：http://vxd.hcnkem.com

C .............. 30
来源：http://uvc.ydzc1.top

C++ ............ 30
来源：http://ugo.jlsjyb.cn

SQL ............ 90
来源：http://nql.hysaishi.cn

Bash ........... 80
来源：http://lwt.9152youxi.cn

Kotlin ......... 15
来源：http://uec.nanxinkj.top

Swift .......... 15
来源：http://zeh.jiagoushi.top

Lua ............ 10
来源：http://pkg.jlsjyb.cn

Perl ........... 10
来源：http://dwo.meibo888.top

Scala .......... 10
来源：http://qwb.sufxvd.cn

------------------------------------
来源：http://gku.meibo888.top

合计 ........... 2106 条
来源：http://pdo.guannengcc.top

按章节统计：
来源：http://jtk.cheryme.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://inu.nanxuanxn.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sff.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xja.hammf.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://unc.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ajz.yongpay.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://srp.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tfj.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gci.ivvv.top


<!-- 参考信息 -->