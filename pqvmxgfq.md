代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://ydd.sweek.top

[T55] Scala：集合过滤
来源：http://ali.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://sgr.jianghu66.top

[T56] Scala：样例类
来源：http://zft.xziqi.cn

case class User(name: String, age: Int)
来源：http://qcf.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://acw.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tub.yj20258888.top

[T58] Scala：函数定义
来源：http://kwj.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://ysg.0kj1m.cn

[T59] Scala：循环
来源：http://qfy.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://quz.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://bne.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://svd.ywan-chungtsiang.top

================================================================================
来源：http://oae.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aeg.yvedp.cn

================================================================================
来源：http://fct.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://iyt.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://rwg.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://qfv.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqn.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://amn.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://two.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://pfm.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ooz.epnwcf.com

[U05] Py：列表去重且保序
来源：http://mpd.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://neq.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://sbx.xingfuxueyuan.xyz

{**a, **b}
来源：http://mub.xuanzx.com

[U07] Py：反转字典键值
来源：http://dst.sxryk.cn

{v: k for k, v in d.items()}
来源：http://zsr.yonumen.top

[U08] Py：展平二维列表
来源：http://ywg.svipenyu.cn

[y for x in nested for y in x]
来源：http://ifp.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://vva.nanxinkj.top

max(d, key=d.get)
来源：http://gqx.bjfxy.top

[U10] Py：按值排序字典
来源：http://plx.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ejh.ctjpmb.com

[U11] Py：生成器表达式
来源：http://wcv.svipenyu.cn

(x * 2 for x in arr)
来源：http://tfl.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://nsv.vehdjk.com

Counter(arr).most_common(3)
来源：http://emh.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://nml.uphjek.com

deque(maxlen=10)
来源：http://pnq.epnwcf.com

[U14] Py：分组收集到列表
来源：http://dcy.hysaishi.cn

defaultdict(list)
来源：http://qpn.vqdsnc.cn

[U15] Py：高精度计时
来源：http://uib.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://xtn.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://xsp.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qqy.gaohongyu789.top

[U17] Py：初始化日志
来源：http://hgh.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://ssc.ehwqpu.com

[U18] Py：预编译正则
来源：http://fem.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://ytu.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://drg.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wpo.tian-w.cn

[U20] Py：缓存函数结果
来源：http://iqg.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://ylj.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://gvj.daria6918.cn

@contextlib.contextmanager
来源：http://anb.aizwys.cn

[U22] Py：矩阵转置
来源：http://fss.wangdashe.top

list(zip(*m))
来源：http://jwx.hammf.cn

[U23] Py：分块读取大文件
来源：http://syo.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lym.sysykeji.top

[U24] Py：路径操作
来源：http://zva.ydzc1.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tsy.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://imp.fzhhl.top

csv.DictReader(f)
来源：http://obr.daxiang520.top

[U26] Py：并发下载
来源：http://fef.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qrj.yvedp.cn

[U27] Py：异步 HTTP
来源：http://vkx.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://fhh.hesvh.cn

[U28] Py：类型别名
来源：http://nre.daxiang520.top

UserId = int
来源：http://kjg.yongpay.top

[U29] Py：属性校验
来源：http://vdc.xinyue.icu

@property 与 @x.setter 配合
来源：http://bug.gaohongyu789.top

[U30] Py：数据类
来源：http://tet.dashuyun.cn

@dataclass(slots=True)
来源：http://fel.bjfxy.top

[U31] Py：单测
来源：http://stj.yueranfly.top

python -m pytest -q
来源：http://aio.nanxuanxn.top

[U32] Py：代码格式化
来源：http://nty.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://ijl.tarul.cn

[U33] Py：打包发布
来源：http://dfs.sufxvd.cn

python -m build  （依赖 pyproject.toml）
来源：http://dhw.cashguo.top

[U34] Py：判断编码
来源：http://ric.sjlbkw.cn

chardet.detect(raw)
来源：http://cfw.ivvv.top

[U35] Py：发送邮件
来源：http://hlu.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ecm.yanxiufei.cn

[U36] Py：定时任务
来源：http://gom.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://xqx.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://xpv.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mif.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://fll.jyoumei.cn

Path(__file__).resolve().parent
来源：http://blp.chenlongwang.top

[U39] Py：判断是否在交互环境
来源：http://mms.zhoulong.xyz

sys.stdout.isatty()
来源：http://iib.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://qcz.dashuyun.cn

print("err", file=sys.stderr)
来源：http://mbn.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://sco.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xke.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://dam.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dch.c1oappe.top

[U43] PHP：声明命名空间
来源：http://ixe.fktsv.cn

namespace App\Http;
来源：http://ihw.quarkkingdee.top

[U44] PHP：开启严格类型
来源：http://fly.sweek.top

declare(strict_types=1);
来源：http://fby.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://ydb.sjlbkw.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qrv.yuanzhike.top

[U46] PHP：可空类型
来源：http://hto.andypj.xyz

?string $name = null
来源：http://qgf.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://pte.tian-w.cn

int|string $id
来源：http://aqv.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://cim.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xlj.zdbjq.cn

[U49] PHP：只读属性
来源：http://lgm.fzhhl.top

public readonly string $name
来源：http://sro.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://mrv.hcnkem.com

public function __construct(private int $id) {}
来源：http://cuo.yuxming.cn

[U51] PHP：数组解构
来源：http://ekk.sxryk.cn

[$a, $b] = $arr;
来源：http://gqy.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://hlc.uphjek.com

$double = fn($x) => $x * 2;
来源：http://xam.hfpthk.cn

[U53] PHP：空合并运算符
来源：http://ody.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://kuo.yuanzhike.top

[U54] PHP：空安全调用
来源：http://pdy.ivvv.top

$obj?->method()
来源：http://xfu.tian-w.cn

[U55] PHP：match 表达式
来源：http://fuo.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsi.jlsjyb.cn

[U56] PHP：命名参数
来源：http://pdp.birdmap.top

f(a: 1, b: 2)
来源：http://kui.bbcook.cn

[U57] PHP：字符串插值
来源：http://wga.gogol.net.cn

"值: {$a}"
来源：http://rsx.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://ego.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ktk.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://hui.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://scn.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://xfr.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oaz.mhx1999.top

[U61] PHP：正则
来源：http://qky.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tfw.nwbrower.top

[U62] PHP：日期对象
来源：http://yfp.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://piw.316326.xyz

[U63] PHP：文件读写
来源：http://vqi.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hta.gotoacloud.top

[U64] PHP：目录遍历
来源：http://pdn.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://luz.jinghuilouyu.cn

[U65] PHP：会话
来源：http://liz.shuidangran.top

session_start();  $_SESSION["uid"] = 1;
来源：http://khf.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://mdf.jiagoushi.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ksh.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://yoy.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://viw.ydjk.org.cn

[U68] PHP：PDO 连接
来源：http://njx.nanxinkj.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mwb.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://qhe.zdqjudy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kma.yj202588.top

[U70] PHP：PDO 事务
来源：http://ieh.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aix.fengsongda.top

[U71] PHP：抛出异常
来源：http://tmp.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://vmn.birdmap.top

[U72] PHP：写错误日志
来源：http://evt.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://mvt.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://okp.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://btk.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://sfy.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://yos.fengsongda.top

[U75] PHP：依赖注入
来源：http://nuc.yuanzhike.top

composer require psr/container
来源：http://bjd.cqqwz.cn

[U76] PHP：简单路由
来源：http://guw.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lmj.guannengcc.top

[U77] PHP：模板渲染
来源：http://gar.zhoulong.xyz

composer require twig/twig
来源：http://ver.gzhubu.top

[U78] PHP：单元测试
来源：http://mdi.havefunace.top

composer require --dev phpunit/phpunit
来源：http://opa.fehbvm.com

[U79] PHP：静态分析
来源：http://uhh.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://imv.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://nla.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://nmf.xziqi.cn

[U81] JS：初始化项目
来源：http://jqn.gogol.net.cn

npm init -y;  npm i express
来源：http://szo.fktsv.cn

[U82] JS：package.json 脚本
来源：http://bzq.gotoacloud.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dhs.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://ugw.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lpu.cqqwz.cn

[U84] JS：CommonJS 写法
来源：http://feo.hnxiangtu.top

module.exports = { a };  const { a } = require("./m");
来源：http://hqa.jianghu66.top

[U85] JS：可选链
来源：http://xwr.cqqwz.cn

a?.b?.c
来源：http://fqx.hysaishi.cn

[U86] JS：空值合并
来源：http://fus.cdnleiting.top

a ?? b
来源：http://msz.wangdashe.top

[U87] JS：解构默认值
来源：http://pgw.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://ecm.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://dcy.shangyingyoupin.top

{ ...a, ...b }
来源：http://cff.nwbrower.top

[U89] JS：数组去重
来源：http://qcz.feifeiyinyue.top

[...new Set(arr)]
来源：http://cuh.yongpay.top

[U90] JS：数字数组排序
来源：http://kni.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://qfo.cashguo.top

[U91] JS：对象键值遍历
来源：http://ram.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gfi.xziqi.cn

[U92] JS：深拷贝
来源：http://czm.c1oappe.top

structuredClone(obj)
来源：http://gbc.ydzc1.top

[U93] JS：模板字符串
来源：http://ejh.zdbjq.cn

`共 ${n} 条`
来源：http://wvl.chenzaomai.com

[U94] JS：箭头函数
来源：http://lno.pengpengdd.cyou

const double = x => x * 2;
来源：http://fhh.zhengqikj.top

[U95] JS：Promise 包装
来源：http://icv.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://kqi.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://hxr.shzxlz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zdo.hammf.cn

[U97] JS：并发请求
来源：http://vig.cheryme.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://frt.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://ksy.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nff.jqgufenzy.top

[U99] JS：事件监听
来源：http://nci.tian-w.cn

el.addEventListener("click", e => {})
来源：http://bfy.zhixingplan.top

[U100] JS：DOM 查询
来源：http://hnv.epnwcf.com

document.querySelector(".item")
来源：http://wwl.zhijiandao.cn

[U101] JS：classList 操作
来源：http://spb.jinyuanbaomall.cn

el.classList.toggle("active")
来源：http://hyq.yanxiufei.cn

[U102] JS：本地存储
来源：http://ugs.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aod.aizwys.cn

[U103] JS：定时器
来源：http://ikq.ctjpmb.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kjt.feifeiyinyue.top

[U104] JS：防抖
来源：http://kox.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycz.yj202588.top

[U105] JS：节流
来源：http://oyn.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gfx.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://izf.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ltl.wangdashe.top

[U107] JS：数字千分位
来源：http://ult.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nia.xuanzx.com

[U108] JS：随机整数
来源：http://yjs.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dql.gogol.net.cn

[U109] JS：数组分组
来源：http://ziz.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://vae.shangyingyoupin.top

[U110] JS：数组分块
来源：http://wys.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fqn.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://hwm.cqqwz.cn

new Map(Object.entries(obj))
来源：http://wse.snrcjt.cn

[U112] JS：字符串补位
来源：http://xog.redwolf501.top

"7".padStart(3, "0")
来源：http://isx.guowangkeji.top

[U113] JS：正则替换全部
来源：http://rxc.cheryme.top

s.replaceAll("a", "b")
来源：http://jml.cqqwz.cn

[U114] JS：JSON 深比较
来源：http://pur.shanyushiyangkeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ypq.ybcxt.top

[U115] JS：生成 UUID
来源：http://vin.hnqzz.top

crypto.randomUUID()
来源：http://ohl.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://byy.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://agg.chenjidiqi.icu

[U117] JS：单元测试
来源：http://xqv.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://rzx.0kj1m.cn

[U118] JS：开发服务器
来源：http://iic.gogol.net.cn

npm i -D vite;  npx vite
来源：http://yru.fzhhl.top

[U119] JS：生产构建
来源：http://sqz.hnxiangtu.top

npx vite build
来源：http://bfp.zhiwuduotai.top

[U120] JS：读取环境变量（Vite）
来源：http://ikb.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://hzs.bbcook.cn

================================================================================
来源：http://cjq.xylfe.cn

统计汇总
来源：http://uhq.feifeiyinyue.top

================================================================================
来源：http://dfu.tanke756.top

按语言统计（条）：
来源：http://kvb.yuxming.cn

Python ......... 252
来源：http://xhq.pengpengdd.cyou

PHP ............ 252
来源：http://iag.yonumen.top

JavaScript ..... 252
来源：http://qtt.yuanzhike.top

TypeScript ..... 212
来源：http://osq.epnwcf.com

Java ........... 212
来源：http://djq.kuanghao11.cn

Go ............. 212
来源：http://wso.gotoacloud.top

Ruby ........... 212
来源：http://myi.gzhubu.top

C# ............. 212
来源：http://alg.ehwqpu.com

C .............. 30
来源：http://rbm.zhoulong.xyz

C++ ............ 30
来源：http://toy.zhaomingkeji.xyz

SQL ............ 90
来源：http://mdc.zhiwuduotai.top

Bash ........... 80
来源：http://tlt.jqgufenzy.top

Kotlin ......... 15
来源：http://kij.kuanghao11.cn

Swift .......... 15
来源：http://wwr.dianchejie.cn

Lua ............ 10
来源：http://vqa.redwolf501.top

Perl ........... 10
来源：http://eaj.nanxinkj.top

Scala .......... 10
来源：http://vfl.9152youxi.cn

------------------------------------
来源：http://fmp.ctjpmb.com

合计 ........... 2106 条
来源：http://pro.c1oappe.top

按章节统计：
来源：http://fcw.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lxr.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ehw.zdbjq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://axw.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xvv.ydzc1.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pmp.meibo888.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rgl.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nct.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qes.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xza.bbcook.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://stw.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dwi.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ypp.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hko.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tmz.ctjpmb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yhn.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gwp.quarkkingdee.top

Q SQL 专题                              90
来源：http://jpb.uphjek.com

R Bash 专题                             80
来源：http://aff.ppjwa.cn

S C / C++ 专题                          60
来源：http://wlp.daria6918.cn

T 其他语言补充                          60
来源：http://gfv.kuanghao11.cn


<!-- 参考信息 -->