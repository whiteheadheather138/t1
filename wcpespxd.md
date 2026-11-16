代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://jxf.nanxinkj.top

[T59] Scala：循环
来源：http://dif.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://ete.yj202588.top

[T60] Scala：折叠
来源：http://iyg.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bhv.yongpay.top

================================================================================
来源：http://mwm.epnwcf.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nua.wangdashe.top

================================================================================
来源：http://hod.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://jlh.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://pnr.cqqwz.cn

[U02] Py：导出 / 安装依赖
来源：http://pvk.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhf.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://ttg.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uqw.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://hec.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zch.nwbrower.top

[U05] Py：列表去重且保序
来源：http://bzq.tian-w.cn

list(dict.fromkeys(arr))
来源：http://akv.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://djd.hysaishi.cn

{**a, **b}
来源：http://oqk.yongpay.top

[U07] Py：反转字典键值
来源：http://hfm.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://dlk.zhengqikj.top

[U08] Py：展平二维列表
来源：http://efi.shuidangran.top

[y for x in nested for y in x]
来源：http://njk.cheryme.top

[U09] Py：字典取最大值的键
来源：http://prm.sxryk.cn

max(d, key=d.get)
来源：http://dgx.bbcook.cn

[U10] Py：按值排序字典
来源：http://xqj.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azr.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://erx.hfpthk.cn

(x * 2 for x in arr)
来源：http://wsp.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://xjo.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://fcw.nanxinkj.top

[U13] Py：固定长度队列
来源：http://lto.yuanzhike.top

deque(maxlen=10)
来源：http://qll.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://kal.cheryme.top

defaultdict(list)
来源：http://kbv.yj202588.top

[U15] Py：高精度计时
来源：http://hcz.guannengcc.top

t = time.perf_counter()
来源：http://zih.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://arw.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bak.jlsjyb.cn

[U17] Py：初始化日志
来源：http://xzm.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://jns.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://lqr.hnqzz.top

pat = re.compile(r"\d+")
来源：http://hcb.yueranfly.top

[U19] Py：正则替换带回调
来源：http://fxq.ehwqpu.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://suc.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://ydw.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://hme.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://ayj.ydjk.org.cn

@contextlib.contextmanager
来源：http://xox.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://ync.ctjpmb.com

list(zip(*m))
来源：http://dzu.fktsv.cn

[U23] Py：分块读取大文件
来源：http://edp.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kjd.jianghu66.top

[U24] Py：路径操作
来源：http://qlc.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dhv.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://rbp.ppjwa.cn

csv.DictReader(f)
来源：http://lgz.mhx1999.top

[U26] Py：并发下载
来源：http://gwg.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yoa.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://avz.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://zsf.hywenlv.cn

[U28] Py：类型别名
来源：http://paw.meibo888.top

UserId = int
来源：http://cwy.mhx1999.top

[U29] Py：属性校验
来源：http://mer.9152youxi.cn

@property 与 @x.setter 配合
来源：http://gfg.iojbl.cn

[U30] Py：数据类
来源：http://kgh.dashuyun.cn

@dataclass(slots=True)
来源：http://biw.hysaishi.cn

[U31] Py：单测
来源：http://hsc.sjlbkw.cn

python -m pytest -q
来源：http://zav.zhixingplan.top

[U32] Py：代码格式化
来源：http://lcp.meibo888.top

ruff format . && ruff check --fix .
来源：http://vae.cheryme.top

[U33] Py：打包发布
来源：http://med.wangdashe.top

python -m build  （依赖 pyproject.toml）
来源：http://oft.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://zyf.cdnleiting.top

chardet.detect(raw)
来源：http://rvn.gzhubu.top

[U35] Py：发送邮件
来源：http://dtz.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hmm.zdbjq.cn

[U36] Py：定时任务
来源：http://lln.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://lco.yongpay.top

[U37] Py：读写 Excel
来源：http://rfk.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://kqz.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://uka.andypj.xyz

Path(__file__).resolve().parent
来源：http://yta.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://rup.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://ekq.xylfe.cn

[U40] Py：打印到标准错误
来源：http://zbj.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://ije.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://fdj.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qkm.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://rbd.chenjidiqi.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gtg.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://xjg.gotoacloud.top

namespace App\Http;
来源：http://bwt.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://hqc.yvedp.cn

declare(strict_types=1);
来源：http://yxr.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://ddr.sufxvd.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lcb.cqqwz.cn

[U46] PHP：可空类型
来源：http://ehh.xuetiantiany.cn

?string $name = null
来源：http://tzm.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://ktn.ctjpmb.com

int|string $id
来源：http://chg.yj20258.top

[U48] PHP：纯枚举
来源：http://iri.cdnleiting.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uzq.hnqzz.top

[U49] PHP：只读属性
来源：http://clu.haohaochexian.top

public readonly string $name
来源：http://vjq.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://jjc.sweek.top

public function __construct(private int $id) {}
来源：http://yxu.ydzc1.top

[U51] PHP：数组解构
来源：http://hog.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://zpn.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://ifx.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://sji.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://gvu.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://sni.nanxinkj.top

[U54] PHP：空安全调用
来源：http://lgo.jianghu66.top

$obj?->method()
来源：http://ous.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://qyq.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rip.fehbvm.com

[U56] PHP：命名参数
来源：http://rbw.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://zjs.shzxlz.cn

[U57] PHP：字符串插值
来源：http://atm.guannengcc.top

"值: {$a}"
来源：http://nsi.tanke756.top

[U58] PHP：数组三件套
来源：http://pcd.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vwk.bbcook.cn

[U59] PHP：自定义排序
来源：http://xuj.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsi.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://qfp.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eqy.fanxiaobao.xyz

[U61] PHP：正则
来源：http://xek.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yih.sjlbkw.cn

[U62] PHP：日期对象
来源：http://pxo.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nws.jlsjyb.cn

[U63] PHP：文件读写
来源：http://soi.ctjpmb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nrm.vehdjk.com

[U64] PHP：目录遍历
来源：http://ihj.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://lul.hongshengwenyu.top

[U65] PHP：会话
来源：http://puq.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dzx.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://njs.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wfk.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://edo.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iil.shangyingyoupin.top

[U68] PHP：PDO 连接
来源：http://xsa.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ywm.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://ntp.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jtm.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://nib.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gis.jiagoushi.top

[U71] PHP：抛出异常
来源：http://qmq.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://fmj.iojbl.cn

[U72] PHP：写错误日志
来源：http://lxq.smart0.xyz

error_log("失败: " . $e->getMessage());
来源：http://wuj.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://wys.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://alu.yfazqb.com

[U74] PHP：读取环境变量
来源：http://sec.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://jdi.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://phr.dianchejie.cn

composer require psr/container
来源：http://bzp.sysykeji.top

[U76] PHP：简单路由
来源：http://ehb.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pdn.yueranfly.top

[U77] PHP：模板渲染
来源：http://gnk.daria6918.cn

composer require twig/twig
来源：http://itw.0kj1m.cn

[U78] PHP：单元测试
来源：http://wor.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://odk.yfazqb.com

[U79] PHP：静态分析
来源：http://sst.xziqi.cn

composer require --dev phpstan/phpstan
来源：http://iiw.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://juz.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://irh.cucudq.cn

[U81] JS：初始化项目
来源：http://upw.andypj.xyz

npm init -y;  npm i express
来源：http://tob.vehdjk.com

[U82] JS：package.json 脚本
来源：http://zub.wangshuangyany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://izs.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://fvf.zhijiandao.cn

export const a = 1;  import { a } from "./m.js";
来源：http://flm.fengsongda.top

[U84] JS：CommonJS 写法
来源：http://ayi.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://hsp.daria6918.cn

[U85] JS：可选链
来源：http://qdf.9152youxi.cn

a?.b?.c
来源：http://jrc.ivvv.top

[U86] JS：空值合并
来源：http://xcu.guowangkeji.top

a ?? b
来源：http://xyg.epnwcf.com

[U87] JS：解构默认值
来源：http://qjm.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://rbc.bjfxy.top

[U88] JS：对象展开合并
来源：http://lst.jinghuilouyu.cn

{ ...a, ...b }
来源：http://mnn.epnwcf.com

[U89] JS：数组去重
来源：http://oxn.jinqigfzy.top

[...new Set(arr)]
来源：http://uuv.fktsv.cn

[U90] JS：数字数组排序
来源：http://aap.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://pzx.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://wrs.shangyingyoupin.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://okg.haohaochexian.top

[U92] JS：深拷贝
来源：http://kdx.sxryk.cn

structuredClone(obj)
来源：http://pky.hnqzz.top

[U93] JS：模板字符串
来源：http://dhw.yueranfly.top

`共 ${n} 条`
来源：http://wmh.quarkkingdee.top

[U94] JS：箭头函数
来源：http://gtz.dashuyun.cn

const double = x => x * 2;
来源：http://xzq.nwbrower.top

[U95] JS：Promise 包装
来源：http://rwc.316326.xyz

new Promise((resolve, reject) => {})
来源：http://jxq.andypj.xyz

[U96] JS：async/await 与异常
来源：http://hsx.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://opb.kuanghao11.cn

[U97] JS：并发请求
来源：http://cvn.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://wqa.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://ijg.xuetiantiany.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tyl.yvedp.cn

[U99] JS：事件监听
来源：http://gdq.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://tyk.cqqwz.cn

[U100] JS：DOM 查询
来源：http://xii.jianghu66.top

document.querySelector(".item")
来源：http://zab.xuanzx.com

[U101] JS：classList 操作
来源：http://vgh.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://cin.ctjpmb.com

[U102] JS：本地存储
来源：http://wwo.guowangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wbp.xinyue.icu

[U103] JS：定时器
来源：http://lua.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xqq.cqqwz.cn

[U104] JS：防抖
来源：http://bmu.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bca.sufxvd.cn

[U105] JS：节流
来源：http://pwt.zhengqikj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xqf.svipenyu.cn

[U106] JS：日期格式化
来源：http://xdv.cdnleiting.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cvw.hywenlv.cn

[U107] JS：数字千分位
来源：http://bxb.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sdi.mhx1999.top

[U108] JS：随机整数
来源：http://xwg.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://whh.yueranfly.top

[U109] JS：数组分组
来源：http://dvg.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://vkt.guowangkeji.top

[U110] JS：数组分块
来源：http://qqq.jlsjyb.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hwu.haohaochexian.top

[U111] JS：对象转 Map
来源：http://rcg.dianchejie.cn

new Map(Object.entries(obj))
来源：http://nbu.fengsongda.top

[U112] JS：字符串补位
来源：http://fsf.yangfankeji.com

"7".padStart(3, "0")
来源：http://piu.hesvh.cn

[U113] JS：正则替换全部
来源：http://zfs.zhongyouzk.top

s.replaceAll("a", "b")
来源：http://giz.uphjek.com

[U114] JS：JSON 深比较
来源：http://gmz.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cdy.hongshengwenyu.top

[U115] JS：生成 UUID
来源：http://qgv.zdqjudy.top

crypto.randomUUID()
来源：http://cqa.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://etg.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://wqq.jyoumei.cn

[U117] JS：单元测试
来源：http://qic.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://knw.cqqwz.cn

[U118] JS：开发服务器
来源：http://xpv.sysykeji.top

npm i -D vite;  npx vite
来源：http://xpr.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://awl.sweek.top

npx vite build
来源：http://xct.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://hqk.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://ock.hysaishi.cn

================================================================================
来源：http://ibv.9152youxi.cn

统计汇总
来源：http://pik.chenjidiqi.icu

================================================================================
来源：http://omy.hfpthk.cn

按语言统计（条）：
来源：http://isk.guannengcc.top

Python ......... 252
来源：http://wse.yj202588.top

PHP ............ 252
来源：http://lyt.sufxvd.cn

JavaScript ..... 252
来源：http://goi.yuanzhike.top

TypeScript ..... 212
来源：http://wmh.chenjidiqi.icu

Java ........... 212
来源：http://zhc.zdbjq.cn

Go ............. 212
来源：http://jhx.epnwcf.com

Ruby ........... 212
来源：http://tzh.shzxlz.cn

C# ............. 212
来源：http://bjh.9152youxi.cn

C .............. 30
来源：http://ssu.svipenyu.cn

C++ ............ 30
来源：http://mxm.cheryme.top

SQL ............ 90
来源：http://bdf.pengpengdd.cyou

Bash ........... 80
来源：http://pff.dianchejie.cn

Kotlin ......... 15
来源：http://tge.yvedp.cn

Swift .......... 15
来源：http://uqd.316326.xyz

Lua ............ 10
来源：http://ync.guannengcc.top

Perl ........... 10
来源：http://bsp.aibaodan.cn

Scala .......... 10
来源：http://zna.nanxuanxn.top

------------------------------------
来源：http://ltz.xylfe.cn

合计 ........... 2106 条
来源：http://ztp.cqqwz.cn

按章节统计：
来源：http://svn.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kax.cashguo.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ezh.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sfx.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://agq.jinghuilouyu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yet.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkv.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qda.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wik.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://abp.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dtm.nanxinkj.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yxv.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nnn.cqqwz.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zoa.snrcjt.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cji.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ttt.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yqb.ehwqpu.com

Q SQL 专题                              90
来源：http://edv.fanxiaobao.xyz

R Bash 专题                             80
来源：http://mem.aizwys.cn

S C / C++ 专题                          60
来源：http://mbz.yj20258.top

T 其他语言补充                          60
来源：http://cnt.pengpengdd.cyou

U 高频实用片段                         120
来源：http://eue.wangdashe.top

------------------------------------
来源：http://xvi.yj20258888.top

合计                                  2106 条
来源：http://lzf.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://xmb.hongshengwenyu.top

使用提醒
来源：http://zuo.zycfv.cn

--------------------------------------------------------------------------------
来源：http://zvr.yvedp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://euu.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jbl.52xcode.cn


<!-- 参考信息 -->