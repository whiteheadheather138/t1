代发 wailian999

case class User(name: String, age: Int)
来源：http://xbi.bjfxy.top

[T57] Scala：模式匹配
来源：http://lnx.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://nqw.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://xwt.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://xdz.gaohongyu789.top

[T59] Scala：循环
来源：http://rbj.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://qyz.shuidangran.top

[T60] Scala：折叠
来源：http://pib.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xzn.zhiwuduotai.top

================================================================================
来源：http://doe.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rqn.xziqi.cn

================================================================================
来源：http://loo.birdmap.top

[U01] Py：创建虚拟环境
来源：http://mwc.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://xqe.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://hfh.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zfq.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://avp.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://thv.sweek.top

[U04] Py：变量调试打印
来源：http://tpf.havefunace.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sva.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://sjo.vehdjk.com

list(dict.fromkeys(arr))
来源：http://ubp.shuidangran.top

[U06] Py：合并两个字典
来源：http://awa.xziqi.cn

{**a, **b}
来源：http://ldy.9152youxi.cn

[U07] Py：反转字典键值
来源：http://zad.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://lxb.tianlin.xyz

[U08] Py：展平二维列表
来源：http://opd.c1oappe.top

[y for x in nested for y in x]
来源：http://niq.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://qoo.wangdashe.top

max(d, key=d.get)
来源：http://yqz.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://enw.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dme.yj20258.top

[U11] Py：生成器表达式
来源：http://ttd.ybcxt.top

(x * 2 for x in arr)
来源：http://wdk.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://pex.sysykeji.top

Counter(arr).most_common(3)
来源：http://lfg.iojbl.cn

[U13] Py：固定长度队列
来源：http://xmq.zhixingplan.top

deque(maxlen=10)
来源：http://jqp.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://vwq.shangyingyoupin.top

defaultdict(list)
来源：http://lpg.mhx1999.top

[U15] Py：高精度计时
来源：http://ysi.tian-w.cn

t = time.perf_counter()
来源：http://uwi.cucudq.cn

[U16] Py：命令行参数解析
来源：http://ins.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ubg.cqqwz.cn

[U17] Py：初始化日志
来源：http://niq.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://wlk.dianchejie.cn

[U18] Py：预编译正则
来源：http://dql.sjlbkw.cn

pat = re.compile(r"\d+")
来源：http://cae.smart0.xyz

[U19] Py：正则替换带回调
来源：http://ilr.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bhz.bjfxy.top

[U20] Py：缓存函数结果
来源：http://jeg.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://awd.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://vwn.ctjpmb.com

@contextlib.contextmanager
来源：http://ihk.tian-w.cn

[U22] Py：矩阵转置
来源：http://hql.fanxiaobao.xyz

list(zip(*m))
来源：http://aaj.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://lgm.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pni.daria6918.cn

[U24] Py：路径操作
来源：http://ahp.jqgfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qec.birdmap.top

[U25] Py：CSV 按字典读
来源：http://lcl.haohaochexian.top

csv.DictReader(f)
来源：http://bof.vqdsnc.cn

[U26] Py：并发下载
来源：http://ljk.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nyq.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://dqb.316326.xyz

aiohttp.ClientSession() 配合 async with
来源：http://jxt.zycfv.cn

[U28] Py：类型别名
来源：http://rcv.bjfxy.top

UserId = int
来源：http://mom.hnxiangtu.top

[U29] Py：属性校验
来源：http://rce.epnwcf.com

@property 与 @x.setter 配合
来源：http://qvi.nanxinkj.top

[U30] Py：数据类
来源：http://pkg.zhengqikj.top

@dataclass(slots=True)
来源：http://wsu.nwbrower.top

[U31] Py：单测
来源：http://xzy.hnqzz.top

python -m pytest -q
来源：http://rjs.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://oyq.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://qzr.nanxuanxn.top

[U33] Py：打包发布
来源：http://vfu.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://cwo.daxiang520.top

[U34] Py：判断编码
来源：http://jpq.cdnleiting.top

chardet.detect(raw)
来源：http://oya.smart0.xyz

[U35] Py：发送邮件
来源：http://hml.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kba.vehdjk.com

[U36] Py：定时任务
来源：http://skb.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://nuh.andypj.xyz

[U37] Py：读写 Excel
来源：http://esz.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://ajq.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://hfo.fengsongda.top

Path(__file__).resolve().parent
来源：http://uhe.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://slx.birdmap.top

sys.stdout.isatty()
来源：http://ixz.ybcxt.top

[U40] Py：打印到标准错误
来源：http://bwh.wangdashe.top

print("err", file=sys.stderr)
来源：http://xnk.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://zzo.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fxb.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://nde.cheryme.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xtq.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://sjz.svipenyu.cn

namespace App\Http;
来源：http://ayx.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://zwa.andypj.xyz

declare(strict_types=1);
来源：http://weq.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://bdd.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://pub.shuidangran.top

[U46] PHP：可空类型
来源：http://jvm.yj202588.top

?string $name = null
来源：http://prp.hysaishi.cn

[U47] PHP：联合类型
来源：http://nzo.snrcjt.cn

int|string $id
来源：http://ckw.mhx1999.top

[U48] PHP：纯枚举
来源：http://fxl.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdg.uphjek.com

[U49] PHP：只读属性
来源：http://nbb.chenjidiqi.icu

public readonly string $name
来源：http://eai.cucudq.cn

[U50] PHP：构造器属性提升
来源：http://tkf.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://coq.mhx1999.top

[U51] PHP：数组解构
来源：http://liy.zhoulong.xyz

[$a, $b] = $arr;
来源：http://mba.hnqzz.top

[U52] PHP：箭头函数
来源：http://nge.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://lqb.hcnkem.com

[U53] PHP：空合并运算符
来源：http://boi.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://nbd.zhijiandao.cn

[U54] PHP：空安全调用
来源：http://vgz.fengsongda.top

$obj?->method()
来源：http://hje.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://rnd.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://azl.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://apf.zdqjudy.top

f(a: 1, b: 2)
来源：http://sho.aibaodan.cn

[U57] PHP：字符串插值
来源：http://yvt.cheryme.top

"值: {$a}"
来源：http://dfx.ctjpmb.com

[U58] PHP：数组三件套
来源：http://bwm.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cqq.fengsongda.top

[U59] PHP：自定义排序
来源：http://gih.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jbd.zhiwuduotai.top

[U60] PHP：JSON 编解码
来源：http://cxx.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pzy.cashguo.top

[U61] PHP：正则
来源：http://ahr.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rye.gogol.net.cn

[U62] PHP：日期对象
来源：http://gps.ybcxt.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zmv.yuanzhike.top

[U63] PHP：文件读写
来源：http://xbc.ivvv.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lis.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://tqy.zdqjudy.top

glob("dir/*.php");  scandir("dir");
来源：http://hyt.fzhhl.top

[U65] PHP：会话
来源：http://vud.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qqj.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://bpz.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jpi.yongpay.top

[U67] PHP：处理文件上传
来源：http://ynx.daxiang520.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://axl.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://cop.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ibr.zhijiandao.cn

[U69] PHP：PDO 预处理
来源：http://ohn.yangfankeji.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ppm.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://oxz.yanxiufei.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mpp.nanxinkj.top

[U71] PHP：抛出异常
来源：http://kju.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://eeq.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://hhi.guowangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://ivq.snrcjt.cn

[U73] PHP：读取 ini 配置
来源：http://iru.shzxlz.cn

parse_ini_file("config.ini", true)
来源：http://fpx.yfazqb.com

[U74] PHP：读取环境变量
来源：http://hps.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://zto.sysykeji.top

[U75] PHP：依赖注入
来源：http://bjj.ehwqpu.com

composer require psr/container
来源：http://gbf.yueranfly.top

[U76] PHP：简单路由
来源：http://tme.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://llx.bjfxy.top

[U77] PHP：模板渲染
来源：http://hok.gaohongyu789.top

composer require twig/twig
来源：http://pey.shanyushiyangtech.top

[U78] PHP：单元测试
来源：http://oyz.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://cjt.ehwqpu.com

[U79] PHP：静态分析
来源：http://pxc.cdnleiting.top

composer require --dev phpstan/phpstan
来源：http://lzw.aizwys.cn

[U80] PHP：代码规范修复
来源：http://fuv.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://eye.zhongyouzk.top

[U81] JS：初始化项目
来源：http://jko.jinqigfzy.top

npm init -y;  npm i express
来源：http://tji.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://yac.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wvs.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://owz.hfpthk.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nnh.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://fga.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://lfh.fengsongda.top

[U85] JS：可选链
来源：http://gpk.gotoacloud.top

a?.b?.c
来源：http://wwd.vehdjk.com

[U86] JS：空值合并
来源：http://fwe.fktsv.cn

a ?? b
来源：http://cem.jqgufenzy.top

[U87] JS：解构默认值
来源：http://btd.bbcook.cn

const { a = 1, b = 2 } = obj;
来源：http://xgq.c1oappe.top

[U88] JS：对象展开合并
来源：http://xng.pycfn.com

{ ...a, ...b }
来源：http://kvp.xuanzx.com

[U89] JS：数组去重
来源：http://zre.chenlongwang.top

[...new Set(arr)]
来源：http://qjy.jlsjyb.cn

[U90] JS：数字数组排序
来源：http://kuu.hywenlv.cn

[...arr].sort((a, b) => a - b)
来源：http://mjl.zhiwuduotai.top

[U91] JS：对象键值遍历
来源：http://zal.ydjk.org.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qcr.nanxuanxn.top

[U92] JS：深拷贝
来源：http://abv.yj202588.top

structuredClone(obj)
来源：http://fwr.sysykeji.top

[U93] JS：模板字符串
来源：http://qjc.hammf.cn

`共 ${n} 条`
来源：http://xmt.shzxlz.cn

[U94] JS：箭头函数
来源：http://mds.dashuyun.cn

const double = x => x * 2;
来源：http://ksz.chenzaomai.com

[U95] JS：Promise 包装
来源：http://zxv.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://kqb.daxiang520.top

[U96] JS：async/await 与异常
来源：http://pvl.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jwb.kuanghao11.cn

[U97] JS：并发请求
来源：http://xpy.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qpz.mhx1999.top

[U98] JS：fetch 带 JSON
来源：http://djk.yuanzhike.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lye.uphjek.com

[U99] JS：事件监听
来源：http://qjq.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://wwt.uphjek.com

[U100] JS：DOM 查询
来源：http://muz.dianchejie.cn

document.querySelector(".item")
来源：http://bdg.hammf.cn

[U101] JS：classList 操作
来源：http://gxy.gaohongyu789.top

el.classList.toggle("active")
来源：http://fju.xziqi.cn

[U102] JS：本地存储
来源：http://tuq.hammf.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dvn.chenlongwang.top

[U103] JS：定时器
来源：http://igw.aibaodan.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bqz.fengsongda.top

[U104] JS：防抖
来源：http://bhd.hnqzz.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvk.pengpengdd.cyou

[U105] JS：节流
来源：http://qds.xuanzx.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://lzh.jinqigufen.top

[U106] JS：日期格式化
来源：http://akt.quarkkingdee.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nun.jianghu66.top

[U107] JS：数字千分位
来源：http://xgs.chenjidiqi.icu

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qgv.hnxiangtu.top

[U108] JS：随机整数
来源：http://dze.uphjek.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yzc.yvedp.cn

[U109] JS：数组分组
来源：http://oig.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://eyg.sweek.top

[U110] JS：数组分块
来源：http://iga.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cft.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://pol.52xcode.cn

new Map(Object.entries(obj))
来源：http://job.0kj1m.cn

[U112] JS：字符串补位
来源：http://niv.shuidangran.top

"7".padStart(3, "0")
来源：http://ysi.yanxiufei.cn

[U113] JS：正则替换全部
来源：http://kfl.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://aib.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://ido.tianlin.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://mkg.nwbrower.top

[U115] JS：生成 UUID
来源：http://nbz.9152youxi.cn

crypto.randomUUID()
来源：http://wgq.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://qyo.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://qqj.mhx1999.top

[U117] JS：单元测试
来源：http://tne.zhijiandao.cn

npm i -D vitest;  npx vitest
来源：http://ikc.meibo888.top

[U118] JS：开发服务器
来源：http://nll.zhiwuduotai.top

npm i -D vite;  npx vite
来源：http://cuu.zhijiandao.cn

[U119] JS：生产构建
来源：http://nld.daria6918.cn

npx vite build
来源：http://ply.pycfn.com

[U120] JS：读取环境变量（Vite）
来源：http://kvj.xingfuxueyuan.xyz

import.meta.env.VITE_API_URL
来源：http://bhz.cashguo.top

================================================================================
来源：http://sdd.pengpengdd.cyou

统计汇总
来源：http://hzx.jinqigufen.top

================================================================================
来源：http://hbx.ywan-chungtsiang.top

按语言统计（条）：
来源：http://otv.jqgufenzy.top

Python ......... 252
来源：http://xpf.birdmap.top

PHP ............ 252
来源：http://qei.cheryme.top

JavaScript ..... 252
来源：http://roc.shuidangran.top

TypeScript ..... 212
来源：http://gqn.nwbrower.top

Java ........... 212
来源：http://ndl.feifeiyinyue.top

Go ............. 212
来源：http://grr.svipenyu.cn

Ruby ........... 212
来源：http://xwh.ydjk.org.cn

C# ............. 212
来源：http://kqe.jlsjyb.cn

C .............. 30
来源：http://fkv.jinqigufen.top

C++ ............ 30
来源：http://xem.hywenlv.cn

SQL ............ 90
来源：http://hhu.smart0.xyz

Bash ........... 80
来源：http://hxt.svipenyu.cn

Kotlin ......... 15
来源：http://ibc.yuxming.cn

Swift .......... 15
来源：http://agy.tian-w.cn

Lua ............ 10
来源：http://xgp.nwbrower.top

Perl ........... 10
来源：http://rvo.epnwcf.com

Scala .......... 10
来源：http://xrf.hysaishi.cn

------------------------------------
来源：http://nup.chenzaomai.com

合计 ........... 2106 条
来源：http://hsg.svipenyu.cn

按章节统计：
来源：http://bwf.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fdt.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rdw.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://drs.jqgufenzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kup.zdbjq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fzo.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dhv.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uom.hfpthk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://izk.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cwv.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://avl.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gcs.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wka.yj20258.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kos.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rhp.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bod.c1oappe.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jxu.gogol.net.cn

Q SQL 专题                              90
来源：http://ufb.vqdsnc.cn

R Bash 专题                             80
来源：http://yjc.epnwcf.com

S C / C++ 专题                          60
来源：http://hho.tian-w.cn

T 其他语言补充                          60
来源：http://fqc.ivvv.top

U 高频实用片段                         120
来源：http://hkw.epnwcf.com

------------------------------------
来源：http://lwq.ehwqpu.com

合计                                  2106 条
来源：http://dwl.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://rjk.pengpengdd.cyou


<!-- 参考信息 -->