代发 wailian999

case class User(name: String, age: Int)
来源：http://snc.svipenyu.cn

[T57] Scala：模式匹配
来源：http://abw.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iyo.wangdashe.top

[T58] Scala：函数定义
来源：http://vse.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://isb.bbcook.cn

[T59] Scala：循环
来源：http://yav.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://uub.bjfxy.top

[T60] Scala：折叠
来源：http://aiv.sweek.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vni.guannengcc.top

================================================================================
来源：http://uqt.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvg.hcnkem.com

================================================================================
来源：http://ekq.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://vkv.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://gho.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://sny.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://naa.yj20258.top

[U03] Py：加载 .env 配置
来源：http://fdk.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://coh.vehdjk.com

[U04] Py：变量调试打印
来源：http://kgg.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kuz.nanxuanxn.top

[U05] Py：列表去重且保序
来源：http://mzy.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://bbt.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://cup.zhengqikj.top

{**a, **b}
来源：http://ggr.chenlongwang.top

[U07] Py：反转字典键值
来源：http://xre.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://xen.haohaochexian.top

[U08] Py：展平二维列表
来源：http://jou.vqdsnc.cn

[y for x in nested for y in x]
来源：http://sej.yongpay.top

[U09] Py：字典取最大值的键
来源：http://mul.yj202588.top

max(d, key=d.get)
来源：http://mkl.jinqigufen.top

[U10] Py：按值排序字典
来源：http://vbz.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uze.zhijiandao.cn

[U11] Py：生成器表达式
来源：http://qno.52xcode.cn

(x * 2 for x in arr)
来源：http://gfj.wangdashe.top

[U12] Py：取出现最多的 3 个元素
来源：http://njy.9152youxi.cn

Counter(arr).most_common(3)
来源：http://jzj.hnqzz.top

[U13] Py：固定长度队列
来源：http://kcw.daria6918.cn

deque(maxlen=10)
来源：http://aay.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://wkw.daxiang520.top

defaultdict(list)
来源：http://add.fktsv.cn

[U15] Py：高精度计时
来源：http://cha.yuanzhike.top

t = time.perf_counter()
来源：http://ata.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://szn.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ysu.hesvh.cn

[U17] Py：初始化日志
来源：http://hvk.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://azd.hcnkem.com

[U18] Py：预编译正则
来源：http://bla.yfazqb.com

pat = re.compile(r"\d+")
来源：http://iel.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://cfm.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mov.smart0.xyz

[U20] Py：缓存函数结果
来源：http://jjn.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://adu.tian-w.cn

[U21] Py：自定义上下文管理器
来源：http://jdb.hesvh.cn

@contextlib.contextmanager
来源：http://smg.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://auo.nanxuanxn.top

list(zip(*m))
来源：http://qzp.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://kzn.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://exo.havefunace.top

[U24] Py：路径操作
来源：http://yep.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jkb.ctjpmb.com

[U25] Py：CSV 按字典读
来源：http://qqs.nanxuanxn.top

csv.DictReader(f)
来源：http://qkv.jlsjyb.cn

[U26] Py：并发下载
来源：http://new.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eis.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://uwi.wangshuangyany.cn

aiohttp.ClientSession() 配合 async with
来源：http://jky.aibaodan.cn

[U28] Py：类型别名
来源：http://lqn.cucudq.cn

UserId = int
来源：http://aaj.bbcook.cn

[U29] Py：属性校验
来源：http://ali.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://znj.tarul.cn

[U30] Py：数据类
来源：http://umz.pengpengdd.cyou

@dataclass(slots=True)
来源：http://juk.ivvv.top

[U31] Py：单测
来源：http://jvy.fehbvm.com

python -m pytest -q
来源：http://ajz.daria6918.cn

[U32] Py：代码格式化
来源：http://bxr.yonumen.top

ruff format . && ruff check --fix .
来源：http://gib.zhijiandao.cn

[U33] Py：打包发布
来源：http://qar.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://fae.nwbrower.top

[U34] Py：判断编码
来源：http://nub.ppjwa.cn

chardet.detect(raw)
来源：http://jgq.quarkkingdee.top

[U35] Py：发送邮件
来源：http://mnd.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qvf.redwolf501.top

[U36] Py：定时任务
来源：http://oyv.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://tck.tanke756.top

[U37] Py：读写 Excel
来源：http://bdh.xuetiantiany.cn

pandas.read_excel / DataFrame.to_excel
来源：http://asq.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://scg.hcnkem.com

Path(__file__).resolve().parent
来源：http://kup.xinyue.icu

[U39] Py：判断是否在交互环境
来源：http://cyj.ppjwa.cn

sys.stdout.isatty()
来源：http://jdp.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://iqb.tianlin.xyz

print("err", file=sys.stderr)
来源：http://xix.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://qpg.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://mnk.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://fda.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kkb.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://stk.jqgfzy.top

namespace App\Http;
来源：http://kyc.smart0.xyz

[U44] PHP：开启严格类型
来源：http://tix.pengpengdd.cyou

declare(strict_types=1);
来源：http://hxm.ppjwa.cn

[U45] PHP：类型声明与返回类型
来源：http://nkv.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jye.ivvv.top

[U46] PHP：可空类型
来源：http://bzt.zhongyouzk.top

?string $name = null
来源：http://dgy.guannengcc.top

[U47] PHP：联合类型
来源：http://eyd.ywan-chungtsiang.top

int|string $id
来源：http://rtu.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://gmx.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fcj.havefunace.top

[U49] PHP：只读属性
来源：http://oap.sjlbkw.cn

public readonly string $name
来源：http://dca.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://eph.snrcjt.cn

public function __construct(private int $id) {}
来源：http://jes.chenlongwang.top

[U51] PHP：数组解构
来源：http://flg.dashuyun.cn

[$a, $b] = $arr;
来源：http://rlz.jinyuanbaomall.cn

[U52] PHP：箭头函数
来源：http://fcn.uphjek.com

$double = fn($x) => $x * 2;
来源：http://rdk.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://usx.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://peg.vehdjk.com

[U54] PHP：空安全调用
来源：http://jgl.tianlin.xyz

$obj?->method()
来源：http://fus.zdbjq.cn

[U55] PHP：match 表达式
来源：http://gdz.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jik.yj202588.top

[U56] PHP：命名参数
来源：http://qxe.meibo888.top

f(a: 1, b: 2)
来源：http://xmx.cashguo.top

[U57] PHP：字符串插值
来源：http://aic.gzhubu.top

"值: {$a}"
来源：http://wti.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://lge.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wpq.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://jly.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vvq.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://iza.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gmi.jlsjyb.cn

[U61] PHP：正则
来源：http://boi.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sbw.uphjek.com

[U62] PHP：日期对象
来源：http://kdz.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://csx.fehbvm.com

[U63] PHP：文件读写
来源：http://zha.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kzr.ppjwa.cn

[U64] PHP：目录遍历
来源：http://mmp.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://vkl.fktsv.cn

[U65] PHP：会话
来源：http://adn.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://yzo.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://ari.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ktx.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://ete.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dfs.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://wpv.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://off.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://nam.daxiang520.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lng.xuanzx.com

[U70] PHP：PDO 事务
来源：http://nao.daria6918.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qge.hnqzz.top

[U71] PHP：抛出异常
来源：http://uyu.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://doo.hywenlv.cn

[U72] PHP：写错误日志
来源：http://vwv.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://glt.hfpthk.cn

[U73] PHP：读取 ini 配置
来源：http://uln.zhongyouzk.top

parse_ini_file("config.ini", true)
来源：http://ehq.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://lhw.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://cdm.wangdashe.top

[U75] PHP：依赖注入
来源：http://szn.gogol.net.cn

composer require psr/container
来源：http://mdc.ehwqpu.com

[U76] PHP：简单路由
来源：http://oar.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ivm.wangshuangyany.cn

[U77] PHP：模板渲染
来源：http://rxs.52xcode.cn

composer require twig/twig
来源：http://bbk.iojbl.cn

[U78] PHP：单元测试
来源：http://fzh.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://woe.cheryme.top

[U79] PHP：静态分析
来源：http://ksq.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://nyk.yj202588.top

[U80] PHP：代码规范修复
来源：http://kmo.fzhhl.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gjy.sweek.top

[U81] JS：初始化项目
来源：http://eke.vqdsnc.cn

npm init -y;  npm i express
来源：http://png.gzhubu.top

[U82] JS：package.json 脚本
来源：http://vag.zhiwuduotai.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ruv.ydjk.org.cn

[U83] JS：ES Module 导入导出
来源：http://anc.wangdashe.top

export const a = 1;  import { a } from "./m.js";
来源：http://ojl.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://gmn.52xcode.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jac.sufxvd.cn

[U85] JS：可选链
来源：http://nil.zdqjudy.top

a?.b?.c
来源：http://cfp.mhx1999.top

[U86] JS：空值合并
来源：http://ufo.cucudq.cn

a ?? b
来源：http://mpi.daria6918.cn

[U87] JS：解构默认值
来源：http://vsz.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://sbf.bjfxy.top

[U88] JS：对象展开合并
来源：http://atm.jyoumei.cn

{ ...a, ...b }
来源：http://tyk.meibo888.top

[U89] JS：数组去重
来源：http://jir.zhixingplan.top

[...new Set(arr)]
来源：http://tha.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://jli.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://eni.hnqzz.top

[U91] JS：对象键值遍历
来源：http://uhv.sysykeji.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hro.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://zrv.nwbrower.top

structuredClone(obj)
来源：http://has.xinyue.icu

[U93] JS：模板字符串
来源：http://kzc.cqqwz.cn

`共 ${n} 条`
来源：http://jlc.yanxiufei.cn

[U94] JS：箭头函数
来源：http://wem.zhaomingkeji.xyz

const double = x => x * 2;
来源：http://swk.xuanzx.com

[U95] JS：Promise 包装
来源：http://wkr.ybcxt.top

new Promise((resolve, reject) => {})
来源：http://chv.pycfn.com

[U96] JS：async/await 与异常
来源：http://ugw.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hcc.jiagoushi.top

[U97] JS：并发请求
来源：http://dvp.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qwz.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://huo.daxiang520.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nzc.wangdashe.top

[U99] JS：事件监听
来源：http://txj.mhx1999.top

el.addEventListener("click", e => {})
来源：http://rof.mhx1999.top

[U100] JS：DOM 查询
来源：http://uau.zhoulong.xyz

document.querySelector(".item")
来源：http://dif.xziqi.cn

[U101] JS：classList 操作
来源：http://wdf.iojbl.cn

el.classList.toggle("active")
来源：http://nkt.nanxinkj.top

[U102] JS：本地存储
来源：http://jhv.xuanzx.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://dbn.cqqwz.cn

[U103] JS：定时器
来源：http://xik.andypj.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zjd.yj20258888.top

[U104] JS：防抖
来源：http://zlr.nwbrower.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vuy.smart0.xyz

[U105] JS：节流
来源：http://apu.vqdsnc.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dvp.cqqwz.cn

[U106] JS：日期格式化
来源：http://vez.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fsj.zhijiandao.cn

[U107] JS：数字千分位
来源：http://kkz.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nds.shuidangran.top

[U108] JS：随机整数
来源：http://chf.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ack.yanxiufei.cn

[U109] JS：数组分组
来源：http://lwh.zhongyouzk.top

Object.groupBy(arr, x => x.type)
来源：http://wsa.shuidangran.top

[U110] JS：数组分块
来源：http://bli.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vqa.cheryme.top

[U111] JS：对象转 Map
来源：http://hkp.bjfxy.top

new Map(Object.entries(obj))
来源：http://ztv.sufxvd.cn

[U112] JS：字符串补位
来源：http://rhi.meibo888.top

"7".padStart(3, "0")
来源：http://mia.pycfn.com

[U113] JS：正则替换全部
来源：http://gok.hywenlv.cn

s.replaceAll("a", "b")
来源：http://yas.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://izp.pycfn.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://rhu.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://lxj.jqgfzy.top

crypto.randomUUID()
来源：http://yzs.xingfuxueyuan.xyz

[U116] JS：类型检查（JSDoc）
来源：http://sjf.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://ueu.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://qpq.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://iyc.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://buf.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://zks.gzhubu.top

[U119] JS：生产构建
来源：http://pvj.zdbjq.cn

npx vite build
来源：http://isv.xylfe.cn

[U120] JS：读取环境变量（Vite）
来源：http://apc.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://lxh.ehwqpu.com

================================================================================
来源：http://ujr.hywenlv.cn

统计汇总
来源：http://kko.tarul.cn

================================================================================
来源：http://ysc.ctjpmb.com

按语言统计（条）：
来源：http://kbk.yuanzhike.top

Python ......... 252
来源：http://qsk.vehdjk.com

PHP ............ 252
来源：http://hia.havefunace.top

JavaScript ..... 252
来源：http://kgs.ydzc1.top

TypeScript ..... 212
来源：http://ncs.jinqigufen.top

Java ........... 212
来源：http://rxp.jinghuilouyu.cn

Go ............. 212
来源：http://hbe.hongshengwenyu.top

Ruby ........... 212
来源：http://tpz.snrcjt.cn

C# ............. 212
来源：http://mwq.zhaomingkeji.xyz

C .............. 30
来源：http://dpk.yangfankeji.com

C++ ............ 30
来源：http://uvr.shuidangran.top

SQL ............ 90
来源：http://okn.nanxinkj.top

Bash ........... 80
来源：http://bnu.sufxvd.cn

Kotlin ......... 15
来源：http://wvu.guannengcc.top

Swift .......... 15
来源：http://tum.fengsongda.top

Lua ............ 10
来源：http://cig.yvedp.cn

Perl ........... 10
来源：http://okq.haohaochexian.top

Scala .......... 10
来源：http://lmt.jqgufenzy.top

------------------------------------
来源：http://hpp.yuanzhike.top

合计 ........... 2106 条
来源：http://kti.yvedp.cn

按章节统计：
来源：http://tdb.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://myd.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bak.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://acf.hcnkem.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yav.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rnr.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://msu.bbcook.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ogb.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hck.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nbi.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://toh.jinqigufen.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ktv.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://key.fzhhl.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zgd.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wco.iojbl.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lgg.sysykeji.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ihs.smart0.xyz

Q SQL 专题                              90
来源：http://fnv.yonumen.top

R Bash 专题                             80
来源：http://efi.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://wkn.fktsv.cn

T 其他语言补充                          60
来源：http://bft.cqqwz.cn

U 高频实用片段                         120
来源：http://oax.shanyushiyangkeji.top

------------------------------------
来源：http://puc.zhengqikj.top

合计                                  2106 条
来源：http://upz.iojbl.cn

--------------------------------------------------------------------------------
来源：http://wxi.zhijiandao.cn


<!-- 参考信息 -->