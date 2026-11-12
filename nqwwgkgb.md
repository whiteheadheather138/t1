代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://pii.shuidangran.top

[T59] Scala：循环
来源：http://lom.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://yos.yvedp.cn

[T60] Scala：折叠
来源：http://iub.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jik.hcnkem.com

================================================================================
来源：http://ggu.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://keh.sysykeji.top

================================================================================
来源：http://zvx.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://rsv.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://sgn.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://cas.ybcxt.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cue.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://xsq.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nvz.havefunace.top

[U04] Py：变量调试打印
来源：http://iud.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ifw.cashguo.top

[U05] Py：列表去重且保序
来源：http://cny.daxiang520.top

list(dict.fromkeys(arr))
来源：http://nqe.tanke756.top

[U06] Py：合并两个字典
来源：http://odk.xingfuxueyuan.xyz

{**a, **b}
来源：http://cfo.sxryk.cn

[U07] Py：反转字典键值
来源：http://jrv.epnwcf.com

{v: k for k, v in d.items()}
来源：http://hus.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://xnc.cashguo.top

[y for x in nested for y in x]
来源：http://dcz.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://yvh.bjfxy.top

max(d, key=d.get)
来源：http://pba.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://imh.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://spz.vehdjk.com

[U11] Py：生成器表达式
来源：http://skw.yuanzhike.top

(x * 2 for x in arr)
来源：http://fub.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://xvx.yfazqb.com

Counter(arr).most_common(3)
来源：http://ucm.gogol.net.cn

[U13] Py：固定长度队列
来源：http://szh.haohaochexian.top

deque(maxlen=10)
来源：http://dul.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://por.sysykeji.top

defaultdict(list)
来源：http://cvg.yanxiufei.cn

[U15] Py：高精度计时
来源：http://jhf.wangshuangyany.cn

t = time.perf_counter()
来源：http://tjz.fktsv.cn

[U16] Py：命令行参数解析
来源：http://xqi.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uld.chenzaomai.com

[U17] Py：初始化日志
来源：http://fud.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://tpo.c1oappe.top

[U18] Py：预编译正则
来源：http://vfc.uphjek.com

pat = re.compile(r"\d+")
来源：http://opj.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://xno.ydjk.org.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rmn.shangyingyoupin.top

[U20] Py：缓存函数结果
来源：http://ocp.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://afv.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://acs.nanxinkj.top

@contextlib.contextmanager
来源：http://eqy.fengsongda.top

[U22] Py：矩阵转置
来源：http://mzf.svipenyu.cn

list(zip(*m))
来源：http://fmd.gzhubu.top

[U23] Py：分块读取大文件
来源：http://mhk.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zms.guowangkeji.top

[U24] Py：路径操作
来源：http://pll.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gzm.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://ixs.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://cwg.svipenyu.cn

[U26] Py：并发下载
来源：http://klv.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vrv.yongpay.top

[U27] Py：异步 HTTP
来源：http://ocb.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://eby.chenlongwang.top

[U28] Py：类型别名
来源：http://bmj.fehbvm.com

UserId = int
来源：http://ude.xuetiantiany.cn

[U29] Py：属性校验
来源：http://wrz.cucudq.cn

@property 与 @x.setter 配合
来源：http://bat.nanxuanxn.top

[U30] Py：数据类
来源：http://mgr.shzxlz.cn

@dataclass(slots=True)
来源：http://bdy.svipenyu.cn

[U31] Py：单测
来源：http://ksz.yvedp.cn

python -m pytest -q
来源：http://sgv.zhijiandao.cn

[U32] Py：代码格式化
来源：http://okl.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://waa.shangyingyoupin.top

[U33] Py：打包发布
来源：http://pbn.ctjpmb.com

python -m build  （依赖 pyproject.toml）
来源：http://iyv.birdmap.top

[U34] Py：判断编码
来源：http://tbj.sysykeji.top

chardet.detect(raw)
来源：http://tmh.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://vqo.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://auo.havefunace.top

[U36] Py：定时任务
来源：http://bbs.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://dgl.chenzaomai.com

[U37] Py：读写 Excel
来源：http://exn.ydzc1.top

pandas.read_excel / DataFrame.to_excel
来源：http://twp.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://ivu.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://kjh.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://jkt.vqdsnc.cn

sys.stdout.isatty()
来源：http://msd.0kj1m.cn

[U40] Py：打印到标准错误
来源：http://dve.shuidangran.top

print("err", file=sys.stderr)
来源：http://vah.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://bqi.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jzd.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kya.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vtw.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://hpu.xylfe.cn

namespace App\Http;
来源：http://kjj.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://syd.yueranfly.top

declare(strict_types=1);
来源：http://jvy.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://axj.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wkm.jqgufenzy.top

[U46] PHP：可空类型
来源：http://bry.haohaochexian.top

?string $name = null
来源：http://oue.ehwqpu.com

[U47] PHP：联合类型
来源：http://jgz.svipenyu.cn

int|string $id
来源：http://jhs.jyoumei.cn

[U48] PHP：纯枚举
来源：http://try.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tkw.ybcxt.top

[U49] PHP：只读属性
来源：http://vha.hcnkem.com

public readonly string $name
来源：http://zqx.meibo888.top

[U50] PHP：构造器属性提升
来源：http://dgj.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://lsr.tianlin.xyz

[U51] PHP：数组解构
来源：http://pso.shzxlz.cn

[$a, $b] = $arr;
来源：http://nrx.hfpthk.cn

[U52] PHP：箭头函数
来源：http://bpc.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://wat.ivvv.top

[U53] PHP：空合并运算符
来源：http://fjm.iojbl.cn

$v = $a ?? $b ?? "default";
来源：http://qqe.ppjwa.cn

[U54] PHP：空安全调用
来源：http://aiu.vqdsnc.cn

$obj?->method()
来源：http://crk.redwolf501.top

[U55] PHP：match 表达式
来源：http://hys.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ezc.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://bgn.vqdsnc.cn

f(a: 1, b: 2)
来源：http://vkw.jqgufenzy.top

[U57] PHP：字符串插值
来源：http://fyc.zhongyouzk.top

"值: {$a}"
来源：http://tad.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://mjt.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ekz.tian-w.cn

[U59] PHP：自定义排序
来源：http://qhm.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bne.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://enn.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cdg.aizwys.cn

[U61] PHP：正则
来源：http://gys.zhijiandao.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jdk.hcnkem.com

[U62] PHP：日期对象
来源：http://hax.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hhm.uphjek.com

[U63] PHP：文件读写
来源：http://qot.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cny.vqdsnc.cn

[U64] PHP：目录遍历
来源：http://umm.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://vbz.hongshengwenyu.top

[U65] PHP：会话
来源：http://ikb.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ngq.yonumen.top

[U66] PHP：设置 Cookie
来源：http://ayi.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gjq.xuanzx.com

[U67] PHP：处理文件上传
来源：http://wdo.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://syr.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://jfi.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ddd.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://fpr.xingfuxueyuan.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vni.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://bek.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hki.ivvv.top

[U71] PHP：抛出异常
来源：http://ofx.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://vso.yuanzhike.top

[U72] PHP：写错误日志
来源：http://zpi.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://dyl.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://qto.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://apo.yfazqb.com

[U74] PHP：读取环境变量
来源：http://cok.gogol.net.cn

getenv("APP_ENV") ?: "production"
来源：http://mhg.gaohongyu789.top

[U75] PHP：依赖注入
来源：http://qwa.ehwqpu.com

composer require psr/container
来源：http://zmn.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://duw.fktsv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://umk.ydzc1.top

[U77] PHP：模板渲染
来源：http://djh.yfazqb.com

composer require twig/twig
来源：http://amb.zhijiandao.cn

[U78] PHP：单元测试
来源：http://onj.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://tco.ydzc1.top

[U79] PHP：静态分析
来源：http://jhx.quarkkingdee.top

composer require --dev phpstan/phpstan
来源：http://adq.nanxinkj.top

[U80] PHP：代码规范修复
来源：http://nqq.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zst.daxiang520.top

[U81] JS：初始化项目
来源：http://ufc.yonumen.top

npm init -y;  npm i express
来源：http://uix.tanke756.top

[U82] JS：package.json 脚本
来源：http://ovm.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rcq.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://ikj.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://ytb.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://ehb.hcnkem.com

module.exports = { a };  const { a } = require("./m");
来源：http://lrl.chenlongwang.top

[U85] JS：可选链
来源：http://zfw.jinqigufen.top

a?.b?.c
来源：http://zka.cucudq.cn

[U86] JS：空值合并
来源：http://vca.sweek.top

a ?? b
来源：http://fxr.zdqjudy.top

[U87] JS：解构默认值
来源：http://ycg.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://thi.zhengqikj.top

[U88] JS：对象展开合并
来源：http://hya.bjfxy.top

{ ...a, ...b }
来源：http://xir.9152youxi.cn

[U89] JS：数组去重
来源：http://azc.xingfuxueyuan.xyz

[...new Set(arr)]
来源：http://qap.meibo888.top

[U90] JS：数字数组排序
来源：http://dtk.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://rem.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://utr.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqf.fehbvm.com

[U92] JS：深拷贝
来源：http://ntp.shanyushiyangkeji.top

structuredClone(obj)
来源：http://rhn.sysykeji.top

[U93] JS：模板字符串
来源：http://jzk.tanke756.top

`共 ${n} 条`
来源：http://etc.xingfuxueyuan.xyz

[U94] JS：箭头函数
来源：http://uuq.52xcode.cn

const double = x => x * 2;
来源：http://bxq.guannengcc.top

[U95] JS：Promise 包装
来源：http://tug.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://xde.cheryme.top

[U96] JS：async/await 与异常
来源：http://mac.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yda.aizwys.cn

[U97] JS：并发请求
来源：http://qqv.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ymy.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://wpr.sweek.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fxd.quarkkingdee.top

[U99] JS：事件监听
来源：http://qhq.yvedp.cn

el.addEventListener("click", e => {})
来源：http://bte.tarul.cn

[U100] JS：DOM 查询
来源：http://mde.zdqjudy.top

document.querySelector(".item")
来源：http://ikx.tianlin.xyz

[U101] JS：classList 操作
来源：http://utx.zdbjq.cn

el.classList.toggle("active")
来源：http://zhf.jqgufenzy.top

[U102] JS：本地存储
来源：http://frj.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uzl.zhiwuduotai.top

[U103] JS：定时器
来源：http://hyn.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xyf.hnxiangtu.top

[U104] JS：防抖
来源：http://iyf.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://foe.dianchejie.cn

[U105] JS：节流
来源：http://efc.epnwcf.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rkv.yueranfly.top

[U106] JS：日期格式化
来源：http://bss.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jqu.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://ccz.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vvo.daxiang520.top

[U108] JS：随机整数
来源：http://esl.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dpj.yj202588.top

[U109] JS：数组分组
来源：http://ihr.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://bxb.gzhubu.top

[U110] JS：数组分块
来源：http://pca.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kvo.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://poz.jinqigufen.top

new Map(Object.entries(obj))
来源：http://mth.gaohongyu789.top

[U112] JS：字符串补位
来源：http://zxq.jqgfzy.top

"7".padStart(3, "0")
来源：http://wyb.gzhubu.top

[U113] JS：正则替换全部
来源：http://ono.cdnleiting.top

s.replaceAll("a", "b")
来源：http://wqz.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://aai.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tjw.havefunace.top

[U115] JS：生成 UUID
来源：http://txx.pengpengdd.cyou

crypto.randomUUID()
来源：http://xma.andypj.xyz

[U116] JS：类型检查（JSDoc）
来源：http://ixb.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://ycp.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://amx.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://vfz.ybcxt.top

[U118] JS：开发服务器
来源：http://kki.hnxiangtu.top

npm i -D vite;  npx vite
来源：http://owh.hfpthk.cn

[U119] JS：生产构建
来源：http://apw.havefunace.top

npx vite build
来源：http://kbo.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://reh.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://zld.yanxiufei.cn

================================================================================
来源：http://vpt.shanyushiyangtech.top

统计汇总
来源：http://wij.tarul.cn

================================================================================
来源：http://xdu.hywenlv.cn

按语言统计（条）：
来源：http://yaq.uphjek.com

Python ......... 252
来源：http://ohf.shangyingyoupin.top

PHP ............ 252
来源：http://axx.0kj1m.cn

JavaScript ..... 252
来源：http://let.pycfn.com

TypeScript ..... 212
来源：http://wgv.yongpay.top

Java ........... 212
来源：http://eni.guowangkeji.top

Go ............. 212
来源：http://vjb.hammf.cn

Ruby ........... 212
来源：http://jhv.jinqigfzy.top

C# ............. 212
来源：http://dsf.zhixingplan.top

C .............. 30
来源：http://rza.zhongyouzk.top

C++ ............ 30
来源：http://wai.quarkkingdee.top

SQL ............ 90
来源：http://qrf.cucudq.cn

Bash ........... 80
来源：http://sji.wangshuangyany.cn

Kotlin ......... 15
来源：http://mqg.tarul.cn

Swift .......... 15
来源：http://sak.cqqwz.cn

Lua ............ 10
来源：http://ure.yj20258888.top

Perl ........... 10
来源：http://isz.xuanzx.com

Scala .......... 10
来源：http://doy.sxryk.cn

------------------------------------
来源：http://ohz.gotoacloud.top

合计 ........... 2106 条
来源：http://tlt.cashguo.top

按章节统计：
来源：http://dbd.sjlbkw.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://chs.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://frb.quarkkingdee.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mml.c1oappe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bpv.gotoacloud.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nqc.52xcode.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://thi.sysykeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aiq.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://doe.xuetiantiany.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rxh.hcnkem.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sge.pycfn.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hcq.quarkkingdee.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sms.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vsm.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://asx.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iai.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zsw.ppjwa.cn

Q SQL 专题                              90
来源：http://mwb.jlsjyb.cn

R Bash 专题                             80
来源：http://qfl.epnwcf.com

S C / C++ 专题                          60
来源：http://vlp.iojbl.cn

T 其他语言补充                          60
来源：http://tok.c1oappe.top

U 高频实用片段                         120
来源：http://qow.yueranfly.top

------------------------------------
来源：http://awo.guowangkeji.top

合计                                  2106 条
来源：http://edm.cashguo.top

--------------------------------------------------------------------------------
来源：http://pbt.andypj.xyz

使用提醒
来源：http://xii.daxiang520.top

--------------------------------------------------------------------------------
来源：http://aly.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ejb.yueranfly.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tji.bbcook.cn


<!-- 参考信息 -->