代发 wailian999

[U17] Py：初始化日志
来源：http://dez.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://vrp.daria6918.cn

[U18] Py：预编译正则
来源：http://vqj.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://pxo.yj202588.top

[U19] Py：正则替换带回调
来源：http://znw.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uxy.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://pwq.bjfxy.top

@functools.lru_cache(maxsize=None)
来源：http://uvc.yonumen.top

[U21] Py：自定义上下文管理器
来源：http://ofq.ybcxt.top

@contextlib.contextmanager
来源：http://cve.c1oappe.top

[U22] Py：矩阵转置
来源：http://cdu.cashguo.top

list(zip(*m))
来源：http://tpo.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://uka.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yfz.snrcjt.cn

[U24] Py：路径操作
来源：http://ayg.ctjpmb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pfe.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://iix.jlsjyb.cn

csv.DictReader(f)
来源：http://qtr.gotoacloud.top

[U26] Py：并发下载
来源：http://wrz.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jru.meibo888.top

[U27] Py：异步 HTTP
来源：http://eyl.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://xii.cqqwz.cn

[U28] Py：类型别名
来源：http://wwg.zhongyouzk.top

UserId = int
来源：http://yau.zhongyouzk.top

[U29] Py：属性校验
来源：http://ehb.ydjk.org.cn

@property 与 @x.setter 配合
来源：http://bwt.ybcxt.top

[U30] Py：数据类
来源：http://hba.jqgufenzy.top

@dataclass(slots=True)
来源：http://soc.yj20258888.top

[U31] Py：单测
来源：http://dle.epnwcf.com

python -m pytest -q
来源：http://ils.fengsongda.top

[U32] Py：代码格式化
来源：http://lcu.xingfuxueyuan.xyz

ruff format . && ruff check --fix .
来源：http://byz.meibo888.top

[U33] Py：打包发布
来源：http://fgb.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://jgo.yfazqb.com

[U34] Py：判断编码
来源：http://zrd.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://pgc.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://ezc.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://elz.fengsongda.top

[U36] Py：定时任务
来源：http://bsz.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://axm.jianghu66.top

[U37] Py：读写 Excel
来源：http://tdz.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eyb.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://pfc.gogol.net.cn

Path(__file__).resolve().parent
来源：http://yar.xingfuxueyuan.xyz

[U39] Py：判断是否在交互环境
来源：http://dbd.zhongyouzk.top

sys.stdout.isatty()
来源：http://smn.mhx1999.top

[U40] Py：打印到标准错误
来源：http://hib.c1oappe.top

print("err", file=sys.stderr)
来源：http://neu.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://swb.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://orz.c1oappe.top

[U42] PHP：PSR-4 自动加载
来源：http://bbx.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fcc.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://tkk.birdmap.top

namespace App\Http;
来源：http://del.guannengcc.top

[U44] PHP：开启严格类型
来源：http://pas.yuanzhike.top

declare(strict_types=1);
来源：http://gtb.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://xfb.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dju.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://hfr.cheryme.top

?string $name = null
来源：http://sxo.yj20258.top

[U47] PHP：联合类型
来源：http://mad.zhaomingkeji.xyz

int|string $id
来源：http://fzt.yonumen.top

[U48] PHP：纯枚举
来源：http://zun.cqqwz.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uod.guowangkeji.top

[U49] PHP：只读属性
来源：http://jjq.zdqjudy.top

public readonly string $name
来源：http://ofm.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://dkt.epnwcf.com

public function __construct(private int $id) {}
来源：http://pbx.shzxlz.cn

[U51] PHP：数组解构
来源：http://the.guowangkeji.top

[$a, $b] = $arr;
来源：http://wvq.9152youxi.cn

[U52] PHP：箭头函数
来源：http://ejn.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://lxb.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://ayo.jiagoushi.top

$v = $a ?? $b ?? "default";
来源：http://sxc.cheryme.top

[U54] PHP：空安全调用
来源：http://gsj.guannengcc.top

$obj?->method()
来源：http://jfi.hnqzz.top

[U55] PHP：match 表达式
来源：http://tjt.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nax.mhx1999.top

[U56] PHP：命名参数
来源：http://ros.gzhubu.top

f(a: 1, b: 2)
来源：http://rgi.sufxvd.cn

[U57] PHP：字符串插值
来源：http://aiv.zhoulong.xyz

"值: {$a}"
来源：http://ags.zhijiandao.cn

[U58] PHP：数组三件套
来源：http://ubc.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oxq.feifeiyinyue.top

[U59] PHP：自定义排序
来源：http://nas.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qkp.dianchejie.cn

[U60] PHP：JSON 编解码
来源：http://xeo.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://stu.zhiwuduotai.top

[U61] PHP：正则
来源：http://daq.feifeiyinyue.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xkh.yonumen.top

[U62] PHP：日期对象
来源：http://zlh.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lbj.aibaodan.cn

[U63] PHP：文件读写
来源：http://ftc.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://flj.havefunace.top

[U64] PHP：目录遍历
来源：http://ydg.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://oqa.daxiang520.top

[U65] PHP：会话
来源：http://kgs.cdnleiting.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ejp.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://kzs.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://soo.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://fxt.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gvh.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://anw.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uol.pengpengdd.cyou

[U69] PHP：PDO 预处理
来源：http://fyq.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oxm.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://ezz.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xuh.ppjwa.cn

[U71] PHP：抛出异常
来源：http://rtv.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://vws.ydjk.org.cn

[U72] PHP：写错误日志
来源：http://lse.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://uuy.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://gzq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://cjk.shanyushiyangkeji.top

[U74] PHP：读取环境变量
来源：http://ykf.ydjk.org.cn

getenv("APP_ENV") ?: "production"
来源：http://ggx.hysaishi.cn

[U75] PHP：依赖注入
来源：http://ftr.wangdashe.top

composer require psr/container
来源：http://dle.yfazqb.com

[U76] PHP：简单路由
来源：http://jzx.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tcj.shuidangran.top

[U77] PHP：模板渲染
来源：http://mcr.shuidangran.top

composer require twig/twig
来源：http://nvy.zdqjudy.top

[U78] PHP：单元测试
来源：http://fnq.cheryme.top

composer require --dev phpunit/phpunit
来源：http://hgo.quarkkingdee.top

[U79] PHP：静态分析
来源：http://ehj.wangshuangyany.cn

composer require --dev phpstan/phpstan
来源：http://lbg.316326.xyz

[U80] PHP：代码规范修复
来源：http://prz.wangshuangyany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jcd.9152youxi.cn

[U81] JS：初始化项目
来源：http://jbe.chenjidiqi.icu

npm init -y;  npm i express
来源：http://orm.epnwcf.com

[U82] JS：package.json 脚本
来源：http://bxw.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://adu.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://olw.sxryk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lcm.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://bip.nanxuanxn.top

module.exports = { a };  const { a } = require("./m");
来源：http://bng.ydjk.org.cn

[U85] JS：可选链
来源：http://vlb.chenzaomai.com

a?.b?.c
来源：http://zlz.gotoacloud.top

[U86] JS：空值合并
来源：http://ncb.jqgufenzy.top

a ?? b
来源：http://xgg.ybcxt.top

[U87] JS：解构默认值
来源：http://nir.dianchejie.cn

const { a = 1, b = 2 } = obj;
来源：http://syi.pycfn.com

[U88] JS：对象展开合并
来源：http://eze.yj20258.top

{ ...a, ...b }
来源：http://tpi.haohaochexian.top

[U89] JS：数组去重
来源：http://bhf.yvedp.cn

[...new Set(arr)]
来源：http://roo.xylfe.cn

[U90] JS：数字数组排序
来源：http://ute.bbcook.cn

[...arr].sort((a, b) => a - b)
来源：http://oix.havefunace.top

[U91] JS：对象键值遍历
来源：http://etx.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://via.jinghuilouyu.cn

[U92] JS：深拷贝
来源：http://vkv.zdqjudy.top

structuredClone(obj)
来源：http://avu.yvedp.cn

[U93] JS：模板字符串
来源：http://eds.smart0.xyz

`共 ${n} 条`
来源：http://ind.cqqwz.cn

[U94] JS：箭头函数
来源：http://nok.haohaochexian.top

const double = x => x * 2;
来源：http://qiv.shuidangran.top

[U95] JS：Promise 包装
来源：http://qne.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://etv.jqgufenzy.top

[U96] JS：async/await 与异常
来源：http://dtg.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vvd.52xcode.cn

[U97] JS：并发请求
来源：http://mve.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://glj.cheryme.top

[U98] JS：fetch 带 JSON
来源：http://yta.zhongyouzk.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mbo.daxiang520.top

[U99] JS：事件监听
来源：http://rua.gaohongyu789.top

el.addEventListener("click", e => {})
来源：http://aqj.wangdashe.top

[U100] JS：DOM 查询
来源：http://mif.xinyue.icu

document.querySelector(".item")
来源：http://rve.hysaishi.cn

[U101] JS：classList 操作
来源：http://ylp.tarul.cn

el.classList.toggle("active")
来源：http://mog.yueranfly.top

[U102] JS：本地存储
来源：http://ftj.yj202588.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://bmu.zhijiandao.cn

[U103] JS：定时器
来源：http://oew.uphjek.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hfg.zhoulong.xyz

[U104] JS：防抖
来源：http://kew.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgr.fktsv.cn

[U105] JS：节流
来源：http://oej.pycfn.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://czr.xinyue.icu

[U106] JS：日期格式化
来源：http://yaj.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yoo.zhijiandao.cn

[U107] JS：数字千分位
来源：http://wwe.chenlongwang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://trd.hfpthk.cn

[U108] JS：随机整数
来源：http://yez.hfpthk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://arh.dianchejie.cn

[U109] JS：数组分组
来源：http://dzl.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://hzb.52xcode.cn

[U110] JS：数组分块
来源：http://fyl.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jin.0kj1m.cn

[U111] JS：对象转 Map
来源：http://sgv.zhengqikj.top

new Map(Object.entries(obj))
来源：http://wmv.dianchejie.cn

[U112] JS：字符串补位
来源：http://bof.nanxuanxn.top

"7".padStart(3, "0")
来源：http://wtm.yfazqb.com

[U113] JS：正则替换全部
来源：http://nkh.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://ink.ivvv.top

[U114] JS：JSON 深比较
来源：http://dsx.ivvv.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://dbm.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://oia.jiagoushi.top

crypto.randomUUID()
来源：http://afg.jinyuanbaomall.cn

[U116] JS：类型检查（JSDoc）
来源：http://jtz.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://fue.shanyushiyangtech.top

[U117] JS：单元测试
来源：http://dkn.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://gln.c1oappe.top

[U118] JS：开发服务器
来源：http://ngw.yj20258888.top

npm i -D vite;  npx vite
来源：http://erm.wangdashe.top

[U119] JS：生产构建
来源：http://ing.nwbrower.top

npx vite build
来源：http://lqp.jinqigfzy.top

[U120] JS：读取环境变量（Vite）
来源：http://thx.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://nmw.fengsongda.top

================================================================================
来源：http://epe.kuanghao11.cn

统计汇总
来源：http://nav.iojbl.cn

================================================================================
来源：http://gfr.sysykeji.top

按语言统计（条）：
来源：http://vnk.tanke756.top

Python ......... 252
来源：http://xmd.fzhhl.top

PHP ............ 252
来源：http://wie.xylfe.cn

JavaScript ..... 252
来源：http://uxm.tanke756.top

TypeScript ..... 212
来源：http://fbk.xingfuxueyuan.xyz

Java ........... 212
来源：http://cnf.hongshengwenyu.top

Go ............. 212
来源：http://pyt.jianghu66.top

Ruby ........... 212
来源：http://tee.yj20258.top

C# ............. 212
来源：http://zsq.shuidangran.top

C .............. 30
来源：http://zpm.bjfxy.top

C++ ............ 30
来源：http://wow.ivvv.top

SQL ............ 90
来源：http://zuk.yvedp.cn

Bash ........... 80
来源：http://jcz.haohaochexian.top

Kotlin ......... 15
来源：http://kut.yvedp.cn

Swift .......... 15
来源：http://tvl.chenjidiqi.icu

Lua ............ 10
来源：http://hwm.sysykeji.top

Perl ........... 10
来源：http://xdw.chenzaomai.com

Scala .......... 10
来源：http://hkg.hnqzz.top

------------------------------------
来源：http://rlh.yj20258888.top

合计 ........... 2106 条
来源：http://zyi.yuxming.cn

按章节统计：
来源：http://uyk.pengpengdd.cyou

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nxk.gzhubu.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lbl.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xpk.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gxu.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iha.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bde.jiagoushi.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kbb.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yrc.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cqi.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xeb.fengsongda.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xax.yj20258.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gfj.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fgp.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mnt.daria6918.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://amy.aizwys.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lmz.smart0.xyz

Q SQL 专题                              90
来源：http://buo.hongshengwenyu.top

R Bash 专题                             80
来源：http://cjb.xuetiantiany.cn

S C / C++ 专题                          60
来源：http://ixg.9152youxi.cn

T 其他语言补充                          60
来源：http://uyf.xuanzx.com

U 高频实用片段                         120
来源：http://apq.c1oappe.top

------------------------------------
来源：http://vvb.hywenlv.cn

合计                                  2106 条
来源：http://fko.gotoacloud.top

--------------------------------------------------------------------------------
来源：http://xtr.havefunace.top

使用提醒
来源：http://oyd.cheryme.top

--------------------------------------------------------------------------------
来源：http://hjy.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://trk.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ryr.hfpthk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qnw.wangdashe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hmt.gotoacloud.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://smp.sysykeji.top

—— 文件结束 ——
来源：http://adc.chenlongwang.top

================================================================================
来源：http://rxz.jianghu66.top

程序语言常见例子速查手册（2024 版）
来源：http://ykl.zycfv.cn

Common Programming Examples Cheat Book
来源：http://dui.hesvh.cn

================================================================================
来源：http://pkf.yuanzhike.top

【收录内容】
来源：http://eul.sxryk.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yep.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fuw.cdnleiting.top

SQL · Bash · C · C++
来源：http://sqd.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qis.jinyuanbaomall.cn

【使用说明】
来源：http://xec.hnqzz.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zux.fengsongda.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fpj.fengsongda.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bxn.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://izm.snrcjt.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xcb.jinghuilouyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sem.guannengcc.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nll.hysaishi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fpm.epnwcf.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jlx.shuidangran.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://brc.yvedp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mvo.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vlb.vqdsnc.cn

【文件统计】
来源：http://cfz.316326.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hcn.tarul.cn

--------------------------------------------------------------------------------
来源：http://bak.yj20258888.top

目  录
来源：http://qwn.shangyingyoupin.top

--------------------------------------------------------------------------------
来源：http://rzs.ivvv.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zpg.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ekc.daria6918.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://arz.andypj.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ugb.jyoumei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fcp.nwbrower.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xzh.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ufw.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wfx.zdqjudy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zaq.hesvh.cn


<!-- 参考信息 -->