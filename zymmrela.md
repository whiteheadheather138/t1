代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://msu.meibo888.top

[T59] Scala：循环
来源：http://hod.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://fec.jlsjyb.cn

[T60] Scala：折叠
来源：http://nga.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lvx.ywan-chungtsiang.top

================================================================================
来源：http://vns.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lth.yuxming.cn

================================================================================
来源：http://teb.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://ibx.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qeg.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://rzi.andypj.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://upr.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://non.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pwd.dashuyun.cn

[U04] Py：变量调试打印
来源：http://vty.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wdg.fengsongda.top

[U05] Py：列表去重且保序
来源：http://kfa.xinyue.icu

list(dict.fromkeys(arr))
来源：http://neg.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://tlm.hywenlv.cn

{**a, **b}
来源：http://apn.xziqi.cn

[U07] Py：反转字典键值
来源：http://gie.bjfxy.top

{v: k for k, v in d.items()}
来源：http://zoo.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://twp.ctjpmb.com

[y for x in nested for y in x]
来源：http://nvb.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://kgo.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://frb.gogol.net.cn

[U10] Py：按值排序字典
来源：http://abd.meibo888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cfl.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://nen.smart0.xyz

(x * 2 for x in arr)
来源：http://mvp.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://odr.cashguo.top

Counter(arr).most_common(3)
来源：http://wfq.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://tkr.zhiwuduotai.top

deque(maxlen=10)
来源：http://svk.iojbl.cn

[U14] Py：分组收集到列表
来源：http://ohp.cqqwz.cn

defaultdict(list)
来源：http://xdu.yonumen.top

[U15] Py：高精度计时
来源：http://whq.chenlongwang.top

t = time.perf_counter()
来源：http://vyy.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://fim.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rkj.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://tou.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://trp.yuanzhike.top

[U18] Py：预编译正则
来源：http://zsw.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://pyq.zycfv.cn

[U19] Py：正则替换带回调
来源：http://bis.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jbv.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://umf.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://omo.meibo888.top

[U21] Py：自定义上下文管理器
来源：http://utf.hnxiangtu.top

@contextlib.contextmanager
来源：http://zgd.zycfv.cn

[U22] Py：矩阵转置
来源：http://dnt.cashguo.top

list(zip(*m))
来源：http://bhw.hammf.cn

[U23] Py：分块读取大文件
来源：http://miy.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://udt.xuetiantiany.cn

[U24] Py：路径操作
来源：http://knz.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rri.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://zoi.yfazqb.com

csv.DictReader(f)
来源：http://kkd.dianchejie.cn

[U26] Py：并发下载
来源：http://rdd.vehdjk.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jek.yj20258.top

[U27] Py：异步 HTTP
来源：http://fkl.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://fif.cheryme.top

[U28] Py：类型别名
来源：http://hok.jqgfzy.top

UserId = int
来源：http://dtx.daria6918.cn

[U29] Py：属性校验
来源：http://ica.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://uhq.yuanzhike.top

[U30] Py：数据类
来源：http://gdg.shuidangran.top

@dataclass(slots=True)
来源：http://smo.yueranfly.top

[U31] Py：单测
来源：http://sqz.gzhubu.top

python -m pytest -q
来源：http://mlf.ydjk.org.cn

[U32] Py：代码格式化
来源：http://tkw.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://lsp.yvedp.cn

[U33] Py：打包发布
来源：http://qfg.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://bcp.zhongyouzk.top

[U34] Py：判断编码
来源：http://wmx.uphjek.com

chardet.detect(raw)
来源：http://uzu.epnwcf.com

[U35] Py：发送邮件
来源：http://awg.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qxd.haohaochexian.top

[U36] Py：定时任务
来源：http://fot.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://pqb.cashguo.top

[U37] Py：读写 Excel
来源：http://fdp.yj202588.top

pandas.read_excel / DataFrame.to_excel
来源：http://mne.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://kfz.aizwys.cn

Path(__file__).resolve().parent
来源：http://gxy.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://kcj.cdnleiting.top

sys.stdout.isatty()
来源：http://kll.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://kod.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://xnz.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://xmw.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tvf.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://mca.pycfn.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bkk.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://rqr.jiagoushi.top

namespace App\Http;
来源：http://lsv.vehdjk.com

[U44] PHP：开启严格类型
来源：http://sxe.bbcook.cn

declare(strict_types=1);
来源：http://djx.aibaodan.cn

[U45] PHP：类型声明与返回类型
来源：http://trw.jinqigufen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://yip.iojbl.cn

[U46] PHP：可空类型
来源：http://fwd.zhixingplan.top

?string $name = null
来源：http://tmz.jiagoushi.top

[U47] PHP：联合类型
来源：http://dty.wangdashe.top

int|string $id
来源：http://imq.xylfe.cn

[U48] PHP：纯枚举
来源：http://mpy.iojbl.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gpx.cqqwz.cn

[U49] PHP：只读属性
来源：http://svp.zdqjudy.top

public readonly string $name
来源：http://unr.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://mmc.hongshengwenyu.top

public function __construct(private int $id) {}
来源：http://nsy.bjfxy.top

[U51] PHP：数组解构
来源：http://vpm.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://zpi.guowangkeji.top

[U52] PHP：箭头函数
来源：http://wxy.316326.xyz

$double = fn($x) => $x * 2;
来源：http://lcq.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://zmj.sweek.top

$v = $a ?? $b ?? "default";
来源：http://qpn.epnwcf.com

[U54] PHP：空安全调用
来源：http://sln.ppjwa.cn

$obj?->method()
来源：http://kpw.jiagoushi.top

[U55] PHP：match 表达式
来源：http://nwv.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://djp.gogol.net.cn

[U56] PHP：命名参数
来源：http://fqq.zdbjq.cn

f(a: 1, b: 2)
来源：http://lwt.zycfv.cn

[U57] PHP：字符串插值
来源：http://mvk.guannengcc.top

"值: {$a}"
来源：http://xoa.smart0.xyz

[U58] PHP：数组三件套
来源：http://wmk.ctjpmb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://muy.ivvv.top

[U59] PHP：自定义排序
来源：http://ctl.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mld.xylfe.cn

[U60] PHP：JSON 编解码
来源：http://mmd.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://poo.sjlbkw.cn

[U61] PHP：正则
来源：http://itd.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pzw.hywenlv.cn

[U62] PHP：日期对象
来源：http://znn.jinqigfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://adk.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://tja.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ugc.zhiwuduotai.top

[U64] PHP：目录遍历
来源：http://hck.gotoacloud.top

glob("dir/*.php");  scandir("dir");
来源：http://qia.zhijiandao.cn

[U65] PHP：会话
来源：http://ryb.sweek.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ocu.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://eyy.gaohongyu789.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wkw.yuxming.cn

[U67] PHP：处理文件上传
来源：http://xpr.nwbrower.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qrw.guannengcc.top

[U68] PHP：PDO 连接
来源：http://bgv.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cjv.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://yye.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vlr.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://cwn.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kbp.tarul.cn

[U71] PHP：抛出异常
来源：http://yfn.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://xpu.jiagoushi.top

[U72] PHP：写错误日志
来源：http://bzf.zhiwuduotai.top

error_log("失败: " . $e->getMessage());
来源：http://rxd.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://oji.daria6918.cn

parse_ini_file("config.ini", true)
来源：http://cvw.xuetiantiany.cn

[U74] PHP：读取环境变量
来源：http://xjn.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://knh.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://zzl.bjfxy.top

composer require psr/container
来源：http://iou.jlsjyb.cn

[U76] PHP：简单路由
来源：http://khd.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fxv.gzhubu.top

[U77] PHP：模板渲染
来源：http://gkr.sufxvd.cn

composer require twig/twig
来源：http://nkj.jqgufenzy.top

[U78] PHP：单元测试
来源：http://vsi.fengsongda.top

composer require --dev phpunit/phpunit
来源：http://gaw.epnwcf.com

[U79] PHP：静态分析
来源：http://aqb.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://pcr.xinyue.icu

[U80] PHP：代码规范修复
来源：http://fuw.mhx1999.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xuo.sxryk.cn

[U81] JS：初始化项目
来源：http://frj.tarul.cn

npm init -y;  npm i express
来源：http://pse.yonumen.top

[U82] JS：package.json 脚本
来源：http://ibs.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tve.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://dnj.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://uti.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://jhp.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://hcw.yanxiufei.cn

[U85] JS：可选链
来源：http://gat.xinyue.icu

a?.b?.c
来源：http://bvb.chenjidiqi.icu

[U86] JS：空值合并
来源：http://eww.xziqi.cn

a ?? b
来源：http://ixk.uphjek.com

[U87] JS：解构默认值
来源：http://hnp.cucudq.cn

const { a = 1, b = 2 } = obj;
来源：http://msl.nwbrower.top

[U88] JS：对象展开合并
来源：http://ahe.ybcxt.top

{ ...a, ...b }
来源：http://ope.shzxlz.cn

[U89] JS：数组去重
来源：http://dwl.jianghu66.top

[...new Set(arr)]
来源：http://tqb.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://tcj.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://rcr.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://pmi.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tbr.yj202588.top

[U92] JS：深拷贝
来源：http://rub.fzhhl.top

structuredClone(obj)
来源：http://yds.cdnleiting.top

[U93] JS：模板字符串
来源：http://lbu.zhixingplan.top

`共 ${n} 条`
来源：http://scq.daria6918.cn

[U94] JS：箭头函数
来源：http://atc.shzxlz.cn

const double = x => x * 2;
来源：http://jps.nanxinkj.top

[U95] JS：Promise 包装
来源：http://nen.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://xls.xziqi.cn

[U96] JS：async/await 与异常
来源：http://xbt.yj202588.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zni.cucudq.cn

[U97] JS：并发请求
来源：http://wek.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://gng.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://lmz.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jzi.meibo888.top

[U99] JS：事件监听
来源：http://qpb.jianghu66.top

el.addEventListener("click", e => {})
来源：http://hsx.316326.xyz

[U100] JS：DOM 查询
来源：http://ota.zhongyouzk.top

document.querySelector(".item")
来源：http://qkm.yuanzhike.top

[U101] JS：classList 操作
来源：http://fdl.sxryk.cn

el.classList.toggle("active")
来源：http://obw.vqdsnc.cn

[U102] JS：本地存储
来源：http://iuu.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://egq.jiagoushi.top

[U103] JS：定时器
来源：http://kiz.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gep.jiagoushi.top

[U104] JS：防抖
来源：http://wwx.jinqigfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wig.zhiwuduotai.top

[U105] JS：节流
来源：http://yud.xuetiantiany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://joy.zhiwuduotai.top

[U106] JS：日期格式化
来源：http://dog.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lfe.zhoulong.xyz

[U107] JS：数字千分位
来源：http://eux.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ptt.jlsjyb.cn

[U108] JS：随机整数
来源：http://qer.xylfe.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ndh.chenzaomai.com

[U109] JS：数组分组
来源：http://dfw.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://xny.gotoacloud.top

[U110] JS：数组分块
来源：http://gdm.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://moj.guannengcc.top

[U111] JS：对象转 Map
来源：http://wvp.havefunace.top

new Map(Object.entries(obj))
来源：http://hjt.bjfxy.top

[U112] JS：字符串补位
来源：http://euv.redwolf501.top

"7".padStart(3, "0")
来源：http://aaj.guowangkeji.top

[U113] JS：正则替换全部
来源：http://amq.sufxvd.cn

s.replaceAll("a", "b")
来源：http://smr.ppjwa.cn

[U114] JS：JSON 深比较
来源：http://iue.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://cyd.gotoacloud.top

[U115] JS：生成 UUID
来源：http://cpe.sjlbkw.cn

crypto.randomUUID()
来源：http://dfs.vqdsnc.cn

[U116] JS：类型检查（JSDoc）
来源：http://jmg.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://afv.sufxvd.cn

[U117] JS：单元测试
来源：http://kcm.pycfn.com

npm i -D vitest;  npx vitest
来源：http://cti.ydzc1.top

[U118] JS：开发服务器
来源：http://zkt.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://pbs.chenzaomai.com

[U119] JS：生产构建
来源：http://puo.gogol.net.cn

npx vite build
来源：http://iwk.wangdashe.top

[U120] JS：读取环境变量（Vite）
来源：http://nmi.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://laa.hysaishi.cn

================================================================================
来源：http://liu.sufxvd.cn

统计汇总
来源：http://lid.zhengqikj.top

================================================================================
来源：http://zax.aibaodan.cn

按语言统计（条）：
来源：http://sls.quarkkingdee.top

Python ......... 252
来源：http://ymy.iojbl.cn

PHP ............ 252
来源：http://mog.hnxiangtu.top

JavaScript ..... 252
来源：http://ofz.hcnkem.com

TypeScript ..... 212
来源：http://hmo.feifeiyinyue.top

Java ........... 212
来源：http://irv.jinyuanbaomall.cn

Go ............. 212
来源：http://dqd.guannengcc.top

Ruby ........... 212
来源：http://exl.ybcxt.top

C# ............. 212
来源：http://yjd.pycfn.com

C .............. 30
来源：http://flk.pycfn.com

C++ ............ 30
来源：http://eul.shanyushiyangkeji.top

SQL ............ 90
来源：http://ngk.hammf.cn

Bash ........... 80
来源：http://rjt.xuetiantiany.cn

Kotlin ......... 15
来源：http://zut.zhaomingkeji.xyz

Swift .......... 15
来源：http://bqy.cucudq.cn

Lua ............ 10
来源：http://rbw.mhx1999.top

Perl ........... 10
来源：http://nnp.andypj.xyz

Scala .......... 10
来源：http://orm.zdqjudy.top

------------------------------------
来源：http://ywt.aibaodan.cn

合计 ........... 2106 条
来源：http://rrh.meibo888.top

按章节统计：
来源：http://kvk.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jtd.jinqigfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kdt.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pop.zycfv.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://erm.shzxlz.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pct.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rtb.sufxvd.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vge.tanke756.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ouk.jlsjyb.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uvm.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wlk.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zfq.xziqi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kjz.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdm.bjfxy.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ksu.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dls.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qke.shangyingyoupin.top

Q SQL 专题                              90
来源：http://ifn.andypj.xyz

R Bash 专题                             80
来源：http://vgz.yj20258.top

S C / C++ 专题                          60
来源：http://bmn.sufxvd.cn

T 其他语言补充                          60
来源：http://ppp.yj20258888.top

U 高频实用片段                         120
来源：http://mra.hywenlv.cn

------------------------------------
来源：http://sxw.yongpay.top

合计                                  2106 条
来源：http://qst.hnqzz.top

--------------------------------------------------------------------------------
来源：http://pat.mhx1999.top

使用提醒
来源：http://vtv.yonumen.top

--------------------------------------------------------------------------------
来源：http://jjm.zhongyouzk.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gtu.jiagoushi.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xkm.ydzc1.top


<!-- 参考信息 -->