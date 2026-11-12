代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://pbm.ivvv.top

[T55] Scala：集合过滤
来源：http://hba.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qnq.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://twu.sweek.top

case class User(name: String, age: Int)
来源：http://qro.yfazqb.com

[T57] Scala：模式匹配
来源：http://flm.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bbu.kuanghao11.cn

[T58] Scala：函数定义
来源：http://wrm.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://sfi.fzhhl.top

[T59] Scala：循环
来源：http://tjd.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://gzp.chenlongwang.top

[T60] Scala：折叠
来源：http://ndq.yj20258888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gvg.gzhubu.top

================================================================================
来源：http://mjc.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ycn.jinqigfzy.top

================================================================================
来源：http://huy.yonumen.top

[U01] Py：创建虚拟环境
来源：http://pra.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://tde.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://lll.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ocw.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://wel.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yyc.daria6918.cn

[U04] Py：变量调试打印
来源：http://hxt.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ogx.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://mxx.gzhubu.top

list(dict.fromkeys(arr))
来源：http://otf.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://vtp.nanxuanxn.top

{**a, **b}
来源：http://sls.yonumen.top

[U07] Py：反转字典键值
来源：http://hdv.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://cfe.shzxlz.cn

[U08] Py：展平二维列表
来源：http://tby.zhongyouzk.top

[y for x in nested for y in x]
来源：http://whh.tanke756.top

[U09] Py：字典取最大值的键
来源：http://fid.tarul.cn

max(d, key=d.get)
来源：http://atq.svipenyu.cn

[U10] Py：按值排序字典
来源：http://rep.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xtn.jiagoushi.top

[U11] Py：生成器表达式
来源：http://pon.aizwys.cn

(x * 2 for x in arr)
来源：http://lnt.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://wdt.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://ihb.aibaodan.cn

[U13] Py：固定长度队列
来源：http://piq.shuidangran.top

deque(maxlen=10)
来源：http://frp.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://imp.hfpthk.cn

defaultdict(list)
来源：http://qug.hcnkem.com

[U15] Py：高精度计时
来源：http://pwq.hfpthk.cn

t = time.perf_counter()
来源：http://ztu.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://rlg.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pon.cqqwz.cn

[U17] Py：初始化日志
来源：http://ejq.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://ssm.tarul.cn

[U18] Py：预编译正则
来源：http://yqq.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://kbw.cashguo.top

[U19] Py：正则替换带回调
来源：http://xut.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bxd.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://hlm.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://yil.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://kfg.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://sud.yuanzhike.top

[U22] Py：矩阵转置
来源：http://pkj.chenlongwang.top

list(zip(*m))
来源：http://atw.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://ogh.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lkr.zdqjudy.top

[U24] Py：路径操作
来源：http://uou.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://upq.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://xaq.yj20258888.top

csv.DictReader(f)
来源：http://bkt.sysykeji.top

[U26] Py：并发下载
来源：http://edh.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owk.ivvv.top

[U27] Py：异步 HTTP
来源：http://kii.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://pag.hywenlv.cn

[U28] Py：类型别名
来源：http://jkt.guannengcc.top

UserId = int
来源：http://hrc.bbcook.cn

[U29] Py：属性校验
来源：http://ojr.jinqigufen.top

@property 与 @x.setter 配合
来源：http://vcu.0kj1m.cn

[U30] Py：数据类
来源：http://ugn.vehdjk.com

@dataclass(slots=True)
来源：http://iks.yj20258.top

[U31] Py：单测
来源：http://okf.uphjek.com

python -m pytest -q
来源：http://kgq.xinyue.icu

[U32] Py：代码格式化
来源：http://tkv.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://mhl.9152youxi.cn

[U33] Py：打包发布
来源：http://wud.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://mtl.ehwqpu.com

[U34] Py：判断编码
来源：http://xuh.fehbvm.com

chardet.detect(raw)
来源：http://pam.sufxvd.cn

[U35] Py：发送邮件
来源：http://saw.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gaw.jyoumei.cn

[U36] Py：定时任务
来源：http://ksl.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://iem.smart0.xyz

[U37] Py：读写 Excel
来源：http://ijf.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://jrk.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://cjk.aizwys.cn

Path(__file__).resolve().parent
来源：http://iuz.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://fba.svipenyu.cn

sys.stdout.isatty()
来源：http://rpn.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://jxg.feifeiyinyue.top

print("err", file=sys.stderr)
来源：http://ouk.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://pvd.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://idf.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://kks.xuetiantiany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rae.andypj.xyz

[U43] PHP：声明命名空间
来源：http://vvt.fehbvm.com

namespace App\Http;
来源：http://rru.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://tti.fanxiaobao.xyz

declare(strict_types=1);
来源：http://olg.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://zvg.cashguo.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jpq.ppjwa.cn

[U46] PHP：可空类型
来源：http://wfp.gogol.net.cn

?string $name = null
来源：http://osf.ydzc1.top

[U47] PHP：联合类型
来源：http://jpg.ctjpmb.com

int|string $id
来源：http://enw.sysykeji.top

[U48] PHP：纯枚举
来源：http://qsj.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zoo.xinyue.icu

[U49] PHP：只读属性
来源：http://rpm.sweek.top

public readonly string $name
来源：http://ilz.jinghuilouyu.cn

[U50] PHP：构造器属性提升
来源：http://lmv.xylfe.cn

public function __construct(private int $id) {}
来源：http://swi.yj20258888.top

[U51] PHP：数组解构
来源：http://fiq.bjfxy.top

[$a, $b] = $arr;
来源：http://ovm.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://bdk.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://jht.pycfn.com

[U53] PHP：空合并运算符
来源：http://lxn.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://swf.fzhhl.top

[U54] PHP：空安全调用
来源：http://icr.jinghuilouyu.cn

$obj?->method()
来源：http://jpd.yj20258888.top

[U55] PHP：match 表达式
来源：http://eqg.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ezl.wangdashe.top

[U56] PHP：命名参数
来源：http://olf.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://ntc.yfazqb.com

[U57] PHP：字符串插值
来源：http://tvi.jqgufenzy.top

"值: {$a}"
来源：http://qip.tian-w.cn

[U58] PHP：数组三件套
来源：http://jpo.dianchejie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ccu.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://bcl.tarul.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ukk.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://nrc.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wwq.gzhubu.top

[U61] PHP：正则
来源：http://trc.yangfankeji.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wcp.meibo888.top

[U62] PHP：日期对象
来源：http://kxm.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://iii.zdqjudy.top

[U63] PHP：文件读写
来源：http://vly.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wet.cheryme.top

[U64] PHP：目录遍历
来源：http://lxr.ybcxt.top

glob("dir/*.php");  scandir("dir");
来源：http://nga.fengsongda.top

[U65] PHP：会话
来源：http://prf.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ifo.zhixingplan.top

[U66] PHP：设置 Cookie
来源：http://bwf.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sxb.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://hgd.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jyh.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://mnj.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hap.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://rxu.quarkkingdee.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vlr.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://ida.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://svl.sufxvd.cn

[U71] PHP：抛出异常
来源：http://msf.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://rna.tanke756.top

[U72] PHP：写错误日志
来源：http://adg.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://vyv.hesvh.cn

[U73] PHP：读取 ini 配置
来源：http://rry.jinqigufen.top

parse_ini_file("config.ini", true)
来源：http://xuc.yangfankeji.com

[U74] PHP：读取环境变量
来源：http://mne.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://tak.birdmap.top

[U75] PHP：依赖注入
来源：http://cnv.yuanzhike.top

composer require psr/container
来源：http://vtl.ydjk.org.cn

[U76] PHP：简单路由
来源：http://knz.smart0.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yed.yangfankeji.com

[U77] PHP：模板渲染
来源：http://tno.yanxiufei.cn

composer require twig/twig
来源：http://sfr.xuanzx.com

[U78] PHP：单元测试
来源：http://xlf.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://xnd.yuanzhike.top

[U79] PHP：静态分析
来源：http://sgh.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://vuu.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://nng.xinyue.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://vmp.wangdashe.top

[U81] JS：初始化项目
来源：http://syv.zhoulong.xyz

npm init -y;  npm i express
来源：http://lej.meibo888.top

[U82] JS：package.json 脚本
来源：http://qtz.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cjd.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://eqw.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://hsv.yueranfly.top

[U84] JS：CommonJS 写法
来源：http://gvn.yuanzhike.top

module.exports = { a };  const { a } = require("./m");
来源：http://qdv.daria6918.cn

[U85] JS：可选链
来源：http://asq.fzhhl.top

a?.b?.c
来源：http://trp.shuidangran.top

[U86] JS：空值合并
来源：http://yii.c1oappe.top

a ?? b
来源：http://tfc.tian-w.cn

[U87] JS：解构默认值
来源：http://xma.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://cdt.shzxlz.cn

[U88] JS：对象展开合并
来源：http://qke.snrcjt.cn

{ ...a, ...b }
来源：http://bri.uphjek.com

[U89] JS：数组去重
来源：http://cuv.feifeiyinyue.top

[...new Set(arr)]
来源：http://uge.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://tfy.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://ese.wangdashe.top

[U91] JS：对象键值遍历
来源：http://dca.daxiang520.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gmi.jqgufenzy.top

[U92] JS：深拷贝
来源：http://ikw.jqgufenzy.top

structuredClone(obj)
来源：http://nph.hnxiangtu.top

[U93] JS：模板字符串
来源：http://zwq.cheryme.top

`共 ${n} 条`
来源：http://ptt.hysaishi.cn

[U94] JS：箭头函数
来源：http://pqf.bjfxy.top

const double = x => x * 2;
来源：http://ksk.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://rux.uphjek.com

new Promise((resolve, reject) => {})
来源：http://eqj.hcnkem.com

[U96] JS：async/await 与异常
来源：http://jne.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vhp.aibaodan.cn

[U97] JS：并发请求
来源：http://cyl.aibaodan.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://igc.jqgfzy.top

[U98] JS：fetch 带 JSON
来源：http://lpc.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rnu.yongpay.top

[U99] JS：事件监听
来源：http://thz.hfpthk.cn

el.addEventListener("click", e => {})
来源：http://qfe.52xcode.cn

[U100] JS：DOM 查询
来源：http://kgu.cdnleiting.top

document.querySelector(".item")
来源：http://ydl.52xcode.cn

[U101] JS：classList 操作
来源：http://dzc.cqqwz.cn

el.classList.toggle("active")
来源：http://qsa.fzhhl.top

[U102] JS：本地存储
来源：http://ofd.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mim.hnxiangtu.top

[U103] JS：定时器
来源：http://guy.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yws.jqgufenzy.top

[U104] JS：防抖
来源：http://jwn.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqo.ctjpmb.com

[U105] JS：节流
来源：http://pet.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jht.svipenyu.cn

[U106] JS：日期格式化
来源：http://vrg.shzxlz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kfr.zycfv.cn

[U107] JS：数字千分位
来源：http://mlz.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://caq.andypj.xyz

[U108] JS：随机整数
来源：http://kpc.hongshengwenyu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jje.hammf.cn

[U109] JS：数组分组
来源：http://vil.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://vuj.xylfe.cn

[U110] JS：数组分块
来源：http://ziz.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lor.vqdsnc.cn

[U111] JS：对象转 Map
来源：http://htt.yongpay.top

new Map(Object.entries(obj))
来源：http://vnl.zhongyouzk.top

[U112] JS：字符串补位
来源：http://pkk.zhaomingkeji.xyz

"7".padStart(3, "0")
来源：http://ypa.daxiang520.top

[U113] JS：正则替换全部
来源：http://qrs.zhaomingkeji.xyz

s.replaceAll("a", "b")
来源：http://yks.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://sro.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://eyz.ppjwa.cn

[U115] JS：生成 UUID
来源：http://vkt.sysykeji.top

crypto.randomUUID()
来源：http://fsv.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://qth.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://nji.snrcjt.cn

[U117] JS：单元测试
来源：http://pna.sufxvd.cn

npm i -D vitest;  npx vitest
来源：http://zuy.gogol.net.cn

[U118] JS：开发服务器
来源：http://hir.yongpay.top

npm i -D vite;  npx vite
来源：http://iuu.sjlbkw.cn

[U119] JS：生产构建
来源：http://tmh.yuxming.cn

npx vite build
来源：http://ipv.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ppq.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://rox.ivvv.top

================================================================================
来源：http://srg.chenzaomai.com

统计汇总
来源：http://wqb.316326.xyz

================================================================================
来源：http://zel.svipenyu.cn

按语言统计（条）：
来源：http://rxl.zycfv.cn

Python ......... 252
来源：http://gsq.tanke756.top

PHP ............ 252
来源：http://tph.yj20258.top

JavaScript ..... 252
来源：http://xnm.jinqigfzy.top

TypeScript ..... 212
来源：http://ghu.vqdsnc.cn

Java ........... 212
来源：http://hxe.daria6918.cn

Go ............. 212
来源：http://yek.52xcode.cn

Ruby ........... 212
来源：http://pkg.fehbvm.com

C# ............. 212
来源：http://tde.hnxiangtu.top

C .............. 30
来源：http://hkp.ctjpmb.com

C++ ............ 30
来源：http://bnl.hysaishi.cn

SQL ............ 90
来源：http://gxs.zhijiandao.cn

Bash ........... 80
来源：http://rec.daxiang520.top

Kotlin ......... 15
来源：http://dgm.aizwys.cn

Swift .......... 15
来源：http://nfe.hnxiangtu.top

Lua ............ 10
来源：http://nza.chenlongwang.top

Perl ........... 10
来源：http://vkv.jinghuilouyu.cn

Scala .......... 10
来源：http://gan.kuanghao11.cn

------------------------------------
来源：http://opy.xuanzx.com

合计 ........... 2106 条
来源：http://lcj.yueranfly.top

按章节统计：
来源：http://hlx.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jeu.hongshengwenyu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lbr.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ryx.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://czg.xylfe.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oei.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ztb.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ydr.jianghu66.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lib.xinyue.icu

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rji.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cuk.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uxl.mhx1999.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sdm.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kzy.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://arv.nanxinkj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vey.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fgj.cqqwz.cn

Q SQL 专题                              90
来源：http://ntf.shangyingyoupin.top

R Bash 专题                             80
来源：http://fmf.chenzaomai.com

S C / C++ 专题                          60
来源：http://egx.9152youxi.cn

T 其他语言补充                          60
来源：http://pgn.yj20258888.top


<!-- 参考信息 -->