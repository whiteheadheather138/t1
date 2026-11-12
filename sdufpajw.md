代发 wailian999

[U03] Py：加载 .env 配置
来源：http://ipp.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dzl.cqqwz.cn

[U04] Py：变量调试打印
来源：http://iyd.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://avg.yfazqb.com

[U05] Py：列表去重且保序
来源：http://ykz.yanxiufei.cn

list(dict.fromkeys(arr))
来源：http://dph.shuidangran.top

[U06] Py：合并两个字典
来源：http://wqa.gogol.net.cn

{**a, **b}
来源：http://sdb.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://oyp.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://zcx.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://kaz.yj20258888.top

[y for x in nested for y in x]
来源：http://mhf.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://bji.ydjk.org.cn

max(d, key=d.get)
来源：http://zuy.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://gcs.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ofi.zhixingplan.top

[U11] Py：生成器表达式
来源：http://jpx.tarul.cn

(x * 2 for x in arr)
来源：http://spc.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://dwg.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://vvy.jqgfzy.top

[U13] Py：固定长度队列
来源：http://lwt.jqgfzy.top

deque(maxlen=10)
来源：http://gyp.yuxming.cn

[U14] Py：分组收集到列表
来源：http://rfb.wangdashe.top

defaultdict(list)
来源：http://rra.hnqzz.top

[U15] Py：高精度计时
来源：http://xof.316326.xyz

t = time.perf_counter()
来源：http://luu.ydzc1.top

[U16] Py：命令行参数解析
来源：http://vzg.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qhg.jqgfzy.top

[U17] Py：初始化日志
来源：http://oup.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://jsi.gzhubu.top

[U18] Py：预编译正则
来源：http://xhs.yj202588.top

pat = re.compile(r"\d+")
来源：http://cjj.cashguo.top

[U19] Py：正则替换带回调
来源：http://mfm.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mfy.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://bxe.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://fic.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://rip.c1oappe.top

@contextlib.contextmanager
来源：http://gyj.dashuyun.cn

[U22] Py：矩阵转置
来源：http://grd.hfpthk.cn

list(zip(*m))
来源：http://zwm.fehbvm.com

[U23] Py：分块读取大文件
来源：http://kso.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dds.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://icb.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lps.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://plm.yuanzhike.top

csv.DictReader(f)
来源：http://hjj.shangyingyoupin.top

[U26] Py：并发下载
来源：http://sze.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kzj.sufxvd.cn

[U27] Py：异步 HTTP
来源：http://fsa.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://pzx.yj202588.top

[U28] Py：类型别名
来源：http://bpn.wangshuangyany.cn

UserId = int
来源：http://pvd.sxryk.cn

[U29] Py：属性校验
来源：http://pkp.sxryk.cn

@property 与 @x.setter 配合
来源：http://mdj.nwbrower.top

[U30] Py：数据类
来源：http://def.vqdsnc.cn

@dataclass(slots=True)
来源：http://hvr.yfazqb.com

[U31] Py：单测
来源：http://fyr.kuanghao11.cn

python -m pytest -q
来源：http://xxx.dianchejie.cn

[U32] Py：代码格式化
来源：http://fjq.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://pod.yueranfly.top

[U33] Py：打包发布
来源：http://qta.ydzc1.top

python -m build  （依赖 pyproject.toml）
来源：http://foi.sjlbkw.cn

[U34] Py：判断编码
来源：http://upk.aizwys.cn

chardet.detect(raw)
来源：http://pcp.zhongyouzk.top

[U35] Py：发送邮件
来源：http://zcn.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kgi.xuetiantiany.cn

[U36] Py：定时任务
来源：http://gpl.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://pka.yuanzhike.top

[U37] Py：读写 Excel
来源：http://cnh.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://gbz.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://tju.tianlin.xyz

Path(__file__).resolve().parent
来源：http://mso.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://slw.feifeiyinyue.top

sys.stdout.isatty()
来源：http://zfy.vehdjk.com

[U40] Py：打印到标准错误
来源：http://grv.yj202588.top

print("err", file=sys.stderr)
来源：http://qht.nanxuanxn.top

[U41] PHP：初始化 Composer 项目
来源：http://cwz.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zaf.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://onq.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://str.mhx1999.top

[U43] PHP：声明命名空间
来源：http://fbk.chenlongwang.top

namespace App\Http;
来源：http://vhf.zdqjudy.top

[U44] PHP：开启严格类型
来源：http://xwj.cucudq.cn

declare(strict_types=1);
来源：http://azs.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://zji.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://buw.hesvh.cn

[U46] PHP：可空类型
来源：http://ooy.hfpthk.cn

?string $name = null
来源：http://quc.ydzc1.top

[U47] PHP：联合类型
来源：http://vno.jinqigufen.top

int|string $id
来源：http://wnf.zdqjudy.top

[U48] PHP：纯枚举
来源：http://xsx.cheryme.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jiq.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://pfu.yvedp.cn

public readonly string $name
来源：http://qnw.hammf.cn

[U50] PHP：构造器属性提升
来源：http://ouz.cdnleiting.top

public function __construct(private int $id) {}
来源：http://fye.pengpengdd.cyou

[U51] PHP：数组解构
来源：http://kqf.chenzaomai.com

[$a, $b] = $arr;
来源：http://btc.yueranfly.top

[U52] PHP：箭头函数
来源：http://him.shanyushiyangtech.top

$double = fn($x) => $x * 2;
来源：http://cht.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://fcr.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://opu.hfpthk.cn

[U54] PHP：空安全调用
来源：http://xrb.shzxlz.cn

$obj?->method()
来源：http://lzy.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://fvz.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sfi.ydjk.org.cn

[U56] PHP：命名参数
来源：http://fft.cheryme.top

f(a: 1, b: 2)
来源：http://wsq.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://rrg.zhixingplan.top

"值: {$a}"
来源：http://zma.bjfxy.top

[U58] PHP：数组三件套
来源：http://mlw.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zod.wangdashe.top

[U59] PHP：自定义排序
来源：http://dws.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ukl.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://pkd.hywenlv.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qom.yangfankeji.com

[U61] PHP：正则
来源：http://qtb.bjfxy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eum.nanxuanxn.top

[U62] PHP：日期对象
来源：http://baa.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mcd.tian-w.cn

[U63] PHP：文件读写
来源：http://efm.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://one.zhixingplan.top

[U64] PHP：目录遍历
来源：http://dod.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://btg.nanxuanxn.top

[U65] PHP：会话
来源：http://xkl.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://eux.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://ngy.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vzf.cdnleiting.top

[U67] PHP：处理文件上传
来源：http://jda.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kwr.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://zwd.gogol.net.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xam.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://kal.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kpn.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://wie.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wft.yvedp.cn

[U71] PHP：抛出异常
来源：http://eip.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://hyj.zycfv.cn

[U72] PHP：写错误日志
来源：http://abl.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://yel.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://yqc.vqdsnc.cn

parse_ini_file("config.ini", true)
来源：http://nff.shuidangran.top

[U74] PHP：读取环境变量
来源：http://faf.xuanzx.com

getenv("APP_ENV") ?: "production"
来源：http://ajp.vehdjk.com

[U75] PHP：依赖注入
来源：http://jmo.birdmap.top

composer require psr/container
来源：http://dge.cqqwz.cn

[U76] PHP：简单路由
来源：http://fxq.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xqw.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://gjk.316326.xyz

composer require twig/twig
来源：http://may.hnxiangtu.top

[U78] PHP：单元测试
来源：http://gxq.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://hvz.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://ztl.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://mbw.sweek.top

[U80] PHP：代码规范修复
来源：http://syg.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://cda.zycfv.cn

[U81] JS：初始化项目
来源：http://zhi.aibaodan.cn

npm init -y;  npm i express
来源：http://kqs.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://tkg.guannengcc.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://slu.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://urq.iojbl.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xun.gogol.net.cn

[U84] JS：CommonJS 写法
来源：http://wnv.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://jil.birdmap.top

[U85] JS：可选链
来源：http://gdk.cucudq.cn

a?.b?.c
来源：http://nzz.birdmap.top

[U86] JS：空值合并
来源：http://gjg.pengpengdd.cyou

a ?? b
来源：http://ama.zdqjudy.top

[U87] JS：解构默认值
来源：http://gce.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://qoe.ivvv.top

[U88] JS：对象展开合并
来源：http://edi.hcnkem.com

{ ...a, ...b }
来源：http://unm.dianchejie.cn

[U89] JS：数组去重
来源：http://tup.ivvv.top

[...new Set(arr)]
来源：http://qfb.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://bqg.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://iwz.meibo888.top

[U91] JS：对象键值遍历
来源：http://hjq.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eid.hnxiangtu.top

[U92] JS：深拷贝
来源：http://dir.andypj.xyz

structuredClone(obj)
来源：http://gtv.hnxiangtu.top

[U93] JS：模板字符串
来源：http://jqq.wangshuangyany.cn

`共 ${n} 条`
来源：http://bem.sxryk.cn

[U94] JS：箭头函数
来源：http://gme.tarul.cn

const double = x => x * 2;
来源：http://czf.ydjk.org.cn

[U95] JS：Promise 包装
来源：http://vix.316326.xyz

new Promise((resolve, reject) => {})
来源：http://nhz.shuidangran.top

[U96] JS：async/await 与异常
来源：http://yic.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gmc.vehdjk.com

[U97] JS：并发请求
来源：http://jtr.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://esc.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://jpn.chenzaomai.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qqp.zycfv.cn

[U99] JS：事件监听
来源：http://pmm.haohaochexian.top

el.addEventListener("click", e => {})
来源：http://meo.jqgfzy.top

[U100] JS：DOM 查询
来源：http://vlj.daxiang520.top

document.querySelector(".item")
来源：http://muj.fengsongda.top

[U101] JS：classList 操作
来源：http://tuh.sxryk.cn

el.classList.toggle("active")
来源：http://idy.yanxiufei.cn

[U102] JS：本地存储
来源：http://vhv.tanke756.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yvo.mhx1999.top

[U103] JS：定时器
来源：http://odq.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wou.316326.xyz

[U104] JS：防抖
来源：http://clq.meibo888.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mmn.xziqi.cn

[U105] JS：节流
来源：http://ucs.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://osz.ybcxt.top

[U106] JS：日期格式化
来源：http://dyp.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ewd.haohaochexian.top

[U107] JS：数字千分位
来源：http://zbi.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://phd.sjlbkw.cn

[U108] JS：随机整数
来源：http://xok.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cfi.yuxming.cn

[U109] JS：数组分组
来源：http://qoc.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://ary.bbcook.cn

[U110] JS：数组分块
来源：http://tsk.xingfuxueyuan.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://znu.vehdjk.com

[U111] JS：对象转 Map
来源：http://pko.zycfv.cn

new Map(Object.entries(obj))
来源：http://emd.daria6918.cn

[U112] JS：字符串补位
来源：http://mbk.jiagoushi.top

"7".padStart(3, "0")
来源：http://frq.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://gme.nwbrower.top

s.replaceAll("a", "b")
来源：http://wce.dashuyun.cn

[U114] JS：JSON 深比较
来源：http://dci.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://jfk.svipenyu.cn

[U115] JS：生成 UUID
来源：http://fzu.c1oappe.top

crypto.randomUUID()
来源：http://mcr.zhixingplan.top

[U116] JS：类型检查（JSDoc）
来源：http://nqo.hnxiangtu.top

/** @param {string} name */ function f(name) {}
来源：http://xeo.c1oappe.top

[U117] JS：单元测试
来源：http://xwh.jiagoushi.top

npm i -D vitest;  npx vitest
来源：http://amp.aibaodan.cn

[U118] JS：开发服务器
来源：http://wib.yonumen.top

npm i -D vite;  npx vite
来源：http://rxk.ybcxt.top

[U119] JS：生产构建
来源：http://vnh.yfazqb.com

npx vite build
来源：http://oue.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://nnp.tianlin.xyz

import.meta.env.VITE_API_URL
来源：http://sbg.guowangkeji.top

================================================================================
来源：http://chc.tarul.cn

统计汇总
来源：http://cle.mhx1999.top

================================================================================
来源：http://oss.wangshuangyany.cn

按语言统计（条）：
来源：http://yvg.xylfe.cn

Python ......... 252
来源：http://awc.52xcode.cn

PHP ............ 252
来源：http://mky.nwbrower.top

JavaScript ..... 252
来源：http://dth.cdnleiting.top

TypeScript ..... 212
来源：http://jxf.cdnleiting.top

Java ........... 212
来源：http://jny.sufxvd.cn

Go ............. 212
来源：http://zin.chenlongwang.top

Ruby ........... 212
来源：http://jcu.daxiang520.top

C# ............. 212
来源：http://vco.yuxming.cn

C .............. 30
来源：http://liw.sweek.top

C++ ............ 30
来源：http://mrm.ctjpmb.com

SQL ............ 90
来源：http://ova.gaohongyu789.top

Bash ........... 80
来源：http://yjp.9152youxi.cn

Kotlin ......... 15
来源：http://akn.zhiwuduotai.top

Swift .......... 15
来源：http://izl.quarkkingdee.top

Lua ............ 10
来源：http://oqs.tarul.cn

Perl ........... 10
来源：http://ivn.cqqwz.cn

Scala .......... 10
来源：http://vzw.chenlongwang.top

------------------------------------
来源：http://iah.jinyuanbaomall.cn

合计 ........... 2106 条
来源：http://czp.svipenyu.cn

按章节统计：
来源：http://emw.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yrj.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://klm.redwolf501.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://igy.iojbl.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gbs.jinqigfzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ltv.xuanzx.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wvm.zycfv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tqv.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fwp.havefunace.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iyq.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zme.gaohongyu789.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hea.nanxinkj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qwp.chenlongwang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uhz.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wpw.epnwcf.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qfw.hysaishi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ffe.cqqwz.cn

Q SQL 专题                              90
来源：http://yoa.aizwys.cn

R Bash 专题                             80
来源：http://jwm.fehbvm.com

S C / C++ 专题                          60
来源：http://hxq.hysaishi.cn

T 其他语言补充                          60
来源：http://amb.sufxvd.cn

U 高频实用片段                         120
来源：http://she.ybcxt.top

------------------------------------
来源：http://lpd.hnqzz.top

合计                                  2106 条
来源：http://bev.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://uoh.ppjwa.cn

使用提醒
来源：http://ohe.pycfn.com

--------------------------------------------------------------------------------
来源：http://yth.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://psk.uphjek.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fyn.gzhubu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://czv.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lzr.316326.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sth.zdqjudy.top

—— 文件结束 ——
来源：http://iib.zdbjq.cn

================================================================================
来源：http://ylr.hywenlv.cn

程序语言常见例子速查手册（2024 版）
来源：http://btm.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://bhh.tian-w.cn

================================================================================
来源：http://cpa.ctjpmb.com

【收录内容】
来源：http://rde.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zhh.wangshuangyany.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kkb.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://dnj.pengpengdd.cyou


<!-- 参考信息 -->