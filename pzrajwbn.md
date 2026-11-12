代发 wailian999

[T49] Perl：函数
来源：http://doe.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nkk.birdmap.top

[T50] Perl：逐行读文件
来源：http://ecy.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kov.zhoulong.xyz

while (my $line = <$fh>) { print $line; }
来源：http://zzh.dianchejie.cn

[T51] Scala：Hello World
来源：http://zed.gogol.net.cn

println("Hello")
来源：http://pvk.bbcook.cn

[T52] Scala：变量
来源：http://ekr.zdbjq.cn

val a = 1;  var b = 2
来源：http://sco.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://ijx.meibo888.top

s"值: $b"
来源：http://whz.c1oappe.top

[T54] Scala：集合映射
来源：http://dbw.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://vhk.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://cze.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://zvm.svipenyu.cn

[T56] Scala：样例类
来源：http://usw.sweek.top

case class User(name: String, age: Int)
来源：http://fwz.svipenyu.cn

[T57] Scala：模式匹配
来源：http://aob.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://stx.daxiang520.top

[T58] Scala：函数定义
来源：http://aof.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://zng.tian-w.cn

[T59] Scala：循环
来源：http://frr.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://qbf.zhengqikj.top

[T60] Scala：折叠
来源：http://vgh.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://shw.fktsv.cn

================================================================================
来源：http://tze.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://swi.xuetiantiany.cn

================================================================================
来源：http://oyw.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://cgk.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://ptp.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://vop.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://srp.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://nnn.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://rym.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://fhm.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ohy.bjfxy.top

[U05] Py：列表去重且保序
来源：http://xzw.fengsongda.top

list(dict.fromkeys(arr))
来源：http://glk.yj20258888.top

[U06] Py：合并两个字典
来源：http://roa.yj20258.top

{**a, **b}
来源：http://gmb.dianchejie.cn

[U07] Py：反转字典键值
来源：http://qwi.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://rwo.52xcode.cn

[U08] Py：展平二维列表
来源：http://svf.zhijiandao.cn

[y for x in nested for y in x]
来源：http://cmy.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://eyl.xinyue.icu

max(d, key=d.get)
来源：http://vrj.yangfankeji.com

[U10] Py：按值排序字典
来源：http://ktj.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wer.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://flq.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://fxg.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fnh.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://bhs.fehbvm.com

[U13] Py：固定长度队列
来源：http://rzq.bjfxy.top

deque(maxlen=10)
来源：http://glz.zhixingplan.top

[U14] Py：分组收集到列表
来源：http://knt.jyoumei.cn

defaultdict(list)
来源：http://aon.sjlbkw.cn

[U15] Py：高精度计时
来源：http://ijj.yangfankeji.com

t = time.perf_counter()
来源：http://uhs.smart0.xyz

[U16] Py：命令行参数解析
来源：http://tvs.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bhq.cashguo.top

[U17] Py：初始化日志
来源：http://kln.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://klu.zdbjq.cn

[U18] Py：预编译正则
来源：http://mcy.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://mjz.gzhubu.top

[U19] Py：正则替换带回调
来源：http://ufk.xinyue.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://geb.zycfv.cn

[U20] Py：缓存函数结果
来源：http://zjh.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://yze.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://wir.yj20258888.top

@contextlib.contextmanager
来源：http://hsh.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://ykr.zhiwuduotai.top

list(zip(*m))
来源：http://fee.hnqzz.top

[U23] Py：分块读取大文件
来源：http://ybj.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lgh.dashuyun.cn

[U24] Py：路径操作
来源：http://xop.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qai.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://geg.andypj.xyz

csv.DictReader(f)
来源：http://aht.hnxiangtu.top

[U26] Py：并发下载
来源：http://uht.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ffa.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://htp.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://azv.hnqzz.top

[U28] Py：类型别名
来源：http://tmn.andypj.xyz

UserId = int
来源：http://emo.svipenyu.cn

[U29] Py：属性校验
来源：http://jgt.ctjpmb.com

@property 与 @x.setter 配合
来源：http://dsq.epnwcf.com

[U30] Py：数据类
来源：http://vdq.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://idx.aizwys.cn

[U31] Py：单测
来源：http://oeo.sjlbkw.cn

python -m pytest -q
来源：http://fkf.cucudq.cn

[U32] Py：代码格式化
来源：http://fyp.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://ogw.0kj1m.cn

[U33] Py：打包发布
来源：http://xhe.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://fqf.zhongyouzk.top

[U34] Py：判断编码
来源：http://bna.yangfankeji.com

chardet.detect(raw)
来源：http://vyi.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://xim.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dhc.epnwcf.com

[U36] Py：定时任务
来源：http://dtm.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://kmc.hfpthk.cn

[U37] Py：读写 Excel
来源：http://suf.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zop.ctjpmb.com

[U38] Py：获取脚本所在目录
来源：http://ivk.zhiwuduotai.top

Path(__file__).resolve().parent
来源：http://qso.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://lst.meibo888.top

sys.stdout.isatty()
来源：http://jpe.bbcook.cn

[U40] Py：打印到标准错误
来源：http://zac.aibaodan.cn

print("err", file=sys.stderr)
来源：http://hik.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://dud.jqgufenzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vkl.mhx1999.top

[U42] PHP：PSR-4 自动加载
来源：http://byr.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nip.yj202588.top

[U43] PHP：声明命名空间
来源：http://par.guowangkeji.top

namespace App\Http;
来源：http://smh.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://qwc.sweek.top

declare(strict_types=1);
来源：http://gex.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://ywh.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://srk.zhengqikj.top

[U46] PHP：可空类型
来源：http://cql.yonumen.top

?string $name = null
来源：http://jtv.smart0.xyz

[U47] PHP：联合类型
来源：http://lwz.zdbjq.cn

int|string $id
来源：http://gxh.mhx1999.top

[U48] PHP：纯枚举
来源：http://yfr.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mjm.tanke756.top

[U49] PHP：只读属性
来源：http://fxw.vqdsnc.cn

public readonly string $name
来源：http://ozl.smart0.xyz

[U50] PHP：构造器属性提升
来源：http://nao.nanxinkj.top

public function __construct(private int $id) {}
来源：http://blw.tian-w.cn

[U51] PHP：数组解构
来源：http://duc.tianlin.xyz

[$a, $b] = $arr;
来源：http://tqo.ydzc1.top

[U52] PHP：箭头函数
来源：http://kjv.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://col.daxiang520.top

[U53] PHP：空合并运算符
来源：http://ywy.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://fjq.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://xij.hesvh.cn

$obj?->method()
来源：http://srt.nwbrower.top

[U55] PHP：match 表达式
来源：http://oki.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xoq.hnxiangtu.top

[U56] PHP：命名参数
来源：http://nvf.fengsongda.top

f(a: 1, b: 2)
来源：http://owl.hammf.cn

[U57] PHP：字符串插值
来源：http://vee.xylfe.cn

"值: {$a}"
来源：http://ejx.zycfv.cn

[U58] PHP：数组三件套
来源：http://leo.zhoulong.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rys.gzhubu.top

[U59] PHP：自定义排序
来源：http://wvb.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vni.yangfankeji.com

[U60] PHP：JSON 编解码
来源：http://xei.fzhhl.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tsg.ydzc1.top

[U61] PHP：正则
来源：http://blq.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dbi.fehbvm.com

[U62] PHP：日期对象
来源：http://tyo.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wjg.jinqigfzy.top

[U63] PHP：文件读写
来源：http://wor.sufxvd.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bgh.jinghuilouyu.cn

[U64] PHP：目录遍历
来源：http://gwt.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://div.snrcjt.cn

[U65] PHP：会话
来源：http://uqb.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qop.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://dyd.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qiz.fktsv.cn

[U67] PHP：处理文件上传
来源：http://rhb.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ogc.xuetiantiany.cn

[U68] PHP：PDO 连接
来源：http://ehf.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lmm.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://zlc.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qxb.zycfv.cn

[U70] PHP：PDO 事务
来源：http://fza.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ekr.uphjek.com

[U71] PHP：抛出异常
来源：http://evp.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://qpy.tian-w.cn

[U72] PHP：写错误日志
来源：http://kre.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://osp.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://wzi.hesvh.cn

parse_ini_file("config.ini", true)
来源：http://kpn.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://bbe.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://hmp.cheryme.top

[U75] PHP：依赖注入
来源：http://sld.daxiang520.top

composer require psr/container
来源：http://upy.guowangkeji.top

[U76] PHP：简单路由
来源：http://hzo.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lkb.dianchejie.cn

[U77] PHP：模板渲染
来源：http://pnz.mhx1999.top

composer require twig/twig
来源：http://imj.iojbl.cn

[U78] PHP：单元测试
来源：http://arg.smart0.xyz

composer require --dev phpunit/phpunit
来源：http://wpb.cqqwz.cn

[U79] PHP：静态分析
来源：http://bij.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://qcq.sufxvd.cn

[U80] PHP：代码规范修复
来源：http://njp.chenlongwang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://msd.shzxlz.cn

[U81] JS：初始化项目
来源：http://gkb.chenjidiqi.icu

npm init -y;  npm i express
来源：http://mhl.xziqi.cn

[U82] JS：package.json 脚本
来源：http://psb.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wsf.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://gmf.316326.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://tcc.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://kou.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://udz.wangshuangyany.cn

[U85] JS：可选链
来源：http://qvi.zhaomingkeji.xyz

a?.b?.c
来源：http://ugx.hnxiangtu.top

[U86] JS：空值合并
来源：http://osa.ppjwa.cn

a ?? b
来源：http://rsj.zdqjudy.top

[U87] JS：解构默认值
来源：http://ufz.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://nyd.daxiang520.top

[U88] JS：对象展开合并
来源：http://tcs.guowangkeji.top

{ ...a, ...b }
来源：http://uju.jqgufenzy.top

[U89] JS：数组去重
来源：http://erq.jinqigufen.top

[...new Set(arr)]
来源：http://uyj.aizwys.cn

[U90] JS：数字数组排序
来源：http://dsl.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://uap.aizwys.cn

[U91] JS：对象键值遍历
来源：http://cte.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lnb.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://ghz.guannengcc.top

structuredClone(obj)
来源：http://mrp.andypj.xyz

[U93] JS：模板字符串
来源：http://ryw.chenjidiqi.icu

`共 ${n} 条`
来源：http://drb.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://rny.sjlbkw.cn

const double = x => x * 2;
来源：http://kad.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://cjc.yongpay.top

new Promise((resolve, reject) => {})
来源：http://alw.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://lhu.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zez.meibo888.top

[U97] JS：并发请求
来源：http://hxs.sxryk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lor.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://ozr.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gri.jlsjyb.cn

[U99] JS：事件监听
来源：http://bag.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://nuw.uphjek.com

[U100] JS：DOM 查询
来源：http://izd.jlsjyb.cn

document.querySelector(".item")
来源：http://kiq.yfazqb.com

[U101] JS：classList 操作
来源：http://end.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://rxs.fengsongda.top

[U102] JS：本地存储
来源：http://dyj.cucudq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ozr.bbcook.cn

[U103] JS：定时器
来源：http://qoc.jlsjyb.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mef.xziqi.cn

[U104] JS：防抖
来源：http://ocs.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ueh.guowangkeji.top

[U105] JS：节流
来源：http://uhu.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iky.quarkkingdee.top

[U106] JS：日期格式化
来源：http://yfb.dianchejie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hmp.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://soq.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://upf.epnwcf.com

[U108] JS：随机整数
来源：http://xbm.fanxiaobao.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iea.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://vbt.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://fht.zhongyouzk.top

[U110] JS：数组分块
来源：http://rcs.hfpthk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yiy.tanke756.top

[U111] JS：对象转 Map
来源：http://mwn.aibaodan.cn

new Map(Object.entries(obj))
来源：http://oig.cdnleiting.top

[U112] JS：字符串补位
来源：http://hbs.zhoulong.xyz

"7".padStart(3, "0")
来源：http://uhc.chenzaomai.com

[U113] JS：正则替换全部
来源：http://fzi.ppjwa.cn

s.replaceAll("a", "b")
来源：http://ush.aizwys.cn

[U114] JS：JSON 深比较
来源：http://hym.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://zum.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://hux.uphjek.com

crypto.randomUUID()
来源：http://knc.yj20258.top

[U116] JS：类型检查（JSDoc）
来源：http://omb.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://guf.jinghuilouyu.cn

[U117] JS：单元测试
来源：http://bgc.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://vsv.tarul.cn

[U118] JS：开发服务器
来源：http://mym.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://cgr.epnwcf.com

[U119] JS：生产构建
来源：http://ntt.ivvv.top

npx vite build
来源：http://qvj.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://yda.ctjpmb.com

import.meta.env.VITE_API_URL
来源：http://dri.xingfuxueyuan.xyz

================================================================================
来源：http://nqz.ydjk.org.cn

统计汇总
来源：http://ibj.fehbvm.com

================================================================================
来源：http://tax.sweek.top

按语言统计（条）：
来源：http://hcz.hcnkem.com

Python ......... 252
来源：http://jbv.jianghu66.top

PHP ............ 252
来源：http://snu.nanxinkj.top

JavaScript ..... 252
来源：http://hdj.daria6918.cn

TypeScript ..... 212
来源：http://hfq.jinyuanbaomall.cn

Java ........... 212
来源：http://zlg.xziqi.cn

Go ............. 212
来源：http://fqk.mhx1999.top

Ruby ........... 212
来源：http://qug.zhongyouzk.top

C# ............. 212
来源：http://cgy.jqgfzy.top

C .............. 30
来源：http://mse.fehbvm.com

C++ ............ 30
来源：http://sgt.yvedp.cn

SQL ............ 90
来源：http://ulm.yonumen.top

Bash ........... 80
来源：http://ybj.dianchejie.cn

Kotlin ......... 15
来源：http://cqs.yvedp.cn

Swift .......... 15
来源：http://qwp.ctjpmb.com

Lua ............ 10
来源：http://zvm.yuanzhike.top

Perl ........... 10
来源：http://faf.fehbvm.com

Scala .......... 10
来源：http://kgp.hywenlv.cn

------------------------------------
来源：http://wxr.ctjpmb.com

合计 ........... 2106 条
来源：http://shy.gzhubu.top

按章节统计：
来源：http://zrt.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hgk.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jnf.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://duz.zdbjq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ukc.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hjx.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://syp.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cwy.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hao.pengpengdd.cyou


<!-- 参考信息 -->