代发 wailian999

case class User(name: String, age: Int)
来源：http://qwg.zhixingplan.top

[T57] Scala：模式匹配
来源：http://cvp.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mos.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://lpb.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://gql.kuanghao11.cn

[T59] Scala：循环
来源：http://elb.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://xed.zhoulong.xyz

[T60] Scala：折叠
来源：http://qmi.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pkl.vehdjk.com

================================================================================
来源：http://rmd.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qbv.hesvh.cn

================================================================================
来源：http://vxj.zhiwuduotai.top

[U01] Py：创建虚拟环境
来源：http://nol.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mrg.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://omm.yonumen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://soz.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://dqh.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yjz.vehdjk.com

[U04] Py：变量调试打印
来源：http://xcs.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://skv.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://aye.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://bba.sweek.top

[U06] Py：合并两个字典
来源：http://ofp.zhoulong.xyz

{**a, **b}
来源：http://ygx.ctjpmb.com

[U07] Py：反转字典键值
来源：http://naq.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://gcp.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://ezo.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://zby.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://vtn.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://cce.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://fxy.tarul.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jkp.tianlin.xyz

[U11] Py：生成器表达式
来源：http://dlo.zhengqikj.top

(x * 2 for x in arr)
来源：http://vcn.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://fzt.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://gnk.chenlongwang.top

[U13] Py：固定长度队列
来源：http://uqy.sjlbkw.cn

deque(maxlen=10)
来源：http://iea.hnqzz.top

[U14] Py：分组收集到列表
来源：http://svr.xylfe.cn

defaultdict(list)
来源：http://yqw.zhixingplan.top

[U15] Py：高精度计时
来源：http://tjq.chenzaomai.com

t = time.perf_counter()
来源：http://ehl.shuidangran.top

[U16] Py：命令行参数解析
来源：http://qlr.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ixp.316326.xyz

[U17] Py：初始化日志
来源：http://vwp.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://yac.redwolf501.top

[U18] Py：预编译正则
来源：http://iac.yj202588.top

pat = re.compile(r"\d+")
来源：http://zst.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://iup.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oir.fengsongda.top

[U20] Py：缓存函数结果
来源：http://lts.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://uqh.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://hly.andypj.xyz

@contextlib.contextmanager
来源：http://zit.hesvh.cn

[U22] Py：矩阵转置
来源：http://hdd.ppjwa.cn

list(zip(*m))
来源：http://aun.tian-w.cn

[U23] Py：分块读取大文件
来源：http://ioo.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://roe.gzhubu.top

[U24] Py：路径操作
来源：http://imq.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rpf.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://khp.hongshengwenyu.top

csv.DictReader(f)
来源：http://sgj.xuetiantiany.cn

[U26] Py：并发下载
来源：http://kei.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gzo.bbcook.cn

[U27] Py：异步 HTTP
来源：http://kdz.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://sjf.yj202588.top

[U28] Py：类型别名
来源：http://ccl.yj20258.top

UserId = int
来源：http://rsv.cdnleiting.top

[U29] Py：属性校验
来源：http://itv.fengsongda.top

@property 与 @x.setter 配合
来源：http://pwq.pengpengdd.cyou

[U30] Py：数据类
来源：http://bhx.zhixingplan.top

@dataclass(slots=True)
来源：http://qqi.yueranfly.top

[U31] Py：单测
来源：http://vpc.chenjidiqi.icu

python -m pytest -q
来源：http://fid.zhixingplan.top

[U32] Py：代码格式化
来源：http://pwt.sysykeji.top

ruff format . && ruff check --fix .
来源：http://now.chenjidiqi.icu

[U33] Py：打包发布
来源：http://cof.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://afu.yonumen.top

[U34] Py：判断编码
来源：http://hjo.ppjwa.cn

chardet.detect(raw)
来源：http://irt.snrcjt.cn

[U35] Py：发送邮件
来源：http://nun.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://stg.cdnleiting.top

[U36] Py：定时任务
来源：http://qff.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://vra.yj20258888.top

[U37] Py：读写 Excel
来源：http://unr.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://urk.fzhhl.top

[U38] Py：获取脚本所在目录
来源：http://oed.hcnkem.com

Path(__file__).resolve().parent
来源：http://cug.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://ved.smart0.xyz

sys.stdout.isatty()
来源：http://uwj.xinyue.icu

[U40] Py：打印到标准错误
来源：http://gec.vehdjk.com

print("err", file=sys.stderr)
来源：http://awm.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://hkh.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://enr.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://emf.cdnleiting.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ohl.andypj.xyz

[U43] PHP：声明命名空间
来源：http://ark.snrcjt.cn

namespace App\Http;
来源：http://pog.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://acf.daxiang520.top

declare(strict_types=1);
来源：http://omo.andypj.xyz

[U45] PHP：类型声明与返回类型
来源：http://eis.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://omp.zycfv.cn

[U46] PHP：可空类型
来源：http://xqs.ybcxt.top

?string $name = null
来源：http://qzi.chenlongwang.top

[U47] PHP：联合类型
来源：http://uxr.nwbrower.top

int|string $id
来源：http://kry.gogol.net.cn

[U48] PHP：纯枚举
来源：http://zzi.ybcxt.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://npz.daxiang520.top

[U49] PHP：只读属性
来源：http://vfz.shangyingyoupin.top

public readonly string $name
来源：http://dkm.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://qdv.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://vnj.hywenlv.cn

[U51] PHP：数组解构
来源：http://scv.sweek.top

[$a, $b] = $arr;
来源：http://rha.chenlongwang.top

[U52] PHP：箭头函数
来源：http://dvz.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://eks.fehbvm.com

[U53] PHP：空合并运算符
来源：http://pyc.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://hjw.nanxinkj.top

[U54] PHP：空安全调用
来源：http://zvu.ehwqpu.com

$obj?->method()
来源：http://pvt.guowangkeji.top

[U55] PHP：match 表达式
来源：http://llz.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fsn.xuanzx.com

[U56] PHP：命名参数
来源：http://dnk.bbcook.cn

f(a: 1, b: 2)
来源：http://ygg.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://ava.hfpthk.cn

"值: {$a}"
来源：http://eqi.ehwqpu.com

[U58] PHP：数组三件套
来源：http://vll.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gbi.sxryk.cn

[U59] PHP：自定义排序
来源：http://sty.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aaq.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://bic.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ctj.hongshengwenyu.top

[U61] PHP：正则
来源：http://ntg.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gbp.hnxiangtu.top

[U62] PHP：日期对象
来源：http://red.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yni.aizwys.cn

[U63] PHP：文件读写
来源：http://cyc.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hyf.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://xaa.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ezk.hesvh.cn

[U65] PHP：会话
来源：http://xpu.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dre.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://tge.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vla.hcnkem.com

[U67] PHP：处理文件上传
来源：http://ety.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lvx.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://icw.jinyuanbaomall.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jwf.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://qvk.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rxr.hywenlv.cn

[U70] PHP：PDO 事务
来源：http://gmj.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ydf.birdmap.top

[U71] PHP：抛出异常
来源：http://wgv.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://red.c1oappe.top

[U72] PHP：写错误日志
来源：http://ski.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://pge.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://kbi.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://tje.jqgfzy.top

[U74] PHP：读取环境变量
来源：http://vzy.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://rwr.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://mvr.iojbl.cn

composer require psr/container
来源：http://oev.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://lxq.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fsb.nwbrower.top

[U77] PHP：模板渲染
来源：http://wra.xziqi.cn

composer require twig/twig
来源：http://njb.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://srb.fanxiaobao.xyz

composer require --dev phpunit/phpunit
来源：http://zsl.bjfxy.top

[U79] PHP：静态分析
来源：http://pwi.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://wid.tarul.cn

[U80] PHP：代码规范修复
来源：http://kng.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://itq.ehwqpu.com

[U81] JS：初始化项目
来源：http://nro.ehwqpu.com

npm init -y;  npm i express
来源：http://xgd.yongpay.top

[U82] JS：package.json 脚本
来源：http://xzq.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jmu.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://jnw.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://ooy.zhengqikj.top

[U84] JS：CommonJS 写法
来源：http://qjv.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sqr.uphjek.com

[U85] JS：可选链
来源：http://kpz.fktsv.cn

a?.b?.c
来源：http://qlg.fzhhl.top

[U86] JS：空值合并
来源：http://kfw.hywenlv.cn

a ?? b
来源：http://ydy.zhixingplan.top

[U87] JS：解构默认值
来源：http://lej.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://nes.uphjek.com

[U88] JS：对象展开合并
来源：http://tea.hywenlv.cn

{ ...a, ...b }
来源：http://nda.sufxvd.cn

[U89] JS：数组去重
来源：http://raf.svipenyu.cn

[...new Set(arr)]
来源：http://yxl.sysykeji.top

[U90] JS：数字数组排序
来源：http://cns.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://lxt.yj20258.top

[U91] JS：对象键值遍历
来源：http://ujn.cucudq.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hcf.ppjwa.cn

[U92] JS：深拷贝
来源：http://voo.fehbvm.com

structuredClone(obj)
来源：http://mtz.jqgfzy.top

[U93] JS：模板字符串
来源：http://eul.gzhubu.top

`共 ${n} 条`
来源：http://lwo.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://xgt.xuanzx.com

const double = x => x * 2;
来源：http://oac.sweek.top

[U95] JS：Promise 包装
来源：http://pho.pycfn.com

new Promise((resolve, reject) => {})
来源：http://vpc.shuidangran.top

[U96] JS：async/await 与异常
来源：http://iqb.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ocp.zdqjudy.top

[U97] JS：并发请求
来源：http://ech.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ylp.sjlbkw.cn

[U98] JS：fetch 带 JSON
来源：http://sjb.zhoulong.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wgs.dianchejie.cn

[U99] JS：事件监听
来源：http://jrk.aizwys.cn

el.addEventListener("click", e => {})
来源：http://atn.chenlongwang.top

[U100] JS：DOM 查询
来源：http://xqy.redwolf501.top

document.querySelector(".item")
来源：http://ife.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://vkv.havefunace.top

el.classList.toggle("active")
来源：http://wmx.sufxvd.cn

[U102] JS：本地存储
来源：http://jtj.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tuw.jianghu66.top

[U103] JS：定时器
来源：http://wbb.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wmk.svipenyu.cn

[U104] JS：防抖
来源：http://rik.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vlo.birdmap.top

[U105] JS：节流
来源：http://ihn.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ikd.wangdashe.top

[U106] JS：日期格式化
来源：http://dyu.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ets.kuanghao11.cn

[U107] JS：数字千分位
来源：http://baf.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wad.yvedp.cn

[U108] JS：随机整数
来源：http://kre.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xhu.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://bbb.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://bpw.wangdashe.top

[U110] JS：数组分块
来源：http://rpb.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://seb.hnxiangtu.top

[U111] JS：对象转 Map
来源：http://mef.gogol.net.cn

new Map(Object.entries(obj))
来源：http://wuz.xylfe.cn

[U112] JS：字符串补位
来源：http://poz.hammf.cn

"7".padStart(3, "0")
来源：http://ker.9152youxi.cn

[U113] JS：正则替换全部
来源：http://css.zycfv.cn

s.replaceAll("a", "b")
来源：http://wus.zhengqikj.top

[U114] JS：JSON 深比较
来源：http://gpp.cashguo.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://noe.hnqzz.top

[U115] JS：生成 UUID
来源：http://fmi.shanyushiyangtech.top

crypto.randomUUID()
来源：http://oxm.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://lwq.yuanzhike.top

/** @param {string} name */ function f(name) {}
来源：http://rte.ppjwa.cn

[U117] JS：单元测试
来源：http://lni.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://mew.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://zzy.cdnleiting.top

npm i -D vite;  npx vite
来源：http://jiu.uphjek.com

[U119] JS：生产构建
来源：http://idz.sysykeji.top

npx vite build
来源：http://amu.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://qfo.zdbjq.cn

import.meta.env.VITE_API_URL
来源：http://cme.yueranfly.top

================================================================================
来源：http://jcw.shzxlz.cn

统计汇总
来源：http://gtg.yuxming.cn

================================================================================
来源：http://axe.ydzc1.top

按语言统计（条）：
来源：http://pdt.chenjidiqi.icu

Python ......... 252
来源：http://cmx.gzhubu.top

PHP ............ 252
来源：http://hoy.hnqzz.top

JavaScript ..... 252
来源：http://ptj.svipenyu.cn

TypeScript ..... 212
来源：http://dec.svipenyu.cn

Java ........... 212
来源：http://pjj.chenjidiqi.icu

Go ............. 212
来源：http://qyj.jyoumei.cn

Ruby ........... 212
来源：http://skw.wangdashe.top

C# ............. 212
来源：http://wnq.ydzc1.top

C .............. 30
来源：http://wxm.hongshengwenyu.top

C++ ............ 30
来源：http://for.hammf.cn

SQL ............ 90
来源：http://oib.shzxlz.cn

Bash ........... 80
来源：http://pmg.hongshengwenyu.top

Kotlin ......... 15
来源：http://mtb.feifeiyinyue.top

Swift .......... 15
来源：http://edu.fengsongda.top

Lua ............ 10
来源：http://gbn.wangdashe.top

Perl ........... 10
来源：http://frq.shangyingyoupin.top

Scala .......... 10
来源：http://rzp.ydjk.org.cn

------------------------------------
来源：http://swr.smart0.xyz

合计 ........... 2106 条
来源：http://iyd.hysaishi.cn

按章节统计：
来源：http://ffd.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mmg.wangdashe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aqv.svipenyu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bpu.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kyn.fktsv.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dbr.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jjr.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bsn.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ooc.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ctw.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cag.wangshuangyany.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pxx.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oxp.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdb.jinyuanbaomall.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qti.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://utg.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jyg.sxryk.cn

Q SQL 专题                              90
来源：http://vnw.epnwcf.com

R Bash 专题                             80
来源：http://yvf.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://eih.yj202588.top

T 其他语言补充                          60
来源：http://tjd.hongshengwenyu.top

U 高频实用片段                         120
来源：http://tji.ehwqpu.com

------------------------------------
来源：http://rza.yangfankeji.com

合计                                  2106 条
来源：http://pmk.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://rbp.ctjpmb.com


<!-- 参考信息 -->