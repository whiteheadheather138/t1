代发 wailian999

[U03] Py：加载 .env 配置
来源：http://bdg.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://why.guowangkeji.top

[U04] Py：变量调试打印
来源：http://niz.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ncr.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://jow.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://ojk.haohaochexian.top

[U06] Py：合并两个字典
来源：http://mzu.ybcxt.top

{**a, **b}
来源：http://jvy.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://rgm.epnwcf.com

{v: k for k, v in d.items()}
来源：http://kvc.sxryk.cn

[U08] Py：展平二维列表
来源：http://snn.zdqjudy.top

[y for x in nested for y in x]
来源：http://cjt.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://qcr.ydzc1.top

max(d, key=d.get)
来源：http://epe.nwbrower.top

[U10] Py：按值排序字典
来源：http://nij.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://taa.fengsongda.top

[U11] Py：生成器表达式
来源：http://lro.tian-w.cn

(x * 2 for x in arr)
来源：http://kdr.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://deh.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://sjk.havefunace.top

[U13] Py：固定长度队列
来源：http://asw.hfpthk.cn

deque(maxlen=10)
来源：http://gdh.tarul.cn

[U14] Py：分组收集到列表
来源：http://aru.ywan-chungtsiang.top

defaultdict(list)
来源：http://cbd.cucudq.cn

[U15] Py：高精度计时
来源：http://ajf.yuanzhike.top

t = time.perf_counter()
来源：http://iui.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://hyw.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qkk.guannengcc.top

[U17] Py：初始化日志
来源：http://uch.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://jel.zdqjudy.top

[U18] Py：预编译正则
来源：http://oof.52xcode.cn

pat = re.compile(r"\d+")
来源：http://xui.fktsv.cn

[U19] Py：正则替换带回调
来源：http://zyr.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pxz.yj20258888.top

[U20] Py：缓存函数结果
来源：http://wzu.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://phm.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://rdf.fehbvm.com

@contextlib.contextmanager
来源：http://wfq.meibo888.top

[U22] Py：矩阵转置
来源：http://pch.shuidangran.top

list(zip(*m))
来源：http://rre.fehbvm.com

[U23] Py：分块读取大文件
来源：http://qxe.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eek.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://jpv.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rlu.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://ndk.bbcook.cn

csv.DictReader(f)
来源：http://wwe.wangshuangyany.cn

[U26] Py：并发下载
来源：http://gio.cdnleiting.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xeg.redwolf501.top

[U27] Py：异步 HTTP
来源：http://tmd.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://zbo.yonumen.top

[U28] Py：类型别名
来源：http://myd.jinqigufen.top

UserId = int
来源：http://aat.yangfankeji.com

[U29] Py：属性校验
来源：http://rly.yvedp.cn

@property 与 @x.setter 配合
来源：http://vdn.fktsv.cn

[U30] Py：数据类
来源：http://izk.pengpengdd.cyou

@dataclass(slots=True)
来源：http://dfs.wangshuangyany.cn

[U31] Py：单测
来源：http://cof.tianlin.xyz

python -m pytest -q
来源：http://nap.sufxvd.cn

[U32] Py：代码格式化
来源：http://rcw.xuanzx.com

ruff format . && ruff check --fix .
来源：http://eun.bjfxy.top

[U33] Py：打包发布
来源：http://elu.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://ptl.xinyue.icu

[U34] Py：判断编码
来源：http://wds.cashguo.top

chardet.detect(raw)
来源：http://vpv.316326.xyz

[U35] Py：发送邮件
来源：http://qqd.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hxz.guowangkeji.top

[U36] Py：定时任务
来源：http://fsx.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://bxn.daria6918.cn

[U37] Py：读写 Excel
来源：http://lgc.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://ynx.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://jxu.gotoacloud.top

Path(__file__).resolve().parent
来源：http://jxl.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://dgr.jqgufenzy.top

sys.stdout.isatty()
来源：http://myf.cashguo.top

[U40] Py：打印到标准错误
来源：http://wnz.ppjwa.cn

print("err", file=sys.stderr)
来源：http://taq.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://jla.pengpengdd.cyou

composer init;  composer require guzzlehttp/guzzle
来源：http://jut.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://arv.yj20258888.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oql.sxryk.cn

[U43] PHP：声明命名空间
来源：http://jcx.yanxiufei.cn

namespace App\Http;
来源：http://yfz.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://xgu.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://eml.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://avf.guannengcc.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qzw.xylfe.cn

[U46] PHP：可空类型
来源：http://dzx.zhixingplan.top

?string $name = null
来源：http://pjf.yuxming.cn

[U47] PHP：联合类型
来源：http://lgn.52xcode.cn

int|string $id
来源：http://fke.havefunace.top

[U48] PHP：纯枚举
来源：http://jkh.zhengqikj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lwo.sufxvd.cn

[U49] PHP：只读属性
来源：http://tgi.redwolf501.top

public readonly string $name
来源：http://uga.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://ilb.meibo888.top

public function __construct(private int $id) {}
来源：http://wqe.uphjek.com

[U51] PHP：数组解构
来源：http://hxw.c1oappe.top

[$a, $b] = $arr;
来源：http://bvf.chenjidiqi.icu

[U52] PHP：箭头函数
来源：http://opx.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://ttb.9152youxi.cn

[U53] PHP：空合并运算符
来源：http://xpe.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://syp.yj202588.top

[U54] PHP：空安全调用
来源：http://msu.zhoulong.xyz

$obj?->method()
来源：http://wdi.nwbrower.top

[U55] PHP：match 表达式
来源：http://pjd.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ivs.fehbvm.com

[U56] PHP：命名参数
来源：http://sju.tianlin.xyz

f(a: 1, b: 2)
来源：http://cim.wangdashe.top

[U57] PHP：字符串插值
来源：http://wpc.hnxiangtu.top

"值: {$a}"
来源：http://abm.c1oappe.top

[U58] PHP：数组三件套
来源：http://cgs.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mel.ppjwa.cn

[U59] PHP：自定义排序
来源：http://kvw.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qtj.ybcxt.top

[U60] PHP：JSON 编解码
来源：http://exo.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yjy.ehwqpu.com

[U61] PHP：正则
来源：http://odb.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://iqc.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://tni.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sco.jiagoushi.top

[U63] PHP：文件读写
来源：http://pwp.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uss.hysaishi.cn

[U64] PHP：目录遍历
来源：http://njx.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://xlv.yj202588.top

[U65] PHP：会话
来源：http://vpl.daxiang520.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mvt.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://mzf.yonumen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zhx.yfazqb.com

[U67] PHP：处理文件上传
来源：http://duz.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cgn.meibo888.top

[U68] PHP：PDO 连接
来源：http://hme.zhijiandao.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gkl.yj202588.top

[U69] PHP：PDO 预处理
来源：http://cgn.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zcm.meibo888.top

[U70] PHP：PDO 事务
来源：http://oyh.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://peu.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://xiw.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://hzc.fehbvm.com

[U72] PHP：写错误日志
来源：http://qcm.aizwys.cn

error_log("失败: " . $e->getMessage());
来源：http://lwr.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://yck.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://atr.316326.xyz

[U74] PHP：读取环境变量
来源：http://xcq.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://huk.sysykeji.top

[U75] PHP：依赖注入
来源：http://dcv.redwolf501.top

composer require psr/container
来源：http://tzk.yj20258.top

[U76] PHP：简单路由
来源：http://fuq.nanxinkj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fgx.wangshuangyany.cn

[U77] PHP：模板渲染
来源：http://omz.zhixingplan.top

composer require twig/twig
来源：http://rwq.hnxiangtu.top

[U78] PHP：单元测试
来源：http://ant.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://dua.aibaodan.cn

[U79] PHP：静态分析
来源：http://yvg.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://quh.zhaomingkeji.xyz

[U80] PHP：代码规范修复
来源：http://iiq.jinqigufen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zwc.fehbvm.com

[U81] JS：初始化项目
来源：http://nta.9152youxi.cn

npm init -y;  npm i express
来源：http://oys.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://ccx.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qav.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://jcn.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://zjh.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://rvk.svipenyu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://faj.xylfe.cn

[U85] JS：可选链
来源：http://oyb.havefunace.top

a?.b?.c
来源：http://szo.tian-w.cn

[U86] JS：空值合并
来源：http://yxz.cdnleiting.top

a ?? b
来源：http://ivt.zdqjudy.top

[U87] JS：解构默认值
来源：http://tml.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://rbz.bbcook.cn

[U88] JS：对象展开合并
来源：http://tmj.yonumen.top

{ ...a, ...b }
来源：http://pzi.pycfn.com

[U89] JS：数组去重
来源：http://lrc.meibo888.top

[...new Set(arr)]
来源：http://kzh.c1oappe.top

[U90] JS：数字数组排序
来源：http://irk.jlsjyb.cn

[...arr].sort((a, b) => a - b)
来源：http://uut.xuanzx.com

[U91] JS：对象键值遍历
来源：http://idj.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mhd.mhx1999.top

[U92] JS：深拷贝
来源：http://lkp.shuidangran.top

structuredClone(obj)
来源：http://ycm.jinqigufen.top

[U93] JS：模板字符串
来源：http://hht.quarkkingdee.top

`共 ${n} 条`
来源：http://igw.ppjwa.cn

[U94] JS：箭头函数
来源：http://iem.andypj.xyz

const double = x => x * 2;
来源：http://vwe.yvedp.cn

[U95] JS：Promise 包装
来源：http://utr.gogol.net.cn

new Promise((resolve, reject) => {})
来源：http://slr.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://fgo.shangyingyoupin.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hwa.guannengcc.top

[U97] JS：并发请求
来源：http://dcm.dianchejie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bfg.smart0.xyz

[U98] JS：fetch 带 JSON
来源：http://mun.dianchejie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wbv.zhixingplan.top

[U99] JS：事件监听
来源：http://zcl.yueranfly.top

el.addEventListener("click", e => {})
来源：http://kzv.sjlbkw.cn

[U100] JS：DOM 查询
来源：http://zml.daria6918.cn

document.querySelector(".item")
来源：http://wdq.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://lsl.sjlbkw.cn

el.classList.toggle("active")
来源：http://wvy.epnwcf.com

[U102] JS：本地存储
来源：http://kom.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://tev.nwbrower.top

[U103] JS：定时器
来源：http://wty.meibo888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://okw.dianchejie.cn

[U104] JS：防抖
来源：http://qfn.hnxiangtu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://acq.shuidangran.top

[U105] JS：节流
来源：http://ett.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pcw.xuanzx.com

[U106] JS：日期格式化
来源：http://qpz.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hfj.jiagoushi.top

[U107] JS：数字千分位
来源：http://imh.dianchejie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uan.pycfn.com

[U108] JS：随机整数
来源：http://qub.daria6918.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wgd.zdqjudy.top

[U109] JS：数组分组
来源：http://mzb.shangyingyoupin.top

Object.groupBy(arr, x => x.type)
来源：http://hrz.smart0.xyz

[U110] JS：数组分块
来源：http://ilw.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pjr.hywenlv.cn

[U111] JS：对象转 Map
来源：http://jpc.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://bpg.shuidangran.top

[U112] JS：字符串补位
来源：http://roh.epnwcf.com

"7".padStart(3, "0")
来源：http://gcb.zhixingplan.top

[U113] JS：正则替换全部
来源：http://wtt.ctjpmb.com

s.replaceAll("a", "b")
来源：http://fcu.tarul.cn

[U114] JS：JSON 深比较
来源：http://iag.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jyz.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://gwh.ybcxt.top

crypto.randomUUID()
来源：http://qfa.hnqzz.top

[U116] JS：类型检查（JSDoc）
来源：http://pew.zhijiandao.cn

/** @param {string} name */ function f(name) {}
来源：http://cmp.jinqigufen.top

[U117] JS：单元测试
来源：http://uqw.ppjwa.cn

npm i -D vitest;  npx vitest
来源：http://qpk.zhixingplan.top

[U118] JS：开发服务器
来源：http://ljz.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://gew.fktsv.cn

[U119] JS：生产构建
来源：http://wem.sysykeji.top

npx vite build
来源：http://awq.fktsv.cn

[U120] JS：读取环境变量（Vite）
来源：http://xxn.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://aed.zhiwuduotai.top

================================================================================
来源：http://zye.smart0.xyz

统计汇总
来源：http://fpc.iojbl.cn

================================================================================
来源：http://rqx.daxiang520.top

按语言统计（条）：
来源：http://cfo.bbcook.cn

Python ......... 252
来源：http://shd.fktsv.cn

PHP ............ 252
来源：http://phu.gaohongyu789.top

JavaScript ..... 252
来源：http://lft.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://ser.shangyingyoupin.top

Java ........... 212
来源：http://sbh.bjfxy.top

Go ............. 212
来源：http://qzz.yj20258888.top

Ruby ........... 212
来源：http://zxr.sufxvd.cn

C# ............. 212
来源：http://gye.birdmap.top

C .............. 30
来源：http://cex.ppjwa.cn

C++ ............ 30
来源：http://ksw.52xcode.cn

SQL ............ 90
来源：http://lkc.xuanzx.com

Bash ........... 80
来源：http://kdf.jlsjyb.cn

Kotlin ......... 15
来源：http://daa.gaohongyu789.top

Swift .......... 15
来源：http://jiw.daria6918.cn

Lua ............ 10
来源：http://jvp.cashguo.top

Perl ........... 10
来源：http://auu.aizwys.cn

Scala .......... 10
来源：http://vgs.jinyuanbaomall.cn

------------------------------------
来源：http://dmu.gotoacloud.top

合计 ........... 2106 条
来源：http://jiw.fehbvm.com

按章节统计：
来源：http://jmz.cashguo.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fby.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hro.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://apw.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://niv.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ffw.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bwf.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lns.birdmap.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aof.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oyh.xuetiantiany.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gmw.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wzv.fzhhl.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nkb.gzhubu.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://muh.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bey.snrcjt.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cgn.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oqj.jqgufenzy.top

Q SQL 专题                              90
来源：http://dxb.svipenyu.cn

R Bash 专题                             80
来源：http://iwb.yonumen.top

S C / C++ 专题                          60
来源：http://zuo.haohaochexian.top

T 其他语言补充                          60
来源：http://hzx.zycfv.cn

U 高频实用片段                         120
来源：http://yor.fzhhl.top

------------------------------------
来源：http://xcf.shanyushiyangkeji.top

合计                                  2106 条
来源：http://vir.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://qlv.shangyingyoupin.top

使用提醒
来源：http://xjk.yj20258888.top

--------------------------------------------------------------------------------
来源：http://thy.nanxinkj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pvm.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://und.zhongyouzk.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jtp.pycfn.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qzl.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uiu.hammf.cn

—— 文件结束 ——
来源：http://qdj.gotoacloud.top

================================================================================
来源：http://zkw.svipenyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://xud.yj20258888.top

Common Programming Examples Cheat Book
来源：http://eio.kuanghao11.cn

================================================================================
来源：http://cvs.zhiwuduotai.top

【收录内容】
来源：http://zjf.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hxk.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://met.zycfv.cn

SQL · Bash · C · C++
来源：http://ufa.zdbjq.cn


<!-- 参考信息 -->