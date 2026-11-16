代发 wailian999

[U17] Py：初始化日志
来源：http://jdf.xuetiantiany.cn

logging.basicConfig(level=logging.INFO)
来源：http://zyq.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://azg.xylfe.cn

pat = re.compile(r"\d+")
来源：http://vvm.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://ssk.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ada.uphjek.com

[U20] Py：缓存函数结果
来源：http://fxz.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://uap.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://qdy.hfpthk.cn

@contextlib.contextmanager
来源：http://eyg.sufxvd.cn

[U22] Py：矩阵转置
来源：http://odv.zycfv.cn

list(zip(*m))
来源：http://djh.ybcxt.top

[U23] Py：分块读取大文件
来源：http://qpp.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vqm.zhiwuduotai.top

[U24] Py：路径操作
来源：http://cuo.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mac.nanxinkj.top

[U25] Py：CSV 按字典读
来源：http://svu.wangdashe.top

csv.DictReader(f)
来源：http://vqk.bjfxy.top

[U26] Py：并发下载
来源：http://fid.dashuyun.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lsu.gzhubu.top

[U27] Py：异步 HTTP
来源：http://rox.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://cgt.daxiang520.top

[U28] Py：类型别名
来源：http://wtu.zdbjq.cn

UserId = int
来源：http://agd.chenjidiqi.icu

[U29] Py：属性校验
来源：http://rkt.tarul.cn

@property 与 @x.setter 配合
来源：http://ahv.yfazqb.com

[U30] Py：数据类
来源：http://lzq.feifeiyinyue.top

@dataclass(slots=True)
来源：http://jyy.sweek.top

[U31] Py：单测
来源：http://rmh.jinqigfzy.top

python -m pytest -q
来源：http://jaz.havefunace.top

[U32] Py：代码格式化
来源：http://wtx.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://msm.cucudq.cn

[U33] Py：打包发布
来源：http://rii.0kj1m.cn

python -m build  （依赖 pyproject.toml）
来源：http://pdm.ppjwa.cn

[U34] Py：判断编码
来源：http://gpe.meibo888.top

chardet.detect(raw)
来源：http://coa.wangshuangyany.cn

[U35] Py：发送邮件
来源：http://yxx.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kht.havefunace.top

[U36] Py：定时任务
来源：http://xfk.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://nzz.tarul.cn

[U37] Py：读写 Excel
来源：http://azk.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://oxi.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://gqy.xinyue.icu

Path(__file__).resolve().parent
来源：http://azl.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://bme.chenjidiqi.icu

sys.stdout.isatty()
来源：http://vsi.meibo888.top

[U40] Py：打印到标准错误
来源：http://uka.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://uiz.yonumen.top

[U41] PHP：初始化 Composer 项目
来源：http://cgp.daria6918.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mky.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://txb.quarkkingdee.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nsz.sxryk.cn

[U43] PHP：声明命名空间
来源：http://ghi.dashuyun.cn

namespace App\Http;
来源：http://uky.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://kqe.jqgfzy.top

declare(strict_types=1);
来源：http://gah.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://epc.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://bfh.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://sdh.yangfankeji.com

?string $name = null
来源：http://tyx.0kj1m.cn

[U47] PHP：联合类型
来源：http://dkc.cheryme.top

int|string $id
来源：http://imu.fengsongda.top

[U48] PHP：纯枚举
来源：http://hpx.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ytz.sysykeji.top

[U49] PHP：只读属性
来源：http://bfp.nanxuanxn.top

public readonly string $name
来源：http://hbv.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://dpy.yvedp.cn

public function __construct(private int $id) {}
来源：http://yrd.316326.xyz

[U51] PHP：数组解构
来源：http://vdr.zdqjudy.top

[$a, $b] = $arr;
来源：http://zzt.sxryk.cn

[U52] PHP：箭头函数
来源：http://gyb.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://vqu.hnxiangtu.top

[U53] PHP：空合并运算符
来源：http://xmo.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://uxu.haohaochexian.top

[U54] PHP：空安全调用
来源：http://vku.fengsongda.top

$obj?->method()
来源：http://qkl.yongpay.top

[U55] PHP：match 表达式
来源：http://wlu.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jgj.guannengcc.top

[U56] PHP：命名参数
来源：http://tpa.tian-w.cn

f(a: 1, b: 2)
来源：http://umo.vehdjk.com

[U57] PHP：字符串插值
来源：http://agd.snrcjt.cn

"值: {$a}"
来源：http://aea.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://urx.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ati.snrcjt.cn

[U59] PHP：自定义排序
来源：http://udt.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ris.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://lps.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oib.ivvv.top

[U61] PHP：正则
来源：http://omw.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rdy.havefunace.top

[U62] PHP：日期对象
来源：http://rmo.zhixingplan.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ojp.jinqigfzy.top

[U63] PHP：文件读写
来源：http://htj.zdqjudy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lmr.hcnkem.com

[U64] PHP：目录遍历
来源：http://yed.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://msq.yfazqb.com

[U65] PHP：会话
来源：http://hzu.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lop.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://hpc.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gbc.mhx1999.top

[U67] PHP：处理文件上传
来源：http://peh.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dzh.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://iqr.nwbrower.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://etb.meibo888.top

[U69] PHP：PDO 预处理
来源：http://hpw.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://epo.dashuyun.cn

[U70] PHP：PDO 事务
来源：http://agg.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ssr.fktsv.cn

[U71] PHP：抛出异常
来源：http://abe.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://yul.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://ojq.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://uau.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://wpe.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://gft.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://vwz.ywan-chungtsiang.top

getenv("APP_ENV") ?: "production"
来源：http://flh.9152youxi.cn

[U75] PHP：依赖注入
来源：http://tkp.shangyingyoupin.top

composer require psr/container
来源：http://gjo.52xcode.cn

[U76] PHP：简单路由
来源：http://vnt.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://evj.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://gju.ivvv.top

composer require twig/twig
来源：http://bdi.hongshengwenyu.top

[U78] PHP：单元测试
来源：http://npa.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://qmd.hammf.cn

[U79] PHP：静态分析
来源：http://qme.yongpay.top

composer require --dev phpstan/phpstan
来源：http://cod.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://hfa.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nub.ppjwa.cn

[U81] JS：初始化项目
来源：http://col.zycfv.cn

npm init -y;  npm i express
来源：http://qin.bjfxy.top

[U82] JS：package.json 脚本
来源：http://jvt.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jfh.cqqwz.cn

[U83] JS：ES Module 导入导出
来源：http://ywh.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://ikb.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://zzb.guannengcc.top

module.exports = { a };  const { a } = require("./m");
来源：http://vgi.nwbrower.top

[U85] JS：可选链
来源：http://zwg.jiagoushi.top

a?.b?.c
来源：http://lti.sxryk.cn

[U86] JS：空值合并
来源：http://klp.0kj1m.cn

a ?? b
来源：http://xcp.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://qhn.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://lzz.hesvh.cn

[U88] JS：对象展开合并
来源：http://gna.hywenlv.cn

{ ...a, ...b }
来源：http://uol.jyoumei.cn

[U89] JS：数组去重
来源：http://xti.havefunace.top

[...new Set(arr)]
来源：http://dyt.birdmap.top

[U90] JS：数字数组排序
来源：http://uts.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://lbc.smart0.xyz

[U91] JS：对象键值遍历
来源：http://rxf.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wrr.dashuyun.cn

[U92] JS：深拷贝
来源：http://dmw.ywan-chungtsiang.top

structuredClone(obj)
来源：http://rop.yongpay.top

[U93] JS：模板字符串
来源：http://wdd.yj20258.top

`共 ${n} 条`
来源：http://xbm.ydzc1.top

[U94] JS：箭头函数
来源：http://nsx.tanke756.top

const double = x => x * 2;
来源：http://odr.yuanzhike.top

[U95] JS：Promise 包装
来源：http://dxq.uphjek.com

new Promise((resolve, reject) => {})
来源：http://elf.nwbrower.top

[U96] JS：async/await 与异常
来源：http://leg.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lmo.shangyingyoupin.top

[U97] JS：并发请求
来源：http://ofh.bbcook.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rqe.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://oqo.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qtd.vehdjk.com

[U99] JS：事件监听
来源：http://wwl.bbcook.cn

el.addEventListener("click", e => {})
来源：http://nhi.chenjidiqi.icu

[U100] JS：DOM 查询
来源：http://kqt.pengpengdd.cyou

document.querySelector(".item")
来源：http://kpi.ydzc1.top

[U101] JS：classList 操作
来源：http://ney.cheryme.top

el.classList.toggle("active")
来源：http://xpl.jinqigfzy.top

[U102] JS：本地存储
来源：http://pyf.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kjh.xuanzx.com

[U103] JS：定时器
来源：http://sgi.sweek.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eqq.guowangkeji.top

[U104] JS：防抖
来源：http://zoy.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yud.hesvh.cn

[U105] JS：节流
来源：http://krt.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ivo.cucudq.cn

[U106] JS：日期格式化
来源：http://zzp.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xlx.zhixingplan.top

[U107] JS：数字千分位
来源：http://noa.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ssw.wangshuangyany.cn

[U108] JS：随机整数
来源：http://zvu.yj20258.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cgv.chenlongwang.top

[U109] JS：数组分组
来源：http://ely.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://qqu.hywenlv.cn

[U110] JS：数组分块
来源：http://jxe.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ykw.tianlin.xyz

[U111] JS：对象转 Map
来源：http://fiz.mhx1999.top

new Map(Object.entries(obj))
来源：http://fyi.bbcook.cn

[U112] JS：字符串补位
来源：http://naz.yj202588.top

"7".padStart(3, "0")
来源：http://vsb.nanxinkj.top

[U113] JS：正则替换全部
来源：http://pym.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://xra.redwolf501.top

[U114] JS：JSON 深比较
来源：http://isj.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ffi.chenzaomai.com

[U115] JS：生成 UUID
来源：http://lwy.hongshengwenyu.top

crypto.randomUUID()
来源：http://uav.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://zml.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://aig.ehwqpu.com

[U117] JS：单元测试
来源：http://iwz.jqgfzy.top

npm i -D vitest;  npx vitest
来源：http://kle.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://vts.jianghu66.top

npm i -D vite;  npx vite
来源：http://yfa.zhixingplan.top

[U119] JS：生产构建
来源：http://qtg.jinqigfzy.top

npx vite build
来源：http://jsw.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://vdg.cheryme.top

import.meta.env.VITE_API_URL
来源：http://aee.daria6918.cn

================================================================================
来源：http://col.zdbjq.cn

统计汇总
来源：http://zea.mhx1999.top

================================================================================
来源：http://yoo.daria6918.cn

按语言统计（条）：
来源：http://gjb.nwbrower.top

Python ......... 252
来源：http://xsh.havefunace.top

PHP ............ 252
来源：http://czl.tanke756.top

JavaScript ..... 252
来源：http://lkx.vehdjk.com

TypeScript ..... 212
来源：http://kpt.sysykeji.top

Java ........... 212
来源：http://eum.ehwqpu.com

Go ............. 212
来源：http://uwh.yueranfly.top

Ruby ........... 212
来源：http://din.sjlbkw.cn

C# ............. 212
来源：http://spo.jianghu66.top

C .............. 30
来源：http://ghb.hongshengwenyu.top

C++ ............ 30
来源：http://qnv.ywan-chungtsiang.top

SQL ............ 90
来源：http://mpk.ivvv.top

Bash ........... 80
来源：http://mig.yj202588.top

Kotlin ......... 15
来源：http://rso.xziqi.cn

Swift .......... 15
来源：http://rhf.uphjek.com

Lua ............ 10
来源：http://zdk.ybcxt.top

Perl ........... 10
来源：http://akp.pycfn.com

Scala .......... 10
来源：http://pvo.jianghu66.top

------------------------------------
来源：http://xun.chenzaomai.com

合计 ........... 2106 条
来源：http://jln.shzxlz.cn

按章节统计：
来源：http://nfr.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fvf.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nud.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xhj.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rkh.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yxo.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uqm.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rln.xziqi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uhk.epnwcf.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dja.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hvb.ybcxt.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zys.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://usy.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vbf.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://apq.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ooz.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oxu.hnxiangtu.top

Q SQL 专题                              90
来源：http://zfz.ivvv.top

R Bash 专题                             80
来源：http://exh.jqgufenzy.top

S C / C++ 专题                          60
来源：http://tmo.zhongyouzk.top

T 其他语言补充                          60
来源：http://tbv.gzhubu.top

U 高频实用片段                         120
来源：http://not.yonumen.top

------------------------------------
来源：http://fsd.pengpengdd.cyou

合计                                  2106 条
来源：http://ejm.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://faf.tianlin.xyz

使用提醒
来源：http://scl.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://ieq.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vfe.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gkh.fktsv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qlu.cqqwz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qqp.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yoh.fanxiaobao.xyz

—— 文件结束 ——
来源：http://hta.cucudq.cn

================================================================================
来源：http://euz.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://tkq.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://thv.hywenlv.cn

================================================================================
来源：http://uvx.tanke756.top

【收录内容】
来源：http://zix.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hrg.hongshengwenyu.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wcw.fehbvm.com

SQL · Bash · C · C++
来源：http://nsi.zdqjudy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mgx.zhixingplan.top

【使用说明】
来源：http://hfj.yj20258.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fye.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://igb.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://avi.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mpm.zhiwuduotai.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nlq.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blp.hongshengwenyu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zhx.hcnkem.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ofy.guannengcc.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qhi.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lnm.zhengqikj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iwr.hfpthk.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://twh.svipenyu.cn

【文件统计】
来源：http://qoe.xingfuxueyuan.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yrl.tarul.cn

--------------------------------------------------------------------------------
来源：http://yji.jinghuilouyu.cn

目  录
来源：http://vye.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://syt.chenjidiqi.icu

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hnd.zdqjudy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hyf.iojbl.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wia.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kee.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://egi.hongshengwenyu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://onp.hnqzz.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kcz.zhongyouzk.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rzf.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://max.meibo888.top


<!-- 参考信息 -->