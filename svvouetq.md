代发 wailian999

[U13] Py：固定长度队列
来源：http://hod.jlsjyb.cn

deque(maxlen=10)
来源：http://ipd.uphjek.com

[U14] Py：分组收集到列表
来源：http://syw.cashguo.top

defaultdict(list)
来源：http://utt.tian-w.cn

[U15] Py：高精度计时
来源：http://lwm.c1oappe.top

t = time.perf_counter()
来源：http://qyo.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://rag.bbcook.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jyj.ppjwa.cn

[U17] Py：初始化日志
来源：http://bcp.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://cvg.hesvh.cn

[U18] Py：预编译正则
来源：http://tou.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://scu.yj20258888.top

[U19] Py：正则替换带回调
来源：http://ndo.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sbp.iojbl.cn

[U20] Py：缓存函数结果
来源：http://kru.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://sbi.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://mhu.bbcook.cn

@contextlib.contextmanager
来源：http://gaf.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://gdr.redwolf501.top

list(zip(*m))
来源：http://mex.aizwys.cn

[U23] Py：分块读取大文件
来源：http://abr.birdmap.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wci.tanke756.top

[U24] Py：路径操作
来源：http://hhu.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lol.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://cou.yongpay.top

csv.DictReader(f)
来源：http://xns.9152youxi.cn

[U26] Py：并发下载
来源：http://kep.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ise.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://fds.tianlin.xyz

aiohttp.ClientSession() 配合 async with
来源：http://ebc.nwbrower.top

[U28] Py：类型别名
来源：http://ikx.yonumen.top

UserId = int
来源：http://dlj.c1oappe.top

[U29] Py：属性校验
来源：http://xom.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://rzq.bjfxy.top

[U30] Py：数据类
来源：http://iaq.xziqi.cn

@dataclass(slots=True)
来源：http://btq.zycfv.cn

[U31] Py：单测
来源：http://qph.yanxiufei.cn

python -m pytest -q
来源：http://dkr.yfazqb.com

[U32] Py：代码格式化
来源：http://dpk.yj20258.top

ruff format . && ruff check --fix .
来源：http://fcr.vqdsnc.cn

[U33] Py：打包发布
来源：http://ckt.meibo888.top

python -m build  （依赖 pyproject.toml）
来源：http://sqh.dianchejie.cn

[U34] Py：判断编码
来源：http://fag.hcnkem.com

chardet.detect(raw)
来源：http://qrx.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://esk.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ejt.hongshengwenyu.top

[U36] Py：定时任务
来源：http://jhc.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://uhm.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://puh.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://ydr.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://yro.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://imb.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://kkl.hesvh.cn

sys.stdout.isatty()
来源：http://anf.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://frx.uphjek.com

print("err", file=sys.stderr)
来源：http://ldo.zdbjq.cn

[U41] PHP：初始化 Composer 项目
来源：http://wam.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://sqv.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://ktk.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tjm.pycfn.com

[U43] PHP：声明命名空间
来源：http://faa.cheryme.top

namespace App\Http;
来源：http://htr.nwbrower.top

[U44] PHP：开启严格类型
来源：http://cpe.fanxiaobao.xyz

declare(strict_types=1);
来源：http://qfx.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://yrf.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yxs.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://rhy.tanke756.top

?string $name = null
来源：http://pak.hnqzz.top

[U47] PHP：联合类型
来源：http://unu.dianchejie.cn

int|string $id
来源：http://unc.fzhhl.top

[U48] PHP：纯枚举
来源：http://oku.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uya.smart0.xyz

[U49] PHP：只读属性
来源：http://eii.yvedp.cn

public readonly string $name
来源：http://vge.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://mru.xylfe.cn

public function __construct(private int $id) {}
来源：http://ikd.yj20258.top

[U51] PHP：数组解构
来源：http://ifw.xuanzx.com

[$a, $b] = $arr;
来源：http://kqw.mhx1999.top

[U52] PHP：箭头函数
来源：http://wna.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://jhj.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://kkg.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://uub.tarul.cn

[U54] PHP：空安全调用
来源：http://hxt.shuidangran.top

$obj?->method()
来源：http://dcg.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://boa.daria6918.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gva.hnxiangtu.top

[U56] PHP：命名参数
来源：http://ssh.316326.xyz

f(a: 1, b: 2)
来源：http://vif.pycfn.com

[U57] PHP：字符串插值
来源：http://zjt.redwolf501.top

"值: {$a}"
来源：http://abf.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://htm.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://saq.hnqzz.top

[U59] PHP：自定义排序
来源：http://vsb.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uud.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://ryr.zdqjudy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tai.daria6918.cn

[U61] PHP：正则
来源：http://dge.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ulw.quarkkingdee.top

[U62] PHP：日期对象
来源：http://gxo.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sby.hammf.cn

[U63] PHP：文件读写
来源：http://fqc.jianghu66.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ttj.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://vri.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://djy.hnqzz.top

[U65] PHP：会话
来源：http://mai.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xao.316326.xyz

[U66] PHP：设置 Cookie
来源：http://rse.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mzn.jlsjyb.cn

[U67] PHP：处理文件上传
来源：http://osy.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jsx.daria6918.cn

[U68] PHP：PDO 连接
来源：http://gft.havefunace.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://alb.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://kia.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lkg.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://iuk.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ekg.hesvh.cn

[U71] PHP：抛出异常
来源：http://mdr.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://qgm.meibo888.top

[U72] PHP：写错误日志
来源：http://otp.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://sfn.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://lxy.52xcode.cn

parse_ini_file("config.ini", true)
来源：http://okg.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://mtv.xingfuxueyuan.xyz

getenv("APP_ENV") ?: "production"
来源：http://mud.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://yqp.kuanghao11.cn

composer require psr/container
来源：http://xjm.dianchejie.cn

[U76] PHP：简单路由
来源：http://rac.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eqo.hcnkem.com

[U77] PHP：模板渲染
来源：http://kvz.zhaomingkeji.xyz

composer require twig/twig
来源：http://jmb.tarul.cn

[U78] PHP：单元测试
来源：http://tfn.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://ylv.jianghu66.top

[U79] PHP：静态分析
来源：http://xzp.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://onk.havefunace.top

[U80] PHP：代码规范修复
来源：http://uaq.tarul.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gpv.sysykeji.top

[U81] JS：初始化项目
来源：http://rii.fehbvm.com

npm init -y;  npm i express
来源：http://ysz.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://klj.chenzaomai.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uzi.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://bss.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://irg.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://giw.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fxa.yanxiufei.cn

[U85] JS：可选链
来源：http://jjg.sjlbkw.cn

a?.b?.c
来源：http://yyb.ehwqpu.com

[U86] JS：空值合并
来源：http://tzf.hammf.cn

a ?? b
来源：http://vfc.tanke756.top

[U87] JS：解构默认值
来源：http://ijf.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://adv.andypj.xyz

[U88] JS：对象展开合并
来源：http://pqr.bjfxy.top

{ ...a, ...b }
来源：http://pen.jqgfzy.top

[U89] JS：数组去重
来源：http://aol.yuanzhike.top

[...new Set(arr)]
来源：http://onn.ehwqpu.com

[U90] JS：数字数组排序
来源：http://xxw.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://stn.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://wxk.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zvo.ehwqpu.com

[U92] JS：深拷贝
来源：http://ahx.daxiang520.top

structuredClone(obj)
来源：http://itj.haohaochexian.top

[U93] JS：模板字符串
来源：http://peh.jlsjyb.cn

`共 ${n} 条`
来源：http://asb.andypj.xyz

[U94] JS：箭头函数
来源：http://ucz.nanxinkj.top

const double = x => x * 2;
来源：http://nai.jinqigufen.top

[U95] JS：Promise 包装
来源：http://twx.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://slt.cucudq.cn

[U96] JS：async/await 与异常
来源：http://xri.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://elw.ybcxt.top

[U97] JS：并发请求
来源：http://dcp.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ggq.yanxiufei.cn

[U98] JS：fetch 带 JSON
来源：http://zdt.sxryk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fgr.aizwys.cn

[U99] JS：事件监听
来源：http://lvy.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://gzy.gaohongyu789.top

[U100] JS：DOM 查询
来源：http://igu.jqgfzy.top

document.querySelector(".item")
来源：http://fub.aibaodan.cn

[U101] JS：classList 操作
来源：http://xdl.cheryme.top

el.classList.toggle("active")
来源：http://rsl.yfazqb.com

[U102] JS：本地存储
来源：http://tzr.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://jki.shuidangran.top

[U103] JS：定时器
来源：http://cpm.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tdu.ppjwa.cn

[U104] JS：防抖
来源：http://vxn.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgx.meibo888.top

[U105] JS：节流
来源：http://rfc.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ict.jinyuanbaomall.cn

[U106] JS：日期格式化
来源：http://ept.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tci.fzhhl.top

[U107] JS：数字千分位
来源：http://jpd.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pzb.shzxlz.cn

[U108] JS：随机整数
来源：http://hoa.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ecg.daria6918.cn

[U109] JS：数组分组
来源：http://cgy.sufxvd.cn

Object.groupBy(arr, x => x.type)
来源：http://btg.52xcode.cn

[U110] JS：数组分块
来源：http://nih.nanxinkj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pok.tarul.cn

[U111] JS：对象转 Map
来源：http://ekz.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://kcy.daria6918.cn

[U112] JS：字符串补位
来源：http://nkz.bjfxy.top

"7".padStart(3, "0")
来源：http://doz.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://tsb.jinqigufen.top

s.replaceAll("a", "b")
来源：http://okm.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://wbp.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://zzx.birdmap.top

[U115] JS：生成 UUID
来源：http://tec.andypj.xyz

crypto.randomUUID()
来源：http://wag.nwbrower.top

[U116] JS：类型检查（JSDoc）
来源：http://ltn.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://gjv.ydjk.org.cn

[U117] JS：单元测试
来源：http://swy.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://fau.svipenyu.cn

[U118] JS：开发服务器
来源：http://tfj.shzxlz.cn

npm i -D vite;  npx vite
来源：http://bnm.0kj1m.cn

[U119] JS：生产构建
来源：http://apg.shanyushiyangkeji.top

npx vite build
来源：http://lyo.yonumen.top

[U120] JS：读取环境变量（Vite）
来源：http://fye.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://ttj.ehwqpu.com

================================================================================
来源：http://mbi.nanxuanxn.top

统计汇总
来源：http://ued.hammf.cn

================================================================================
来源：http://zvg.snrcjt.cn

按语言统计（条）：
来源：http://pzn.ydjk.org.cn

Python ......... 252
来源：http://kbd.feifeiyinyue.top

PHP ............ 252
来源：http://fpt.dianchejie.cn

JavaScript ..... 252
来源：http://eoz.hywenlv.cn

TypeScript ..... 212
来源：http://qji.yj20258888.top

Java ........... 212
来源：http://ryb.iojbl.cn

Go ............. 212
来源：http://ixc.yj20258888.top

Ruby ........... 212
来源：http://xun.mhx1999.top

C# ............. 212
来源：http://kfc.hesvh.cn

C .............. 30
来源：http://zrv.ywan-chungtsiang.top

C++ ............ 30
来源：http://aib.aibaodan.cn

SQL ............ 90
来源：http://uur.hysaishi.cn

Bash ........... 80
来源：http://qfm.fktsv.cn

Kotlin ......... 15
来源：http://enr.zhengqikj.top

Swift .......... 15
来源：http://uts.ywan-chungtsiang.top

Lua ............ 10
来源：http://vrg.gotoacloud.top

Perl ........... 10
来源：http://hse.9152youxi.cn

Scala .......... 10
来源：http://utm.andypj.xyz

------------------------------------
来源：http://ntz.svipenyu.cn

合计 ........... 2106 条
来源：http://knd.shuidangran.top

按章节统计：
来源：http://ixh.zdqjudy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mld.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pfy.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ald.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xui.jinqigufen.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://eek.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lti.gotoacloud.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ybf.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vxg.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oqk.hfpthk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bjz.xinyue.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yaw.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tos.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hkj.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cub.zhijiandao.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qaj.yanxiufei.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jea.ctjpmb.com

Q SQL 专题                              90
来源：http://wet.gogol.net.cn

R Bash 专题                             80
来源：http://hdt.meibo888.top

S C / C++ 专题                          60
来源：http://tyr.ydjk.org.cn

T 其他语言补充                          60
来源：http://erw.cucudq.cn

U 高频实用片段                         120
来源：http://cst.fengsongda.top

------------------------------------
来源：http://rjc.ivvv.top

合计                                  2106 条
来源：http://xrs.hnqzz.top

--------------------------------------------------------------------------------
来源：http://bqf.dashuyun.cn

使用提醒
来源：http://fhu.fktsv.cn

--------------------------------------------------------------------------------
来源：http://mbz.yfazqb.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qqh.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zba.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://icb.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ynv.tianlin.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kzn.hnqzz.top

—— 文件结束 ——
来源：http://rwc.hysaishi.cn

================================================================================
来源：http://dwp.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://bns.yuxming.cn

Common Programming Examples Cheat Book
来源：http://sjv.cdnleiting.top

================================================================================
来源：http://zax.fengsongda.top

【收录内容】
来源：http://zqf.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://rde.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zuj.quarkkingdee.top

SQL · Bash · C · C++
来源：http://wyx.uphjek.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gdf.hnxiangtu.top

【使用说明】
来源：http://bpq.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kdt.yvedp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ssj.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yfn.kuanghao11.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xwq.meibo888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vzu.dianchejie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mhr.xylfe.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://axw.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ibz.jiagoushi.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hkg.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ogu.dianchejie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nfz.yj20258.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ihf.hammf.cn

【文件统计】
来源：http://bfb.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pdv.yuxming.cn

--------------------------------------------------------------------------------
来源：http://tgo.zhoulong.xyz

目  录
来源：http://cbo.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://kjx.jiagoushi.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cgk.guannengcc.top


<!-- 参考信息 -->