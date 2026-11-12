代发 wailian999

[U15] Py：高精度计时
来源：http://len.hcnkem.com

t = time.perf_counter()
来源：http://ock.redwolf501.top

[U16] Py：命令行参数解析
来源：http://ijc.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xug.yuanzhike.top

[U17] Py：初始化日志
来源：http://kqy.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://orh.wangdashe.top

[U18] Py：预编译正则
来源：http://ktt.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://qvu.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://npp.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tzb.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://idy.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://ynk.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://cvy.jinqigufen.top

@contextlib.contextmanager
来源：http://gpg.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://pge.hcnkem.com

list(zip(*m))
来源：http://oyh.dashuyun.cn

[U23] Py：分块读取大文件
来源：http://spw.ivvv.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djf.birdmap.top

[U24] Py：路径操作
来源：http://yzj.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://syi.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://swv.jyoumei.cn

csv.DictReader(f)
来源：http://wvu.hywenlv.cn

[U26] Py：并发下载
来源：http://iqv.zdqjudy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ieh.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://drr.haohaochexian.top

aiohttp.ClientSession() 配合 async with
来源：http://fzg.nanxinkj.top

[U28] Py：类型别名
来源：http://gdx.nanxinkj.top

UserId = int
来源：http://ici.vehdjk.com

[U29] Py：属性校验
来源：http://ynu.feifeiyinyue.top

@property 与 @x.setter 配合
来源：http://bot.chenjidiqi.icu

[U30] Py：数据类
来源：http://ifx.yj20258888.top

@dataclass(slots=True)
来源：http://too.fktsv.cn

[U31] Py：单测
来源：http://cxo.zhaomingkeji.xyz

python -m pytest -q
来源：http://knv.yj20258.top

[U32] Py：代码格式化
来源：http://kvb.yfazqb.com

ruff format . && ruff check --fix .
来源：http://sdg.nanxinkj.top

[U33] Py：打包发布
来源：http://goy.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://hnd.epnwcf.com

[U34] Py：判断编码
来源：http://nlj.tarul.cn

chardet.detect(raw)
来源：http://xgf.yj202588.top

[U35] Py：发送邮件
来源：http://hfv.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://luo.fengsongda.top

[U36] Py：定时任务
来源：http://nmz.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://hjs.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://eou.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://lth.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://wih.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://fer.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://eak.tarul.cn

sys.stdout.isatty()
来源：http://jvh.vehdjk.com

[U40] Py：打印到标准错误
来源：http://bpu.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://vrx.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://zay.dianchejie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sgv.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://tue.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eut.zycfv.cn

[U43] PHP：声明命名空间
来源：http://ifr.ppjwa.cn

namespace App\Http;
来源：http://emb.xziqi.cn

[U44] PHP：开启严格类型
来源：http://eqf.jinqigufen.top

declare(strict_types=1);
来源：http://asu.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://yqo.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://sfq.ctjpmb.com

[U46] PHP：可空类型
来源：http://nmz.cashguo.top

?string $name = null
来源：http://nzf.sxryk.cn

[U47] PHP：联合类型
来源：http://upm.zycfv.cn

int|string $id
来源：http://ous.daxiang520.top

[U48] PHP：纯枚举
来源：http://yzp.dashuyun.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bsy.yfazqb.com

[U49] PHP：只读属性
来源：http://mmn.zhixingplan.top

public readonly string $name
来源：http://oqp.yfazqb.com

[U50] PHP：构造器属性提升
来源：http://swo.svipenyu.cn

public function __construct(private int $id) {}
来源：http://dzn.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://sts.yonumen.top

[$a, $b] = $arr;
来源：http://dme.zhengqikj.top

[U52] PHP：箭头函数
来源：http://ung.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://kgc.daria6918.cn

[U53] PHP：空合并运算符
来源：http://zjx.chenlongwang.top

$v = $a ?? $b ?? "default";
来源：http://gzz.haohaochexian.top

[U54] PHP：空安全调用
来源：http://koo.jinqigfzy.top

$obj?->method()
来源：http://gvr.sweek.top

[U55] PHP：match 表达式
来源：http://azv.hfpthk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rnu.yfazqb.com

[U56] PHP：命名参数
来源：http://uig.hcnkem.com

f(a: 1, b: 2)
来源：http://nbc.snrcjt.cn

[U57] PHP：字符串插值
来源：http://aiu.meibo888.top

"值: {$a}"
来源：http://xok.316326.xyz

[U58] PHP：数组三件套
来源：http://qog.yonumen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://weg.fengsongda.top

[U59] PHP：自定义排序
来源：http://sqx.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zqj.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://gps.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ojt.chenzaomai.com

[U61] PHP：正则
来源：http://pca.zdqjudy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hyg.fzhhl.top

[U62] PHP：日期对象
来源：http://qfq.tanke756.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vsp.svipenyu.cn

[U63] PHP：文件读写
来源：http://avb.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ivu.shzxlz.cn

[U64] PHP：目录遍历
来源：http://pof.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://rll.smart0.xyz

[U65] PHP：会话
来源：http://lpz.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kjd.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://hty.redwolf501.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xco.52xcode.cn

[U67] PHP：处理文件上传
来源：http://fxm.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gmc.fzhhl.top

[U68] PHP：PDO 连接
来源：http://xmf.yfazqb.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gxi.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://fgf.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mbi.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://stf.ydjk.org.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ifj.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://nou.yangfankeji.com

throw new RuntimeException("失败", 500);
来源：http://sjx.jqgfzy.top

[U72] PHP：写错误日志
来源：http://yeb.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://uzi.chenjidiqi.icu

[U73] PHP：读取 ini 配置
来源：http://qfl.birdmap.top

parse_ini_file("config.ini", true)
来源：http://wnz.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://qff.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://xan.zdqjudy.top

[U75] PHP：依赖注入
来源：http://bhb.52xcode.cn

composer require psr/container
来源：http://xjn.pengpengdd.cyou

[U76] PHP：简单路由
来源：http://cqr.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ibw.quarkkingdee.top

[U77] PHP：模板渲染
来源：http://uei.hcnkem.com

composer require twig/twig
来源：http://ssu.tarul.cn

[U78] PHP：单元测试
来源：http://bfv.ivvv.top

composer require --dev phpunit/phpunit
来源：http://cgg.shanyushiyangkeji.top

[U79] PHP：静态分析
来源：http://yzt.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://yda.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://wcv.andypj.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ubw.nanxinkj.top

[U81] JS：初始化项目
来源：http://xbu.ydjk.org.cn

npm init -y;  npm i express
来源：http://tyv.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://fho.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zhn.cashguo.top

[U83] JS：ES Module 导入导出
来源：http://pgr.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xzz.ivvv.top

[U84] JS：CommonJS 写法
来源：http://xzh.shanyushiyangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://ksv.yj20258.top

[U85] JS：可选链
来源：http://csl.yueranfly.top

a?.b?.c
来源：http://oby.c1oappe.top

[U86] JS：空值合并
来源：http://iuq.xingfuxueyuan.xyz

a ?? b
来源：http://zsu.jinqigufen.top

[U87] JS：解构默认值
来源：http://rcc.hesvh.cn

const { a = 1, b = 2 } = obj;
来源：http://tms.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://alp.fzhhl.top

{ ...a, ...b }
来源：http://iwm.gzhubu.top

[U89] JS：数组去重
来源：http://bzu.xylfe.cn

[...new Set(arr)]
来源：http://suw.shuidangran.top

[U90] JS：数字数组排序
来源：http://hor.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://qkn.daxiang520.top

[U91] JS：对象键值遍历
来源：http://erp.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gqn.haohaochexian.top

[U92] JS：深拷贝
来源：http://gtr.sysykeji.top

structuredClone(obj)
来源：http://ysg.wangdashe.top

[U93] JS：模板字符串
来源：http://mte.sufxvd.cn

`共 ${n} 条`
来源：http://bcg.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://dsj.xinyue.icu

const double = x => x * 2;
来源：http://epc.guowangkeji.top

[U95] JS：Promise 包装
来源：http://etq.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://ftm.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://inz.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rhp.wangdashe.top

[U97] JS：并发请求
来源：http://jqv.nwbrower.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://mqf.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://wch.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vty.fengsongda.top

[U99] JS：事件监听
来源：http://xlw.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://caf.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://rri.gaohongyu789.top

document.querySelector(".item")
来源：http://enk.zdqjudy.top

[U101] JS：classList 操作
来源：http://otu.jinghuilouyu.cn

el.classList.toggle("active")
来源：http://yeu.xziqi.cn

[U102] JS：本地存储
来源：http://acj.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://vqe.jqgufenzy.top

[U103] JS：定时器
来源：http://gbq.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vud.shuidangran.top

[U104] JS：防抖
来源：http://nbs.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://meg.pycfn.com

[U105] JS：节流
来源：http://klo.cashguo.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bph.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://qpc.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mao.hcnkem.com

[U107] JS：数字千分位
来源：http://jbm.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qgj.sweek.top

[U108] JS：随机整数
来源：http://npr.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://chi.shangyingyoupin.top

[U109] JS：数组分组
来源：http://ebs.yonumen.top

Object.groupBy(arr, x => x.type)
来源：http://emo.guannengcc.top

[U110] JS：数组分块
来源：http://acx.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://igs.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://bht.fengsongda.top

new Map(Object.entries(obj))
来源：http://wsu.zhaomingkeji.xyz

[U112] JS：字符串补位
来源：http://kgp.zhoulong.xyz

"7".padStart(3, "0")
来源：http://rye.zhengqikj.top

[U113] JS：正则替换全部
来源：http://jex.cucudq.cn

s.replaceAll("a", "b")
来源：http://oss.feifeiyinyue.top

[U114] JS：JSON 深比较
来源：http://dqe.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gpw.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://bvt.kuanghao11.cn

crypto.randomUUID()
来源：http://eqf.tian-w.cn

[U116] JS：类型检查（JSDoc）
来源：http://fzw.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://egy.hcnkem.com

[U117] JS：单元测试
来源：http://lnm.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://qfu.xuanzx.com

[U118] JS：开发服务器
来源：http://sfw.yuxming.cn

npm i -D vite;  npx vite
来源：http://pzv.zdqjudy.top

[U119] JS：生产构建
来源：http://wfs.epnwcf.com

npx vite build
来源：http://bif.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://gjk.jqgfzy.top

import.meta.env.VITE_API_URL
来源：http://bgj.vehdjk.com

================================================================================
来源：http://cxu.tianlin.xyz

统计汇总
来源：http://iru.epnwcf.com

================================================================================
来源：http://dci.smart0.xyz

按语言统计（条）：
来源：http://qke.shanyushiyangtech.top

Python ......... 252
来源：http://ovj.0kj1m.cn

PHP ............ 252
来源：http://zko.zhoulong.xyz

JavaScript ..... 252
来源：http://bvs.mhx1999.top

TypeScript ..... 212
来源：http://qez.fengsongda.top

Java ........... 212
来源：http://lle.yj20258888.top

Go ............. 212
来源：http://wgy.316326.xyz

Ruby ........... 212
来源：http://ber.zhiwuduotai.top

C# ............. 212
来源：http://tqh.9152youxi.cn

C .............. 30
来源：http://iyr.meibo888.top

C++ ............ 30
来源：http://xhs.wangdashe.top

SQL ............ 90
来源：http://rps.gotoacloud.top

Bash ........... 80
来源：http://tmj.nanxuanxn.top

Kotlin ......... 15
来源：http://pwx.cdnleiting.top

Swift .......... 15
来源：http://yzf.yj20258.top

Lua ............ 10
来源：http://jgo.cqqwz.cn

Perl ........... 10
来源：http://nxi.vqdsnc.cn

Scala .......... 10
来源：http://jgp.52xcode.cn

------------------------------------
来源：http://kji.shuidangran.top

合计 ........... 2106 条
来源：http://qpx.yuxming.cn

按章节统计：
来源：http://noc.pycfn.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gol.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ckd.yangfankeji.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tii.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ywd.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tgi.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ogt.jyoumei.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kxe.52xcode.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pil.birdmap.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nwe.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://htt.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ixj.xinyue.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jxy.0kj1m.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ttp.meibo888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zkf.gaohongyu789.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hwk.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xnt.cucudq.cn

Q SQL 专题                              90
来源：http://ttq.cucudq.cn

R Bash 专题                             80
来源：http://udm.cucudq.cn

S C / C++ 专题                          60
来源：http://kjg.hysaishi.cn

T 其他语言补充                          60
来源：http://rvt.xuetiantiany.cn

U 高频实用片段                         120
来源：http://bon.cqqwz.cn

------------------------------------
来源：http://fwn.hnqzz.top

合计                                  2106 条
来源：http://vsj.birdmap.top

--------------------------------------------------------------------------------
来源：http://pkp.hammf.cn

使用提醒
来源：http://wlf.yj202588.top

--------------------------------------------------------------------------------
来源：http://szm.birdmap.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xvv.cashguo.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bdk.uphjek.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fyo.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ysh.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qic.yuanzhike.top

—— 文件结束 ——
来源：http://lpe.jinyuanbaomall.cn

================================================================================
来源：http://fpb.jinyuanbaomall.cn

程序语言常见例子速查手册（2024 版）
来源：http://lkx.zhixingplan.top

Common Programming Examples Cheat Book
来源：http://cnk.hnxiangtu.top

================================================================================
来源：http://kql.jqgufenzy.top

【收录内容】
来源：http://iwc.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://cbh.nwbrower.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hmy.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://agm.yj202588.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xcb.xylfe.cn

【使用说明】
来源：http://zhp.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cfo.fanxiaobao.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gif.shanyushiyangkeji.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iog.sxryk.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ozo.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zhp.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jcu.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mlk.jyoumei.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://csj.svipenyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pzo.yj202588.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vsa.yuanzhike.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qls.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vgv.zdqjudy.top

【文件统计】
来源：http://vhs.yonumen.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lvj.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://pid.mhx1999.top

目  录
来源：http://dtm.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://aql.jqgfzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ycy.gogol.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bep.hnqzz.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rhw.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mxr.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nmi.cheryme.top


<!-- 参考信息 -->