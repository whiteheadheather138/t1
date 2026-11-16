代发 wailian999

[T47] Perl：正则捕获
来源：http://nuy.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pxp.52xcode.cn

[T48] Perl：正则替换
来源：http://yqc.hcnkem.com

$s =~ s/old/new/g;
来源：http://wwn.zhoulong.xyz

[T49] Perl：函数
来源：http://brn.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ffl.iojbl.cn

[T50] Perl：逐行读文件
来源：http://zvz.vehdjk.com

open my $fh, "<", "a.txt" or die $!;
来源：http://tsl.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://eoo.smart0.xyz

[T51] Scala：Hello World
来源：http://nqf.wangshuangyany.cn

println("Hello")
来源：http://qfn.yongpay.top

[T52] Scala：变量
来源：http://iff.cheryme.top

val a = 1;  var b = 2
来源：http://izv.zycfv.cn

[T53] Scala：字符串插值
来源：http://tns.zhoulong.xyz

s"值: $b"
来源：http://yqm.cqqwz.cn

[T54] Scala：集合映射
来源：http://vjs.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://wxx.uphjek.com

[T55] Scala：集合过滤
来源：http://osm.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lav.bjfxy.top

[T56] Scala：样例类
来源：http://xdc.chenzaomai.com

case class User(name: String, age: Int)
来源：http://min.xuanzx.com

[T57] Scala：模式匹配
来源：http://yld.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cln.shuidangran.top

[T58] Scala：函数定义
来源：http://hju.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://hfw.xziqi.cn

[T59] Scala：循环
来源：http://vcr.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://psw.9152youxi.cn

[T60] Scala：折叠
来源：http://ygb.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ebd.xziqi.cn

================================================================================
来源：http://mqc.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://txt.yangfankeji.com

================================================================================
来源：http://ncu.haohaochexian.top

[U01] Py：创建虚拟环境
来源：http://esq.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gik.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://cbi.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fwy.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://rih.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://oir.shuidangran.top

[U04] Py：变量调试打印
来源：http://trs.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zid.sxryk.cn

[U05] Py：列表去重且保序
来源：http://ndt.bjfxy.top

list(dict.fromkeys(arr))
来源：http://cze.havefunace.top

[U06] Py：合并两个字典
来源：http://scn.ehwqpu.com

{**a, **b}
来源：http://fzy.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://zgm.fehbvm.com

{v: k for k, v in d.items()}
来源：http://kya.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://yvg.xuanzx.com

[y for x in nested for y in x]
来源：http://srf.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://wsn.zdbjq.cn

max(d, key=d.get)
来源：http://owa.zdqjudy.top

[U10] Py：按值排序字典
来源：http://zcn.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vwa.xylfe.cn

[U11] Py：生成器表达式
来源：http://qnw.jqgfzy.top

(x * 2 for x in arr)
来源：http://ifd.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://xue.havefunace.top

Counter(arr).most_common(3)
来源：http://flk.svipenyu.cn

[U13] Py：固定长度队列
来源：http://cmx.meibo888.top

deque(maxlen=10)
来源：http://szh.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://yse.tarul.cn

defaultdict(list)
来源：http://xps.aibaodan.cn

[U15] Py：高精度计时
来源：http://fhz.yonumen.top

t = time.perf_counter()
来源：http://kum.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://med.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uzl.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://ppl.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://djj.gogol.net.cn

[U18] Py：预编译正则
来源：http://ucl.fehbvm.com

pat = re.compile(r"\d+")
来源：http://eck.zhiwuduotai.top

[U19] Py：正则替换带回调
来源：http://xyb.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyq.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://rya.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://tkg.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://jaf.bjfxy.top

@contextlib.contextmanager
来源：http://xfi.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://wmf.shanyushiyangtech.top

list(zip(*m))
来源：http://dir.shuidangran.top

[U23] Py：分块读取大文件
来源：http://lot.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aqn.tanke756.top

[U24] Py：路径操作
来源：http://uzk.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udm.52xcode.cn

[U25] Py：CSV 按字典读
来源：http://flc.ydjk.org.cn

csv.DictReader(f)
来源：http://hgm.cashguo.top

[U26] Py：并发下载
来源：http://qzl.fengsongda.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zdl.fehbvm.com

[U27] Py：异步 HTTP
来源：http://hnk.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://hni.guannengcc.top

[U28] Py：类型别名
来源：http://qgh.sweek.top

UserId = int
来源：http://omm.fehbvm.com

[U29] Py：属性校验
来源：http://yfb.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://vke.jinghuilouyu.cn

[U30] Py：数据类
来源：http://snc.cheryme.top

@dataclass(slots=True)
来源：http://nar.xziqi.cn

[U31] Py：单测
来源：http://xas.sxryk.cn

python -m pytest -q
来源：http://roj.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://qqh.daria6918.cn

ruff format . && ruff check --fix .
来源：http://rta.fengsongda.top

[U33] Py：打包发布
来源：http://fka.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://jwr.svipenyu.cn

[U34] Py：判断编码
来源：http://wve.cdnleiting.top

chardet.detect(raw)
来源：http://kon.zhoulong.xyz

[U35] Py：发送邮件
来源：http://thh.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rki.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://hfd.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://snm.guowangkeji.top

[U37] Py：读写 Excel
来源：http://wtb.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://jnd.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://qts.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://cxk.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://ggx.yfazqb.com

sys.stdout.isatty()
来源：http://oyv.sysykeji.top

[U40] Py：打印到标准错误
来源：http://uey.tarul.cn

print("err", file=sys.stderr)
来源：http://mgs.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://iyx.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jjj.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://twq.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qzh.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://vdt.smart0.xyz

namespace App\Http;
来源：http://raq.xziqi.cn

[U44] PHP：开启严格类型
来源：http://hir.birdmap.top

declare(strict_types=1);
来源：http://vch.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://trm.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://enz.nanxuanxn.top

[U46] PHP：可空类型
来源：http://kfa.xziqi.cn

?string $name = null
来源：http://nob.jlsjyb.cn

[U47] PHP：联合类型
来源：http://uqp.svipenyu.cn

int|string $id
来源：http://qyw.jyoumei.cn

[U48] PHP：纯枚举
来源：http://hwe.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vub.sweek.top

[U49] PHP：只读属性
来源：http://qcg.hnxiangtu.top

public readonly string $name
来源：http://ptl.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://eap.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://xqy.chenzaomai.com

[U51] PHP：数组解构
来源：http://fwc.wangdashe.top

[$a, $b] = $arr;
来源：http://lpc.chenlongwang.top

[U52] PHP：箭头函数
来源：http://gkn.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://ute.ivvv.top

[U53] PHP：空合并运算符
来源：http://ust.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://tht.yonumen.top

[U54] PHP：空安全调用
来源：http://tee.epnwcf.com

$obj?->method()
来源：http://bgm.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://efv.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ybz.hnqzz.top

[U56] PHP：命名参数
来源：http://cob.yonumen.top

f(a: 1, b: 2)
来源：http://iyd.gogol.net.cn

[U57] PHP：字符串插值
来源：http://fga.vqdsnc.cn

"值: {$a}"
来源：http://dqj.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://fqz.sysykeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xyp.iojbl.cn

[U59] PHP：自定义排序
来源：http://hba.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bjk.yongpay.top

[U60] PHP：JSON 编解码
来源：http://wzg.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pmj.52xcode.cn

[U61] PHP：正则
来源：http://nmk.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ocy.vehdjk.com

[U62] PHP：日期对象
来源：http://opy.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ers.iojbl.cn

[U63] PHP：文件读写
来源：http://flv.xingfuxueyuan.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yij.xinyue.icu

[U64] PHP：目录遍历
来源：http://hcg.yj20258888.top

glob("dir/*.php");  scandir("dir");
来源：http://mnu.9152youxi.cn

[U65] PHP：会话
来源：http://sye.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lmh.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://iuk.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://viq.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://gep.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kea.haohaochexian.top

[U68] PHP：PDO 连接
来源：http://yvf.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zxd.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://hum.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wno.yj20258888.top

[U70] PHP：PDO 事务
来源：http://hzn.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ynk.hnqzz.top

[U71] PHP：抛出异常
来源：http://apn.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://zze.iojbl.cn

[U72] PHP：写错误日志
来源：http://wkg.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://lyu.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://drb.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://fim.xylfe.cn

[U74] PHP：读取环境变量
来源：http://mxr.jinqigfzy.top

getenv("APP_ENV") ?: "production"
来源：http://plk.yj202588.top

[U75] PHP：依赖注入
来源：http://ocd.xuetiantiany.cn

composer require psr/container
来源：http://zqf.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://fmv.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vgm.dianchejie.cn

[U77] PHP：模板渲染
来源：http://swu.xuetiantiany.cn

composer require twig/twig
来源：http://oqr.zdqjudy.top

[U78] PHP：单元测试
来源：http://exj.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://xuk.hysaishi.cn

[U79] PHP：静态分析
来源：http://zlj.redwolf501.top

composer require --dev phpstan/phpstan
来源：http://ive.zhixingplan.top

[U80] PHP：代码规范修复
来源：http://lcp.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://thp.hcnkem.com

[U81] JS：初始化项目
来源：http://xkb.sjlbkw.cn

npm init -y;  npm i express
来源：http://aoy.sysykeji.top

[U82] JS：package.json 脚本
来源：http://bsr.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://arl.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://otq.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://glx.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://uka.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://gvk.xylfe.cn

[U85] JS：可选链
来源：http://ovy.zhoulong.xyz

a?.b?.c
来源：http://yfa.ybcxt.top

[U86] JS：空值合并
来源：http://okt.feifeiyinyue.top

a ?? b
来源：http://swm.fengsongda.top

[U87] JS：解构默认值
来源：http://xrm.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://axa.gotoacloud.top

[U88] JS：对象展开合并
来源：http://kfm.andypj.xyz

{ ...a, ...b }
来源：http://twu.sxryk.cn

[U89] JS：数组去重
来源：http://wwe.uphjek.com

[...new Set(arr)]
来源：http://xnv.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://oqc.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://hnk.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://dua.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://plj.0kj1m.cn

[U92] JS：深拷贝
来源：http://yic.jinyuanbaomall.cn

structuredClone(obj)
来源：http://iua.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://iuk.vqdsnc.cn

`共 ${n} 条`
来源：http://sji.yfazqb.com

[U94] JS：箭头函数
来源：http://wfj.hywenlv.cn

const double = x => x * 2;
来源：http://qmm.hcnkem.com

[U95] JS：Promise 包装
来源：http://owt.yuanzhike.top

new Promise((resolve, reject) => {})
来源：http://bkw.jinqigufen.top

[U96] JS：async/await 与异常
来源：http://kjq.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xzf.sxryk.cn

[U97] JS：并发请求
来源：http://pvi.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qpt.ywan-chungtsiang.top

[U98] JS：fetch 带 JSON
来源：http://tzo.pycfn.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://htn.0kj1m.cn

[U99] JS：事件监听
来源：http://adf.jinqigfzy.top

el.addEventListener("click", e => {})
来源：http://qti.shuidangran.top

[U100] JS：DOM 查询
来源：http://hfx.wangshuangyany.cn

document.querySelector(".item")
来源：http://nln.hfpthk.cn

[U101] JS：classList 操作
来源：http://kam.hnxiangtu.top

el.classList.toggle("active")
来源：http://jsa.wangdashe.top

[U102] JS：本地存储
来源：http://clf.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zkv.0kj1m.cn

[U103] JS：定时器
来源：http://cls.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qvh.hnxiangtu.top

[U104] JS：防抖
来源：http://cmx.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ouf.zhiwuduotai.top

[U105] JS：节流
来源：http://onl.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zsj.nanxinkj.top

[U106] JS：日期格式化
来源：http://blg.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zoj.cashguo.top

[U107] JS：数字千分位
来源：http://bck.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ioa.shuidangran.top

[U108] JS：随机整数
来源：http://cze.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wka.hfpthk.cn

[U109] JS：数组分组
来源：http://kqs.hfpthk.cn

Object.groupBy(arr, x => x.type)
来源：http://lke.zycfv.cn

[U110] JS：数组分块
来源：http://fxp.ybcxt.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kcz.nwbrower.top

[U111] JS：对象转 Map
来源：http://aez.ybcxt.top

new Map(Object.entries(obj))
来源：http://yxx.mhx1999.top

[U112] JS：字符串补位
来源：http://djq.gogol.net.cn

"7".padStart(3, "0")
来源：http://enb.daxiang520.top

[U113] JS：正则替换全部
来源：http://blh.c1oappe.top

s.replaceAll("a", "b")
来源：http://mig.zhijiandao.cn

[U114] JS：JSON 深比较
来源：http://huw.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jwl.shuidangran.top

[U115] JS：生成 UUID
来源：http://nzq.bjfxy.top

crypto.randomUUID()
来源：http://wzg.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://kue.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://xcb.fengsongda.top

[U117] JS：单元测试
来源：http://xmr.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://dxd.bjfxy.top

[U118] JS：开发服务器
来源：http://rpj.hnqzz.top

npm i -D vite;  npx vite
来源：http://vbq.gogol.net.cn

[U119] JS：生产构建
来源：http://gig.nwbrower.top

npx vite build
来源：http://fdn.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://kqp.yvedp.cn

import.meta.env.VITE_API_URL
来源：http://xgt.9152youxi.cn

================================================================================
来源：http://emf.xingfuxueyuan.xyz

统计汇总
来源：http://soi.shangyingyoupin.top

================================================================================
来源：http://eqe.snrcjt.cn

按语言统计（条）：
来源：http://bug.ivvv.top

Python ......... 252
来源：http://xmi.sjlbkw.cn

PHP ............ 252
来源：http://dki.shanyushiyangkeji.top

JavaScript ..... 252
来源：http://oeb.zhiwuduotai.top

TypeScript ..... 212
来源：http://twa.shanyushiyangtech.top

Java ........... 212
来源：http://rrt.sweek.top

Go ............. 212
来源：http://yns.epnwcf.com

Ruby ........... 212
来源：http://tci.yj202588.top

C# ............. 212
来源：http://gbp.zhengqikj.top

C .............. 30
来源：http://mgr.jianghu66.top

C++ ............ 30
来源：http://kqi.andypj.xyz

SQL ............ 90
来源：http://nea.havefunace.top

Bash ........... 80
来源：http://hag.dashuyun.cn

Kotlin ......... 15
来源：http://tet.jianghu66.top

Swift .......... 15
来源：http://dvq.ybcxt.top

Lua ............ 10
来源：http://trq.hnqzz.top

Perl ........... 10
来源：http://jse.jinqigfzy.top

Scala .......... 10
来源：http://kvz.52xcode.cn

------------------------------------
来源：http://dxe.chenzaomai.com

合计 ........... 2106 条
来源：http://aph.fehbvm.com

按章节统计：
来源：http://jzw.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xiw.9152youxi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rqb.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sja.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bin.jinqigfzy.top


<!-- 参考信息 -->