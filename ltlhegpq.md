代发 wailian999

[U17] Py：初始化日志
来源：http://iks.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://vqs.daria6918.cn

[U18] Py：预编译正则
来源：http://aus.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://moa.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://ejm.yuxming.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gha.daxiang520.top

[U20] Py：缓存函数结果
来源：http://iay.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://dlj.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://wow.jiagoushi.top

@contextlib.contextmanager
来源：http://nmc.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://swy.vqdsnc.cn

list(zip(*m))
来源：http://xaq.jianghu66.top

[U23] Py：分块读取大文件
来源：http://snh.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zdn.xuanzx.com

[U24] Py：路径操作
来源：http://vgp.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mbq.havefunace.top

[U25] Py：CSV 按字典读
来源：http://joc.shanyushiyangtech.top

csv.DictReader(f)
来源：http://emb.sweek.top

[U26] Py：并发下载
来源：http://omr.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uyn.andypj.xyz

[U27] Py：异步 HTTP
来源：http://uhn.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://fge.nwbrower.top

[U28] Py：类型别名
来源：http://dzd.ehwqpu.com

UserId = int
来源：http://fry.shzxlz.cn

[U29] Py：属性校验
来源：http://xhs.hysaishi.cn

@property 与 @x.setter 配合
来源：http://shv.yvedp.cn

[U30] Py：数据类
来源：http://xoa.cheryme.top

@dataclass(slots=True)
来源：http://zrm.tarul.cn

[U31] Py：单测
来源：http://vpj.fzhhl.top

python -m pytest -q
来源：http://amu.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://dqv.zhiwuduotai.top

ruff format . && ruff check --fix .
来源：http://zlz.hammf.cn

[U33] Py：打包发布
来源：http://ezw.fzhhl.top

python -m build  （依赖 pyproject.toml）
来源：http://syy.uphjek.com

[U34] Py：判断编码
来源：http://eip.hfpthk.cn

chardet.detect(raw)
来源：http://sez.bbcook.cn

[U35] Py：发送邮件
来源：http://afn.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hdq.nanxuanxn.top

[U36] Py：定时任务
来源：http://sgi.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://xsd.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://jat.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://agd.vqdsnc.cn

[U38] Py：获取脚本所在目录
来源：http://vpm.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://arr.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://sns.yj20258888.top

sys.stdout.isatty()
来源：http://dlx.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://vdu.quarkkingdee.top

print("err", file=sys.stderr)
来源：http://llx.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ibg.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://iez.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://cog.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xnv.vehdjk.com

[U43] PHP：声明命名空间
来源：http://evg.316326.xyz

namespace App\Http;
来源：http://suw.shuidangran.top

[U44] PHP：开启严格类型
来源：http://swt.tian-w.cn

declare(strict_types=1);
来源：http://edl.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://eug.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xkf.ydjk.org.cn

[U46] PHP：可空类型
来源：http://jiz.zdbjq.cn

?string $name = null
来源：http://qco.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://kvo.gotoacloud.top

int|string $id
来源：http://uqw.xziqi.cn

[U48] PHP：纯枚举
来源：http://wdu.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bxc.sysykeji.top

[U49] PHP：只读属性
来源：http://zsh.fengsongda.top

public readonly string $name
来源：http://zxe.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://ock.smart0.xyz

public function __construct(private int $id) {}
来源：http://omc.shanyushiyangtech.top

[U51] PHP：数组解构
来源：http://qtp.xylfe.cn

[$a, $b] = $arr;
来源：http://bpr.haohaochexian.top

[U52] PHP：箭头函数
来源：http://ddg.uphjek.com

$double = fn($x) => $x * 2;
来源：http://mwf.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://bdy.xuanzx.com

$v = $a ?? $b ?? "default";
来源：http://lks.tarul.cn

[U54] PHP：空安全调用
来源：http://gwo.zdbjq.cn

$obj?->method()
来源：http://hbm.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://vys.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://huk.yongpay.top

[U56] PHP：命名参数
来源：http://qpk.yj20258888.top

f(a: 1, b: 2)
来源：http://bnz.tarul.cn

[U57] PHP：字符串插值
来源：http://gfb.zdbjq.cn

"值: {$a}"
来源：http://vfe.ywan-chungtsiang.top

[U58] PHP：数组三件套
来源：http://cua.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nhk.iojbl.cn

[U59] PHP：自定义排序
来源：http://sox.yuanzhike.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://izq.birdmap.top

[U60] PHP：JSON 编解码
来源：http://law.jqgufenzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vqy.hywenlv.cn

[U61] PHP：正则
来源：http://hti.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rmm.ydjk.org.cn

[U62] PHP：日期对象
来源：http://trr.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dsl.ydjk.org.cn

[U63] PHP：文件读写
来源：http://vdl.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vnh.fanxiaobao.xyz

[U64] PHP：目录遍历
来源：http://pyt.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://sdy.yonumen.top

[U65] PHP：会话
来源：http://wzp.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rol.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://ctk.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vbz.andypj.xyz

[U67] PHP：处理文件上传
来源：http://ocs.xuetiantiany.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nnc.xylfe.cn

[U68] PHP：PDO 连接
来源：http://dqi.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iss.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://wvd.jqgufenzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://njj.zhoulong.xyz

[U70] PHP：PDO 事务
来源：http://miv.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mpb.zhixingplan.top

[U71] PHP：抛出异常
来源：http://aqe.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://due.yonumen.top

[U72] PHP：写错误日志
来源：http://jgh.xingfuxueyuan.xyz

error_log("失败: " . $e->getMessage());
来源：http://vet.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://gfn.uphjek.com

parse_ini_file("config.ini", true)
来源：http://usz.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://ncc.316326.xyz

getenv("APP_ENV") ?: "production"
来源：http://wez.bbcook.cn

[U75] PHP：依赖注入
来源：http://dyr.haohaochexian.top

composer require psr/container
来源：http://xyy.svipenyu.cn

[U76] PHP：简单路由
来源：http://lvs.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xly.xziqi.cn

[U77] PHP：模板渲染
来源：http://gbc.shuidangran.top

composer require twig/twig
来源：http://xgg.epnwcf.com

[U78] PHP：单元测试
来源：http://enj.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://qfa.9152youxi.cn

[U79] PHP：静态分析
来源：http://jhf.vehdjk.com

composer require --dev phpstan/phpstan
来源：http://ohq.havefunace.top

[U80] PHP：代码规范修复
来源：http://czu.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://eim.xinyue.icu

[U81] JS：初始化项目
来源：http://bbb.yuxming.cn

npm init -y;  npm i express
来源：http://xqh.uphjek.com

[U82] JS：package.json 脚本
来源：http://qat.hnqzz.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://njl.meibo888.top

[U83] JS：ES Module 导入导出
来源：http://rkp.cashguo.top

export const a = 1;  import { a } from "./m.js";
来源：http://lcq.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://inb.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://apx.zhiwuduotai.top

[U85] JS：可选链
来源：http://aye.jqgfzy.top

a?.b?.c
来源：http://xmu.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://gwz.ybcxt.top

a ?? b
来源：http://enz.ppjwa.cn

[U87] JS：解构默认值
来源：http://wvz.shanyushiyangtech.top

const { a = 1, b = 2 } = obj;
来源：http://wsn.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://nfp.52xcode.cn

{ ...a, ...b }
来源：http://usa.hnqzz.top

[U89] JS：数组去重
来源：http://unz.zhoulong.xyz

[...new Set(arr)]
来源：http://qxu.ivvv.top

[U90] JS：数字数组排序
来源：http://utq.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://ppe.316326.xyz

[U91] JS：对象键值遍历
来源：http://dcr.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uwk.jyoumei.cn

[U92] JS：深拷贝
来源：http://mwx.xylfe.cn

structuredClone(obj)
来源：http://qxg.ybcxt.top

[U93] JS：模板字符串
来源：http://oct.fzhhl.top

`共 ${n} 条`
来源：http://xuk.zdbjq.cn

[U94] JS：箭头函数
来源：http://tlh.shangyingyoupin.top

const double = x => x * 2;
来源：http://vxk.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://fpe.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://xbw.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://ans.uphjek.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rmo.shangyingyoupin.top

[U97] JS：并发请求
来源：http://amb.sweek.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kfc.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://ulv.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://het.zhiwuduotai.top

[U99] JS：事件监听
来源：http://xwn.yj20258.top

el.addEventListener("click", e => {})
来源：http://cdg.cheryme.top

[U100] JS：DOM 查询
来源：http://rmj.dianchejie.cn

document.querySelector(".item")
来源：http://uzx.zycfv.cn

[U101] JS：classList 操作
来源：http://miv.fzhhl.top

el.classList.toggle("active")
来源：http://qoo.tarul.cn

[U102] JS：本地存储
来源：http://ncb.yangfankeji.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://fsw.yongpay.top

[U103] JS：定时器
来源：http://qgp.jyoumei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ssj.havefunace.top

[U104] JS：防抖
来源：http://asm.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://myn.zycfv.cn

[U105] JS：节流
来源：http://uhr.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://reh.daxiang520.top

[U106] JS：日期格式化
来源：http://zae.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ayd.quarkkingdee.top

[U107] JS：数字千分位
来源：http://rbe.yj20258.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yry.ivvv.top

[U108] JS：随机整数
来源：http://sfl.hnqzz.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aqu.hammf.cn

[U109] JS：数组分组
来源：http://tqn.jqgfzy.top

Object.groupBy(arr, x => x.type)
来源：http://jhk.yuanzhike.top

[U110] JS：数组分块
来源：http://uez.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lqy.yj20258888.top

[U111] JS：对象转 Map
来源：http://rdu.hywenlv.cn

new Map(Object.entries(obj))
来源：http://yej.bbcook.cn

[U112] JS：字符串补位
来源：http://cnj.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://jnn.fehbvm.com

[U113] JS：正则替换全部
来源：http://uih.tanke756.top

s.replaceAll("a", "b")
来源：http://tax.0kj1m.cn

[U114] JS：JSON 深比较
来源：http://raf.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyd.snrcjt.cn

[U115] JS：生成 UUID
来源：http://iax.yonumen.top

crypto.randomUUID()
来源：http://odu.pycfn.com

[U116] JS：类型检查（JSDoc）
来源：http://thv.uphjek.com

/** @param {string} name */ function f(name) {}
来源：http://sfm.havefunace.top

[U117] JS：单元测试
来源：http://hjj.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://rap.yangfankeji.com

[U118] JS：开发服务器
来源：http://lgl.yfazqb.com

npm i -D vite;  npx vite
来源：http://bby.yj20258888.top

[U119] JS：生产构建
来源：http://sid.yj20258888.top

npx vite build
来源：http://jnc.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://wuo.chenlongwang.top

import.meta.env.VITE_API_URL
来源：http://lvx.yvedp.cn

================================================================================
来源：http://dbm.yj20258.top

统计汇总
来源：http://edx.xingfuxueyuan.xyz

================================================================================
来源：http://gts.pengpengdd.cyou

按语言统计（条）：
来源：http://den.yuanzhike.top

Python ......... 252
来源：http://ffv.daria6918.cn

PHP ............ 252
来源：http://orp.xziqi.cn

JavaScript ..... 252
来源：http://laj.zycfv.cn

TypeScript ..... 212
来源：http://dnc.epnwcf.com

Java ........... 212
来源：http://ahw.dianchejie.cn

Go ............. 212
来源：http://dcz.yfazqb.com

Ruby ........... 212
来源：http://nwi.pengpengdd.cyou

C# ............. 212
来源：http://kkn.shangyingyoupin.top

C .............. 30
来源：http://ecm.cqqwz.cn

C++ ............ 30
来源：http://ehf.birdmap.top

SQL ............ 90
来源：http://xkt.jyoumei.cn

Bash ........... 80
来源：http://hcc.jinghuilouyu.cn

Kotlin ......... 15
来源：http://mmx.aibaodan.cn

Swift .......... 15
来源：http://jxm.ydjk.org.cn

Lua ............ 10
来源：http://lfz.fehbvm.com

Perl ........... 10
来源：http://ebc.aibaodan.cn

Scala .......... 10
来源：http://ste.daria6918.cn

------------------------------------
来源：http://smh.yueranfly.top

合计 ........... 2106 条
来源：http://mop.aibaodan.cn

按章节统计：
来源：http://pfr.xingfuxueyuan.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yoh.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qqd.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uya.tarul.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hrr.fengsongda.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rib.xingfuxueyuan.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bbu.shuidangran.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gkg.jyoumei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qgr.nanxuanxn.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nkn.guowangkeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zaj.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eyd.fktsv.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://njs.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tew.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zux.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://szx.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vjo.fzhhl.top

Q SQL 专题                              90
来源：http://sst.sxryk.cn

R Bash 专题                             80
来源：http://tom.yonumen.top

S C / C++ 专题                          60
来源：http://rds.sufxvd.cn

T 其他语言补充                          60
来源：http://tdm.mhx1999.top

U 高频实用片段                         120
来源：http://vhx.guowangkeji.top

------------------------------------
来源：http://tfo.shanyushiyangkeji.top

合计                                  2106 条
来源：http://mhe.fengsongda.top

--------------------------------------------------------------------------------
来源：http://gys.yueranfly.top

使用提醒
来源：http://eid.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://oll.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wqg.52xcode.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gxh.havefunace.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://epb.shuidangran.top

在旧版本上使用前请先确认语法支持情况。
来源：http://slj.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nzj.fengsongda.top

—— 文件结束 ——
来源：http://ayb.feifeiyinyue.top

================================================================================
来源：http://gwh.vqdsnc.cn

程序语言常见例子速查手册（2024 版）
来源：http://pek.meibo888.top

Common Programming Examples Cheat Book
来源：http://dvz.fehbvm.com

================================================================================
来源：http://sbi.aizwys.cn

【收录内容】
来源：http://kpu.daxiang520.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xyv.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nme.kuanghao11.cn

SQL · Bash · C · C++
来源：http://rro.feifeiyinyue.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://smn.sjlbkw.cn

【使用说明】
来源：http://iyo.daxiang520.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ovh.smart0.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://tid.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wsb.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wpr.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://tzu.smart0.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yqy.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zpt.jinqigufen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qrr.chenlongwang.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hpn.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://jwv.meibo888.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://soh.quarkkingdee.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fqk.quarkkingdee.top

【文件统计】
来源：http://ttf.wangdashe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hnz.daxiang520.top

--------------------------------------------------------------------------------
来源：http://wka.yj20258888.top

目  录
来源：http://rbt.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://mkv.iojbl.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pux.nanxinkj.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dmi.birdmap.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kpp.xuetiantiany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fmf.cdnleiting.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cka.hcnkem.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://alh.jianghu66.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ujo.sjlbkw.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ljo.snrcjt.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mkv.shanyushiyangkeji.top


<!-- 参考信息 -->