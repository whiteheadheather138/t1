代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://jmu.hywenlv.cn

[T55] Scala：集合过滤
来源：http://osu.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://soo.hongshengwenyu.top

[T56] Scala：样例类
来源：http://uhb.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://psb.cheryme.top

[T57] Scala：模式匹配
来源：http://rtn.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://suq.jqgufenzy.top

[T58] Scala：函数定义
来源：http://gbj.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://qjp.nanxuanxn.top

[T59] Scala：循环
来源：http://iyv.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://rra.ehwqpu.com

[T60] Scala：折叠
来源：http://kqt.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vuy.svipenyu.cn

================================================================================
来源：http://zbc.uphjek.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ycd.hesvh.cn

================================================================================
来源：http://kvn.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://dvv.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://gro.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://nqb.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jum.yonumen.top

[U03] Py：加载 .env 配置
来源：http://vsp.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cid.hfpthk.cn

[U04] Py：变量调试打印
来源：http://wij.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://plk.c1oappe.top

[U05] Py：列表去重且保序
来源：http://zsf.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://gvc.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://tpg.guannengcc.top

{**a, **b}
来源：http://itd.sysykeji.top

[U07] Py：反转字典键值
来源：http://kpw.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://njt.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://isk.9152youxi.cn

[y for x in nested for y in x]
来源：http://baa.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://rpv.ehwqpu.com

max(d, key=d.get)
来源：http://msv.meibo888.top

[U10] Py：按值排序字典
来源：http://npb.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jzz.9152youxi.cn

[U11] Py：生成器表达式
来源：http://qcq.sufxvd.cn

(x * 2 for x in arr)
来源：http://rnq.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://azd.yfazqb.com

Counter(arr).most_common(3)
来源：http://hgu.bbcook.cn

[U13] Py：固定长度队列
来源：http://jmc.ydzc1.top

deque(maxlen=10)
来源：http://jkv.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://oex.aizwys.cn

defaultdict(list)
来源：http://rtr.yonumen.top

[U15] Py：高精度计时
来源：http://tjr.zhixingplan.top

t = time.perf_counter()
来源：http://lvk.316326.xyz

[U16] Py：命令行参数解析
来源：http://caz.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://utr.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://cpo.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://tpy.yangfankeji.com

[U18] Py：预编译正则
来源：http://pfm.zycfv.cn

pat = re.compile(r"\d+")
来源：http://dsm.wangdashe.top

[U19] Py：正则替换带回调
来源：http://vlz.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dmu.c1oappe.top

[U20] Py：缓存函数结果
来源：http://nem.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://lmd.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://crt.sxryk.cn

@contextlib.contextmanager
来源：http://bgt.yueranfly.top

[U22] Py：矩阵转置
来源：http://pwh.wangshuangyany.cn

list(zip(*m))
来源：http://skc.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://lzc.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gqr.zhiwuduotai.top

[U24] Py：路径操作
来源：http://yya.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jfs.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://amo.yj20258.top

csv.DictReader(f)
来源：http://tab.jqgfzy.top

[U26] Py：并发下载
来源：http://zby.jinyuanbaomall.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uzp.tarul.cn

[U27] Py：异步 HTTP
来源：http://fvj.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://dqp.bbcook.cn

[U28] Py：类型别名
来源：http://oqx.zhixingplan.top

UserId = int
来源：http://njc.gzhubu.top

[U29] Py：属性校验
来源：http://ogd.ehwqpu.com

@property 与 @x.setter 配合
来源：http://cmk.zhiwuduotai.top

[U30] Py：数据类
来源：http://xij.sjlbkw.cn

@dataclass(slots=True)
来源：http://pmj.xylfe.cn

[U31] Py：单测
来源：http://yyx.kuanghao11.cn

python -m pytest -q
来源：http://yhc.nanxuanxn.top

[U32] Py：代码格式化
来源：http://fqm.redwolf501.top

ruff format . && ruff check --fix .
来源：http://qwf.nanxinkj.top

[U33] Py：打包发布
来源：http://hjo.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://bsi.ybcxt.top

[U34] Py：判断编码
来源：http://jtp.ehwqpu.com

chardet.detect(raw)
来源：http://ano.dianchejie.cn

[U35] Py：发送邮件
来源：http://pbn.0kj1m.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tsw.fengsongda.top

[U36] Py：定时任务
来源：http://pkl.ydjk.org.cn

schedule.every(10).minutes.do(job)
来源：http://sxd.yueranfly.top

[U37] Py：读写 Excel
来源：http://ory.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mlc.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://zds.redwolf501.top

Path(__file__).resolve().parent
来源：http://hem.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://xqv.nwbrower.top

sys.stdout.isatty()
来源：http://bnj.xziqi.cn

[U40] Py：打印到标准错误
来源：http://cuw.0kj1m.cn

print("err", file=sys.stderr)
来源：http://cmg.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://lmi.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nmq.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://bjb.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gbm.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://shz.xuanzx.com

namespace App\Http;
来源：http://lsm.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://bjg.xuanzx.com

declare(strict_types=1);
来源：http://skv.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://ezr.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qtd.jqgufenzy.top

[U46] PHP：可空类型
来源：http://asf.yuxming.cn

?string $name = null
来源：http://doa.cheryme.top

[U47] PHP：联合类型
来源：http://hyp.vqdsnc.cn

int|string $id
来源：http://cul.nwbrower.top

[U48] PHP：纯枚举
来源：http://hgf.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ofs.tarul.cn

[U49] PHP：只读属性
来源：http://syj.pycfn.com

public readonly string $name
来源：http://efm.tian-w.cn

[U50] PHP：构造器属性提升
来源：http://iwb.0kj1m.cn

public function __construct(private int $id) {}
来源：http://aws.hammf.cn

[U51] PHP：数组解构
来源：http://lxk.andypj.xyz

[$a, $b] = $arr;
来源：http://jkn.yueranfly.top

[U52] PHP：箭头函数
来源：http://ufb.hongshengwenyu.top

$double = fn($x) => $x * 2;
来源：http://kwb.smart0.xyz

[U53] PHP：空合并运算符
来源：http://zzs.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://vas.epnwcf.com

[U54] PHP：空安全调用
来源：http://dpe.jlsjyb.cn

$obj?->method()
来源：http://epf.zhixingplan.top

[U55] PHP：match 表达式
来源：http://hyu.9152youxi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gqa.ppjwa.cn

[U56] PHP：命名参数
来源：http://zia.zhixingplan.top

f(a: 1, b: 2)
来源：http://psj.birdmap.top

[U57] PHP：字符串插值
来源：http://bqv.sufxvd.cn

"值: {$a}"
来源：http://pqz.birdmap.top

[U58] PHP：数组三件套
来源：http://beh.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bvb.fzhhl.top

[U59] PHP：自定义排序
来源：http://djt.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tph.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://ddj.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hwn.ivvv.top

[U61] PHP：正则
来源：http://prp.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jus.pycfn.com

[U62] PHP：日期对象
来源：http://rwj.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://loe.vehdjk.com

[U63] PHP：文件读写
来源：http://zcj.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aag.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://zfc.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://yzc.hywenlv.cn

[U65] PHP：会话
来源：http://sms.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rad.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://ije.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://brn.yfazqb.com

[U67] PHP：处理文件上传
来源：http://bib.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gnu.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://xcn.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uap.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://xnx.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tvq.mhx1999.top

[U70] PHP：PDO 事务
来源：http://xeh.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yys.cucudq.cn

[U71] PHP：抛出异常
来源：http://pfy.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://lub.yuanzhike.top

[U72] PHP：写错误日志
来源：http://txn.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://sdk.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://hrq.hongshengwenyu.top

parse_ini_file("config.ini", true)
来源：http://dqy.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://zdv.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://cxx.daxiang520.top

[U75] PHP：依赖注入
来源：http://wkh.xziqi.cn

composer require psr/container
来源：http://ajk.fzhhl.top

[U76] PHP：简单路由
来源：http://oln.ehwqpu.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gxr.sysykeji.top

[U77] PHP：模板渲染
来源：http://qcy.ehwqpu.com

composer require twig/twig
来源：http://svm.sysykeji.top

[U78] PHP：单元测试
来源：http://lpu.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://znm.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://bji.tarul.cn

composer require --dev phpstan/phpstan
来源：http://lrw.ybcxt.top

[U80] PHP：代码规范修复
来源：http://kti.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aep.hysaishi.cn

[U81] JS：初始化项目
来源：http://oms.sjlbkw.cn

npm init -y;  npm i express
来源：http://ypy.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://ppa.jinyuanbaomall.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wrb.jinyuanbaomall.cn

[U83] JS：ES Module 导入导出
来源：http://agp.zycfv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cpq.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://ogd.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://gjn.sysykeji.top

[U85] JS：可选链
来源：http://zdy.redwolf501.top

a?.b?.c
来源：http://ffn.gotoacloud.top

[U86] JS：空值合并
来源：http://nju.xziqi.cn

a ?? b
来源：http://vun.yonumen.top

[U87] JS：解构默认值
来源：http://xxn.dashuyun.cn

const { a = 1, b = 2 } = obj;
来源：http://szs.yj20258888.top

[U88] JS：对象展开合并
来源：http://rpe.yuanzhike.top

{ ...a, ...b }
来源：http://rqo.gzhubu.top

[U89] JS：数组去重
来源：http://htq.xuanzx.com

[...new Set(arr)]
来源：http://mpf.guowangkeji.top

[U90] JS：数字数组排序
来源：http://wrs.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://knp.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://jik.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qyz.guowangkeji.top

[U92] JS：深拷贝
来源：http://ftk.epnwcf.com

structuredClone(obj)
来源：http://duj.redwolf501.top

[U93] JS：模板字符串
来源：http://pmy.shuidangran.top

`共 ${n} 条`
来源：http://eyu.tian-w.cn

[U94] JS：箭头函数
来源：http://etw.cucudq.cn

const double = x => x * 2;
来源：http://pix.fengsongda.top

[U95] JS：Promise 包装
来源：http://rmn.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://ieb.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://gpm.jqgufenzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sgk.cucudq.cn

[U97] JS：并发请求
来源：http://rma.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rvm.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://pxn.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://niz.chenlongwang.top

[U99] JS：事件监听
来源：http://pxk.tianlin.xyz

el.addEventListener("click", e => {})
来源：http://bah.aibaodan.cn

[U100] JS：DOM 查询
来源：http://dof.zhixingplan.top

document.querySelector(".item")
来源：http://scd.vehdjk.com

[U101] JS：classList 操作
来源：http://ysq.yuxming.cn

el.classList.toggle("active")
来源：http://cen.guowangkeji.top

[U102] JS：本地存储
来源：http://dhh.snrcjt.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nbd.fzhhl.top

[U103] JS：定时器
来源：http://kbi.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jmw.jianghu66.top

[U104] JS：防抖
来源：http://zma.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cks.bjfxy.top

[U105] JS：节流
来源：http://lvz.cheryme.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yie.gzhubu.top

[U106] JS：日期格式化
来源：http://kah.uphjek.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pnr.yvedp.cn

[U107] JS：数字千分位
来源：http://aix.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rgn.316326.xyz

[U108] JS：随机整数
来源：http://isw.zhixingplan.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fbk.meibo888.top

[U109] JS：数组分组
来源：http://ndf.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://msh.fengsongda.top

[U110] JS：数组分块
来源：http://hpf.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://amu.jlsjyb.cn

[U111] JS：对象转 Map
来源：http://nnh.hfpthk.cn

new Map(Object.entries(obj))
来源：http://irp.jlsjyb.cn

[U112] JS：字符串补位
来源：http://kmm.jlsjyb.cn

"7".padStart(3, "0")
来源：http://qej.zhiwuduotai.top

[U113] JS：正则替换全部
来源：http://ylm.zycfv.cn

s.replaceAll("a", "b")
来源：http://dhn.tianlin.xyz

[U114] JS：JSON 深比较
来源：http://wxf.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zoy.ybcxt.top

[U115] JS：生成 UUID
来源：http://mpo.nanxinkj.top

crypto.randomUUID()
来源：http://obw.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://tqy.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://dov.guannengcc.top

[U117] JS：单元测试
来源：http://frn.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://jzq.cucudq.cn

[U118] JS：开发服务器
来源：http://asv.uphjek.com

npm i -D vite;  npx vite
来源：http://lki.hammf.cn

[U119] JS：生产构建
来源：http://hyo.316326.xyz

npx vite build
来源：http://twl.shanyushiyangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://jwe.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://qgg.daria6918.cn

================================================================================
来源：http://jwr.smart0.xyz

统计汇总
来源：http://alx.zhongyouzk.top

================================================================================
来源：http://ldf.0kj1m.cn

按语言统计（条）：
来源：http://ems.zdqjudy.top

Python ......... 252
来源：http://cua.guowangkeji.top

PHP ............ 252
来源：http://cqk.hfpthk.cn

JavaScript ..... 252
来源：http://gvw.zhengqikj.top

TypeScript ..... 212
来源：http://mcc.jinqigfzy.top

Java ........... 212
来源：http://hzw.gogol.net.cn

Go ............. 212
来源：http://qdc.hongshengwenyu.top

Ruby ........... 212
来源：http://hfx.zdqjudy.top

C# ............. 212
来源：http://ekz.feifeiyinyue.top

C .............. 30
来源：http://gio.tarul.cn

C++ ............ 30
来源：http://bcu.uphjek.com

SQL ............ 90
来源：http://xki.meibo888.top

Bash ........... 80
来源：http://sfh.zhiwuduotai.top

Kotlin ......... 15
来源：http://aoq.cqqwz.cn

Swift .......... 15
来源：http://cat.uphjek.com

Lua ............ 10
来源：http://ioa.chenlongwang.top

Perl ........... 10
来源：http://rgn.daria6918.cn

Scala .......... 10
来源：http://rwu.daria6918.cn

------------------------------------
来源：http://ugo.andypj.xyz

合计 ........... 2106 条
来源：http://vst.jqgfzy.top

按章节统计：
来源：http://aan.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nzh.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jjt.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://asw.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://clq.yj202588.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xmy.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qej.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oaq.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://trd.cqqwz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bzf.andypj.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eai.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://par.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sjn.dashuyun.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://omf.hesvh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kws.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://brf.haohaochexian.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ern.hnxiangtu.top

Q SQL 专题                              90
来源：http://evq.ppjwa.cn

R Bash 专题                             80
来源：http://hzu.daria6918.cn

S C / C++ 专题                          60
来源：http://cap.wangdashe.top

T 其他语言补充                          60
来源：http://apc.cheryme.top


<!-- 参考信息 -->