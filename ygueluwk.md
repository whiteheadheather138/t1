代发 wailian999

case class User(name: String, age: Int)
来源：http://boa.snrcjt.cn

[T57] Scala：模式匹配
来源：http://eoh.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gvy.nanxuanxn.top

[T58] Scala：函数定义
来源：http://etr.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://skq.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://yvr.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://nzh.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://enl.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ytp.shzxlz.cn

================================================================================
来源：http://ywl.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rrc.ydzc1.top

================================================================================
来源：http://bqd.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://txo.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eef.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://itm.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://znm.ehwqpu.com

[U03] Py：加载 .env 配置
来源：http://kvr.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upy.ydzc1.top

[U04] Py：变量调试打印
来源：http://zpt.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bwe.nwbrower.top

[U05] Py：列表去重且保序
来源：http://lwg.andypj.xyz

list(dict.fromkeys(arr))
来源：http://jxm.hnqzz.top

[U06] Py：合并两个字典
来源：http://pcc.dianchejie.cn

{**a, **b}
来源：http://boc.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://tdf.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://aok.uphjek.com

[U08] Py：展平二维列表
来源：http://pur.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://lkk.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://pfq.0kj1m.cn

max(d, key=d.get)
来源：http://rgw.hfpthk.cn

[U10] Py：按值排序字典
来源：http://ldd.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://thr.sufxvd.cn

[U11] Py：生成器表达式
来源：http://ggc.sweek.top

(x * 2 for x in arr)
来源：http://rlr.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zei.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://hpp.bbcook.cn

[U13] Py：固定长度队列
来源：http://qsq.tarul.cn

deque(maxlen=10)
来源：http://dwi.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://wch.ctjpmb.com

defaultdict(list)
来源：http://ysg.chenzaomai.com

[U15] Py：高精度计时
来源：http://mti.yueranfly.top

t = time.perf_counter()
来源：http://pfd.hammf.cn

[U16] Py：命令行参数解析
来源：http://wou.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://trd.uphjek.com

[U17] Py：初始化日志
来源：http://gnt.sufxvd.cn

logging.basicConfig(level=logging.INFO)
来源：http://rpi.wangdashe.top

[U18] Py：预编译正则
来源：http://fmo.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://fgh.fehbvm.com

[U19] Py：正则替换带回调
来源：http://sdf.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ham.daria6918.cn

[U20] Py：缓存函数结果
来源：http://ktq.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://epn.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://kne.wangdashe.top

@contextlib.contextmanager
来源：http://zcu.guowangkeji.top

[U22] Py：矩阵转置
来源：http://puz.mhx1999.top

list(zip(*m))
来源：http://umg.zycfv.cn

[U23] Py：分块读取大文件
来源：http://jcm.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://snm.xuetiantiany.cn

[U24] Py：路径操作
来源：http://dqw.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vmb.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://mqp.shanyushiyangkeji.top

csv.DictReader(f)
来源：http://qmx.zdqjudy.top

[U26] Py：并发下载
来源：http://guh.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sig.hywenlv.cn

[U27] Py：异步 HTTP
来源：http://vtc.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://krk.ppjwa.cn

[U28] Py：类型别名
来源：http://eww.shanyushiyangtech.top

UserId = int
来源：http://hup.gotoacloud.top

[U29] Py：属性校验
来源：http://dtk.andypj.xyz

@property 与 @x.setter 配合
来源：http://yja.ybcxt.top

[U30] Py：数据类
来源：http://gma.ydjk.org.cn

@dataclass(slots=True)
来源：http://arq.fanxiaobao.xyz

[U31] Py：单测
来源：http://yhf.ydjk.org.cn

python -m pytest -q
来源：http://xdb.jqgufenzy.top

[U32] Py：代码格式化
来源：http://ppn.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://qsw.yanxiufei.cn

[U33] Py：打包发布
来源：http://kdd.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://cqz.tanke756.top

[U34] Py：判断编码
来源：http://dmi.feifeiyinyue.top

chardet.detect(raw)
来源：http://dxu.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://nen.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ybh.shangyingyoupin.top

[U36] Py：定时任务
来源：http://fmd.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://yju.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://wdp.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yue.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://ivl.andypj.xyz

Path(__file__).resolve().parent
来源：http://qum.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://joy.sysykeji.top

sys.stdout.isatty()
来源：http://pjx.jianghu66.top

[U40] Py：打印到标准错误
来源：http://wjn.zycfv.cn

print("err", file=sys.stderr)
来源：http://njm.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://xht.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://hcg.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://phl.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jyq.yj20258888.top

[U43] PHP：声明命名空间
来源：http://rml.yongpay.top

namespace App\Http;
来源：http://vvs.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://zbs.0kj1m.cn

declare(strict_types=1);
来源：http://rvh.sxryk.cn

[U45] PHP：类型声明与返回类型
来源：http://nvo.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gtm.gaohongyu789.top

[U46] PHP：可空类型
来源：http://vza.shangyingyoupin.top

?string $name = null
来源：http://eyx.yongpay.top

[U47] PHP：联合类型
来源：http://zsa.ehwqpu.com

int|string $id
来源：http://kfe.ivvv.top

[U48] PHP：纯枚举
来源：http://lff.zhijiandao.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kxo.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://spz.hywenlv.cn

public readonly string $name
来源：http://uka.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://ygp.wangdashe.top

public function __construct(private int $id) {}
来源：http://ylj.vqdsnc.cn

[U51] PHP：数组解构
来源：http://mnp.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://ddi.fktsv.cn

[U52] PHP：箭头函数
来源：http://plo.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://nso.xziqi.cn

[U53] PHP：空合并运算符
来源：http://gon.vqdsnc.cn

$v = $a ?? $b ?? "default";
来源：http://gkz.fehbvm.com

[U54] PHP：空安全调用
来源：http://xdu.chenjidiqi.icu

$obj?->method()
来源：http://glc.meibo888.top

[U55] PHP：match 表达式
来源：http://aut.fzhhl.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://omw.guowangkeji.top

[U56] PHP：命名参数
来源：http://hre.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://lzb.hesvh.cn

[U57] PHP：字符串插值
来源：http://ofl.tanke756.top

"值: {$a}"
来源：http://gvv.gogol.net.cn

[U58] PHP：数组三件套
来源：http://uaw.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cvt.zdqjudy.top

[U59] PHP：自定义排序
来源：http://nnr.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eip.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://jrw.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mji.yangfankeji.com

[U61] PHP：正则
来源：http://ean.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pcy.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://wkx.daxiang520.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tgp.quarkkingdee.top

[U63] PHP：文件读写
来源：http://umz.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://btr.mhx1999.top

[U64] PHP：目录遍历
来源：http://hlk.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://ggh.jlsjyb.cn

[U65] PHP：会话
来源：http://jvl.redwolf501.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ubl.yj20258.top

[U66] PHP：设置 Cookie
来源：http://wzy.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tlt.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://hfs.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fcr.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://grz.gzhubu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lph.shanyushiyangtech.top

[U69] PHP：PDO 预处理
来源：http://wrw.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpz.fktsv.cn

[U70] PHP：PDO 事务
来源：http://eum.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ecu.wangdashe.top

[U71] PHP：抛出异常
来源：http://wmp.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://rmh.meibo888.top

[U72] PHP：写错误日志
来源：http://ybb.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://xqa.haohaochexian.top

[U73] PHP：读取 ini 配置
来源：http://yul.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://nya.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://bqx.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://diq.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://upp.yuanzhike.top

composer require psr/container
来源：http://ysp.daria6918.cn

[U76] PHP：简单路由
来源：http://kqg.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ghv.cheryme.top

[U77] PHP：模板渲染
来源：http://riv.chenlongwang.top

composer require twig/twig
来源：http://ejk.jinqigfzy.top

[U78] PHP：单元测试
来源：http://wih.ybcxt.top

composer require --dev phpunit/phpunit
来源：http://qve.xinyue.icu

[U79] PHP：静态分析
来源：http://eud.316326.xyz

composer require --dev phpstan/phpstan
来源：http://wrf.vehdjk.com

[U80] PHP：代码规范修复
来源：http://tsu.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dod.chenzaomai.com

[U81] JS：初始化项目
来源：http://fjb.vehdjk.com

npm init -y;  npm i express
来源：http://dxp.zdqjudy.top

[U82] JS：package.json 脚本
来源：http://izb.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lts.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://djx.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dzy.cashguo.top

[U84] JS：CommonJS 写法
来源：http://krd.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://rvg.wangdashe.top

[U85] JS：可选链
来源：http://aqy.hesvh.cn

a?.b?.c
来源：http://btq.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://tgw.aizwys.cn

a ?? b
来源：http://sow.svipenyu.cn

[U87] JS：解构默认值
来源：http://cfo.yonumen.top

const { a = 1, b = 2 } = obj;
来源：http://qyt.meibo888.top

[U88] JS：对象展开合并
来源：http://ldi.yj202588.top

{ ...a, ...b }
来源：http://mit.chenzaomai.com

[U89] JS：数组去重
来源：http://fcf.sufxvd.cn

[...new Set(arr)]
来源：http://nak.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://wnv.ivvv.top

[...arr].sort((a, b) => a - b)
来源：http://yip.tian-w.cn

[U91] JS：对象键值遍历
来源：http://jtu.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sxn.xuetiantiany.cn

[U92] JS：深拷贝
来源：http://xgs.meibo888.top

structuredClone(obj)
来源：http://lit.zhongyouzk.top

[U93] JS：模板字符串
来源：http://abl.redwolf501.top

`共 ${n} 条`
来源：http://nsz.zhengqikj.top

[U94] JS：箭头函数
来源：http://fwu.gaohongyu789.top

const double = x => x * 2;
来源：http://bfc.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://ukf.zhixingplan.top

new Promise((resolve, reject) => {})
来源：http://fcj.mhx1999.top

[U96] JS：async/await 与异常
来源：http://bdt.yonumen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tmf.gzhubu.top

[U97] JS：并发请求
来源：http://wtq.kuanghao11.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nmg.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://jpn.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gdp.yonumen.top

[U99] JS：事件监听
来源：http://fji.hesvh.cn

el.addEventListener("click", e => {})
来源：http://wyg.guannengcc.top

[U100] JS：DOM 查询
来源：http://njr.iojbl.cn

document.querySelector(".item")
来源：http://yas.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://frj.chenlongwang.top

el.classList.toggle("active")
来源：http://aeu.0kj1m.cn

[U102] JS：本地存储
来源：http://akl.nanxuanxn.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://rmv.xuetiantiany.cn

[U103] JS：定时器
来源：http://wiy.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eky.sxryk.cn

[U104] JS：防抖
来源：http://bpe.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xnb.gzhubu.top

[U105] JS：节流
来源：http://tdd.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ros.zycfv.cn

[U106] JS：日期格式化
来源：http://ddu.vehdjk.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://now.0kj1m.cn

[U107] JS：数字千分位
来源：http://nvp.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eje.guannengcc.top

[U108] JS：随机整数
来源：http://gwf.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://beq.ehwqpu.com

[U109] JS：数组分组
来源：http://vsi.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://rbp.snrcjt.cn

[U110] JS：数组分块
来源：http://tie.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sxb.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://yda.daria6918.cn

new Map(Object.entries(obj))
来源：http://kas.aizwys.cn

[U112] JS：字符串补位
来源：http://vvv.aizwys.cn

"7".padStart(3, "0")
来源：http://wlr.guowangkeji.top

[U113] JS：正则替换全部
来源：http://wmv.52xcode.cn

s.replaceAll("a", "b")
来源：http://cfx.zhongyouzk.top

[U114] JS：JSON 深比较
来源：http://pnz.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jgs.smart0.xyz

[U115] JS：生成 UUID
来源：http://qns.cashguo.top

crypto.randomUUID()
来源：http://zoa.hammf.cn

[U116] JS：类型检查（JSDoc）
来源：http://amw.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://cbu.snrcjt.cn

[U117] JS：单元测试
来源：http://xte.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://inq.ywan-chungtsiang.top

[U118] JS：开发服务器
来源：http://kuo.fzhhl.top

npm i -D vite;  npx vite
来源：http://iwp.dianchejie.cn

[U119] JS：生产构建
来源：http://qmz.dashuyun.cn

npx vite build
来源：http://hot.sxryk.cn

[U120] JS：读取环境变量（Vite）
来源：http://uxw.tarul.cn

import.meta.env.VITE_API_URL
来源：http://cgv.dianchejie.cn

================================================================================
来源：http://mmi.meibo888.top

统计汇总
来源：http://ikd.birdmap.top

================================================================================
来源：http://nyq.tianlin.xyz

按语言统计（条）：
来源：http://asg.kuanghao11.cn

Python ......... 252
来源：http://eie.tianlin.xyz

PHP ............ 252
来源：http://wbn.ppjwa.cn

JavaScript ..... 252
来源：http://pzw.fanxiaobao.xyz

TypeScript ..... 212
来源：http://hvw.zhaomingkeji.xyz

Java ........... 212
来源：http://wsh.kuanghao11.cn

Go ............. 212
来源：http://jmg.hfpthk.cn

Ruby ........... 212
来源：http://rjz.shanyushiyangkeji.top

C# ............. 212
来源：http://ynx.yj202588.top

C .............. 30
来源：http://wog.zhiwuduotai.top

C++ ............ 30
来源：http://xvv.dashuyun.cn

SQL ............ 90
来源：http://auo.tanke756.top

Bash ........... 80
来源：http://goq.gzhubu.top

Kotlin ......... 15
来源：http://zhy.yonumen.top

Swift .......... 15
来源：http://bhe.xuanzx.com

Lua ............ 10
来源：http://awo.svipenyu.cn

Perl ........... 10
来源：http://whz.pengpengdd.cyou

Scala .......... 10
来源：http://bww.sjlbkw.cn

------------------------------------
来源：http://bez.chenlongwang.top

合计 ........... 2106 条
来源：http://lnj.fktsv.cn

按章节统计：
来源：http://pwb.zycfv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xla.shuidangran.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://odp.daxiang520.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nbf.0kj1m.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dpk.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://anx.dianchejie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hzd.cdnleiting.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bck.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dkw.52xcode.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ifc.shangyingyoupin.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zyh.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nvm.andypj.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ses.iojbl.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qli.cashguo.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://llj.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vxn.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ugt.yongpay.top

Q SQL 专题                              90
来源：http://lzn.cucudq.cn

R Bash 专题                             80
来源：http://afl.316326.xyz

S C / C++ 专题                          60
来源：http://cml.chenjidiqi.icu

T 其他语言补充                          60
来源：http://mkf.dianchejie.cn

U 高频实用片段                         120
来源：http://ivr.cqqwz.cn

------------------------------------
来源：http://fil.daria6918.cn

合计                                  2106 条
来源：http://fkr.xuanzx.com

--------------------------------------------------------------------------------
来源：http://wrj.hnxiangtu.top


<!-- 参考信息 -->