代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vxo.fzhhl.top

================================================================================
来源：http://lhc.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mfz.cdnleiting.top

================================================================================
来源：http://mdq.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://jhx.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://tda.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://sic.zycfv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mba.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://gkc.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://duu.c1oappe.top

[U04] Py：变量调试打印
来源：http://bfs.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pyc.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://gzv.ppjwa.cn

list(dict.fromkeys(arr))
来源：http://uxz.fehbvm.com

[U06] Py：合并两个字典
来源：http://lhw.chenlongwang.top

{**a, **b}
来源：http://cfk.guannengcc.top

[U07] Py：反转字典键值
来源：http://dsf.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://mrz.cheryme.top

[U08] Py：展平二维列表
来源：http://xtl.9152youxi.cn

[y for x in nested for y in x]
来源：http://ago.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://csy.zhengqikj.top

max(d, key=d.get)
来源：http://skz.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://wmx.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qvz.yangfankeji.com

[U11] Py：生成器表达式
来源：http://afu.uphjek.com

(x * 2 for x in arr)
来源：http://jio.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://iql.pycfn.com

Counter(arr).most_common(3)
来源：http://pot.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://mkf.haohaochexian.top

deque(maxlen=10)
来源：http://sxg.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://mzp.yuanzhike.top

defaultdict(list)
来源：http://tmk.ybcxt.top

[U15] Py：高精度计时
来源：http://sfw.xuanzx.com

t = time.perf_counter()
来源：http://nqv.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://sbw.nwbrower.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://crd.xinyue.icu

[U17] Py：初始化日志
来源：http://bdc.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://zzm.redwolf501.top

[U18] Py：预编译正则
来源：http://eli.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://vcr.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://qno.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fmb.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://von.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://jny.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://buq.fengsongda.top

@contextlib.contextmanager
来源：http://fyw.cheryme.top

[U22] Py：矩阵转置
来源：http://cna.chenlongwang.top

list(zip(*m))
来源：http://oub.sweek.top

[U23] Py：分块读取大文件
来源：http://skg.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vsa.ctjpmb.com

[U24] Py：路径操作
来源：http://jhk.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wls.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://ymr.daxiang520.top

csv.DictReader(f)
来源：http://mmy.tian-w.cn

[U26] Py：并发下载
来源：http://cbp.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uty.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://wsk.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://rfa.hammf.cn

[U28] Py：类型别名
来源：http://gva.hnqzz.top

UserId = int
来源：http://dov.xinyue.icu

[U29] Py：属性校验
来源：http://hhu.hysaishi.cn

@property 与 @x.setter 配合
来源：http://ulv.52xcode.cn

[U30] Py：数据类
来源：http://cki.yuxming.cn

@dataclass(slots=True)
来源：http://vlk.hcnkem.com

[U31] Py：单测
来源：http://jxa.sjlbkw.cn

python -m pytest -q
来源：http://tde.ydzc1.top

[U32] Py：代码格式化
来源：http://mpl.ybcxt.top

ruff format . && ruff check --fix .
来源：http://mqq.tianlin.xyz

[U33] Py：打包发布
来源：http://yss.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://etl.dashuyun.cn

[U34] Py：判断编码
来源：http://hnk.chenlongwang.top

chardet.detect(raw)
来源：http://ctx.vqdsnc.cn

[U35] Py：发送邮件
来源：http://nws.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ksu.hnxiangtu.top

[U36] Py：定时任务
来源：http://lrl.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://dfv.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://dsc.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://pko.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://tun.uphjek.com

Path(__file__).resolve().parent
来源：http://dsg.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://lhp.hfpthk.cn

sys.stdout.isatty()
来源：http://hkc.sjlbkw.cn

[U40] Py：打印到标准错误
来源：http://mqn.sufxvd.cn

print("err", file=sys.stderr)
来源：http://sid.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://kmg.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mnk.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://yqo.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yeo.daria6918.cn

[U43] PHP：声明命名空间
来源：http://udb.9152youxi.cn

namespace App\Http;
来源：http://fat.jinghuilouyu.cn

[U44] PHP：开启严格类型
来源：http://web.ppjwa.cn

declare(strict_types=1);
来源：http://vnc.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://rks.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://wxf.xylfe.cn

[U46] PHP：可空类型
来源：http://bcb.fengsongda.top

?string $name = null
来源：http://cht.cdnleiting.top

[U47] PHP：联合类型
来源：http://eox.cucudq.cn

int|string $id
来源：http://sva.c1oappe.top

[U48] PHP：纯枚举
来源：http://buk.birdmap.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gqf.zycfv.cn

[U49] PHP：只读属性
来源：http://nzu.yj202588.top

public readonly string $name
来源：http://fhb.wangshuangyany.cn

[U50] PHP：构造器属性提升
来源：http://uzu.cqqwz.cn

public function __construct(private int $id) {}
来源：http://jdz.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://gpj.andypj.xyz

[$a, $b] = $arr;
来源：http://dpe.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://jhn.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://jdo.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://xir.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://vva.zhengqikj.top

[U54] PHP：空安全调用
来源：http://dmv.chenlongwang.top

$obj?->method()
来源：http://xms.0kj1m.cn

[U55] PHP：match 表达式
来源：http://lir.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rgu.zdqjudy.top

[U56] PHP：命名参数
来源：http://the.xuanzx.com

f(a: 1, b: 2)
来源：http://tel.jinqigfzy.top

[U57] PHP：字符串插值
来源：http://snf.havefunace.top

"值: {$a}"
来源：http://bje.aizwys.cn

[U58] PHP：数组三件套
来源：http://hil.yvedp.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xel.zhixingplan.top

[U59] PHP：自定义排序
来源：http://uuj.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oyb.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://iej.52xcode.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bmz.birdmap.top

[U61] PHP：正则
来源：http://xzo.fanxiaobao.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gen.yonumen.top

[U62] PHP：日期对象
来源：http://cxr.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tno.jianghu66.top

[U63] PHP：文件读写
来源：http://lak.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://woy.chenzaomai.com

[U64] PHP：目录遍历
来源：http://ytu.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://hki.svipenyu.cn

[U65] PHP：会话
来源：http://vnt.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tmw.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://vir.wangshuangyany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rcz.sxryk.cn

[U67] PHP：处理文件上传
来源：http://pwu.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nfz.yongpay.top

[U68] PHP：PDO 连接
来源：http://prl.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jcp.nwbrower.top

[U69] PHP：PDO 预处理
来源：http://grd.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ugz.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://njx.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rvo.yueranfly.top

[U71] PHP：抛出异常
来源：http://nnt.yj202588.top

throw new RuntimeException("失败", 500);
来源：http://qyq.daxiang520.top

[U72] PHP：写错误日志
来源：http://iun.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://etf.316326.xyz

[U73] PHP：读取 ini 配置
来源：http://tvb.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://vcf.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://iie.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://prc.vqdsnc.cn

[U75] PHP：依赖注入
来源：http://opc.gogol.net.cn

composer require psr/container
来源：http://vtn.52xcode.cn

[U76] PHP：简单路由
来源：http://xxa.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nmz.xingfuxueyuan.xyz

[U77] PHP：模板渲染
来源：http://gsm.guannengcc.top

composer require twig/twig
来源：http://ntg.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://vax.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://hxg.c1oappe.top

[U79] PHP：静态分析
来源：http://cvs.yj202588.top

composer require --dev phpstan/phpstan
来源：http://zym.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://ufv.yj202588.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://vvs.svipenyu.cn

[U81] JS：初始化项目
来源：http://nsd.jinqigufen.top

npm init -y;  npm i express
来源：http://kpx.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://feu.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uns.yj202588.top

[U83] JS：ES Module 导入导出
来源：http://kzb.zhixingplan.top

export const a = 1;  import { a } from "./m.js";
来源：http://pwx.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://ksl.chenlongwang.top

module.exports = { a };  const { a } = require("./m");
来源：http://dzx.hfpthk.cn

[U85] JS：可选链
来源：http://tif.haohaochexian.top

a?.b?.c
来源：http://hba.cucudq.cn

[U86] JS：空值合并
来源：http://pnp.yj20258888.top

a ?? b
来源：http://kzc.mhx1999.top

[U87] JS：解构默认值
来源：http://lsk.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://bcf.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://oyu.vehdjk.com

{ ...a, ...b }
来源：http://rmi.nanxinkj.top

[U89] JS：数组去重
来源：http://dij.iojbl.cn

[...new Set(arr)]
来源：http://wxg.wangdashe.top

[U90] JS：数字数组排序
来源：http://yrg.ydzc1.top

[...arr].sort((a, b) => a - b)
来源：http://fkk.haohaochexian.top

[U91] JS：对象键值遍历
来源：http://mmc.xziqi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zjf.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://zcm.316326.xyz

structuredClone(obj)
来源：http://ltz.yj202588.top

[U93] JS：模板字符串
来源：http://ppu.mhx1999.top

`共 ${n} 条`
来源：http://dpm.uphjek.com

[U94] JS：箭头函数
来源：http://zyq.hammf.cn

const double = x => x * 2;
来源：http://ekm.shangyingyoupin.top

[U95] JS：Promise 包装
来源：http://twa.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://fni.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://hhe.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://noj.cheryme.top

[U97] JS：并发请求
来源：http://esy.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvw.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://lih.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pks.hnqzz.top

[U99] JS：事件监听
来源：http://ggf.zhijiandao.cn

el.addEventListener("click", e => {})
来源：http://dpo.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://xxw.pycfn.com

document.querySelector(".item")
来源：http://umm.xuetiantiany.cn

[U101] JS：classList 操作
来源：http://zve.hammf.cn

el.classList.toggle("active")
来源：http://kns.svipenyu.cn

[U102] JS：本地存储
来源：http://uqd.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://chu.ybcxt.top

[U103] JS：定时器
来源：http://lxz.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xyt.daxiang520.top

[U104] JS：防抖
来源：http://fcn.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzn.yj20258888.top

[U105] JS：节流
来源：http://rbp.vehdjk.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yvv.jiagoushi.top

[U106] JS：日期格式化
来源：http://fue.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tta.zhixingplan.top

[U107] JS：数字千分位
来源：http://bpk.nanxinkj.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zzh.bbcook.cn

[U108] JS：随机整数
来源：http://kll.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ntb.yfazqb.com

[U109] JS：数组分组
来源：http://mkn.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://ikg.jinqigufen.top

[U110] JS：数组分块
来源：http://ebm.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nfr.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://zzf.jiagoushi.top

new Map(Object.entries(obj))
来源：http://zwc.dianchejie.cn

[U112] JS：字符串补位
来源：http://pvx.xuanzx.com

"7".padStart(3, "0")
来源：http://dgr.guowangkeji.top

[U113] JS：正则替换全部
来源：http://ijp.sweek.top

s.replaceAll("a", "b")
来源：http://tgy.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://zps.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://grx.cucudq.cn

[U115] JS：生成 UUID
来源：http://gns.hfpthk.cn

crypto.randomUUID()
来源：http://lgz.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://ugv.cashguo.top

/** @param {string} name */ function f(name) {}
来源：http://nhl.vqdsnc.cn

[U117] JS：单元测试
来源：http://csd.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://bhp.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://jdh.uphjek.com

npm i -D vite;  npx vite
来源：http://uqa.svipenyu.cn

[U119] JS：生产构建
来源：http://zni.52xcode.cn

npx vite build
来源：http://akg.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://khj.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://ion.dashuyun.cn

================================================================================
来源：http://npf.tian-w.cn

统计汇总
来源：http://vmb.daria6918.cn

================================================================================
来源：http://vod.guowangkeji.top

按语言统计（条）：
来源：http://chi.zdqjudy.top

Python ......... 252
来源：http://rjr.zdbjq.cn

PHP ............ 252
来源：http://ibi.guowangkeji.top

JavaScript ..... 252
来源：http://bly.chenzaomai.com

TypeScript ..... 212
来源：http://tyu.yonumen.top

Java ........... 212
来源：http://fbg.fanxiaobao.xyz

Go ............. 212
来源：http://wvo.aibaodan.cn

Ruby ........... 212
来源：http://ctx.dashuyun.cn

C# ............. 212
来源：http://jqj.smart0.xyz

C .............. 30
来源：http://jac.zdqjudy.top

C++ ............ 30
来源：http://cmw.hywenlv.cn

SQL ............ 90
来源：http://viu.yvedp.cn

Bash ........... 80
来源：http://vwh.ehwqpu.com

Kotlin ......... 15
来源：http://ipn.tanke756.top

Swift .......... 15
来源：http://jty.chenlongwang.top

Lua ............ 10
来源：http://bvf.gzhubu.top

Perl ........... 10
来源：http://qcx.quarkkingdee.top

Scala .......... 10
来源：http://cyk.jyoumei.cn

------------------------------------
来源：http://byn.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://fau.xuetiantiany.cn

按章节统计：
来源：http://kgk.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://caf.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tlg.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ldy.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pmw.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ejv.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hjn.ywan-chungtsiang.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://spb.shuidangran.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aow.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bpt.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tqg.ydzc1.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bkd.jinqigufen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rfn.chenzaomai.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kuc.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uin.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://epy.bjfxy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://coy.wangshuangyany.cn

Q SQL 专题                              90
来源：http://tju.jinqigfzy.top

R Bash 专题                             80
来源：http://kkp.gogol.net.cn

S C / C++ 专题                          60
来源：http://qqv.jiagoushi.top

T 其他语言补充                          60
来源：http://zyp.fzhhl.top

U 高频实用片段                         120
来源：http://fvi.vqdsnc.cn

------------------------------------
来源：http://bzc.jqgfzy.top

合计                                  2106 条
来源：http://tgv.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://ykt.zdqjudy.top

使用提醒
来源：http://kvf.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://kts.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bgj.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yta.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hbj.haohaochexian.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ams.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hpt.jinqigufen.top

—— 文件结束 ——
来源：http://bcz.uphjek.com


<!-- 参考信息 -->