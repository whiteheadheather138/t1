代发 wailian999

[T49] Perl：函数
来源：http://zdf.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://daq.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://ors.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zjj.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://htb.c1oappe.top

[T51] Scala：Hello World
来源：http://zcx.fktsv.cn

println("Hello")
来源：http://uke.quarkkingdee.top

[T52] Scala：变量
来源：http://whg.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://ofw.gotoacloud.top

[T53] Scala：字符串插值
来源：http://yma.meibo888.top

s"值: $b"
来源：http://dte.yvedp.cn

[T54] Scala：集合映射
来源：http://ztr.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://pva.birdmap.top

[T55] Scala：集合过滤
来源：http://vcl.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://jxc.haohaochexian.top

[T56] Scala：样例类
来源：http://vjm.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://tqn.zycfv.cn

[T57] Scala：模式匹配
来源：http://dkh.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://svb.yuxming.cn

[T58] Scala：函数定义
来源：http://crr.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bxt.gaohongyu789.top

[T59] Scala：循环
来源：http://diw.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://mnc.fengsongda.top

[T60] Scala：折叠
来源：http://gso.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mmt.daria6918.cn

================================================================================
来源：http://gwx.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dcy.zhixingplan.top

================================================================================
来源：http://vjg.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://plv.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://svh.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://izq.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qgz.sjlbkw.cn

[U03] Py：加载 .env 配置
来源：http://tpg.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://rtt.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://hrj.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lrs.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://qft.pycfn.com

list(dict.fromkeys(arr))
来源：http://epm.gzhubu.top

[U06] Py：合并两个字典
来源：http://xoo.vqdsnc.cn

{**a, **b}
来源：http://bpy.xinyue.icu

[U07] Py：反转字典键值
来源：http://oqg.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://fqu.yfazqb.com

[U08] Py：展平二维列表
来源：http://ehj.yangfankeji.com

[y for x in nested for y in x]
来源：http://fwn.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://fza.zhengqikj.top

max(d, key=d.get)
来源：http://kgh.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://kqf.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zur.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://ehl.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://bqo.jiagoushi.top

[U12] Py：取出现最多的 3 个元素
来源：http://qmz.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://zyn.chenjidiqi.icu

[U13] Py：固定长度队列
来源：http://oqx.haohaochexian.top

deque(maxlen=10)
来源：http://qbj.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://xqc.shanyushiyangtech.top

defaultdict(list)
来源：http://fyv.ehwqpu.com

[U15] Py：高精度计时
来源：http://act.wangdashe.top

t = time.perf_counter()
来源：http://fov.zycfv.cn

[U16] Py：命令行参数解析
来源：http://jvh.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ext.tarul.cn

[U17] Py：初始化日志
来源：http://wgr.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://hdz.9152youxi.cn

[U18] Py：预编译正则
来源：http://jne.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://qif.iojbl.cn

[U19] Py：正则替换带回调
来源：http://mfa.jqgfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ouc.fanxiaobao.xyz

[U20] Py：缓存函数结果
来源：http://fel.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://ace.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://dvb.xylfe.cn

@contextlib.contextmanager
来源：http://gjh.zdbjq.cn

[U22] Py：矩阵转置
来源：http://zvi.gzhubu.top

list(zip(*m))
来源：http://bcf.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://xxd.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jgu.tarul.cn

[U24] Py：路径操作
来源：http://tui.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vwl.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://lrk.jianghu66.top

csv.DictReader(f)
来源：http://aww.shangyingyoupin.top

[U26] Py：并发下载
来源：http://woi.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://owd.svipenyu.cn

[U27] Py：异步 HTTP
来源：http://nut.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://mij.yueranfly.top

[U28] Py：类型别名
来源：http://mmg.smart0.xyz

UserId = int
来源：http://icc.yonumen.top

[U29] Py：属性校验
来源：http://tea.0kj1m.cn

@property 与 @x.setter 配合
来源：http://ylw.ehwqpu.com

[U30] Py：数据类
来源：http://dom.wangshuangyany.cn

@dataclass(slots=True)
来源：http://qfu.daxiang520.top

[U31] Py：单测
来源：http://fos.gaohongyu789.top

python -m pytest -q
来源：http://hoz.sjlbkw.cn

[U32] Py：代码格式化
来源：http://ijf.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://mpp.nanxuanxn.top

[U33] Py：打包发布
来源：http://vmb.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://ris.zhiwuduotai.top

[U34] Py：判断编码
来源：http://hex.yongpay.top

chardet.detect(raw)
来源：http://cqd.jqgfzy.top

[U35] Py：发送邮件
来源：http://abo.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://law.shuidangran.top

[U36] Py：定时任务
来源：http://ztv.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://vto.chenjidiqi.icu

[U37] Py：读写 Excel
来源：http://fui.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jwt.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://wpg.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://mpk.haohaochexian.top

[U39] Py：判断是否在交互环境
来源：http://gfq.hammf.cn

sys.stdout.isatty()
来源：http://gbn.andypj.xyz

[U40] Py：打印到标准错误
来源：http://jhl.birdmap.top

print("err", file=sys.stderr)
来源：http://nfy.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://trm.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mwo.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://ksf.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xif.yangfankeji.com

[U43] PHP：声明命名空间
来源：http://bfs.xingfuxueyuan.xyz

namespace App\Http;
来源：http://vht.ctjpmb.com

[U44] PHP：开启严格类型
来源：http://ble.sxryk.cn

declare(strict_types=1);
来源：http://lst.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://nty.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tph.iojbl.cn

[U46] PHP：可空类型
来源：http://pqq.iojbl.cn

?string $name = null
来源：http://ffn.yj20258888.top

[U47] PHP：联合类型
来源：http://jfn.jqgufenzy.top

int|string $id
来源：http://mui.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://ass.chenlongwang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pet.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://tpn.zdbjq.cn

public readonly string $name
来源：http://jcv.fengsongda.top

[U50] PHP：构造器属性提升
来源：http://bzg.ydzc1.top

public function __construct(private int $id) {}
来源：http://qqb.cheryme.top

[U51] PHP：数组解构
来源：http://wai.hnqzz.top

[$a, $b] = $arr;
来源：http://yzi.xylfe.cn

[U52] PHP：箭头函数
来源：http://bup.yj202588.top

$double = fn($x) => $x * 2;
来源：http://wxn.fengsongda.top

[U53] PHP：空合并运算符
来源：http://rcj.kuanghao11.cn

$v = $a ?? $b ?? "default";
来源：http://ogs.zhixingplan.top

[U54] PHP：空安全调用
来源：http://yln.svipenyu.cn

$obj?->method()
来源：http://taj.gotoacloud.top

[U55] PHP：match 表达式
来源：http://thf.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://krg.pycfn.com

[U56] PHP：命名参数
来源：http://wrz.cashguo.top

f(a: 1, b: 2)
来源：http://jkq.ybcxt.top

[U57] PHP：字符串插值
来源：http://mvh.aizwys.cn

"值: {$a}"
来源：http://fvc.aibaodan.cn

[U58] PHP：数组三件套
来源：http://fpj.yfazqb.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ert.gogol.net.cn

[U59] PHP：自定义排序
来源：http://hgy.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmp.havefunace.top

[U60] PHP：JSON 编解码
来源：http://rmd.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rcy.jinqigufen.top

[U61] PHP：正则
来源：http://aqw.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aqs.epnwcf.com

[U62] PHP：日期对象
来源：http://tkb.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://epf.shzxlz.cn

[U63] PHP：文件读写
来源：http://qkv.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wtz.daxiang520.top

[U64] PHP：目录遍历
来源：http://eqa.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://aov.feifeiyinyue.top

[U65] PHP：会话
来源：http://yxk.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ayh.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://cxq.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pnl.fktsv.cn

[U67] PHP：处理文件上传
来源：http://ofa.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nxr.hywenlv.cn

[U68] PHP：PDO 连接
来源：http://gdm.tianlin.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kxb.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://hlv.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fzf.pycfn.com

[U70] PHP：PDO 事务
来源：http://sdc.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wsf.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://wjs.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://qjk.jianghu66.top

[U72] PHP：写错误日志
来源：http://sdg.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://zns.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://vri.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://hpx.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://lku.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://oew.cucudq.cn

[U75] PHP：依赖注入
来源：http://lne.jinqigfzy.top

composer require psr/container
来源：http://knd.daria6918.cn

[U76] PHP：简单路由
来源：http://qke.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yyt.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://gvu.xuanzx.com

composer require twig/twig
来源：http://uqd.xylfe.cn

[U78] PHP：单元测试
来源：http://xvr.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://xni.shanyushiyangtech.top

[U79] PHP：静态分析
来源：http://xec.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://fop.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://gyf.bbcook.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nvt.hywenlv.cn

[U81] JS：初始化项目
来源：http://hcv.tianlin.xyz

npm init -y;  npm i express
来源：http://trm.52xcode.cn

[U82] JS：package.json 脚本
来源：http://yed.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://apv.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://qdn.gaohongyu789.top

export const a = 1;  import { a } from "./m.js";
来源：http://npx.jyoumei.cn

[U84] JS：CommonJS 写法
来源：http://hph.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://hbb.gzhubu.top

[U85] JS：可选链
来源：http://smo.sysykeji.top

a?.b?.c
来源：http://ocm.sjlbkw.cn

[U86] JS：空值合并
来源：http://odx.zhaomingkeji.xyz

a ?? b
来源：http://vfs.iojbl.cn

[U87] JS：解构默认值
来源：http://pqr.iojbl.cn

const { a = 1, b = 2 } = obj;
来源：http://hll.yonumen.top

[U88] JS：对象展开合并
来源：http://ykj.hfpthk.cn

{ ...a, ...b }
来源：http://mnn.birdmap.top

[U89] JS：数组去重
来源：http://uat.ctjpmb.com

[...new Set(arr)]
来源：http://mtf.ybcxt.top

[U90] JS：数字数组排序
来源：http://vut.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://hlk.cashguo.top

[U91] JS：对象键值遍历
来源：http://irx.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lqc.zdqjudy.top

[U92] JS：深拷贝
来源：http://lsa.yj20258888.top

structuredClone(obj)
来源：http://wsb.ivvv.top

[U93] JS：模板字符串
来源：http://bpe.yongpay.top

`共 ${n} 条`
来源：http://wmn.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://tkz.shangyingyoupin.top

const double = x => x * 2;
来源：http://eqs.jqgfzy.top

[U95] JS：Promise 包装
来源：http://uca.epnwcf.com

new Promise((resolve, reject) => {})
来源：http://xvz.fehbvm.com

[U96] JS：async/await 与异常
来源：http://ajq.hcnkem.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ixw.hongshengwenyu.top

[U97] JS：并发请求
来源：http://uec.zdqjudy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hkc.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://rbg.sysykeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ljp.zhengqikj.top

[U99] JS：事件监听
来源：http://cnt.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://ljt.yfazqb.com

[U100] JS：DOM 查询
来源：http://yju.ppjwa.cn

document.querySelector(".item")
来源：http://sqp.fengsongda.top

[U101] JS：classList 操作
来源：http://dbf.zycfv.cn

el.classList.toggle("active")
来源：http://kyw.jlsjyb.cn

[U102] JS：本地存储
来源：http://olf.ivvv.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hew.cqqwz.cn

[U103] JS：定时器
来源：http://wob.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cjb.vehdjk.com

[U104] JS：防抖
来源：http://tca.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyw.jinqigfzy.top

[U105] JS：节流
来源：http://fgs.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://htv.0kj1m.cn

[U106] JS：日期格式化
来源：http://mem.daria6918.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ezt.birdmap.top

[U107] JS：数字千分位
来源：http://env.pycfn.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://srr.bjfxy.top

[U108] JS：随机整数
来源：http://ftm.chenlongwang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pnw.aizwys.cn

[U109] JS：数组分组
来源：http://zxi.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://psa.xinyue.icu

[U110] JS：数组分块
来源：http://pey.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zgc.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://dcx.xuetiantiany.cn

new Map(Object.entries(obj))
来源：http://zza.nwbrower.top

[U112] JS：字符串补位
来源：http://jms.cucudq.cn

"7".padStart(3, "0")
来源：http://lqn.xziqi.cn

[U113] JS：正则替换全部
来源：http://ifv.birdmap.top

s.replaceAll("a", "b")
来源：http://nqz.sysykeji.top

[U114] JS：JSON 深比较
来源：http://crz.0kj1m.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vzw.zhengqikj.top

[U115] JS：生成 UUID
来源：http://crp.jinghuilouyu.cn

crypto.randomUUID()
来源：http://mmw.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://mgl.fengsongda.top

/** @param {string} name */ function f(name) {}
来源：http://xfj.meibo888.top

[U117] JS：单元测试
来源：http://ack.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://jni.fktsv.cn

[U118] JS：开发服务器
来源：http://zso.c1oappe.top

npm i -D vite;  npx vite
来源：http://qwv.316326.xyz

[U119] JS：生产构建
来源：http://sxm.yonumen.top

npx vite build
来源：http://vst.guannengcc.top

[U120] JS：读取环境变量（Vite）
来源：http://ais.aizwys.cn

import.meta.env.VITE_API_URL
来源：http://ypg.tian-w.cn

================================================================================
来源：http://yis.dashuyun.cn

统计汇总
来源：http://gxs.guowangkeji.top

================================================================================
来源：http://lwq.guowangkeji.top

按语言统计（条）：
来源：http://qdj.chenjidiqi.icu

Python ......... 252
来源：http://yyg.52xcode.cn

PHP ............ 252
来源：http://ira.cashguo.top

JavaScript ..... 252
来源：http://ron.wangdashe.top

TypeScript ..... 212
来源：http://cls.jiagoushi.top

Java ........... 212
来源：http://swd.zhongyouzk.top

Go ............. 212
来源：http://sxa.hysaishi.cn

Ruby ........... 212
来源：http://pse.ctjpmb.com

C# ............. 212
来源：http://cmv.zycfv.cn

C .............. 30
来源：http://jup.cucudq.cn

C++ ............ 30
来源：http://tdm.cucudq.cn

SQL ............ 90
来源：http://vyu.fengsongda.top

Bash ........... 80
来源：http://ljx.hesvh.cn

Kotlin ......... 15
来源：http://jsu.shangyingyoupin.top

Swift .......... 15
来源：http://icp.vqdsnc.cn

Lua ............ 10
来源：http://teu.hywenlv.cn

Perl ........... 10
来源：http://tzc.bjfxy.top

Scala .......... 10
来源：http://azb.jinqigufen.top

------------------------------------
来源：http://rrd.gogol.net.cn

合计 ........... 2106 条
来源：http://yfy.jqgufenzy.top

按章节统计：
来源：http://ozp.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rcy.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xji.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://yyl.shuidangran.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nlt.cashguo.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kfw.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iqu.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xgq.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dvl.hysaishi.cn


<!-- 参考信息 -->