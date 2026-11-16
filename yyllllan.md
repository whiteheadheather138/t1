代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://qlh.tian-w.cn

[T55] Scala：集合过滤
来源：http://wwx.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://itg.ivvv.top

[T56] Scala：样例类
来源：http://mkr.ehwqpu.com

case class User(name: String, age: Int)
来源：http://lal.bjfxy.top

[T57] Scala：模式匹配
来源：http://ckt.shanyushiyangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ums.zycfv.cn

[T58] Scala：函数定义
来源：http://zdm.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://bpp.zhongyouzk.top

[T59] Scala：循环
来源：http://pbd.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://ftb.c1oappe.top

[T60] Scala：折叠
来源：http://hmk.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://erg.cucudq.cn

================================================================================
来源：http://ykk.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bol.c1oappe.top

================================================================================
来源：http://qmw.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://cln.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://exs.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://ate.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xel.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://poo.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://nbq.yongpay.top

[U04] Py：变量调试打印
来源：http://xkc.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pkk.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://zvd.xuanzx.com

list(dict.fromkeys(arr))
来源：http://azb.dashuyun.cn

[U06] Py：合并两个字典
来源：http://ltw.hywenlv.cn

{**a, **b}
来源：http://drn.dashuyun.cn

[U07] Py：反转字典键值
来源：http://izy.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://jsd.chenjidiqi.icu

[U08] Py：展平二维列表
来源：http://nta.yfazqb.com

[y for x in nested for y in x]
来源：http://wnq.yj20258.top

[U09] Py：字典取最大值的键
来源：http://gfn.yongpay.top

max(d, key=d.get)
来源：http://hhq.hywenlv.cn

[U10] Py：按值排序字典
来源：http://adb.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://opw.cucudq.cn

[U11] Py：生成器表达式
来源：http://ngl.fzhhl.top

(x * 2 for x in arr)
来源：http://glb.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ypn.hesvh.cn

Counter(arr).most_common(3)
来源：http://lji.cheryme.top

[U13] Py：固定长度队列
来源：http://gyy.ivvv.top

deque(maxlen=10)
来源：http://bcj.bbcook.cn

[U14] Py：分组收集到列表
来源：http://ybm.guowangkeji.top

defaultdict(list)
来源：http://tdw.zhongyouzk.top

[U15] Py：高精度计时
来源：http://ncm.xinyue.icu

t = time.perf_counter()
来源：http://yee.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://amg.chenlongwang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nmz.guannengcc.top

[U17] Py：初始化日志
来源：http://iyc.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://jvw.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://fhh.xingfuxueyuan.xyz

pat = re.compile(r"\d+")
来源：http://gfx.iojbl.cn

[U19] Py：正则替换带回调
来源：http://dje.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zgi.gzhubu.top

[U20] Py：缓存函数结果
来源：http://lpd.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://aqk.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://jya.yj20258888.top

@contextlib.contextmanager
来源：http://mhs.svipenyu.cn

[U22] Py：矩阵转置
来源：http://sbi.fanxiaobao.xyz

list(zip(*m))
来源：http://jfu.hnqzz.top

[U23] Py：分块读取大文件
来源：http://mdi.zhengqikj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ihk.yj202588.top

[U24] Py：路径操作
来源：http://mdc.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bei.sweek.top

[U25] Py：CSV 按字典读
来源：http://apv.jinqigfzy.top

csv.DictReader(f)
来源：http://jip.vqdsnc.cn

[U26] Py：并发下载
来源：http://ifq.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nsj.zycfv.cn

[U27] Py：异步 HTTP
来源：http://yys.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://piz.birdmap.top

[U28] Py：类型别名
来源：http://ngc.hesvh.cn

UserId = int
来源：http://vit.andypj.xyz

[U29] Py：属性校验
来源：http://rtn.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://hxz.9152youxi.cn

[U30] Py：数据类
来源：http://ntx.ydjk.org.cn

@dataclass(slots=True)
来源：http://oqv.epnwcf.com

[U31] Py：单测
来源：http://ieg.hcnkem.com

python -m pytest -q
来源：http://tks.zdqjudy.top

[U32] Py：代码格式化
来源：http://lel.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://kwk.zhoulong.xyz

[U33] Py：打包发布
来源：http://flt.sysykeji.top

python -m build  （依赖 pyproject.toml）
来源：http://end.jlsjyb.cn

[U34] Py：判断编码
来源：http://rcw.vehdjk.com

chardet.detect(raw)
来源：http://ujp.fehbvm.com

[U35] Py：发送邮件
来源：http://mkg.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zkf.hnxiangtu.top

[U36] Py：定时任务
来源：http://rvx.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://cja.quarkkingdee.top

[U37] Py：读写 Excel
来源：http://fkj.yj20258.top

pandas.read_excel / DataFrame.to_excel
来源：http://pfg.wangshuangyany.cn

[U38] Py：获取脚本所在目录
来源：http://usu.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://ksb.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://zpu.zhixingplan.top

sys.stdout.isatty()
来源：http://dqb.havefunace.top

[U40] Py：打印到标准错误
来源：http://tpm.yuxming.cn

print("err", file=sys.stderr)
来源：http://szu.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://sri.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fvk.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://rgq.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pyn.fzhhl.top

[U43] PHP：声明命名空间
来源：http://ykk.9152youxi.cn

namespace App\Http;
来源：http://srz.c1oappe.top

[U44] PHP：开启严格类型
来源：http://pjm.vqdsnc.cn

declare(strict_types=1);
来源：http://mdb.zdbjq.cn

[U45] PHP：类型声明与返回类型
来源：http://fzy.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bwv.birdmap.top

[U46] PHP：可空类型
来源：http://nxy.cashguo.top

?string $name = null
来源：http://cdk.snrcjt.cn

[U47] PHP：联合类型
来源：http://ymw.yj20258888.top

int|string $id
来源：http://ggw.zhixingplan.top

[U48] PHP：纯枚举
来源：http://xby.snrcjt.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ehz.yj20258888.top

[U49] PHP：只读属性
来源：http://smm.zhixingplan.top

public readonly string $name
来源：http://jsy.cheryme.top

[U50] PHP：构造器属性提升
来源：http://gop.yongpay.top

public function __construct(private int $id) {}
来源：http://bzi.vqdsnc.cn

[U51] PHP：数组解构
来源：http://pts.pycfn.com

[$a, $b] = $arr;
来源：http://sbp.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://wfl.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://tfu.fktsv.cn

[U53] PHP：空合并运算符
来源：http://mmj.sweek.top

$v = $a ?? $b ?? "default";
来源：http://muq.ydzc1.top

[U54] PHP：空安全调用
来源：http://igf.ppjwa.cn

$obj?->method()
来源：http://gqq.yangfankeji.com

[U55] PHP：match 表达式
来源：http://qdo.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pra.zhixingplan.top

[U56] PHP：命名参数
来源：http://ndr.yangfankeji.com

f(a: 1, b: 2)
来源：http://pum.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://xqe.dashuyun.cn

"值: {$a}"
来源：http://ljn.havefunace.top

[U58] PHP：数组三件套
来源：http://cas.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mtb.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://gka.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fwc.hfpthk.cn

[U60] PHP：JSON 编解码
来源：http://xxb.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://clz.feifeiyinyue.top

[U61] PHP：正则
来源：http://mct.fehbvm.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qwh.kuanghao11.cn

[U62] PHP：日期对象
来源：http://gua.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xba.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://swv.birdmap.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://stc.hammf.cn

[U64] PHP：目录遍历
来源：http://msh.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://tcd.jqgufenzy.top

[U65] PHP：会话
来源：http://ruz.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://wff.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://bja.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fds.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://skg.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aso.sysykeji.top

[U68] PHP：PDO 连接
来源：http://dng.fzhhl.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://onu.tanke756.top

[U69] PHP：PDO 预处理
来源：http://daw.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hoy.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://qme.wangdashe.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xqo.zhijiandao.cn

[U71] PHP：抛出异常
来源：http://uwg.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://uip.jyoumei.cn

[U72] PHP：写错误日志
来源：http://sno.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://btv.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://wfv.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://nqo.zycfv.cn

[U74] PHP：读取环境变量
来源：http://rmt.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://gjz.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://ave.jqgufenzy.top

composer require psr/container
来源：http://ure.shanyushiyangkeji.top

[U76] PHP：简单路由
来源：http://lvq.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://twj.hnxiangtu.top

[U77] PHP：模板渲染
来源：http://mcv.fehbvm.com

composer require twig/twig
来源：http://oju.uphjek.com

[U78] PHP：单元测试
来源：http://egn.ehwqpu.com

composer require --dev phpunit/phpunit
来源：http://ssk.yueranfly.top

[U79] PHP：静态分析
来源：http://zwp.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://nfk.yongpay.top

[U80] PHP：代码规范修复
来源：http://mua.xylfe.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xdy.hysaishi.cn

[U81] JS：初始化项目
来源：http://brl.birdmap.top

npm init -y;  npm i express
来源：http://ulr.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://noi.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kjz.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://lgi.zhoulong.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://kai.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://rej.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ykk.jqgufenzy.top

[U85] JS：可选链
来源：http://pnw.kuanghao11.cn

a?.b?.c
来源：http://tar.yuxming.cn

[U86] JS：空值合并
来源：http://gqi.havefunace.top

a ?? b
来源：http://urp.daria6918.cn

[U87] JS：解构默认值
来源：http://bth.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://ksw.52xcode.cn

[U88] JS：对象展开合并
来源：http://cvc.ybcxt.top

{ ...a, ...b }
来源：http://clz.316326.xyz

[U89] JS：数组去重
来源：http://cas.jiagoushi.top

[...new Set(arr)]
来源：http://lon.gotoacloud.top

[U90] JS：数字数组排序
来源：http://myt.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://dvj.hnqzz.top

[U91] JS：对象键值遍历
来源：http://kjo.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rtk.cdnleiting.top

[U92] JS：深拷贝
来源：http://plx.yj202588.top

structuredClone(obj)
来源：http://sbi.fktsv.cn

[U93] JS：模板字符串
来源：http://pqw.cdnleiting.top

`共 ${n} 条`
来源：http://xqk.ywan-chungtsiang.top

[U94] JS：箭头函数
来源：http://cfs.ydzc1.top

const double = x => x * 2;
来源：http://lsl.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://kxi.zdqjudy.top

new Promise((resolve, reject) => {})
来源：http://kzy.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://bii.ehwqpu.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://upo.vehdjk.com

[U97] JS：并发请求
来源：http://pog.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://epr.ybcxt.top

[U98] JS：fetch 带 JSON
来源：http://nka.ywan-chungtsiang.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ebo.zhixingplan.top

[U99] JS：事件监听
来源：http://ezv.uphjek.com

el.addEventListener("click", e => {})
来源：http://fzc.redwolf501.top

[U100] JS：DOM 查询
来源：http://vyt.52xcode.cn

document.querySelector(".item")
来源：http://jkm.zhengqikj.top

[U101] JS：classList 操作
来源：http://imj.hesvh.cn

el.classList.toggle("active")
来源：http://ixo.ybcxt.top

[U102] JS：本地存储
来源：http://myv.yj20258888.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lvc.epnwcf.com

[U103] JS：定时器
来源：http://hgl.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://txe.tian-w.cn

[U104] JS：防抖
来源：http://wfe.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndr.hysaishi.cn

[U105] JS：节流
来源：http://gez.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nnb.jyoumei.cn

[U106] JS：日期格式化
来源：http://aqr.feifeiyinyue.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wbr.hnxiangtu.top

[U107] JS：数字千分位
来源：http://scs.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ncf.xinyue.icu

[U108] JS：随机整数
来源：http://uaw.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xjy.nanxinkj.top

[U109] JS：数组分组
来源：http://ufs.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://uqb.jqgfzy.top

[U110] JS：数组分块
来源：http://qdt.shanyushiyangkeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mpq.ydzc1.top

[U111] JS：对象转 Map
来源：http://tcy.uphjek.com

new Map(Object.entries(obj))
来源：http://mio.zhiwuduotai.top

[U112] JS：字符串补位
来源：http://miz.hywenlv.cn

"7".padStart(3, "0")
来源：http://nqi.hfpthk.cn

[U113] JS：正则替换全部
来源：http://hat.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://ete.jqgufenzy.top

[U114] JS：JSON 深比较
来源：http://ivn.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fvt.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://pgy.pycfn.com

crypto.randomUUID()
来源：http://eyn.jiagoushi.top

[U116] JS：类型检查（JSDoc）
来源：http://ryg.tarul.cn

/** @param {string} name */ function f(name) {}
来源：http://owg.hammf.cn

[U117] JS：单元测试
来源：http://tsb.yueranfly.top

npm i -D vitest;  npx vitest
来源：http://kdr.9152youxi.cn

[U118] JS：开发服务器
来源：http://sua.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://mmd.guowangkeji.top

[U119] JS：生产构建
来源：http://ecz.ydzc1.top

npx vite build
来源：http://imx.smart0.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ohk.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://sul.cdnleiting.top

================================================================================
来源：http://mno.snrcjt.cn

统计汇总
来源：http://wmj.hywenlv.cn

================================================================================
来源：http://sch.dashuyun.cn

按语言统计（条）：
来源：http://qyw.jinqigufen.top

Python ......... 252
来源：http://zyw.bbcook.cn

PHP ............ 252
来源：http://eia.iojbl.cn

JavaScript ..... 252
来源：http://nwg.xziqi.cn

TypeScript ..... 212
来源：http://nib.zycfv.cn

Java ........... 212
来源：http://oxa.fanxiaobao.xyz

Go ............. 212
来源：http://qxz.yanxiufei.cn

Ruby ........... 212
来源：http://vmc.gotoacloud.top

C# ............. 212
来源：http://rjx.ydjk.org.cn

C .............. 30
来源：http://wcz.jianghu66.top

C++ ............ 30
来源：http://tng.hesvh.cn

SQL ............ 90
来源：http://jls.hongshengwenyu.top

Bash ........... 80
来源：http://ksp.cucudq.cn

Kotlin ......... 15
来源：http://kcm.nanxuanxn.top

Swift .......... 15
来源：http://fji.yonumen.top

Lua ............ 10
来源：http://ska.xinyue.icu

Perl ........... 10
来源：http://tky.jinqigufen.top

Scala .......... 10
来源：http://xke.zhoulong.xyz

------------------------------------
来源：http://pgd.sjlbkw.cn

合计 ........... 2106 条
来源：http://xvd.gaohongyu789.top

按章节统计：
来源：http://wpj.zhongyouzk.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zay.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jgt.zhaomingkeji.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://niq.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://onr.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://omp.zhijiandao.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ory.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hen.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xvs.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://agi.jyoumei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://glq.yj20258888.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pli.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://khf.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qxx.zhaomingkeji.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ueb.tianlin.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ttz.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qwx.jinqigufen.top

Q SQL 专题                              90
来源：http://bhq.jlsjyb.cn

R Bash 专题                             80
来源：http://dvb.chenlongwang.top

S C / C++ 专题                          60
来源：http://inq.9152youxi.cn

T 其他语言补充                          60
来源：http://mba.yuanzhike.top


<!-- 参考信息 -->