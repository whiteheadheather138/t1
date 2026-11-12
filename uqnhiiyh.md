代发 wailian999

[U15] Py：高精度计时
来源：http://cvb.nwbrower.top

t = time.perf_counter()
来源：http://eun.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://oaq.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bnx.bjfxy.top

[U17] Py：初始化日志
来源：http://xrj.hammf.cn

logging.basicConfig(level=logging.INFO)
来源：http://bju.zdqjudy.top

[U18] Py：预编译正则
来源：http://qhq.uphjek.com

pat = re.compile(r"\d+")
来源：http://joq.xylfe.cn

[U19] Py：正则替换带回调
来源：http://thf.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nhe.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://etb.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://jin.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://phe.hnxiangtu.top

@contextlib.contextmanager
来源：http://uuy.xziqi.cn

[U22] Py：矩阵转置
来源：http://kff.aizwys.cn

list(zip(*m))
来源：http://ycj.cucudq.cn

[U23] Py：分块读取大文件
来源：http://cif.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qtf.mhx1999.top

[U24] Py：路径操作
来源：http://xek.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nuc.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://wjt.yj20258.top

csv.DictReader(f)
来源：http://elz.chenzaomai.com

[U26] Py：并发下载
来源：http://hsg.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://try.yuxming.cn

[U27] Py：异步 HTTP
来源：http://tok.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://gfy.xziqi.cn

[U28] Py：类型别名
来源：http://smu.cdnleiting.top

UserId = int
来源：http://exq.sjlbkw.cn

[U29] Py：属性校验
来源：http://tpw.nwbrower.top

@property 与 @x.setter 配合
来源：http://png.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://lbp.jqgufenzy.top

@dataclass(slots=True)
来源：http://bcw.gotoacloud.top

[U31] Py：单测
来源：http://ppe.havefunace.top

python -m pytest -q
来源：http://epe.zhengqikj.top

[U32] Py：代码格式化
来源：http://iaf.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://kil.redwolf501.top

[U33] Py：打包发布
来源：http://gux.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://uyz.zhiwuduotai.top

[U34] Py：判断编码
来源：http://vpf.zhengqikj.top

chardet.detect(raw)
来源：http://hki.aibaodan.cn

[U35] Py：发送邮件
来源：http://nlw.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://toc.zdbjq.cn

[U36] Py：定时任务
来源：http://mov.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://zrq.jyoumei.cn

[U37] Py：读写 Excel
来源：http://ddc.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://nxr.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://tza.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://yew.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://xnc.cheryme.top

sys.stdout.isatty()
来源：http://srw.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://lgm.yj20258.top

print("err", file=sys.stderr)
来源：http://qnx.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://ieh.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://noj.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://pbx.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dws.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://zqt.yvedp.cn

namespace App\Http;
来源：http://cyv.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://jkd.aizwys.cn

declare(strict_types=1);
来源：http://fjk.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://bab.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ahq.nanxinkj.top

[U46] PHP：可空类型
来源：http://xkj.vqdsnc.cn

?string $name = null
来源：http://rcb.xziqi.cn

[U47] PHP：联合类型
来源：http://llj.bjfxy.top

int|string $id
来源：http://rtq.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://yuy.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uwx.tianlin.xyz

[U49] PHP：只读属性
来源：http://omv.shanyushiyangtech.top

public readonly string $name
来源：http://nfi.birdmap.top

[U50] PHP：构造器属性提升
来源：http://zzo.fehbvm.com

public function __construct(private int $id) {}
来源：http://iqu.ydzc1.top

[U51] PHP：数组解构
来源：http://jat.guannengcc.top

[$a, $b] = $arr;
来源：http://pmw.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://ire.yj202588.top

$double = fn($x) => $x * 2;
来源：http://huw.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://grj.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://xhi.daria6918.cn

[U54] PHP：空安全调用
来源：http://cln.zhijiandao.cn

$obj?->method()
来源：http://mza.zdbjq.cn

[U55] PHP：match 表达式
来源：http://qdv.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://udl.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://tge.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://hwj.wangdashe.top

[U57] PHP：字符串插值
来源：http://oga.cheryme.top

"值: {$a}"
来源：http://sgb.fehbvm.com

[U58] PHP：数组三件套
来源：http://vja.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mmd.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://hzi.sufxvd.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tjq.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://hgm.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ogu.sufxvd.cn

[U61] PHP：正则
来源：http://ufn.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qmh.guannengcc.top

[U62] PHP：日期对象
来源：http://mgg.cqqwz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://onh.yuxming.cn

[U63] PHP：文件读写
来源：http://zql.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uly.cheryme.top

[U64] PHP：目录遍历
来源：http://wso.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://nll.svipenyu.cn

[U65] PHP：会话
来源：http://pog.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wwm.hammf.cn

[U66] PHP：设置 Cookie
来源：http://hfc.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nfr.uphjek.com

[U67] PHP：处理文件上传
来源：http://srn.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jrx.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://zqq.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kjk.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://mss.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fox.yvedp.cn

[U70] PHP：PDO 事务
来源：http://bjk.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qot.yj20258.top

[U71] PHP：抛出异常
来源：http://dik.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://oqn.yanxiufei.cn

[U72] PHP：写错误日志
来源：http://qgt.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://ckd.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://hhl.cdnleiting.top

parse_ini_file("config.ini", true)
来源：http://mlo.zycfv.cn

[U74] PHP：读取环境变量
来源：http://ihq.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://dzz.xuanzx.com

[U75] PHP：依赖注入
来源：http://ucr.ybcxt.top

composer require psr/container
来源：http://tbt.xylfe.cn

[U76] PHP：简单路由
来源：http://xil.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bux.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://gmg.xziqi.cn

composer require twig/twig
来源：http://eho.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://rdj.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://yni.shzxlz.cn

[U79] PHP：静态分析
来源：http://bjq.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://nlt.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://ecq.cheryme.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://enn.guowangkeji.top

[U81] JS：初始化项目
来源：http://cgo.bjfxy.top

npm init -y;  npm i express
来源：http://jua.fengsongda.top

[U82] JS：package.json 脚本
来源：http://khi.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eww.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://vio.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wmw.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://fjj.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ecu.jlsjyb.cn

[U85] JS：可选链
来源：http://gsu.shangyingyoupin.top

a?.b?.c
来源：http://azj.jianghu66.top

[U86] JS：空值合并
来源：http://owj.cqqwz.cn

a ?? b
来源：http://nuf.yonumen.top

[U87] JS：解构默认值
来源：http://kpi.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://pbg.dianchejie.cn

[U88] JS：对象展开合并
来源：http://bze.zdbjq.cn

{ ...a, ...b }
来源：http://ewv.gaohongyu789.top

[U89] JS：数组去重
来源：http://lvl.jlsjyb.cn

[...new Set(arr)]
来源：http://cun.tanke756.top

[U90] JS：数字数组排序
来源：http://ina.bjfxy.top

[...arr].sort((a, b) => a - b)
来源：http://ayc.tian-w.cn

[U91] JS：对象键值遍历
来源：http://low.hcnkem.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kut.tanke756.top

[U92] JS：深拷贝
来源：http://ktd.yuanzhike.top

structuredClone(obj)
来源：http://vfg.vqdsnc.cn

[U93] JS：模板字符串
来源：http://wmr.sxryk.cn

`共 ${n} 条`
来源：http://iqu.gotoacloud.top

[U94] JS：箭头函数
来源：http://wjr.sysykeji.top

const double = x => x * 2;
来源：http://emp.sjlbkw.cn

[U95] JS：Promise 包装
来源：http://tac.yonumen.top

new Promise((resolve, reject) => {})
来源：http://fsw.jqgfzy.top

[U96] JS：async/await 与异常
来源：http://fqe.nanxinkj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hig.hnqzz.top

[U97] JS：并发请求
来源：http://uas.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://inz.chenlongwang.top

[U98] JS：fetch 带 JSON
来源：http://yfs.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zgl.sufxvd.cn

[U99] JS：事件监听
来源：http://iib.xylfe.cn

el.addEventListener("click", e => {})
来源：http://wjv.nwbrower.top

[U100] JS：DOM 查询
来源：http://jbw.nwbrower.top

document.querySelector(".item")
来源：http://pma.yuxming.cn

[U101] JS：classList 操作
来源：http://gfr.wangshuangyany.cn

el.classList.toggle("active")
来源：http://bdf.daxiang520.top

[U102] JS：本地存储
来源：http://bgd.meibo888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jay.fanxiaobao.xyz

[U103] JS：定时器
来源：http://pkh.ivvv.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://whn.tian-w.cn

[U104] JS：防抖
来源：http://anj.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zfg.jyoumei.cn

[U105] JS：节流
来源：http://zgw.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tvo.hnqzz.top

[U106] JS：日期格式化
来源：http://cto.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewm.nanxinkj.top

[U107] JS：数字千分位
来源：http://dfh.xinyue.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zfr.svipenyu.cn

[U108] JS：随机整数
来源：http://snm.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aca.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://fia.yongpay.top

Object.groupBy(arr, x => x.type)
来源：http://crt.yj20258888.top

[U110] JS：数组分块
来源：http://puk.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lyr.sysykeji.top

[U111] JS：对象转 Map
来源：http://fzn.nanxuanxn.top

new Map(Object.entries(obj))
来源：http://led.kuanghao11.cn

[U112] JS：字符串补位
来源：http://jzd.guannengcc.top

"7".padStart(3, "0")
来源：http://dws.daria6918.cn

[U113] JS：正则替换全部
来源：http://flq.pycfn.com

s.replaceAll("a", "b")
来源：http://zyg.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://sxu.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rqc.mhx1999.top

[U115] JS：生成 UUID
来源：http://ahq.redwolf501.top

crypto.randomUUID()
来源：http://lfc.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://qnn.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://som.vqdsnc.cn

[U117] JS：单元测试
来源：http://shw.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://iyw.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://rsw.jianghu66.top

npm i -D vite;  npx vite
来源：http://sez.yvedp.cn

[U119] JS：生产构建
来源：http://tmc.chenlongwang.top

npx vite build
来源：http://noe.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://ozq.uphjek.com

import.meta.env.VITE_API_URL
来源：http://api.yonumen.top

================================================================================
来源：http://qrs.yangfankeji.com

统计汇总
来源：http://hvd.wangshuangyany.cn

================================================================================
来源：http://mhi.gogol.net.cn

按语言统计（条）：
来源：http://wno.gzhubu.top

Python ......... 252
来源：http://ntx.tanke756.top

PHP ............ 252
来源：http://ife.guowangkeji.top

JavaScript ..... 252
来源：http://xvf.jlsjyb.cn

TypeScript ..... 212
来源：http://jbr.nwbrower.top

Java ........... 212
来源：http://esm.jinqigufen.top

Go ............. 212
来源：http://pvu.ydzc1.top

Ruby ........... 212
来源：http://pmh.yj20258888.top

C# ............. 212
来源：http://hab.nwbrower.top

C .............. 30
来源：http://jov.yanxiufei.cn

C++ ............ 30
来源：http://hti.9152youxi.cn

SQL ............ 90
来源：http://haf.bbcook.cn

Bash ........... 80
来源：http://dlb.haohaochexian.top

Kotlin ......... 15
来源：http://tpf.nanxuanxn.top

Swift .......... 15
来源：http://tfy.vqdsnc.cn

Lua ............ 10
来源：http://gpd.meibo888.top

Perl ........... 10
来源：http://asj.bbcook.cn

Scala .......... 10
来源：http://ipo.316326.xyz

------------------------------------
来源：http://cfo.hnqzz.top

合计 ........... 2106 条
来源：http://ifm.aibaodan.cn

按章节统计：
来源：http://har.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vtr.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://awx.tianlin.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ivt.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yio.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dns.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fdc.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gsr.zhixingplan.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hkn.shuidangran.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mtq.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tpd.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ifq.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dfc.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://efg.ppjwa.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gqh.andypj.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xsx.birdmap.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ich.52xcode.cn

Q SQL 专题                              90
来源：http://txk.yuxming.cn

R Bash 专题                             80
来源：http://fiy.c1oappe.top

S C / C++ 专题                          60
来源：http://upv.bbcook.cn

T 其他语言补充                          60
来源：http://egb.pengpengdd.cyou

U 高频实用片段                         120
来源：http://gxj.aibaodan.cn

------------------------------------
来源：http://hmk.fzhhl.top

合计                                  2106 条
来源：http://wsn.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ail.52xcode.cn

使用提醒
来源：http://qnm.sysykeji.top

--------------------------------------------------------------------------------
来源：http://cdx.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nxo.havefunace.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://svc.nanxuanxn.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ylr.aizwys.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nsf.mhx1999.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://huf.aizwys.cn

—— 文件结束 ——
来源：http://zde.dianchejie.cn

================================================================================
来源：http://itf.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://xjz.guowangkeji.top

Common Programming Examples Cheat Book
来源：http://yvq.zdbjq.cn

================================================================================
来源：http://ner.shangyingyoupin.top

【收录内容】
来源：http://utb.fzhhl.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ksa.guannengcc.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ocp.fanxiaobao.xyz

SQL · Bash · C · C++
来源：http://edw.xinyue.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://shu.fktsv.cn

【使用说明】
来源：http://zsc.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ebc.hesvh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lna.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bes.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bku.shuidangran.top

Bash:  Shell         C:     C             C++:   C++
来源：http://asg.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bvr.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ixk.cucudq.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xot.ivvv.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bww.xziqi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pxx.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ajl.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hoq.hcnkem.com

【文件统计】
来源：http://iha.c1oappe.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fpz.fehbvm.com

--------------------------------------------------------------------------------
来源：http://xvl.hammf.cn

目  录
来源：http://kon.guannengcc.top

--------------------------------------------------------------------------------
来源：http://qbr.jqgufenzy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vji.hongshengwenyu.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yjs.xingfuxueyuan.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lot.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zks.0kj1m.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://inl.sjlbkw.cn


<!-- 参考信息 -->