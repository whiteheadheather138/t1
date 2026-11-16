代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://uts.fktsv.cn

[T51] Scala：Hello World
来源：http://bpx.shangyingyoupin.top

println("Hello")
来源：http://vym.yvedp.cn

[T52] Scala：变量
来源：http://ywr.yonumen.top

val a = 1;  var b = 2
来源：http://gal.sufxvd.cn

[T53] Scala：字符串插值
来源：http://xiq.hesvh.cn

s"值: $b"
来源：http://bqi.chenzaomai.com

[T54] Scala：集合映射
来源：http://hrb.xinyue.icu

List(1, 2, 3).map(_ * 2)
来源：http://agi.yueranfly.top

[T55] Scala：集合过滤
来源：http://twd.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://xev.wangdashe.top

[T56] Scala：样例类
来源：http://nfs.mhx1999.top

case class User(name: String, age: Int)
来源：http://hgz.ivvv.top

[T57] Scala：模式匹配
来源：http://eov.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jdr.wangdashe.top

[T58] Scala：函数定义
来源：http://pbs.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://vco.jinqigfzy.top

[T59] Scala：循环
来源：http://kjw.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://duk.birdmap.top

[T60] Scala：折叠
来源：http://hmj.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zlg.fanxiaobao.xyz

================================================================================
来源：http://pzw.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lcq.jinqigfzy.top

================================================================================
来源：http://azr.birdmap.top

[U01] Py：创建虚拟环境
来源：http://uqu.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://vkh.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://apb.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vrd.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://sxa.ppjwa.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ape.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://qac.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zcs.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://pwo.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://ofk.zdbjq.cn

[U06] Py：合并两个字典
来源：http://btm.aizwys.cn

{**a, **b}
来源：http://wgb.xuanzx.com

[U07] Py：反转字典键值
来源：http://fby.havefunace.top

{v: k for k, v in d.items()}
来源：http://hxl.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://thm.snrcjt.cn

[y for x in nested for y in x]
来源：http://ibn.gzhubu.top

[U09] Py：字典取最大值的键
来源：http://jdr.gogol.net.cn

max(d, key=d.get)
来源：http://jzl.birdmap.top

[U10] Py：按值排序字典
来源：http://hog.chenjidiqi.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nhi.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://atk.shanyushiyangkeji.top

(x * 2 for x in arr)
来源：http://rgc.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://ric.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://wwe.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://xmd.fengsongda.top

deque(maxlen=10)
来源：http://vtd.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://nsq.0kj1m.cn

defaultdict(list)
来源：http://kzl.guowangkeji.top

[U15] Py：高精度计时
来源：http://bxp.mhx1999.top

t = time.perf_counter()
来源：http://ups.guowangkeji.top

[U16] Py：命令行参数解析
来源：http://uak.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jrv.316326.xyz

[U17] Py：初始化日志
来源：http://mzc.ydzc1.top

logging.basicConfig(level=logging.INFO)
来源：http://jaz.mhx1999.top

[U18] Py：预编译正则
来源：http://wvq.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://jtn.jqgfzy.top

[U19] Py：正则替换带回调
来源：http://yms.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lrv.zhixingplan.top

[U20] Py：缓存函数结果
来源：http://sic.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://peu.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://hkj.jinqigfzy.top

@contextlib.contextmanager
来源：http://bxc.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://vri.yfazqb.com

list(zip(*m))
来源：http://qyk.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://rzk.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://few.vqdsnc.cn

[U24] Py：路径操作
来源：http://hid.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://deb.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://utt.zdqjudy.top

csv.DictReader(f)
来源：http://kzl.wangshuangyany.cn

[U26] Py：并发下载
来源：http://mpx.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://okh.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://srk.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://soi.yj202588.top

[U28] Py：类型别名
来源：http://lml.shzxlz.cn

UserId = int
来源：http://plt.hywenlv.cn

[U29] Py：属性校验
来源：http://ogr.fengsongda.top

@property 与 @x.setter 配合
来源：http://sxf.sufxvd.cn

[U30] Py：数据类
来源：http://mvr.jyoumei.cn

@dataclass(slots=True)
来源：http://suj.bbcook.cn

[U31] Py：单测
来源：http://pwy.haohaochexian.top

python -m pytest -q
来源：http://een.smart0.xyz

[U32] Py：代码格式化
来源：http://ylk.ydzc1.top

ruff format . && ruff check --fix .
来源：http://wmu.svipenyu.cn

[U33] Py：打包发布
来源：http://ytr.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://ldm.bjfxy.top

[U34] Py：判断编码
来源：http://wud.pycfn.com

chardet.detect(raw)
来源：http://stf.fzhhl.top

[U35] Py：发送邮件
来源：http://cms.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zhp.smart0.xyz

[U36] Py：定时任务
来源：http://lks.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://lxy.svipenyu.cn

[U37] Py：读写 Excel
来源：http://izt.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://fbq.tianlin.xyz

[U38] Py：获取脚本所在目录
来源：http://opl.hnqzz.top

Path(__file__).resolve().parent
来源：http://cny.zycfv.cn

[U39] Py：判断是否在交互环境
来源：http://ypc.chenjidiqi.icu

sys.stdout.isatty()
来源：http://whq.yfazqb.com

[U40] Py：打印到标准错误
来源：http://oid.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://vbr.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://gyi.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cla.redwolf501.top

[U42] PHP：PSR-4 自动加载
来源：http://zhy.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jgp.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://jyn.wangshuangyany.cn

namespace App\Http;
来源：http://bik.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://axz.zhengqikj.top

declare(strict_types=1);
来源：http://lcc.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://qpy.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ior.ydjk.org.cn

[U46] PHP：可空类型
来源：http://cqc.wangshuangyany.cn

?string $name = null
来源：http://cgl.gotoacloud.top

[U47] PHP：联合类型
来源：http://dvd.c1oappe.top

int|string $id
来源：http://oal.zhixingplan.top

[U48] PHP：纯枚举
来源：http://xwi.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brj.hywenlv.cn

[U49] PHP：只读属性
来源：http://ken.iojbl.cn

public readonly string $name
来源：http://mkj.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://vab.bjfxy.top

public function __construct(private int $id) {}
来源：http://zws.chenzaomai.com

[U51] PHP：数组解构
来源：http://gzl.fengsongda.top

[$a, $b] = $arr;
来源：http://qfc.quarkkingdee.top

[U52] PHP：箭头函数
来源：http://ebc.zdbjq.cn

$double = fn($x) => $x * 2;
来源：http://mog.cashguo.top

[U53] PHP：空合并运算符
来源：http://bef.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://guv.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://bet.chenzaomai.com

$obj?->method()
来源：http://qsp.gzhubu.top

[U55] PHP：match 表达式
来源：http://rvw.havefunace.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bmb.jqgfzy.top

[U56] PHP：命名参数
来源：http://fhh.jianghu66.top

f(a: 1, b: 2)
来源：http://nkv.dashuyun.cn

[U57] PHP：字符串插值
来源：http://iba.aizwys.cn

"值: {$a}"
来源：http://wjv.bbcook.cn

[U58] PHP：数组三件套
来源：http://oaz.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://all.tarul.cn

[U59] PHP：自定义排序
来源：http://nat.yangfankeji.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://orm.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://oqa.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gou.hnxiangtu.top

[U61] PHP：正则
来源：http://pfa.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eqr.zhijiandao.cn

[U62] PHP：日期对象
来源：http://aol.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yqi.haohaochexian.top

[U63] PHP：文件读写
来源：http://vll.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zlc.zdqjudy.top

[U64] PHP：目录遍历
来源：http://lmb.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://kde.xinyue.icu

[U65] PHP：会话
来源：http://ljk.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://oke.yfazqb.com

[U66] PHP：设置 Cookie
来源：http://ybr.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lpv.52xcode.cn

[U67] PHP：处理文件上传
来源：http://idf.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fxf.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://jvx.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eep.sweek.top

[U69] PHP：PDO 预处理
来源：http://arl.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tuj.ybcxt.top

[U70] PHP：PDO 事务
来源：http://cam.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uud.sweek.top

[U71] PHP：抛出异常
来源：http://gnh.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://gha.sufxvd.cn

[U72] PHP：写错误日志
来源：http://aro.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://zcp.sweek.top

[U73] PHP：读取 ini 配置
来源：http://eef.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://tkm.yangfankeji.com

[U74] PHP：读取环境变量
来源：http://nxe.ywan-chungtsiang.top

getenv("APP_ENV") ?: "production"
来源：http://ean.tian-w.cn

[U75] PHP：依赖注入
来源：http://ftv.nanxuanxn.top

composer require psr/container
来源：http://ctp.yvedp.cn

[U76] PHP：简单路由
来源：http://dlp.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ayw.xuanzx.com

[U77] PHP：模板渲染
来源：http://cxi.cdnleiting.top

composer require twig/twig
来源：http://fof.hysaishi.cn

[U78] PHP：单元测试
来源：http://gay.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://fqv.haohaochexian.top

[U79] PHP：静态分析
来源：http://lxm.havefunace.top

composer require --dev phpstan/phpstan
来源：http://jez.yj202588.top

[U80] PHP：代码规范修复
来源：http://cbx.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ugw.xziqi.cn

[U81] JS：初始化项目
来源：http://qgo.smart0.xyz

npm init -y;  npm i express
来源：http://juz.cdnleiting.top

[U82] JS：package.json 脚本
来源：http://cml.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mgy.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://cuv.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://lpf.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://wvf.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wsm.ywan-chungtsiang.top

[U85] JS：可选链
来源：http://heu.zhoulong.xyz

a?.b?.c
来源：http://tte.fehbvm.com

[U86] JS：空值合并
来源：http://pul.yuanzhike.top

a ?? b
来源：http://oey.shuidangran.top

[U87] JS：解构默认值
来源：http://djm.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://oub.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://jfv.uphjek.com

{ ...a, ...b }
来源：http://hae.fehbvm.com

[U89] JS：数组去重
来源：http://zoq.snrcjt.cn

[...new Set(arr)]
来源：http://omr.ydzc1.top

[U90] JS：数字数组排序
来源：http://ucr.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://glm.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://lly.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uwp.jlsjyb.cn

[U92] JS：深拷贝
来源：http://bai.bjfxy.top

structuredClone(obj)
来源：http://jxg.hnqzz.top

[U93] JS：模板字符串
来源：http://rxs.zhixingplan.top

`共 ${n} 条`
来源：http://fzq.gzhubu.top

[U94] JS：箭头函数
来源：http://ihe.ivvv.top

const double = x => x * 2;
来源：http://esc.chenlongwang.top

[U95] JS：Promise 包装
来源：http://wvo.svipenyu.cn

new Promise((resolve, reject) => {})
来源：http://uyv.smart0.xyz

[U96] JS：async/await 与异常
来源：http://dsl.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ibp.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://cas.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://wmz.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://ghb.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nwh.ivvv.top

[U99] JS：事件监听
来源：http://pgu.daxiang520.top

el.addEventListener("click", e => {})
来源：http://sfk.hongshengwenyu.top

[U100] JS：DOM 查询
来源：http://yto.andypj.xyz

document.querySelector(".item")
来源：http://pte.dianchejie.cn

[U101] JS：classList 操作
来源：http://fpi.feifeiyinyue.top

el.classList.toggle("active")
来源：http://qhd.zdqjudy.top

[U102] JS：本地存储
来源：http://unp.dianchejie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bdh.daxiang520.top

[U103] JS：定时器
来源：http://mom.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mmt.tarul.cn

[U104] JS：防抖
来源：http://xmu.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yuy.fengsongda.top

[U105] JS：节流
来源：http://mea.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nrp.wangdashe.top

[U106] JS：日期格式化
来源：http://hvh.pycfn.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kvz.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://vnr.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lnu.andypj.xyz

[U108] JS：随机整数
来源：http://kmi.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ine.vehdjk.com

[U109] JS：数组分组
来源：http://xym.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://uzx.epnwcf.com

[U110] JS：数组分块
来源：http://eyb.daxiang520.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zxc.ywan-chungtsiang.top

[U111] JS：对象转 Map
来源：http://lyc.yueranfly.top

new Map(Object.entries(obj))
来源：http://ymq.cucudq.cn

[U112] JS：字符串补位
来源：http://yxw.hnxiangtu.top

"7".padStart(3, "0")
来源：http://twp.yfazqb.com

[U113] JS：正则替换全部
来源：http://cex.cdnleiting.top

s.replaceAll("a", "b")
来源：http://yjj.ehwqpu.com

[U114] JS：JSON 深比较
来源：http://bpa.andypj.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://eth.shuidangran.top

[U115] JS：生成 UUID
来源：http://loi.dashuyun.cn

crypto.randomUUID()
来源：http://xal.chenjidiqi.icu

[U116] JS：类型检查（JSDoc）
来源：http://nuo.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://shh.jianghu66.top

[U117] JS：单元测试
来源：http://ydk.52xcode.cn

npm i -D vitest;  npx vitest
来源：http://yuf.hcnkem.com

[U118] JS：开发服务器
来源：http://phc.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://cpr.jinyuanbaomall.cn

[U119] JS：生产构建
来源：http://dcy.havefunace.top

npx vite build
来源：http://atq.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://nqb.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://nvv.jinyuanbaomall.cn

================================================================================
来源：http://sgq.chenlongwang.top

统计汇总
来源：http://ytr.svipenyu.cn

================================================================================
来源：http://lho.zhoulong.xyz

按语言统计（条）：
来源：http://qco.hongshengwenyu.top

Python ......... 252
来源：http://pxc.xylfe.cn

PHP ............ 252
来源：http://oym.vqdsnc.cn

JavaScript ..... 252
来源：http://kls.gaohongyu789.top

TypeScript ..... 212
来源：http://yrh.fanxiaobao.xyz

Java ........... 212
来源：http://kwq.hongshengwenyu.top

Go ............. 212
来源：http://bcv.xinyue.icu

Ruby ........... 212
来源：http://ipj.ybcxt.top

C# ............. 212
来源：http://qka.hnqzz.top

C .............. 30
来源：http://brh.hfpthk.cn

C++ ............ 30
来源：http://ehh.zhijiandao.cn

SQL ............ 90
来源：http://uzf.yonumen.top

Bash ........... 80
来源：http://hmn.bjfxy.top

Kotlin ......... 15
来源：http://kyi.yj20258.top

Swift .......... 15
来源：http://bxt.sweek.top

Lua ............ 10
来源：http://poc.zycfv.cn

Perl ........... 10
来源：http://oqb.vehdjk.com

Scala .......... 10
来源：http://usa.wangdashe.top

------------------------------------
来源：http://nlc.hnxiangtu.top

合计 ........... 2106 条
来源：http://hsa.zhijiandao.cn

按章节统计：
来源：http://rgc.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pgj.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zdk.chenlongwang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ffc.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://svx.jqgfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://izd.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uqr.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://brk.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xtl.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rjl.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bzs.zhixingplan.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uln.sufxvd.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ais.tian-w.cn


<!-- 参考信息 -->