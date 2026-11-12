代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://ymd.andypj.xyz

[T59] Scala：循环
来源：http://ghb.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://yeb.guannengcc.top

[T60] Scala：折叠
来源：http://yoh.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kgl.0kj1m.cn

================================================================================
来源：http://pds.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zjv.mhx1999.top

================================================================================
来源：http://hnq.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://npu.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://vhv.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://ojd.meibo888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rpj.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://uax.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ujn.cqqwz.cn

[U04] Py：变量调试打印
来源：http://ils.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eoc.jinghuilouyu.cn

[U05] Py：列表去重且保序
来源：http://zhq.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://nmk.yj20258.top

[U06] Py：合并两个字典
来源：http://jab.jqgfzy.top

{**a, **b}
来源：http://nwc.cashguo.top

[U07] Py：反转字典键值
来源：http://gte.xylfe.cn

{v: k for k, v in d.items()}
来源：http://azb.dianchejie.cn

[U08] Py：展平二维列表
来源：http://fad.wangdashe.top

[y for x in nested for y in x]
来源：http://lwn.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://fsf.ivvv.top

max(d, key=d.get)
来源：http://dcz.hammf.cn

[U10] Py：按值排序字典
来源：http://xnq.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gsy.cashguo.top

[U11] Py：生成器表达式
来源：http://bjf.daria6918.cn

(x * 2 for x in arr)
来源：http://xmb.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://ifh.gzhubu.top

Counter(arr).most_common(3)
来源：http://kid.dianchejie.cn

[U13] Py：固定长度队列
来源：http://syr.shangyingyoupin.top

deque(maxlen=10)
来源：http://cun.epnwcf.com

[U14] Py：分组收集到列表
来源：http://vxj.uphjek.com

defaultdict(list)
来源：http://cqk.kuanghao11.cn

[U15] Py：高精度计时
来源：http://uwm.316326.xyz

t = time.perf_counter()
来源：http://vcr.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://krl.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rse.cqqwz.cn

[U17] Py：初始化日志
来源：http://iom.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://qit.chenzaomai.com

[U18] Py：预编译正则
来源：http://pwp.yj20258.top

pat = re.compile(r"\d+")
来源：http://ylm.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://ifb.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qlq.cucudq.cn

[U20] Py：缓存函数结果
来源：http://hdr.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://yfg.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://yno.fktsv.cn

@contextlib.contextmanager
来源：http://bcq.pycfn.com

[U22] Py：矩阵转置
来源：http://tye.redwolf501.top

list(zip(*m))
来源：http://kun.zhixingplan.top

[U23] Py：分块读取大文件
来源：http://dgd.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dpi.quarkkingdee.top

[U24] Py：路径操作
来源：http://chz.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yno.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://upb.zdqjudy.top

csv.DictReader(f)
来源：http://ckn.yongpay.top

[U26] Py：并发下载
来源：http://hmy.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zcb.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://gow.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://fse.cheryme.top

[U28] Py：类型别名
来源：http://zxb.aibaodan.cn

UserId = int
来源：http://gmm.hongshengwenyu.top

[U29] Py：属性校验
来源：http://iyf.zdbjq.cn

@property 与 @x.setter 配合
来源：http://diu.shuidangran.top

[U30] Py：数据类
来源：http://fqf.yuxming.cn

@dataclass(slots=True)
来源：http://kis.tian-w.cn

[U31] Py：单测
来源：http://tcw.vqdsnc.cn

python -m pytest -q
来源：http://opr.ivvv.top

[U32] Py：代码格式化
来源：http://bhs.fzhhl.top

ruff format . && ruff check --fix .
来源：http://hjp.tianlin.xyz

[U33] Py：打包发布
来源：http://oph.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://nrt.hnxiangtu.top

[U34] Py：判断编码
来源：http://puk.xuanzx.com

chardet.detect(raw)
来源：http://gue.hnqzz.top

[U35] Py：发送邮件
来源：http://xka.fanxiaobao.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nht.sysykeji.top

[U36] Py：定时任务
来源：http://ikx.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://pwu.mhx1999.top

[U37] Py：读写 Excel
来源：http://yow.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yzc.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://qmy.zhongyouzk.top

Path(__file__).resolve().parent
来源：http://hnq.chenzaomai.com

[U39] Py：判断是否在交互环境
来源：http://luj.cheryme.top

sys.stdout.isatty()
来源：http://iwd.sxryk.cn

[U40] Py：打印到标准错误
来源：http://obt.ctjpmb.com

print("err", file=sys.stderr)
来源：http://tcj.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://pcq.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lmq.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://geo.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jqz.guannengcc.top

[U43] PHP：声明命名空间
来源：http://twc.zhiwuduotai.top

namespace App\Http;
来源：http://rfj.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://ddp.tian-w.cn

declare(strict_types=1);
来源：http://fni.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://lnj.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fch.ywan-chungtsiang.top

[U46] PHP：可空类型
来源：http://bnl.ydzc1.top

?string $name = null
来源：http://kqu.ybcxt.top

[U47] PHP：联合类型
来源：http://fkw.yvedp.cn

int|string $id
来源：http://xhw.gzhubu.top

[U48] PHP：纯枚举
来源：http://wjn.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lil.jqgfzy.top

[U49] PHP：只读属性
来源：http://jsb.svipenyu.cn

public readonly string $name
来源：http://ald.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://oxa.hfpthk.cn

public function __construct(private int $id) {}
来源：http://qim.vehdjk.com

[U51] PHP：数组解构
来源：http://nop.cheryme.top

[$a, $b] = $arr;
来源：http://vnd.dashuyun.cn

[U52] PHP：箭头函数
来源：http://hzw.birdmap.top

$double = fn($x) => $x * 2;
来源：http://oja.pycfn.com

[U53] PHP：空合并运算符
来源：http://bga.52xcode.cn

$v = $a ?? $b ?? "default";
来源：http://ztj.cheryme.top

[U54] PHP：空安全调用
来源：http://zpb.ppjwa.cn

$obj?->method()
来源：http://myw.ivvv.top

[U55] PHP：match 表达式
来源：http://kmw.cqqwz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vge.yvedp.cn

[U56] PHP：命名参数
来源：http://bfw.haohaochexian.top

f(a: 1, b: 2)
来源：http://ily.uphjek.com

[U57] PHP：字符串插值
来源：http://zob.wangshuangyany.cn

"值: {$a}"
来源：http://dbx.ctjpmb.com

[U58] PHP：数组三件套
来源：http://hkt.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xnk.daria6918.cn

[U59] PHP：自定义排序
来源：http://yco.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sha.tanke756.top

[U60] PHP：JSON 编解码
来源：http://dna.jinyuanbaomall.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zau.nanxinkj.top

[U61] PHP：正则
来源：http://iha.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vjt.sxryk.cn

[U62] PHP：日期对象
来源：http://ugn.ydjk.org.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ybu.cucudq.cn

[U63] PHP：文件读写
来源：http://kvf.vqdsnc.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zuf.hnqzz.top

[U64] PHP：目录遍历
来源：http://gfi.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://aog.hammf.cn

[U65] PHP：会话
来源：http://loz.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://yhq.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://jto.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bbh.vehdjk.com

[U67] PHP：处理文件上传
来源：http://ysb.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vbo.gzhubu.top

[U68] PHP：PDO 连接
来源：http://tvk.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oxg.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://okr.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dxn.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://qbb.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ejw.hammf.cn

[U71] PHP：抛出异常
来源：http://kkt.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://rzx.0kj1m.cn

[U72] PHP：写错误日志
来源：http://nqe.meibo888.top

error_log("失败: " . $e->getMessage());
来源：http://sno.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://wft.zhijiandao.cn

parse_ini_file("config.ini", true)
来源：http://kmq.jianghu66.top

[U74] PHP：读取环境变量
来源：http://ngr.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://bhm.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://cyz.quarkkingdee.top

composer require psr/container
来源：http://ewv.ydjk.org.cn

[U76] PHP：简单路由
来源：http://ezl.kuanghao11.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bvn.ybcxt.top

[U77] PHP：模板渲染
来源：http://aik.jinyuanbaomall.cn

composer require twig/twig
来源：http://dzp.daria6918.cn

[U78] PHP：单元测试
来源：http://aez.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://zmo.xuanzx.com

[U79] PHP：静态分析
来源：http://ntm.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://yel.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://ygn.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://loh.xuanzx.com

[U81] JS：初始化项目
来源：http://cwv.fehbvm.com

npm init -y;  npm i express
来源：http://fge.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://piq.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pgf.yuanzhike.top

[U83] JS：ES Module 导入导出
来源：http://bwk.redwolf501.top

export const a = 1;  import { a } from "./m.js";
来源：http://kku.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://miv.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://uvx.aibaodan.cn

[U85] JS：可选链
来源：http://jfj.yj20258888.top

a?.b?.c
来源：http://fop.chenlongwang.top

[U86] JS：空值合并
来源：http://xde.xuanzx.com

a ?? b
来源：http://wii.daria6918.cn

[U87] JS：解构默认值
来源：http://zzv.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://msk.ybcxt.top

[U88] JS：对象展开合并
来源：http://cyz.ppjwa.cn

{ ...a, ...b }
来源：http://uuh.meibo888.top

[U89] JS：数组去重
来源：http://fbz.yvedp.cn

[...new Set(arr)]
来源：http://smw.yuanzhike.top

[U90] JS：数字数组排序
来源：http://bdd.fanxiaobao.xyz

[...arr].sort((a, b) => a - b)
来源：http://eef.ehwqpu.com

[U91] JS：对象键值遍历
来源：http://txn.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qjq.guowangkeji.top

[U92] JS：深拷贝
来源：http://ost.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://qud.sufxvd.cn

[U93] JS：模板字符串
来源：http://oyc.cashguo.top

`共 ${n} 条`
来源：http://ljp.chenjidiqi.icu

[U94] JS：箭头函数
来源：http://mrc.sxryk.cn

const double = x => x * 2;
来源：http://cfb.nwbrower.top

[U95] JS：Promise 包装
来源：http://mtv.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://wyu.bbcook.cn

[U96] JS：async/await 与异常
来源：http://apc.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zyx.dianchejie.cn

[U97] JS：并发请求
来源：http://cwz.ydzc1.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rwe.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://xhd.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ynh.fengsongda.top

[U99] JS：事件监听
来源：http://csk.hesvh.cn

el.addEventListener("click", e => {})
来源：http://chq.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://mlv.chenlongwang.top

document.querySelector(".item")
来源：http://yde.zhoulong.xyz

[U101] JS：classList 操作
来源：http://ngt.aibaodan.cn

el.classList.toggle("active")
来源：http://nfv.uphjek.com

[U102] JS：本地存储
来源：http://kyg.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jei.sweek.top

[U103] JS：定时器
来源：http://dfd.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ovx.yuxming.cn

[U104] JS：防抖
来源：http://ufj.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hnc.chenzaomai.com

[U105] JS：节流
来源：http://qto.ppjwa.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dsq.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://rll.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mjw.fzhhl.top

[U107] JS：数字千分位
来源：http://xms.zhongyouzk.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jtq.uphjek.com

[U108] JS：随机整数
来源：http://omn.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nwz.zycfv.cn

[U109] JS：数组分组
来源：http://jtl.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://fkx.jinqigfzy.top

[U110] JS：数组分块
来源：http://epy.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tgo.yonumen.top

[U111] JS：对象转 Map
来源：http://glb.zycfv.cn

new Map(Object.entries(obj))
来源：http://hmb.ehwqpu.com

[U112] JS：字符串补位
来源：http://rvf.shzxlz.cn

"7".padStart(3, "0")
来源：http://yrq.316326.xyz

[U113] JS：正则替换全部
来源：http://euv.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://cla.nwbrower.top

[U114] JS：JSON 深比较
来源：http://ixb.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hdn.meibo888.top

[U115] JS：生成 UUID
来源：http://owp.wangdashe.top

crypto.randomUUID()
来源：http://tox.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://ylr.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://vwv.wangdashe.top

[U117] JS：单元测试
来源：http://qqv.yj202588.top

npm i -D vitest;  npx vitest
来源：http://vaj.feifeiyinyue.top

[U118] JS：开发服务器
来源：http://akr.yueranfly.top

npm i -D vite;  npx vite
来源：http://mvm.xuetiantiany.cn

[U119] JS：生产构建
来源：http://ibn.xuanzx.com

npx vite build
来源：http://jhw.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://zsc.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://ppy.xingfuxueyuan.xyz

================================================================================
来源：http://kpf.zdqjudy.top

统计汇总
来源：http://rhn.gogol.net.cn

================================================================================
来源：http://kza.ctjpmb.com

按语言统计（条）：
来源：http://ypz.hywenlv.cn

Python ......... 252
来源：http://dfh.hnxiangtu.top

PHP ............ 252
来源：http://yxy.vehdjk.com

JavaScript ..... 252
来源：http://rdo.ivvv.top

TypeScript ..... 212
来源：http://vvn.gzhubu.top

Java ........... 212
来源：http://xke.daxiang520.top

Go ............. 212
来源：http://toh.ehwqpu.com

Ruby ........... 212
来源：http://cac.tianlin.xyz

C# ............. 212
来源：http://hmu.svipenyu.cn

C .............. 30
来源：http://bfk.zhoulong.xyz

C++ ............ 30
来源：http://rda.52xcode.cn

SQL ............ 90
来源：http://wys.yangfankeji.com

Bash ........... 80
来源：http://eaq.sysykeji.top

Kotlin ......... 15
来源：http://wif.yanxiufei.cn

Swift .......... 15
来源：http://yfx.yfazqb.com

Lua ............ 10
来源：http://hle.xingfuxueyuan.xyz

Perl ........... 10
来源：http://kmq.zdbjq.cn

Scala .......... 10
来源：http://xkm.haohaochexian.top

------------------------------------
来源：http://ehg.bjfxy.top

合计 ........... 2106 条
来源：http://ank.aibaodan.cn

按章节统计：
来源：http://klm.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tvi.jlsjyb.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lhk.yuxming.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://omj.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tse.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fcd.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nna.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cga.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tfk.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kdn.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nnl.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xmr.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nac.yvedp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lbi.vehdjk.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gyj.yongpay.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ipt.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lgg.sufxvd.cn

Q SQL 专题                              90
来源：http://ify.zdbjq.cn

R Bash 专题                             80
来源：http://mek.chenjidiqi.icu

S C / C++ 专题                          60
来源：http://mdo.yueranfly.top

T 其他语言补充                          60
来源：http://aew.sxryk.cn

U 高频实用片段                         120
来源：http://lhs.fengsongda.top

------------------------------------
来源：http://cbp.gotoacloud.top

合计                                  2106 条
来源：http://eka.kuanghao11.cn

--------------------------------------------------------------------------------
来源：http://fom.hysaishi.cn

使用提醒
来源：http://jde.uphjek.com

--------------------------------------------------------------------------------
来源：http://xqk.ydzc1.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yzy.mhx1999.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mrv.yj20258888.top


<!-- 参考信息 -->