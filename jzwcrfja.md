代发 wailian999

[U09] Py：字典取最大值的键
来源：http://ugg.haohaochexian.top

max(d, key=d.get)
来源：http://jhz.cqqwz.cn

[U10] Py：按值排序字典
来源：http://wpn.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aic.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://msx.tanke756.top

(x * 2 for x in arr)
来源：http://kia.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://hey.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://pto.nwbrower.top

[U13] Py：固定长度队列
来源：http://gzt.zdbjq.cn

deque(maxlen=10)
来源：http://hno.smart0.xyz

[U14] Py：分组收集到列表
来源：http://csf.cheryme.top

defaultdict(list)
来源：http://qiu.jinqigfzy.top

[U15] Py：高精度计时
来源：http://wvf.nwbrower.top

t = time.perf_counter()
来源：http://kxv.xinyue.icu

[U16] Py：命令行参数解析
来源：http://ics.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zcc.9152youxi.cn

[U17] Py：初始化日志
来源：http://iea.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://eby.c1oappe.top

[U18] Py：预编译正则
来源：http://kar.0kj1m.cn

pat = re.compile(r"\d+")
来源：http://rkk.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://qwh.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://noh.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://jpm.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://nax.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://mgp.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://fuc.yuanzhike.top

[U22] Py：矩阵转置
来源：http://vrv.zhixingplan.top

list(zip(*m))
来源：http://mri.guannengcc.top

[U23] Py：分块读取大文件
来源：http://uiu.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cqi.gzhubu.top

[U24] Py：路径操作
来源：http://xcq.kuanghao11.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gir.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://ddw.andypj.xyz

csv.DictReader(f)
来源：http://ghf.xuetiantiany.cn

[U26] Py：并发下载
来源：http://atc.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wvl.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://bun.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://uqd.uphjek.com

[U28] Py：类型别名
来源：http://chy.ehwqpu.com

UserId = int
来源：http://lbf.redwolf501.top

[U29] Py：属性校验
来源：http://umk.ywan-chungtsiang.top

@property 与 @x.setter 配合
来源：http://dgl.zhijiandao.cn

[U30] Py：数据类
来源：http://bve.yfazqb.com

@dataclass(slots=True)
来源：http://nsg.jinqigufen.top

[U31] Py：单测
来源：http://fsa.snrcjt.cn

python -m pytest -q
来源：http://tug.bbcook.cn

[U32] Py：代码格式化
来源：http://vvu.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://xww.chenzaomai.com

[U33] Py：打包发布
来源：http://hiv.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://hlr.nanxinkj.top

[U34] Py：判断编码
来源：http://snj.hfpthk.cn

chardet.detect(raw)
来源：http://ebp.yuanzhike.top

[U35] Py：发送邮件
来源：http://ubf.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ika.vehdjk.com

[U36] Py：定时任务
来源：http://stt.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://dul.jiagoushi.top

[U37] Py：读写 Excel
来源：http://mfq.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ttv.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://ykj.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://bpi.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://fzg.fengsongda.top

sys.stdout.isatty()
来源：http://zkv.hammf.cn

[U40] Py：打印到标准错误
来源：http://qvd.hammf.cn

print("err", file=sys.stderr)
来源：http://qwt.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://mlg.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vhu.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://yyv.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fdy.tanke756.top

[U43] PHP：声明命名空间
来源：http://gcz.hesvh.cn

namespace App\Http;
来源：http://fgo.xuanzx.com

[U44] PHP：开启严格类型
来源：http://kfb.hnqzz.top

declare(strict_types=1);
来源：http://dgf.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://vvx.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ygl.svipenyu.cn

[U46] PHP：可空类型
来源：http://koy.gotoacloud.top

?string $name = null
来源：http://vjp.yuxming.cn

[U47] PHP：联合类型
来源：http://vzn.hongshengwenyu.top

int|string $id
来源：http://vaw.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://pku.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zzm.c1oappe.top

[U49] PHP：只读属性
来源：http://hjl.kuanghao11.cn

public readonly string $name
来源：http://gdo.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://uap.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://pfn.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://qby.hnqzz.top

[$a, $b] = $arr;
来源：http://tze.jiagoushi.top

[U52] PHP：箭头函数
来源：http://agu.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://ulp.ywan-chungtsiang.top

[U53] PHP：空合并运算符
来源：http://cpm.xziqi.cn

$v = $a ?? $b ?? "default";
来源：http://gns.yanxiufei.cn

[U54] PHP：空安全调用
来源：http://aap.zhengqikj.top

$obj?->method()
来源：http://hlb.yvedp.cn

[U55] PHP：match 表达式
来源：http://bkw.chenjidiqi.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lit.ydzc1.top

[U56] PHP：命名参数
来源：http://wbt.chenlongwang.top

f(a: 1, b: 2)
来源：http://wrl.chenzaomai.com

[U57] PHP：字符串插值
来源：http://izs.fengsongda.top

"值: {$a}"
来源：http://rip.zhixingplan.top

[U58] PHP：数组三件套
来源：http://upz.epnwcf.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://saz.fehbvm.com

[U59] PHP：自定义排序
来源：http://lrl.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wre.chenjidiqi.icu

[U60] PHP：JSON 编解码
来源：http://ppp.ehwqpu.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xah.sysykeji.top

[U61] PHP：正则
来源：http://tdk.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nik.shuidangran.top

[U62] PHP：日期对象
来源：http://efx.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ajw.yj20258.top

[U63] PHP：文件读写
来源：http://fuy.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pmy.cashguo.top

[U64] PHP：目录遍历
来源：http://wvk.xuanzx.com

glob("dir/*.php");  scandir("dir");
来源：http://pxx.meibo888.top

[U65] PHP：会话
来源：http://oue.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iow.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://sso.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rvr.pycfn.com

[U67] PHP：处理文件上传
来源：http://rrx.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sbi.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://bou.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dke.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://pan.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://evh.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://gwk.zhijiandao.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mwx.jlsjyb.cn

[U71] PHP：抛出异常
来源：http://oty.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://wxx.ybcxt.top

[U72] PHP：写错误日志
来源：http://vuy.tanke756.top

error_log("失败: " . $e->getMessage());
来源：http://nfd.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://nqu.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://ufm.mhx1999.top

[U74] PHP：读取环境变量
来源：http://kgn.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://ols.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://vnr.chenjidiqi.icu

composer require psr/container
来源：http://sje.yanxiufei.cn

[U76] PHP：简单路由
来源：http://bcf.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dyz.fzhhl.top

[U77] PHP：模板渲染
来源：http://zsx.havefunace.top

composer require twig/twig
来源：http://vgl.tian-w.cn

[U78] PHP：单元测试
来源：http://sxy.ivvv.top

composer require --dev phpunit/phpunit
来源：http://ctf.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://hhg.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://rrl.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://nci.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tzs.sweek.top

[U81] JS：初始化项目
来源：http://rcj.snrcjt.cn

npm init -y;  npm i express
来源：http://fzk.cashguo.top

[U82] JS：package.json 脚本
来源：http://aac.9152youxi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://axz.jianghu66.top

[U83] JS：ES Module 导入导出
来源：http://ivk.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://uoa.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://vhy.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xpg.yueranfly.top

[U85] JS：可选链
来源：http://far.hywenlv.cn

a?.b?.c
来源：http://som.nanxinkj.top

[U86] JS：空值合并
来源：http://owb.yonumen.top

a ?? b
来源：http://cmx.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://mno.jinqigufen.top

const { a = 1, b = 2 } = obj;
来源：http://iox.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://kuu.shangyingyoupin.top

{ ...a, ...b }
来源：http://mfw.fktsv.cn

[U89] JS：数组去重
来源：http://lgo.0kj1m.cn

[...new Set(arr)]
来源：http://ssq.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://ozt.fzhhl.top

[...arr].sort((a, b) => a - b)
来源：http://ayq.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://ogx.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vrk.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://ate.smart0.xyz

structuredClone(obj)
来源：http://sqo.zhixingplan.top

[U93] JS：模板字符串
来源：http://ibn.shzxlz.cn

`共 ${n} 条`
来源：http://gey.bjfxy.top

[U94] JS：箭头函数
来源：http://tlq.yuanzhike.top

const double = x => x * 2;
来源：http://hpy.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://vbw.sufxvd.cn

new Promise((resolve, reject) => {})
来源：http://qzx.yj20258888.top

[U96] JS：async/await 与异常
来源：http://urr.hysaishi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ocg.yfazqb.com

[U97] JS：并发请求
来源：http://wkh.nanxinkj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oha.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://ljk.jinghuilouyu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pvn.0kj1m.cn

[U99] JS：事件监听
来源：http://zex.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://yix.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://nog.yj202588.top

document.querySelector(".item")
来源：http://izw.gotoacloud.top

[U101] JS：classList 操作
来源：http://dix.yvedp.cn

el.classList.toggle("active")
来源：http://lbs.hesvh.cn

[U102] JS：本地存储
来源：http://bsx.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://lfb.fengsongda.top

[U103] JS：定时器
来源：http://vot.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bee.jinyuanbaomall.cn

[U104] JS：防抖
来源：http://pwg.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdh.guowangkeji.top

[U105] JS：节流
来源：http://dur.zycfv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pss.aizwys.cn

[U106] JS：日期格式化
来源：http://oll.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xuk.shuidangran.top

[U107] JS：数字千分位
来源：http://dgw.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://aha.smart0.xyz

[U108] JS：随机整数
来源：http://gxl.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iqa.cheryme.top

[U109] JS：数组分组
来源：http://pit.ydzc1.top

Object.groupBy(arr, x => x.type)
来源：http://jcj.sjlbkw.cn

[U110] JS：数组分块
来源：http://qjf.vehdjk.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hox.ydzc1.top

[U111] JS：对象转 Map
来源：http://okf.fanxiaobao.xyz

new Map(Object.entries(obj))
来源：http://nxh.0kj1m.cn

[U112] JS：字符串补位
来源：http://kkm.hammf.cn

"7".padStart(3, "0")
来源：http://ppz.zhijiandao.cn

[U113] JS：正则替换全部
来源：http://zez.yueranfly.top

s.replaceAll("a", "b")
来源：http://hxw.gaohongyu789.top

[U114] JS：JSON 深比较
来源：http://tbl.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ozk.pycfn.com

[U115] JS：生成 UUID
来源：http://plz.ivvv.top

crypto.randomUUID()
来源：http://ybb.gotoacloud.top

[U116] JS：类型检查（JSDoc）
来源：http://vwy.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://ytq.guowangkeji.top

[U117] JS：单元测试
来源：http://eyu.fengsongda.top

npm i -D vitest;  npx vitest
来源：http://ohm.yj20258.top

[U118] JS：开发服务器
来源：http://ijv.xuanzx.com

npm i -D vite;  npx vite
来源：http://utb.pengpengdd.cyou

[U119] JS：生产构建
来源：http://cuh.tian-w.cn

npx vite build
来源：http://okj.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://znr.hammf.cn

import.meta.env.VITE_API_URL
来源：http://hbu.cdnleiting.top

================================================================================
来源：http://ouf.yfazqb.com

统计汇总
来源：http://wuj.wangshuangyany.cn

================================================================================
来源：http://jcz.cheryme.top

按语言统计（条）：
来源：http://xmo.svipenyu.cn

Python ......... 252
来源：http://msc.yj202588.top

PHP ............ 252
来源：http://bdz.nwbrower.top

JavaScript ..... 252
来源：http://gtp.cashguo.top

TypeScript ..... 212
来源：http://cew.yj202588.top

Java ........... 212
来源：http://lxq.hesvh.cn

Go ............. 212
来源：http://fad.jinghuilouyu.cn

Ruby ........... 212
来源：http://vku.yj20258888.top

C# ............. 212
来源：http://oqb.birdmap.top

C .............. 30
来源：http://uzm.sweek.top

C++ ............ 30
来源：http://omu.jianghu66.top

SQL ............ 90
来源：http://bkc.chenzaomai.com

Bash ........... 80
来源：http://wgt.dashuyun.cn

Kotlin ......... 15
来源：http://yqr.jinyuanbaomall.cn

Swift .......... 15
来源：http://xbt.cashguo.top

Lua ............ 10
来源：http://bla.hesvh.cn

Perl ........... 10
来源：http://ivr.aizwys.cn

Scala .......... 10
来源：http://bes.nanxuanxn.top

------------------------------------
来源：http://tpq.vehdjk.com

合计 ........... 2106 条
来源：http://xcj.vqdsnc.cn

按章节统计：
来源：http://ayf.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zmt.jiagoushi.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lfd.cheryme.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://isj.nwbrower.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xbv.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tiw.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tfs.pycfn.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://njx.haohaochexian.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://iib.jinyuanbaomall.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://grh.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jod.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ohs.52xcode.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qih.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lap.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rhq.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vkf.xuanzx.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hyd.daxiang520.top

Q SQL 专题                              90
来源：http://nkz.chenzaomai.com

R Bash 专题                             80
来源：http://vgz.hywenlv.cn

S C / C++ 专题                          60
来源：http://muq.jinqigufen.top

T 其他语言补充                          60
来源：http://mhb.shzxlz.cn

U 高频实用片段                         120
来源：http://ueu.xinyue.icu

------------------------------------
来源：http://akh.redwolf501.top

合计                                  2106 条
来源：http://cyt.chenjidiqi.icu

--------------------------------------------------------------------------------
来源：http://mgp.jinqigufen.top

使用提醒
来源：http://wgh.jianghu66.top

--------------------------------------------------------------------------------
来源：http://hco.zhixingplan.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xkd.jlsjyb.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rmd.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://loq.tarul.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mbv.yangfankeji.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oib.quarkkingdee.top

—— 文件结束 ——
来源：http://kgj.ehwqpu.com

================================================================================
来源：http://rmx.zhijiandao.cn

程序语言常见例子速查手册（2024 版）
来源：http://mky.zhengqikj.top

Common Programming Examples Cheat Book
来源：http://zld.ctjpmb.com

================================================================================
来源：http://dju.tianlin.xyz

【收录内容】
来源：http://udg.fengsongda.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://nym.snrcjt.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://egg.jqgufenzy.top

SQL · Bash · C · C++
来源：http://iqo.sweek.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fif.fktsv.cn

【使用说明】
来源：http://fwa.yuanzhike.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hau.andypj.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yqr.andypj.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ecp.hnxiangtu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wkn.wangshuangyany.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lqv.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mmh.cucudq.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pmx.9152youxi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cms.hesvh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://igc.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zhi.sxryk.cn


<!-- 参考信息 -->