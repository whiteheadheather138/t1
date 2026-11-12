代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://vlq.cqqwz.cn

[T55] Scala：集合过滤
来源：http://sof.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://few.yueranfly.top

[T56] Scala：样例类
来源：http://rhh.havefunace.top

case class User(name: String, age: Int)
来源：http://tzt.uphjek.com

[T57] Scala：模式匹配
来源：http://lbt.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://fif.yj20258888.top

[T58] Scala：函数定义
来源：http://jds.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://lxr.gogol.net.cn

[T59] Scala：循环
来源：http://bcb.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://cxc.tanke756.top

[T60] Scala：折叠
来源：http://gux.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xzu.chenzaomai.com

================================================================================
来源：http://ull.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jrb.bjfxy.top

================================================================================
来源：http://nim.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://nrz.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://oun.c1oappe.top

[U02] Py：导出 / 安装依赖
来源：http://tlz.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nxa.cheryme.top

[U03] Py：加载 .env 配置
来源：http://ykk.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zft.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://ozx.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hqd.52xcode.cn

[U05] Py：列表去重且保序
来源：http://qku.guannengcc.top

list(dict.fromkeys(arr))
来源：http://dom.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://fpc.zdbjq.cn

{**a, **b}
来源：http://ghv.ppjwa.cn

[U07] Py：反转字典键值
来源：http://txq.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://fuu.smart0.xyz

[U08] Py：展平二维列表
来源：http://jdc.yuxming.cn

[y for x in nested for y in x]
来源：http://npx.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://ekj.hnqzz.top

max(d, key=d.get)
来源：http://ybc.zhijiandao.cn

[U10] Py：按值排序字典
来源：http://fda.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rou.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://ife.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://eri.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fmk.vehdjk.com

Counter(arr).most_common(3)
来源：http://ddi.ctjpmb.com

[U13] Py：固定长度队列
来源：http://jrn.52xcode.cn

deque(maxlen=10)
来源：http://zmg.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://ccw.zhoulong.xyz

defaultdict(list)
来源：http://mcg.shzxlz.cn

[U15] Py：高精度计时
来源：http://iyn.daxiang520.top

t = time.perf_counter()
来源：http://jra.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://dtj.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ifk.hnxiangtu.top

[U17] Py：初始化日志
来源：http://abw.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://umt.gaohongyu789.top

[U18] Py：预编译正则
来源：http://jti.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://mkn.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://nzu.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fyg.xuetiantiany.cn

[U20] Py：缓存函数结果
来源：http://vuv.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://ntz.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://iey.xuetiantiany.cn

@contextlib.contextmanager
来源：http://esw.svipenyu.cn

[U22] Py：矩阵转置
来源：http://zit.daxiang520.top

list(zip(*m))
来源：http://nhb.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://adl.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uxo.fengsongda.top

[U24] Py：路径操作
来源：http://bpp.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://etr.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://cdy.zhijiandao.cn

csv.DictReader(f)
来源：http://ibu.sysykeji.top

[U26] Py：并发下载
来源：http://nps.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jrv.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://rbl.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://qfw.c1oappe.top

[U28] Py：类型别名
来源：http://ows.yangfankeji.com

UserId = int
来源：http://deg.pengpengdd.cyou

[U29] Py：属性校验
来源：http://wyq.cashguo.top

@property 与 @x.setter 配合
来源：http://isn.tianlin.xyz

[U30] Py：数据类
来源：http://plt.zhiwuduotai.top

@dataclass(slots=True)
来源：http://tnn.hongshengwenyu.top

[U31] Py：单测
来源：http://ylu.fktsv.cn

python -m pytest -q
来源：http://kkt.haohaochexian.top

[U32] Py：代码格式化
来源：http://qpx.iojbl.cn

ruff format . && ruff check --fix .
来源：http://kus.birdmap.top

[U33] Py：打包发布
来源：http://dhq.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://awa.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://gwt.daxiang520.top

chardet.detect(raw)
来源：http://fqs.ivvv.top

[U35] Py：发送邮件
来源：http://eho.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ugc.gogol.net.cn

[U36] Py：定时任务
来源：http://gdm.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://mxx.gotoacloud.top

[U37] Py：读写 Excel
来源：http://jjk.bjfxy.top

pandas.read_excel / DataFrame.to_excel
来源：http://ocq.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://eri.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://die.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://ppo.zhijiandao.cn

sys.stdout.isatty()
来源：http://rbt.fehbvm.com

[U40] Py：打印到标准错误
来源：http://zcx.yueranfly.top

print("err", file=sys.stderr)
来源：http://xpd.jinyuanbaomall.cn

[U41] PHP：初始化 Composer 项目
来源：http://upt.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uhm.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://nqz.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hru.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://lan.yonumen.top

namespace App\Http;
来源：http://ruu.hcnkem.com

[U44] PHP：开启严格类型
来源：http://cem.jqgufenzy.top

declare(strict_types=1);
来源：http://dnc.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://nfq.zhiwuduotai.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://flt.jqgufenzy.top

[U46] PHP：可空类型
来源：http://sml.hcnkem.com

?string $name = null
来源：http://ucs.xuanzx.com

[U47] PHP：联合类型
来源：http://ebl.feifeiyinyue.top

int|string $id
来源：http://eut.andypj.xyz

[U48] PHP：纯枚举
来源：http://bxh.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mqe.gogol.net.cn

[U49] PHP：只读属性
来源：http://pnr.jinyuanbaomall.cn

public readonly string $name
来源：http://nsa.yj202588.top

[U50] PHP：构造器属性提升
来源：http://rjv.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://dnk.meibo888.top

[U51] PHP：数组解构
来源：http://bgy.jiagoushi.top

[$a, $b] = $arr;
来源：http://kct.zhixingplan.top

[U52] PHP：箭头函数
来源：http://cei.hywenlv.cn

$double = fn($x) => $x * 2;
来源：http://fig.chenzaomai.com

[U53] PHP：空合并运算符
来源：http://pip.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://ale.sysykeji.top

[U54] PHP：空安全调用
来源：http://wyy.zhaomingkeji.xyz

$obj?->method()
来源：http://red.jianghu66.top

[U55] PHP：match 表达式
来源：http://weq.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lfv.hywenlv.cn

[U56] PHP：命名参数
来源：http://tie.hfpthk.cn

f(a: 1, b: 2)
来源：http://dxl.yj202588.top

[U57] PHP：字符串插值
来源：http://lrp.fzhhl.top

"值: {$a}"
来源：http://rtr.shzxlz.cn

[U58] PHP：数组三件套
来源：http://pxd.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fji.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://cin.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vuh.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://aio.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zga.316326.xyz

[U61] PHP：正则
来源：http://wks.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://alg.fehbvm.com

[U62] PHP：日期对象
来源：http://vkw.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xzc.havefunace.top

[U63] PHP：文件读写
来源：http://mom.jinyuanbaomall.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://num.yongpay.top

[U64] PHP：目录遍历
来源：http://brs.guannengcc.top

glob("dir/*.php");  scandir("dir");
来源：http://idq.cdnleiting.top

[U65] PHP：会话
来源：http://ryt.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qtr.shuidangran.top

[U66] PHP：设置 Cookie
来源：http://ucu.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eyj.fktsv.cn

[U67] PHP：处理文件上传
来源：http://xyz.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vox.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://nue.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bet.zdqjudy.top

[U69] PHP：PDO 预处理
来源：http://bwt.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vpx.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://vna.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ipq.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://iwf.c1oappe.top

throw new RuntimeException("失败", 500);
来源：http://tsu.fzhhl.top

[U72] PHP：写错误日志
来源：http://oxs.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://usc.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://dzx.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://umg.gzhubu.top

[U74] PHP：读取环境变量
来源：http://rkm.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://nji.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://hso.sjlbkw.cn

composer require psr/container
来源：http://omc.nwbrower.top

[U76] PHP：简单路由
来源：http://elj.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nxy.zdbjq.cn

[U77] PHP：模板渲染
来源：http://uwf.sjlbkw.cn

composer require twig/twig
来源：http://dqb.jianghu66.top

[U78] PHP：单元测试
来源：http://wrz.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://xic.hnqzz.top

[U79] PHP：静态分析
来源：http://ovi.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://nwa.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://eag.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cvb.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://waz.quarkkingdee.top

npm init -y;  npm i express
来源：http://rhm.ivvv.top

[U82] JS：package.json 脚本
来源：http://hyr.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lud.cheryme.top

[U83] JS：ES Module 导入导出
来源：http://qua.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://ddm.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://vqq.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://iuu.yanxiufei.cn

[U85] JS：可选链
来源：http://ouc.jiagoushi.top

a?.b?.c
来源：http://ttx.uphjek.com

[U86] JS：空值合并
来源：http://xiw.gaohongyu789.top

a ?? b
来源：http://zuv.zycfv.cn

[U87] JS：解构默认值
来源：http://mpg.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://jsf.pengpengdd.cyou

[U88] JS：对象展开合并
来源：http://vmh.sweek.top

{ ...a, ...b }
来源：http://kdq.vehdjk.com

[U89] JS：数组去重
来源：http://odq.shzxlz.cn

[...new Set(arr)]
来源：http://jkb.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://xos.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://rxv.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://dng.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cfc.zhijiandao.cn

[U92] JS：深拷贝
来源：http://hir.daxiang520.top

structuredClone(obj)
来源：http://xnz.cucudq.cn

[U93] JS：模板字符串
来源：http://jbv.52xcode.cn

`共 ${n} 条`
来源：http://gkl.quarkkingdee.top

[U94] JS：箭头函数
来源：http://spk.c1oappe.top

const double = x => x * 2;
来源：http://qxk.vqdsnc.cn

[U95] JS：Promise 包装
来源：http://rna.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://poz.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://hyg.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wqm.chenzaomai.com

[U97] JS：并发请求
来源：http://vbd.fktsv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mgq.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://ldn.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rnk.meibo888.top

[U99] JS：事件监听
来源：http://oco.pycfn.com

el.addEventListener("click", e => {})
来源：http://cke.iojbl.cn

[U100] JS：DOM 查询
来源：http://rju.jiagoushi.top

document.querySelector(".item")
来源：http://bex.sysykeji.top

[U101] JS：classList 操作
来源：http://ddh.shangyingyoupin.top

el.classList.toggle("active")
来源：http://wla.tian-w.cn

[U102] JS：本地存储
来源：http://udl.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lay.iojbl.cn

[U103] JS：定时器
来源：http://eft.xuanzx.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jyt.ydjk.org.cn

[U104] JS：防抖
来源：http://rsz.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cht.zhixingplan.top

[U105] JS：节流
来源：http://ggp.ctjpmb.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wom.chenlongwang.top

[U106] JS：日期格式化
来源：http://yvb.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jom.52xcode.cn

[U107] JS：数字千分位
来源：http://rpe.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bio.yonumen.top

[U108] JS：随机整数
来源：http://acy.fengsongda.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hil.yfazqb.com

[U109] JS：数组分组
来源：http://gtj.yvedp.cn

Object.groupBy(arr, x => x.type)
来源：http://fst.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://ymq.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://oef.hysaishi.cn

[U111] JS：对象转 Map
来源：http://xyl.smart0.xyz

new Map(Object.entries(obj))
来源：http://bge.nanxinkj.top

[U112] JS：字符串补位
来源：http://woe.yj202588.top

"7".padStart(3, "0")
来源：http://smy.xuetiantiany.cn

[U113] JS：正则替换全部
来源：http://pbe.pycfn.com

s.replaceAll("a", "b")
来源：http://dmu.jinghuilouyu.cn

[U114] JS：JSON 深比较
来源：http://bpv.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://arh.aizwys.cn

[U115] JS：生成 UUID
来源：http://nrr.xziqi.cn

crypto.randomUUID()
来源：http://hlx.guannengcc.top

[U116] JS：类型检查（JSDoc）
来源：http://gby.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://cgg.0kj1m.cn

[U117] JS：单元测试
来源：http://shg.zhengqikj.top

npm i -D vitest;  npx vitest
来源：http://xth.jiagoushi.top

[U118] JS：开发服务器
来源：http://xuz.zhijiandao.cn

npm i -D vite;  npx vite
来源：http://zet.shanyushiyangtech.top

[U119] JS：生产构建
来源：http://fyz.shangyingyoupin.top

npx vite build
来源：http://pyx.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://czd.zhengqikj.top

import.meta.env.VITE_API_URL
来源：http://poo.cheryme.top

================================================================================
来源：http://olv.nwbrower.top

统计汇总
来源：http://smz.yongpay.top

================================================================================
来源：http://bit.sysykeji.top

按语言统计（条）：
来源：http://wcj.kuanghao11.cn

Python ......... 252
来源：http://xyp.shanyushiyangtech.top

PHP ............ 252
来源：http://cdt.feifeiyinyue.top

JavaScript ..... 252
来源：http://bbq.jinqigufen.top

TypeScript ..... 212
来源：http://svm.c1oappe.top

Java ........... 212
来源：http://pur.gotoacloud.top

Go ............. 212
来源：http://fsz.redwolf501.top

Ruby ........... 212
来源：http://ewo.ehwqpu.com

C# ............. 212
来源：http://lts.redwolf501.top

C .............. 30
来源：http://rfo.wangshuangyany.cn

C++ ............ 30
来源：http://ixv.birdmap.top

SQL ............ 90
来源：http://soi.wangdashe.top

Bash ........... 80
来源：http://oty.snrcjt.cn

Kotlin ......... 15
来源：http://zml.52xcode.cn

Swift .......... 15
来源：http://ilf.jinqigfzy.top

Lua ............ 10
来源：http://tqk.snrcjt.cn

Perl ........... 10
来源：http://edc.andypj.xyz

Scala .......... 10
来源：http://tjz.sufxvd.cn

------------------------------------
来源：http://bme.gzhubu.top

合计 ........... 2106 条
来源：http://yrn.jinqigufen.top

按章节统计：
来源：http://lid.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iks.chenlongwang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jem.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://npe.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jiw.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yka.yfazqb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hwa.316326.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ymh.316326.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bim.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uuq.pycfn.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://spv.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hhh.shanyushiyangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iqw.hesvh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ake.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vmo.xuetiantiany.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dqi.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://iui.0kj1m.cn

Q SQL 专题                              90
来源：http://eny.feifeiyinyue.top

R Bash 专题                             80
来源：http://pyo.nwbrower.top

S C / C++ 专题                          60
来源：http://dmm.guannengcc.top

T 其他语言补充                          60
来源：http://ath.yuanzhike.top


<!-- 参考信息 -->