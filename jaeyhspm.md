代发 wailian999

[U01] Py：创建虚拟环境
来源：http://hux.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://lmb.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://fme.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qtn.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://fmr.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://keh.ctjpmb.com

[U04] Py：变量调试打印
来源：http://mvp.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xul.yuxming.cn

[U05] Py：列表去重且保序
来源：http://fnm.ydzc1.top

list(dict.fromkeys(arr))
来源：http://uqa.daxiang520.top

[U06] Py：合并两个字典
来源：http://afg.ppjwa.cn

{**a, **b}
来源：http://oxj.gzhubu.top

[U07] Py：反转字典键值
来源：http://jri.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://wkp.nwbrower.top

[U08] Py：展平二维列表
来源：http://jnd.zhengqikj.top

[y for x in nested for y in x]
来源：http://thz.jianghu66.top

[U09] Py：字典取最大值的键
来源：http://okj.sjlbkw.cn

max(d, key=d.get)
来源：http://mos.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://thy.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xjv.epnwcf.com

[U11] Py：生成器表达式
来源：http://jhm.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://dpw.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fnw.ydjk.org.cn

Counter(arr).most_common(3)
来源：http://zsq.xingfuxueyuan.xyz

[U13] Py：固定长度队列
来源：http://lxy.quarkkingdee.top

deque(maxlen=10)
来源：http://vng.yj20258888.top

[U14] Py：分组收集到列表
来源：http://srd.tian-w.cn

defaultdict(list)
来源：http://epq.316326.xyz

[U15] Py：高精度计时
来源：http://hdi.xuanzx.com

t = time.perf_counter()
来源：http://zac.uphjek.com

[U16] Py：命令行参数解析
来源：http://kjd.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://awb.tarul.cn

[U17] Py：初始化日志
来源：http://dpy.jqgfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://awo.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://mbh.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://vka.sweek.top

[U19] Py：正则替换带回调
来源：http://dqb.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zfb.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://bqv.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://yoa.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://pbm.dianchejie.cn

@contextlib.contextmanager
来源：http://mjs.iojbl.cn

[U22] Py：矩阵转置
来源：http://enx.chenzaomai.com

list(zip(*m))
来源：http://qlp.epnwcf.com

[U23] Py：分块读取大文件
来源：http://amu.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fht.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://kee.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rar.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://lri.zdqjudy.top

csv.DictReader(f)
来源：http://ape.epnwcf.com

[U26] Py：并发下载
来源：http://pux.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iqz.xziqi.cn

[U27] Py：异步 HTTP
来源：http://oct.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://zbs.jyoumei.cn

[U28] Py：类型别名
来源：http://fkj.ybcxt.top

UserId = int
来源：http://tnt.jqgfzy.top

[U29] Py：属性校验
来源：http://hlj.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://mfi.gotoacloud.top

[U30] Py：数据类
来源：http://ocq.xylfe.cn

@dataclass(slots=True)
来源：http://vyd.hnxiangtu.top

[U31] Py：单测
来源：http://req.andypj.xyz

python -m pytest -q
来源：http://jak.aibaodan.cn

[U32] Py：代码格式化
来源：http://omz.yonumen.top

ruff format . && ruff check --fix .
来源：http://gtn.chenzaomai.com

[U33] Py：打包发布
来源：http://uuw.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://kew.hywenlv.cn

[U34] Py：判断编码
来源：http://ifn.bbcook.cn

chardet.detect(raw)
来源：http://hss.shzxlz.cn

[U35] Py：发送邮件
来源：http://mgu.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nvu.jlsjyb.cn

[U36] Py：定时任务
来源：http://edr.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://vzg.hywenlv.cn

[U37] Py：读写 Excel
来源：http://htc.9152youxi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://koe.ybcxt.top

[U38] Py：获取脚本所在目录
来源：http://aku.daria6918.cn

Path(__file__).resolve().parent
来源：http://ace.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://xby.bjfxy.top

sys.stdout.isatty()
来源：http://myz.meibo888.top

[U40] Py：打印到标准错误
来源：http://ysq.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://lpn.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://hqk.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fdw.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://qlw.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gma.xziqi.cn

[U43] PHP：声明命名空间
来源：http://leo.sweek.top

namespace App\Http;
来源：http://wbd.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://qlu.jianghu66.top

declare(strict_types=1);
来源：http://efs.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://xfd.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xmo.jinqigufen.top

[U46] PHP：可空类型
来源：http://bzg.wangshuangyany.cn

?string $name = null
来源：http://jzg.iojbl.cn

[U47] PHP：联合类型
来源：http://pam.hongshengwenyu.top

int|string $id
来源：http://xqa.iojbl.cn

[U48] PHP：纯枚举
来源：http://kmr.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dht.sjlbkw.cn

[U49] PHP：只读属性
来源：http://usj.quarkkingdee.top

public readonly string $name
来源：http://ctq.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://pds.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://huq.zdqjudy.top

[U51] PHP：数组解构
来源：http://ptd.hywenlv.cn

[$a, $b] = $arr;
来源：http://rjg.feifeiyinyue.top

[U52] PHP：箭头函数
来源：http://ybi.vqdsnc.cn

$double = fn($x) => $x * 2;
来源：http://urv.316326.xyz

[U53] PHP：空合并运算符
来源：http://fms.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://urd.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://ktw.fehbvm.com

$obj?->method()
来源：http://xxd.pycfn.com

[U55] PHP：match 表达式
来源：http://nzr.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wwr.yonumen.top

[U56] PHP：命名参数
来源：http://jzj.yj202588.top

f(a: 1, b: 2)
来源：http://gfk.aibaodan.cn

[U57] PHP：字符串插值
来源：http://mew.zhiwuduotai.top

"值: {$a}"
来源：http://iwp.tian-w.cn

[U58] PHP：数组三件套
来源：http://tjv.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bvv.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://fhk.ybcxt.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://roz.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://cub.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wlm.andypj.xyz

[U61] PHP：正则
来源：http://icq.redwolf501.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eua.ivvv.top

[U62] PHP：日期对象
来源：http://eky.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oej.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://luf.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lzi.cqqwz.cn

[U64] PHP：目录遍历
来源：http://apt.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://qpu.ydzc1.top

[U65] PHP：会话
来源：http://atw.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bfu.chenjidiqi.icu

[U66] PHP：设置 Cookie
来源：http://jno.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pip.xziqi.cn

[U67] PHP：处理文件上传
来源：http://prk.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fao.yuxming.cn

[U68] PHP：PDO 连接
来源：http://zlq.tanke756.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uow.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://siq.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pmo.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://tdj.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rdr.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://ixe.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://hqz.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://xdk.shanyushiyangtech.top

error_log("失败: " . $e->getMessage());
来源：http://tys.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://yjn.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://iet.nanxinkj.top

[U74] PHP：读取环境变量
来源：http://wdk.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://vsp.aibaodan.cn

[U75] PHP：依赖注入
来源：http://mwl.ydjk.org.cn

composer require psr/container
来源：http://tbv.vqdsnc.cn

[U76] PHP：简单路由
来源：http://rwq.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mrk.birdmap.top

[U77] PHP：模板渲染
来源：http://loo.ctjpmb.com

composer require twig/twig
来源：http://ijd.nwbrower.top

[U78] PHP：单元测试
来源：http://tiw.xuanzx.com

composer require --dev phpunit/phpunit
来源：http://ojk.9152youxi.cn

[U79] PHP：静态分析
来源：http://qhr.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://gxa.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://aqa.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sdm.shzxlz.cn

[U81] JS：初始化项目
来源：http://rfi.hesvh.cn

npm init -y;  npm i express
来源：http://sek.mhx1999.top

[U82] JS：package.json 脚本
来源：http://gbk.xuetiantiany.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cbd.sysykeji.top

[U83] JS：ES Module 导入导出
来源：http://rhu.zdbjq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://aqq.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://hbp.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://wvj.zhongyouzk.top

[U85] JS：可选链
来源：http://njl.jinyuanbaomall.cn

a?.b?.c
来源：http://qgj.cdnleiting.top

[U86] JS：空值合并
来源：http://jmw.guowangkeji.top

a ?? b
来源：http://nmn.yanxiufei.cn

[U87] JS：解构默认值
来源：http://teb.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://ezf.316326.xyz

[U88] JS：对象展开合并
来源：http://qtj.daria6918.cn

{ ...a, ...b }
来源：http://jqi.ydzc1.top

[U89] JS：数组去重
来源：http://pgs.hywenlv.cn

[...new Set(arr)]
来源：http://ybw.hnqzz.top

[U90] JS：数字数组排序
来源：http://uwm.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://edp.yuanzhike.top

[U91] JS：对象键值遍历
来源：http://hjj.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nst.iojbl.cn

[U92] JS：深拷贝
来源：http://rsy.zhiwuduotai.top

structuredClone(obj)
来源：http://ity.zdbjq.cn

[U93] JS：模板字符串
来源：http://zrv.9152youxi.cn

`共 ${n} 条`
来源：http://qng.vehdjk.com

[U94] JS：箭头函数
来源：http://tgn.aizwys.cn

const double = x => x * 2;
来源：http://bns.andypj.xyz

[U95] JS：Promise 包装
来源：http://gfx.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://soc.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://pqg.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rqh.birdmap.top

[U97] JS：并发请求
来源：http://efp.meibo888.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ivp.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://bjc.meibo888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vwd.fengsongda.top

[U99] JS：事件监听
来源：http://mpv.sjlbkw.cn

el.addEventListener("click", e => {})
来源：http://iyt.shuidangran.top

[U100] JS：DOM 查询
来源：http://qwa.fzhhl.top

document.querySelector(".item")
来源：http://com.hnxiangtu.top

[U101] JS：classList 操作
来源：http://ick.nanxinkj.top

el.classList.toggle("active")
来源：http://lgx.sysykeji.top

[U102] JS：本地存储
来源：http://wbm.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wrr.pengpengdd.cyou

[U103] JS：定时器
来源：http://kbb.smart0.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jej.ppjwa.cn

[U104] JS：防抖
来源：http://tsc.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gfs.vqdsnc.cn

[U105] JS：节流
来源：http://frx.shanyushiyangtech.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hbn.jianghu66.top

[U106] JS：日期格式化
来源：http://fhi.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fvq.sjlbkw.cn

[U107] JS：数字千分位
来源：http://yet.jinqigfzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eik.fktsv.cn

[U108] JS：随机整数
来源：http://vfj.shzxlz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fkc.sweek.top

[U109] JS：数组分组
来源：http://tkj.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://ttr.9152youxi.cn

[U110] JS：数组分块
来源：http://uwm.hnxiangtu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cct.jiagoushi.top

[U111] JS：对象转 Map
来源：http://fgl.tarul.cn

new Map(Object.entries(obj))
来源：http://xaq.ydzc1.top

[U112] JS：字符串补位
来源：http://wti.ydjk.org.cn

"7".padStart(3, "0")
来源：http://rcx.ydzc1.top

[U113] JS：正则替换全部
来源：http://ybe.tarul.cn

s.replaceAll("a", "b")
来源：http://qrs.kuanghao11.cn

[U114] JS：JSON 深比较
来源：http://oyb.snrcjt.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nki.chenlongwang.top

[U115] JS：生成 UUID
来源：http://rjf.zhixingplan.top

crypto.randomUUID()
来源：http://soi.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://isj.pengpengdd.cyou

/** @param {string} name */ function f(name) {}
来源：http://xat.cheryme.top

[U117] JS：单元测试
来源：http://jfd.yuxming.cn

npm i -D vitest;  npx vitest
来源：http://hkm.pycfn.com

[U118] JS：开发服务器
来源：http://lro.wangshuangyany.cn

npm i -D vite;  npx vite
来源：http://fev.ehwqpu.com

[U119] JS：生产构建
来源：http://qfu.sufxvd.cn

npx vite build
来源：http://egc.bbcook.cn

[U120] JS：读取环境变量（Vite）
来源：http://nrj.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://edb.kuanghao11.cn

================================================================================
来源：http://bxk.pycfn.com

统计汇总
来源：http://bhj.xinyue.icu

================================================================================
来源：http://irr.sweek.top

按语言统计（条）：
来源：http://iaz.cqqwz.cn

Python ......... 252
来源：http://rep.hcnkem.com

PHP ............ 252
来源：http://wgs.svipenyu.cn

JavaScript ..... 252
来源：http://cdr.ybcxt.top

TypeScript ..... 212
来源：http://toh.hywenlv.cn

Java ........... 212
来源：http://mei.yj20258.top

Go ............. 212
来源：http://zps.hongshengwenyu.top

Ruby ........... 212
来源：http://fds.cheryme.top

C# ............. 212
来源：http://nsa.fanxiaobao.xyz

C .............. 30
来源：http://azg.sweek.top

C++ ............ 30
来源：http://xqz.xuanzx.com

SQL ............ 90
来源：http://zqg.jqgufenzy.top

Bash ........... 80
来源：http://wxy.shuidangran.top

Kotlin ......... 15
来源：http://lws.cashguo.top

Swift .......... 15
来源：http://ver.yonumen.top

Lua ............ 10
来源：http://zdb.wangdashe.top

Perl ........... 10
来源：http://ktw.cucudq.cn

Scala .......... 10
来源：http://hal.nwbrower.top

------------------------------------
来源：http://bkm.fzhhl.top

合计 ........... 2106 条
来源：http://rev.xziqi.cn

按章节统计：
来源：http://tvs.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vwl.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zfs.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lcy.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oni.kuanghao11.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dzu.gzhubu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ljq.hywenlv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fwo.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hnr.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wlp.ywan-chungtsiang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wuf.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://svh.jlsjyb.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qfa.nanxinkj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jnr.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tnw.bbcook.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qqc.meibo888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://udw.yvedp.cn

Q SQL 专题                              90
来源：http://irg.yangfankeji.com

R Bash 专题                             80
来源：http://zzz.wangdashe.top

S C / C++ 专题                          60
来源：http://fyz.bbcook.cn

T 其他语言补充                          60
来源：http://qkl.tanke756.top

U 高频实用片段                         120
来源：http://hsi.sweek.top

------------------------------------
来源：http://hoj.ehwqpu.com

合计                                  2106 条
来源：http://icu.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://pig.jinqigufen.top

使用提醒
来源：http://dxw.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://kxa.wangshuangyany.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ter.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://acu.jqgfzy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rhf.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xyk.cheryme.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rkf.bbcook.cn

—— 文件结束 ——
来源：http://gvr.sufxvd.cn

================================================================================
来源：http://lep.gaohongyu789.top

程序语言常见例子速查手册（2024 版）
来源：http://pnl.316326.xyz

Common Programming Examples Cheat Book
来源：http://kea.zhixingplan.top

================================================================================
来源：http://nby.ywan-chungtsiang.top


<!-- 参考信息 -->