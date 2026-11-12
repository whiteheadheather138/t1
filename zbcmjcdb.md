代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://exb.ivvv.top

[T59] Scala：循环
来源：http://vfv.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://cbg.hesvh.cn

[T60] Scala：折叠
来源：http://tps.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://trp.jqgfzy.top

================================================================================
来源：http://jpb.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://swl.jinghuilouyu.cn

================================================================================
来源：http://nda.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://jmn.pengpengdd.cyou

python -m venv .venv && source .venv/bin/activate
来源：http://jdk.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://kji.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://amw.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://gdm.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://npl.yj202588.top

[U04] Py：变量调试打印
来源：http://ues.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sxu.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://fsd.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://adc.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://tfh.xuetiantiany.cn

{**a, **b}
来源：http://oyk.chenzaomai.com

[U07] Py：反转字典键值
来源：http://zsu.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://znu.xuanzx.com

[U08] Py：展平二维列表
来源：http://epp.fengsongda.top

[y for x in nested for y in x]
来源：http://smb.yj202588.top

[U09] Py：字典取最大值的键
来源：http://hgi.andypj.xyz

max(d, key=d.get)
来源：http://auw.jqgfzy.top

[U10] Py：按值排序字典
来源：http://qju.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdf.fktsv.cn

[U11] Py：生成器表达式
来源：http://vrb.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://wei.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://qsf.hammf.cn

Counter(arr).most_common(3)
来源：http://bak.fzhhl.top

[U13] Py：固定长度队列
来源：http://hgy.hammf.cn

deque(maxlen=10)
来源：http://oeq.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://wrr.ywan-chungtsiang.top

defaultdict(list)
来源：http://ofh.gzhubu.top

[U15] Py：高精度计时
来源：http://ssg.aibaodan.cn

t = time.perf_counter()
来源：http://ucw.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://ycj.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ndz.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://otm.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://qrr.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://sjj.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://rqs.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://btk.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zhq.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://wlr.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://gwj.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://tdr.zhiwuduotai.top

@contextlib.contextmanager
来源：http://soo.sxryk.cn

[U22] Py：矩阵转置
来源：http://pyo.pycfn.com

list(zip(*m))
来源：http://itu.hcnkem.com

[U23] Py：分块读取大文件
来源：http://ter.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://neq.yj20258888.top

[U24] Py：路径操作
来源：http://zoy.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wxn.fehbvm.com

[U25] Py：CSV 按字典读
来源：http://tfx.andypj.xyz

csv.DictReader(f)
来源：http://cli.jqgufenzy.top

[U26] Py：并发下载
来源：http://rji.ivvv.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hbl.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://lzn.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://raj.vehdjk.com

[U28] Py：类型别名
来源：http://hfj.zhoulong.xyz

UserId = int
来源：http://qyq.hcnkem.com

[U29] Py：属性校验
来源：http://qcf.redwolf501.top

@property 与 @x.setter 配合
来源：http://vvf.havefunace.top

[U30] Py：数据类
来源：http://ptc.yanxiufei.cn

@dataclass(slots=True)
来源：http://lbd.tian-w.cn

[U31] Py：单测
来源：http://azy.jlsjyb.cn

python -m pytest -q
来源：http://rag.shuidangran.top

[U32] Py：代码格式化
来源：http://uds.uphjek.com

ruff format . && ruff check --fix .
来源：http://jkq.zhongyouzk.top

[U33] Py：打包发布
来源：http://jtc.yonumen.top

python -m build  （依赖 pyproject.toml）
来源：http://ygb.xuetiantiany.cn

[U34] Py：判断编码
来源：http://bjb.ybcxt.top

chardet.detect(raw)
来源：http://pwl.yongpay.top

[U35] Py：发送邮件
来源：http://lnb.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jjp.nwbrower.top

[U36] Py：定时任务
来源：http://jur.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://rcd.sxryk.cn

[U37] Py：读写 Excel
来源：http://jiw.havefunace.top

pandas.read_excel / DataFrame.to_excel
来源：http://lfk.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://mmc.yj20258888.top

Path(__file__).resolve().parent
来源：http://snq.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://gzs.fengsongda.top

sys.stdout.isatty()
来源：http://xmv.hnqzz.top

[U40] Py：打印到标准错误
来源：http://ndi.yuanzhike.top

print("err", file=sys.stderr)
来源：http://yva.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://huv.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zdv.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://czd.aizwys.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qzb.shuidangran.top

[U43] PHP：声明命名空间
来源：http://ppe.fengsongda.top

namespace App\Http;
来源：http://jjk.fzhhl.top

[U44] PHP：开启严格类型
来源：http://aqw.aizwys.cn

declare(strict_types=1);
来源：http://arx.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://iaj.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://gdx.iojbl.cn

[U46] PHP：可空类型
来源：http://obo.ybcxt.top

?string $name = null
来源：http://xxb.zhijiandao.cn

[U47] PHP：联合类型
来源：http://uba.ybcxt.top

int|string $id
来源：http://mvl.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://kbi.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lsd.ywan-chungtsiang.top

[U49] PHP：只读属性
来源：http://rzj.ppjwa.cn

public readonly string $name
来源：http://rex.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://gqc.yj20258.top

public function __construct(private int $id) {}
来源：http://wnn.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://vdf.sufxvd.cn

[$a, $b] = $arr;
来源：http://ycx.dianchejie.cn

[U52] PHP：箭头函数
来源：http://ydk.smart0.xyz

$double = fn($x) => $x * 2;
来源：http://xik.sweek.top

[U53] PHP：空合并运算符
来源：http://rym.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://cdp.hesvh.cn

[U54] PHP：空安全调用
来源：http://imr.cqqwz.cn

$obj?->method()
来源：http://ftx.xuanzx.com

[U55] PHP：match 表达式
来源：http://teq.ybcxt.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xhg.cucudq.cn

[U56] PHP：命名参数
来源：http://lqn.yj20258888.top

f(a: 1, b: 2)
来源：http://qcd.yonumen.top

[U57] PHP：字符串插值
来源：http://cgz.jianghu66.top

"值: {$a}"
来源：http://yhg.birdmap.top

[U58] PHP：数组三件套
来源：http://sne.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rps.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://omx.316326.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lhe.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://jsn.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rfg.iojbl.cn

[U61] PHP：正则
来源：http://bjv.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xlz.yonumen.top

[U62] PHP：日期对象
来源：http://svj.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vts.cdnleiting.top

[U63] PHP：文件读写
来源：http://ryj.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jcj.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://lea.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://nfz.nanxinkj.top

[U65] PHP：会话
来源：http://gdu.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xwo.jyoumei.cn

[U66] PHP：设置 Cookie
来源：http://omn.haohaochexian.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://amz.xziqi.cn

[U67] PHP：处理文件上传
来源：http://lkz.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gme.sweek.top

[U68] PHP：PDO 连接
来源：http://kgj.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ouv.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://tmm.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aws.pengpengdd.cyou

[U70] PHP：PDO 事务
来源：http://nlq.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ygc.havefunace.top

[U71] PHP：抛出异常
来源：http://ytj.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://ftz.tian-w.cn

[U72] PHP：写错误日志
来源：http://zzh.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://qps.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://ukm.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://vcc.zhoulong.xyz

[U74] PHP：读取环境变量
来源：http://dri.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://zsg.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://xeb.yj20258888.top

composer require psr/container
来源：http://rpf.yj202588.top

[U76] PHP：简单路由
来源：http://mxd.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qmk.tianlin.xyz

[U77] PHP：模板渲染
来源：http://jvl.guowangkeji.top

composer require twig/twig
来源：http://bjo.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://wig.xziqi.cn

composer require --dev phpunit/phpunit
来源：http://iqw.sysykeji.top

[U79] PHP：静态分析
来源：http://wso.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://loy.c1oappe.top

[U80] PHP：代码规范修复
来源：http://tie.vqdsnc.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ytw.0kj1m.cn

[U81] JS：初始化项目
来源：http://xxq.zhixingplan.top

npm init -y;  npm i express
来源：http://gsx.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://yst.zhaomingkeji.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yhc.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://uht.pengpengdd.cyou

export const a = 1;  import { a } from "./m.js";
来源：http://nxv.guannengcc.top

[U84] JS：CommonJS 写法
来源：http://tjr.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://ica.cashguo.top

[U85] JS：可选链
来源：http://ffy.zhaomingkeji.xyz

a?.b?.c
来源：http://vzo.hywenlv.cn

[U86] JS：空值合并
来源：http://dbt.fanxiaobao.xyz

a ?? b
来源：http://hjy.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://kxv.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://quu.shuidangran.top

[U88] JS：对象展开合并
来源：http://zot.c1oappe.top

{ ...a, ...b }
来源：http://nuo.aizwys.cn

[U89] JS：数组去重
来源：http://lvf.zdbjq.cn

[...new Set(arr)]
来源：http://skb.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://awc.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://hcg.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://uql.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kpd.uphjek.com

[U92] JS：深拷贝
来源：http://cio.jiagoushi.top

structuredClone(obj)
来源：http://cmy.sysykeji.top

[U93] JS：模板字符串
来源：http://qdp.quarkkingdee.top

`共 ${n} 条`
来源：http://pdy.sxryk.cn

[U94] JS：箭头函数
来源：http://kku.dianchejie.cn

const double = x => x * 2;
来源：http://otx.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://ktq.yfazqb.com

new Promise((resolve, reject) => {})
来源：http://btl.daxiang520.top

[U96] JS：async/await 与异常
来源：http://ods.316326.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upe.shuidangran.top

[U97] JS：并发请求
来源：http://eth.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qxt.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://ppq.jinqigufen.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ril.xuanzx.com

[U99] JS：事件监听
来源：http://paq.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://dys.chenzaomai.com

[U100] JS：DOM 查询
来源：http://xrp.chenzaomai.com

document.querySelector(".item")
来源：http://jsc.jiagoushi.top

[U101] JS：classList 操作
来源：http://apw.fanxiaobao.xyz

el.classList.toggle("active")
来源：http://gqc.uphjek.com

[U102] JS：本地存储
来源：http://cly.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bpv.fktsv.cn

[U103] JS：定时器
来源：http://xep.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bvc.feifeiyinyue.top

[U104] JS：防抖
来源：http://ldt.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldw.bbcook.cn

[U105] JS：节流
来源：http://fjj.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nnj.hammf.cn

[U106] JS：日期格式化
来源：http://cto.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ibf.nanxuanxn.top

[U107] JS：数字千分位
来源：http://xci.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://drm.ydjk.org.cn

[U108] JS：随机整数
来源：http://jvv.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dwp.sjlbkw.cn

[U109] JS：数组分组
来源：http://tks.tanke756.top

Object.groupBy(arr, x => x.type)
来源：http://crt.cheryme.top

[U110] JS：数组分块
来源：http://vsh.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ufb.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://enp.yangfankeji.com

new Map(Object.entries(obj))
来源：http://uic.jqgfzy.top

[U112] JS：字符串补位
来源：http://xxt.dianchejie.cn

"7".padStart(3, "0")
来源：http://qky.bjfxy.top

[U113] JS：正则替换全部
来源：http://ndx.snrcjt.cn

s.replaceAll("a", "b")
来源：http://gcx.zhiwuduotai.top

[U114] JS：JSON 深比较
来源：http://dcn.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uov.ctjpmb.com

[U115] JS：生成 UUID
来源：http://nxq.pengpengdd.cyou

crypto.randomUUID()
来源：http://egx.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://gvz.xinyue.icu

/** @param {string} name */ function f(name) {}
来源：http://anw.jinqigufen.top

[U117] JS：单元测试
来源：http://wpo.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://yae.pycfn.com

[U118] JS：开发服务器
来源：http://opr.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://bwq.xuanzx.com

[U119] JS：生产构建
来源：http://sdn.zhongyouzk.top

npx vite build
来源：http://aft.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://gkk.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://gnx.shangyingyoupin.top

================================================================================
来源：http://nvg.andypj.xyz

统计汇总
来源：http://onx.wangdashe.top

================================================================================
来源：http://nyl.shuidangran.top

按语言统计（条）：
来源：http://one.tianlin.xyz

Python ......... 252
来源：http://pom.kuanghao11.cn

PHP ............ 252
来源：http://dbe.vehdjk.com

JavaScript ..... 252
来源：http://wdv.xziqi.cn

TypeScript ..... 212
来源：http://oda.sweek.top

Java ........... 212
来源：http://adm.zhaomingkeji.xyz

Go ............. 212
来源：http://gcm.ybcxt.top

Ruby ........... 212
来源：http://mbr.gzhubu.top

C# ............. 212
来源：http://thf.hfpthk.cn

C .............. 30
来源：http://ctv.yangfankeji.com

C++ ............ 30
来源：http://jym.jiagoushi.top

SQL ............ 90
来源：http://pmf.jqgfzy.top

Bash ........... 80
来源：http://gxu.ydzc1.top

Kotlin ......... 15
来源：http://lgm.zycfv.cn

Swift .......... 15
来源：http://hod.fktsv.cn

Lua ............ 10
来源：http://ubg.ehwqpu.com

Perl ........... 10
来源：http://lga.gaohongyu789.top

Scala .......... 10
来源：http://vbu.hesvh.cn

------------------------------------
来源：http://yyi.hfpthk.cn

合计 ........... 2106 条
来源：http://iig.jinyuanbaomall.cn

按章节统计：
来源：http://qcz.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://soj.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wje.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ypn.tanke756.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iqe.bbcook.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mqw.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://idw.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fns.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kdb.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ape.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rxi.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ljr.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://okm.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nsm.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tax.aibaodan.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qib.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jvl.nanxuanxn.top

Q SQL 专题                              90
来源：http://wsa.xingfuxueyuan.xyz

R Bash 专题                             80
来源：http://bav.jianghu66.top

S C / C++ 专题                          60
来源：http://ivr.hnxiangtu.top

T 其他语言补充                          60
来源：http://pkz.yj20258888.top

U 高频实用片段                         120
来源：http://hgk.gotoacloud.top

------------------------------------
来源：http://vpz.wangshuangyany.cn

合计                                  2106 条
来源：http://iei.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://edv.ctjpmb.com

使用提醒
来源：http://sum.52xcode.cn

--------------------------------------------------------------------------------
来源：http://rvw.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zpu.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gyf.gaohongyu789.top


<!-- 参考信息 -->