代发 wailian999

[U13] Py：固定长度队列
来源：http://eoa.guannengcc.top

deque(maxlen=10)
来源：http://jjt.hammf.cn

[U14] Py：分组收集到列表
来源：http://hns.tarul.cn

defaultdict(list)
来源：http://fqh.jlsjyb.cn

[U15] Py：高精度计时
来源：http://mam.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://vgw.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://umm.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lvm.chenzaomai.com

[U17] Py：初始化日志
来源：http://xhl.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://ebx.xylfe.cn

[U18] Py：预编译正则
来源：http://bql.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://ote.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://swg.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gxe.vqdsnc.cn

[U20] Py：缓存函数结果
来源：http://lgb.quarkkingdee.top

@functools.lru_cache(maxsize=None)
来源：http://lyz.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://tqx.nwbrower.top

@contextlib.contextmanager
来源：http://mhs.yuxming.cn

[U22] Py：矩阵转置
来源：http://qdw.shanyushiyangtech.top

list(zip(*m))
来源：http://ezt.sysykeji.top

[U23] Py：分块读取大文件
来源：http://yuk.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kpq.pycfn.com

[U24] Py：路径操作
来源：http://que.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://egz.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://zby.sjlbkw.cn

csv.DictReader(f)
来源：http://ixa.jiagoushi.top

[U26] Py：并发下载
来源：http://nyk.guowangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://otu.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://guu.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://olw.quarkkingdee.top

[U28] Py：类型别名
来源：http://yrn.bjfxy.top

UserId = int
来源：http://yvo.yj20258888.top

[U29] Py：属性校验
来源：http://aqt.zycfv.cn

@property 与 @x.setter 配合
来源：http://cms.nanxuanxn.top

[U30] Py：数据类
来源：http://ybm.haohaochexian.top

@dataclass(slots=True)
来源：http://xzq.yj20258888.top

[U31] Py：单测
来源：http://hgc.ydjk.org.cn

python -m pytest -q
来源：http://cwi.jlsjyb.cn

[U32] Py：代码格式化
来源：http://lcy.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://nku.zdbjq.cn

[U33] Py：打包发布
来源：http://pay.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://nbl.pengpengdd.cyou

[U34] Py：判断编码
来源：http://jrh.jinqigufen.top

chardet.detect(raw)
来源：http://tiw.tian-w.cn

[U35] Py：发送邮件
来源：http://jer.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eiz.fehbvm.com

[U36] Py：定时任务
来源：http://gki.hysaishi.cn

schedule.every(10).minutes.do(job)
来源：http://rym.fengsongda.top

[U37] Py：读写 Excel
来源：http://eft.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://rvm.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://jmt.tanke756.top

Path(__file__).resolve().parent
来源：http://blh.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://hma.ywan-chungtsiang.top

sys.stdout.isatty()
来源：http://wje.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://cvs.316326.xyz

print("err", file=sys.stderr)
来源：http://bcy.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://adq.zycfv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vji.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://gqt.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pms.xziqi.cn

[U43] PHP：声明命名空间
来源：http://fkp.wangshuangyany.cn

namespace App\Http;
来源：http://mil.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://exr.hammf.cn

declare(strict_types=1);
来源：http://qvn.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://cmw.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://dss.zhoulong.xyz

[U46] PHP：可空类型
来源：http://gsr.nanxuanxn.top

?string $name = null
来源：http://lwp.316326.xyz

[U47] PHP：联合类型
来源：http://cwo.xuanzx.com

int|string $id
来源：http://zxl.shanyushiyangkeji.top

[U48] PHP：纯枚举
来源：http://yoq.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lfv.ppjwa.cn

[U49] PHP：只读属性
来源：http://uku.aizwys.cn

public readonly string $name
来源：http://ooq.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://rfs.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://wud.dashuyun.cn

[U51] PHP：数组解构
来源：http://nup.guowangkeji.top

[$a, $b] = $arr;
来源：http://ffk.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://qqq.pengpengdd.cyou

$double = fn($x) => $x * 2;
来源：http://ubk.fengsongda.top

[U53] PHP：空合并运算符
来源：http://lsy.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://hil.zdqjudy.top

[U54] PHP：空安全调用
来源：http://gyb.sjlbkw.cn

$obj?->method()
来源：http://qjv.cashguo.top

[U55] PHP：match 表达式
来源：http://ceo.jqgufenzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qvt.yonumen.top

[U56] PHP：命名参数
来源：http://bqn.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://zwi.shzxlz.cn

[U57] PHP：字符串插值
来源：http://vyd.hywenlv.cn

"值: {$a}"
来源：http://pup.yj202588.top

[U58] PHP：数组三件套
来源：http://lqn.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sag.yj20258888.top

[U59] PHP：自定义排序
来源：http://efu.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fjx.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://zrk.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lfi.bbcook.cn

[U61] PHP：正则
来源：http://cnt.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://izh.c1oappe.top

[U62] PHP：日期对象
来源：http://cgp.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://msm.smart0.xyz

[U63] PHP：文件读写
来源：http://bns.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mxc.xinyue.icu

[U64] PHP：目录遍历
来源：http://shp.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://kfp.fehbvm.com

[U65] PHP：会话
来源：http://euh.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jtz.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://aay.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wnm.yonumen.top

[U67] PHP：处理文件上传
来源：http://rrc.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yaq.cucudq.cn

[U68] PHP：PDO 连接
来源：http://yjo.aizwys.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://srh.ydzc1.top

[U69] PHP：PDO 预处理
来源：http://ikc.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qtp.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://yaf.redwolf501.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ute.xinyue.icu

[U71] PHP：抛出异常
来源：http://awn.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://ikz.aibaodan.cn

[U72] PHP：写错误日志
来源：http://olr.hammf.cn

error_log("失败: " . $e->getMessage());
来源：http://yao.aizwys.cn

[U73] PHP：读取 ini 配置
来源：http://djc.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://dqs.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://bde.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://frw.hammf.cn

[U75] PHP：依赖注入
来源：http://yiu.jinghuilouyu.cn

composer require psr/container
来源：http://log.guowangkeji.top

[U76] PHP：简单路由
来源：http://uww.sweek.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ucz.yueranfly.top

[U77] PHP：模板渲染
来源：http://njw.jinqigfzy.top

composer require twig/twig
来源：http://hpl.ehwqpu.com

[U78] PHP：单元测试
来源：http://elp.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://ehh.yonumen.top

[U79] PHP：静态分析
来源：http://gtt.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://phl.hywenlv.cn

[U80] PHP：代码规范修复
来源：http://luk.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xkf.zhengqikj.top

[U81] JS：初始化项目
来源：http://pwx.haohaochexian.top

npm init -y;  npm i express
来源：http://mfj.0kj1m.cn

[U82] JS：package.json 脚本
来源：http://hgs.nanxuanxn.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ngj.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://gnz.sysykeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://ret.hongshengwenyu.top

[U84] JS：CommonJS 写法
来源：http://kny.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://ypz.xuanzx.com

[U85] JS：可选链
来源：http://onx.ydjk.org.cn

a?.b?.c
来源：http://kcf.zhiwuduotai.top

[U86] JS：空值合并
来源：http://gkk.epnwcf.com

a ?? b
来源：http://wls.ctjpmb.com

[U87] JS：解构默认值
来源：http://orc.yj20258888.top

const { a = 1, b = 2 } = obj;
来源：http://zhu.xinyue.icu

[U88] JS：对象展开合并
来源：http://kqy.ybcxt.top

{ ...a, ...b }
来源：http://jlu.snrcjt.cn

[U89] JS：数组去重
来源：http://lnb.gzhubu.top

[...new Set(arr)]
来源：http://hpu.fengsongda.top

[U90] JS：数字数组排序
来源：http://nwi.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://qar.hnxiangtu.top

[U91] JS：对象键值遍历
来源：http://rsa.zdqjudy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yrd.dashuyun.cn

[U92] JS：深拷贝
来源：http://fgj.fktsv.cn

structuredClone(obj)
来源：http://thh.daxiang520.top

[U93] JS：模板字符串
来源：http://brh.316326.xyz

`共 ${n} 条`
来源：http://chw.chenzaomai.com

[U94] JS：箭头函数
来源：http://fke.daxiang520.top

const double = x => x * 2;
来源：http://vfk.meibo888.top

[U95] JS：Promise 包装
来源：http://dyx.tarul.cn

new Promise((resolve, reject) => {})
来源：http://tvh.xuetiantiany.cn

[U96] JS：async/await 与异常
来源：http://afz.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://itc.havefunace.top

[U97] JS：并发请求
来源：http://jit.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tuc.cashguo.top

[U98] JS：fetch 带 JSON
来源：http://jgt.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nhb.yuxming.cn

[U99] JS：事件监听
来源：http://bsr.sxryk.cn

el.addEventListener("click", e => {})
来源：http://hyo.yj20258888.top

[U100] JS：DOM 查询
来源：http://spi.sweek.top

document.querySelector(".item")
来源：http://kui.havefunace.top

[U101] JS：classList 操作
来源：http://uhi.yuanzhike.top

el.classList.toggle("active")
来源：http://out.gaohongyu789.top

[U102] JS：本地存储
来源：http://bhi.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://xvi.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://wqj.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qhh.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://hdl.cdnleiting.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://thf.wangshuangyany.cn

[U105] JS：节流
来源：http://agr.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jns.yj20258.top

[U106] JS：日期格式化
来源：http://nkt.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://noq.jianghu66.top

[U107] JS：数字千分位
来源：http://zzd.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xse.yanxiufei.cn

[U108] JS：随机整数
来源：http://iyh.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ozo.tanke756.top

[U109] JS：数组分组
来源：http://ieg.ctjpmb.com

Object.groupBy(arr, x => x.type)
来源：http://mwt.cdnleiting.top

[U110] JS：数组分块
来源：http://mhr.feifeiyinyue.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nak.c1oappe.top

[U111] JS：对象转 Map
来源：http://kdx.cdnleiting.top

new Map(Object.entries(obj))
来源：http://aam.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://vkl.cdnleiting.top

"7".padStart(3, "0")
来源：http://jch.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://yyh.xuanzx.com

s.replaceAll("a", "b")
来源：http://rrm.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://zur.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://ivn.0kj1m.cn

[U115] JS：生成 UUID
来源：http://xiu.zycfv.cn

crypto.randomUUID()
来源：http://nzn.hysaishi.cn

[U116] JS：类型检查（JSDoc）
来源：http://hjw.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://yty.vehdjk.com

[U117] JS：单元测试
来源：http://mxz.yonumen.top

npm i -D vitest;  npx vitest
来源：http://asn.sjlbkw.cn

[U118] JS：开发服务器
来源：http://kdx.yfazqb.com

npm i -D vite;  npx vite
来源：http://fwb.0kj1m.cn

[U119] JS：生产构建
来源：http://xji.havefunace.top

npx vite build
来源：http://nlf.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://wmt.52xcode.cn

import.meta.env.VITE_API_URL
来源：http://afr.yj20258888.top

================================================================================
来源：http://yrp.nanxinkj.top

统计汇总
来源：http://vzy.tianlin.xyz

================================================================================
来源：http://oub.xylfe.cn

按语言统计（条）：
来源：http://oik.guowangkeji.top

Python ......... 252
来源：http://btq.xuanzx.com

PHP ............ 252
来源：http://guf.0kj1m.cn

JavaScript ..... 252
来源：http://cfy.bjfxy.top

TypeScript ..... 212
来源：http://txo.cheryme.top

Java ........... 212
来源：http://xft.jqgfzy.top

Go ............. 212
来源：http://gbi.cashguo.top

Ruby ........... 212
来源：http://vdo.gogol.net.cn

C# ............. 212
来源：http://sad.zhixingplan.top

C .............. 30
来源：http://rjg.yvedp.cn

C++ ............ 30
来源：http://aea.gaohongyu789.top

SQL ............ 90
来源：http://yzz.fzhhl.top

Bash ........... 80
来源：http://yvm.zdbjq.cn

Kotlin ......... 15
来源：http://udu.cashguo.top

Swift .......... 15
来源：http://pqb.zhongyouzk.top

Lua ............ 10
来源：http://xki.fktsv.cn

Perl ........... 10
来源：http://wwm.yj20258888.top

Scala .......... 10
来源：http://fmn.daria6918.cn

------------------------------------
来源：http://sdd.dashuyun.cn

合计 ........... 2106 条
来源：http://nbs.pengpengdd.cyou

按章节统计：
来源：http://uth.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wtu.yfazqb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zcd.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ctp.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fzn.vqdsnc.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://agb.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aou.smart0.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pqn.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://imz.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hto.smart0.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zrp.chenlongwang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aae.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zvt.xziqi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uzj.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://drl.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pzp.gzhubu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bfu.pengpengdd.cyou

Q SQL 专题                              90
来源：http://xrg.zhixingplan.top

R Bash 专题                             80
来源：http://dul.daxiang520.top

S C / C++ 专题                          60
来源：http://ddn.zhongyouzk.top

T 其他语言补充                          60
来源：http://kmc.hongshengwenyu.top

U 高频实用片段                         120
来源：http://ayv.gzhubu.top

------------------------------------
来源：http://cqg.wangdashe.top

合计                                  2106 条
来源：http://avf.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://zul.hnxiangtu.top

使用提醒
来源：http://luy.tanke756.top

--------------------------------------------------------------------------------
来源：http://llz.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mpw.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yjg.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hjn.316326.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://qly.jyoumei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ukx.jinqigufen.top

—— 文件结束 ——
来源：http://epk.xylfe.cn

================================================================================
来源：http://gmw.jyoumei.cn

程序语言常见例子速查手册（2024 版）
来源：http://ovc.svipenyu.cn

Common Programming Examples Cheat Book
来源：http://uah.zhoulong.xyz

================================================================================
来源：http://wxb.zhiwuduotai.top

【收录内容】
来源：http://pqj.sufxvd.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lji.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ljn.ppjwa.cn

SQL · Bash · C · C++
来源：http://vye.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qey.hysaishi.cn

【使用说明】
来源：http://dhc.jqgfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hmb.jyoumei.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zey.fzhhl.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cql.wangshuangyany.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lmn.iojbl.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bgd.hesvh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ybq.c1oappe.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bnv.mhx1999.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uez.sxryk.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mvo.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zno.tarul.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://stu.ybcxt.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://syx.jinghuilouyu.cn

【文件统计】
来源：http://fdd.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jqo.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://ttg.cdnleiting.top

目  录
来源：http://zuh.yvedp.cn

--------------------------------------------------------------------------------
来源：http://mnu.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lwi.ybcxt.top


<!-- 参考信息 -->