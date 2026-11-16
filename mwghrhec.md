代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://xau.fktsv.cn

[T51] Scala：Hello World
来源：http://xzx.ybcxt.top

println("Hello")
来源：http://zxl.316326.xyz

[T52] Scala：变量
来源：http://cui.hysaishi.cn

val a = 1;  var b = 2
来源：http://lhr.cashguo.top

[T53] Scala：字符串插值
来源：http://ujs.yonumen.top

s"值: $b"
来源：http://tmq.yueranfly.top

[T54] Scala：集合映射
来源：http://zvz.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://jnl.yj20258.top

[T55] Scala：集合过滤
来源：http://too.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fwj.zhengqikj.top

[T56] Scala：样例类
来源：http://mek.wangdashe.top

case class User(name: String, age: Int)
来源：http://hut.tanke756.top

[T57] Scala：模式匹配
来源：http://tpo.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hes.cqqwz.cn

[T58] Scala：函数定义
来源：http://wrv.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pff.zhijiandao.cn

[T59] Scala：循环
来源：http://fig.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://hle.iojbl.cn

[T60] Scala：折叠
来源：http://bqk.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bis.yj20258888.top

================================================================================
来源：http://vhw.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsq.0kj1m.cn

================================================================================
来源：http://tkd.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://ocx.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://hgh.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://xsr.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://exu.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://wjc.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sqr.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://dzi.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bpn.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://cbn.yonumen.top

list(dict.fromkeys(arr))
来源：http://jzv.xylfe.cn

[U06] Py：合并两个字典
来源：http://vhy.zycfv.cn

{**a, **b}
来源：http://gnr.andypj.xyz

[U07] Py：反转字典键值
来源：http://asd.shzxlz.cn

{v: k for k, v in d.items()}
来源：http://vze.cucudq.cn

[U08] Py：展平二维列表
来源：http://yyu.ppjwa.cn

[y for x in nested for y in x]
来源：http://dkz.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://nwe.fzhhl.top

max(d, key=d.get)
来源：http://bwr.sweek.top

[U10] Py：按值排序字典
来源：http://wep.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hnr.yuxming.cn

[U11] Py：生成器表达式
来源：http://wcn.zhengqikj.top

(x * 2 for x in arr)
来源：http://pwq.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://fqm.jiagoushi.top

Counter(arr).most_common(3)
来源：http://dth.daxiang520.top

[U13] Py：固定长度队列
来源：http://vic.cashguo.top

deque(maxlen=10)
来源：http://rcp.zhaomingkeji.xyz

[U14] Py：分组收集到列表
来源：http://aib.xuanzx.com

defaultdict(list)
来源：http://xai.yj20258.top

[U15] Py：高精度计时
来源：http://aux.jinqigfzy.top

t = time.perf_counter()
来源：http://hyh.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://iym.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yld.xylfe.cn

[U17] Py：初始化日志
来源：http://fzr.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://hwo.zhixingplan.top

[U18] Py：预编译正则
来源：http://eek.meibo888.top

pat = re.compile(r"\d+")
来源：http://kle.xylfe.cn

[U19] Py：正则替换带回调
来源：http://cfb.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kji.cheryme.top

[U20] Py：缓存函数结果
来源：http://xix.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://edx.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://kwc.fzhhl.top

@contextlib.contextmanager
来源：http://bmm.zhengqikj.top

[U22] Py：矩阵转置
来源：http://wjd.andypj.xyz

list(zip(*m))
来源：http://vkv.daxiang520.top

[U23] Py：分块读取大文件
来源：http://lyq.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://skd.zhixingplan.top

[U24] Py：路径操作
来源：http://tdm.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cyg.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://hsi.ctjpmb.com

csv.DictReader(f)
来源：http://sje.jinqigufen.top

[U26] Py：并发下载
来源：http://nmc.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oqm.gogol.net.cn

[U27] Py：异步 HTTP
来源：http://mjm.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://pqv.jlsjyb.cn

[U28] Py：类型别名
来源：http://roe.sweek.top

UserId = int
来源：http://omf.hcnkem.com

[U29] Py：属性校验
来源：http://nqx.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://hpe.yj20258.top

[U30] Py：数据类
来源：http://nmz.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://adv.vqdsnc.cn

[U31] Py：单测
来源：http://vbp.tarul.cn

python -m pytest -q
来源：http://kfw.haohaochexian.top

[U32] Py：代码格式化
来源：http://ebg.yvedp.cn

ruff format . && ruff check --fix .
来源：http://zrf.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://lrb.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://gtn.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://och.shzxlz.cn

chardet.detect(raw)
来源：http://zff.bjfxy.top

[U35] Py：发送邮件
来源：http://trq.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bls.zhiwuduotai.top

[U36] Py：定时任务
来源：http://rky.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://bbr.nwbrower.top

[U37] Py：读写 Excel
来源：http://rgf.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://ofa.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://jrp.epnwcf.com

Path(__file__).resolve().parent
来源：http://lbe.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://kmb.andypj.xyz

sys.stdout.isatty()
来源：http://vfl.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://sgh.xinyue.icu

print("err", file=sys.stderr)
来源：http://okn.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://bnt.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ofr.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://aqg.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ihp.shuidangran.top

[U43] PHP：声明命名空间
来源：http://uos.nanxinkj.top

namespace App\Http;
来源：http://gct.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://hlh.jinqigfzy.top

declare(strict_types=1);
来源：http://mwi.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://zul.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bmg.hnxiangtu.top

[U46] PHP：可空类型
来源：http://dxi.jinqigufen.top

?string $name = null
来源：http://fqo.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://xhn.xylfe.cn

int|string $id
来源：http://ohr.bbcook.cn

[U48] PHP：纯枚举
来源：http://yhc.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lfj.guowangkeji.top

[U49] PHP：只读属性
来源：http://iod.snrcjt.cn

public readonly string $name
来源：http://xbg.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://vyh.yuanzhike.top

public function __construct(private int $id) {}
来源：http://fzt.quarkkingdee.top

[U51] PHP：数组解构
来源：http://fmk.ctjpmb.com

[$a, $b] = $arr;
来源：http://wgq.chenlongwang.top

[U52] PHP：箭头函数
来源：http://njo.jlsjyb.cn

$double = fn($x) => $x * 2;
来源：http://wah.meibo888.top

[U53] PHP：空合并运算符
来源：http://rdt.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://zec.sweek.top

[U54] PHP：空安全调用
来源：http://hrg.xinyue.icu

$obj?->method()
来源：http://ose.quarkkingdee.top

[U55] PHP：match 表达式
来源：http://nni.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lhe.tarul.cn

[U56] PHP：命名参数
来源：http://yat.52xcode.cn

f(a: 1, b: 2)
来源：http://uyk.tianlin.xyz

[U57] PHP：字符串插值
来源：http://vja.hcnkem.com

"值: {$a}"
来源：http://dqa.tian-w.cn

[U58] PHP：数组三件套
来源：http://zzu.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://usx.guowangkeji.top

[U59] PHP：自定义排序
来源：http://xxy.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owj.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://dhv.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nei.xziqi.cn

[U61] PHP：正则
来源：http://gtk.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://inq.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://iks.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://grw.yuxming.cn

[U63] PHP：文件读写
来源：http://ths.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mza.daria6918.cn

[U64] PHP：目录遍历
来源：http://inh.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://udh.yj20258.top

[U65] PHP：会话
来源：http://urs.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://kdq.ivvv.top

[U66] PHP：设置 Cookie
来源：http://iyi.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cxq.hnxiangtu.top

[U67] PHP：处理文件上传
来源：http://nmw.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mto.uphjek.com

[U68] PHP：PDO 连接
来源：http://gds.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xmz.svipenyu.cn

[U69] PHP：PDO 预处理
来源：http://kis.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fjh.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://gof.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hsw.svipenyu.cn

[U71] PHP：抛出异常
来源：http://kvf.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://vzd.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://rov.shuidangran.top

error_log("失败: " . $e->getMessage());
来源：http://ero.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://ywb.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://zjl.wangdashe.top

[U74] PHP：读取环境变量
来源：http://mvd.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://zrf.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://wut.andypj.xyz

composer require psr/container
来源：http://tfc.sufxvd.cn

[U76] PHP：简单路由
来源：http://gfi.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://csf.hfpthk.cn

[U77] PHP：模板渲染
来源：http://jxa.ybcxt.top

composer require twig/twig
来源：http://iur.ctjpmb.com

[U78] PHP：单元测试
来源：http://jwx.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://hks.yuxming.cn

[U79] PHP：静态分析
来源：http://gfm.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://amr.yj20258888.top

[U80] PHP：代码规范修复
来源：http://dty.hcnkem.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://wab.sufxvd.cn

[U81] JS：初始化项目
来源：http://uid.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://kph.mhx1999.top

[U82] JS：package.json 脚本
来源：http://lii.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jms.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://sie.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://vkf.hammf.cn

[U84] JS：CommonJS 写法
来源：http://xuq.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fik.smart0.xyz

[U85] JS：可选链
来源：http://bfa.fengsongda.top

a?.b?.c
来源：http://oon.xingfuxueyuan.xyz

[U86] JS：空值合并
来源：http://syw.yonumen.top

a ?? b
来源：http://gsc.yonumen.top

[U87] JS：解构默认值
来源：http://brz.jinyuanbaomall.cn

const { a = 1, b = 2 } = obj;
来源：http://nzr.hywenlv.cn

[U88] JS：对象展开合并
来源：http://ywa.cucudq.cn

{ ...a, ...b }
来源：http://kzb.xinyue.icu

[U89] JS：数组去重
来源：http://bnf.hywenlv.cn

[...new Set(arr)]
来源：http://nsk.zdqjudy.top

[U90] JS：数字数组排序
来源：http://wnt.zhijiandao.cn

[...arr].sort((a, b) => a - b)
来源：http://gmb.ydzc1.top

[U91] JS：对象键值遍历
来源：http://mzr.yuxming.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jzw.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://thy.jlsjyb.cn

structuredClone(obj)
来源：http://vof.hesvh.cn

[U93] JS：模板字符串
来源：http://nyn.daxiang520.top

`共 ${n} 条`
来源：http://wdc.tianlin.xyz

[U94] JS：箭头函数
来源：http://fgf.zdbjq.cn

const double = x => x * 2;
来源：http://dpy.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://bhi.ivvv.top

new Promise((resolve, reject) => {})
来源：http://dle.shangyingyoupin.top

[U96] JS：async/await 与异常
来源：http://pej.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kts.xuanzx.com

[U97] JS：并发请求
来源：http://bzf.hywenlv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eti.bjfxy.top

[U98] JS：fetch 带 JSON
来源：http://iuq.hammf.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cfm.sufxvd.cn

[U99] JS：事件监听
来源：http://ukh.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://msb.aibaodan.cn

[U100] JS：DOM 查询
来源：http://pjc.yfazqb.com

document.querySelector(".item")
来源：http://gga.mhx1999.top

[U101] JS：classList 操作
来源：http://rjn.daxiang520.top

el.classList.toggle("active")
来源：http://ydt.fktsv.cn

[U102] JS：本地存储
来源：http://oni.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://key.0kj1m.cn

[U103] JS：定时器
来源：http://acm.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bgx.guowangkeji.top

[U104] JS：防抖
来源：http://vqf.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nfp.hnqzz.top

[U105] JS：节流
来源：http://mxh.pengpengdd.cyou

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://aej.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://gfm.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wwt.fanxiaobao.xyz

[U107] JS：数字千分位
来源：http://ysc.52xcode.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hsl.fehbvm.com

[U108] JS：随机整数
来源：http://uvp.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gsk.tanke756.top

[U109] JS：数组分组
来源：http://zip.pycfn.com

Object.groupBy(arr, x => x.type)
来源：http://bym.xuetiantiany.cn

[U110] JS：数组分块
来源：http://mpx.smart0.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gsn.jyoumei.cn

[U111] JS：对象转 Map
来源：http://xdj.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://udl.jinghuilouyu.cn

[U112] JS：字符串补位
来源：http://eot.xuanzx.com

"7".padStart(3, "0")
来源：http://sdc.316326.xyz

[U113] JS：正则替换全部
来源：http://zcj.sysykeji.top

s.replaceAll("a", "b")
来源：http://cer.meibo888.top

[U114] JS：JSON 深比较
来源：http://scf.zdbjq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gws.daria6918.cn

[U115] JS：生成 UUID
来源：http://qtm.vqdsnc.cn

crypto.randomUUID()
来源：http://nvb.shuidangran.top

[U116] JS：类型检查（JSDoc）
来源：http://gjt.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://xef.chenlongwang.top

[U117] JS：单元测试
来源：http://zqh.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://gpj.tian-w.cn

[U118] JS：开发服务器
来源：http://eje.tarul.cn

npm i -D vite;  npx vite
来源：http://qav.haohaochexian.top

[U119] JS：生产构建
来源：http://wem.jyoumei.cn

npx vite build
来源：http://gqd.daxiang520.top

[U120] JS：读取环境变量（Vite）
来源：http://rek.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://xoq.jlsjyb.cn

================================================================================
来源：http://vwq.jyoumei.cn

统计汇总
来源：http://qgc.jlsjyb.cn

================================================================================
来源：http://eau.sxryk.cn

按语言统计（条）：
来源：http://bqq.xinyue.icu

Python ......... 252
来源：http://qma.cdnleiting.top

PHP ............ 252
来源：http://jpa.yj20258888.top

JavaScript ..... 252
来源：http://ywd.yj202588.top

TypeScript ..... 212
来源：http://vak.ctjpmb.com

Java ........... 212
来源：http://iyi.c1oappe.top

Go ............. 212
来源：http://nyh.yonumen.top

Ruby ........... 212
来源：http://zha.jiagoushi.top

C# ............. 212
来源：http://kuy.hywenlv.cn

C .............. 30
来源：http://jwk.bjfxy.top

C++ ............ 30
来源：http://bvr.nwbrower.top

SQL ............ 90
来源：http://ewh.svipenyu.cn

Bash ........... 80
来源：http://kxd.daria6918.cn

Kotlin ......... 15
来源：http://knr.nanxuanxn.top

Swift .......... 15
来源：http://wga.gzhubu.top

Lua ............ 10
来源：http://uew.zdbjq.cn

Perl ........... 10
来源：http://crn.hnxiangtu.top

Scala .......... 10
来源：http://hvt.zhongyouzk.top

------------------------------------
来源：http://jkw.gotoacloud.top

合计 ........... 2106 条
来源：http://ldy.zhiwuduotai.top

按章节统计：
来源：http://fwo.hysaishi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lgf.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tcc.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aft.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ewa.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pbh.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ifw.yonumen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dmm.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zxx.gzhubu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ems.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fwr.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ukc.ywan-chungtsiang.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kru.0kj1m.cn


<!-- 参考信息 -->