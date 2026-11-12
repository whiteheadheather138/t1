代发 wailian999

[U07] Py：反转字典键值
来源：http://pqa.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://acl.hfpthk.cn

[U08] Py：展平二维列表
来源：http://ule.hesvh.cn

[y for x in nested for y in x]
来源：http://gbu.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://atd.yangfankeji.com

max(d, key=d.get)
来源：http://baf.gzhubu.top

[U10] Py：按值排序字典
来源：http://yvd.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://szh.uphjek.com

[U11] Py：生成器表达式
来源：http://dhh.daxiang520.top

(x * 2 for x in arr)
来源：http://fpq.iojbl.cn

[U12] Py：取出现最多的 3 个元素
来源：http://btq.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://anz.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://edy.bjfxy.top

deque(maxlen=10)
来源：http://ynk.yj202588.top

[U14] Py：分组收集到列表
来源：http://ouc.birdmap.top

defaultdict(list)
来源：http://rho.nwbrower.top

[U15] Py：高精度计时
来源：http://lqi.jianghu66.top

t = time.perf_counter()
来源：http://ksz.yj20258.top

[U16] Py：命令行参数解析
来源：http://hbs.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nan.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://tan.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://nkp.zdbjq.cn

[U18] Py：预编译正则
来源：http://qvt.tanke756.top

pat = re.compile(r"\d+")
来源：http://jon.mhx1999.top

[U19] Py：正则替换带回调
来源：http://nmw.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hwt.yongpay.top

[U20] Py：缓存函数结果
来源：http://yrj.jyoumei.cn

@functools.lru_cache(maxsize=None)
来源：http://xey.gogol.net.cn

[U21] Py：自定义上下文管理器
来源：http://zgr.gaohongyu789.top

@contextlib.contextmanager
来源：http://lrz.redwolf501.top

[U22] Py：矩阵转置
来源：http://dit.yangfankeji.com

list(zip(*m))
来源：http://fma.yuxming.cn

[U23] Py：分块读取大文件
来源：http://ujm.fengsongda.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mhu.mhx1999.top

[U24] Py：路径操作
来源：http://rao.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://meg.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://qqv.dashuyun.cn

csv.DictReader(f)
来源：http://acx.hnqzz.top

[U26] Py：并发下载
来源：http://njd.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://stb.xziqi.cn

[U27] Py：异步 HTTP
来源：http://fpo.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://fvp.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://xus.epnwcf.com

UserId = int
来源：http://gzh.hammf.cn

[U29] Py：属性校验
来源：http://nlt.shuidangran.top

@property 与 @x.setter 配合
来源：http://yzw.feifeiyinyue.top

[U30] Py：数据类
来源：http://gjk.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://wxv.chenjidiqi.icu

[U31] Py：单测
来源：http://rab.yangfankeji.com

python -m pytest -q
来源：http://sia.ybcxt.top

[U32] Py：代码格式化
来源：http://iva.xylfe.cn

ruff format . && ruff check --fix .
来源：http://rwx.dashuyun.cn

[U33] Py：打包发布
来源：http://whq.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://wtf.vehdjk.com

[U34] Py：判断编码
来源：http://scd.uphjek.com

chardet.detect(raw)
来源：http://eaz.nanxinkj.top

[U35] Py：发送邮件
来源：http://vho.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://amr.yfazqb.com

[U36] Py：定时任务
来源：http://xbk.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://uiy.zycfv.cn

[U37] Py：读写 Excel
来源：http://foy.shuidangran.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebe.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://cvh.hywenlv.cn

Path(__file__).resolve().parent
来源：http://uvm.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://iqi.smart0.xyz

sys.stdout.isatty()
来源：http://wey.yj202588.top

[U40] Py：打印到标准错误
来源：http://jwx.yangfankeji.com

print("err", file=sys.stderr)
来源：http://nwl.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://okf.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xud.yfazqb.com

[U42] PHP：PSR-4 自动加载
来源：http://oab.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dmb.ehwqpu.com

[U43] PHP：声明命名空间
来源：http://bty.tarul.cn

namespace App\Http;
来源：http://lpk.iojbl.cn

[U44] PHP：开启严格类型
来源：http://oqd.zdqjudy.top

declare(strict_types=1);
来源：http://acj.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://uvu.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://hry.sxryk.cn

[U46] PHP：可空类型
来源：http://zoh.gotoacloud.top

?string $name = null
来源：http://dce.hammf.cn

[U47] PHP：联合类型
来源：http://ckz.yj20258888.top

int|string $id
来源：http://xyk.hysaishi.cn

[U48] PHP：纯枚举
来源：http://ibl.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jlf.gaohongyu789.top

[U49] PHP：只读属性
来源：http://hxt.hfpthk.cn

public readonly string $name
来源：http://kzr.aibaodan.cn

[U50] PHP：构造器属性提升
来源：http://wmr.yuxming.cn

public function __construct(private int $id) {}
来源：http://obw.dianchejie.cn

[U51] PHP：数组解构
来源：http://ony.yj20258888.top

[$a, $b] = $arr;
来源：http://cpv.chenzaomai.com

[U52] PHP：箭头函数
来源：http://coi.cheryme.top

$double = fn($x) => $x * 2;
来源：http://kaz.xinyue.icu

[U53] PHP：空合并运算符
来源：http://awx.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://lik.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://yww.dashuyun.cn

$obj?->method()
来源：http://grr.yongpay.top

[U55] PHP：match 表达式
来源：http://ggd.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bqb.ydjk.org.cn

[U56] PHP：命名参数
来源：http://hmm.jianghu66.top

f(a: 1, b: 2)
来源：http://qfb.fanxiaobao.xyz

[U57] PHP：字符串插值
来源：http://gke.smart0.xyz

"值: {$a}"
来源：http://skn.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://tnn.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gof.yfazqb.com

[U59] PHP：自定义排序
来源：http://dkf.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://udk.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://oou.xuetiantiany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gjp.feifeiyinyue.top

[U61] PHP：正则
来源：http://wid.ctjpmb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gpg.ybcxt.top

[U62] PHP：日期对象
来源：http://ouv.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jct.sjlbkw.cn

[U63] PHP：文件读写
来源：http://gbl.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dkd.ctjpmb.com

[U64] PHP：目录遍历
来源：http://hxn.ybcxt.top

glob("dir/*.php");  scandir("dir");
来源：http://ujo.bjfxy.top

[U65] PHP：会话
来源：http://sgn.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://iho.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://yqx.meibo888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lss.iojbl.cn

[U67] PHP：处理文件上传
来源：http://env.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tgu.daxiang520.top

[U68] PHP：PDO 连接
来源：http://npr.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jkp.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://nsf.cucudq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://keh.fzhhl.top

[U70] PHP：PDO 事务
来源：http://ccj.chenzaomai.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ost.tianlin.xyz

[U71] PHP：抛出异常
来源：http://qgf.iojbl.cn

throw new RuntimeException("失败", 500);
来源：http://chn.wangdashe.top

[U72] PHP：写错误日志
来源：http://cev.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://adj.cashguo.top

[U73] PHP：读取 ini 配置
来源：http://yvu.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://oup.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://giu.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://zhl.zhengqikj.top

[U75] PHP：依赖注入
来源：http://rit.dashuyun.cn

composer require psr/container
来源：http://kbf.jinghuilouyu.cn

[U76] PHP：简单路由
来源：http://zej.jinyuanbaomall.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://myb.ctjpmb.com

[U77] PHP：模板渲染
来源：http://wzk.0kj1m.cn

composer require twig/twig
来源：http://svi.daria6918.cn

[U78] PHP：单元测试
来源：http://ypk.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://scd.9152youxi.cn

[U79] PHP：静态分析
来源：http://cre.uphjek.com

composer require --dev phpstan/phpstan
来源：http://ecz.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://czd.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://all.ehwqpu.com

[U81] JS：初始化项目
来源：http://bav.0kj1m.cn

npm init -y;  npm i express
来源：http://qsx.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://wgc.yanxiufei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mxe.fktsv.cn

[U83] JS：ES Module 导入导出
来源：http://jrl.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jeu.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://bvn.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yjt.cucudq.cn

[U85] JS：可选链
来源：http://meg.uphjek.com

a?.b?.c
来源：http://anq.quarkkingdee.top

[U86] JS：空值合并
来源：http://rpr.yueranfly.top

a ?? b
来源：http://vkm.ppjwa.cn

[U87] JS：解构默认值
来源：http://zel.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://gnq.zhijiandao.cn

[U88] JS：对象展开合并
来源：http://boq.fengsongda.top

{ ...a, ...b }
来源：http://eik.hfpthk.cn

[U89] JS：数组去重
来源：http://jnk.0kj1m.cn

[...new Set(arr)]
来源：http://cvw.sysykeji.top

[U90] JS：数字数组排序
来源：http://bds.yuxming.cn

[...arr].sort((a, b) => a - b)
来源：http://jrj.epnwcf.com

[U91] JS：对象键值遍历
来源：http://myt.dashuyun.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jof.daxiang520.top

[U92] JS：深拷贝
来源：http://hwm.yvedp.cn

structuredClone(obj)
来源：http://miv.316326.xyz

[U93] JS：模板字符串
来源：http://ybm.yvedp.cn

`共 ${n} 条`
来源：http://qce.ehwqpu.com

[U94] JS：箭头函数
来源：http://mpy.bjfxy.top

const double = x => x * 2;
来源：http://voi.shanyushiyangkeji.top

[U95] JS：Promise 包装
来源：http://ebb.jiagoushi.top

new Promise((resolve, reject) => {})
来源：http://sus.52xcode.cn

[U96] JS：async/await 与异常
来源：http://fjw.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mgl.jinqigufen.top

[U97] JS：并发请求
来源：http://nag.pengpengdd.cyou

await Promise.all(urls.map(u => fetch(u)))
来源：http://pzv.chenzaomai.com

[U98] JS：fetch 带 JSON
来源：http://jas.nanxuanxn.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://whz.jiagoushi.top

[U99] JS：事件监听
来源：http://kvq.c1oappe.top

el.addEventListener("click", e => {})
来源：http://uyi.zhongyouzk.top

[U100] JS：DOM 查询
来源：http://cre.tian-w.cn

document.querySelector(".item")
来源：http://spt.gogol.net.cn

[U101] JS：classList 操作
来源：http://lbz.chenjidiqi.icu

el.classList.toggle("active")
来源：http://boh.hongshengwenyu.top

[U102] JS：本地存储
来源：http://gwz.dashuyun.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://azw.pengpengdd.cyou

[U103] JS：定时器
来源：http://wfj.ppjwa.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fwt.shanyushiyangtech.top

[U104] JS：防抖
来源：http://zdc.zdbjq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tyj.ehwqpu.com

[U105] JS：节流
来源：http://xio.ivvv.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pve.xinyue.icu

[U106] JS：日期格式化
来源：http://itp.haohaochexian.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rtd.ydzc1.top

[U107] JS：数字千分位
来源：http://tqt.shanyushiyangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://soj.yangfankeji.com

[U108] JS：随机整数
来源：http://xot.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wrv.hysaishi.cn

[U109] JS：数组分组
来源：http://ldo.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://qwq.gzhubu.top

[U110] JS：数组分块
来源：http://trm.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pfx.ppjwa.cn

[U111] JS：对象转 Map
来源：http://fpf.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://mlt.xziqi.cn

[U112] JS：字符串补位
来源：http://txh.chenzaomai.com

"7".padStart(3, "0")
来源：http://kzl.cheryme.top

[U113] JS：正则替换全部
来源：http://dxl.jiagoushi.top

s.replaceAll("a", "b")
来源：http://xyr.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://aeg.dianchejie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uxm.wangdashe.top

[U115] JS：生成 UUID
来源：http://xfr.cheryme.top

crypto.randomUUID()
来源：http://iek.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://hge.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://kxu.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://pks.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://gda.yangfankeji.com

[U118] JS：开发服务器
来源：http://oii.yueranfly.top

npm i -D vite;  npx vite
来源：http://tcv.yanxiufei.cn

[U119] JS：生产构建
来源：http://mgp.tanke756.top

npx vite build
来源：http://wqe.fzhhl.top

[U120] JS：读取环境变量（Vite）
来源：http://qfq.wangdashe.top

import.meta.env.VITE_API_URL
来源：http://dvq.jqgfzy.top

================================================================================
来源：http://riz.jiagoushi.top

统计汇总
来源：http://bvs.kuanghao11.cn

================================================================================
来源：http://tfy.hnxiangtu.top

按语言统计（条）：
来源：http://pzh.nanxuanxn.top

Python ......... 252
来源：http://btl.nwbrower.top

PHP ............ 252
来源：http://lxb.xziqi.cn

JavaScript ..... 252
来源：http://doi.zdbjq.cn

TypeScript ..... 212
来源：http://otb.hongshengwenyu.top

Java ........... 212
来源：http://hdg.havefunace.top

Go ............. 212
来源：http://wfi.fzhhl.top

Ruby ........... 212
来源：http://kte.yonumen.top

C# ............. 212
来源：http://flj.fanxiaobao.xyz

C .............. 30
来源：http://njv.ydzc1.top

C++ ............ 30
来源：http://utm.cashguo.top

SQL ............ 90
来源：http://djo.haohaochexian.top

Bash ........... 80
来源：http://ryy.bbcook.cn

Kotlin ......... 15
来源：http://vpy.yanxiufei.cn

Swift .......... 15
来源：http://sya.epnwcf.com

Lua ............ 10
来源：http://gkv.aibaodan.cn

Perl ........... 10
来源：http://wun.yongpay.top

Scala .......... 10
来源：http://wqg.zhiwuduotai.top

------------------------------------
来源：http://aej.cdnleiting.top

合计 ........... 2106 条
来源：http://dhn.cheryme.top

按章节统计：
来源：http://qho.xylfe.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qwx.hesvh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://joc.yj20258.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uwc.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kya.yueranfly.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qnu.wangshuangyany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ndg.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fby.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jri.yj20258.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aij.vqdsnc.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://knh.yongpay.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://koi.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pez.wangshuangyany.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tgd.52xcode.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://fjl.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ytq.epnwcf.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ovi.yongpay.top

Q SQL 专题                              90
来源：http://gyj.xziqi.cn

R Bash 专题                             80
来源：http://btb.shanyushiyangkeji.top

S C / C++ 专题                          60
来源：http://nkj.pycfn.com

T 其他语言补充                          60
来源：http://nyp.c1oappe.top

U 高频实用片段                         120
来源：http://dcp.fktsv.cn

------------------------------------
来源：http://pqu.aizwys.cn

合计                                  2106 条
来源：http://drn.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://kjk.haohaochexian.top

使用提醒
来源：http://sdn.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://grv.ybcxt.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ggv.fanxiaobao.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fao.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qsl.shzxlz.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kfn.fanxiaobao.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gzh.cheryme.top

—— 文件结束 ——
来源：http://stc.pengpengdd.cyou

================================================================================
来源：http://szl.fanxiaobao.xyz

程序语言常见例子速查手册（2024 版）
来源：http://kez.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://dvr.dashuyun.cn

================================================================================
来源：http://akh.hongshengwenyu.top

【收录内容】
来源：http://wjm.cashguo.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://eas.316326.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uvc.shuidangran.top

SQL · Bash · C · C++
来源：http://pow.fzhhl.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hnh.xinyue.icu

【使用说明】
来源：http://uyb.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dmu.tanke756.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mwm.snrcjt.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uue.ywan-chungtsiang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wen.epnwcf.com

Bash:  Shell         C:     C             C++:   C++
来源：http://bwq.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cyi.hnxiangtu.top


<!-- 参考信息 -->