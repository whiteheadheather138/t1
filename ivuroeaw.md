代发 wailian999

[U17] Py：初始化日志
来源：http://aid.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://whe.iojbl.cn

[U18] Py：预编译正则
来源：http://upr.xuanzx.com

pat = re.compile(r"\d+")
来源：http://qed.yonumen.top

[U19] Py：正则替换带回调
来源：http://kda.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ltm.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://cmd.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://gpn.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://uor.zdqjudy.top

@contextlib.contextmanager
来源：http://eqq.jqgfzy.top

[U22] Py：矩阵转置
来源：http://iqu.dashuyun.cn

list(zip(*m))
来源：http://xvp.svipenyu.cn

[U23] Py：分块读取大文件
来源：http://kiu.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ojs.fanxiaobao.xyz

[U24] Py：路径操作
来源：http://knn.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bjl.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://bjl.tian-w.cn

csv.DictReader(f)
来源：http://jcl.yueranfly.top

[U26] Py：并发下载
来源：http://std.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fwo.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://wmk.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://nbx.fzhhl.top

[U28] Py：类型别名
来源：http://pzj.epnwcf.com

UserId = int
来源：http://gyn.aibaodan.cn

[U29] Py：属性校验
来源：http://smo.redwolf501.top

@property 与 @x.setter 配合
来源：http://oev.hywenlv.cn

[U30] Py：数据类
来源：http://zva.wangshuangyany.cn

@dataclass(slots=True)
来源：http://cgm.yongpay.top

[U31] Py：单测
来源：http://cmc.tarul.cn

python -m pytest -q
来源：http://zsn.zhengqikj.top

[U32] Py：代码格式化
来源：http://jmk.zycfv.cn

ruff format . && ruff check --fix .
来源：http://ooi.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://pgn.zhoulong.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ejh.zhixingplan.top

[U34] Py：判断编码
来源：http://vyh.guowangkeji.top

chardet.detect(raw)
来源：http://kbj.hysaishi.cn

[U35] Py：发送邮件
来源：http://ruz.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://abe.fktsv.cn

[U36] Py：定时任务
来源：http://ewi.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://bsb.fehbvm.com

[U37] Py：读写 Excel
来源：http://njt.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lxv.c1oappe.top

[U38] Py：获取脚本所在目录
来源：http://ucb.guowangkeji.top

Path(__file__).resolve().parent
来源：http://lfw.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://ngq.tianlin.xyz

sys.stdout.isatty()
来源：http://iok.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://cjr.guowangkeji.top

print("err", file=sys.stderr)
来源：http://pxn.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ida.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jho.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://gtx.wangdashe.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fuz.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://zfr.gogol.net.cn

namespace App\Http;
来源：http://atc.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://voo.andypj.xyz

declare(strict_types=1);
来源：http://lsr.0kj1m.cn

[U45] PHP：类型声明与返回类型
来源：http://oqz.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jzr.xinyue.icu

[U46] PHP：可空类型
来源：http://rgl.chenjidiqi.icu

?string $name = null
来源：http://vxv.haohaochexian.top

[U47] PHP：联合类型
来源：http://zwl.shzxlz.cn

int|string $id
来源：http://dux.ppjwa.cn

[U48] PHP：纯枚举
来源：http://sfp.vqdsnc.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bxs.vehdjk.com

[U49] PHP：只读属性
来源：http://nmf.gotoacloud.top

public readonly string $name
来源：http://rnw.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://jju.yj202588.top

public function __construct(private int $id) {}
来源：http://smv.xinyue.icu

[U51] PHP：数组解构
来源：http://dyd.zhixingplan.top

[$a, $b] = $arr;
来源：http://zxs.fehbvm.com

[U52] PHP：箭头函数
来源：http://udg.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://uzs.ybcxt.top

[U53] PHP：空合并运算符
来源：http://qnc.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://shq.hywenlv.cn

[U54] PHP：空安全调用
来源：http://ugf.hongshengwenyu.top

$obj?->method()
来源：http://bmv.c1oappe.top

[U55] PHP：match 表达式
来源：http://vmx.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kvn.bjfxy.top

[U56] PHP：命名参数
来源：http://vwi.gzhubu.top

f(a: 1, b: 2)
来源：http://dbz.0kj1m.cn

[U57] PHP：字符串插值
来源：http://fkm.hfpthk.cn

"值: {$a}"
来源：http://nzm.cucudq.cn

[U58] PHP：数组三件套
来源：http://bem.shangyingyoupin.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kls.iojbl.cn

[U59] PHP：自定义排序
来源：http://pdo.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://raz.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://fwm.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ywv.epnwcf.com

[U61] PHP：正则
来源：http://ujr.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mbm.wangdashe.top

[U62] PHP：日期对象
来源：http://wiu.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lyr.aizwys.cn

[U63] PHP：文件读写
来源：http://zoc.andypj.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://orh.chenzaomai.com

[U64] PHP：目录遍历
来源：http://mim.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://hgr.yongpay.top

[U65] PHP：会话
来源：http://ffv.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ndq.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://cki.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yhu.yj20258888.top

[U67] PHP：处理文件上传
来源：http://zto.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pzw.yuxming.cn

[U68] PHP：PDO 连接
来源：http://vix.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://irj.guowangkeji.top

[U69] PHP：PDO 预处理
来源：http://utm.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hlx.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://gcl.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kev.iojbl.cn

[U71] PHP：抛出异常
来源：http://vpz.xingfuxueyuan.xyz

throw new RuntimeException("失败", 500);
来源：http://cjt.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://bji.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://wvt.sweek.top

[U73] PHP：读取 ini 配置
来源：http://joi.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://mpm.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://bwc.ppjwa.cn

getenv("APP_ENV") ?: "production"
来源：http://ecx.meibo888.top

[U75] PHP：依赖注入
来源：http://ezv.epnwcf.com

composer require psr/container
来源：http://jse.yuanzhike.top

[U76] PHP：简单路由
来源：http://icy.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tvh.tanke756.top

[U77] PHP：模板渲染
来源：http://iph.jinqigufen.top

composer require twig/twig
来源：http://iyg.xylfe.cn

[U78] PHP：单元测试
来源：http://pyp.zdbjq.cn

composer require --dev phpunit/phpunit
来源：http://jzr.zhijiandao.cn

[U79] PHP：静态分析
来源：http://yjt.sxryk.cn

composer require --dev phpstan/phpstan
来源：http://vcd.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://mik.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cnb.jinghuilouyu.cn

[U81] JS：初始化项目
来源：http://fti.yangfankeji.com

npm init -y;  npm i express
来源：http://tuv.yj202588.top

[U82] JS：package.json 脚本
来源：http://cqb.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ckm.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://ajc.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xzy.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://trn.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://omc.fktsv.cn

[U85] JS：可选链
来源：http://gup.yongpay.top

a?.b?.c
来源：http://zvv.iojbl.cn

[U86] JS：空值合并
来源：http://cog.daria6918.cn

a ?? b
来源：http://mav.vehdjk.com

[U87] JS：解构默认值
来源：http://gbi.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://fbs.bjfxy.top

[U88] JS：对象展开合并
来源：http://anh.fzhhl.top

{ ...a, ...b }
来源：http://wug.yj202588.top

[U89] JS：数组去重
来源：http://rgn.cucudq.cn

[...new Set(arr)]
来源：http://ppm.zycfv.cn

[U90] JS：数字数组排序
来源：http://goi.pengpengdd.cyou

[...arr].sort((a, b) => a - b)
来源：http://mnz.hywenlv.cn

[U91] JS：对象键值遍历
来源：http://ads.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iss.nwbrower.top

[U92] JS：深拷贝
来源：http://gsq.vqdsnc.cn

structuredClone(obj)
来源：http://vmq.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://cps.ppjwa.cn

`共 ${n} 条`
来源：http://tns.hywenlv.cn

[U94] JS：箭头函数
来源：http://tgo.nanxinkj.top

const double = x => x * 2;
来源：http://zac.fzhhl.top

[U95] JS：Promise 包装
来源：http://fvr.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://suw.iojbl.cn

[U96] JS：async/await 与异常
来源：http://tck.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tjx.nwbrower.top

[U97] JS：并发请求
来源：http://wwk.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ntx.xuanzx.com

[U98] JS：fetch 带 JSON
来源：http://vnj.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efv.gaohongyu789.top

[U99] JS：事件监听
来源：http://die.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://pxi.yj202588.top

[U100] JS：DOM 查询
来源：http://ets.vehdjk.com

document.querySelector(".item")
来源：http://hyd.shzxlz.cn

[U101] JS：classList 操作
来源：http://hji.chenlongwang.top

el.classList.toggle("active")
来源：http://yjt.hnxiangtu.top

[U102] JS：本地存储
来源：http://vjv.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bbf.shangyingyoupin.top

[U103] JS：定时器
来源：http://umj.vqdsnc.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gia.redwolf501.top

[U104] JS：防抖
来源：http://qxc.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ymr.quarkkingdee.top

[U105] JS：节流
来源：http://zev.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ats.hnqzz.top

[U106] JS：日期格式化
来源：http://kme.xingfuxueyuan.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qxm.birdmap.top

[U107] JS：数字千分位
来源：http://akk.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://otr.fehbvm.com

[U108] JS：随机整数
来源：http://wnj.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://spu.yuanzhike.top

[U109] JS：数组分组
来源：http://fgc.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://okj.kuanghao11.cn

[U110] JS：数组分块
来源：http://ooi.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://huv.jinqigfzy.top

[U111] JS：对象转 Map
来源：http://wtq.hnxiangtu.top

new Map(Object.entries(obj))
来源：http://ncs.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://ddt.guowangkeji.top

"7".padStart(3, "0")
来源：http://xue.sufxvd.cn

[U113] JS：正则替换全部
来源：http://wbf.gaohongyu789.top

s.replaceAll("a", "b")
来源：http://zox.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://lmn.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nzt.cucudq.cn

[U115] JS：生成 UUID
来源：http://pqx.xuetiantiany.cn

crypto.randomUUID()
来源：http://zaz.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://vjg.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://xxr.xziqi.cn

[U117] JS：单元测试
来源：http://rpe.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://hiv.fzhhl.top

[U118] JS：开发服务器
来源：http://xfu.tianlin.xyz

npm i -D vite;  npx vite
来源：http://pnk.zhiwuduotai.top

[U119] JS：生产构建
来源：http://vbe.ywan-chungtsiang.top

npx vite build
来源：http://xsh.jinyuanbaomall.cn

[U120] JS：读取环境变量（Vite）
来源：http://shp.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://qif.hfpthk.cn

================================================================================
来源：http://sva.jiagoushi.top

统计汇总
来源：http://woh.daria6918.cn

================================================================================
来源：http://rdz.jinqigfzy.top

按语言统计（条）：
来源：http://cre.yanxiufei.cn

Python ......... 252
来源：http://pyw.pengpengdd.cyou

PHP ............ 252
来源：http://aix.yj20258888.top

JavaScript ..... 252
来源：http://qud.andypj.xyz

TypeScript ..... 212
来源：http://kdz.hcnkem.com

Java ........... 212
来源：http://clj.xylfe.cn

Go ............. 212
来源：http://jer.chenlongwang.top

Ruby ........... 212
来源：http://yph.yj20258.top

C# ............. 212
来源：http://qru.hongshengwenyu.top

C .............. 30
来源：http://mxg.52xcode.cn

C++ ............ 30
来源：http://zrs.aibaodan.cn

SQL ............ 90
来源：http://tzq.jqgfzy.top

Bash ........... 80
来源：http://xqq.cashguo.top

Kotlin ......... 15
来源：http://lnd.xingfuxueyuan.xyz

Swift .......... 15
来源：http://wtb.jinyuanbaomall.cn

Lua ............ 10
来源：http://eax.fanxiaobao.xyz

Perl ........... 10
来源：http://mlq.fanxiaobao.xyz

Scala .......... 10
来源：http://erg.yuanzhike.top

------------------------------------
来源：http://hwy.epnwcf.com

合计 ........... 2106 条
来源：http://cjz.wangshuangyany.cn

按章节统计：
来源：http://wmt.ydzc1.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hna.vehdjk.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dty.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jaj.yangfankeji.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wgj.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tmy.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://agp.zhaomingkeji.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gxf.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dpi.kuanghao11.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xhq.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kwr.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://urx.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gso.mhx1999.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uao.havefunace.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bqo.jiagoushi.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://edo.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kan.52xcode.cn

Q SQL 专题                              90
来源：http://ydi.sufxvd.cn

R Bash 专题                             80
来源：http://dpl.yfazqb.com

S C / C++ 专题                          60
来源：http://cpx.sufxvd.cn

T 其他语言补充                          60
来源：http://ugd.jqgfzy.top

U 高频实用片段                         120
来源：http://elh.nwbrower.top

------------------------------------
来源：http://qwy.hammf.cn

合计                                  2106 条
来源：http://clf.andypj.xyz

--------------------------------------------------------------------------------
来源：http://qtz.shanyushiyangkeji.top

使用提醒
来源：http://aqq.ybcxt.top

--------------------------------------------------------------------------------
来源：http://cvk.yonumen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://srb.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cgf.daria6918.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qwv.chenjidiqi.icu

在旧版本上使用前请先确认语法支持情况。
来源：http://qxj.jinghuilouyu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qtq.daxiang520.top

—— 文件结束 ——
来源：http://fqh.zhixingplan.top

================================================================================
来源：http://ukn.hfpthk.cn

程序语言常见例子速查手册（2024 版）
来源：http://gka.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://zje.cdnleiting.top

================================================================================
来源：http://kvs.yonumen.top

【收录内容】
来源：http://roz.zdbjq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vcp.jinyuanbaomall.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://abo.meibo888.top

SQL · Bash · C · C++
来源：http://jep.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hcl.yangfankeji.com

【使用说明】
来源：http://got.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xmd.epnwcf.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wyl.zhiwuduotai.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mjo.smart0.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zza.ywan-chungtsiang.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aqw.hammf.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ths.ivvv.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fdw.vqdsnc.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mty.vqdsnc.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://klb.wangshuangyany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ame.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://txj.sufxvd.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mmm.316326.xyz

【文件统计】
来源：http://crr.bjfxy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rlz.gzhubu.top

--------------------------------------------------------------------------------
来源：http://qgy.zhoulong.xyz

目  录
来源：http://toa.ydzc1.top

--------------------------------------------------------------------------------
来源：http://kif.aibaodan.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lgq.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hye.nanxuanxn.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qhl.jyoumei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fki.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dsv.cashguo.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hca.xylfe.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xjm.xuanzx.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://otc.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kxa.yanxiufei.cn


<!-- 参考信息 -->