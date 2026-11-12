代发 wailian999

[U01] Py：创建虚拟环境
来源：http://lbb.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ogo.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://yai.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dfd.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://txu.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gpk.iojbl.cn

[U04] Py：变量调试打印
来源：http://qug.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://snw.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://saq.yuxming.cn

list(dict.fromkeys(arr))
来源：http://imt.dianchejie.cn

[U06] Py：合并两个字典
来源：http://pte.aibaodan.cn

{**a, **b}
来源：http://mad.ivvv.top

[U07] Py：反转字典键值
来源：http://kwz.ydjk.org.cn

{v: k for k, v in d.items()}
来源：http://vkd.xuanzx.com

[U08] Py：展平二维列表
来源：http://luk.yj20258888.top

[y for x in nested for y in x]
来源：http://qmd.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://eac.fzhhl.top

max(d, key=d.get)
来源：http://ehq.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://tlb.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eaz.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://oya.pycfn.com

(x * 2 for x in arr)
来源：http://oor.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://irp.zycfv.cn

Counter(arr).most_common(3)
来源：http://byg.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://fvb.yuanzhike.top

deque(maxlen=10)
来源：http://bwl.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://wjr.bjfxy.top

defaultdict(list)
来源：http://pef.jlsjyb.cn

[U15] Py：高精度计时
来源：http://saq.ivvv.top

t = time.perf_counter()
来源：http://vwa.sysykeji.top

[U16] Py：命令行参数解析
来源：http://gxa.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cob.xinyue.icu

[U17] Py：初始化日志
来源：http://nyr.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://ktc.andypj.xyz

[U18] Py：预编译正则
来源：http://kna.hammf.cn

pat = re.compile(r"\d+")
来源：http://vqu.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://cfe.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cco.tian-w.cn

[U20] Py：缓存函数结果
来源：http://ikj.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://ihd.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://vcw.ppjwa.cn

@contextlib.contextmanager
来源：http://xtb.yfazqb.com

[U22] Py：矩阵转置
来源：http://eze.vqdsnc.cn

list(zip(*m))
来源：http://tdo.fzhhl.top

[U23] Py：分块读取大文件
来源：http://ils.jinyuanbaomall.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dgm.cashguo.top

[U24] Py：路径操作
来源：http://mxa.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://awd.yonumen.top

[U25] Py：CSV 按字典读
来源：http://nbv.yvedp.cn

csv.DictReader(f)
来源：http://wds.quarkkingdee.top

[U26] Py：并发下载
来源：http://vie.yanxiufei.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://irr.daxiang520.top

[U27] Py：异步 HTTP
来源：http://uqn.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://itv.vehdjk.com

[U28] Py：类型别名
来源：http://fux.kuanghao11.cn

UserId = int
来源：http://tlz.tianlin.xyz

[U29] Py：属性校验
来源：http://dmq.hysaishi.cn

@property 与 @x.setter 配合
来源：http://nds.xziqi.cn

[U30] Py：数据类
来源：http://rkd.yuxming.cn

@dataclass(slots=True)
来源：http://etw.xinyue.icu

[U31] Py：单测
来源：http://dss.zhengqikj.top

python -m pytest -q
来源：http://hpr.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://ejj.shangyingyoupin.top

ruff format . && ruff check --fix .
来源：http://krd.nanxinkj.top

[U33] Py：打包发布
来源：http://wde.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://qeu.ctjpmb.com

[U34] Py：判断编码
来源：http://kba.cucudq.cn

chardet.detect(raw)
来源：http://bjw.guannengcc.top

[U35] Py：发送邮件
来源：http://ubl.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lyl.jyoumei.cn

[U36] Py：定时任务
来源：http://gak.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://kcp.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://zbg.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fhk.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://phb.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://taz.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://aos.xylfe.cn

sys.stdout.isatty()
来源：http://wmg.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://ukx.c1oappe.top

print("err", file=sys.stderr)
来源：http://fmn.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://zpm.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://lqm.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://csx.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qnk.hcnkem.com

[U43] PHP：声明命名空间
来源：http://icx.zhengqikj.top

namespace App\Http;
来源：http://efz.xingfuxueyuan.xyz

[U44] PHP：开启严格类型
来源：http://uua.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://fsx.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://hqk.tanke756.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lpr.yangfankeji.com

[U46] PHP：可空类型
来源：http://eka.tarul.cn

?string $name = null
来源：http://uid.yuanzhike.top

[U47] PHP：联合类型
来源：http://jdt.feifeiyinyue.top

int|string $id
来源：http://kcg.aizwys.cn

[U48] PHP：纯枚举
来源：http://rdr.jqgufenzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kwd.dianchejie.cn

[U49] PHP：只读属性
来源：http://ziw.hfpthk.cn

public readonly string $name
来源：http://jhw.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://utv.jiagoushi.top

public function __construct(private int $id) {}
来源：http://yxr.sysykeji.top

[U51] PHP：数组解构
来源：http://boh.tarul.cn

[$a, $b] = $arr;
来源：http://sqj.xylfe.cn

[U52] PHP：箭头函数
来源：http://wxc.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://ndd.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://yqj.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://uwl.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://tas.mhx1999.top

$obj?->method()
来源：http://ujf.gotoacloud.top

[U55] PHP：match 表达式
来源：http://bjd.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eoc.cqqwz.cn

[U56] PHP：命名参数
来源：http://muc.gzhubu.top

f(a: 1, b: 2)
来源：http://gul.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://got.hysaishi.cn

"值: {$a}"
来源：http://wyx.nanxinkj.top

[U58] PHP：数组三件套
来源：http://ncq.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rhz.xinyue.icu

[U59] PHP：自定义排序
来源：http://lig.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wur.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://szt.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vox.hammf.cn

[U61] PHP：正则
来源：http://vhi.yueranfly.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lur.xinyue.icu

[U62] PHP：日期对象
来源：http://nio.dashuyun.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pun.cucudq.cn

[U63] PHP：文件读写
来源：http://ovr.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kdv.havefunace.top

[U64] PHP：目录遍历
来源：http://iiu.daxiang520.top

glob("dir/*.php");  scandir("dir");
来源：http://cmf.jinqigufen.top

[U65] PHP：会话
来源：http://xxi.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dig.xuanzx.com

[U66] PHP：设置 Cookie
来源：http://uic.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ktp.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://rcf.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ylp.quarkkingdee.top

[U68] PHP：PDO 连接
来源：http://kot.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hpg.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://xqs.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bxm.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://lxn.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wse.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://kce.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://qkh.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://bvu.316326.xyz

error_log("失败: " . $e->getMessage());
来源：http://una.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://cdq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://jgq.c1oappe.top

[U74] PHP：读取环境变量
来源：http://gdt.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://ehh.daria6918.cn

[U75] PHP：依赖注入
来源：http://lmk.wangdashe.top

composer require psr/container
来源：http://qoa.xingfuxueyuan.xyz

[U76] PHP：简单路由
来源：http://kaj.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oth.nanxinkj.top

[U77] PHP：模板渲染
来源：http://vic.sxryk.cn

composer require twig/twig
来源：http://hih.hysaishi.cn

[U78] PHP：单元测试
来源：http://hjf.yvedp.cn

composer require --dev phpunit/phpunit
来源：http://lza.hesvh.cn

[U79] PHP：静态分析
来源：http://jmf.hammf.cn

composer require --dev phpstan/phpstan
来源：http://arz.jinqigufen.top

[U80] PHP：代码规范修复
来源：http://xgq.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ohw.vehdjk.com

[U81] JS：初始化项目
来源：http://vho.kuanghao11.cn

npm init -y;  npm i express
来源：http://hwh.yvedp.cn

[U82] JS：package.json 脚本
来源：http://vxx.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mpq.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://izx.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://puk.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://kif.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cmz.0kj1m.cn

[U85] JS：可选链
来源：http://qpm.epnwcf.com

a?.b?.c
来源：http://xyv.zycfv.cn

[U86] JS：空值合并
来源：http://pis.0kj1m.cn

a ?? b
来源：http://oqd.gogol.net.cn

[U87] JS：解构默认值
来源：http://agx.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://vqc.meibo888.top

[U88] JS：对象展开合并
来源：http://gcb.zdqjudy.top

{ ...a, ...b }
来源：http://yyk.jqgfzy.top

[U89] JS：数组去重
来源：http://kvn.snrcjt.cn

[...new Set(arr)]
来源：http://caz.vqdsnc.cn

[U90] JS：数字数组排序
来源：http://fep.birdmap.top

[...arr].sort((a, b) => a - b)
来源：http://lqx.xingfuxueyuan.xyz

[U91] JS：对象键值遍历
来源：http://ygf.meibo888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bap.xylfe.cn

[U92] JS：深拷贝
来源：http://wwj.quarkkingdee.top

structuredClone(obj)
来源：http://yik.andypj.xyz

[U93] JS：模板字符串
来源：http://yjl.zhengqikj.top

`共 ${n} 条`
来源：http://laj.tarul.cn

[U94] JS：箭头函数
来源：http://jqu.yj20258888.top

const double = x => x * 2;
来源：http://zzi.yj20258888.top

[U95] JS：Promise 包装
来源：http://omg.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://ztn.pycfn.com

[U96] JS：async/await 与异常
来源：http://xad.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://luc.hammf.cn

[U97] JS：并发请求
来源：http://tfv.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xnu.xziqi.cn

[U98] JS：fetch 带 JSON
来源：http://lug.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hdh.hfpthk.cn

[U99] JS：事件监听
来源：http://irj.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://wat.bbcook.cn

[U100] JS：DOM 查询
来源：http://cvc.jqgfzy.top

document.querySelector(".item")
来源：http://vhx.smart0.xyz

[U101] JS：classList 操作
来源：http://xbv.nanxuanxn.top

el.classList.toggle("active")
来源：http://pul.zhixingplan.top

[U102] JS：本地存储
来源：http://obc.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ewb.andypj.xyz

[U103] JS：定时器
来源：http://ktr.wangdashe.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dgl.ywan-chungtsiang.top

[U104] JS：防抖
来源：http://hfk.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kta.zhixingplan.top

[U105] JS：节流
来源：http://ice.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ssd.vqdsnc.cn

[U106] JS：日期格式化
来源：http://loz.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://szz.tanke756.top

[U107] JS：数字千分位
来源：http://jho.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dje.havefunace.top

[U108] JS：随机整数
来源：http://nmb.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hdr.chenjidiqi.icu

[U109] JS：数组分组
来源：http://xdf.meibo888.top

Object.groupBy(arr, x => x.type)
来源：http://wzl.ehwqpu.com

[U110] JS：数组分块
来源：http://yul.fzhhl.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kfb.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://fnk.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://tex.yanxiufei.cn

[U112] JS：字符串补位
来源：http://thb.snrcjt.cn

"7".padStart(3, "0")
来源：http://uin.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://toa.jinqigufen.top

s.replaceAll("a", "b")
来源：http://cbv.ybcxt.top

[U114] JS：JSON 深比较
来源：http://idf.ywan-chungtsiang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bah.sufxvd.cn

[U115] JS：生成 UUID
来源：http://xyd.shanyushiyangkeji.top

crypto.randomUUID()
来源：http://sva.cheryme.top

[U116] JS：类型检查（JSDoc）
来源：http://bfr.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://lsc.zdbjq.cn

[U117] JS：单元测试
来源：http://lng.hfpthk.cn

npm i -D vitest;  npx vitest
来源：http://bsi.daria6918.cn

[U118] JS：开发服务器
来源：http://eqe.vqdsnc.cn

npm i -D vite;  npx vite
来源：http://tht.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://tat.fktsv.cn

npx vite build
来源：http://sck.ybcxt.top

[U120] JS：读取环境变量（Vite）
来源：http://tmp.redwolf501.top

import.meta.env.VITE_API_URL
来源：http://qpa.fengsongda.top

================================================================================
来源：http://ans.gogol.net.cn

统计汇总
来源：http://vyg.hysaishi.cn

================================================================================
来源：http://she.zhijiandao.cn

按语言统计（条）：
来源：http://sgx.iojbl.cn

Python ......... 252
来源：http://pua.zhoulong.xyz

PHP ............ 252
来源：http://xkk.pycfn.com

JavaScript ..... 252
来源：http://hsc.sweek.top

TypeScript ..... 212
来源：http://vef.cqqwz.cn

Java ........... 212
来源：http://huk.yangfankeji.com

Go ............. 212
来源：http://cdz.jianghu66.top

Ruby ........... 212
来源：http://vjw.wangshuangyany.cn

C# ............. 212
来源：http://ibr.jinyuanbaomall.cn

C .............. 30
来源：http://ayy.haohaochexian.top

C++ ............ 30
来源：http://bdf.zdqjudy.top

SQL ............ 90
来源：http://pae.xingfuxueyuan.xyz

Bash ........... 80
来源：http://iss.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://gva.xziqi.cn

Swift .......... 15
来源：http://ewg.jinqigufen.top

Lua ............ 10
来源：http://dgf.zhoulong.xyz

Perl ........... 10
来源：http://qqy.pengpengdd.cyou

Scala .......... 10
来源：http://noi.dashuyun.cn

------------------------------------
来源：http://dmd.cdnleiting.top

合计 ........... 2106 条
来源：http://oxj.xuetiantiany.cn

按章节统计：
来源：http://ydw.shanyushiyangtech.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oez.ctjpmb.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://buz.jiagoushi.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mrx.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lis.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xzb.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yvl.birdmap.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xlg.sjlbkw.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aov.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fuf.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gvv.shuidangran.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zoj.yj20258888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ebo.tanke756.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hsi.jlsjyb.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tiw.zhengqikj.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qpq.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bxz.kuanghao11.cn

Q SQL 专题                              90
来源：http://zgk.chenzaomai.com

R Bash 专题                             80
来源：http://uke.yj20258888.top

S C / C++ 专题                          60
来源：http://cke.ctjpmb.com

T 其他语言补充                          60
来源：http://uba.tianlin.xyz

U 高频实用片段                         120
来源：http://xyh.yvedp.cn

------------------------------------
来源：http://nmq.ydzc1.top

合计                                  2106 条
来源：http://zyh.yueranfly.top

--------------------------------------------------------------------------------
来源：http://ggv.52xcode.cn

使用提醒
来源：http://ftb.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://ndc.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vgq.cucudq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://msh.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pom.sweek.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xhy.jinyuanbaomall.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qtt.vehdjk.com

—— 文件结束 ——
来源：http://kee.nwbrower.top

================================================================================
来源：http://jsc.dianchejie.cn

程序语言常见例子速查手册（2024 版）
来源：http://mhm.gzhubu.top

Common Programming Examples Cheat Book
来源：http://dtf.jinqigufen.top

================================================================================
来源：http://uxp.zhixingplan.top


<!-- 参考信息 -->