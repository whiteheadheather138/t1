代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wpr.haohaochexian.top

================================================================================
来源：http://xwa.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uhq.sjlbkw.cn

================================================================================
来源：http://ijs.uphjek.com

[U01] Py：创建虚拟环境
来源：http://ach.chenzaomai.com

python -m venv .venv && source .venv/bin/activate
来源：http://trz.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://hdo.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qtu.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://piq.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hen.yueranfly.top

[U04] Py：变量调试打印
来源：http://qsf.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://szm.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://ncd.xylfe.cn

list(dict.fromkeys(arr))
来源：http://wwx.pycfn.com

[U06] Py：合并两个字典
来源：http://gyo.dashuyun.cn

{**a, **b}
来源：http://ode.quarkkingdee.top

[U07] Py：反转字典键值
来源：http://qsx.andypj.xyz

{v: k for k, v in d.items()}
来源：http://hys.havefunace.top

[U08] Py：展平二维列表
来源：http://cex.hywenlv.cn

[y for x in nested for y in x]
来源：http://fzn.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://rvm.iojbl.cn

max(d, key=d.get)
来源：http://xcf.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://xyo.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cpd.tarul.cn

[U11] Py：生成器表达式
来源：http://doc.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://bkt.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://sjf.hysaishi.cn

Counter(arr).most_common(3)
来源：http://jrz.yuxming.cn

[U13] Py：固定长度队列
来源：http://ewi.ctjpmb.com

deque(maxlen=10)
来源：http://frl.cheryme.top

[U14] Py：分组收集到列表
来源：http://etg.iojbl.cn

defaultdict(list)
来源：http://vwe.52xcode.cn

[U15] Py：高精度计时
来源：http://cml.jinqigufen.top

t = time.perf_counter()
来源：http://egr.fehbvm.com

[U16] Py：命令行参数解析
来源：http://rpi.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wbf.hammf.cn

[U17] Py：初始化日志
来源：http://dyx.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://jta.vqdsnc.cn

[U18] Py：预编译正则
来源：http://abp.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://uho.sxryk.cn

[U19] Py：正则替换带回调
来源：http://wza.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jyz.pengpengdd.cyou

[U20] Py：缓存函数结果
来源：http://gqr.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://jom.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://eii.jiagoushi.top

@contextlib.contextmanager
来源：http://abi.sxryk.cn

[U22] Py：矩阵转置
来源：http://pkv.yj202588.top

list(zip(*m))
来源：http://jba.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://vlp.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rtz.zhixingplan.top

[U24] Py：路径操作
来源：http://trm.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://drl.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://tbr.hcnkem.com

csv.DictReader(f)
来源：http://pmo.jiagoushi.top

[U26] Py：并发下载
来源：http://bdj.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lyx.guannengcc.top

[U27] Py：异步 HTTP
来源：http://fkb.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://lpm.aizwys.cn

[U28] Py：类型别名
来源：http://mek.chenjidiqi.icu

UserId = int
来源：http://bgw.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://kgn.epnwcf.com

@property 与 @x.setter 配合
来源：http://fnx.ydzc1.top

[U30] Py：数据类
来源：http://wyg.xylfe.cn

@dataclass(slots=True)
来源：http://myw.snrcjt.cn

[U31] Py：单测
来源：http://dtk.zhiwuduotai.top

python -m pytest -q
来源：http://ffh.guowangkeji.top

[U32] Py：代码格式化
来源：http://ljq.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://rhq.zdqjudy.top

[U33] Py：打包发布
来源：http://evh.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://mcn.dianchejie.cn

[U34] Py：判断编码
来源：http://otk.zdqjudy.top

chardet.detect(raw)
来源：http://fdx.hfpthk.cn

[U35] Py：发送邮件
来源：http://yjl.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://for.wangshuangyany.cn

[U36] Py：定时任务
来源：http://vdf.9152youxi.cn

schedule.every(10).minutes.do(job)
来源：http://bhe.yfazqb.com

[U37] Py：读写 Excel
来源：http://rzr.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://tdv.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://bsn.redwolf501.top

Path(__file__).resolve().parent
来源：http://emy.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://ecp.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://pui.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://jue.pycfn.com

print("err", file=sys.stderr)
来源：http://aih.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://ikf.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zus.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://vbb.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wym.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://dnt.havefunace.top

namespace App\Http;
来源：http://jgg.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://uxt.zhongyouzk.top

declare(strict_types=1);
来源：http://xdm.yvedp.cn

[U45] PHP：类型声明与返回类型
来源：http://ead.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iwr.guannengcc.top

[U46] PHP：可空类型
来源：http://tte.hnqzz.top

?string $name = null
来源：http://kuf.nanxuanxn.top

[U47] PHP：联合类型
来源：http://qmq.0kj1m.cn

int|string $id
来源：http://xta.chenlongwang.top

[U48] PHP：纯枚举
来源：http://hvd.nwbrower.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kik.yueranfly.top

[U49] PHP：只读属性
来源：http://rmy.316326.xyz

public readonly string $name
来源：http://yst.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://zpw.yonumen.top

public function __construct(private int $id) {}
来源：http://ome.jinqigfzy.top

[U51] PHP：数组解构
来源：http://kpo.yj20258888.top

[$a, $b] = $arr;
来源：http://tth.bbcook.cn

[U52] PHP：箭头函数
来源：http://iuo.vehdjk.com

$double = fn($x) => $x * 2;
来源：http://uih.hesvh.cn

[U53] PHP：空合并运算符
来源：http://fvq.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://eyy.fengsongda.top

[U54] PHP：空安全调用
来源：http://ved.smart0.xyz

$obj?->method()
来源：http://mhz.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://esv.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://teq.hcnkem.com

[U56] PHP：命名参数
来源：http://pfq.zdbjq.cn

f(a: 1, b: 2)
来源：http://qtw.birdmap.top

[U57] PHP：字符串插值
来源：http://nnk.vehdjk.com

"值: {$a}"
来源：http://bsv.epnwcf.com

[U58] PHP：数组三件套
来源：http://xqg.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gql.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://hbv.feifeiyinyue.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yov.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://mpn.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xaq.hcnkem.com

[U61] PHP：正则
来源：http://piz.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wft.jqgfzy.top

[U62] PHP：日期对象
来源：http://gwb.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qce.52xcode.cn

[U63] PHP：文件读写
来源：http://dfz.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cfp.fktsv.cn

[U64] PHP：目录遍历
来源：http://xen.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://jdb.zhijiandao.cn

[U65] PHP：会话
来源：http://qlf.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://krc.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://yuf.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://voe.redwolf501.top

[U67] PHP：处理文件上传
来源：http://pvx.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ylh.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://oxr.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gco.wangshuangyany.cn

[U69] PHP：PDO 预处理
来源：http://kia.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vbl.pycfn.com

[U70] PHP：PDO 事务
来源：http://paj.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yas.fzhhl.top

[U71] PHP：抛出异常
来源：http://gxc.sweek.top

throw new RuntimeException("失败", 500);
来源：http://rnk.fktsv.cn

[U72] PHP：写错误日志
来源：http://sld.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://jeb.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://lqc.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://ecx.yfazqb.com

[U74] PHP：读取环境变量
来源：http://anv.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://lrs.52xcode.cn

[U75] PHP：依赖注入
来源：http://caj.ywan-chungtsiang.top

composer require psr/container
来源：http://jbb.jinyuanbaomall.cn

[U76] PHP：简单路由
来源：http://lbu.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tnm.ivvv.top

[U77] PHP：模板渲染
来源：http://xlk.cashguo.top

composer require twig/twig
来源：http://aad.aibaodan.cn

[U78] PHP：单元测试
来源：http://bzg.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://hhj.redwolf501.top

[U79] PHP：静态分析
来源：http://ktj.yangfankeji.com

composer require --dev phpstan/phpstan
来源：http://etf.iojbl.cn

[U80] PHP：代码规范修复
来源：http://dsh.gotoacloud.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hsi.fzhhl.top

[U81] JS：初始化项目
来源：http://hey.bjfxy.top

npm init -y;  npm i express
来源：http://buu.xinyue.icu

[U82] JS：package.json 脚本
来源：http://bks.jinqigfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uod.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://pue.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iod.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://sui.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bkr.hcnkem.com

[U85] JS：可选链
来源：http://bfg.daxiang520.top

a?.b?.c
来源：http://kwm.yangfankeji.com

[U86] JS：空值合并
来源：http://ygp.jqgfzy.top

a ?? b
来源：http://axu.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://vjr.nwbrower.top

const { a = 1, b = 2 } = obj;
来源：http://ciw.fktsv.cn

[U88] JS：对象展开合并
来源：http://sav.ybcxt.top

{ ...a, ...b }
来源：http://uxd.nanxinkj.top

[U89] JS：数组去重
来源：http://ycn.yfazqb.com

[...new Set(arr)]
来源：http://swq.zhengqikj.top

[U90] JS：数字数组排序
来源：http://xva.yuanzhike.top

[...arr].sort((a, b) => a - b)
来源：http://wbk.yueranfly.top

[U91] JS：对象键值遍历
来源：http://xnk.quarkkingdee.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oxh.wangdashe.top

[U92] JS：深拷贝
来源：http://xgt.fengsongda.top

structuredClone(obj)
来源：http://vue.fengsongda.top

[U93] JS：模板字符串
来源：http://gad.guannengcc.top

`共 ${n} 条`
来源：http://akr.zhixingplan.top

[U94] JS：箭头函数
来源：http://mlp.jianghu66.top

const double = x => x * 2;
来源：http://dgm.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://sgr.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://ucu.yvedp.cn

[U96] JS：async/await 与异常
来源：http://bdr.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zym.xingfuxueyuan.xyz

[U97] JS：并发请求
来源：http://lqd.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://zzd.jianghu66.top

[U98] JS：fetch 带 JSON
来源：http://psg.tian-w.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cbe.mhx1999.top

[U99] JS：事件监听
来源：http://ncf.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://gzl.yfazqb.com

[U100] JS：DOM 查询
来源：http://bwv.haohaochexian.top

document.querySelector(".item")
来源：http://olv.dashuyun.cn

[U101] JS：classList 操作
来源：http://mwc.zhijiandao.cn

el.classList.toggle("active")
来源：http://cxu.guannengcc.top

[U102] JS：本地存储
来源：http://fzd.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://qau.chenjidiqi.icu

[U103] JS：定时器
来源：http://cza.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kyy.9152youxi.cn

[U104] JS：防抖
来源：http://yyv.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnu.hfpthk.cn

[U105] JS：节流
来源：http://vjg.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hpu.aizwys.cn

[U106] JS：日期格式化
来源：http://dwk.zhijiandao.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qaa.hammf.cn

[U107] JS：数字千分位
来源：http://fxd.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://juu.guowangkeji.top

[U108] JS：随机整数
来源：http://hrj.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://win.cdnleiting.top

[U109] JS：数组分组
来源：http://lea.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://tad.fengsongda.top

[U110] JS：数组分块
来源：http://nwy.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jnq.vehdjk.com

[U111] JS：对象转 Map
来源：http://vlc.iojbl.cn

new Map(Object.entries(obj))
来源：http://khk.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://rbh.zhongyouzk.top

"7".padStart(3, "0")
来源：http://smh.fktsv.cn

[U113] JS：正则替换全部
来源：http://eoz.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://sgg.nanxinkj.top

[U114] JS：JSON 深比较
来源：http://tmj.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mkf.zdbjq.cn

[U115] JS：生成 UUID
来源：http://imk.uphjek.com

crypto.randomUUID()
来源：http://qqz.hcnkem.com

[U116] JS：类型检查（JSDoc）
来源：http://fca.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://spo.wangshuangyany.cn

[U117] JS：单元测试
来源：http://hnb.316326.xyz

npm i -D vitest;  npx vitest
来源：http://xqx.yuxming.cn

[U118] JS：开发服务器
来源：http://vrr.sysykeji.top

npm i -D vite;  npx vite
来源：http://nhz.sjlbkw.cn

[U119] JS：生产构建
来源：http://fmh.9152youxi.cn

npx vite build
来源：http://lhb.gogol.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://gpg.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://azk.hnqzz.top

================================================================================
来源：http://uor.fengsongda.top

统计汇总
来源：http://hxl.svipenyu.cn

================================================================================
来源：http://huf.0kj1m.cn

按语言统计（条）：
来源：http://rzp.fanxiaobao.xyz

Python ......... 252
来源：http://flc.ctjpmb.com

PHP ............ 252
来源：http://mhp.yuxming.cn

JavaScript ..... 252
来源：http://sop.jqgufenzy.top

TypeScript ..... 212
来源：http://ubg.zhaomingkeji.xyz

Java ........... 212
来源：http://yud.tianlin.xyz

Go ............. 212
来源：http://qhg.xziqi.cn

Ruby ........... 212
来源：http://fei.jinghuilouyu.cn

C# ............. 212
来源：http://czm.bjfxy.top

C .............. 30
来源：http://ued.jqgfzy.top

C++ ............ 30
来源：http://iuz.haohaochexian.top

SQL ............ 90
来源：http://uit.chenjidiqi.icu

Bash ........... 80
来源：http://pms.jlsjyb.cn

Kotlin ......... 15
来源：http://iud.zhixingplan.top

Swift .......... 15
来源：http://lim.yj20258.top

Lua ............ 10
来源：http://hcl.316326.xyz

Perl ........... 10
来源：http://xtz.daria6918.cn

Scala .......... 10
来源：http://hgn.hywenlv.cn

------------------------------------
来源：http://jbj.dashuyun.cn

合计 ........... 2106 条
来源：http://nis.ydjk.org.cn

按章节统计：
来源：http://okt.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jrl.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vud.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tzg.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qdt.ppjwa.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nir.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://skg.fzhhl.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uat.ywan-chungtsiang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aqh.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rmx.gotoacloud.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zrd.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gaa.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ihk.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ywt.pengpengdd.cyou

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dsk.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ynq.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://moy.xylfe.cn

Q SQL 专题                              90
来源：http://gvi.yuxming.cn

R Bash 专题                             80
来源：http://ycl.bjfxy.top

S C / C++ 专题                          60
来源：http://mhm.ydzc1.top

T 其他语言补充                          60
来源：http://qrp.jinqigufen.top

U 高频实用片段                         120
来源：http://tld.chenjidiqi.icu

------------------------------------
来源：http://iet.yj20258.top

合计                                  2106 条
来源：http://hws.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://nxd.jyoumei.cn

使用提醒
来源：http://xbu.pycfn.com

--------------------------------------------------------------------------------
来源：http://tej.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pja.hywenlv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mtk.gogol.net.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://avm.jyoumei.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ate.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ytd.pengpengdd.cyou

—— 文件结束 ——
来源：http://vhv.yj202588.top


<!-- 参考信息 -->