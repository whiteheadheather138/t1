代发 wailian999

[U01] Py：创建虚拟环境
来源：http://xyr.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://nzw.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://yps.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lko.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://pek.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vlu.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://vsd.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lpp.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://zpr.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://hdt.jinqigufen.top

[U06] Py：合并两个字典
来源：http://xix.nwbrower.top

{**a, **b}
来源：http://hch.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://ixt.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://zpj.ydzc1.top

[U08] Py：展平二维列表
来源：http://rvk.zhijiandao.cn

[y for x in nested for y in x]
来源：http://jnu.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://pic.ydjk.org.cn

max(d, key=d.get)
来源：http://qhz.tian-w.cn

[U10] Py：按值排序字典
来源：http://lub.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qsb.haohaochexian.top

[U11] Py：生成器表达式
来源：http://iuq.cucudq.cn

(x * 2 for x in arr)
来源：http://dig.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://lgf.chenlongwang.top

Counter(arr).most_common(3)
来源：http://gsq.daxiang520.top

[U13] Py：固定长度队列
来源：http://xcl.hysaishi.cn

deque(maxlen=10)
来源：http://ull.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://etb.zhijiandao.cn

defaultdict(list)
来源：http://udg.yj20258888.top

[U15] Py：高精度计时
来源：http://xwj.daria6918.cn

t = time.perf_counter()
来源：http://pwo.vehdjk.com

[U16] Py：命令行参数解析
来源：http://pxh.jiagoushi.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xxr.epnwcf.com

[U17] Py：初始化日志
来源：http://kdq.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://roe.9152youxi.cn

[U18] Py：预编译正则
来源：http://bii.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://mbz.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://olk.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bjl.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://ite.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://kzg.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://hqu.zdqjudy.top

@contextlib.contextmanager
来源：http://oxk.hywenlv.cn

[U22] Py：矩阵转置
来源：http://hia.shzxlz.cn

list(zip(*m))
来源：http://ole.yueranfly.top

[U23] Py：分块读取大文件
来源：http://ecc.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cqa.hywenlv.cn

[U24] Py：路径操作
来源：http://byi.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://npk.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://tsy.ctjpmb.com

csv.DictReader(f)
来源：http://ajc.52xcode.cn

[U26] Py：并发下载
来源：http://quv.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ies.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://kxd.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://ugj.sxryk.cn

[U28] Py：类型别名
来源：http://wcv.ctjpmb.com

UserId = int
来源：http://acw.birdmap.top

[U29] Py：属性校验
来源：http://vie.ehwqpu.com

@property 与 @x.setter 配合
来源：http://kzx.zhengqikj.top

[U30] Py：数据类
来源：http://odb.shangyingyoupin.top

@dataclass(slots=True)
来源：http://lak.yueranfly.top

[U31] Py：单测
来源：http://muo.havefunace.top

python -m pytest -q
来源：http://eyl.tanke756.top

[U32] Py：代码格式化
来源：http://xii.sufxvd.cn

ruff format . && ruff check --fix .
来源：http://lvd.zhoulong.xyz

[U33] Py：打包发布
来源：http://yrx.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://msk.shangyingyoupin.top

[U34] Py：判断编码
来源：http://yfo.xuetiantiany.cn

chardet.detect(raw)
来源：http://wkg.jlsjyb.cn

[U35] Py：发送邮件
来源：http://ohk.svipenyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ahd.sxryk.cn

[U36] Py：定时任务
来源：http://mwd.xingfuxueyuan.xyz

schedule.every(10).minutes.do(job)
来源：http://hxt.sufxvd.cn

[U37] Py：读写 Excel
来源：http://agp.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://jvt.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://okl.gzhubu.top

Path(__file__).resolve().parent
来源：http://srw.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://zzq.havefunace.top

sys.stdout.isatty()
来源：http://ura.cashguo.top

[U40] Py：打印到标准错误
来源：http://mvl.yueranfly.top

print("err", file=sys.stderr)
来源：http://ejz.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://ply.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://znc.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://mka.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wkv.yvedp.cn

[U43] PHP：声明命名空间
来源：http://oqo.hysaishi.cn

namespace App\Http;
来源：http://ciz.aizwys.cn

[U44] PHP：开启严格类型
来源：http://kkj.ydzc1.top

declare(strict_types=1);
来源：http://mtf.daria6918.cn

[U45] PHP：类型声明与返回类型
来源：http://vuz.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ssk.yuanzhike.top

[U46] PHP：可空类型
来源：http://pek.sweek.top

?string $name = null
来源：http://jqb.yuanzhike.top

[U47] PHP：联合类型
来源：http://kmw.yj202588.top

int|string $id
来源：http://gfh.pycfn.com

[U48] PHP：纯枚举
来源：http://dfs.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hhs.jlsjyb.cn

[U49] PHP：只读属性
来源：http://ijl.tian-w.cn

public readonly string $name
来源：http://izg.jinqigufen.top

[U50] PHP：构造器属性提升
来源：http://qkq.gzhubu.top

public function __construct(private int $id) {}
来源：http://emd.cucudq.cn

[U51] PHP：数组解构
来源：http://rwe.ehwqpu.com

[$a, $b] = $arr;
来源：http://fqr.jianghu66.top

[U52] PHP：箭头函数
来源：http://icj.tianlin.xyz

$double = fn($x) => $x * 2;
来源：http://dva.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://nrc.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://ztu.andypj.xyz

[U54] PHP：空安全调用
来源：http://lui.yangfankeji.com

$obj?->method()
来源：http://qpr.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://lix.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ouj.vehdjk.com

[U56] PHP：命名参数
来源：http://zbc.cashguo.top

f(a: 1, b: 2)
来源：http://jah.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://npx.fktsv.cn

"值: {$a}"
来源：http://bkn.daxiang520.top

[U58] PHP：数组三件套
来源：http://lsn.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qke.chenzaomai.com

[U59] PHP：自定义排序
来源：http://zku.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fnc.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://wah.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://izm.tianlin.xyz

[U61] PHP：正则
来源：http://mtx.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fsa.xziqi.cn

[U62] PHP：日期对象
来源：http://tba.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://srt.nwbrower.top

[U63] PHP：文件读写
来源：http://lnh.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://czr.zhengqikj.top

[U64] PHP：目录遍历
来源：http://bdi.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://nmr.jianghu66.top

[U65] PHP：会话
来源：http://sbs.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://yfz.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://fng.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ceb.epnwcf.com

[U67] PHP：处理文件上传
来源：http://ovh.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fnf.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://dsc.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cpd.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://wks.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gql.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://otq.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sya.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://ykb.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://sjn.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://lkj.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://its.pycfn.com

[U73] PHP：读取 ini 配置
来源：http://qig.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://juu.daxiang520.top

[U74] PHP：读取环境变量
来源：http://xui.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://seq.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://tdv.zhengqikj.top

composer require psr/container
来源：http://qcz.zhoulong.xyz

[U76] PHP：简单路由
来源：http://tnl.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tcw.zhijiandao.cn

[U77] PHP：模板渲染
来源：http://yvu.shanyushiyangkeji.top

composer require twig/twig
来源：http://wli.shzxlz.cn

[U78] PHP：单元测试
来源：http://dng.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://jgs.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://ssx.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://jxr.cucudq.cn

[U80] PHP：代码规范修复
来源：http://azy.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bya.xinyue.icu

[U81] JS：初始化项目
来源：http://tgm.zhengqikj.top

npm init -y;  npm i express
来源：http://yvd.xylfe.cn

[U82] JS：package.json 脚本
来源：http://idz.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oby.gogol.net.cn

[U83] JS：ES Module 导入导出
来源：http://mid.nwbrower.top

export const a = 1;  import { a } from "./m.js";
来源：http://dqa.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://npw.jinqigufen.top

module.exports = { a };  const { a } = require("./m");
来源：http://nbd.pycfn.com

[U85] JS：可选链
来源：http://jny.pycfn.com

a?.b?.c
来源：http://kaf.yj202588.top

[U86] JS：空值合并
来源：http://xry.quarkkingdee.top

a ?? b
来源：http://ita.jiagoushi.top

[U87] JS：解构默认值
来源：http://ytt.aizwys.cn

const { a = 1, b = 2 } = obj;
来源：http://nxp.uphjek.com

[U88] JS：对象展开合并
来源：http://zme.ydzc1.top

{ ...a, ...b }
来源：http://ppt.fehbvm.com

[U89] JS：数组去重
来源：http://aae.fzhhl.top

[...new Set(arr)]
来源：http://uxt.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://skf.tian-w.cn

[...arr].sort((a, b) => a - b)
来源：http://cgb.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://bms.bjfxy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jki.hesvh.cn

[U92] JS：深拷贝
来源：http://zic.cucudq.cn

structuredClone(obj)
来源：http://uxw.sxryk.cn

[U93] JS：模板字符串
来源：http://niu.hcnkem.com

`共 ${n} 条`
来源：http://nsd.nwbrower.top

[U94] JS：箭头函数
来源：http://sei.yanxiufei.cn

const double = x => x * 2;
来源：http://wdc.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://wrr.uphjek.com

new Promise((resolve, reject) => {})
来源：http://wki.ydzc1.top

[U96] JS：async/await 与异常
来源：http://czy.iojbl.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yko.daxiang520.top

[U97] JS：并发请求
来源：http://pxd.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iiu.pycfn.com

[U98] JS：fetch 带 JSON
来源：http://rml.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://snv.xuanzx.com

[U99] JS：事件监听
来源：http://qia.hesvh.cn

el.addEventListener("click", e => {})
来源：http://kfs.meibo888.top

[U100] JS：DOM 查询
来源：http://tgy.zycfv.cn

document.querySelector(".item")
来源：http://vct.tarul.cn

[U101] JS：classList 操作
来源：http://jos.zdqjudy.top

el.classList.toggle("active")
来源：http://qat.gzhubu.top

[U102] JS：本地存储
来源：http://bsy.zycfv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ayh.vqdsnc.cn

[U103] JS：定时器
来源：http://gzc.xinyue.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sgg.chenjidiqi.icu

[U104] JS：防抖
来源：http://kro.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dso.fanxiaobao.xyz

[U105] JS：节流
来源：http://xlu.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kkm.tianlin.xyz

[U106] JS：日期格式化
来源：http://qfi.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cmz.zhijiandao.cn

[U107] JS：数字千分位
来源：http://vlb.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rcx.sufxvd.cn

[U108] JS：随机整数
来源：http://lbf.jinqigfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://moh.smart0.xyz

[U109] JS：数组分组
来源：http://mzr.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://gyx.yanxiufei.cn

[U110] JS：数组分块
来源：http://gea.zdqjudy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hol.smart0.xyz

[U111] JS：对象转 Map
来源：http://rkm.smart0.xyz

new Map(Object.entries(obj))
来源：http://obi.jqgufenzy.top

[U112] JS：字符串补位
来源：http://nvu.tarul.cn

"7".padStart(3, "0")
来源：http://cvv.316326.xyz

[U113] JS：正则替换全部
来源：http://iom.bbcook.cn

s.replaceAll("a", "b")
来源：http://qeb.yueranfly.top

[U114] JS：JSON 深比较
来源：http://mrk.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://opy.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://psl.daxiang520.top

crypto.randomUUID()
来源：http://dvk.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://usl.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://ajr.jinqigufen.top

[U117] JS：单元测试
来源：http://jcl.pycfn.com

npm i -D vitest;  npx vitest
来源：http://usg.xylfe.cn

[U118] JS：开发服务器
来源：http://vjg.zdbjq.cn

npm i -D vite;  npx vite
来源：http://ivy.zhixingplan.top

[U119] JS：生产构建
来源：http://etj.epnwcf.com

npx vite build
来源：http://ygh.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://utu.xuanzx.com

import.meta.env.VITE_API_URL
来源：http://xrp.fanxiaobao.xyz

================================================================================
来源：http://hqm.xuanzx.com

统计汇总
来源：http://udo.ydzc1.top

================================================================================
来源：http://dcv.smart0.xyz

按语言统计（条）：
来源：http://wqd.shanyushiyangtech.top

Python ......... 252
来源：http://utx.hywenlv.cn

PHP ............ 252
来源：http://gpx.jlsjyb.cn

JavaScript ..... 252
来源：http://oln.cashguo.top

TypeScript ..... 212
来源：http://iti.zdqjudy.top

Java ........... 212
来源：http://mry.ybcxt.top

Go ............. 212
来源：http://aij.kuanghao11.cn

Ruby ........... 212
来源：http://ugs.hysaishi.cn

C# ............. 212
来源：http://acr.yj20258888.top

C .............. 30
来源：http://vve.shangyingyoupin.top

C++ ............ 30
来源：http://ojm.chenjidiqi.icu

SQL ............ 90
来源：http://dxa.gzhubu.top

Bash ........... 80
来源：http://ctv.wangdashe.top

Kotlin ......... 15
来源：http://geh.zhixingplan.top

Swift .......... 15
来源：http://bit.sjlbkw.cn

Lua ............ 10
来源：http://fge.gotoacloud.top

Perl ........... 10
来源：http://lkb.cucudq.cn

Scala .......... 10
来源：http://spf.fengsongda.top

------------------------------------
来源：http://chf.smart0.xyz

合计 ........... 2106 条
来源：http://htr.andypj.xyz

按章节统计：
来源：http://byo.ehwqpu.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mhl.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ubx.jinyuanbaomall.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ilk.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dql.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nll.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gmb.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aqb.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rhn.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sid.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://itx.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zgu.pengpengdd.cyou

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://liw.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://szw.jqgfzy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://imx.jqgufenzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zfq.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vdr.dianchejie.cn

Q SQL 专题                              90
来源：http://mpv.52xcode.cn

R Bash 专题                             80
来源：http://xff.yj20258.top

S C / C++ 专题                          60
来源：http://ysn.sysykeji.top

T 其他语言补充                          60
来源：http://vdk.gaohongyu789.top

U 高频实用片段                         120
来源：http://qhg.hammf.cn

------------------------------------
来源：http://kbs.quarkkingdee.top

合计                                  2106 条
来源：http://dqi.epnwcf.com

--------------------------------------------------------------------------------
来源：http://ifb.shanyushiyangkeji.top

使用提醒
来源：http://wnc.316326.xyz

--------------------------------------------------------------------------------
来源：http://nas.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vci.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nfc.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://aqw.guowangkeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zdr.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://msa.ydzc1.top

—— 文件结束 ——
来源：http://ybl.cqqwz.cn

================================================================================
来源：http://wnx.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://yrr.tian-w.cn

Common Programming Examples Cheat Book
来源：http://acz.316326.xyz

================================================================================
来源：http://fsr.cdnleiting.top


<!-- 参考信息 -->