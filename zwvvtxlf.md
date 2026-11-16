代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nqf.52xcode.cn

================================================================================
来源：http://hkl.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qqx.zycfv.cn

================================================================================
来源：http://hen.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://xjp.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://cie.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://hsm.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ybr.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://wow.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wmh.c1oappe.top

[U04] Py：变量调试打印
来源：http://rmx.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://roz.dashuyun.cn

[U05] Py：列表去重且保序
来源：http://fab.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://vpx.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://soc.yfazqb.com

{**a, **b}
来源：http://sux.tarul.cn

[U07] Py：反转字典键值
来源：http://zye.xinyue.icu

{v: k for k, v in d.items()}
来源：http://fgh.zdbjq.cn

[U08] Py：展平二维列表
来源：http://bdk.ivvv.top

[y for x in nested for y in x]
来源：http://nwo.hammf.cn

[U09] Py：字典取最大值的键
来源：http://ptd.xylfe.cn

max(d, key=d.get)
来源：http://xeq.ppjwa.cn

[U10] Py：按值排序字典
来源：http://azr.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oem.pycfn.com

[U11] Py：生成器表达式
来源：http://dhb.xuanzx.com

(x * 2 for x in arr)
来源：http://bad.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mdf.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://vdi.yuxming.cn

[U13] Py：固定长度队列
来源：http://owj.fehbvm.com

deque(maxlen=10)
来源：http://sah.uphjek.com

[U14] Py：分组收集到列表
来源：http://mup.fengsongda.top

defaultdict(list)
来源：http://rse.sweek.top

[U15] Py：高精度计时
来源：http://kbz.yonumen.top

t = time.perf_counter()
来源：http://jqp.iojbl.cn

[U16] Py：命令行参数解析
来源：http://qqf.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jqu.xinyue.icu

[U17] Py：初始化日志
来源：http://wwv.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://amg.cashguo.top

[U18] Py：预编译正则
来源：http://uzj.cucudq.cn

pat = re.compile(r"\d+")
来源：http://njj.hesvh.cn

[U19] Py：正则替换带回调
来源：http://cje.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jms.sxryk.cn

[U20] Py：缓存函数结果
来源：http://zvj.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://gxn.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://zcz.xinyue.icu

@contextlib.contextmanager
来源：http://zqf.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://hud.aibaodan.cn

list(zip(*m))
来源：http://tqj.c1oappe.top

[U23] Py：分块读取大文件
来源：http://oox.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tnp.jianghu66.top

[U24] Py：路径操作
来源：http://awe.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bqf.tarul.cn

[U25] Py：CSV 按字典读
来源：http://ocw.hcnkem.com

csv.DictReader(f)
来源：http://dzx.hammf.cn

[U26] Py：并发下载
来源：http://cnm.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pcz.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://qic.redwolf501.top

aiohttp.ClientSession() 配合 async with
来源：http://cjv.wangshuangyany.cn

[U28] Py：类型别名
来源：http://bud.sxryk.cn

UserId = int
来源：http://rdr.meibo888.top

[U29] Py：属性校验
来源：http://phs.hammf.cn

@property 与 @x.setter 配合
来源：http://ntx.snrcjt.cn

[U30] Py：数据类
来源：http://ysj.52xcode.cn

@dataclass(slots=True)
来源：http://bqq.guowangkeji.top

[U31] Py：单测
来源：http://dpy.guowangkeji.top

python -m pytest -q
来源：http://mwa.cashguo.top

[U32] Py：代码格式化
来源：http://lhm.c1oappe.top

ruff format . && ruff check --fix .
来源：http://xun.cheryme.top

[U33] Py：打包发布
来源：http://ols.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://ogu.mhx1999.top

[U34] Py：判断编码
来源：http://jlz.haohaochexian.top

chardet.detect(raw)
来源：http://qwi.nwbrower.top

[U35] Py：发送邮件
来源：http://ajn.c1oappe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iaw.fzhhl.top

[U36] Py：定时任务
来源：http://fzy.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://egm.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://gyr.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ejm.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://ocv.birdmap.top

Path(__file__).resolve().parent
来源：http://tny.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://rkc.hammf.cn

sys.stdout.isatty()
来源：http://xnh.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://zdt.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://ktd.quarkkingdee.top

[U41] PHP：初始化 Composer 项目
来源：http://xxx.gotoacloud.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vlf.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hgk.9152youxi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jmd.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://cdg.haohaochexian.top

namespace App\Http;
来源：http://lru.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://wds.mhx1999.top

declare(strict_types=1);
来源：http://vcr.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://wai.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://emr.gaohongyu789.top

[U46] PHP：可空类型
来源：http://hfl.yj202588.top

?string $name = null
来源：http://ujn.nwbrower.top

[U47] PHP：联合类型
来源：http://vin.jinghuilouyu.cn

int|string $id
来源：http://asu.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://fcd.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wsz.ehwqpu.com

[U49] PHP：只读属性
来源：http://dqb.hcnkem.com

public readonly string $name
来源：http://wba.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://ezt.fehbvm.com

public function __construct(private int $id) {}
来源：http://gyr.jinqigfzy.top

[U51] PHP：数组解构
来源：http://tzh.wangdashe.top

[$a, $b] = $arr;
来源：http://khv.cucudq.cn

[U52] PHP：箭头函数
来源：http://qch.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://pqy.ivvv.top

[U53] PHP：空合并运算符
来源：http://tbw.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://vpj.316326.xyz

[U54] PHP：空安全调用
来源：http://vmf.jyoumei.cn

$obj?->method()
来源：http://giv.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://czm.yonumen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xnk.hammf.cn

[U56] PHP：命名参数
来源：http://xse.daxiang520.top

f(a: 1, b: 2)
来源：http://jtf.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://mzo.pycfn.com

"值: {$a}"
来源：http://dzr.316326.xyz

[U58] PHP：数组三件套
来源：http://txu.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qev.chenzaomai.com

[U59] PHP：自定义排序
来源：http://jsk.xylfe.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dwi.hesvh.cn

[U60] PHP：JSON 编解码
来源：http://git.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fcr.daria6918.cn

[U61] PHP：正则
来源：http://pmc.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rtt.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://jxc.zhongyouzk.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://evj.nanxuanxn.top

[U63] PHP：文件读写
来源：http://ycc.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ydz.fzhhl.top

[U64] PHP：目录遍历
来源：http://cxf.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://waq.ivvv.top

[U65] PHP：会话
来源：http://yom.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rjp.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://urm.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cai.cqqwz.cn

[U67] PHP：处理文件上传
来源：http://yau.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gzv.kuanghao11.cn

[U68] PHP：PDO 连接
来源：http://mje.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://poh.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://mii.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lob.hammf.cn

[U70] PHP：PDO 事务
来源：http://ozq.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fkl.chenzaomai.com

[U71] PHP：抛出异常
来源：http://oxk.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://lzj.birdmap.top

[U72] PHP：写错误日志
来源：http://kti.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://wcp.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://nek.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://pww.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://crh.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://ykq.xuanzx.com

[U75] PHP：依赖注入
来源：http://vbu.xziqi.cn

composer require psr/container
来源：http://npc.fzhhl.top

[U76] PHP：简单路由
来源：http://ozo.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xkw.nwbrower.top

[U77] PHP：模板渲染
来源：http://kix.ydjk.org.cn

composer require twig/twig
来源：http://zyz.jqgufenzy.top

[U78] PHP：单元测试
来源：http://aio.ppjwa.cn

composer require --dev phpunit/phpunit
来源：http://ipx.yj20258888.top

[U79] PHP：静态分析
来源：http://jrb.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://ghd.c1oappe.top

[U80] PHP：代码规范修复
来源：http://uxu.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://izl.jinqigufen.top

[U81] JS：初始化项目
来源：http://cya.sysykeji.top

npm init -y;  npm i express
来源：http://ebb.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://xmv.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ahc.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://vpt.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://jsu.cheryme.top

[U84] JS：CommonJS 写法
来源：http://opa.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://rbv.jqgfzy.top

[U85] JS：可选链
来源：http://hln.zhijiandao.cn

a?.b?.c
来源：http://diw.jyoumei.cn

[U86] JS：空值合并
来源：http://mqb.ivvv.top

a ?? b
来源：http://ruw.yuanzhike.top

[U87] JS：解构默认值
来源：http://dxf.c1oappe.top

const { a = 1, b = 2 } = obj;
来源：http://gpb.yuanzhike.top

[U88] JS：对象展开合并
来源：http://eqr.yongpay.top

{ ...a, ...b }
来源：http://gkr.ydjk.org.cn

[U89] JS：数组去重
来源：http://rqn.ppjwa.cn

[...new Set(arr)]
来源：http://maf.zdbjq.cn

[U90] JS：数字数组排序
来源：http://aqc.jinqigufen.top

[...arr].sort((a, b) => a - b)
来源：http://xnn.ybcxt.top

[U91] JS：对象键值遍历
来源：http://mry.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ube.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://nuc.sufxvd.cn

structuredClone(obj)
来源：http://zdd.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://qzu.jqgufenzy.top

`共 ${n} 条`
来源：http://uhl.zdqjudy.top

[U94] JS：箭头函数
来源：http://egi.meibo888.top

const double = x => x * 2;
来源：http://kxy.mhx1999.top

[U95] JS：Promise 包装
来源：http://sqw.fktsv.cn

new Promise((resolve, reject) => {})
来源：http://zgn.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://jca.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://top.bbcook.cn

[U97] JS：并发请求
来源：http://evy.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lxg.xingfuxueyuan.xyz

[U98] JS：fetch 带 JSON
来源：http://lau.smart0.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ren.yuxming.cn

[U99] JS：事件监听
来源：http://haq.yj202588.top

el.addEventListener("click", e => {})
来源：http://qxp.zhiwuduotai.top

[U100] JS：DOM 查询
来源：http://ttj.ybcxt.top

document.querySelector(".item")
来源：http://upd.epnwcf.com

[U101] JS：classList 操作
来源：http://uqs.meibo888.top

el.classList.toggle("active")
来源：http://hpp.cashguo.top

[U102] JS：本地存储
来源：http://bfs.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jfk.ppjwa.cn

[U103] JS：定时器
来源：http://jjf.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ijx.jiagoushi.top

[U104] JS：防抖
来源：http://rna.jinghuilouyu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lle.tianlin.xyz

[U105] JS：节流
来源：http://tyj.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ksh.pycfn.com

[U106] JS：日期格式化
来源：http://sxp.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xyu.dashuyun.cn

[U107] JS：数字千分位
来源：http://qfv.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gbk.quarkkingdee.top

[U108] JS：随机整数
来源：http://lhm.aibaodan.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://did.chenlongwang.top

[U109] JS：数组分组
来源：http://evh.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://vvh.iojbl.cn

[U110] JS：数组分块
来源：http://miv.ppjwa.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bor.9152youxi.cn

[U111] JS：对象转 Map
来源：http://nri.dashuyun.cn

new Map(Object.entries(obj))
来源：http://loa.cucudq.cn

[U112] JS：字符串补位
来源：http://qiq.zhiwuduotai.top

"7".padStart(3, "0")
来源：http://jmq.xuanzx.com

[U113] JS：正则替换全部
来源：http://udg.sxryk.cn

s.replaceAll("a", "b")
来源：http://qdj.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://jvf.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lyw.aizwys.cn

[U115] JS：生成 UUID
来源：http://lvu.sxryk.cn

crypto.randomUUID()
来源：http://lnz.hesvh.cn

[U116] JS：类型检查（JSDoc）
来源：http://dam.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://rjl.zdbjq.cn

[U117] JS：单元测试
来源：http://bpe.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://jrw.aizwys.cn

[U118] JS：开发服务器
来源：http://arg.shuidangran.top

npm i -D vite;  npx vite
来源：http://atu.52xcode.cn

[U119] JS：生产构建
来源：http://tas.gogol.net.cn

npx vite build
来源：http://llb.shanyushiyangtech.top

[U120] JS：读取环境变量（Vite）
来源：http://fqr.jiagoushi.top

import.meta.env.VITE_API_URL
来源：http://ztk.9152youxi.cn

================================================================================
来源：http://dtd.dianchejie.cn

统计汇总
来源：http://phr.zycfv.cn

================================================================================
来源：http://vty.hfpthk.cn

按语言统计（条）：
来源：http://ltd.guannengcc.top

Python ......... 252
来源：http://xaa.redwolf501.top

PHP ............ 252
来源：http://pja.yj202588.top

JavaScript ..... 252
来源：http://aoe.sufxvd.cn

TypeScript ..... 212
来源：http://peb.xuetiantiany.cn

Java ........... 212
来源：http://nwp.jianghu66.top

Go ............. 212
来源：http://eqn.xuetiantiany.cn

Ruby ........... 212
来源：http://ntx.xingfuxueyuan.xyz

C# ............. 212
来源：http://hrk.yfazqb.com

C .............. 30
来源：http://ujd.feifeiyinyue.top

C++ ............ 30
来源：http://kvu.smart0.xyz

SQL ............ 90
来源：http://ssw.dashuyun.cn

Bash ........... 80
来源：http://uag.zdbjq.cn

Kotlin ......... 15
来源：http://mpc.nanxuanxn.top

Swift .......... 15
来源：http://iud.yvedp.cn

Lua ............ 10
来源：http://tss.shuidangran.top

Perl ........... 10
来源：http://cez.ppjwa.cn

Scala .......... 10
来源：http://rwp.fanxiaobao.xyz

------------------------------------
来源：http://ttu.cucudq.cn

合计 ........... 2106 条
来源：http://dhr.yonumen.top

按章节统计：
来源：http://jbm.yj202588.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://msl.redwolf501.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hek.hnxiangtu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://siq.shanyushiyangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wah.xinyue.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pyf.bbcook.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mea.wangdashe.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xkc.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://diq.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bxb.yuanzhike.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qhf.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fdx.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://soy.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://efl.uphjek.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ztm.yfazqb.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://npt.zhaomingkeji.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hmp.bbcook.cn

Q SQL 专题                              90
来源：http://wyv.gotoacloud.top

R Bash 专题                             80
来源：http://xxg.shanyushiyangtech.top

S C / C++ 专题                          60
来源：http://zbx.shzxlz.cn

T 其他语言补充                          60
来源：http://dkw.meibo888.top

U 高频实用片段                         120
来源：http://kse.hnqzz.top

------------------------------------
来源：http://qpw.ivvv.top

合计                                  2106 条
来源：http://pfw.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://dce.zhaomingkeji.xyz

使用提醒
来源：http://snq.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://ktw.snrcjt.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://epm.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vdh.fzhhl.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zov.hysaishi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bzy.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://uef.zhiwuduotai.top

—— 文件结束 ——
来源：http://cqw.sweek.top


<!-- 参考信息 -->