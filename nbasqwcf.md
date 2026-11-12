代发 wailian999

[U15] Py：高精度计时
来源：http://fjt.uphjek.com

t = time.perf_counter()
来源：http://egl.bjfxy.top

[U16] Py：命令行参数解析
来源：http://lsr.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ybk.daria6918.cn

[U17] Py：初始化日志
来源：http://odp.chenlongwang.top

logging.basicConfig(level=logging.INFO)
来源：http://fyd.sjlbkw.cn

[U18] Py：预编译正则
来源：http://rnk.fktsv.cn

pat = re.compile(r"\d+")
来源：http://wwe.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://aof.yuanzhike.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://slk.epnwcf.com

[U20] Py：缓存函数结果
来源：http://khc.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://vuh.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://cmw.wangshuangyany.cn

@contextlib.contextmanager
来源：http://mje.ehwqpu.com

[U22] Py：矩阵转置
来源：http://axc.aizwys.cn

list(zip(*m))
来源：http://fem.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://mcu.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://axc.ppjwa.cn

[U24] Py：路径操作
来源：http://upl.bbcook.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iqy.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://nto.yonumen.top

csv.DictReader(f)
来源：http://ssg.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://tfp.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bjn.epnwcf.com

[U27] Py：异步 HTTP
来源：http://dby.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://qel.uphjek.com

[U28] Py：类型别名
来源：http://fca.hcnkem.com

UserId = int
来源：http://bdm.hnxiangtu.top

[U29] Py：属性校验
来源：http://vli.havefunace.top

@property 与 @x.setter 配合
来源：http://cbj.hnqzz.top

[U30] Py：数据类
来源：http://aih.sjlbkw.cn

@dataclass(slots=True)
来源：http://ubd.yvedp.cn

[U31] Py：单测
来源：http://psq.haohaochexian.top

python -m pytest -q
来源：http://gdk.cashguo.top

[U32] Py：代码格式化
来源：http://xrn.zycfv.cn

ruff format . && ruff check --fix .
来源：http://gyc.hammf.cn

[U33] Py：打包发布
来源：http://ykb.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://pnv.jiagoushi.top

[U34] Py：判断编码
来源：http://aih.gzhubu.top

chardet.detect(raw)
来源：http://vci.jinghuilouyu.cn

[U35] Py：发送邮件
来源：http://yqg.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tfz.yfazqb.com

[U36] Py：定时任务
来源：http://dra.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://jne.sysykeji.top

[U37] Py：读写 Excel
来源：http://wtj.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://lkf.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://yir.daria6918.cn

Path(__file__).resolve().parent
来源：http://lat.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://djn.52xcode.cn

sys.stdout.isatty()
来源：http://apt.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://euj.fehbvm.com

print("err", file=sys.stderr)
来源：http://uti.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://ufi.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vjk.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://hih.chenlongwang.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vgh.ybcxt.top

[U43] PHP：声明命名空间
来源：http://ooq.chenjidiqi.icu

namespace App\Http;
来源：http://mqb.nwbrower.top

[U44] PHP：开启严格类型
来源：http://cjj.zdqjudy.top

declare(strict_types=1);
来源：http://asn.guowangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://vdn.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sco.zhijiandao.cn

[U46] PHP：可空类型
来源：http://isl.jqgfzy.top

?string $name = null
来源：http://lbh.guannengcc.top

[U47] PHP：联合类型
来源：http://swz.ywan-chungtsiang.top

int|string $id
来源：http://qan.zycfv.cn

[U48] PHP：纯枚举
来源：http://pzl.yueranfly.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jni.yonumen.top

[U49] PHP：只读属性
来源：http://flu.zycfv.cn

public readonly string $name
来源：http://afa.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://mdz.sjlbkw.cn

public function __construct(private int $id) {}
来源：http://zof.dashuyun.cn

[U51] PHP：数组解构
来源：http://ozt.c1oappe.top

[$a, $b] = $arr;
来源：http://dfx.vehdjk.com

[U52] PHP：箭头函数
来源：http://obx.uphjek.com

$double = fn($x) => $x * 2;
来源：http://kmn.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://vzk.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://pye.epnwcf.com

[U54] PHP：空安全调用
来源：http://nzl.jlsjyb.cn

$obj?->method()
来源：http://awt.zhiwuduotai.top

[U55] PHP：match 表达式
来源：http://ynf.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eaf.ivvv.top

[U56] PHP：命名参数
来源：http://vtx.ppjwa.cn

f(a: 1, b: 2)
来源：http://zht.guowangkeji.top

[U57] PHP：字符串插值
来源：http://buq.vehdjk.com

"值: {$a}"
来源：http://mud.hnqzz.top

[U58] PHP：数组三件套
来源：http://ajb.zdqjudy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wdd.hysaishi.cn

[U59] PHP：自定义排序
来源：http://eqf.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pij.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://jkb.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eeh.hesvh.cn

[U61] PHP：正则
来源：http://acl.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qji.fktsv.cn

[U62] PHP：日期对象
来源：http://fgl.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qed.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://oyi.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vrr.zycfv.cn

[U64] PHP：目录遍历
来源：http://hrm.hnqzz.top

glob("dir/*.php");  scandir("dir");
来源：http://icm.zhijiandao.cn

[U65] PHP：会话
来源：http://mwf.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://rkl.havefunace.top

[U66] PHP：设置 Cookie
来源：http://hyp.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rmu.aizwys.cn

[U67] PHP：处理文件上传
来源：http://vnw.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dte.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://slc.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rfr.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://lgs.hesvh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pvk.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://hzg.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://utd.nanxinkj.top

[U71] PHP：抛出异常
来源：http://gfz.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://ynb.jinghuilouyu.cn

[U72] PHP：写错误日志
来源：http://oft.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://qkk.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://nqz.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://mpt.cashguo.top

[U74] PHP：读取环境变量
来源：http://npg.wangdashe.top

getenv("APP_ENV") ?: "production"
来源：http://hen.yueranfly.top

[U75] PHP：依赖注入
来源：http://tan.wangdashe.top

composer require psr/container
来源：http://uic.zhongyouzk.top

[U76] PHP：简单路由
来源：http://ymx.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://eyb.guannengcc.top

[U77] PHP：模板渲染
来源：http://sgs.mhx1999.top

composer require twig/twig
来源：http://wbx.yj20258888.top

[U78] PHP：单元测试
来源：http://zlq.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://wjl.feifeiyinyue.top

[U79] PHP：静态分析
来源：http://yyt.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://nuy.52xcode.cn

[U80] PHP：代码规范修复
来源：http://fkv.feifeiyinyue.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nrd.andypj.xyz

[U81] JS：初始化项目
来源：http://qxp.hywenlv.cn

npm init -y;  npm i express
来源：http://mmc.ybcxt.top

[U82] JS：package.json 脚本
来源：http://tqi.shangyingyoupin.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wnc.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://vop.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nbj.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://pfh.sjlbkw.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dcf.hongshengwenyu.top

[U85] JS：可选链
来源：http://lao.gogol.net.cn

a?.b?.c
来源：http://qea.hysaishi.cn

[U86] JS：空值合并
来源：http://xeu.zycfv.cn

a ?? b
来源：http://run.cheryme.top

[U87] JS：解构默认值
来源：http://btx.tarul.cn

const { a = 1, b = 2 } = obj;
来源：http://gud.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://srt.cucudq.cn

{ ...a, ...b }
来源：http://dmj.tianlin.xyz

[U89] JS：数组去重
来源：http://crx.xuanzx.com

[...new Set(arr)]
来源：http://kds.c1oappe.top

[U90] JS：数字数组排序
来源：http://hby.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://mgd.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://our.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kgv.jinqigufen.top

[U92] JS：深拷贝
来源：http://mlz.gzhubu.top

structuredClone(obj)
来源：http://nhw.cucudq.cn

[U93] JS：模板字符串
来源：http://gwg.dianchejie.cn

`共 ${n} 条`
来源：http://cld.shuidangran.top

[U94] JS：箭头函数
来源：http://ztb.xuanzx.com

const double = x => x * 2;
来源：http://jqf.fengsongda.top

[U95] JS：Promise 包装
来源：http://fsx.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://obk.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://hng.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ufc.0kj1m.cn

[U97] JS：并发请求
来源：http://wqd.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aya.daxiang520.top

[U98] JS：fetch 带 JSON
来源：http://loh.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eli.jqgfzy.top

[U99] JS：事件监听
来源：http://qwo.mhx1999.top

el.addEventListener("click", e => {})
来源：http://qoo.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://tek.yongpay.top

document.querySelector(".item")
来源：http://ymt.yueranfly.top

[U101] JS：classList 操作
来源：http://skl.wangdashe.top

el.classList.toggle("active")
来源：http://ztg.xuanzx.com

[U102] JS：本地存储
来源：http://avk.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vhe.hesvh.cn

[U103] JS：定时器
来源：http://xbc.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ijd.sweek.top

[U104] JS：防抖
来源：http://bvn.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvc.ywan-chungtsiang.top

[U105] JS：节流
来源：http://kos.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://idn.quarkkingdee.top

[U106] JS：日期格式化
来源：http://dda.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tmt.chenzaomai.com

[U107] JS：数字千分位
来源：http://bjr.iojbl.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wou.uphjek.com

[U108] JS：随机整数
来源：http://dzh.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yda.meibo888.top

[U109] JS：数组分组
来源：http://qdu.shuidangran.top

Object.groupBy(arr, x => x.type)
来源：http://zug.fengsongda.top

[U110] JS：数组分块
来源：http://cux.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xgs.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://lbc.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://zew.jinqigfzy.top

[U112] JS：字符串补位
来源：http://ruz.tarul.cn

"7".padStart(3, "0")
来源：http://uya.cdnleiting.top

[U113] JS：正则替换全部
来源：http://kqy.shuidangran.top

s.replaceAll("a", "b")
来源：http://hsm.mhx1999.top

[U114] JS：JSON 深比较
来源：http://ejo.hnxiangtu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://loa.dianchejie.cn

[U115] JS：生成 UUID
来源：http://uxg.havefunace.top

crypto.randomUUID()
来源：http://umv.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://mnx.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://pkg.birdmap.top

[U117] JS：单元测试
来源：http://piq.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://ffh.chenzaomai.com

[U118] JS：开发服务器
来源：http://zeq.316326.xyz

npm i -D vite;  npx vite
来源：http://unf.daxiang520.top

[U119] JS：生产构建
来源：http://hml.havefunace.top

npx vite build
来源：http://zoe.zhaomingkeji.xyz

[U120] JS：读取环境变量（Vite）
来源：http://pnd.guannengcc.top

import.meta.env.VITE_API_URL
来源：http://ygi.ivvv.top

================================================================================
来源：http://iqe.tian-w.cn

统计汇总
来源：http://jjc.aibaodan.cn

================================================================================
来源：http://hcm.zhoulong.xyz

按语言统计（条）：
来源：http://qko.aibaodan.cn

Python ......... 252
来源：http://hgv.sufxvd.cn

PHP ............ 252
来源：http://fxq.fzhhl.top

JavaScript ..... 252
来源：http://fuf.wangdashe.top

TypeScript ..... 212
来源：http://cmp.guannengcc.top

Java ........... 212
来源：http://rmb.nwbrower.top

Go ............. 212
来源：http://yra.chenjidiqi.icu

Ruby ........... 212
来源：http://jeb.zdbjq.cn

C# ............. 212
来源：http://gey.iojbl.cn

C .............. 30
来源：http://mgh.xingfuxueyuan.xyz

C++ ............ 30
来源：http://zga.yangfankeji.com

SQL ............ 90
来源：http://qju.yfazqb.com

Bash ........... 80
来源：http://lwd.jianghu66.top

Kotlin ......... 15
来源：http://wtd.ydzc1.top

Swift .......... 15
来源：http://pcd.feifeiyinyue.top

Lua ............ 10
来源：http://twa.dianchejie.cn

Perl ........... 10
来源：http://iyl.jqgufenzy.top

Scala .......... 10
来源：http://pca.aibaodan.cn

------------------------------------
来源：http://beg.uphjek.com

合计 ........... 2106 条
来源：http://efh.yanxiufei.cn

按章节统计：
来源：http://mmo.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pkw.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pxq.kuanghao11.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://krb.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uak.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sxk.chenzaomai.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zvg.wangshuangyany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tyg.0kj1m.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xfv.yangfankeji.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qcf.ydjk.org.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pwj.cashguo.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ibf.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lus.xinyue.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vcu.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nov.cucudq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qas.52xcode.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://awl.vehdjk.com

Q SQL 专题                              90
来源：http://zhp.fzhhl.top

R Bash 专题                             80
来源：http://zsh.c1oappe.top

S C / C++ 专题                          60
来源：http://ukx.xylfe.cn

T 其他语言补充                          60
来源：http://lun.jinqigufen.top

U 高频实用片段                         120
来源：http://kzb.zdqjudy.top

------------------------------------
来源：http://osa.jiagoushi.top

合计                                  2106 条
来源：http://mgn.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://zxz.sufxvd.cn

使用提醒
来源：http://rfi.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://hpy.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pgs.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hbw.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ssa.ehwqpu.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qzu.feifeiyinyue.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qis.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://fbu.guowangkeji.top

================================================================================
来源：http://avm.smart0.xyz

程序语言常见例子速查手册（2024 版）
来源：http://fyb.chenlongwang.top

Common Programming Examples Cheat Book
来源：http://fav.shuidangran.top

================================================================================
来源：http://rlv.fzhhl.top

【收录内容】
来源：http://bsa.dashuyun.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sya.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jnv.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://mgz.hfpthk.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xes.yangfankeji.com

【使用说明】
来源：http://vjg.shzxlz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fym.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qfy.hongshengwenyu.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://enw.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hbf.cheryme.top

Bash:  Shell         C:     C             C++:   C++
来源：http://idv.zhongyouzk.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://khp.redwolf501.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wua.fanxiaobao.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://avl.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ppv.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cre.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wre.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hme.shanyushiyangtech.top

【文件统计】
来源：http://xao.bbcook.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://htm.yongpay.top

--------------------------------------------------------------------------------
来源：http://ezz.nanxinkj.top

目  录
来源：http://cvs.yfazqb.com

--------------------------------------------------------------------------------
来源：http://jlj.52xcode.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lun.0kj1m.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ggy.c1oappe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://grf.xziqi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pkq.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://saj.hnqzz.top


<!-- 参考信息 -->