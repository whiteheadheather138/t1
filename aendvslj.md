代发 wailian999

[U01] Py：创建虚拟环境
来源：http://acw.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://zlg.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://ukt.yuxming.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://btb.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://huk.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://zgb.ivvv.top

[U04] Py：变量调试打印
来源：http://ial.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dvp.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://zca.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://deu.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://nyg.redwolf501.top

{**a, **b}
来源：http://iti.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://hyk.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://kbz.jinqigufen.top

[U08] Py：展平二维列表
来源：http://cig.zhoulong.xyz

[y for x in nested for y in x]
来源：http://epx.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://wph.guowangkeji.top

max(d, key=d.get)
来源：http://rpo.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://xqz.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ngs.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://hyl.svipenyu.cn

(x * 2 for x in arr)
来源：http://zuk.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://coi.tarul.cn

Counter(arr).most_common(3)
来源：http://ggn.yj20258.top

[U13] Py：固定长度队列
来源：http://ivr.ydjk.org.cn

deque(maxlen=10)
来源：http://nxt.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://tsk.zhiwuduotai.top

defaultdict(list)
来源：http://xub.yvedp.cn

[U15] Py：高精度计时
来源：http://mzq.xuanzx.com

t = time.perf_counter()
来源：http://fnx.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://ihz.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckg.kuanghao11.cn

[U17] Py：初始化日志
来源：http://qpc.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://esw.daria6918.cn

[U18] Py：预编译正则
来源：http://faz.c1oappe.top

pat = re.compile(r"\d+")
来源：http://mbm.shanyushiyangkeji.top

[U19] Py：正则替换带回调
来源：http://zvr.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://aar.iojbl.cn

[U20] Py：缓存函数结果
来源：http://hvd.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://tuj.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://idd.jlsjyb.cn

@contextlib.contextmanager
来源：http://ktn.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://jwm.sweek.top

list(zip(*m))
来源：http://cuc.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://zjs.yuxming.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lnr.yuanzhike.top

[U24] Py：路径操作
来源：http://qcu.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tcx.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://xbv.uphjek.com

csv.DictReader(f)
来源：http://ibk.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://dtw.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://moy.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://ulj.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://bin.fzhhl.top

[U28] Py：类型别名
来源：http://cgs.xingfuxueyuan.xyz

UserId = int
来源：http://fls.fehbvm.com

[U29] Py：属性校验
来源：http://wlo.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://qph.aizwys.cn

[U30] Py：数据类
来源：http://zmz.aibaodan.cn

@dataclass(slots=True)
来源：http://ftt.tian-w.cn

[U31] Py：单测
来源：http://rgu.zhiwuduotai.top

python -m pytest -q
来源：http://dyj.xuanzx.com

[U32] Py：代码格式化
来源：http://pox.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://lmt.gaohongyu789.top

[U33] Py：打包发布
来源：http://zrq.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://sgm.pengpengdd.cyou

[U34] Py：判断编码
来源：http://icx.fktsv.cn

chardet.detect(raw)
来源：http://mlz.zhijiandao.cn

[U35] Py：发送邮件
来源：http://caj.52xcode.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://psv.hongshengwenyu.top

[U36] Py：定时任务
来源：http://vht.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://xps.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://qmd.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nut.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://fnk.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://zod.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://iva.redwolf501.top

sys.stdout.isatty()
来源：http://ocl.vqdsnc.cn

[U40] Py：打印到标准错误
来源：http://xzf.fktsv.cn

print("err", file=sys.stderr)
来源：http://bts.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://eiu.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mse.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://mmi.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xzc.xingfuxueyuan.xyz

[U43] PHP：声明命名空间
来源：http://ycf.bjfxy.top

namespace App\Http;
来源：http://fjo.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://aiv.sweek.top

declare(strict_types=1);
来源：http://nvy.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://tvl.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xeg.yfazqb.com

[U46] PHP：可空类型
来源：http://hku.c1oappe.top

?string $name = null
来源：http://poi.gogol.net.cn

[U47] PHP：联合类型
来源：http://iws.hammf.cn

int|string $id
来源：http://yql.ctjpmb.com

[U48] PHP：纯枚举
来源：http://usa.ppjwa.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mcf.jinqigufen.top

[U49] PHP：只读属性
来源：http://nve.shanyushiyangkeji.top

public readonly string $name
来源：http://spr.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://azk.tianlin.xyz

public function __construct(private int $id) {}
来源：http://ldn.kuanghao11.cn

[U51] PHP：数组解构
来源：http://dtm.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://mui.hfpthk.cn

[U52] PHP：箭头函数
来源：http://pwh.zhiwuduotai.top

$double = fn($x) => $x * 2;
来源：http://jxm.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://veb.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://dyt.xuetiantiany.cn

[U54] PHP：空安全调用
来源：http://jqj.jinqigfzy.top

$obj?->method()
来源：http://xyr.cqqwz.cn

[U55] PHP：match 表达式
来源：http://gir.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yoo.yongpay.top

[U56] PHP：命名参数
来源：http://iio.ybcxt.top

f(a: 1, b: 2)
来源：http://cou.hfpthk.cn

[U57] PHP：字符串插值
来源：http://aqi.shanyushiyangtech.top

"值: {$a}"
来源：http://wmo.epnwcf.com

[U58] PHP：数组三件套
来源：http://zqj.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wyu.ivvv.top

[U59] PHP：自定义排序
来源：http://rro.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gak.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://aor.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gex.aibaodan.cn

[U61] PHP：正则
来源：http://jbg.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vnl.ydjk.org.cn

[U62] PHP：日期对象
来源：http://ukl.jyoumei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kgi.sjlbkw.cn

[U63] PHP：文件读写
来源：http://ztm.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pzr.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://fna.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://rna.shzxlz.cn

[U65] PHP：会话
来源：http://tnp.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pef.jinqigfzy.top

[U66] PHP：设置 Cookie
来源：http://mzc.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ocm.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://jmm.xuanzx.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ozk.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://kui.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xhv.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://rbk.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wgk.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://frr.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://aij.nwbrower.top

[U71] PHP：抛出异常
来源：http://pum.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://kns.sweek.top

[U72] PHP：写错误日志
来源：http://crl.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://oyj.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://ioe.316326.xyz

parse_ini_file("config.ini", true)
来源：http://ckd.c1oappe.top

[U74] PHP：读取环境变量
来源：http://qnq.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://yst.tianlin.xyz

[U75] PHP：依赖注入
来源：http://caz.zhongyouzk.top

composer require psr/container
来源：http://hkr.tanke756.top

[U76] PHP：简单路由
来源：http://fzh.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jlp.fengsongda.top

[U77] PHP：模板渲染
来源：http://fxd.xuetiantiany.cn

composer require twig/twig
来源：http://vln.zhixingplan.top

[U78] PHP：单元测试
来源：http://uzd.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://oho.fengsongda.top

[U79] PHP：静态分析
来源：http://knf.ctjpmb.com

composer require --dev phpstan/phpstan
来源：http://agf.gogol.net.cn

[U80] PHP：代码规范修复
来源：http://ppo.zhoulong.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://mkr.yueranfly.top

[U81] JS：初始化项目
来源：http://inu.shzxlz.cn

npm init -y;  npm i express
来源：http://bqx.svipenyu.cn

[U82] JS：package.json 脚本
来源：http://zzo.jlsjyb.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bad.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://pxf.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://rgu.shzxlz.cn

[U84] JS：CommonJS 写法
来源：http://atz.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qkq.aizwys.cn

[U85] JS：可选链
来源：http://kgs.ehwqpu.com

a?.b?.c
来源：http://jmg.havefunace.top

[U86] JS：空值合并
来源：http://ddl.yuanzhike.top

a ?? b
来源：http://yqv.ydzc1.top

[U87] JS：解构默认值
来源：http://yij.yangfankeji.com

const { a = 1, b = 2 } = obj;
来源：http://qdu.pycfn.com

[U88] JS：对象展开合并
来源：http://lva.bjfxy.top

{ ...a, ...b }
来源：http://omq.c1oappe.top

[U89] JS：数组去重
来源：http://zlo.cashguo.top

[...new Set(arr)]
来源：http://fkp.xziqi.cn

[U90] JS：数字数组排序
来源：http://ock.yuanzhike.top

[...arr].sort((a, b) => a - b)
来源：http://cmk.sysykeji.top

[U91] JS：对象键值遍历
来源：http://zsr.yanxiufei.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qkf.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://kje.havefunace.top

structuredClone(obj)
来源：http://gnj.chenlongwang.top

[U93] JS：模板字符串
来源：http://pgs.vehdjk.com

`共 ${n} 条`
来源：http://drj.zdqjudy.top

[U94] JS：箭头函数
来源：http://agw.zycfv.cn

const double = x => x * 2;
来源：http://fxy.cheryme.top

[U95] JS：Promise 包装
来源：http://sxx.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://jxl.yonumen.top

[U96] JS：async/await 与异常
来源：http://ubl.nanxuanxn.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lxm.yangfankeji.com

[U97] JS：并发请求
来源：http://xmx.birdmap.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kjl.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://glz.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bmi.dashuyun.cn

[U99] JS：事件监听
来源：http://dwr.cucudq.cn

el.addEventListener("click", e => {})
来源：http://ggd.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://vji.shzxlz.cn

document.querySelector(".item")
来源：http://fdn.zycfv.cn

[U101] JS：classList 操作
来源：http://jaz.hnxiangtu.top

el.classList.toggle("active")
来源：http://isa.yuxming.cn

[U102] JS：本地存储
来源：http://txm.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oyx.yj202588.top

[U103] JS：定时器
来源：http://exy.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pvb.jqgfzy.top

[U104] JS：防抖
来源：http://bth.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jje.jinghuilouyu.cn

[U105] JS：节流
来源：http://dmu.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ucy.guowangkeji.top

[U106] JS：日期格式化
来源：http://xzq.yvedp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vue.vehdjk.com

[U107] JS：数字千分位
来源：http://eyy.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oxm.zdbjq.cn

[U108] JS：随机整数
来源：http://swx.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mct.andypj.xyz

[U109] JS：数组分组
来源：http://zmu.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://ssc.cucudq.cn

[U110] JS：数组分块
来源：http://lvz.xziqi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tep.yonumen.top

[U111] JS：对象转 Map
来源：http://awq.aibaodan.cn

new Map(Object.entries(obj))
来源：http://yfx.dianchejie.cn

[U112] JS：字符串补位
来源：http://ame.uphjek.com

"7".padStart(3, "0")
来源：http://oeo.tianlin.xyz

[U113] JS：正则替换全部
来源：http://kuo.sysykeji.top

s.replaceAll("a", "b")
来源：http://uvx.316326.xyz

[U114] JS：JSON 深比较
来源：http://ovq.jinghuilouyu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uhz.zhixingplan.top

[U115] JS：生成 UUID
来源：http://zjr.wangshuangyany.cn

crypto.randomUUID()
来源：http://ebu.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://jmr.jlsjyb.cn

/** @param {string} name */ function f(name) {}
来源：http://cez.yuxming.cn

[U117] JS：单元测试
来源：http://xsh.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://jdk.dashuyun.cn

[U118] JS：开发服务器
来源：http://dnc.jyoumei.cn

npm i -D vite;  npx vite
来源：http://ifq.cucudq.cn

[U119] JS：生产构建
来源：http://ykj.ehwqpu.com

npx vite build
来源：http://lqw.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://wgf.daxiang520.top

import.meta.env.VITE_API_URL
来源：http://rvb.c1oappe.top

================================================================================
来源：http://fcm.shuidangran.top

统计汇总
来源：http://zzt.daxiang520.top

================================================================================
来源：http://stm.bbcook.cn

按语言统计（条）：
来源：http://wat.smart0.xyz

Python ......... 252
来源：http://fgi.sufxvd.cn

PHP ............ 252
来源：http://vfw.yj202588.top

JavaScript ..... 252
来源：http://sga.cucudq.cn

TypeScript ..... 212
来源：http://fvt.xuetiantiany.cn

Java ........... 212
来源：http://wbe.hywenlv.cn

Go ............. 212
来源：http://ebf.52xcode.cn

Ruby ........... 212
来源：http://vrv.jqgufenzy.top

C# ............. 212
来源：http://zpm.gzhubu.top

C .............. 30
来源：http://ktw.yonumen.top

C++ ............ 30
来源：http://pjl.mhx1999.top

SQL ............ 90
来源：http://azj.cheryme.top

Bash ........... 80
来源：http://dcx.yj202588.top

Kotlin ......... 15
来源：http://qrk.cheryme.top

Swift .......... 15
来源：http://qmi.zhixingplan.top

Lua ............ 10
来源：http://shg.jiagoushi.top

Perl ........... 10
来源：http://krd.shanyushiyangkeji.top

Scala .......... 10
来源：http://pco.gzhubu.top

------------------------------------
来源：http://mbi.chenzaomai.com

合计 ........... 2106 条
来源：http://fcm.nanxinkj.top

按章节统计：
来源：http://ema.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bxn.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tnm.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ely.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dgv.yvedp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oim.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nmc.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cbd.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tyz.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://amq.pengpengdd.cyou

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sdk.0kj1m.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sos.jyoumei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://oys.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kbg.yvedp.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://igs.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://owk.zhengqikj.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iio.quarkkingdee.top

Q SQL 专题                              90
来源：http://dog.ydzc1.top

R Bash 专题                             80
来源：http://rhm.ctjpmb.com

S C / C++ 专题                          60
来源：http://rce.cqqwz.cn

T 其他语言补充                          60
来源：http://mkg.jinqigfzy.top

U 高频实用片段                         120
来源：http://syc.9152youxi.cn

------------------------------------
来源：http://fon.feifeiyinyue.top

合计                                  2106 条
来源：http://lwy.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://vvr.cucudq.cn

使用提醒
来源：http://tnt.epnwcf.com

--------------------------------------------------------------------------------
来源：http://oie.ppjwa.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wea.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aeb.fengsongda.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kdv.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://anl.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oip.yonumen.top

—— 文件结束 ——
来源：http://byi.hysaishi.cn

================================================================================
来源：http://byp.redwolf501.top

程序语言常见例子速查手册（2024 版）
来源：http://oqy.jianghu66.top

Common Programming Examples Cheat Book
来源：http://isj.shanyushiyangkeji.top

================================================================================
来源：http://tdj.fanxiaobao.xyz


<!-- 参考信息 -->