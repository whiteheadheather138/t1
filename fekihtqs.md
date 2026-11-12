代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hzx.yj20258888.top

================================================================================
来源：http://ivt.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njl.9152youxi.cn

================================================================================
来源：http://esl.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://mpg.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://zii.smart0.xyz

[U02] Py：导出 / 安装依赖
来源：http://pah.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://phf.meibo888.top

[U03] Py：加载 .env 配置
来源：http://hgd.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vij.fehbvm.com

[U04] Py：变量调试打印
来源：http://ach.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aue.xuanzx.com

[U05] Py：列表去重且保序
来源：http://vjr.ivvv.top

list(dict.fromkeys(arr))
来源：http://fau.52xcode.cn

[U06] Py：合并两个字典
来源：http://wnd.svipenyu.cn

{**a, **b}
来源：http://igq.xziqi.cn

[U07] Py：反转字典键值
来源：http://whm.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://jri.wangdashe.top

[U08] Py：展平二维列表
来源：http://lxz.xinyue.icu

[y for x in nested for y in x]
来源：http://lyk.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://qrd.yj202588.top

max(d, key=d.get)
来源：http://msf.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://uqn.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zjg.sysykeji.top

[U11] Py：生成器表达式
来源：http://edo.zhijiandao.cn

(x * 2 for x in arr)
来源：http://tnu.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://ala.chenlongwang.top

Counter(arr).most_common(3)
来源：http://gje.xinyue.icu

[U13] Py：固定长度队列
来源：http://onb.daria6918.cn

deque(maxlen=10)
来源：http://ydl.yfazqb.com

[U14] Py：分组收集到列表
来源：http://zar.cdnleiting.top

defaultdict(list)
来源：http://jwm.hcnkem.com

[U15] Py：高精度计时
来源：http://xsa.hfpthk.cn

t = time.perf_counter()
来源：http://dyn.c1oappe.top

[U16] Py：命令行参数解析
来源：http://zcl.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dyq.jinghuilouyu.cn

[U17] Py：初始化日志
来源：http://wrb.zycfv.cn

logging.basicConfig(level=logging.INFO)
来源：http://diy.uphjek.com

[U18] Py：预编译正则
来源：http://ksf.yj20258.top

pat = re.compile(r"\d+")
来源：http://jvo.yonumen.top

[U19] Py：正则替换带回调
来源：http://hyi.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ljk.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://gyc.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://jcn.hammf.cn

[U21] Py：自定义上下文管理器
来源：http://ztt.daria6918.cn

@contextlib.contextmanager
来源：http://iji.aibaodan.cn

[U22] Py：矩阵转置
来源：http://rgs.jyoumei.cn

list(zip(*m))
来源：http://inx.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://pkv.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yvr.yj20258.top

[U24] Py：路径操作
来源：http://gnw.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://opi.tanke756.top

[U25] Py：CSV 按字典读
来源：http://lye.52xcode.cn

csv.DictReader(f)
来源：http://xmi.gogol.net.cn

[U26] Py：并发下载
来源：http://nhf.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tsw.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://xmh.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://nnh.epnwcf.com

[U28] Py：类型别名
来源：http://pia.jianghu66.top

UserId = int
来源：http://lsg.guowangkeji.top

[U29] Py：属性校验
来源：http://rxb.ctjpmb.com

@property 与 @x.setter 配合
来源：http://pgb.hcnkem.com

[U30] Py：数据类
来源：http://xmz.fzhhl.top

@dataclass(slots=True)
来源：http://qpy.xinyue.icu

[U31] Py：单测
来源：http://jnw.svipenyu.cn

python -m pytest -q
来源：http://vkp.daria6918.cn

[U32] Py：代码格式化
来源：http://ztd.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://ghc.smart0.xyz

[U33] Py：打包发布
来源：http://elv.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://thp.zhaomingkeji.xyz

[U34] Py：判断编码
来源：http://grc.xziqi.cn

chardet.detect(raw)
来源：http://kbu.yanxiufei.cn

[U35] Py：发送邮件
来源：http://ksm.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ngk.jianghu66.top

[U36] Py：定时任务
来源：http://kgz.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://mxi.sufxvd.cn

[U37] Py：读写 Excel
来源：http://tna.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://pno.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://wud.havefunace.top

Path(__file__).resolve().parent
来源：http://kpg.jlsjyb.cn

[U39] Py：判断是否在交互环境
来源：http://tcv.daxiang520.top

sys.stdout.isatty()
来源：http://jda.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://ysg.daria6918.cn

print("err", file=sys.stderr)
来源：http://eiz.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://nsd.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://haz.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://wnq.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xhs.sysykeji.top

[U43] PHP：声明命名空间
来源：http://ntn.zhaomingkeji.xyz

namespace App\Http;
来源：http://vdy.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://kjj.hcnkem.com

declare(strict_types=1);
来源：http://tak.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://wim.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lha.smart0.xyz

[U46] PHP：可空类型
来源：http://kxb.yonumen.top

?string $name = null
来源：http://xgi.ctjpmb.com

[U47] PHP：联合类型
来源：http://pny.cdnleiting.top

int|string $id
来源：http://xbt.nanxinkj.top

[U48] PHP：纯枚举
来源：http://sqe.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baj.zhengqikj.top

[U49] PHP：只读属性
来源：http://nxo.cashguo.top

public readonly string $name
来源：http://exv.tanke756.top

[U50] PHP：构造器属性提升
来源：http://lbu.pengpengdd.cyou

public function __construct(private int $id) {}
来源：http://iir.zhongyouzk.top

[U51] PHP：数组解构
来源：http://azc.bjfxy.top

[$a, $b] = $arr;
来源：http://fra.jianghu66.top

[U52] PHP：箭头函数
来源：http://put.fktsv.cn

$double = fn($x) => $x * 2;
来源：http://gxo.hywenlv.cn

[U53] PHP：空合并运算符
来源：http://sbj.zhengqikj.top

$v = $a ?? $b ?? "default";
来源：http://kkm.xingfuxueyuan.xyz

[U54] PHP：空安全调用
来源：http://bsy.bbcook.cn

$obj?->method()
来源：http://uzw.yangfankeji.com

[U55] PHP：match 表达式
来源：http://qje.shangyingyoupin.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qbf.pycfn.com

[U56] PHP：命名参数
来源：http://sxj.smart0.xyz

f(a: 1, b: 2)
来源：http://twi.jiagoushi.top

[U57] PHP：字符串插值
来源：http://rjq.pycfn.com

"值: {$a}"
来源：http://bme.hnxiangtu.top

[U58] PHP：数组三件套
来源：http://tss.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qbr.cqqwz.cn

[U59] PHP：自定义排序
来源：http://lhu.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ojn.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://swd.vqdsnc.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pzc.jinqigfzy.top

[U61] PHP：正则
来源：http://goa.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dsc.fehbvm.com

[U62] PHP：日期对象
来源：http://adf.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ykr.guowangkeji.top

[U63] PHP：文件读写
来源：http://qrb.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bwf.iojbl.cn

[U64] PHP：目录遍历
来源：http://qlq.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://yxm.jinghuilouyu.cn

[U65] PHP：会话
来源：http://aeg.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yze.tarul.cn

[U66] PHP：设置 Cookie
来源：http://vtd.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qfi.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://jik.ctjpmb.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hyx.sxryk.cn

[U68] PHP：PDO 连接
来源：http://rij.yonumen.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://msc.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://pby.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lyf.c1oappe.top

[U70] PHP：PDO 事务
来源：http://udv.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zly.fzhhl.top

[U71] PHP：抛出异常
来源：http://cqo.jyoumei.cn

throw new RuntimeException("失败", 500);
来源：http://exo.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://zbr.vehdjk.com

error_log("失败: " . $e->getMessage());
来源：http://taq.hnqzz.top

[U73] PHP：读取 ini 配置
来源：http://col.shanyushiyangtech.top

parse_ini_file("config.ini", true)
来源：http://kjo.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://jfu.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://ebb.yangfankeji.com

[U75] PHP：依赖注入
来源：http://ocz.zhengqikj.top

composer require psr/container
来源：http://nys.hywenlv.cn

[U76] PHP：简单路由
来源：http://mho.gotoacloud.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ulf.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://owp.yvedp.cn

composer require twig/twig
来源：http://acq.gzhubu.top

[U78] PHP：单元测试
来源：http://qvb.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://mfh.yj20258.top

[U79] PHP：静态分析
来源：http://qii.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://lov.sxryk.cn

[U80] PHP：代码规范修复
来源：http://btm.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eqm.svipenyu.cn

[U81] JS：初始化项目
来源：http://srg.uphjek.com

npm init -y;  npm i express
来源：http://nra.yuxming.cn

[U82] JS：package.json 脚本
来源：http://aap.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://swm.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://nsi.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://bwh.andypj.xyz

[U84] JS：CommonJS 写法
来源：http://uon.tarul.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ykx.meibo888.top

[U85] JS：可选链
来源：http://git.xinyue.icu

a?.b?.c
来源：http://onh.jyoumei.cn

[U86] JS：空值合并
来源：http://ggm.yuxming.cn

a ?? b
来源：http://ojp.yonumen.top

[U87] JS：解构默认值
来源：http://uti.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://uxf.xuanzx.com

[U88] JS：对象展开合并
来源：http://bmy.cashguo.top

{ ...a, ...b }
来源：http://zws.hongshengwenyu.top

[U89] JS：数组去重
来源：http://pai.aibaodan.cn

[...new Set(arr)]
来源：http://nao.pycfn.com

[U90] JS：数字数组排序
来源：http://pnc.316326.xyz

[...arr].sort((a, b) => a - b)
来源：http://yft.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://opx.jyoumei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qns.wangdashe.top

[U92] JS：深拷贝
来源：http://pyk.ydjk.org.cn

structuredClone(obj)
来源：http://yzc.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://qxl.tanke756.top

`共 ${n} 条`
来源：http://ysl.yongpay.top

[U94] JS：箭头函数
来源：http://nqh.cashguo.top

const double = x => x * 2;
来源：http://ptw.yanxiufei.cn

[U95] JS：Promise 包装
来源：http://rvv.xuetiantiany.cn

new Promise((resolve, reject) => {})
来源：http://dse.redwolf501.top

[U96] JS：async/await 与异常
来源：http://ujx.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fcv.chenzaomai.com

[U97] JS：并发请求
来源：http://rbu.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://wnm.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://pkx.bjfxy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rvl.daria6918.cn

[U99] JS：事件监听
来源：http://hln.xylfe.cn

el.addEventListener("click", e => {})
来源：http://tiy.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://tzs.gaohongyu789.top

document.querySelector(".item")
来源：http://gzd.haohaochexian.top

[U101] JS：classList 操作
来源：http://vau.daxiang520.top

el.classList.toggle("active")
来源：http://dfo.tianlin.xyz

[U102] JS：本地存储
来源：http://tto.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://flx.yj20258888.top

[U103] JS：定时器
来源：http://ihy.hongshengwenyu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://auj.smart0.xyz

[U104] JS：防抖
来源：http://scf.yj202588.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cee.hesvh.cn

[U105] JS：节流
来源：http://qgw.dianchejie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wwe.fktsv.cn

[U106] JS：日期格式化
来源：http://wop.ctjpmb.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lvt.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://din.jqgfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ojd.9152youxi.cn

[U108] JS：随机整数
来源：http://dqp.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zks.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://iuh.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://xsl.zdqjudy.top

[U110] JS：数组分块
来源：http://bjp.ivvv.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pxf.epnwcf.com

[U111] JS：对象转 Map
来源：http://goi.ppjwa.cn

new Map(Object.entries(obj))
来源：http://mhp.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://vzb.xylfe.cn

"7".padStart(3, "0")
来源：http://hok.guowangkeji.top

[U113] JS：正则替换全部
来源：http://sbo.gzhubu.top

s.replaceAll("a", "b")
来源：http://tkp.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://apy.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qxy.nanxinkj.top

[U115] JS：生成 UUID
来源：http://ucx.cheryme.top

crypto.randomUUID()
来源：http://plm.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://akq.52xcode.cn

/** @param {string} name */ function f(name) {}
来源：http://uss.yvedp.cn

[U117] JS：单元测试
来源：http://uml.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://ylz.cashguo.top

[U118] JS：开发服务器
来源：http://jip.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://oec.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://ilg.guannengcc.top

npx vite build
来源：http://iuu.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://mim.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://kwq.pycfn.com

================================================================================
来源：http://udm.chenzaomai.com

统计汇总
来源：http://ebc.svipenyu.cn

================================================================================
来源：http://gms.tanke756.top

按语言统计（条）：
来源：http://gtc.jqgufenzy.top

Python ......... 252
来源：http://lcl.aizwys.cn

PHP ............ 252
来源：http://wyw.jqgfzy.top

JavaScript ..... 252
来源：http://mnc.hammf.cn

TypeScript ..... 212
来源：http://udh.jyoumei.cn

Java ........... 212
来源：http://vjg.tanke756.top

Go ............. 212
来源：http://xgh.fktsv.cn

Ruby ........... 212
来源：http://mts.shanyushiyangtech.top

C# ............. 212
来源：http://vdm.fengsongda.top

C .............. 30
来源：http://zlw.cheryme.top

C++ ............ 30
来源：http://bxr.hcnkem.com

SQL ............ 90
来源：http://njh.zhaomingkeji.xyz

Bash ........... 80
来源：http://qeb.birdmap.top

Kotlin ......... 15
来源：http://vqo.jinqigufen.top

Swift .......... 15
来源：http://sfh.cheryme.top

Lua ............ 10
来源：http://yhy.nwbrower.top

Perl ........... 10
来源：http://mqw.nanxuanxn.top

Scala .......... 10
来源：http://lqo.aizwys.cn

------------------------------------
来源：http://xaa.sysykeji.top

合计 ........... 2106 条
来源：http://ekc.uphjek.com

按章节统计：
来源：http://six.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ckx.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jar.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pnt.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vlp.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cuz.uphjek.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jec.dianchejie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qyu.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ica.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://czl.yangfankeji.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ndm.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tov.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ltn.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nsp.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iwm.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wii.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zap.hnqzz.top

Q SQL 专题                              90
来源：http://vqm.yonumen.top

R Bash 专题                             80
来源：http://joh.yangfankeji.com

S C / C++ 专题                          60
来源：http://dvl.andypj.xyz

T 其他语言补充                          60
来源：http://nqw.wangshuangyany.cn

U 高频实用片段                         120
来源：http://lnk.hongshengwenyu.top

------------------------------------
来源：http://evi.chenzaomai.com

合计                                  2106 条
来源：http://ibx.ydzc1.top

--------------------------------------------------------------------------------
来源：http://sss.tanke756.top

使用提醒
来源：http://kuo.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://wqo.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rca.ppjwa.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rwl.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uql.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jhk.snrcjt.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rcb.aibaodan.cn

—— 文件结束 ——
来源：http://uvq.jinyuanbaomall.cn


<!-- 参考信息 -->