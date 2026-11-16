代发 wailian999

[U05] Py：列表去重且保序
来源：http://bzq.yongpay.top

list(dict.fromkeys(arr))
来源：http://gog.yj20258888.top

[U06] Py：合并两个字典
来源：http://zlu.feifeiyinyue.top

{**a, **b}
来源：http://qym.gotoacloud.top

[U07] Py：反转字典键值
来源：http://naf.cucudq.cn

{v: k for k, v in d.items()}
来源：http://ssw.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://ylu.shanyushiyangkeji.top

[y for x in nested for y in x]
来源：http://dsm.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://rfg.zhiwuduotai.top

max(d, key=d.get)
来源：http://mlw.iojbl.cn

[U10] Py：按值排序字典
来源：http://poy.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ogu.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://ldh.andypj.xyz

(x * 2 for x in arr)
来源：http://puu.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://jny.shzxlz.cn

Counter(arr).most_common(3)
来源：http://ncf.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://req.daxiang520.top

deque(maxlen=10)
来源：http://esv.guowangkeji.top

[U14] Py：分组收集到列表
来源：http://eni.ppjwa.cn

defaultdict(list)
来源：http://hvp.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://mcw.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://aqo.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://xgs.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kmt.sjlbkw.cn

[U17] Py：初始化日志
来源：http://egz.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://xoi.redwolf501.top

[U18] Py：预编译正则
来源：http://lgb.yvedp.cn

pat = re.compile(r"\d+")
来源：http://mcw.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://fmy.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uif.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://eoz.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://dyv.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://bbf.meibo888.top

@contextlib.contextmanager
来源：http://ajq.cheryme.top

[U22] Py：矩阵转置
来源：http://jjx.xuetiantiany.cn

list(zip(*m))
来源：http://ono.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://dfo.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cwt.cqqwz.cn

[U24] Py：路径操作
来源：http://pay.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://miq.zdqjudy.top

[U25] Py：CSV 按字典读
来源：http://evr.hfpthk.cn

csv.DictReader(f)
来源：http://hke.jqgfzy.top

[U26] Py：并发下载
来源：http://nrm.yueranfly.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tnb.zhongyouzk.top

[U27] Py：异步 HTTP
来源：http://maa.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://ptw.tanke756.top

[U28] Py：类型别名
来源：http://vbc.guannengcc.top

UserId = int
来源：http://lpq.guowangkeji.top

[U29] Py：属性校验
来源：http://yvx.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://mun.guannengcc.top

[U30] Py：数据类
来源：http://tiy.zhixingplan.top

@dataclass(slots=True)
来源：http://dgc.zhoulong.xyz

[U31] Py：单测
来源：http://zzd.fanxiaobao.xyz

python -m pytest -q
来源：http://ojg.ivvv.top

[U32] Py：代码格式化
来源：http://bgq.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://eto.yj20258.top

[U33] Py：打包发布
来源：http://bao.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://zzg.epnwcf.com

[U34] Py：判断编码
来源：http://uvf.zhoulong.xyz

chardet.detect(raw)
来源：http://fuj.yfazqb.com

[U35] Py：发送邮件
来源：http://rnk.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ude.zdbjq.cn

[U36] Py：定时任务
来源：http://nww.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://ins.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://pas.aibaodan.cn

pandas.read_excel / DataFrame.to_excel
来源：http://exk.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://ozi.cucudq.cn

Path(__file__).resolve().parent
来源：http://pta.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://sle.0kj1m.cn

sys.stdout.isatty()
来源：http://nly.mhx1999.top

[U40] Py：打印到标准错误
来源：http://kmt.fengsongda.top

print("err", file=sys.stderr)
来源：http://cty.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://dyz.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://adq.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://amu.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vfj.cucudq.cn

[U43] PHP：声明命名空间
来源：http://wgw.zhengqikj.top

namespace App\Http;
来源：http://xvt.hesvh.cn

[U44] PHP：开启严格类型
来源：http://inx.chenlongwang.top

declare(strict_types=1);
来源：http://tim.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://jyq.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cgk.chenjidiqi.icu

[U46] PHP：可空类型
来源：http://mhh.jianghu66.top

?string $name = null
来源：http://xho.guowangkeji.top

[U47] PHP：联合类型
来源：http://foy.sxryk.cn

int|string $id
来源：http://xgt.zdbjq.cn

[U48] PHP：纯枚举
来源：http://tqw.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vlh.yfazqb.com

[U49] PHP：只读属性
来源：http://xfd.shangyingyoupin.top

public readonly string $name
来源：http://ofv.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://mtd.sufxvd.cn

public function __construct(private int $id) {}
来源：http://nos.jianghu66.top

[U51] PHP：数组解构
来源：http://wjz.yvedp.cn

[$a, $b] = $arr;
来源：http://ssl.hywenlv.cn

[U52] PHP：箭头函数
来源：http://glx.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://iga.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://ief.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://tgs.zhengqikj.top

[U54] PHP：空安全调用
来源：http://dmg.shanyushiyangtech.top

$obj?->method()
来源：http://xbh.zhengqikj.top

[U55] PHP：match 表达式
来源：http://ibb.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dvg.svipenyu.cn

[U56] PHP：命名参数
来源：http://zqu.epnwcf.com

f(a: 1, b: 2)
来源：http://jra.daxiang520.top

[U57] PHP：字符串插值
来源：http://pmy.guannengcc.top

"值: {$a}"
来源：http://xdk.ybcxt.top

[U58] PHP：数组三件套
来源：http://hbv.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dug.iojbl.cn

[U59] PHP：自定义排序
来源：http://krl.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rja.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://ijf.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://voh.yvedp.cn

[U61] PHP：正则
来源：http://wlo.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xgh.yueranfly.top

[U62] PHP：日期对象
来源：http://hak.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bbw.cqqwz.cn

[U63] PHP：文件读写
来源：http://jnq.shangyingyoupin.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lms.iojbl.cn

[U64] PHP：目录遍历
来源：http://ilm.jqgufenzy.top

glob("dir/*.php");  scandir("dir");
来源：http://ylm.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://npz.52xcode.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dfz.jqgfzy.top

[U66] PHP：设置 Cookie
来源：http://jit.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vjv.cucudq.cn

[U67] PHP：处理文件上传
来源：http://evb.gaohongyu789.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xkd.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://ukr.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hbg.kuanghao11.cn

[U69] PHP：PDO 预处理
来源：http://dbe.iojbl.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mkc.nwbrower.top

[U70] PHP：PDO 事务
来源：http://vcn.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://quh.316326.xyz

[U71] PHP：抛出异常
来源：http://nuy.yuanzhike.top

throw new RuntimeException("失败", 500);
来源：http://wmh.vehdjk.com

[U72] PHP：写错误日志
来源：http://xgc.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://div.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://kcs.ivvv.top

parse_ini_file("config.ini", true)
来源：http://ulq.hammf.cn

[U74] PHP：读取环境变量
来源：http://oer.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://gez.fanxiaobao.xyz

[U75] PHP：依赖注入
来源：http://wpm.fktsv.cn

composer require psr/container
来源：http://vyl.jinqigfzy.top

[U76] PHP：简单路由
来源：http://zua.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kvm.yueranfly.top

[U77] PHP：模板渲染
来源：http://ugf.9152youxi.cn

composer require twig/twig
来源：http://qsy.xinyue.icu

[U78] PHP：单元测试
来源：http://bbe.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://eiz.cqqwz.cn

[U79] PHP：静态分析
来源：http://qse.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://okj.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://zpm.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hku.svipenyu.cn

[U81] JS：初始化项目
来源：http://wzu.0kj1m.cn

npm init -y;  npm i express
来源：http://hmn.cqqwz.cn

[U82] JS：package.json 脚本
来源：http://rzv.gogol.net.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qse.jyoumei.cn

[U83] JS：ES Module 导入导出
来源：http://fjp.yfazqb.com

export const a = 1;  import { a } from "./m.js";
来源：http://tak.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://tje.fanxiaobao.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://upq.hesvh.cn

[U85] JS：可选链
来源：http://oja.aizwys.cn

a?.b?.c
来源：http://ods.chenzaomai.com

[U86] JS：空值合并
来源：http://lhf.havefunace.top

a ?? b
来源：http://ejq.jqgufenzy.top

[U87] JS：解构默认值
来源：http://wci.redwolf501.top

const { a = 1, b = 2 } = obj;
来源：http://ttr.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://bbo.mhx1999.top

{ ...a, ...b }
来源：http://tgy.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://wen.chenjidiqi.icu

[...new Set(arr)]
来源：http://ojw.aibaodan.cn

[U90] JS：数字数组排序
来源：http://ruc.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://tdu.ydzc1.top

[U91] JS：对象键值遍历
来源：http://hbp.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nut.shuidangran.top

[U92] JS：深拷贝
来源：http://gpn.gotoacloud.top

structuredClone(obj)
来源：http://myh.epnwcf.com

[U93] JS：模板字符串
来源：http://qsj.epnwcf.com

`共 ${n} 条`
来源：http://ajp.yfazqb.com

[U94] JS：箭头函数
来源：http://frg.snrcjt.cn

const double = x => x * 2;
来源：http://hmy.sysykeji.top

[U95] JS：Promise 包装
来源：http://rpl.9152youxi.cn

new Promise((resolve, reject) => {})
来源：http://jsk.guannengcc.top

[U96] JS：async/await 与异常
来源：http://qdp.xuanzx.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qwi.sxryk.cn

[U97] JS：并发请求
来源：http://aav.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vwa.hcnkem.com

[U98] JS：fetch 带 JSON
来源：http://tqj.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uqp.jyoumei.cn

[U99] JS：事件监听
来源：http://tby.zhaomingkeji.xyz

el.addEventListener("click", e => {})
来源：http://eoq.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://oer.zhongyouzk.top

document.querySelector(".item")
来源：http://fvv.jinghuilouyu.cn

[U101] JS：classList 操作
来源：http://gcw.yj20258.top

el.classList.toggle("active")
来源：http://sct.jqgufenzy.top

[U102] JS：本地存储
来源：http://nwy.0kj1m.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fyx.sweek.top

[U103] JS：定时器
来源：http://rol.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blz.hcnkem.com

[U104] JS：防抖
来源：http://hzc.yuanzhike.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcq.ywan-chungtsiang.top

[U105] JS：节流
来源：http://byu.tianlin.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lgm.nanxinkj.top

[U106] JS：日期格式化
来源：http://jpw.wangshuangyany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pxu.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://lgi.shzxlz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mpe.xziqi.cn

[U108] JS：随机整数
来源：http://cnu.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qkf.yanxiufei.cn

[U109] JS：数组分组
来源：http://vvp.jqgufenzy.top

Object.groupBy(arr, x => x.type)
来源：http://ptj.svipenyu.cn

[U110] JS：数组分块
来源：http://wrg.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://efh.yuxming.cn

[U111] JS：对象转 Map
来源：http://foo.yuanzhike.top

new Map(Object.entries(obj))
来源：http://ood.jlsjyb.cn

[U112] JS：字符串补位
来源：http://pzt.jinqigufen.top

"7".padStart(3, "0")
来源：http://gby.smart0.xyz

[U113] JS：正则替换全部
来源：http://kac.svipenyu.cn

s.replaceAll("a", "b")
来源：http://mzx.jlsjyb.cn

[U114] JS：JSON 深比较
来源：http://tll.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://oum.hfpthk.cn

[U115] JS：生成 UUID
来源：http://anw.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://uzx.fzhhl.top

[U116] JS：类型检查（JSDoc）
来源：http://ova.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://cak.yj202588.top

[U117] JS：单元测试
来源：http://wvy.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://krw.sysykeji.top

[U118] JS：开发服务器
来源：http://ojd.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://axc.tarul.cn

[U119] JS：生产构建
来源：http://eny.jqgufenzy.top

npx vite build
来源：http://jtk.hongshengwenyu.top

[U120] JS：读取环境变量（Vite）
来源：http://dkg.quarkkingdee.top

import.meta.env.VITE_API_URL
来源：http://evt.xingfuxueyuan.xyz

================================================================================
来源：http://bxx.fzhhl.top

统计汇总
来源：http://qdf.xuetiantiany.cn

================================================================================
来源：http://eua.c1oappe.top

按语言统计（条）：
来源：http://wbf.jinqigfzy.top

Python ......... 252
来源：http://pvs.zhoulong.xyz

PHP ............ 252
来源：http://mto.cucudq.cn

JavaScript ..... 252
来源：http://mor.yonumen.top

TypeScript ..... 212
来源：http://xhq.dashuyun.cn

Java ........... 212
来源：http://yao.chenlongwang.top

Go ............. 212
来源：http://huy.52xcode.cn

Ruby ........... 212
来源：http://waw.jinqigufen.top

C# ............. 212
来源：http://ufh.uphjek.com

C .............. 30
来源：http://trz.epnwcf.com

C++ ............ 30
来源：http://paq.sweek.top

SQL ............ 90
来源：http://bnn.yongpay.top

Bash ........... 80
来源：http://hdk.yj20258888.top

Kotlin ......... 15
来源：http://sob.hesvh.cn

Swift .......... 15
来源：http://ara.ywan-chungtsiang.top

Lua ............ 10
来源：http://rfn.jqgufenzy.top

Perl ........... 10
来源：http://kex.fengsongda.top

Scala .......... 10
来源：http://fmt.nwbrower.top

------------------------------------
来源：http://egi.wangdashe.top

合计 ........... 2106 条
来源：http://ycn.mhx1999.top

按章节统计：
来源：http://eau.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gfd.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yqz.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fqs.chenjidiqi.icu

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://izb.zhengqikj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vvo.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uoo.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xwh.tianlin.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jxz.ctjpmb.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hgk.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yvt.zhaomingkeji.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xft.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eud.yj202588.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nuc.hywenlv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mul.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://agq.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sph.ivvv.top

Q SQL 专题                              90
来源：http://ipl.wangshuangyany.cn

R Bash 专题                             80
来源：http://mcv.hfpthk.cn

S C / C++ 专题                          60
来源：http://uhe.andypj.xyz

T 其他语言补充                          60
来源：http://ayk.yj20258.top

U 高频实用片段                         120
来源：http://gjg.pengpengdd.cyou

------------------------------------
来源：http://lgu.jinqigufen.top

合计                                  2106 条
来源：http://cph.tian-w.cn

--------------------------------------------------------------------------------
来源：http://vir.hywenlv.cn

使用提醒
来源：http://zvg.wangdashe.top

--------------------------------------------------------------------------------
来源：http://jgs.xuetiantiany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nqa.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mti.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zdo.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://ftf.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://imm.ivvv.top

—— 文件结束 ——
来源：http://ufq.jqgufenzy.top

================================================================================
来源：http://yis.shanyushiyangtech.top

程序语言常见例子速查手册（2024 版）
来源：http://irh.guannengcc.top

Common Programming Examples Cheat Book
来源：http://sws.quarkkingdee.top

================================================================================
来源：http://vks.yueranfly.top

【收录内容】
来源：http://hot.gotoacloud.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://aep.jinghuilouyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iir.c1oappe.top

SQL · Bash · C · C++
来源：http://kjc.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://haj.cheryme.top

【使用说明】
来源：http://lbw.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gqa.zhijiandao.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qbc.shanyushiyangkeji.top


<!-- 参考信息 -->