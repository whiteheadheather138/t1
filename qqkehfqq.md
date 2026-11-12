代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://yev.fehbvm.com

[T59] Scala：循环
来源：http://ocq.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://zuz.cdnleiting.top

[T60] Scala：折叠
来源：http://jpx.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aki.havefunace.top

================================================================================
来源：http://bbx.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hff.yfazqb.com

================================================================================
来源：http://hwe.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://oqs.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aqt.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://psr.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rdu.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://ktv.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kpu.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://dnn.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vgj.smart0.xyz

[U05] Py：列表去重且保序
来源：http://ssm.birdmap.top

list(dict.fromkeys(arr))
来源：http://cut.chenzaomai.com

[U06] Py：合并两个字典
来源：http://ifp.gotoacloud.top

{**a, **b}
来源：http://sgb.yonumen.top

[U07] Py：反转字典键值
来源：http://won.xinyue.icu

{v: k for k, v in d.items()}
来源：http://jyc.c1oappe.top

[U08] Py：展平二维列表
来源：http://rda.hcnkem.com

[y for x in nested for y in x]
来源：http://mix.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://pkd.yuxming.cn

max(d, key=d.get)
来源：http://sxs.zycfv.cn

[U10] Py：按值排序字典
来源：http://axi.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aik.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://unm.shuidangran.top

(x * 2 for x in arr)
来源：http://nbg.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rwj.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://mqg.sxryk.cn

[U13] Py：固定长度队列
来源：http://aux.9152youxi.cn

deque(maxlen=10)
来源：http://nev.pycfn.com

[U14] Py：分组收集到列表
来源：http://xrz.pycfn.com

defaultdict(list)
来源：http://vuo.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://dqn.fktsv.cn

t = time.perf_counter()
来源：http://ukq.sweek.top

[U16] Py：命令行参数解析
来源：http://osi.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dki.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://eyg.dianchejie.cn

logging.basicConfig(level=logging.INFO)
来源：http://qbc.sjlbkw.cn

[U18] Py：预编译正则
来源：http://kjh.zhoulong.xyz

pat = re.compile(r"\d+")
来源：http://rpi.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://brl.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jzf.zhijiandao.cn

[U20] Py：缓存函数结果
来源：http://awz.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://zwv.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://exy.vehdjk.com

@contextlib.contextmanager
来源：http://zrk.dianchejie.cn

[U22] Py：矩阵转置
来源：http://ihr.zhongyouzk.top

list(zip(*m))
来源：http://frh.shzxlz.cn

[U23] Py：分块读取大文件
来源：http://enc.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gjw.52xcode.cn

[U24] Py：路径操作
来源：http://ucy.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fya.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://myf.yuxming.cn

csv.DictReader(f)
来源：http://wnb.gogol.net.cn

[U26] Py：并发下载
来源：http://mfu.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mov.chenzaomai.com

[U27] Py：异步 HTTP
来源：http://mtf.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://dht.hcnkem.com

[U28] Py：类型别名
来源：http://wdo.ehwqpu.com

UserId = int
来源：http://akn.fehbvm.com

[U29] Py：属性校验
来源：http://lno.gogol.net.cn

@property 与 @x.setter 配合
来源：http://tlf.fanxiaobao.xyz

[U30] Py：数据类
来源：http://zsq.daxiang520.top

@dataclass(slots=True)
来源：http://lsz.shanyushiyangtech.top

[U31] Py：单测
来源：http://lrt.guowangkeji.top

python -m pytest -q
来源：http://zjz.zhoulong.xyz

[U32] Py：代码格式化
来源：http://phk.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://fnk.yj20258888.top

[U33] Py：打包发布
来源：http://wcf.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://mgo.hnxiangtu.top

[U34] Py：判断编码
来源：http://vnr.hfpthk.cn

chardet.detect(raw)
来源：http://zfe.birdmap.top

[U35] Py：发送邮件
来源：http://xoq.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://arh.sxryk.cn

[U36] Py：定时任务
来源：http://peb.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://vqe.fktsv.cn

[U37] Py：读写 Excel
来源：http://jvk.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://brs.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://pjg.316326.xyz

Path(__file__).resolve().parent
来源：http://iak.hnxiangtu.top

[U39] Py：判断是否在交互环境
来源：http://xvd.zhongyouzk.top

sys.stdout.isatty()
来源：http://cjm.snrcjt.cn

[U40] Py：打印到标准错误
来源：http://beq.hfpthk.cn

print("err", file=sys.stderr)
来源：http://bwv.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://jtg.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uyh.hnqzz.top

[U42] PHP：PSR-4 自动加载
来源：http://bnl.yanxiufei.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uqf.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://vpw.zdbjq.cn

namespace App\Http;
来源：http://itv.chenjidiqi.icu

[U44] PHP：开启严格类型
来源：http://eqq.hcnkem.com

declare(strict_types=1);
来源：http://efk.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://nvq.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xpn.zycfv.cn

[U46] PHP：可空类型
来源：http://uvi.jyoumei.cn

?string $name = null
来源：http://cjz.gogol.net.cn

[U47] PHP：联合类型
来源：http://bup.xingfuxueyuan.xyz

int|string $id
来源：http://lzu.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://vss.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vtl.jlsjyb.cn

[U49] PHP：只读属性
来源：http://txk.nanxuanxn.top

public readonly string $name
来源：http://irp.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://otf.sxryk.cn

public function __construct(private int $id) {}
来源：http://ncu.haohaochexian.top

[U51] PHP：数组解构
来源：http://kjt.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://cmt.shuidangran.top

[U52] PHP：箭头函数
来源：http://hid.tarul.cn

$double = fn($x) => $x * 2;
来源：http://mkh.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://awi.guannengcc.top

$v = $a ?? $b ?? "default";
来源：http://unu.ydjk.org.cn

[U54] PHP：空安全调用
来源：http://ezq.zhoulong.xyz

$obj?->method()
来源：http://sws.hongshengwenyu.top

[U55] PHP：match 表达式
来源：http://wne.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zmn.316326.xyz

[U56] PHP：命名参数
来源：http://qky.zhongyouzk.top

f(a: 1, b: 2)
来源：http://qtf.zycfv.cn

[U57] PHP：字符串插值
来源：http://syc.zdqjudy.top

"值: {$a}"
来源：http://yhy.sxryk.cn

[U58] PHP：数组三件套
来源：http://kag.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xbr.c1oappe.top

[U59] PHP：自定义排序
来源：http://rha.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://whb.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://oic.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://omr.xuetiantiany.cn

[U61] PHP：正则
来源：http://mmf.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ilg.sxryk.cn

[U62] PHP：日期对象
来源：http://raa.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://brh.haohaochexian.top

[U63] PHP：文件读写
来源：http://cel.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fsx.jianghu66.top

[U64] PHP：目录遍历
来源：http://vvc.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ltt.shuidangran.top

[U65] PHP：会话
来源：http://fpz.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://nnu.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://vcc.smart0.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ewr.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://bcm.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gwt.svipenyu.cn

[U68] PHP：PDO 连接
来源：http://ulp.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lta.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://njs.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mqi.hesvh.cn

[U70] PHP：PDO 事务
来源：http://wdg.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xbr.sweek.top

[U71] PHP：抛出异常
来源：http://iei.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://cbj.wangshuangyany.cn

[U72] PHP：写错误日志
来源：http://jbt.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://gmx.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://clu.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://app.xinyue.icu

[U74] PHP：读取环境变量
来源：http://xdj.bbcook.cn

getenv("APP_ENV") ?: "production"
来源：http://mew.chenjidiqi.icu

[U75] PHP：依赖注入
来源：http://gou.fengsongda.top

composer require psr/container
来源：http://icm.bbcook.cn

[U76] PHP：简单路由
来源：http://jxe.yj20258.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ntd.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://adc.nanxuanxn.top

composer require twig/twig
来源：http://orl.hcnkem.com

[U78] PHP：单元测试
来源：http://dlz.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://krz.fktsv.cn

[U79] PHP：静态分析
来源：http://ykv.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://mjn.yfazqb.com

[U80] PHP：代码规范修复
来源：http://rdr.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://koe.xinyue.icu

[U81] JS：初始化项目
来源：http://pse.andypj.xyz

npm init -y;  npm i express
来源：http://ohm.tarul.cn

[U82] JS：package.json 脚本
来源：http://mmw.feifeiyinyue.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lcd.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://txd.jqgufenzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://tkd.cheryme.top

[U84] JS：CommonJS 写法
来源：http://tlr.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://kmo.nanxinkj.top

[U85] JS：可选链
来源：http://dxt.hcnkem.com

a?.b?.c
来源：http://pya.hcnkem.com

[U86] JS：空值合并
来源：http://nqg.xingfuxueyuan.xyz

a ?? b
来源：http://nxz.tanke756.top

[U87] JS：解构默认值
来源：http://mdp.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://qht.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://ygt.shanyushiyangkeji.top

{ ...a, ...b }
来源：http://wzm.ivvv.top

[U89] JS：数组去重
来源：http://fwy.gzhubu.top

[...new Set(arr)]
来源：http://kig.snrcjt.cn

[U90] JS：数字数组排序
来源：http://jii.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://yny.cashguo.top

[U91] JS：对象键值遍历
来源：http://maf.yj202588.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xlz.sjlbkw.cn

[U92] JS：深拷贝
来源：http://gcy.hcnkem.com

structuredClone(obj)
来源：http://ltv.ppjwa.cn

[U93] JS：模板字符串
来源：http://lbz.zhoulong.xyz

`共 ${n} 条`
来源：http://ioe.zhengqikj.top

[U94] JS：箭头函数
来源：http://gpy.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://xib.shzxlz.cn

[U95] JS：Promise 包装
来源：http://dio.quarkkingdee.top

new Promise((resolve, reject) => {})
来源：http://nfn.cashguo.top

[U96] JS：async/await 与异常
来源：http://lro.jinqigufen.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vdq.zhiwuduotai.top

[U97] JS：并发请求
来源：http://xkd.hnqzz.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pwx.aizwys.cn

[U98] JS：fetch 带 JSON
来源：http://nrg.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tlc.fktsv.cn

[U99] JS：事件监听
来源：http://eqn.snrcjt.cn

el.addEventListener("click", e => {})
来源：http://hte.hnxiangtu.top

[U100] JS：DOM 查询
来源：http://xvk.gotoacloud.top

document.querySelector(".item")
来源：http://hzg.zdbjq.cn

[U101] JS：classList 操作
来源：http://vxa.andypj.xyz

el.classList.toggle("active")
来源：http://ssq.shuidangran.top

[U102] JS：本地存储
来源：http://heg.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hqv.cucudq.cn

[U103] JS：定时器
来源：http://dse.redwolf501.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vgi.cdnleiting.top

[U104] JS：防抖
来源：http://kmu.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vub.sjlbkw.cn

[U105] JS：节流
来源：http://qcx.redwolf501.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sjm.sufxvd.cn

[U106] JS：日期格式化
来源：http://yxz.zdqjudy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hqv.fehbvm.com

[U107] JS：数字千分位
来源：http://yxm.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pea.hywenlv.cn

[U108] JS：随机整数
来源：http://iew.c1oappe.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mux.cheryme.top

[U109] JS：数组分组
来源：http://xeg.gaohongyu789.top

Object.groupBy(arr, x => x.type)
来源：http://ewv.mhx1999.top

[U110] JS：数组分块
来源：http://fzd.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://szr.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://bwp.gotoacloud.top

new Map(Object.entries(obj))
来源：http://biw.xziqi.cn

[U112] JS：字符串补位
来源：http://axg.ehwqpu.com

"7".padStart(3, "0")
来源：http://yfq.mhx1999.top

[U113] JS：正则替换全部
来源：http://phj.cucudq.cn

s.replaceAll("a", "b")
来源：http://kuy.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://zey.sweek.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mxy.zycfv.cn

[U115] JS：生成 UUID
来源：http://wnp.ctjpmb.com

crypto.randomUUID()
来源：http://wsc.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://ctl.yanxiufei.cn

/** @param {string} name */ function f(name) {}
来源：http://hik.daria6918.cn

[U117] JS：单元测试
来源：http://ssa.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://reb.shzxlz.cn

[U118] JS：开发服务器
来源：http://uad.vehdjk.com

npm i -D vite;  npx vite
来源：http://kvy.zycfv.cn

[U119] JS：生产构建
来源：http://iku.hcnkem.com

npx vite build
来源：http://qqz.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://vul.ydjk.org.cn

import.meta.env.VITE_API_URL
来源：http://osc.jinqigufen.top

================================================================================
来源：http://xdf.dashuyun.cn

统计汇总
来源：http://mvx.gaohongyu789.top

================================================================================
来源：http://jyt.yonumen.top

按语言统计（条）：
来源：http://ydo.yangfankeji.com

Python ......... 252
来源：http://dwq.bjfxy.top

PHP ............ 252
来源：http://zrt.feifeiyinyue.top

JavaScript ..... 252
来源：http://tae.xingfuxueyuan.xyz

TypeScript ..... 212
来源：http://mjj.hcnkem.com

Java ........... 212
来源：http://lak.chenzaomai.com

Go ............. 212
来源：http://kvh.xuanzx.com

Ruby ........... 212
来源：http://mog.kuanghao11.cn

C# ............. 212
来源：http://ddz.gzhubu.top

C .............. 30
来源：http://zzx.epnwcf.com

C++ ............ 30
来源：http://rtb.vqdsnc.cn

SQL ............ 90
来源：http://wur.yfazqb.com

Bash ........... 80
来源：http://ehe.hesvh.cn

Kotlin ......... 15
来源：http://exe.jiagoushi.top

Swift .......... 15
来源：http://udk.316326.xyz

Lua ............ 10
来源：http://yod.tanke756.top

Perl ........... 10
来源：http://qwb.redwolf501.top

Scala .......... 10
来源：http://bik.cdnleiting.top

------------------------------------
来源：http://coh.uphjek.com

合计 ........... 2106 条
来源：http://iya.feifeiyinyue.top

按章节统计：
来源：http://yuk.yueranfly.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zkt.jinyuanbaomall.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nty.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ggv.sufxvd.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ssx.nanxuanxn.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wgy.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bwx.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lsc.dashuyun.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://afc.andypj.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rhc.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vyf.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://opj.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bhe.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pye.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gkz.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wpq.wangshuangyany.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tsm.zycfv.cn

Q SQL 专题                              90
来源：http://fbo.aibaodan.cn

R Bash 专题                             80
来源：http://ofm.quarkkingdee.top

S C / C++ 专题                          60
来源：http://bca.zycfv.cn

T 其他语言补充                          60
来源：http://ndf.cheryme.top

U 高频实用片段                         120
来源：http://xlu.ywan-chungtsiang.top

------------------------------------
来源：http://bbv.tianlin.xyz

合计                                  2106 条
来源：http://esf.yj202588.top

--------------------------------------------------------------------------------
来源：http://drv.pycfn.com

使用提醒
来源：http://qcz.fanxiaobao.xyz

--------------------------------------------------------------------------------
来源：http://zhk.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rar.fktsv.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://idt.xuetiantiany.cn


<!-- 参考信息 -->