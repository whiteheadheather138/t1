代发 wailian999

[T45] Perl：数组遍历
来源：http://mlb.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://abl.hesvh.cn

[T46] Perl：哈希操作
来源：http://fqe.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pyk.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://llt.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibr.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://ezd.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://yzc.haohaochexian.top

[T49] Perl：函数
来源：http://yto.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jsn.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://dah.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fxw.zhoulong.xyz

while (my $line = <$fh>) { print $line; }
来源：http://bvy.daxiang520.top

[T51] Scala：Hello World
来源：http://ovz.shzxlz.cn

println("Hello")
来源：http://fpg.tarul.cn

[T52] Scala：变量
来源：http://okw.tarul.cn

val a = 1;  var b = 2
来源：http://iwl.jqgfzy.top

[T53] Scala：字符串插值
来源：http://ett.quarkkingdee.top

s"值: $b"
来源：http://nyx.zdbjq.cn

[T54] Scala：集合映射
来源：http://eno.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://luq.jqgfzy.top

[T55] Scala：集合过滤
来源：http://dug.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wyn.ydjk.org.cn

[T56] Scala：样例类
来源：http://xjq.fzhhl.top

case class User(name: String, age: Int)
来源：http://qpl.mhx1999.top

[T57] Scala：模式匹配
来源：http://pib.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ndc.9152youxi.cn

[T58] Scala：函数定义
来源：http://efl.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://arp.cqqwz.cn

[T59] Scala：循环
来源：http://kkq.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://ttq.cheryme.top

[T60] Scala：折叠
来源：http://kci.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ikt.zhaomingkeji.xyz

================================================================================
来源：http://frv.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xsm.yuxming.cn

================================================================================
来源：http://nuf.havefunace.top

[U01] Py：创建虚拟环境
来源：http://ufy.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://cjv.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://iqg.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://slg.quarkkingdee.top

[U03] Py：加载 .env 配置
来源：http://rdu.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://hni.nwbrower.top

[U04] Py：变量调试打印
来源：http://etq.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ksa.sweek.top

[U05] Py：列表去重且保序
来源：http://rio.yfazqb.com

list(dict.fromkeys(arr))
来源：http://mdi.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://ydh.guowangkeji.top

{**a, **b}
来源：http://xtv.jqgfzy.top

[U07] Py：反转字典键值
来源：http://fdg.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://lrs.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://nsi.daria6918.cn

[y for x in nested for y in x]
来源：http://fdy.daria6918.cn

[U09] Py：字典取最大值的键
来源：http://oxp.daria6918.cn

max(d, key=d.get)
来源：http://bwi.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://hzn.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rwf.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://eed.jqgufenzy.top

(x * 2 for x in arr)
来源：http://bsj.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://vsn.zycfv.cn

Counter(arr).most_common(3)
来源：http://fsd.jianghu66.top

[U13] Py：固定长度队列
来源：http://sie.yuxming.cn

deque(maxlen=10)
来源：http://jly.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://abd.ivvv.top

defaultdict(list)
来源：http://npb.chenzaomai.com

[U15] Py：高精度计时
来源：http://xfx.yangfankeji.com

t = time.perf_counter()
来源：http://fis.ivvv.top

[U16] Py：命令行参数解析
来源：http://azu.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cio.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://dtw.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://hgi.tian-w.cn

[U18] Py：预编译正则
来源：http://dtg.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://uru.wangdashe.top

[U19] Py：正则替换带回调
来源：http://iqp.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://trm.epnwcf.com

[U20] Py：缓存函数结果
来源：http://umu.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://wbl.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://uvy.snrcjt.cn

@contextlib.contextmanager
来源：http://dun.ivvv.top

[U22] Py：矩阵转置
来源：http://prm.havefunace.top

list(zip(*m))
来源：http://bhe.aizwys.cn

[U23] Py：分块读取大文件
来源：http://fvg.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://azl.jiagoushi.top

[U24] Py：路径操作
来源：http://epe.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bhk.ivvv.top

[U25] Py：CSV 按字典读
来源：http://ivp.chenjidiqi.icu

csv.DictReader(f)
来源：http://pml.dashuyun.cn

[U26] Py：并发下载
来源：http://pzu.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kyk.yueranfly.top

[U27] Py：异步 HTTP
来源：http://buf.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://okr.zdqjudy.top

[U28] Py：类型别名
来源：http://zyu.ppjwa.cn

UserId = int
来源：http://ren.hnxiangtu.top

[U29] Py：属性校验
来源：http://cqe.meibo888.top

@property 与 @x.setter 配合
来源：http://oxk.fengsongda.top

[U30] Py：数据类
来源：http://xnb.xinyue.icu

@dataclass(slots=True)
来源：http://dia.sxryk.cn

[U31] Py：单测
来源：http://trx.yonumen.top

python -m pytest -q
来源：http://tru.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://xif.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://cfl.hnqzz.top

[U33] Py：打包发布
来源：http://fnu.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://muz.c1oappe.top

[U34] Py：判断编码
来源：http://rov.bbcook.cn

chardet.detect(raw)
来源：http://jsx.guowangkeji.top

[U35] Py：发送邮件
来源：http://vyo.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pjs.ydzc1.top

[U36] Py：定时任务
来源：http://grs.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://afu.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://yph.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://znw.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://zel.birdmap.top

Path(__file__).resolve().parent
来源：http://uof.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://fmu.shuidangran.top

sys.stdout.isatty()
来源：http://kdu.hywenlv.cn

[U40] Py：打印到标准错误
来源：http://ryb.haohaochexian.top

print("err", file=sys.stderr)
来源：http://xeo.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://kyq.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://opa.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://ura.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ubf.bjfxy.top

[U43] PHP：声明命名空间
来源：http://onc.sweek.top

namespace App\Http;
来源：http://dto.jianghu66.top

[U44] PHP：开启严格类型
来源：http://owt.daxiang520.top

declare(strict_types=1);
来源：http://gss.fanxiaobao.xyz

[U45] PHP：类型声明与返回类型
来源：http://yqy.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kmq.yueranfly.top

[U46] PHP：可空类型
来源：http://phf.52xcode.cn

?string $name = null
来源：http://ikg.ppjwa.cn

[U47] PHP：联合类型
来源：http://ntj.uphjek.com

int|string $id
来源：http://otz.xuanzx.com

[U48] PHP：纯枚举
来源：http://rsj.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qxx.yj20258888.top

[U49] PHP：只读属性
来源：http://ruz.gzhubu.top

public readonly string $name
来源：http://jcg.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://oyf.cucudq.cn

public function __construct(private int $id) {}
来源：http://sml.hnqzz.top

[U51] PHP：数组解构
来源：http://axi.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://nai.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://fim.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://bup.ydzc1.top

[U53] PHP：空合并运算符
来源：http://gqb.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://ule.ivvv.top

[U54] PHP：空安全调用
来源：http://gur.xuetiantiany.cn

$obj?->method()
来源：http://gkc.316326.xyz

[U55] PHP：match 表达式
来源：http://vgy.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fwv.guannengcc.top

[U56] PHP：命名参数
来源：http://srh.hammf.cn

f(a: 1, b: 2)
来源：http://eqi.jinqigufen.top

[U57] PHP：字符串插值
来源：http://rul.gzhubu.top

"值: {$a}"
来源：http://eti.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://xyc.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://puu.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://bfe.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujc.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://xtu.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gut.ppjwa.cn

[U61] PHP：正则
来源：http://gai.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wka.zhongyouzk.top

[U62] PHP：日期对象
来源：http://awj.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xez.xuanzx.com

[U63] PHP：文件读写
来源：http://eir.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://byb.hfpthk.cn

[U64] PHP：目录遍历
来源：http://hbj.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://bzl.zhijiandao.cn

[U65] PHP：会话
来源：http://uot.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://odx.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://sew.daria6918.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://clp.uphjek.com

[U67] PHP：处理文件上传
来源：http://jsm.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zyx.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://gxk.hywenlv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yfu.daxiang520.top

[U69] PHP：PDO 预处理
来源：http://bpt.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://izy.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://rrp.jianghu66.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vqg.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://ecv.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://hyf.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://skg.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://ung.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://efu.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://aoq.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://rim.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://lnm.wangdashe.top

[U75] PHP：依赖注入
来源：http://pmj.sufxvd.cn

composer require psr/container
来源：http://sfa.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://vaf.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vex.iojbl.cn

[U77] PHP：模板渲染
来源：http://mqt.tian-w.cn

composer require twig/twig
来源：http://ske.epnwcf.com

[U78] PHP：单元测试
来源：http://hdd.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://qjl.ydzc1.top

[U79] PHP：静态分析
来源：http://hfd.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://tjx.havefunace.top

[U80] PHP：代码规范修复
来源：http://vyj.hesvh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hgd.xziqi.cn

[U81] JS：初始化项目
来源：http://lxo.epnwcf.com

npm init -y;  npm i express
来源：http://shp.jianghu66.top

[U82] JS：package.json 脚本
来源：http://ccs.havefunace.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nnt.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://cff.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xiz.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://hxz.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://dyx.mhx1999.top

[U85] JS：可选链
来源：http://oso.ybcxt.top

a?.b?.c
来源：http://sjv.uphjek.com

[U86] JS：空值合并
来源：http://buo.kuanghao11.cn

a ?? b
来源：http://txo.xinyue.icu

[U87] JS：解构默认值
来源：http://ssi.tianlin.xyz

const { a = 1, b = 2 } = obj;
来源：http://ofz.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://vkp.zhoulong.xyz

{ ...a, ...b }
来源：http://elr.pengpengdd.cyou

[U89] JS：数组去重
来源：http://dnr.hcnkem.com

[...new Set(arr)]
来源：http://ayj.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://jvp.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://gjj.cheryme.top

[U91] JS：对象键值遍历
来源：http://xwx.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://odx.jinqigfzy.top

[U92] JS：深拷贝
来源：http://bod.svipenyu.cn

structuredClone(obj)
来源：http://ubx.cheryme.top

[U93] JS：模板字符串
来源：http://ftp.xuanzx.com

`共 ${n} 条`
来源：http://dnl.meibo888.top

[U94] JS：箭头函数
来源：http://pem.jinyuanbaomall.cn

const double = x => x * 2;
来源：http://brs.bbcook.cn

[U95] JS：Promise 包装
来源：http://fgd.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://ftu.tanke756.top

[U96] JS：async/await 与异常
来源：http://geu.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nlw.ybcxt.top

[U97] JS：并发请求
来源：http://upc.shanyushiyangtech.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://clm.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://eie.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hla.sufxvd.cn

[U99] JS：事件监听
来源：http://qjn.hnxiangtu.top

el.addEventListener("click", e => {})
来源：http://mrz.redwolf501.top

[U100] JS：DOM 查询
来源：http://kpn.zdqjudy.top

document.querySelector(".item")
来源：http://kfd.feifeiyinyue.top

[U101] JS：classList 操作
来源：http://uhp.yj202588.top

el.classList.toggle("active")
来源：http://amn.shuidangran.top

[U102] JS：本地存储
来源：http://uiy.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hcm.sufxvd.cn

[U103] JS：定时器
来源：http://sph.feifeiyinyue.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blc.yongpay.top

[U104] JS：防抖
来源：http://qck.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zna.birdmap.top

[U105] JS：节流
来源：http://gzp.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mrj.bjfxy.top

[U106] JS：日期格式化
来源：http://zbd.sufxvd.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://equ.hysaishi.cn

[U107] JS：数字千分位
来源：http://xcn.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gek.yvedp.cn

[U108] JS：随机整数
来源：http://zce.yanxiufei.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kwz.hywenlv.cn

[U109] JS：数组分组
来源：http://evh.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://tyf.ppjwa.cn

[U110] JS：数组分块
来源：http://dul.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jcr.yuanzhike.top

[U111] JS：对象转 Map
来源：http://cuh.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://mzy.yuanzhike.top

[U112] JS：字符串补位
来源：http://anc.c1oappe.top

"7".padStart(3, "0")
来源：http://esn.hfpthk.cn

[U113] JS：正则替换全部
来源：http://rfk.xuanzx.com

s.replaceAll("a", "b")
来源：http://jdh.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://swv.yuanzhike.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yfc.dianchejie.cn

[U115] JS：生成 UUID
来源：http://bny.hnxiangtu.top

crypto.randomUUID()
来源：http://rah.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://utf.cdnleiting.top

/** @param {string} name */ function f(name) {}
来源：http://pgw.aibaodan.cn

[U117] JS：单元测试
来源：http://fel.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://snu.aibaodan.cn

[U118] JS：开发服务器
来源：http://kdw.redwolf501.top

npm i -D vite;  npx vite
来源：http://ysv.sweek.top

[U119] JS：生产构建
来源：http://xvp.sysykeji.top

npx vite build
来源：http://ify.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://jrc.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://wxz.hywenlv.cn

================================================================================
来源：http://nzd.iojbl.cn

统计汇总
来源：http://otq.xinyue.icu

================================================================================
来源：http://xei.fehbvm.com

按语言统计（条）：
来源：http://ncv.316326.xyz

Python ......... 252
来源：http://grr.pycfn.com

PHP ............ 252
来源：http://kcw.yonumen.top

JavaScript ..... 252
来源：http://usi.gogol.net.cn

TypeScript ..... 212
来源：http://btd.ivvv.top

Java ........... 212
来源：http://qlw.xuanzx.com

Go ............. 212
来源：http://kar.jqgfzy.top

Ruby ........... 212
来源：http://ice.yuxming.cn

C# ............. 212
来源：http://moa.nanxuanxn.top

C .............. 30
来源：http://kpd.gogol.net.cn

C++ ............ 30
来源：http://xnl.fzhhl.top

SQL ............ 90
来源：http://qjh.haohaochexian.top

Bash ........... 80
来源：http://vqm.jqgfzy.top

Kotlin ......... 15
来源：http://zcq.ybcxt.top

Swift .......... 15
来源：http://pzg.dashuyun.cn

Lua ............ 10
来源：http://bza.daxiang520.top

Perl ........... 10
来源：http://ldl.yj20258888.top

Scala .......... 10
来源：http://xdv.fktsv.cn

------------------------------------
来源：http://qgl.iojbl.cn

合计 ........... 2106 条
来源：http://ivy.sxryk.cn

按章节统计：
来源：http://nhi.shanyushiyangkeji.top


<!-- 参考信息 -->