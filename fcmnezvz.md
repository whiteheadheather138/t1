代发 wailian999

[U11] Py：生成器表达式
来源：http://ygc.gotoacloud.top

(x * 2 for x in arr)
来源：http://cea.wangshuangyany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fog.yueranfly.top

Counter(arr).most_common(3)
来源：http://wrc.jinghuilouyu.cn

[U13] Py：固定长度队列
来源：http://fuz.yj20258.top

deque(maxlen=10)
来源：http://tgq.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://ckp.tian-w.cn

defaultdict(list)
来源：http://xhs.hammf.cn

[U15] Py：高精度计时
来源：http://bjm.pengpengdd.cyou

t = time.perf_counter()
来源：http://bad.aizwys.cn

[U16] Py：命令行参数解析
来源：http://wxl.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zet.snrcjt.cn

[U17] Py：初始化日志
来源：http://gwj.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ito.ctjpmb.com

[U18] Py：预编译正则
来源：http://cdo.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://qsg.iojbl.cn

[U19] Py：正则替换带回调
来源：http://occ.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ugt.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://zvg.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://gbg.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://ryl.gotoacloud.top

@contextlib.contextmanager
来源：http://msh.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://xhl.sufxvd.cn

list(zip(*m))
来源：http://svo.yj202588.top

[U23] Py：分块读取大文件
来源：http://yle.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ilf.fengsongda.top

[U24] Py：路径操作
来源：http://ovg.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ndh.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://sja.zycfv.cn

csv.DictReader(f)
来源：http://uji.yangfankeji.com

[U26] Py：并发下载
来源：http://pvz.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ngc.zhoulong.xyz

[U27] Py：异步 HTTP
来源：http://zvn.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://som.wangdashe.top

[U28] Py：类型别名
来源：http://jzx.birdmap.top

UserId = int
来源：http://axz.daria6918.cn

[U29] Py：属性校验
来源：http://qek.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://ond.yvedp.cn

[U30] Py：数据类
来源：http://lqu.haohaochexian.top

@dataclass(slots=True)
来源：http://ofp.zhiwuduotai.top

[U31] Py：单测
来源：http://lcc.xziqi.cn

python -m pytest -q
来源：http://tmo.hfpthk.cn

[U32] Py：代码格式化
来源：http://qxg.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://qhd.jlsjyb.cn

[U33] Py：打包发布
来源：http://kkj.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://zuy.jlsjyb.cn

[U34] Py：判断编码
来源：http://kpc.fzhhl.top

chardet.detect(raw)
来源：http://von.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://odp.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hgc.jinqigfzy.top

[U36] Py：定时任务
来源：http://jlj.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://huq.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://hby.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://evc.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://nfi.iojbl.cn

Path(__file__).resolve().parent
来源：http://qjs.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://okj.yongpay.top

sys.stdout.isatty()
来源：http://hwa.shanyushiyangkeji.top

[U40] Py：打印到标准错误
来源：http://xue.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://fsu.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://kbr.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wkn.nanxuanxn.top

[U42] PHP：PSR-4 自动加载
来源：http://qnb.zdqjudy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sox.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://qei.zhongyouzk.top

namespace App\Http;
来源：http://ilq.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://jrw.nanxinkj.top

declare(strict_types=1);
来源：http://zjm.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://tsa.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yde.tianlin.xyz

[U46] PHP：可空类型
来源：http://szs.hammf.cn

?string $name = null
来源：http://wep.daria6918.cn

[U47] PHP：联合类型
来源：http://xoc.cucudq.cn

int|string $id
来源：http://apc.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://mul.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jvg.quarkkingdee.top

[U49] PHP：只读属性
来源：http://xvx.yuanzhike.top

public readonly string $name
来源：http://ewb.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://acv.yangfankeji.com

public function __construct(private int $id) {}
来源：http://gkg.sweek.top

[U51] PHP：数组解构
来源：http://cts.mhx1999.top

[$a, $b] = $arr;
来源：http://hon.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://dwk.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://mdc.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://ypx.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://zhi.jinqigufen.top

[U54] PHP：空安全调用
来源：http://lmo.iojbl.cn

$obj?->method()
来源：http://ipa.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://cac.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xej.zhaomingkeji.xyz

[U56] PHP：命名参数
来源：http://byh.gotoacloud.top

f(a: 1, b: 2)
来源：http://mot.zdbjq.cn

[U57] PHP：字符串插值
来源：http://gny.fktsv.cn

"值: {$a}"
来源：http://aby.shanyushiyangkeji.top

[U58] PHP：数组三件套
来源：http://aez.guannengcc.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ywx.ivvv.top

[U59] PHP：自定义排序
来源：http://sip.daxiang520.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nhf.sufxvd.cn

[U60] PHP：JSON 编解码
来源：http://nlp.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nrl.smart0.xyz

[U61] PHP：正则
来源：http://cnz.hammf.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://isv.guannengcc.top

[U62] PHP：日期对象
来源：http://owh.hongshengwenyu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gol.yvedp.cn

[U63] PHP：文件读写
来源：http://kyp.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xpi.meibo888.top

[U64] PHP：目录遍历
来源：http://tkj.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://fej.smart0.xyz

[U65] PHP：会话
来源：http://pcu.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qjx.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://bre.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://evf.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://jpe.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://erd.zhengqikj.top

[U68] PHP：PDO 连接
来源：http://exn.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yab.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://gcv.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hoo.xylfe.cn

[U70] PHP：PDO 事务
来源：http://saz.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wnp.ehwqpu.com

[U71] PHP：抛出异常
来源：http://kue.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://jkk.ydzc1.top

[U72] PHP：写错误日志
来源：http://dgp.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://ams.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://avo.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://ugc.zdqjudy.top

[U74] PHP：读取环境变量
来源：http://swl.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://vwx.bbcook.cn

[U75] PHP：依赖注入
来源：http://kte.hywenlv.cn

composer require psr/container
来源：http://rml.cqqwz.cn

[U76] PHP：简单路由
来源：http://fuy.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vvh.fzhhl.top

[U77] PHP：模板渲染
来源：http://qwe.ehwqpu.com

composer require twig/twig
来源：http://izy.chenjidiqi.icu

[U78] PHP：单元测试
来源：http://dvc.meibo888.top

composer require --dev phpunit/phpunit
来源：http://tgs.jqgufenzy.top

[U79] PHP：静态分析
来源：http://nhf.havefunace.top

composer require --dev phpstan/phpstan
来源：http://ptm.pycfn.com

[U80] PHP：代码规范修复
来源：http://cqf.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdo.hywenlv.cn

[U81] JS：初始化项目
来源：http://paj.daria6918.cn

npm init -y;  npm i express
来源：http://lcj.vehdjk.com

[U82] JS：package.json 脚本
来源：http://gfe.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vxl.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://zlz.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jch.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://mjv.daxiang520.top

module.exports = { a };  const { a } = require("./m");
来源：http://tbh.jinyuanbaomall.cn

[U85] JS：可选链
来源：http://owu.fanxiaobao.xyz

a?.b?.c
来源：http://hri.guannengcc.top

[U86] JS：空值合并
来源：http://rke.zhoulong.xyz

a ?? b
来源：http://mrr.daria6918.cn

[U87] JS：解构默认值
来源：http://xwp.hysaishi.cn

const { a = 1, b = 2 } = obj;
来源：http://jhe.zycfv.cn

[U88] JS：对象展开合并
来源：http://bjw.gzhubu.top

{ ...a, ...b }
来源：http://esu.ppjwa.cn

[U89] JS：数组去重
来源：http://flc.cashguo.top

[...new Set(arr)]
来源：http://ory.ybcxt.top

[U90] JS：数字数组排序
来源：http://mmc.dashuyun.cn

[...arr].sort((a, b) => a - b)
来源：http://vpq.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://cvr.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ear.jqgfzy.top

[U92] JS：深拷贝
来源：http://aml.daxiang520.top

structuredClone(obj)
来源：http://yll.birdmap.top

[U93] JS：模板字符串
来源：http://zfs.feifeiyinyue.top

`共 ${n} 条`
来源：http://fza.cheryme.top

[U94] JS：箭头函数
来源：http://zzt.bjfxy.top

const double = x => x * 2;
来源：http://izb.fzhhl.top

[U95] JS：Promise 包装
来源：http://oaz.xingfuxueyuan.xyz

new Promise((resolve, reject) => {})
来源：http://tps.guannengcc.top

[U96] JS：async/await 与异常
来源：http://ccr.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fpx.ivvv.top

[U97] JS：并发请求
来源：http://zyu.ydjk.org.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dwq.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://cwz.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dkq.fengsongda.top

[U99] JS：事件监听
来源：http://euq.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://hwb.yonumen.top

[U100] JS：DOM 查询
来源：http://fnb.yueranfly.top

document.querySelector(".item")
来源：http://ggc.chenzaomai.com

[U101] JS：classList 操作
来源：http://rex.yfazqb.com

el.classList.toggle("active")
来源：http://wod.yj20258888.top

[U102] JS：本地存储
来源：http://fxu.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://var.yuxming.cn

[U103] JS：定时器
来源：http://nzd.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ywg.uphjek.com

[U104] JS：防抖
来源：http://lxk.zhengqikj.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ilp.vehdjk.com

[U105] JS：节流
来源：http://qdo.ydzc1.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sea.quarkkingdee.top

[U106] JS：日期格式化
来源：http://rha.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hqr.gaohongyu789.top

[U107] JS：数字千分位
来源：http://dbg.hnqzz.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sit.wangdashe.top

[U108] JS：随机整数
来源：http://ust.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uxh.fengsongda.top

[U109] JS：数组分组
来源：http://zfm.zhaomingkeji.xyz

Object.groupBy(arr, x => x.type)
来源：http://uhk.jqgufenzy.top

[U110] JS：数组分块
来源：http://imz.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cfr.cdnleiting.top

[U111] JS：对象转 Map
来源：http://pyn.nwbrower.top

new Map(Object.entries(obj))
来源：http://jlg.uphjek.com

[U112] JS：字符串补位
来源：http://geu.jlsjyb.cn

"7".padStart(3, "0")
来源：http://ikx.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://djt.sxryk.cn

s.replaceAll("a", "b")
来源：http://nof.52xcode.cn

[U114] JS：JSON 深比较
来源：http://sus.fanxiaobao.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://rkt.epnwcf.com

[U115] JS：生成 UUID
来源：http://msn.bbcook.cn

crypto.randomUUID()
来源：http://xhq.ppjwa.cn

[U116] JS：类型检查（JSDoc）
来源：http://drj.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://quv.chenzaomai.com

[U117] JS：单元测试
来源：http://tld.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://grn.snrcjt.cn

[U118] JS：开发服务器
来源：http://zzi.smart0.xyz

npm i -D vite;  npx vite
来源：http://qvj.wangshuangyany.cn

[U119] JS：生产构建
来源：http://hep.xingfuxueyuan.xyz

npx vite build
来源：http://exz.jiagoushi.top

[U120] JS：读取环境变量（Vite）
来源：http://uom.9152youxi.cn

import.meta.env.VITE_API_URL
来源：http://ytx.ybcxt.top

================================================================================
来源：http://xvo.fzhhl.top

统计汇总
来源：http://ofa.c1oappe.top

================================================================================
来源：http://zfl.ehwqpu.com

按语言统计（条）：
来源：http://hnv.fanxiaobao.xyz

Python ......... 252
来源：http://ozj.ybcxt.top

PHP ............ 252
来源：http://ddr.quarkkingdee.top

JavaScript ..... 252
来源：http://vgb.dianchejie.cn

TypeScript ..... 212
来源：http://pgi.redwolf501.top

Java ........... 212
来源：http://ijw.aizwys.cn

Go ............. 212
来源：http://tsw.zhaomingkeji.xyz

Ruby ........... 212
来源：http://mmn.wangdashe.top

C# ............. 212
来源：http://bal.hywenlv.cn

C .............. 30
来源：http://gzh.yueranfly.top

C++ ............ 30
来源：http://ghz.quarkkingdee.top

SQL ............ 90
来源：http://fdi.jlsjyb.cn

Bash ........... 80
来源：http://imh.ybcxt.top

Kotlin ......... 15
来源：http://aro.xylfe.cn

Swift .......... 15
来源：http://ttf.hongshengwenyu.top

Lua ............ 10
来源：http://adt.fzhhl.top

Perl ........... 10
来源：http://gtg.yangfankeji.com

Scala .......... 10
来源：http://cgf.cheryme.top

------------------------------------
来源：http://zho.hnxiangtu.top

合计 ........... 2106 条
来源：http://eeu.nwbrower.top

按章节统计：
来源：http://kaz.xuetiantiany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wbr.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://twy.zhijiandao.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xtl.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vpj.wangdashe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xhd.tian-w.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tol.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qal.shanyushiyangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rul.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fuh.xziqi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hrp.sufxvd.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gll.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hni.hammf.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kpz.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mjq.xinyue.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://muj.shuidangran.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wqa.sxryk.cn

Q SQL 专题                              90
来源：http://iov.meibo888.top

R Bash 专题                             80
来源：http://lhr.aizwys.cn

S C / C++ 专题                          60
来源：http://omo.snrcjt.cn

T 其他语言补充                          60
来源：http://lps.zdqjudy.top

U 高频实用片段                         120
来源：http://pwo.yj20258888.top

------------------------------------
来源：http://hxe.jyoumei.cn

合计                                  2106 条
来源：http://yqo.smart0.xyz

--------------------------------------------------------------------------------
来源：http://hte.feifeiyinyue.top

使用提醒
来源：http://plx.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://aqf.gaohongyu789.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xkp.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yek.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fhe.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://nsf.hnxiangtu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cwo.hammf.cn

—— 文件结束 ——
来源：http://ups.bbcook.cn

================================================================================
来源：http://ntt.hcnkem.com

程序语言常见例子速查手册（2024 版）
来源：http://nya.fktsv.cn

Common Programming Examples Cheat Book
来源：http://mpk.feifeiyinyue.top

================================================================================
来源：http://neo.zycfv.cn

【收录内容】
来源：http://jtk.aizwys.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://iwn.guowangkeji.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hiw.fzhhl.top

SQL · Bash · C · C++
来源：http://vmt.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eyp.guowangkeji.top

【使用说明】
来源：http://whq.yanxiufei.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ieb.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://exq.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qic.haohaochexian.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ilq.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yda.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pnb.yfazqb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://klc.meibo888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hba.jyoumei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wxd.ppjwa.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vbu.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ahw.fanxiaobao.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ggr.hesvh.cn

【文件统计】
来源：http://rub.chenlongwang.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hdm.zhongyouzk.top


<!-- 参考信息 -->