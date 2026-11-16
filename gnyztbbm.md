代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://jon.cdnleiting.top

[T59] Scala：循环
来源：http://slz.zdbjq.cn

for (i <- 1 to 10) println(i)
来源：http://xkf.hnxiangtu.top

[T60] Scala：折叠
来源：http://szm.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ecj.0kj1m.cn

================================================================================
来源：http://ajm.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://izm.hnxiangtu.top

================================================================================
来源：http://lzq.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://fql.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://zda.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://nfx.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nko.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://ryc.cucudq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yjc.yj20258.top

[U04] Py：变量调试打印
来源：http://rhz.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zoa.sxryk.cn

[U05] Py：列表去重且保序
来源：http://bwa.mhx1999.top

list(dict.fromkeys(arr))
来源：http://coh.havefunace.top

[U06] Py：合并两个字典
来源：http://mbi.wangdashe.top

{**a, **b}
来源：http://uwn.hywenlv.cn

[U07] Py：反转字典键值
来源：http://cqh.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://uli.daxiang520.top

[U08] Py：展平二维列表
来源：http://rej.meibo888.top

[y for x in nested for y in x]
来源：http://tmb.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://cfr.gzhubu.top

max(d, key=d.get)
来源：http://xue.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://imu.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yyt.mhx1999.top

[U11] Py：生成器表达式
来源：http://rxc.guannengcc.top

(x * 2 for x in arr)
来源：http://mqo.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://apt.tarul.cn

Counter(arr).most_common(3)
来源：http://rnt.svipenyu.cn

[U13] Py：固定长度队列
来源：http://trn.jinqigufen.top

deque(maxlen=10)
来源：http://vxy.andypj.xyz

[U14] Py：分组收集到列表
来源：http://imd.yfazqb.com

defaultdict(list)
来源：http://ojs.zdbjq.cn

[U15] Py：高精度计时
来源：http://lgt.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://blo.52xcode.cn

[U16] Py：命令行参数解析
来源：http://eqb.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwv.vehdjk.com

[U17] Py：初始化日志
来源：http://jhj.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://lye.xingfuxueyuan.xyz

[U18] Py：预编译正则
来源：http://wut.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://lyi.aizwys.cn

[U19] Py：正则替换带回调
来源：http://ghk.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dvw.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://xqi.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://alb.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://bwc.tarul.cn

@contextlib.contextmanager
来源：http://jyj.xuanzx.com

[U22] Py：矩阵转置
来源：http://hry.svipenyu.cn

list(zip(*m))
来源：http://oun.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://ujs.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ynu.hnxiangtu.top

[U24] Py：路径操作
来源：http://oho.shanyushiyangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fyo.yangfankeji.com

[U25] Py：CSV 按字典读
来源：http://sem.hcnkem.com

csv.DictReader(f)
来源：http://uho.daria6918.cn

[U26] Py：并发下载
来源：http://cpx.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qij.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://keh.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://anr.cashguo.top

[U28] Py：类型别名
来源：http://ylh.0kj1m.cn

UserId = int
来源：http://vok.yuxming.cn

[U29] Py：属性校验
来源：http://vhj.jqgfzy.top

@property 与 @x.setter 配合
来源：http://zdk.yfazqb.com

[U30] Py：数据类
来源：http://krh.yangfankeji.com

@dataclass(slots=True)
来源：http://gok.gogol.net.cn

[U31] Py：单测
来源：http://mvp.vehdjk.com

python -m pytest -q
来源：http://dca.hysaishi.cn

[U32] Py：代码格式化
来源：http://hdj.ybcxt.top

ruff format . && ruff check --fix .
来源：http://cfs.fengsongda.top

[U33] Py：打包发布
来源：http://dyl.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://rgz.gaohongyu789.top

[U34] Py：判断编码
来源：http://dor.zdqjudy.top

chardet.detect(raw)
来源：http://oor.smart0.xyz

[U35] Py：发送邮件
来源：http://jjt.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://upw.fzhhl.top

[U36] Py：定时任务
来源：http://jer.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://bjf.dashuyun.cn

[U37] Py：读写 Excel
来源：http://hwn.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://onq.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://qtx.ybcxt.top

Path(__file__).resolve().parent
来源：http://paa.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://ejn.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://pdj.mhx1999.top

[U40] Py：打印到标准错误
来源：http://kba.uphjek.com

print("err", file=sys.stderr)
来源：http://mle.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://iin.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tsq.sweek.top

[U42] PHP：PSR-4 自动加载
来源：http://onp.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aor.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://feo.iojbl.cn

namespace App\Http;
来源：http://cfc.epnwcf.com

[U44] PHP：开启严格类型
来源：http://pfb.shanyushiyangtech.top

declare(strict_types=1);
来源：http://jrx.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://kcp.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yrs.xuanzx.com

[U46] PHP：可空类型
来源：http://uzt.yvedp.cn

?string $name = null
来源：http://qxu.xingfuxueyuan.xyz

[U47] PHP：联合类型
来源：http://owq.hesvh.cn

int|string $id
来源：http://bvx.nanxinkj.top

[U48] PHP：纯枚举
来源：http://upi.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fkw.smart0.xyz

[U49] PHP：只读属性
来源：http://bms.shangyingyoupin.top

public readonly string $name
来源：http://ieg.yj20258.top

[U50] PHP：构造器属性提升
来源：http://cqw.jinqigufen.top

public function __construct(private int $id) {}
来源：http://pbc.xziqi.cn

[U51] PHP：数组解构
来源：http://tsw.cdnleiting.top

[$a, $b] = $arr;
来源：http://vuu.zdbjq.cn

[U52] PHP：箭头函数
来源：http://fyr.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://elw.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://xbw.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://txd.hesvh.cn

[U54] PHP：空安全调用
来源：http://vsy.nanxinkj.top

$obj?->method()
来源：http://znk.zhengqikj.top

[U55] PHP：match 表达式
来源：http://ouw.zhoulong.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lwg.hammf.cn

[U56] PHP：命名参数
来源：http://egk.birdmap.top

f(a: 1, b: 2)
来源：http://pgv.sysykeji.top

[U57] PHP：字符串插值
来源：http://ntj.gzhubu.top

"值: {$a}"
来源：http://tid.fengsongda.top

[U58] PHP：数组三件套
来源：http://vzs.shanyushiyangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zgu.hnqzz.top

[U59] PHP：自定义排序
来源：http://hyr.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tix.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://uwt.meibo888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tlf.hammf.cn

[U61] PHP：正则
来源：http://gpr.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eft.bjfxy.top

[U62] PHP：日期对象
来源：http://llj.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ykw.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://lmx.hongshengwenyu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://slo.aibaodan.cn

[U64] PHP：目录遍历
来源：http://lri.tian-w.cn

glob("dir/*.php");  scandir("dir");
来源：http://hfk.tarul.cn

[U65] PHP：会话
来源：http://rqc.ydzc1.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lzd.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://azp.yuxming.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vrs.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://fmo.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ktz.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://lon.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ouu.yueranfly.top

[U69] PHP：PDO 预处理
来源：http://hnp.yongpay.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vfr.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://fnx.0kj1m.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lht.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://hgc.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://ozb.0kj1m.cn

[U72] PHP：写错误日志
来源：http://lge.havefunace.top

error_log("失败: " . $e->getMessage());
来源：http://sgj.guowangkeji.top

[U73] PHP：读取 ini 配置
来源：http://lhq.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://fet.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://vym.jyoumei.cn

getenv("APP_ENV") ?: "production"
来源：http://jde.yvedp.cn

[U75] PHP：依赖注入
来源：http://ouw.hnxiangtu.top

composer require psr/container
来源：http://vsr.yj202588.top

[U76] PHP：简单路由
来源：http://wcw.daria6918.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pih.jianghu66.top

[U77] PHP：模板渲染
来源：http://snb.tarul.cn

composer require twig/twig
来源：http://zmj.dianchejie.cn

[U78] PHP：单元测试
来源：http://ghh.fzhhl.top

composer require --dev phpunit/phpunit
来源：http://oka.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://fnw.bjfxy.top

composer require --dev phpstan/phpstan
来源：http://mis.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://ajy.hnxiangtu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nui.zhixingplan.top

[U81] JS：初始化项目
来源：http://rkp.zhoulong.xyz

npm init -y;  npm i express
来源：http://nrh.daxiang520.top

[U82] JS：package.json 脚本
来源：http://khs.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hde.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://tbu.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://axs.guowangkeji.top

[U84] JS：CommonJS 写法
来源：http://clt.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://tpp.aizwys.cn

[U85] JS：可选链
来源：http://qmb.vehdjk.com

a?.b?.c
来源：http://yjq.gaohongyu789.top

[U86] JS：空值合并
来源：http://fgx.hfpthk.cn

a ?? b
来源：http://gts.ivvv.top

[U87] JS：解构默认值
来源：http://mhs.yuanzhike.top

const { a = 1, b = 2 } = obj;
来源：http://mej.jyoumei.cn

[U88] JS：对象展开合并
来源：http://mmz.chenlongwang.top

{ ...a, ...b }
来源：http://par.wangdashe.top

[U89] JS：数组去重
来源：http://usn.zhoulong.xyz

[...new Set(arr)]
来源：http://hjq.fzhhl.top

[U90] JS：数字数组排序
来源：http://gwb.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://vrx.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://zpy.birdmap.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://etj.fktsv.cn

[U92] JS：深拷贝
来源：http://nsv.gotoacloud.top

structuredClone(obj)
来源：http://tqr.zhengqikj.top

[U93] JS：模板字符串
来源：http://mrl.hnxiangtu.top

`共 ${n} 条`
来源：http://zza.sjlbkw.cn

[U94] JS：箭头函数
来源：http://plx.zhiwuduotai.top

const double = x => x * 2;
来源：http://reg.yonumen.top

[U95] JS：Promise 包装
来源：http://ukb.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://taa.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://sxl.chenjidiqi.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ozw.bbcook.cn

[U97] JS：并发请求
来源：http://vpc.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mkd.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://jam.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dxa.tanke756.top

[U99] JS：事件监听
来源：http://qfk.xylfe.cn

el.addEventListener("click", e => {})
来源：http://nai.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://wwh.zycfv.cn

document.querySelector(".item")
来源：http://uym.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://ddk.meibo888.top

el.classList.toggle("active")
来源：http://och.jyoumei.cn

[U102] JS：本地存储
来源：http://vwd.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://zbe.fzhhl.top

[U103] JS：定时器
来源：http://ubq.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ekb.redwolf501.top

[U104] JS：防抖
来源：http://kpo.sweek.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvq.yuxming.cn

[U105] JS：节流
来源：http://pjs.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pqh.chenzaomai.com

[U106] JS：日期格式化
来源：http://zty.vqdsnc.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://frc.vehdjk.com

[U107] JS：数字千分位
来源：http://jzz.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://okm.xylfe.cn

[U108] JS：随机整数
来源：http://rtb.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ztn.yonumen.top

[U109] JS：数组分组
来源：http://lty.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://rsh.jyoumei.cn

[U110] JS：数组分块
来源：http://gig.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tde.feifeiyinyue.top

[U111] JS：对象转 Map
来源：http://crk.fzhhl.top

new Map(Object.entries(obj))
来源：http://oeb.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://nxo.ehwqpu.com

"7".padStart(3, "0")
来源：http://vty.nanxinkj.top

[U113] JS：正则替换全部
来源：http://ewo.fzhhl.top

s.replaceAll("a", "b")
来源：http://jpr.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://laa.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://qdv.jiagoushi.top

[U115] JS：生成 UUID
来源：http://ftq.cqqwz.cn

crypto.randomUUID()
来源：http://qgf.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://zul.316326.xyz

/** @param {string} name */ function f(name) {}
来源：http://kib.xziqi.cn

[U117] JS：单元测试
来源：http://ags.shangyingyoupin.top

npm i -D vitest;  npx vitest
来源：http://nyv.bbcook.cn

[U118] JS：开发服务器
来源：http://boi.sufxvd.cn

npm i -D vite;  npx vite
来源：http://fwf.yongpay.top

[U119] JS：生产构建
来源：http://kbc.daria6918.cn

npx vite build
来源：http://mee.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://dmo.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://oeo.ybcxt.top

================================================================================
来源：http://zqn.sxryk.cn

统计汇总
来源：http://xkm.zdqjudy.top

================================================================================
来源：http://pzg.andypj.xyz

按语言统计（条）：
来源：http://fdi.shanyushiyangtech.top

Python ......... 252
来源：http://vbh.sxryk.cn

PHP ............ 252
来源：http://hpv.zhengqikj.top

JavaScript ..... 252
来源：http://arx.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://gfk.hongshengwenyu.top

Java ........... 212
来源：http://nlr.gotoacloud.top

Go ............. 212
来源：http://tqj.smart0.xyz

Ruby ........... 212
来源：http://sdj.bbcook.cn

C# ............. 212
来源：http://mtt.andypj.xyz

C .............. 30
来源：http://fdi.bbcook.cn

C++ ............ 30
来源：http://cet.shanyushiyangkeji.top

SQL ............ 90
来源：http://fpb.hnqzz.top

Bash ........... 80
来源：http://rgo.bbcook.cn

Kotlin ......... 15
来源：http://ngk.iojbl.cn

Swift .......... 15
来源：http://moz.fengsongda.top

Lua ............ 10
来源：http://mcr.shuidangran.top

Perl ........... 10
来源：http://rmb.hcnkem.com

Scala .......... 10
来源：http://izf.haohaochexian.top

------------------------------------
来源：http://ghx.bjfxy.top

合计 ........... 2106 条
来源：http://beu.daxiang520.top

按章节统计：
来源：http://xbr.chenjidiqi.icu

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://osg.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gxp.pengpengdd.cyou

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fbh.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://csg.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lfd.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rsy.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kfc.gzhubu.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ive.dashuyun.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://doc.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wxp.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://phl.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rit.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://edh.hnqzz.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aur.fengsongda.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qho.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://whv.zhoulong.xyz

Q SQL 专题                              90
来源：http://soe.jiagoushi.top

R Bash 专题                             80
来源：http://wpp.nwbrower.top

S C / C++ 专题                          60
来源：http://vzn.bjfxy.top

T 其他语言补充                          60
来源：http://gvy.zycfv.cn

U 高频实用片段                         120
来源：http://ylk.birdmap.top

------------------------------------
来源：http://sxd.gzhubu.top

合计                                  2106 条
来源：http://ibx.bbcook.cn

--------------------------------------------------------------------------------
来源：http://air.jinyuanbaomall.cn

使用提醒
来源：http://nsc.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://vhf.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://spe.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pps.hammf.cn


<!-- 参考信息 -->