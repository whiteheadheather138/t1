代发 wailian999

[U17] Py：初始化日志
来源：http://iqo.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://dcd.nanxuanxn.top

[U18] Py：预编译正则
来源：http://abg.hcnkem.com

pat = re.compile(r"\d+")
来源：http://pzn.jianghu66.top

[U19] Py：正则替换带回调
来源：http://ofv.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://spk.pycfn.com

[U20] Py：缓存函数结果
来源：http://qih.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://ajw.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://lsl.yfazqb.com

@contextlib.contextmanager
来源：http://gwd.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://fqy.fehbvm.com

list(zip(*m))
来源：http://qdk.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://uuk.hfpthk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wnc.redwolf501.top

[U24] Py：路径操作
来源：http://epy.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sde.ivvv.top

[U25] Py：CSV 按字典读
来源：http://zno.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://arx.zdbjq.cn

[U26] Py：并发下载
来源：http://pzu.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xow.shuidangran.top

[U27] Py：异步 HTTP
来源：http://nof.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://jrg.ctjpmb.com

[U28] Py：类型别名
来源：http://mnb.zhoulong.xyz

UserId = int
来源：http://ekj.fanxiaobao.xyz

[U29] Py：属性校验
来源：http://wsu.shzxlz.cn

@property 与 @x.setter 配合
来源：http://vyb.fanxiaobao.xyz

[U30] Py：数据类
来源：http://cjn.sufxvd.cn

@dataclass(slots=True)
来源：http://nsi.pengpengdd.cyou

[U31] Py：单测
来源：http://tvo.haohaochexian.top

python -m pytest -q
来源：http://tsh.yj20258888.top

[U32] Py：代码格式化
来源：http://fmb.xziqi.cn

ruff format . && ruff check --fix .
来源：http://grr.ctjpmb.com

[U33] Py：打包发布
来源：http://pyp.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://mjq.jqgfzy.top

[U34] Py：判断编码
来源：http://lub.svipenyu.cn

chardet.detect(raw)
来源：http://xdy.vqdsnc.cn

[U35] Py：发送邮件
来源：http://pbq.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iei.pengpengdd.cyou

[U36] Py：定时任务
来源：http://krf.aizwys.cn

schedule.every(10).minutes.do(job)
来源：http://eog.iojbl.cn

[U37] Py：读写 Excel
来源：http://orv.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://cfr.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://pyf.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://ggz.yj20258888.top

[U39] Py：判断是否在交互环境
来源：http://jyh.gotoacloud.top

sys.stdout.isatty()
来源：http://pbm.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://pnr.xziqi.cn

print("err", file=sys.stderr)
来源：http://lgk.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://xth.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://siv.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://xgd.sweek.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wwj.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://leu.sxryk.cn

namespace App\Http;
来源：http://jit.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://imw.mhx1999.top

declare(strict_types=1);
来源：http://rdb.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://rze.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rcg.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://nfw.ppjwa.cn

?string $name = null
来源：http://ezg.hysaishi.cn

[U47] PHP：联合类型
来源：http://beq.pengpengdd.cyou

int|string $id
来源：http://uce.bbcook.cn

[U48] PHP：纯枚举
来源：http://tmq.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zjp.sweek.top

[U49] PHP：只读属性
来源：http://ipr.jinghuilouyu.cn

public readonly string $name
来源：http://jbt.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://bfg.gogol.net.cn

public function __construct(private int $id) {}
来源：http://iae.hysaishi.cn

[U51] PHP：数组解构
来源：http://wfk.gogol.net.cn

[$a, $b] = $arr;
来源：http://uay.ehwqpu.com

[U52] PHP：箭头函数
来源：http://uqy.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://byb.ybcxt.top

[U53] PHP：空合并运算符
来源：http://hos.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://wxt.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://lhb.yvedp.cn

$obj?->method()
来源：http://xaa.shuidangran.top

[U55] PHP：match 表达式
来源：http://cfx.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cfq.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://qwa.fehbvm.com

f(a: 1, b: 2)
来源：http://mvi.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://bdu.hywenlv.cn

"值: {$a}"
来源：http://hha.cucudq.cn

[U58] PHP：数组三件套
来源：http://ilg.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lba.tian-w.cn

[U59] PHP：自定义排序
来源：http://ajf.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tva.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://guk.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blq.shzxlz.cn

[U61] PHP：正则
来源：http://mtj.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jrb.cqqwz.cn

[U62] PHP：日期对象
来源：http://mkg.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lse.jinyuanbaomall.cn

[U63] PHP：文件读写
来源：http://pwt.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://htq.aizwys.cn

[U64] PHP：目录遍历
来源：http://kpo.yfazqb.com

glob("dir/*.php");  scandir("dir");
来源：http://mcg.guowangkeji.top

[U65] PHP：会话
来源：http://cvo.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://etd.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://tun.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xbn.smart0.xyz

[U67] PHP：处理文件上传
来源：http://odg.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iyx.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://fzf.xinyue.icu

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://niu.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://niw.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fqd.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://uln.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zse.cucudq.cn

[U71] PHP：抛出异常
来源：http://leq.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://nwv.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://lzf.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://jmu.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://cey.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://hva.andypj.xyz

[U74] PHP：读取环境变量
来源：http://lzk.yuxming.cn

getenv("APP_ENV") ?: "production"
来源：http://kww.fzhhl.top

[U75] PHP：依赖注入
来源：http://aap.yueranfly.top

composer require psr/container
来源：http://uwd.birdmap.top

[U76] PHP：简单路由
来源：http://dij.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://unx.jyoumei.cn

[U77] PHP：模板渲染
来源：http://dtb.yvedp.cn

composer require twig/twig
来源：http://byb.xziqi.cn

[U78] PHP：单元测试
来源：http://vyd.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://pkm.iojbl.cn

[U79] PHP：静态分析
来源：http://bjs.jinqigfzy.top

composer require --dev phpstan/phpstan
来源：http://lwm.yueranfly.top

[U80] PHP：代码规范修复
来源：http://vfw.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://djv.smart0.xyz

[U81] JS：初始化项目
来源：http://fhz.shangyingyoupin.top

npm init -y;  npm i express
来源：http://ypf.fktsv.cn

[U82] JS：package.json 脚本
来源：http://bot.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ufp.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://pam.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zcq.fktsv.cn

[U84] JS：CommonJS 写法
来源：http://kdu.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://mqd.daria6918.cn

[U85] JS：可选链
来源：http://vwl.hnxiangtu.top

a?.b?.c
来源：http://bme.tanke756.top

[U86] JS：空值合并
来源：http://nxa.cashguo.top

a ?? b
来源：http://jqv.uphjek.com

[U87] JS：解构默认值
来源：http://wzq.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://brx.nwbrower.top

[U88] JS：对象展开合并
来源：http://tfg.fengsongda.top

{ ...a, ...b }
来源：http://drw.yonumen.top

[U89] JS：数组去重
来源：http://kia.zhixingplan.top

[...new Set(arr)]
来源：http://twq.hfpthk.cn

[U90] JS：数字数组排序
来源：http://twu.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://eer.wangdashe.top

[U91] JS：对象键值遍历
来源：http://fen.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ghc.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://uil.ctjpmb.com

structuredClone(obj)
来源：http://oeh.daxiang520.top

[U93] JS：模板字符串
来源：http://qfy.jqgfzy.top

`共 ${n} 条`
来源：http://ulk.9152youxi.cn

[U94] JS：箭头函数
来源：http://xwu.jlsjyb.cn

const double = x => x * 2;
来源：http://qqm.c1oappe.top

[U95] JS：Promise 包装
来源：http://nnb.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://uct.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://uvk.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hne.dashuyun.cn

[U97] JS：并发请求
来源：http://fgz.hcnkem.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://sgr.hysaishi.cn

[U98] JS：fetch 带 JSON
来源：http://wla.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://szg.daxiang520.top

[U99] JS：事件监听
来源：http://mye.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://pqg.zhixingplan.top

[U100] JS：DOM 查询
来源：http://wds.sufxvd.cn

document.querySelector(".item")
来源：http://vsw.jinqigfzy.top

[U101] JS：classList 操作
来源：http://cvm.yongpay.top

el.classList.toggle("active")
来源：http://vmb.andypj.xyz

[U102] JS：本地存储
来源：http://ljq.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://twa.zhongyouzk.top

[U103] JS：定时器
来源：http://cgc.chenzaomai.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lov.hfpthk.cn

[U104] JS：防抖
来源：http://twq.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wws.hnxiangtu.top

[U105] JS：节流
来源：http://mrj.xingfuxueyuan.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nmq.hywenlv.cn

[U106] JS：日期格式化
来源：http://jww.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dnv.fengsongda.top

[U107] JS：数字千分位
来源：http://tqt.fzhhl.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zaj.yj20258.top

[U108] JS：随机整数
来源：http://kzk.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ftf.cashguo.top

[U109] JS：数组分组
来源：http://slu.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://spt.yj202588.top

[U110] JS：数组分块
来源：http://zom.hammf.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://efh.xuanzx.com

[U111] JS：对象转 Map
来源：http://mzl.yj20258.top

new Map(Object.entries(obj))
来源：http://iyp.hnxiangtu.top

[U112] JS：字符串补位
来源：http://fax.yongpay.top

"7".padStart(3, "0")
来源：http://ibx.aizwys.cn

[U113] JS：正则替换全部
来源：http://dlo.bbcook.cn

s.replaceAll("a", "b")
来源：http://zym.wangdashe.top

[U114] JS：JSON 深比较
来源：http://krf.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://sts.ybcxt.top

[U115] JS：生成 UUID
来源：http://yll.dashuyun.cn

crypto.randomUUID()
来源：http://gxk.quarkkingdee.top

[U116] JS：类型检查（JSDoc）
来源：http://hfy.shanyushiyangtech.top

/** @param {string} name */ function f(name) {}
来源：http://yik.shangyingyoupin.top

[U117] JS：单元测试
来源：http://cgq.yj20258.top

npm i -D vitest;  npx vitest
来源：http://nbr.yonumen.top

[U118] JS：开发服务器
来源：http://fak.yangfankeji.com

npm i -D vite;  npx vite
来源：http://mrz.hcnkem.com

[U119] JS：生产构建
来源：http://ggz.uphjek.com

npx vite build
来源：http://hjo.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://web.c1oappe.top

import.meta.env.VITE_API_URL
来源：http://bim.zhongyouzk.top

================================================================================
来源：http://yah.pengpengdd.cyou

统计汇总
来源：http://xyq.pycfn.com

================================================================================
来源：http://dip.pycfn.com

按语言统计（条）：
来源：http://lhc.jinqigufen.top

Python ......... 252
来源：http://kju.nanxuanxn.top

PHP ............ 252
来源：http://kau.uphjek.com

JavaScript ..... 252
来源：http://mlo.bjfxy.top

TypeScript ..... 212
来源：http://zkl.smart0.xyz

Java ........... 212
来源：http://gum.sweek.top

Go ............. 212
来源：http://aha.yangfankeji.com

Ruby ........... 212
来源：http://ony.shanyushiyangkeji.top

C# ............. 212
来源：http://dvx.jinqigfzy.top

C .............. 30
来源：http://ube.0kj1m.cn

C++ ............ 30
来源：http://mrc.cdnleiting.top

SQL ............ 90
来源：http://cqz.guowangkeji.top

Bash ........... 80
来源：http://mzg.ydzc1.top

Kotlin ......... 15
来源：http://cfm.svipenyu.cn

Swift .......... 15
来源：http://lst.wangshuangyany.cn

Lua ............ 10
来源：http://avx.chenzaomai.com

Perl ........... 10
来源：http://kwl.jqgfzy.top

Scala .......... 10
来源：http://ntp.shangyingyoupin.top

------------------------------------
来源：http://ocd.shanyushiyangtech.top

合计 ........... 2106 条
来源：http://rtd.sjlbkw.cn

按章节统计：
来源：http://piu.guowangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ift.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xml.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ctq.cheryme.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xge.sweek.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tne.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kpx.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bsq.cashguo.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ejk.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cpu.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zpq.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gfz.hnxiangtu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://peh.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nir.yongpay.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kqb.yuxming.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rns.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qei.52xcode.cn

Q SQL 专题                              90
来源：http://kyf.daxiang520.top

R Bash 专题                             80
来源：http://nih.hysaishi.cn

S C / C++ 专题                          60
来源：http://txo.9152youxi.cn

T 其他语言补充                          60
来源：http://dqr.bbcook.cn

U 高频实用片段                         120
来源：http://gfr.hnxiangtu.top

------------------------------------
来源：http://wha.yongpay.top

合计                                  2106 条
来源：http://kmx.yvedp.cn

--------------------------------------------------------------------------------
来源：http://jje.316326.xyz

使用提醒
来源：http://fth.andypj.xyz

--------------------------------------------------------------------------------
来源：http://jcg.hammf.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fkp.shangyingyoupin.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://atl.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lif.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://sng.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://omc.yanxiufei.cn

—— 文件结束 ——
来源：http://hiw.ehwqpu.com

================================================================================
来源：http://tpy.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://uxb.316326.xyz

Common Programming Examples Cheat Book
来源：http://jto.nwbrower.top

================================================================================
来源：http://jpt.hnqzz.top

【收录内容】
来源：http://jiv.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://urc.9152youxi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mdm.fehbvm.com

SQL · Bash · C · C++
来源：http://pvy.zhoulong.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ixe.haohaochexian.top

【使用说明】
来源：http://dsq.epnwcf.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qxx.yj20258.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wkp.birdmap.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rkf.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hau.c1oappe.top

Bash:  Shell         C:     C             C++:   C++
来源：http://iji.daria6918.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zss.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ouu.sufxvd.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wbk.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qor.dianchejie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uef.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yfg.ydjk.org.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://chx.zhoulong.xyz

【文件统计】
来源：http://kmx.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://aej.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://sls.bjfxy.top

目  录
来源：http://coj.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://azb.hammf.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xxy.hnxiangtu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xve.zycfv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qbt.c1oappe.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jgl.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hmm.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tdh.yvedp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rsd.nwbrower.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tie.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hrs.yonumen.top


<!-- 参考信息 -->