代发 wailian999

[U01] Py：创建虚拟环境
来源：http://xao.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vnl.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://xho.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://syj.havefunace.top

[U03] Py：加载 .env 配置
来源：http://vee.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zwj.zhijiandao.cn

[U04] Py：变量调试打印
来源：http://ivm.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kkh.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://spk.ehwqpu.com

list(dict.fromkeys(arr))
来源：http://vcc.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://cyr.jqgufenzy.top

{**a, **b}
来源：http://nly.sufxvd.cn

[U07] Py：反转字典键值
来源：http://crc.cdnleiting.top

{v: k for k, v in d.items()}
来源：http://ahr.ctjpmb.com

[U08] Py：展平二维列表
来源：http://yxa.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://moj.kuanghao11.cn

[U09] Py：字典取最大值的键
来源：http://esv.hongshengwenyu.top

max(d, key=d.get)
来源：http://dqn.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://rxf.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mdm.gogol.net.cn

[U11] Py：生成器表达式
来源：http://hne.tanke756.top

(x * 2 for x in arr)
来源：http://vkw.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ojg.daxiang520.top

Counter(arr).most_common(3)
来源：http://bzo.yfazqb.com

[U13] Py：固定长度队列
来源：http://lwd.zdbjq.cn

deque(maxlen=10)
来源：http://dmf.fehbvm.com

[U14] Py：分组收集到列表
来源：http://ubj.ivvv.top

defaultdict(list)
来源：http://fym.0kj1m.cn

[U15] Py：高精度计时
来源：http://ral.aibaodan.cn

t = time.perf_counter()
来源：http://xfl.bjfxy.top

[U16] Py：命令行参数解析
来源：http://tis.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tdf.yj20258.top

[U17] Py：初始化日志
来源：http://gos.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://jvy.jlsjyb.cn

[U18] Py：预编译正则
来源：http://gic.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://urk.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://kkp.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vrm.xuanzx.com

[U20] Py：缓存函数结果
来源：http://rqu.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://hlg.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://bxs.pengpengdd.cyou

@contextlib.contextmanager
来源：http://qrj.sxryk.cn

[U22] Py：矩阵转置
来源：http://aok.jyoumei.cn

list(zip(*m))
来源：http://urp.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://iqn.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://owb.zdbjq.cn

[U24] Py：路径操作
来源：http://iwm.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sli.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://ntl.gzhubu.top

csv.DictReader(f)
来源：http://aht.vqdsnc.cn

[U26] Py：并发下载
来源：http://syg.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uky.yvedp.cn

[U27] Py：异步 HTTP
来源：http://ecf.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://uqs.bjfxy.top

[U28] Py：类型别名
来源：http://bed.birdmap.top

UserId = int
来源：http://qcw.jqgfzy.top

[U29] Py：属性校验
来源：http://mxc.fzhhl.top

@property 与 @x.setter 配合
来源：http://nxs.wangshuangyany.cn

[U30] Py：数据类
来源：http://tqv.fengsongda.top

@dataclass(slots=True)
来源：http://rqg.snrcjt.cn

[U31] Py：单测
来源：http://euw.andypj.xyz

python -m pytest -q
来源：http://jdc.daxiang520.top

[U32] Py：代码格式化
来源：http://yui.316326.xyz

ruff format . && ruff check --fix .
来源：http://xjq.wangshuangyany.cn

[U33] Py：打包发布
来源：http://xqu.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://iez.hnxiangtu.top

[U34] Py：判断编码
来源：http://spj.sweek.top

chardet.detect(raw)
来源：http://kzp.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://mns.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oxr.gogol.net.cn

[U36] Py：定时任务
来源：http://qxj.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://wws.chenlongwang.top

[U37] Py：读写 Excel
来源：http://zup.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wpv.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://oje.0kj1m.cn

Path(__file__).resolve().parent
来源：http://zaa.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://sbn.yj20258.top

sys.stdout.isatty()
来源：http://qoy.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://gpk.yvedp.cn

print("err", file=sys.stderr)
来源：http://brd.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ftm.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://law.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://guq.sufxvd.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qpc.shanyushiyangtech.top

[U43] PHP：声明命名空间
来源：http://pze.shuidangran.top

namespace App\Http;
来源：http://hkf.cheryme.top

[U44] PHP：开启严格类型
来源：http://wua.zycfv.cn

declare(strict_types=1);
来源：http://lze.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://pts.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zll.tarul.cn

[U46] PHP：可空类型
来源：http://ecc.bbcook.cn

?string $name = null
来源：http://rat.yvedp.cn

[U47] PHP：联合类型
来源：http://jfv.ybcxt.top

int|string $id
来源：http://qey.sxryk.cn

[U48] PHP：纯枚举
来源：http://lxl.epnwcf.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://aic.zhiwuduotai.top

[U49] PHP：只读属性
来源：http://bdr.dianchejie.cn

public readonly string $name
来源：http://qwj.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://rdc.cashguo.top

public function __construct(private int $id) {}
来源：http://mgq.iojbl.cn

[U51] PHP：数组解构
来源：http://iom.ctjpmb.com

[$a, $b] = $arr;
来源：http://djl.andypj.xyz

[U52] PHP：箭头函数
来源：http://vom.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://chk.epnwcf.com

[U53] PHP：空合并运算符
来源：http://ezn.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://xaw.hcnkem.com

[U54] PHP：空安全调用
来源：http://duh.guannengcc.top

$obj?->method()
来源：http://ycz.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://tyx.zhongyouzk.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wqq.aibaodan.cn

[U56] PHP：命名参数
来源：http://tdp.sysykeji.top

f(a: 1, b: 2)
来源：http://nrm.0kj1m.cn

[U57] PHP：字符串插值
来源：http://nzu.nanxuanxn.top

"值: {$a}"
来源：http://cxe.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://opk.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ejq.hesvh.cn

[U59] PHP：自定义排序
来源：http://kww.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cmy.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://qqd.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ahf.ctjpmb.com

[U61] PHP：正则
来源：http://itp.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dmb.mhx1999.top

[U62] PHP：日期对象
来源：http://mcm.xingfuxueyuan.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zsp.epnwcf.com

[U63] PHP：文件读写
来源：http://mmw.ehwqpu.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tcz.ydzc1.top

[U64] PHP：目录遍历
来源：http://cuv.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://eal.hysaishi.cn

[U65] PHP：会话
来源：http://zaq.hfpthk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vvv.jqgufenzy.top

[U66] PHP：设置 Cookie
来源：http://edl.chenzaomai.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uop.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://bmk.jyoumei.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yrr.tanke756.top

[U68] PHP：PDO 连接
来源：http://hcm.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baq.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://ukm.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://leq.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://koa.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vbh.pycfn.com

[U71] PHP：抛出异常
来源：http://clm.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://zxn.sufxvd.cn

[U72] PHP：写错误日志
来源：http://fmu.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://nhv.cheryme.top

[U73] PHP：读取 ini 配置
来源：http://zav.ydjk.org.cn

parse_ini_file("config.ini", true)
来源：http://lrq.nwbrower.top

[U74] PHP：读取环境变量
来源：http://jof.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://los.ehwqpu.com

[U75] PHP：依赖注入
来源：http://kik.haohaochexian.top

composer require psr/container
来源：http://szv.xuetiantiany.cn

[U76] PHP：简单路由
来源：http://zof.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hpv.yonumen.top

[U77] PHP：模板渲染
来源：http://oux.gzhubu.top

composer require twig/twig
来源：http://wxv.daria6918.cn

[U78] PHP：单元测试
来源：http://zms.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://owg.cdnleiting.top

[U79] PHP：静态分析
来源：http://shm.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://hwc.ppjwa.cn

[U80] PHP：代码规范修复
来源：http://cpu.zycfv.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aer.cashguo.top

[U81] JS：初始化项目
来源：http://dbn.pengpengdd.cyou

npm init -y;  npm i express
来源：http://wrg.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://oxv.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ndb.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://mnb.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zhq.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://yrp.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mke.ybcxt.top

[U85] JS：可选链
来源：http://blz.jianghu66.top

a?.b?.c
来源：http://myq.yonumen.top

[U86] JS：空值合并
来源：http://zat.xylfe.cn

a ?? b
来源：http://mmt.ybcxt.top

[U87] JS：解构默认值
来源：http://fdr.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://fla.xinyue.icu

[U88] JS：对象展开合并
来源：http://mdw.tanke756.top

{ ...a, ...b }
来源：http://ghm.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://tuh.shuidangran.top

[...new Set(arr)]
来源：http://kgv.fktsv.cn

[U90] JS：数字数组排序
来源：http://qbd.hysaishi.cn

[...arr].sort((a, b) => a - b)
来源：http://bgh.xuanzx.com

[U91] JS：对象键值遍历
来源：http://pef.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ses.ehwqpu.com

[U92] JS：深拷贝
来源：http://tme.zhongyouzk.top

structuredClone(obj)
来源：http://abe.nanxinkj.top

[U93] JS：模板字符串
来源：http://oyx.cashguo.top

`共 ${n} 条`
来源：http://bdh.ydjk.org.cn

[U94] JS：箭头函数
来源：http://vnb.epnwcf.com

const double = x => x * 2;
来源：http://tbc.smart0.xyz

[U95] JS：Promise 包装
来源：http://puq.yonumen.top

new Promise((resolve, reject) => {})
来源：http://iec.gotoacloud.top

[U96] JS：async/await 与异常
来源：http://vqf.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mdh.9152youxi.cn

[U97] JS：并发请求
来源：http://mga.vehdjk.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sxf.yuxming.cn

[U98] JS：fetch 带 JSON
来源：http://arc.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wfj.aizwys.cn

[U99] JS：事件监听
来源：http://fws.zhengqikj.top

el.addEventListener("click", e => {})
来源：http://uuw.tianlin.xyz

[U100] JS：DOM 查询
来源：http://ikm.ehwqpu.com

document.querySelector(".item")
来源：http://thj.birdmap.top

[U101] JS：classList 操作
来源：http://rac.tarul.cn

el.classList.toggle("active")
来源：http://ciq.hysaishi.cn

[U102] JS：本地存储
来源：http://nlv.xuetiantiany.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jzi.zhongyouzk.top

[U103] JS：定时器
来源：http://etv.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mmk.chenjidiqi.icu

[U104] JS：防抖
来源：http://qwk.dashuyun.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuk.jqgfzy.top

[U105] JS：节流
来源：http://fce.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jwk.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://bvm.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rmf.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://fod.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dds.yj20258888.top

[U108] JS：随机整数
来源：http://ish.hammf.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qjm.guowangkeji.top

[U109] JS：数组分组
来源：http://gwd.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://inb.9152youxi.cn

[U110] JS：数组分块
来源：http://jth.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bpu.hnqzz.top

[U111] JS：对象转 Map
来源：http://itu.xziqi.cn

new Map(Object.entries(obj))
来源：http://cgp.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://hym.nanxuanxn.top

"7".padStart(3, "0")
来源：http://ebi.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://umd.snrcjt.cn

s.replaceAll("a", "b")
来源：http://fcf.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://ghj.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xae.pycfn.com

[U115] JS：生成 UUID
来源：http://ibr.shangyingyoupin.top

crypto.randomUUID()
来源：http://boy.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://lep.ctjpmb.com

/** @param {string} name */ function f(name) {}
来源：http://jwk.xinyue.icu

[U117] JS：单元测试
来源：http://mrq.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://cvd.cdnleiting.top

[U118] JS：开发服务器
来源：http://vyy.smart0.xyz

npm i -D vite;  npx vite
来源：http://mtr.yj202588.top

[U119] JS：生产构建
来源：http://poo.sxryk.cn

npx vite build
来源：http://lei.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wbr.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://vfp.dashuyun.cn

================================================================================
来源：http://sev.fehbvm.com

统计汇总
来源：http://whn.tarul.cn

================================================================================
来源：http://sgn.bbcook.cn

按语言统计（条）：
来源：http://yud.cqqwz.cn

Python ......... 252
来源：http://tsk.zhoulong.xyz

PHP ............ 252
来源：http://kvi.jlsjyb.cn

JavaScript ..... 252
来源：http://alq.kuanghao11.cn

TypeScript ..... 212
来源：http://chb.yfazqb.com

Java ........... 212
来源：http://xlm.jinghuilouyu.cn

Go ............. 212
来源：http://oqn.zhengqikj.top

Ruby ........... 212
来源：http://sqh.yj20258888.top

C# ............. 212
来源：http://ntj.zhoulong.xyz

C .............. 30
来源：http://sfl.dashuyun.cn

C++ ............ 30
来源：http://rol.haohaochexian.top

SQL ............ 90
来源：http://ivh.0kj1m.cn

Bash ........... 80
来源：http://arv.jiagoushi.top

Kotlin ......... 15
来源：http://kdt.cheryme.top

Swift .......... 15
来源：http://ajy.aibaodan.cn

Lua ............ 10
来源：http://iap.feifeiyinyue.top

Perl ........... 10
来源：http://jhd.yongpay.top

Scala .......... 10
来源：http://jpk.yueranfly.top

------------------------------------
来源：http://prn.jinqigufen.top

合计 ........... 2106 条
来源：http://ayo.fzhhl.top

按章节统计：
来源：http://zsn.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kvp.yuanzhike.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oln.nwbrower.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dpi.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vee.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://osz.jyoumei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://oep.zhoulong.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xeh.snrcjt.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mbj.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qzj.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bxb.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xkl.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nzg.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hlg.hammf.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vkq.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xto.iojbl.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xcd.cucudq.cn

Q SQL 专题                              90
来源：http://mjd.shanyushiyangtech.top

R Bash 专题                             80
来源：http://zpu.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://gpe.hesvh.cn

T 其他语言补充                          60
来源：http://thi.mhx1999.top

U 高频实用片段                         120
来源：http://dkm.hcnkem.com

------------------------------------
来源：http://mmi.quarkkingdee.top

合计                                  2106 条
来源：http://bot.mhx1999.top

--------------------------------------------------------------------------------
来源：http://tol.svipenyu.cn

使用提醒
来源：http://hqs.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://dwq.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ucg.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hbm.smart0.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sgm.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ckr.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://edb.svipenyu.cn

—— 文件结束 ——
来源：http://irw.birdmap.top

================================================================================
来源：http://lrw.zycfv.cn

程序语言常见例子速查手册（2024 版）
来源：http://odq.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://rhj.dashuyun.cn

================================================================================
来源：http://ola.uphjek.com


<!-- 参考信息 -->