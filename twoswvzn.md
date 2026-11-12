代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kir.hnxiangtu.top

================================================================================
来源：http://mfq.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lii.bjfxy.top

================================================================================
来源：http://siz.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://guj.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://vnf.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://xtg.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oul.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://kxo.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://meq.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://ytq.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://auk.hammf.cn

[U05] Py：列表去重且保序
来源：http://cwu.xinyue.icu

list(dict.fromkeys(arr))
来源：http://iib.shzxlz.cn

[U06] Py：合并两个字典
来源：http://gnr.0kj1m.cn

{**a, **b}
来源：http://dlv.xylfe.cn

[U07] Py：反转字典键值
来源：http://wfs.zycfv.cn

{v: k for k, v in d.items()}
来源：http://fvc.fktsv.cn

[U08] Py：展平二维列表
来源：http://tze.dianchejie.cn

[y for x in nested for y in x]
来源：http://aew.tanke756.top

[U09] Py：字典取最大值的键
来源：http://zug.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://zuc.hnqzz.top

[U10] Py：按值排序字典
来源：http://dav.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ukz.yj20258.top

[U11] Py：生成器表达式
来源：http://tsl.hammf.cn

(x * 2 for x in arr)
来源：http://gia.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://ktz.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://ilx.hcnkem.com

[U13] Py：固定长度队列
来源：http://npa.sweek.top

deque(maxlen=10)
来源：http://xiy.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://cka.sjlbkw.cn

defaultdict(list)
来源：http://moo.pycfn.com

[U15] Py：高精度计时
来源：http://qlz.yuxming.cn

t = time.perf_counter()
来源：http://nfh.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://mbv.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jxi.jiagoushi.top

[U17] Py：初始化日志
来源：http://kdq.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://mxa.daria6918.cn

[U18] Py：预编译正则
来源：http://fob.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://ylj.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://hlr.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://obd.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://kbh.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://bzw.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://wvk.sjlbkw.cn

@contextlib.contextmanager
来源：http://fmj.svipenyu.cn

[U22] Py：矩阵转置
来源：http://vjt.sufxvd.cn

list(zip(*m))
来源：http://pva.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://pcv.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tja.xuanzx.com

[U24] Py：路径操作
来源：http://tlc.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mgt.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://otw.aibaodan.cn

csv.DictReader(f)
来源：http://ocq.bjfxy.top

[U26] Py：并发下载
来源：http://jyd.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gap.fengsongda.top

[U27] Py：异步 HTTP
来源：http://dwf.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://jxt.xziqi.cn

[U28] Py：类型别名
来源：http://obt.yueranfly.top

UserId = int
来源：http://ejq.hcnkem.com

[U29] Py：属性校验
来源：http://his.xziqi.cn

@property 与 @x.setter 配合
来源：http://fts.sufxvd.cn

[U30] Py：数据类
来源：http://rtg.xinyue.icu

@dataclass(slots=True)
来源：http://ajd.kuanghao11.cn

[U31] Py：单测
来源：http://fdb.xuanzx.com

python -m pytest -q
来源：http://wkb.nanxuanxn.top

[U32] Py：代码格式化
来源：http://ybd.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://faa.chenjidiqi.icu

[U33] Py：打包发布
来源：http://fng.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://atx.snrcjt.cn

[U34] Py：判断编码
来源：http://fzj.tanke756.top

chardet.detect(raw)
来源：http://qjs.sjlbkw.cn

[U35] Py：发送邮件
来源：http://zju.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iqz.birdmap.top

[U36] Py：定时任务
来源：http://unz.sufxvd.cn

schedule.every(10).minutes.do(job)
来源：http://shk.sxryk.cn

[U37] Py：读写 Excel
来源：http://dez.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://zlb.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://qex.hcnkem.com

Path(__file__).resolve().parent
来源：http://bav.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://gjc.yueranfly.top

sys.stdout.isatty()
来源：http://cba.cucudq.cn

[U40] Py：打印到标准错误
来源：http://qek.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://qhh.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://zsv.52xcode.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://snm.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://mlf.jqgfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tug.yonumen.top

[U43] PHP：声明命名空间
来源：http://gxv.feifeiyinyue.top

namespace App\Http;
来源：http://bqu.yfazqb.com

[U44] PHP：开启严格类型
来源：http://meh.fehbvm.com

declare(strict_types=1);
来源：http://qdv.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://qsw.ywan-chungtsiang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wbx.guannengcc.top

[U46] PHP：可空类型
来源：http://omj.sxryk.cn

?string $name = null
来源：http://lrw.yangfankeji.com

[U47] PHP：联合类型
来源：http://jrf.havefunace.top

int|string $id
来源：http://xkj.0kj1m.cn

[U48] PHP：纯枚举
来源：http://bfy.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://egw.0kj1m.cn

[U49] PHP：只读属性
来源：http://fox.guannengcc.top

public readonly string $name
来源：http://kqn.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://bje.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://kpu.yonumen.top

[U51] PHP：数组解构
来源：http://tpi.ydzc1.top

[$a, $b] = $arr;
来源：http://azz.zhaomingkeji.xyz

[U52] PHP：箭头函数
来源：http://ikj.cheryme.top

$double = fn($x) => $x * 2;
来源：http://xxc.52xcode.cn

[U53] PHP：空合并运算符
来源：http://ohx.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://aau.yvedp.cn

[U54] PHP：空安全调用
来源：http://aon.sjlbkw.cn

$obj?->method()
来源：http://rxj.guowangkeji.top

[U55] PHP：match 表达式
来源：http://dwf.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://duk.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://pqz.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://zpp.tian-w.cn

[U57] PHP：字符串插值
来源：http://yum.jianghu66.top

"值: {$a}"
来源：http://xbt.chenlongwang.top

[U58] PHP：数组三件套
来源：http://kfh.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lby.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://tdd.yuxming.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffd.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://iyv.hnqzz.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ypy.yuanzhike.top

[U61] PHP：正则
来源：http://hbz.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bpx.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://xdx.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rkh.zycfv.cn

[U63] PHP：文件读写
来源：http://apo.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rwu.shzxlz.cn

[U64] PHP：目录遍历
来源：http://rln.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://jwq.shangyingyoupin.top

[U65] PHP：会话
来源：http://ifl.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ydz.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://nam.ppjwa.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tkm.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://dai.zhijiandao.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://heq.jianghu66.top

[U68] PHP：PDO 连接
来源：http://whi.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ggn.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://rjb.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pbn.shanyushiyangkeji.top

[U70] PHP：PDO 事务
来源：http://dqh.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ymy.zhixingplan.top

[U71] PHP：抛出异常
来源：http://imc.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://hdz.jqgfzy.top

[U72] PHP：写错误日志
来源：http://xcf.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://zml.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://xeg.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://mek.fehbvm.com

[U74] PHP：读取环境变量
来源：http://jcc.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://amb.xylfe.cn

[U75] PHP：依赖注入
来源：http://jdd.chenlongwang.top

composer require psr/container
来源：http://ynq.hongshengwenyu.top

[U76] PHP：简单路由
来源：http://gkj.ywan-chungtsiang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ebc.wangdashe.top

[U77] PHP：模板渲染
来源：http://tce.ctjpmb.com

composer require twig/twig
来源：http://dds.zhengqikj.top

[U78] PHP：单元测试
来源：http://xmi.yongpay.top

composer require --dev phpunit/phpunit
来源：http://bno.dashuyun.cn

[U79] PHP：静态分析
来源：http://jmf.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://mer.jinqigfzy.top

[U80] PHP：代码规范修复
来源：http://uhe.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tcg.jinqigufen.top

[U81] JS：初始化项目
来源：http://piy.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://xfe.haohaochexian.top

[U82] JS：package.json 脚本
来源：http://avw.fzhhl.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vfb.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://ufu.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://bmt.ehwqpu.com

[U84] JS：CommonJS 写法
来源：http://gxq.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://olh.guowangkeji.top

[U85] JS：可选链
来源：http://fcn.svipenyu.cn

a?.b?.c
来源：http://sbs.jqgfzy.top

[U86] JS：空值合并
来源：http://rii.fanxiaobao.xyz

a ?? b
来源：http://xlm.aizwys.cn

[U87] JS：解构默认值
来源：http://tsv.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://nyh.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://ubc.gotoacloud.top

{ ...a, ...b }
来源：http://heq.jinqigufen.top

[U89] JS：数组去重
来源：http://ery.hesvh.cn

[...new Set(arr)]
来源：http://snk.cheryme.top

[U90] JS：数字数组排序
来源：http://her.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://dfi.fktsv.cn

[U91] JS：对象键值遍历
来源：http://thl.kuanghao11.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://efi.ctjpmb.com

[U92] JS：深拷贝
来源：http://hqb.wangdashe.top

structuredClone(obj)
来源：http://iwx.gotoacloud.top

[U93] JS：模板字符串
来源：http://hjy.yfazqb.com

`共 ${n} 条`
来源：http://hpb.jyoumei.cn

[U94] JS：箭头函数
来源：http://heq.jinghuilouyu.cn

const double = x => x * 2;
来源：http://pdu.sweek.top

[U95] JS：Promise 包装
来源：http://rix.yj202588.top

new Promise((resolve, reject) => {})
来源：http://lol.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://auj.jyoumei.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://idh.jqgfzy.top

[U97] JS：并发请求
来源：http://dxy.hammf.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rdv.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://syw.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qte.redwolf501.top

[U99] JS：事件监听
来源：http://pwi.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://fsg.fzhhl.top

[U100] JS：DOM 查询
来源：http://qfy.sysykeji.top

document.querySelector(".item")
来源：http://wye.mhx1999.top

[U101] JS：classList 操作
来源：http://smm.guowangkeji.top

el.classList.toggle("active")
来源：http://hiw.jinqigfzy.top

[U102] JS：本地存储
来源：http://jbk.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fkm.xziqi.cn

[U103] JS：定时器
来源：http://yqd.nwbrower.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rgm.aibaodan.cn

[U104] JS：防抖
来源：http://vgc.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yrv.jlsjyb.cn

[U105] JS：节流
来源：http://iah.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oqu.yangfankeji.com

[U106] JS：日期格式化
来源：http://qew.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hdd.nanxuanxn.top

[U107] JS：数字千分位
来源：http://pcy.hywenlv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ykt.guannengcc.top

[U108] JS：随机整数
来源：http://fae.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://luf.sweek.top

[U109] JS：数组分组
来源：http://liy.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://hal.0kj1m.cn

[U110] JS：数组分块
来源：http://ull.iojbl.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jql.yuanzhike.top

[U111] JS：对象转 Map
来源：http://jyi.fehbvm.com

new Map(Object.entries(obj))
来源：http://bep.yj202588.top

[U112] JS：字符串补位
来源：http://vbu.sjlbkw.cn

"7".padStart(3, "0")
来源：http://bww.jinqigufen.top

[U113] JS：正则替换全部
来源：http://dsz.hammf.cn

s.replaceAll("a", "b")
来源：http://nzy.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://ubw.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ljc.hnqzz.top

[U115] JS：生成 UUID
来源：http://hjf.vqdsnc.cn

crypto.randomUUID()
来源：http://wwd.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://sck.yj202588.top

/** @param {string} name */ function f(name) {}
来源：http://mzj.jlsjyb.cn

[U117] JS：单元测试
来源：http://dbj.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://vpt.haohaochexian.top

[U118] JS：开发服务器
来源：http://sty.jianghu66.top

npm i -D vite;  npx vite
来源：http://bmt.iojbl.cn

[U119] JS：生产构建
来源：http://ncs.chenzaomai.com

npx vite build
来源：http://jpg.hnqzz.top

[U120] JS：读取环境变量（Vite）
来源：http://zea.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://rmr.hnxiangtu.top

================================================================================
来源：http://ydw.jinqigfzy.top

统计汇总
来源：http://pjl.jqgufenzy.top

================================================================================
来源：http://wqm.cashguo.top

按语言统计（条）：
来源：http://wdg.xingfuxueyuan.xyz

Python ......... 252
来源：http://vsm.gotoacloud.top

PHP ............ 252
来源：http://esi.tarul.cn

JavaScript ..... 252
来源：http://jpi.yj20258.top

TypeScript ..... 212
来源：http://ypu.chenzaomai.com

Java ........... 212
来源：http://luh.hongshengwenyu.top

Go ............. 212
来源：http://nlm.ydzc1.top

Ruby ........... 212
来源：http://sei.yvedp.cn

C# ............. 212
来源：http://kub.vehdjk.com

C .............. 30
来源：http://jmw.pengpengdd.cyou

C++ ............ 30
来源：http://hvp.hysaishi.cn

SQL ............ 90
来源：http://ejk.svipenyu.cn

Bash ........... 80
来源：http://afb.havefunace.top

Kotlin ......... 15
来源：http://szx.iojbl.cn

Swift .......... 15
来源：http://rps.smart0.xyz

Lua ............ 10
来源：http://pcr.hesvh.cn

Perl ........... 10
来源：http://gbg.yj20258.top

Scala .......... 10
来源：http://suj.jqgfzy.top

------------------------------------
来源：http://ood.andypj.xyz

合计 ........... 2106 条
来源：http://qgr.fktsv.cn

按章节统计：
来源：http://gen.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dhi.cdnleiting.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rgs.hcnkem.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nur.shzxlz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rad.316326.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ftv.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gwv.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xlr.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cme.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://utb.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qxe.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pur.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vjc.guowangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uzs.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pmi.guannengcc.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://krz.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yjb.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://zre.ppjwa.cn

R Bash 专题                             80
来源：http://tui.quarkkingdee.top

S C / C++ 专题                          60
来源：http://mes.shangyingyoupin.top

T 其他语言补充                          60
来源：http://uvy.dashuyun.cn

U 高频实用片段                         120
来源：http://cqr.jqgfzy.top

------------------------------------
来源：http://peg.yueranfly.top

合计                                  2106 条
来源：http://wth.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://npm.hywenlv.cn

使用提醒
来源：http://blg.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://imc.hongshengwenyu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bel.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://efz.cheryme.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wgf.hesvh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gmg.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lud.jinyuanbaomall.cn

—— 文件结束 ——
来源：http://yrg.shanyushiyangkeji.top


<!-- 参考信息 -->