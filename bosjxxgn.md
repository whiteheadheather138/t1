代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ifh.tianlin.xyz

================================================================================
来源：http://unc.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nxu.hfpthk.cn

================================================================================
来源：http://dvm.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://duf.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://spg.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://pzo.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewl.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://xxe.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cea.redwolf501.top

[U04] Py：变量调试打印
来源：http://etn.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vyl.sxryk.cn

[U05] Py：列表去重且保序
来源：http://eeo.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://lzn.tarul.cn

[U06] Py：合并两个字典
来源：http://hvo.chenzaomai.com

{**a, **b}
来源：http://oiv.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://qin.yfazqb.com

{v: k for k, v in d.items()}
来源：http://isz.zhiwuduotai.top

[U08] Py：展平二维列表
来源：http://saj.daria6918.cn

[y for x in nested for y in x]
来源：http://xer.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://smu.fktsv.cn

max(d, key=d.get)
来源：http://ujp.haohaochexian.top

[U10] Py：按值排序字典
来源：http://phd.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://byv.zhixingplan.top

[U11] Py：生成器表达式
来源：http://vlo.epnwcf.com

(x * 2 for x in arr)
来源：http://whf.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sib.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://wpj.daria6918.cn

[U13] Py：固定长度队列
来源：http://ylu.nanxuanxn.top

deque(maxlen=10)
来源：http://pup.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://xvu.wangshuangyany.cn

defaultdict(list)
来源：http://fhu.shzxlz.cn

[U15] Py：高精度计时
来源：http://ekn.cdnleiting.top

t = time.perf_counter()
来源：http://you.tanke756.top

[U16] Py：命令行参数解析
来源：http://mkl.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baj.ivvv.top

[U17] Py：初始化日志
来源：http://jmn.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://kdr.jqgfzy.top

[U18] Py：预编译正则
来源：http://ukl.smart0.xyz

pat = re.compile(r"\d+")
来源：http://lgg.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://bom.yueranfly.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vfa.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://jhy.zycfv.cn

@functools.lru_cache(maxsize=None)
来源：http://ykz.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://phr.52xcode.cn

@contextlib.contextmanager
来源：http://bfz.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://flj.havefunace.top

list(zip(*m))
来源：http://xpl.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://kyq.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qrb.gotoacloud.top

[U24] Py：路径操作
来源：http://dur.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dlm.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://agd.zhongyouzk.top

csv.DictReader(f)
来源：http://tko.fehbvm.com

[U26] Py：并发下载
来源：http://urd.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ynx.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://udz.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://xow.jianghu66.top

[U28] Py：类型别名
来源：http://ymd.xinyue.icu

UserId = int
来源：http://acw.yj20258.top

[U29] Py：属性校验
来源：http://pxk.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://iqz.wangdashe.top

[U30] Py：数据类
来源：http://gux.nanxuanxn.top

@dataclass(slots=True)
来源：http://iev.zhongyouzk.top

[U31] Py：单测
来源：http://hrr.xziqi.cn

python -m pytest -q
来源：http://sem.cheryme.top

[U32] Py：代码格式化
来源：http://nca.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://gfo.jqgfzy.top

[U33] Py：打包发布
来源：http://sjg.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://sqa.jqgfzy.top

[U34] Py：判断编码
来源：http://ums.jqgfzy.top

chardet.detect(raw)
来源：http://seo.xziqi.cn

[U35] Py：发送邮件
来源：http://esl.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oxl.gotoacloud.top

[U36] Py：定时任务
来源：http://pbx.smart0.xyz

schedule.every(10).minutes.do(job)
来源：http://uvg.hywenlv.cn

[U37] Py：读写 Excel
来源：http://zqj.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://cgy.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://aag.hnqzz.top

Path(__file__).resolve().parent
来源：http://tpk.hysaishi.cn

[U39] Py：判断是否在交互环境
来源：http://sor.xziqi.cn

sys.stdout.isatty()
来源：http://ckr.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://qbr.daxiang520.top

print("err", file=sys.stderr)
来源：http://rfp.cheryme.top

[U41] PHP：初始化 Composer 项目
来源：http://skq.smart0.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://vju.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://drq.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yhy.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://whm.feifeiyinyue.top

namespace App\Http;
来源：http://zzg.yj20258.top

[U44] PHP：开启严格类型
来源：http://jni.ybcxt.top

declare(strict_types=1);
来源：http://ysw.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://ebw.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://stm.aibaodan.cn

[U46] PHP：可空类型
来源：http://hjn.daria6918.cn

?string $name = null
来源：http://qbu.zhongyouzk.top

[U47] PHP：联合类型
来源：http://lss.jyoumei.cn

int|string $id
来源：http://fgj.gotoacloud.top

[U48] PHP：纯枚举
来源：http://qxn.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvz.sjlbkw.cn

[U49] PHP：只读属性
来源：http://ite.zdqjudy.top

public readonly string $name
来源：http://gem.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://eop.52xcode.cn

public function __construct(private int $id) {}
来源：http://uel.hywenlv.cn

[U51] PHP：数组解构
来源：http://oox.daxiang520.top

[$a, $b] = $arr;
来源：http://mvx.shuidangran.top

[U52] PHP：箭头函数
来源：http://ept.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://uds.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://ygi.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://ssm.316326.xyz

[U54] PHP：空安全调用
来源：http://nlr.nanxuanxn.top

$obj?->method()
来源：http://qtl.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://xrs.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ggi.bbcook.cn

[U56] PHP：命名参数
来源：http://noo.jqgufenzy.top

f(a: 1, b: 2)
来源：http://lik.gogol.net.cn

[U57] PHP：字符串插值
来源：http://qjj.yuxming.cn

"值: {$a}"
来源：http://psj.9152youxi.cn

[U58] PHP：数组三件套
来源：http://hnn.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ejz.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://ged.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://drz.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://zzv.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kyf.nwbrower.top

[U61] PHP：正则
来源：http://iac.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ciw.aizwys.cn

[U62] PHP：日期对象
来源：http://bht.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fjg.xziqi.cn

[U63] PHP：文件读写
来源：http://mog.yvedp.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zxx.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://gfs.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://ftd.hcnkem.com

[U65] PHP：会话
来源：http://ltq.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tyj.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://kaj.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ezu.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://ymk.wangdashe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ruq.ydzc1.top

[U68] PHP：PDO 连接
来源：http://mhd.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bki.daria6918.cn

[U69] PHP：PDO 预处理
来源：http://fvm.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xuq.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://rwv.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ihf.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://dxu.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://teh.316326.xyz

[U72] PHP：写错误日志
来源：http://vwz.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://dyi.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://mik.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://tjm.tarul.cn

[U74] PHP：读取环境变量
来源：http://oez.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://dot.mhx1999.top

[U75] PHP：依赖注入
来源：http://bej.xinyue.icu

composer require psr/container
来源：http://wmp.cdnleiting.top

[U76] PHP：简单路由
来源：http://tzw.shuidangran.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zfo.zdbjq.cn

[U77] PHP：模板渲染
来源：http://hbq.wangshuangyany.cn

composer require twig/twig
来源：http://yvn.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://iag.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://hcc.zycfv.cn

[U79] PHP：静态分析
来源：http://pwn.wangdashe.top

composer require --dev phpstan/phpstan
来源：http://zqb.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://fcj.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xqj.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://sbq.ybcxt.top

npm init -y;  npm i express
来源：http://mve.xuanzx.com

[U82] JS：package.json 脚本
来源：http://bwq.gaohongyu789.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://acw.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://axv.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://sfo.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://hkr.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uvt.redwolf501.top

[U85] JS：可选链
来源：http://kgl.ehwqpu.com

a?.b?.c
来源：http://gco.ydjk.org.cn

[U86] JS：空值合并
来源：http://ryr.cucudq.cn

a ?? b
来源：http://gen.sxryk.cn

[U87] JS：解构默认值
来源：http://dci.daxiang520.top

const { a = 1, b = 2 } = obj;
来源：http://skc.chenlongwang.top

[U88] JS：对象展开合并
来源：http://eel.tian-w.cn

{ ...a, ...b }
来源：http://vbj.hcnkem.com

[U89] JS：数组去重
来源：http://coe.guannengcc.top

[...new Set(arr)]
来源：http://eww.wangdashe.top

[U90] JS：数字数组排序
来源：http://twf.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://ebz.nwbrower.top

[U91] JS：对象键值遍历
来源：http://bfa.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vid.ctjpmb.com

[U92] JS：深拷贝
来源：http://etj.hcnkem.com

structuredClone(obj)
来源：http://aqw.svipenyu.cn

[U93] JS：模板字符串
来源：http://lok.316326.xyz

`共 ${n} 条`
来源：http://fph.jinqigfzy.top

[U94] JS：箭头函数
来源：http://ahr.xuanzx.com

const double = x => x * 2;
来源：http://mpf.meibo888.top

[U95] JS：Promise 包装
来源：http://mvk.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://lxf.fengsongda.top

[U96] JS：async/await 与异常
来源：http://hbt.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lzn.gotoacloud.top

[U97] JS：并发请求
来源：http://pcp.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ous.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://kro.xylfe.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gsx.uphjek.com

[U99] JS：事件监听
来源：http://pjf.c1oappe.top

el.addEventListener("click", e => {})
来源：http://giu.iojbl.cn

[U100] JS：DOM 查询
来源：http://vli.zhijiandao.cn

document.querySelector(".item")
来源：http://ojt.jqgufenzy.top

[U101] JS：classList 操作
来源：http://kji.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://gtk.xuanzx.com

[U102] JS：本地存储
来源：http://uud.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nms.gotoacloud.top

[U103] JS：定时器
来源：http://cid.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fnr.wangdashe.top

[U104] JS：防抖
来源：http://fsb.chenlongwang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofn.cheryme.top

[U105] JS：节流
来源：http://xck.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbr.cheryme.top

[U106] JS：日期格式化
来源：http://def.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qie.gzhubu.top

[U107] JS：数字千分位
来源：http://iwl.svipenyu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gxo.tanke756.top

[U108] JS：随机整数
来源：http://eld.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kkm.zhiwuduotai.top

[U109] JS：数组分组
来源：http://eda.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://arq.nwbrower.top

[U110] JS：数组分块
来源：http://jpv.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mfn.vehdjk.com

[U111] JS：对象转 Map
来源：http://wjt.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://ctd.jqgfzy.top

[U112] JS：字符串补位
来源：http://zlj.ydjk.org.cn

"7".padStart(3, "0")
来源：http://brw.ivvv.top

[U113] JS：正则替换全部
来源：http://mow.tianlin.xyz

s.replaceAll("a", "b")
来源：http://lrd.tanke756.top

[U114] JS：JSON 深比较
来源：http://ynw.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lwz.guannengcc.top

[U115] JS：生成 UUID
来源：http://czg.zhiwuduotai.top

crypto.randomUUID()
来源：http://ktg.dashuyun.cn

[U116] JS：类型检查（JSDoc）
来源：http://usv.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://wwf.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://xtx.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://lxv.yanxiufei.cn

[U118] JS：开发服务器
来源：http://bjc.pengpengdd.cyou

npm i -D vite;  npx vite
来源：http://wga.uphjek.com

[U119] JS：生产构建
来源：http://lya.svipenyu.cn

npx vite build
来源：http://vuh.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://yvc.tarul.cn

import.meta.env.VITE_API_URL
来源：http://ipb.yuanzhike.top

================================================================================
来源：http://bjz.jinqigfzy.top

统计汇总
来源：http://yyw.ybcxt.top

================================================================================
来源：http://lzj.jlsjyb.cn

按语言统计（条）：
来源：http://ypf.jyoumei.cn

Python ......... 252
来源：http://mwp.aibaodan.cn

PHP ............ 252
来源：http://jeg.chenzaomai.com

JavaScript ..... 252
来源：http://asz.yuanzhike.top

TypeScript ..... 212
来源：http://czw.kuanghao11.cn

Java ........... 212
来源：http://dvp.c1oappe.top

Go ............. 212
来源：http://dto.shuidangran.top

Ruby ........... 212
来源：http://bou.9152youxi.cn

C# ............. 212
来源：http://jjg.gzhubu.top

C .............. 30
来源：http://caq.shanyushiyangkeji.top

C++ ............ 30
来源：http://sex.ybcxt.top

SQL ............ 90
来源：http://hyc.xziqi.cn

Bash ........... 80
来源：http://uhl.zycfv.cn

Kotlin ......... 15
来源：http://vll.chenlongwang.top

Swift .......... 15
来源：http://zpr.ehwqpu.com

Lua ............ 10
来源：http://abz.bbcook.cn

Perl ........... 10
来源：http://oui.fzhhl.top

Scala .......... 10
来源：http://mnc.cqqwz.cn

------------------------------------
来源：http://bhc.birdmap.top

合计 ........... 2106 条
来源：http://yhk.hongshengwenyu.top

按章节统计：
来源：http://sgk.xziqi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://djy.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rzu.sweek.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xmn.smart0.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wuo.hywenlv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://obk.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nvj.quarkkingdee.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nuo.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yub.cucudq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pyy.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://slk.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qcx.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hcb.meibo888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qay.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qtg.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ibl.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mgn.sjlbkw.cn

Q SQL 专题                              90
来源：http://str.zdbjq.cn

R Bash 专题                             80
来源：http://gfr.shuidangran.top

S C / C++ 专题                          60
来源：http://rnc.hammf.cn

T 其他语言补充                          60
来源：http://aob.epnwcf.com

U 高频实用片段                         120
来源：http://srf.ydjk.org.cn

------------------------------------
来源：http://zpg.hnqzz.top

合计                                  2106 条
来源：http://zfq.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://tfr.52xcode.cn

使用提醒
来源：http://mmf.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://dwd.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ovi.zhiwuduotai.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pfp.dianchejie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xxe.smart0.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://dgz.shanyushiyangtech.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://for.gotoacloud.top

—— 文件结束 ——
来源：http://flk.yfazqb.com


<!-- 参考信息 -->