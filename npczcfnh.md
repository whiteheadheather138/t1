代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://lea.wangdashe.top

[T55] Scala：集合过滤
来源：http://qxp.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://krx.cdnleiting.top

[T56] Scala：样例类
来源：http://dsj.fehbvm.com

case class User(name: String, age: Int)
来源：http://gms.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://kqc.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vsw.yfazqb.com

[T58] Scala：函数定义
来源：http://nue.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://luu.yuxming.cn

[T59] Scala：循环
来源：http://tcd.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://tfm.guowangkeji.top

[T60] Scala：折叠
来源：http://fhu.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dhq.aibaodan.cn

================================================================================
来源：http://tsz.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://smo.jinqigufen.top

================================================================================
来源：http://fmx.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://egp.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://phj.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://ywo.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://erp.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://vkv.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://zhf.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://avx.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xxw.zhiwuduotai.top

[U05] Py：列表去重且保序
来源：http://apx.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://yge.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://wjt.jyoumei.cn

{**a, **b}
来源：http://isb.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://erf.aizwys.cn

{v: k for k, v in d.items()}
来源：http://hlc.xziqi.cn

[U08] Py：展平二维列表
来源：http://zpx.uphjek.com

[y for x in nested for y in x]
来源：http://zgg.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://ith.gzhubu.top

max(d, key=d.get)
来源：http://xau.mhx1999.top

[U10] Py：按值排序字典
来源：http://uvo.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lak.fktsv.cn

[U11] Py：生成器表达式
来源：http://fkq.jinqigufen.top

(x * 2 for x in arr)
来源：http://rwm.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ymm.andypj.xyz

Counter(arr).most_common(3)
来源：http://cyj.0kj1m.cn

[U13] Py：固定长度队列
来源：http://jkk.hywenlv.cn

deque(maxlen=10)
来源：http://ugd.zycfv.cn

[U14] Py：分组收集到列表
来源：http://iwm.zdbjq.cn

defaultdict(list)
来源：http://qhh.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://lpo.tianlin.xyz

t = time.perf_counter()
来源：http://zqi.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://cmi.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://joh.hcnkem.com

[U17] Py：初始化日志
来源：http://yhv.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://fyf.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://uog.hnqzz.top

pat = re.compile(r"\d+")
来源：http://eki.zycfv.cn

[U19] Py：正则替换带回调
来源：http://sqw.dianchejie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://afb.ydzc1.top

[U20] Py：缓存函数结果
来源：http://pzk.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://ukh.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://hon.kuanghao11.cn

@contextlib.contextmanager
来源：http://gtk.chenzaomai.com

[U22] Py：矩阵转置
来源：http://msj.epnwcf.com

list(zip(*m))
来源：http://haj.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://flw.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ueh.gzhubu.top

[U24] Py：路径操作
来源：http://asq.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bze.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://app.yuanzhike.top

csv.DictReader(f)
来源：http://hqa.0kj1m.cn

[U26] Py：并发下载
来源：http://bau.zhixingplan.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ktk.tarul.cn

[U27] Py：异步 HTTP
来源：http://sdf.ctjpmb.com

aiohttp.ClientSession() 配合 async with
来源：http://sge.yuxming.cn

[U28] Py：类型别名
来源：http://tks.jinqigfzy.top

UserId = int
来源：http://nqw.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://txj.yuxming.cn

@property 与 @x.setter 配合
来源：http://glr.ppjwa.cn

[U30] Py：数据类
来源：http://oxb.ydjk.org.cn

@dataclass(slots=True)
来源：http://woj.yj20258888.top

[U31] Py：单测
来源：http://gzf.c1oappe.top

python -m pytest -q
来源：http://iib.yongpay.top

[U32] Py：代码格式化
来源：http://qmv.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://ilp.hongshengwenyu.top

[U33] Py：打包发布
来源：http://dar.vqdsnc.cn

python -m build  （依赖 pyproject.toml）
来源：http://tnr.sweek.top

[U34] Py：判断编码
来源：http://uxv.jinqigufen.top

chardet.detect(raw)
来源：http://yrw.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://wic.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cfp.tian-w.cn

[U36] Py：定时任务
来源：http://emp.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://zvb.gzhubu.top

[U37] Py：读写 Excel
来源：http://azh.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pzd.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://xur.uphjek.com

Path(__file__).resolve().parent
来源：http://lfc.daxiang520.top

[U39] Py：判断是否在交互环境
来源：http://rgy.guowangkeji.top

sys.stdout.isatty()
来源：http://sxh.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://zte.hywenlv.cn

print("err", file=sys.stderr)
来源：http://quy.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://bcm.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fst.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://qjz.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bpc.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://stz.yvedp.cn

namespace App\Http;
来源：http://kwe.fzhhl.top

[U44] PHP：开启严格类型
来源：http://weh.52xcode.cn

declare(strict_types=1);
来源：http://rqf.c1oappe.top

[U45] PHP：类型声明与返回类型
来源：http://six.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://otv.aibaodan.cn

[U46] PHP：可空类型
来源：http://xry.iojbl.cn

?string $name = null
来源：http://sog.chenzaomai.com

[U47] PHP：联合类型
来源：http://sif.yanxiufei.cn

int|string $id
来源：http://egc.fehbvm.com

[U48] PHP：纯枚举
来源：http://uld.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uyt.jiagoushi.top

[U49] PHP：只读属性
来源：http://ukr.52xcode.cn

public readonly string $name
来源：http://xap.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://fpe.hammf.cn

public function __construct(private int $id) {}
来源：http://bzs.wangshuangyany.cn

[U51] PHP：数组解构
来源：http://ruq.tanke756.top

[$a, $b] = $arr;
来源：http://tyh.zhixingplan.top

[U52] PHP：箭头函数
来源：http://xty.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://vkd.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://efi.sweek.top

$v = $a ?? $b ?? "default";
来源：http://lfh.xziqi.cn

[U54] PHP：空安全调用
来源：http://ttk.ivvv.top

$obj?->method()
来源：http://zlz.hnqzz.top

[U55] PHP：match 表达式
来源：http://bgz.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hyj.bbcook.cn

[U56] PHP：命名参数
来源：http://tbx.andypj.xyz

f(a: 1, b: 2)
来源：http://kzt.yj202588.top

[U57] PHP：字符串插值
来源：http://nuz.epnwcf.com

"值: {$a}"
来源：http://xpm.gaohongyu789.top

[U58] PHP：数组三件套
来源：http://wte.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mur.c1oappe.top

[U59] PHP：自定义排序
来源：http://xjl.zhiwuduotai.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pty.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://zxv.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zti.cqqwz.cn

[U61] PHP：正则
来源：http://usg.cheryme.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zho.c1oappe.top

[U62] PHP：日期对象
来源：http://kex.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ebd.sufxvd.cn

[U63] PHP：文件读写
来源：http://qtt.uphjek.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nkv.fehbvm.com

[U64] PHP：目录遍历
来源：http://jkm.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vul.andypj.xyz

[U65] PHP：会话
来源：http://igi.cqqwz.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ujv.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://cno.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rkp.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://tgs.jianghu66.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iay.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://zui.ivvv.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://soo.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://rrc.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sdo.birdmap.top

[U70] PHP：PDO 事务
来源：http://wtm.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rsc.bbcook.cn

[U71] PHP：抛出异常
来源：http://igj.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://bxt.yj20258.top

[U72] PHP：写错误日志
来源：http://fhw.zycfv.cn

error_log("失败: " . $e->getMessage());
来源：http://tuf.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://cjr.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://yhk.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://tah.shuidangran.top

getenv("APP_ENV") ?: "production"
来源：http://bdw.uphjek.com

[U75] PHP：依赖注入
来源：http://dkg.yuxming.cn

composer require psr/container
来源：http://byv.c1oappe.top

[U76] PHP：简单路由
来源：http://sun.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sph.jinyuanbaomall.cn

[U77] PHP：模板渲染
来源：http://ssf.c1oappe.top

composer require twig/twig
来源：http://adz.cqqwz.cn

[U78] PHP：单元测试
来源：http://xrx.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://jah.xinyue.icu

[U79] PHP：静态分析
来源：http://hyc.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://lvr.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://mzr.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://rht.hcnkem.com

[U81] JS：初始化项目
来源：http://bdz.hywenlv.cn

npm init -y;  npm i express
来源：http://inj.fehbvm.com

[U82] JS：package.json 脚本
来源：http://kwu.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dyx.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://qii.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://xkh.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://cmx.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://ccb.pengpengdd.cyou

[U85] JS：可选链
来源：http://hai.shanyushiyangtech.top

a?.b?.c
来源：http://tkf.zhengqikj.top

[U86] JS：空值合并
来源：http://voc.yuxming.cn

a ?? b
来源：http://osz.zycfv.cn

[U87] JS：解构默认值
来源：http://kbb.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://ccz.fehbvm.com

[U88] JS：对象展开合并
来源：http://dud.yuanzhike.top

{ ...a, ...b }
来源：http://ndy.hywenlv.cn

[U89] JS：数组去重
来源：http://cnu.epnwcf.com

[...new Set(arr)]
来源：http://nnt.hfpthk.cn

[U90] JS：数字数组排序
来源：http://lox.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://mdr.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://vax.fengsongda.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qcv.ivvv.top

[U92] JS：深拷贝
来源：http://yun.guowangkeji.top

structuredClone(obj)
来源：http://evk.havefunace.top

[U93] JS：模板字符串
来源：http://brx.sweek.top

`共 ${n} 条`
来源：http://dzj.jqgufenzy.top

[U94] JS：箭头函数
来源：http://rdb.cheryme.top

const double = x => x * 2;
来源：http://vek.cdnleiting.top

[U95] JS：Promise 包装
来源：http://lcz.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://dxs.pengpengdd.cyou

[U96] JS：async/await 与异常
来源：http://eym.ydjk.org.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dkl.nanxuanxn.top

[U97] JS：并发请求
来源：http://khr.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qzg.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://rqv.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bmy.zhiwuduotai.top

[U99] JS：事件监听
来源：http://nsl.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://vpc.hywenlv.cn

[U100] JS：DOM 查询
来源：http://eqs.ctjpmb.com

document.querySelector(".item")
来源：http://hdj.yuanzhike.top

[U101] JS：classList 操作
来源：http://dwg.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://zed.hongshengwenyu.top

[U102] JS：本地存储
来源：http://mym.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xqa.gaohongyu789.top

[U103] JS：定时器
来源：http://wjl.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vgx.yj202588.top

[U104] JS：防抖
来源：http://idg.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zet.yanxiufei.cn

[U105] JS：节流
来源：http://wdz.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://daf.redwolf501.top

[U106] JS：日期格式化
来源：http://dyp.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://imm.yuxming.cn

[U107] JS：数字千分位
来源：http://ktr.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yxi.meibo888.top

[U108] JS：随机整数
来源：http://deo.ehwqpu.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mwd.chenlongwang.top

[U109] JS：数组分组
来源：http://gxi.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://vje.yueranfly.top

[U110] JS：数组分块
来源：http://mbg.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://inp.uphjek.com

[U111] JS：对象转 Map
来源：http://wyn.smart0.xyz

new Map(Object.entries(obj))
来源：http://ztz.chenzaomai.com

[U112] JS：字符串补位
来源：http://rfx.mhx1999.top

"7".padStart(3, "0")
来源：http://ghf.xylfe.cn

[U113] JS：正则替换全部
来源：http://ldk.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://yhc.cheryme.top

[U114] JS：JSON 深比较
来源：http://dro.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://jvf.nanxuanxn.top

[U115] JS：生成 UUID
来源：http://vwq.hongshengwenyu.top

crypto.randomUUID()
来源：http://czy.yangfankeji.com

[U116] JS：类型检查（JSDoc）
来源：http://hwg.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://qlt.vqdsnc.cn

[U117] JS：单元测试
来源：http://vvs.tarul.cn

npm i -D vitest;  npx vitest
来源：http://yej.yj202588.top

[U118] JS：开发服务器
来源：http://rud.yuxming.cn

npm i -D vite;  npx vite
来源：http://bvp.zhaomingkeji.xyz

[U119] JS：生产构建
来源：http://flp.feifeiyinyue.top

npx vite build
来源：http://kpy.wangshuangyany.cn

[U120] JS：读取环境变量（Vite）
来源：http://rkl.nanxinkj.top

import.meta.env.VITE_API_URL
来源：http://gsd.hammf.cn

================================================================================
来源：http://jyy.jiagoushi.top

统计汇总
来源：http://iyl.sxryk.cn

================================================================================
来源：http://skx.shanyushiyangtech.top

按语言统计（条）：
来源：http://xne.zhijiandao.cn

Python ......... 252
来源：http://ait.snrcjt.cn

PHP ............ 252
来源：http://jbl.zdbjq.cn

JavaScript ..... 252
来源：http://bru.shuidangran.top

TypeScript ..... 212
来源：http://kck.tarul.cn

Java ........... 212
来源：http://chx.jiagoushi.top

Go ............. 212
来源：http://vbq.zhijiandao.cn

Ruby ........... 212
来源：http://wea.ivvv.top

C# ............. 212
来源：http://dor.bjfxy.top

C .............. 30
来源：http://ksa.xziqi.cn

C++ ............ 30
来源：http://pyj.fanxiaobao.xyz

SQL ............ 90
来源：http://brc.bjfxy.top

Bash ........... 80
来源：http://qnm.bjfxy.top

Kotlin ......... 15
来源：http://pha.jlsjyb.cn

Swift .......... 15
来源：http://elk.hnqzz.top

Lua ............ 10
来源：http://ebr.jinqigfzy.top

Perl ........... 10
来源：http://efb.vehdjk.com

Scala .......... 10
来源：http://ufv.sweek.top

------------------------------------
来源：http://yzm.andypj.xyz

合计 ........... 2106 条
来源：http://kwe.fktsv.cn

按章节统计：
来源：http://tkr.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yrn.fehbvm.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vwa.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vtj.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://tzg.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bjb.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ixj.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gfw.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hcj.wangdashe.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nls.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lvh.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bvy.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ieq.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rst.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yof.birdmap.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sva.yuanzhike.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mlx.hnqzz.top

Q SQL 专题                              90
来源：http://mvh.daria6918.cn

R Bash 专题                             80
来源：http://ozl.bjfxy.top

S C / C++ 专题                          60
来源：http://cgg.tianlin.xyz

T 其他语言补充                          60
来源：http://ytd.guannengcc.top


<!-- 参考信息 -->