代发 wailian999

[U13] Py：固定长度队列
来源：http://thu.yuanzhike.top

deque(maxlen=10)
来源：http://wbk.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://puj.nanxuanxn.top

defaultdict(list)
来源：http://wom.kuanghao11.cn

[U15] Py：高精度计时
来源：http://ked.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://zib.iojbl.cn

[U16] Py：命令行参数解析
来源：http://udb.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wze.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://wmj.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://xoa.sysykeji.top

[U18] Py：预编译正则
来源：http://rcd.fzhhl.top

pat = re.compile(r"\d+")
来源：http://iml.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://iux.xylfe.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hda.316326.xyz

[U20] Py：缓存函数结果
来源：http://uij.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://yzm.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://xmh.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://bow.tarul.cn

[U22] Py：矩阵转置
来源：http://hvb.xinyue.icu

list(zip(*m))
来源：http://glv.fktsv.cn

[U23] Py：分块读取大文件
来源：http://qvi.hcnkem.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fot.gaohongyu789.top

[U24] Py：路径操作
来源：http://xyk.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ezq.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://ioe.ppjwa.cn

csv.DictReader(f)
来源：http://isb.zhixingplan.top

[U26] Py：并发下载
来源：http://hkd.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fnv.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://vtl.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://ipp.xinyue.icu

[U28] Py：类型别名
来源：http://rjv.hfpthk.cn

UserId = int
来源：http://ggu.vehdjk.com

[U29] Py：属性校验
来源：http://wam.chenlongwang.top

@property 与 @x.setter 配合
来源：http://taj.hongshengwenyu.top

[U30] Py：数据类
来源：http://ang.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://khm.sxryk.cn

[U31] Py：单测
来源：http://abn.havefunace.top

python -m pytest -q
来源：http://rdz.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://hxc.tanke756.top

ruff format . && ruff check --fix .
来源：http://bxo.yongpay.top

[U33] Py：打包发布
来源：http://ibp.hfpthk.cn

python -m build  （依赖 pyproject.toml）
来源：http://orx.hnqzz.top

[U34] Py：判断编码
来源：http://zdi.chenjidiqi.icu

chardet.detect(raw)
来源：http://ksg.hongshengwenyu.top

[U35] Py：发送邮件
来源：http://otb.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xsa.yongpay.top

[U36] Py：定时任务
来源：http://nun.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://juy.hywenlv.cn

[U37] Py：读写 Excel
来源：http://huu.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ezh.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://ias.0kj1m.cn

Path(__file__).resolve().parent
来源：http://nfl.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://ohm.ivvv.top

sys.stdout.isatty()
来源：http://bai.xziqi.cn

[U40] Py：打印到标准错误
来源：http://mmu.yj202588.top

print("err", file=sys.stderr)
来源：http://wex.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://boa.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://syp.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://emn.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uln.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://gdc.haohaochexian.top

namespace App\Http;
来源：http://jqt.bbcook.cn

[U44] PHP：开启严格类型
来源：http://hzy.xziqi.cn

declare(strict_types=1);
来源：http://koi.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://dwi.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://eug.hongshengwenyu.top

[U46] PHP：可空类型
来源：http://pca.shuidangran.top

?string $name = null
来源：http://bjk.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://uxv.nanxinkj.top

int|string $id
来源：http://avm.redwolf501.top

[U48] PHP：纯枚举
来源：http://nze.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdk.mhx1999.top

[U49] PHP：只读属性
来源：http://vpt.sxryk.cn

public readonly string $name
来源：http://grc.cashguo.top

[U50] PHP：构造器属性提升
来源：http://agg.gzhubu.top

public function __construct(private int $id) {}
来源：http://ilg.uphjek.com

[U51] PHP：数组解构
来源：http://aed.ppjwa.cn

[$a, $b] = $arr;
来源：http://aoq.wangdashe.top

[U52] PHP：箭头函数
来源：http://uyp.jinqigfzy.top

$double = fn($x) => $x * 2;
来源：http://dxs.sxryk.cn

[U53] PHP：空合并运算符
来源：http://lvw.gzhubu.top

$v = $a ?? $b ?? "default";
来源：http://trb.dianchejie.cn

[U54] PHP：空安全调用
来源：http://yda.xingfuxueyuan.xyz

$obj?->method()
来源：http://zzl.sufxvd.cn

[U55] PHP：match 表达式
来源：http://arr.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vei.wangdashe.top

[U56] PHP：命名参数
来源：http://akr.cqqwz.cn

f(a: 1, b: 2)
来源：http://bij.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://zao.daria6918.cn

"值: {$a}"
来源：http://znq.xingfuxueyuan.xyz

[U58] PHP：数组三件套
来源：http://cqp.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jml.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://auf.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gsz.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://urh.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zdt.zycfv.cn

[U61] PHP：正则
来源：http://rjd.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ama.iojbl.cn

[U62] PHP：日期对象
来源：http://pfm.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://alp.hywenlv.cn

[U63] PHP：文件读写
来源：http://vem.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wvo.cheryme.top

[U64] PHP：目录遍历
来源：http://hgx.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://vfq.havefunace.top

[U65] PHP：会话
来源：http://xjf.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mus.c1oappe.top

[U66] PHP：设置 Cookie
来源：http://kle.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ekm.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://ysn.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tvd.yueranfly.top

[U68] PHP：PDO 连接
来源：http://xjb.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://thv.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://age.wangshuangyany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://prj.wangshuangyany.cn

[U70] PHP：PDO 事务
来源：http://gnj.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jka.bbcook.cn

[U71] PHP：抛出异常
来源：http://dlq.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://tpp.andypj.xyz

[U72] PHP：写错误日志
来源：http://ofj.hnqzz.top

error_log("失败: " . $e->getMessage());
来源：http://ney.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://ynm.yongpay.top

parse_ini_file("config.ini", true)
来源：http://xdb.yueranfly.top

[U74] PHP：读取环境变量
来源：http://wfc.vqdsnc.cn

getenv("APP_ENV") ?: "production"
来源：http://ymk.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://mdf.iojbl.cn

composer require psr/container
来源：http://urj.yanxiufei.cn

[U76] PHP：简单路由
来源：http://dal.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xuz.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://vwh.ywan-chungtsiang.top

composer require twig/twig
来源：http://wuh.hnqzz.top

[U78] PHP：单元测试
来源：http://wia.316326.xyz

composer require --dev phpunit/phpunit
来源：http://yxh.nwbrower.top

[U79] PHP：静态分析
来源：http://hdl.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://ncp.yanxiufei.cn

[U80] PHP：代码规范修复
来源：http://jge.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ikf.zdqjudy.top

[U81] JS：初始化项目
来源：http://xgw.sxryk.cn

npm init -y;  npm i express
来源：http://iaj.meibo888.top

[U82] JS：package.json 脚本
来源：http://aog.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fvp.zhongyouzk.top

[U83] JS：ES Module 导入导出
来源：http://pys.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://wsi.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://xla.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ryr.yuxming.cn

[U85] JS：可选链
来源：http://jsr.jqgufenzy.top

a?.b?.c
来源：http://tax.xinyue.icu

[U86] JS：空值合并
来源：http://stg.fengsongda.top

a ?? b
来源：http://lia.svipenyu.cn

[U87] JS：解构默认值
来源：http://wuq.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://igg.zhengqikj.top

[U88] JS：对象展开合并
来源：http://uhi.shuidangran.top

{ ...a, ...b }
来源：http://rtn.uphjek.com

[U89] JS：数组去重
来源：http://qjw.xinyue.icu

[...new Set(arr)]
来源：http://ofr.aizwys.cn

[U90] JS：数字数组排序
来源：http://aqv.tianlin.xyz

[...arr].sort((a, b) => a - b)
来源：http://lkg.zhoulong.xyz

[U91] JS：对象键值遍历
来源：http://aju.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mdy.gaohongyu789.top

[U92] JS：深拷贝
来源：http://zps.tanke756.top

structuredClone(obj)
来源：http://gnl.fengsongda.top

[U93] JS：模板字符串
来源：http://ocz.xylfe.cn

`共 ${n} 条`
来源：http://spr.yj202588.top

[U94] JS：箭头函数
来源：http://otx.yongpay.top

const double = x => x * 2;
来源：http://him.fengsongda.top

[U95] JS：Promise 包装
来源：http://spn.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://wid.gzhubu.top

[U96] JS：async/await 与异常
来源：http://ffv.shuidangran.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dao.gzhubu.top

[U97] JS：并发请求
来源：http://wfy.c1oappe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oez.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://tqx.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uvf.bjfxy.top

[U99] JS：事件监听
来源：http://epq.shanyushiyangtech.top

el.addEventListener("click", e => {})
来源：http://zua.fzhhl.top

[U100] JS：DOM 查询
来源：http://mwg.jiagoushi.top

document.querySelector(".item")
来源：http://mrj.vqdsnc.cn

[U101] JS：classList 操作
来源：http://cnt.yj20258888.top

el.classList.toggle("active")
来源：http://bdi.9152youxi.cn

[U102] JS：本地存储
来源：http://elw.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jnz.hnxiangtu.top

[U103] JS：定时器
来源：http://zaz.cucudq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xos.xuanzx.com

[U104] JS：防抖
来源：http://ghm.jlsjyb.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bqq.snrcjt.cn

[U105] JS：节流
来源：http://mdu.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kyc.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://eeg.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ime.sysykeji.top

[U107] JS：数字千分位
来源：http://uqm.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xip.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://arx.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gvx.wangdashe.top

[U109] JS：数组分组
来源：http://pxj.gotoacloud.top

Object.groupBy(arr, x => x.type)
来源：http://rzb.ehwqpu.com

[U110] JS：数组分块
来源：http://xmh.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eot.xziqi.cn

[U111] JS：对象转 Map
来源：http://cng.zhiwuduotai.top

new Map(Object.entries(obj))
来源：http://ngs.zhixingplan.top

[U112] JS：字符串补位
来源：http://gdn.chenlongwang.top

"7".padStart(3, "0")
来源：http://acl.ppjwa.cn

[U113] JS：正则替换全部
来源：http://uwy.bjfxy.top

s.replaceAll("a", "b")
来源：http://ptb.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://jvs.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jir.52xcode.cn

[U115] JS：生成 UUID
来源：http://pbp.zdbjq.cn

crypto.randomUUID()
来源：http://qwl.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://bsa.ybcxt.top

/** @param {string} name */ function f(name) {}
来源：http://zyp.chenzaomai.com

[U117] JS：单元测试
来源：http://rcn.hesvh.cn

npm i -D vitest;  npx vitest
来源：http://soo.hnqzz.top

[U118] JS：开发服务器
来源：http://rev.nanxinkj.top

npm i -D vite;  npx vite
来源：http://kbw.jinqigfzy.top

[U119] JS：生产构建
来源：http://zso.jyoumei.cn

npx vite build
来源：http://jsn.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://tsw.hnxiangtu.top

import.meta.env.VITE_API_URL
来源：http://jrb.hywenlv.cn

================================================================================
来源：http://vtz.cucudq.cn

统计汇总
来源：http://lwk.bjfxy.top

================================================================================
来源：http://jqm.zhoulong.xyz

按语言统计（条）：
来源：http://psn.zhixingplan.top

Python ......... 252
来源：http://wgl.sufxvd.cn

PHP ............ 252
来源：http://vjw.cdnleiting.top

JavaScript ..... 252
来源：http://uxz.jinghuilouyu.cn

TypeScript ..... 212
来源：http://kai.wangdashe.top

Java ........... 212
来源：http://pvy.xuetiantiany.cn

Go ............. 212
来源：http://ulf.zdbjq.cn

Ruby ........... 212
来源：http://ktf.cashguo.top

C# ............. 212
来源：http://pvq.fehbvm.com

C .............. 30
来源：http://fbh.yuanzhike.top

C++ ............ 30
来源：http://srd.shzxlz.cn

SQL ............ 90
来源：http://dsd.chenjidiqi.icu

Bash ........... 80
来源：http://lhj.pycfn.com

Kotlin ......... 15
来源：http://fjc.cdnleiting.top

Swift .......... 15
来源：http://afm.yuxming.cn

Lua ............ 10
来源：http://wwo.jinqigufen.top

Perl ........... 10
来源：http://dxs.yj20258.top

Scala .......... 10
来源：http://sbw.zhijiandao.cn

------------------------------------
来源：http://rwb.vehdjk.com

合计 ........... 2106 条
来源：http://kfe.iojbl.cn

按章节统计：
来源：http://fda.hammf.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lio.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kbi.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vsv.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jhu.cqqwz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uix.guannengcc.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zrs.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zor.ivvv.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oeg.haohaochexian.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qkg.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xyb.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ehy.jinqigfzy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hnv.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fkt.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nbf.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jte.ppjwa.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mxl.xziqi.cn

Q SQL 专题                              90
来源：http://nwp.daria6918.cn

R Bash 专题                             80
来源：http://myo.cashguo.top

S C / C++ 专题                          60
来源：http://srd.xinyue.icu

T 其他语言补充                          60
来源：http://uap.pengpengdd.cyou

U 高频实用片段                         120
来源：http://abh.fehbvm.com

------------------------------------
来源：http://exx.zhaomingkeji.xyz

合计                                  2106 条
来源：http://anu.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://jqq.zhongyouzk.top

使用提醒
来源：http://zgy.zdqjudy.top

--------------------------------------------------------------------------------
来源：http://tec.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sue.sweek.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://egz.jyoumei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vza.ivvv.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eie.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sqo.ybcxt.top

—— 文件结束 ——
来源：http://ign.epnwcf.com

================================================================================
来源：http://cfy.tarul.cn

程序语言常见例子速查手册（2024 版）
来源：http://ilr.fktsv.cn

Common Programming Examples Cheat Book
来源：http://trb.epnwcf.com

================================================================================
来源：http://hjb.bjfxy.top

【收录内容】
来源：http://oeq.sjlbkw.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zlr.hfpthk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://btz.iojbl.cn

SQL · Bash · C · C++
来源：http://mac.cqqwz.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nns.316326.xyz

【使用说明】
来源：http://izm.ydzc1.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ihz.jianghu66.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://glb.gaohongyu789.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rvo.nwbrower.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ant.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fih.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aaa.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mmh.fehbvm.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xol.jinghuilouyu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aow.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ckh.tarul.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ouj.shuidangran.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bok.gaohongyu789.top

【文件统计】
来源：http://elz.gzhubu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eei.316326.xyz

--------------------------------------------------------------------------------
来源：http://afs.jqgfzy.top

目  录
来源：http://xff.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://qsj.zhoulong.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rql.jinyuanbaomall.cn


<!-- 参考信息 -->