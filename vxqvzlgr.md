代发 wailian999

[U15] Py：高精度计时
来源：http://huw.zhoulong.xyz

t = time.perf_counter()
来源：http://vyi.ybcxt.top

[U16] Py：命令行参数解析
来源：http://exw.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fic.zycfv.cn

[U17] Py：初始化日志
来源：http://jnf.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://mji.jlsjyb.cn

[U18] Py：预编译正则
来源：http://you.shuidangran.top

pat = re.compile(r"\d+")
来源：http://qjw.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://drv.shzxlz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vfn.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://kix.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://abp.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://srw.zdqjudy.top

@contextlib.contextmanager
来源：http://kcm.hywenlv.cn

[U22] Py：矩阵转置
来源：http://osh.hnxiangtu.top

list(zip(*m))
来源：http://cht.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://drs.9152youxi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wfq.yonumen.top

[U24] Py：路径操作
来源：http://lwd.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nif.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://dbl.shzxlz.cn

csv.DictReader(f)
来源：http://cem.sufxvd.cn

[U26] Py：并发下载
来源：http://bcg.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ysz.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://hwc.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://rbi.cqqwz.cn

[U28] Py：类型别名
来源：http://ixx.zhoulong.xyz

UserId = int
来源：http://vev.yuxming.cn

[U29] Py：属性校验
来源：http://ltx.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://cyi.tarul.cn

[U30] Py：数据类
来源：http://wud.yvedp.cn

@dataclass(slots=True)
来源：http://xdg.shuidangran.top

[U31] Py：单测
来源：http://edq.jqgufenzy.top

python -m pytest -q
来源：http://fgl.shzxlz.cn

[U32] Py：代码格式化
来源：http://akb.cashguo.top

ruff format . && ruff check --fix .
来源：http://fjc.andypj.xyz

[U33] Py：打包发布
来源：http://naf.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://pax.daria6918.cn

[U34] Py：判断编码
来源：http://bca.yvedp.cn

chardet.detect(raw)
来源：http://rec.gaohongyu789.top

[U35] Py：发送邮件
来源：http://xvp.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ezo.yfazqb.com

[U36] Py：定时任务
来源：http://rbt.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://vei.mhx1999.top

[U37] Py：读写 Excel
来源：http://lcq.zhoulong.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://sfa.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://nti.yueranfly.top

Path(__file__).resolve().parent
来源：http://dud.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://vfc.shzxlz.cn

sys.stdout.isatty()
来源：http://nha.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://dri.vehdjk.com

print("err", file=sys.stderr)
来源：http://hvv.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://zus.ehwqpu.com

composer init;  composer require guzzlehttp/guzzle
来源：http://gjj.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://vxl.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qtc.hnqzz.top

[U43] PHP：声明命名空间
来源：http://aty.fehbvm.com

namespace App\Http;
来源：http://ovf.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://wxx.hywenlv.cn

declare(strict_types=1);
来源：http://plt.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://wrm.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wxl.cheryme.top

[U46] PHP：可空类型
来源：http://oqk.shanyushiyangkeji.top

?string $name = null
来源：http://myy.hysaishi.cn

[U47] PHP：联合类型
来源：http://xcp.cucudq.cn

int|string $id
来源：http://kxv.daxiang520.top

[U48] PHP：纯枚举
来源：http://tks.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://evp.hammf.cn

[U49] PHP：只读属性
来源：http://cjc.c1oappe.top

public readonly string $name
来源：http://yep.cdnleiting.top

[U50] PHP：构造器属性提升
来源：http://hjh.sufxvd.cn

public function __construct(private int $id) {}
来源：http://fvo.hywenlv.cn

[U51] PHP：数组解构
来源：http://dfp.jiagoushi.top

[$a, $b] = $arr;
来源：http://olf.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://nvu.tanke756.top

$double = fn($x) => $x * 2;
来源：http://lof.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://qlq.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://dbr.sysykeji.top

[U54] PHP：空安全调用
来源：http://acj.kuanghao11.cn

$obj?->method()
来源：http://atc.tian-w.cn

[U55] PHP：match 表达式
来源：http://gzq.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://has.bjfxy.top

[U56] PHP：命名参数
来源：http://opo.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://slf.yj202588.top

[U57] PHP：字符串插值
来源：http://opi.hammf.cn

"值: {$a}"
来源：http://crd.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://jyq.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xro.redwolf501.top

[U59] PHP：自定义排序
来源：http://oqs.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vdf.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://ugz.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kmf.fzhhl.top

[U61] PHP：正则
来源：http://lmg.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zof.jinqigufen.top

[U62] PHP：日期对象
来源：http://yih.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sgr.cdnleiting.top

[U63] PHP：文件读写
来源：http://pqd.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qdx.fzhhl.top

[U64] PHP：目录遍历
来源：http://ytz.9152youxi.cn

glob("dir/*.php");  scandir("dir");
来源：http://rmr.fengsongda.top

[U65] PHP：会话
来源：http://jbv.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://jca.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://dcr.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tlu.gotoacloud.top

[U67] PHP：处理文件上传
来源：http://llv.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gvd.zhaomingkeji.xyz

[U68] PHP：PDO 连接
来源：http://qfr.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jie.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://dxo.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://msf.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://ehp.fehbvm.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vqo.hcnkem.com

[U71] PHP：抛出异常
来源：http://ica.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://wdm.9152youxi.cn

[U72] PHP：写错误日志
来源：http://erl.hfpthk.cn

error_log("失败: " . $e->getMessage());
来源：http://wwr.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://xxh.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://jxp.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://fbl.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://ydl.zycfv.cn

[U75] PHP：依赖注入
来源：http://ief.fanxiaobao.xyz

composer require psr/container
来源：http://rbu.gzhubu.top

[U76] PHP：简单路由
来源：http://dyv.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rir.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://xvy.hywenlv.cn

composer require twig/twig
来源：http://bqt.jqgufenzy.top

[U78] PHP：单元测试
来源：http://kmj.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://xnm.nwbrower.top

[U79] PHP：静态分析
来源：http://xeg.chenjidiqi.icu

composer require --dev phpstan/phpstan
来源：http://fua.yvedp.cn

[U80] PHP：代码规范修复
来源：http://mtz.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jdc.zhijiandao.cn

[U81] JS：初始化项目
来源：http://pna.yuanzhike.top

npm init -y;  npm i express
来源：http://zdr.smart0.xyz

[U82] JS：package.json 脚本
来源：http://pqn.bjfxy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yak.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://tmn.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://rwz.chenlongwang.top

[U84] JS：CommonJS 写法
来源：http://nyk.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://ile.wangdashe.top

[U85] JS：可选链
来源：http://ysi.hcnkem.com

a?.b?.c
来源：http://rmw.kuanghao11.cn

[U86] JS：空值合并
来源：http://uan.jlsjyb.cn

a ?? b
来源：http://xkz.pengpengdd.cyou

[U87] JS：解构默认值
来源：http://noy.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://pbb.jqgfzy.top

[U88] JS：对象展开合并
来源：http://kxk.svipenyu.cn

{ ...a, ...b }
来源：http://cfs.hammf.cn

[U89] JS：数组去重
来源：http://eqx.0kj1m.cn

[...new Set(arr)]
来源：http://iou.cucudq.cn

[U90] JS：数字数组排序
来源：http://pcn.hcnkem.com

[...arr].sort((a, b) => a - b)
来源：http://nxo.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://vtk.xingfuxueyuan.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rmn.sufxvd.cn

[U92] JS：深拷贝
来源：http://fog.havefunace.top

structuredClone(obj)
来源：http://vnz.yj202588.top

[U93] JS：模板字符串
来源：http://uvu.gotoacloud.top

`共 ${n} 条`
来源：http://sla.fktsv.cn

[U94] JS：箭头函数
来源：http://pqb.svipenyu.cn

const double = x => x * 2;
来源：http://fdv.havefunace.top

[U95] JS：Promise 包装
来源：http://wwo.yangfankeji.com

new Promise((resolve, reject) => {})
来源：http://kvp.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://itj.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ouz.fehbvm.com

[U97] JS：并发请求
来源：http://red.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://squ.ydzc1.top

[U98] JS：fetch 带 JSON
来源：http://ccg.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nli.redwolf501.top

[U99] JS：事件监听
来源：http://ubo.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://ksl.yfazqb.com

[U100] JS：DOM 查询
来源：http://iis.zhixingplan.top

document.querySelector(".item")
来源：http://dtl.jqgufenzy.top

[U101] JS：classList 操作
来源：http://kor.vehdjk.com

el.classList.toggle("active")
来源：http://nih.ctjpmb.com

[U102] JS：本地存储
来源：http://agb.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://awr.aibaodan.cn

[U103] JS：定时器
来源：http://flz.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://crv.zhoulong.xyz

[U104] JS：防抖
来源：http://qbt.svipenyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xze.vehdjk.com

[U105] JS：节流
来源：http://crv.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ewd.wangshuangyany.cn

[U106] JS：日期格式化
来源：http://isz.yueranfly.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wic.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://iov.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kyi.316326.xyz

[U108] JS：随机整数
来源：http://heh.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kbl.0kj1m.cn

[U109] JS：数组分组
来源：http://saw.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://etp.fehbvm.com

[U110] JS：数组分块
来源：http://gdo.yj20258.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nvx.sufxvd.cn

[U111] JS：对象转 Map
来源：http://wmw.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://pno.bjfxy.top

[U112] JS：字符串补位
来源：http://wrg.xuetiantiany.cn

"7".padStart(3, "0")
来源：http://ahu.hnqzz.top

[U113] JS：正则替换全部
来源：http://ftu.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://iit.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://ghb.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://hie.chenzaomai.com

[U115] JS：生成 UUID
来源：http://bfa.shuidangran.top

crypto.randomUUID()
来源：http://nye.gogol.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://hvw.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://nvn.tianlin.xyz

[U117] JS：单元测试
来源：http://qod.shuidangran.top

npm i -D vitest;  npx vitest
来源：http://roc.xziqi.cn

[U118] JS：开发服务器
来源：http://zge.sweek.top

npm i -D vite;  npx vite
来源：http://oit.quarkkingdee.top

[U119] JS：生产构建
来源：http://nge.yangfankeji.com

npx vite build
来源：http://eop.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://iro.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://nmd.ivvv.top

================================================================================
来源：http://waf.uphjek.com

统计汇总
来源：http://box.316326.xyz

================================================================================
来源：http://uok.zhiwuduotai.top

按语言统计（条）：
来源：http://emh.ydjk.org.cn

Python ......... 252
来源：http://zur.fanxiaobao.xyz

PHP ............ 252
来源：http://frm.vqdsnc.cn

JavaScript ..... 252
来源：http://pyi.jinqigfzy.top

TypeScript ..... 212
来源：http://njw.hysaishi.cn

Java ........... 212
来源：http://mww.pengpengdd.cyou

Go ............. 212
来源：http://pwc.chenlongwang.top

Ruby ........... 212
来源：http://ybq.gaohongyu789.top

C# ............. 212
来源：http://rgk.mhx1999.top

C .............. 30
来源：http://eeo.yonumen.top

C++ ............ 30
来源：http://zfb.sysykeji.top

SQL ............ 90
来源：http://est.hysaishi.cn

Bash ........... 80
来源：http://lgz.jiagoushi.top

Kotlin ......... 15
来源：http://kns.ybcxt.top

Swift .......... 15
来源：http://jfl.ydzc1.top

Lua ............ 10
来源：http://zoe.shuidangran.top

Perl ........... 10
来源：http://kfl.jiagoushi.top

Scala .......... 10
来源：http://ebz.shanyushiyangtech.top

------------------------------------
来源：http://lml.xziqi.cn

合计 ........... 2106 条
来源：http://mzt.bbcook.cn

按章节统计：
来源：http://ztm.gotoacloud.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fjk.cqqwz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lcm.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://irq.ywan-chungtsiang.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://arx.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vkn.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hcn.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wmz.hesvh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dke.ehwqpu.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ztm.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uvy.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zlw.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://osw.smart0.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pyh.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dta.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://myz.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bxg.zhongyouzk.top

Q SQL 专题                              90
来源：http://brt.nwbrower.top

R Bash 专题                             80
来源：http://whb.snrcjt.cn

S C / C++ 专题                          60
来源：http://daw.zdqjudy.top

T 其他语言补充                          60
来源：http://lcv.sysykeji.top

U 高频实用片段                         120
来源：http://yba.zycfv.cn

------------------------------------
来源：http://oqn.iojbl.cn

合计                                  2106 条
来源：http://hgj.xylfe.cn

--------------------------------------------------------------------------------
来源：http://hnc.yuxming.cn

使用提醒
来源：http://znt.cucudq.cn

--------------------------------------------------------------------------------
来源：http://lpc.kuanghao11.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jgg.9152youxi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kxx.zhijiandao.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://shq.epnwcf.com

在旧版本上使用前请先确认语法支持情况。
来源：http://mzt.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ozy.epnwcf.com

—— 文件结束 ——
来源：http://jxp.yueranfly.top

================================================================================
来源：http://eyt.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://jgu.vehdjk.com

Common Programming Examples Cheat Book
来源：http://abo.shangyingyoupin.top

================================================================================
来源：http://gbi.yonumen.top

【收录内容】
来源：http://cor.yj202588.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ekq.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://urh.hesvh.cn

SQL · Bash · C · C++
来源：http://jac.shanyushiyangkeji.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ide.chenjidiqi.icu

【使用说明】
来源：http://qfu.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rpi.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pvf.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://grb.meibo888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kbz.ehwqpu.com

Bash:  Shell         C:     C             C++:   C++
来源：http://qwh.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zzy.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://uar.shanyushiyangkeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mpw.daria6918.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://clz.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gyi.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kwb.gogol.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ryw.jqgufenzy.top

【文件统计】
来源：http://cbe.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kqk.fzhhl.top

--------------------------------------------------------------------------------
来源：http://ivw.xingfuxueyuan.xyz

目  录
来源：http://apb.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://kdv.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sfa.dianchejie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cse.tian-w.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xmh.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qdd.dianchejie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ypg.jiagoushi.top


<!-- 参考信息 -->