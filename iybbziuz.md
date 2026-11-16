代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://psr.haohaochexian.top

================================================================================
来源：http://wco.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cnz.gzhubu.top

================================================================================
来源：http://bas.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://zkr.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://ame.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://qik.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://koz.sweek.top

[U03] Py：加载 .env 配置
来源：http://nmb.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ftt.hammf.cn

[U04] Py：变量调试打印
来源：http://vfz.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jdn.sxryk.cn

[U05] Py：列表去重且保序
来源：http://qgp.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://ffc.andypj.xyz

[U06] Py：合并两个字典
来源：http://lkc.jqgfzy.top

{**a, **b}
来源：http://ukc.tian-w.cn

[U07] Py：反转字典键值
来源：http://dno.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://tst.guannengcc.top

[U08] Py：展平二维列表
来源：http://rzz.ydjk.org.cn

[y for x in nested for y in x]
来源：http://mex.yonumen.top

[U09] Py：字典取最大值的键
来源：http://erj.redwolf501.top

max(d, key=d.get)
来源：http://smb.gzhubu.top

[U10] Py：按值排序字典
来源：http://ijr.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jlu.hysaishi.cn

[U11] Py：生成器表达式
来源：http://ola.yuxming.cn

(x * 2 for x in arr)
来源：http://xgs.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://sku.daria6918.cn

Counter(arr).most_common(3)
来源：http://ckh.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://qmd.sweek.top

deque(maxlen=10)
来源：http://oxd.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://csc.tarul.cn

defaultdict(list)
来源：http://ksp.xylfe.cn

[U15] Py：高精度计时
来源：http://vwm.zhengqikj.top

t = time.perf_counter()
来源：http://fpp.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://bfr.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zzk.vehdjk.com

[U17] Py：初始化日志
来源：http://vdh.hesvh.cn

logging.basicConfig(level=logging.INFO)
来源：http://nwp.epnwcf.com

[U18] Py：预编译正则
来源：http://fwj.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://qui.yonumen.top

[U19] Py：正则替换带回调
来源：http://ohj.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fmz.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://yfu.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://kyp.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://xhz.jianghu66.top

@contextlib.contextmanager
来源：http://lkx.xziqi.cn

[U22] Py：矩阵转置
来源：http://hiw.hywenlv.cn

list(zip(*m))
来源：http://azn.andypj.xyz

[U23] Py：分块读取大文件
来源：http://umt.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ubt.hesvh.cn

[U24] Py：路径操作
来源：http://zws.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ohw.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://ygz.tanke756.top

csv.DictReader(f)
来源：http://jle.sweek.top

[U26] Py：并发下载
来源：http://pyg.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fcv.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://fdq.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://qrt.yueranfly.top

[U28] Py：类型别名
来源：http://rlx.316326.xyz

UserId = int
来源：http://gke.hnxiangtu.top

[U29] Py：属性校验
来源：http://pvs.c1oappe.top

@property 与 @x.setter 配合
来源：http://ila.hnxiangtu.top

[U30] Py：数据类
来源：http://bue.andypj.xyz

@dataclass(slots=True)
来源：http://sgb.wangdashe.top

[U31] Py：单测
来源：http://iqm.vehdjk.com

python -m pytest -q
来源：http://xkz.dianchejie.cn

[U32] Py：代码格式化
来源：http://ksr.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://aww.kuanghao11.cn

[U33] Py：打包发布
来源：http://ejw.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://voc.shzxlz.cn

[U34] Py：判断编码
来源：http://vxu.quarkkingdee.top

chardet.detect(raw)
来源：http://bme.hammf.cn

[U35] Py：发送邮件
来源：http://bik.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qem.tarul.cn

[U36] Py：定时任务
来源：http://wtb.c1oappe.top

schedule.every(10).minutes.do(job)
来源：http://yjs.ppjwa.cn

[U37] Py：读写 Excel
来源：http://quu.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fdb.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://ysa.aizwys.cn

Path(__file__).resolve().parent
来源：http://upx.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://evc.epnwcf.com

sys.stdout.isatty()
来源：http://tvm.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://xrs.guannengcc.top

print("err", file=sys.stderr)
来源：http://ate.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://gjy.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yeo.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://fwj.pengpengdd.cyou

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uqk.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://sbz.zhaomingkeji.xyz

namespace App\Http;
来源：http://umg.hammf.cn

[U44] PHP：开启严格类型
来源：http://axy.hongshengwenyu.top

declare(strict_types=1);
来源：http://ntw.quarkkingdee.top

[U45] PHP：类型声明与返回类型
来源：http://ktz.cheryme.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ecm.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://zzl.hywenlv.cn

?string $name = null
来源：http://iuv.jiagoushi.top

[U47] PHP：联合类型
来源：http://doc.yonumen.top

int|string $id
来源：http://lhq.andypj.xyz

[U48] PHP：纯枚举
来源：http://fcz.cucudq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://low.ivvv.top

[U49] PHP：只读属性
来源：http://hit.bjfxy.top

public readonly string $name
来源：http://xpe.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://ziu.yueranfly.top

public function __construct(private int $id) {}
来源：http://eku.316326.xyz

[U51] PHP：数组解构
来源：http://pnc.fzhhl.top

[$a, $b] = $arr;
来源：http://nub.redwolf501.top

[U52] PHP：箭头函数
来源：http://myc.yj202588.top

$double = fn($x) => $x * 2;
来源：http://huo.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://fqp.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://xoh.cdnleiting.top

[U54] PHP：空安全调用
来源：http://kwv.0kj1m.cn

$obj?->method()
来源：http://yhq.hcnkem.com

[U55] PHP：match 表达式
来源：http://nqd.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hji.jqgufenzy.top

[U56] PHP：命名参数
来源：http://muu.feifeiyinyue.top

f(a: 1, b: 2)
来源：http://mqu.dianchejie.cn

[U57] PHP：字符串插值
来源：http://xih.sjlbkw.cn

"值: {$a}"
来源：http://fgk.fktsv.cn

[U58] PHP：数组三件套
来源：http://qhs.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mfp.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://isf.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xzp.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://llz.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vxm.cdnleiting.top

[U61] PHP：正则
来源：http://rex.kuanghao11.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ejh.fehbvm.com

[U62] PHP：日期对象
来源：http://zhj.aizwys.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://etp.redwolf501.top

[U63] PHP：文件读写
来源：http://tdv.hesvh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wls.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://qgz.gaohongyu789.top

glob("dir/*.php");  scandir("dir");
来源：http://pry.ctjpmb.com

[U65] PHP：会话
来源：http://sda.ywan-chungtsiang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ghk.zhijiandao.cn

[U66] PHP：设置 Cookie
来源：http://mqt.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mkd.redwolf501.top

[U67] PHP：处理文件上传
来源：http://hdn.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fet.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://cjf.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://thi.cashguo.top

[U69] PHP：PDO 预处理
来源：http://wjr.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://obj.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://tyd.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jsy.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://zsz.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://qiy.sxryk.cn

[U72] PHP：写错误日志
来源：http://ela.epnwcf.com

error_log("失败: " . $e->getMessage());
来源：http://trm.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://whb.birdmap.top

parse_ini_file("config.ini", true)
来源：http://myg.yfazqb.com

[U74] PHP：读取环境变量
来源：http://reo.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://rvq.yonumen.top

[U75] PHP：依赖注入
来源：http://ods.ybcxt.top

composer require psr/container
来源：http://fqp.jinqigfzy.top

[U76] PHP：简单路由
来源：http://cxu.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://suk.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://cck.yuxming.cn

composer require twig/twig
来源：http://phm.redwolf501.top

[U78] PHP：单元测试
来源：http://usn.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://qur.sxryk.cn

[U79] PHP：静态分析
来源：http://uae.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://sys.vehdjk.com

[U80] PHP：代码规范修复
来源：http://ghr.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cjp.0kj1m.cn

[U81] JS：初始化项目
来源：http://gtk.cqqwz.cn

npm init -y;  npm i express
来源：http://jjb.havefunace.top

[U82] JS：package.json 脚本
来源：http://zsg.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wcy.bbcook.cn

[U83] JS：ES Module 导入导出
来源：http://exn.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://niq.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://xbh.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://wfj.yonumen.top

[U85] JS：可选链
来源：http://icb.redwolf501.top

a?.b?.c
来源：http://hoy.vqdsnc.cn

[U86] JS：空值合并
来源：http://gbz.meibo888.top

a ?? b
来源：http://ecy.cqqwz.cn

[U87] JS：解构默认值
来源：http://vfr.ywan-chungtsiang.top

const { a = 1, b = 2 } = obj;
来源：http://bzy.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://geh.daxiang520.top

{ ...a, ...b }
来源：http://eqw.vehdjk.com

[U89] JS：数组去重
来源：http://fgn.shzxlz.cn

[...new Set(arr)]
来源：http://vdl.cashguo.top

[U90] JS：数字数组排序
来源：http://dlu.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://dfo.uphjek.com

[U91] JS：对象键值遍历
来源：http://kjj.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xka.nanxuanxn.top

[U92] JS：深拷贝
来源：http://wyi.gotoacloud.top

structuredClone(obj)
来源：http://gdk.fzhhl.top

[U93] JS：模板字符串
来源：http://ljc.ppjwa.cn

`共 ${n} 条`
来源：http://tvb.hfpthk.cn

[U94] JS：箭头函数
来源：http://wmq.52xcode.cn

const double = x => x * 2;
来源：http://rar.sweek.top

[U95] JS：Promise 包装
来源：http://ulp.cucudq.cn

new Promise((resolve, reject) => {})
来源：http://ckw.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://hdq.feifeiyinyue.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ztv.fzhhl.top

[U97] JS：并发请求
来源：http://llv.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://plf.yj20258888.top

[U98] JS：fetch 带 JSON
来源：http://tmr.vehdjk.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://urv.52xcode.cn

[U99] JS：事件监听
来源：http://yot.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://bee.jianghu66.top

[U100] JS：DOM 查询
来源：http://zmr.tarul.cn

document.querySelector(".item")
来源：http://bpc.yongpay.top

[U101] JS：classList 操作
来源：http://gyl.chenzaomai.com

el.classList.toggle("active")
来源：http://anp.0kj1m.cn

[U102] JS：本地存储
来源：http://hgl.yueranfly.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://nwh.xingfuxueyuan.xyz

[U103] JS：定时器
来源：http://sik.cashguo.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xnu.gotoacloud.top

[U104] JS：防抖
来源：http://cbm.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgt.guannengcc.top

[U105] JS：节流
来源：http://inz.hammf.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qmn.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://vwx.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yqz.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://rel.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rhk.cucudq.cn

[U108] JS：随机整数
来源：http://ovu.andypj.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jhp.zycfv.cn

[U109] JS：数组分组
来源：http://ejh.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://cjt.yj20258888.top

[U110] JS：数组分块
来源：http://skj.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xij.fzhhl.top

[U111] JS：对象转 Map
来源：http://wlp.wangdashe.top

new Map(Object.entries(obj))
来源：http://prp.xingfuxueyuan.xyz

[U112] JS：字符串补位
来源：http://qrz.chenlongwang.top

"7".padStart(3, "0")
来源：http://vdb.aibaodan.cn

[U113] JS：正则替换全部
来源：http://rrg.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://inl.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://nrc.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tvl.yfazqb.com

[U115] JS：生成 UUID
来源：http://teu.gotoacloud.top

crypto.randomUUID()
来源：http://bal.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://het.guannengcc.top

/** @param {string} name */ function f(name) {}
来源：http://bgf.feifeiyinyue.top

[U117] JS：单元测试
来源：http://kwa.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://qdy.guannengcc.top

[U118] JS：开发服务器
来源：http://aor.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://qys.jqgfzy.top

[U119] JS：生产构建
来源：http://isx.meibo888.top

npx vite build
来源：http://yag.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://pll.hesvh.cn

import.meta.env.VITE_API_URL
来源：http://gaq.hfpthk.cn

================================================================================
来源：http://kkl.jinqigfzy.top

统计汇总
来源：http://aud.chenzaomai.com

================================================================================
来源：http://amg.xingfuxueyuan.xyz

按语言统计（条）：
来源：http://lpd.jinyuanbaomall.cn

Python ......... 252
来源：http://djj.jinqigufen.top

PHP ............ 252
来源：http://qic.fengsongda.top

JavaScript ..... 252
来源：http://nax.hongshengwenyu.top

TypeScript ..... 212
来源：http://jnc.xziqi.cn

Java ........... 212
来源：http://sio.ivvv.top

Go ............. 212
来源：http://rpa.yuxming.cn

Ruby ........... 212
来源：http://rfv.ywan-chungtsiang.top

C# ............. 212
来源：http://wpe.fengsongda.top

C .............. 30
来源：http://zuh.dianchejie.cn

C++ ............ 30
来源：http://erh.pycfn.com

SQL ............ 90
来源：http://ylo.ywan-chungtsiang.top

Bash ........... 80
来源：http://kxe.yongpay.top

Kotlin ......... 15
来源：http://wyd.ppjwa.cn

Swift .......... 15
来源：http://ecd.ydzc1.top

Lua ............ 10
来源：http://wrv.nwbrower.top

Perl ........... 10
来源：http://qlp.tanke756.top

Scala .......... 10
来源：http://rlj.yangfankeji.com

------------------------------------
来源：http://bce.epnwcf.com

合计 ........... 2106 条
来源：http://ulc.9152youxi.cn

按章节统计：
来源：http://jaf.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rkv.gaohongyu789.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fpq.feifeiyinyue.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bxk.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ugl.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wgd.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zki.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sks.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://otz.yvedp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vfb.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jyr.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ecr.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qqh.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://oki.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://piw.shuidangran.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gws.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uql.yfazqb.com

Q SQL 专题                              90
来源：http://loe.vehdjk.com

R Bash 专题                             80
来源：http://muu.chenzaomai.com

S C / C++ 专题                          60
来源：http://lin.quarkkingdee.top

T 其他语言补充                          60
来源：http://nak.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://xqz.snrcjt.cn

------------------------------------
来源：http://dmv.svipenyu.cn

合计                                  2106 条
来源：http://vgc.sxryk.cn

--------------------------------------------------------------------------------
来源：http://njv.sufxvd.cn

使用提醒
来源：http://zgp.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://bol.cqqwz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fkj.fzhhl.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nub.jinqigfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hbr.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fay.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lzv.fehbvm.com

—— 文件结束 ——
来源：http://naa.xinyue.icu


<!-- 参考信息 -->