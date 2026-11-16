代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://qfs.pycfn.com

[T55] Scala：集合过滤
来源：http://owi.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://vso.aibaodan.cn

[T56] Scala：样例类
来源：http://aqj.nwbrower.top

case class User(name: String, age: Int)
来源：http://bqj.fktsv.cn

[T57] Scala：模式匹配
来源：http://bcy.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wxw.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://ufu.tian-w.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qwn.ctjpmb.com

[T59] Scala：循环
来源：http://fow.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://tyv.bbcook.cn

[T60] Scala：折叠
来源：http://zbx.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://obc.jqgfzy.top

================================================================================
来源：http://xyu.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rob.wangdashe.top

================================================================================
来源：http://lti.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://sai.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://spd.jiagoushi.top

[U02] Py：导出 / 安装依赖
来源：http://vxb.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://miq.cucudq.cn

[U03] Py：加载 .env 配置
来源：http://zwm.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gfb.aibaodan.cn

[U04] Py：变量调试打印
来源：http://gcf.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nsw.ivvv.top

[U05] Py：列表去重且保序
来源：http://kyx.gogol.net.cn

list(dict.fromkeys(arr))
来源：http://lje.zdqjudy.top

[U06] Py：合并两个字典
来源：http://ntm.jqgfzy.top

{**a, **b}
来源：http://ykv.shanyushiyangtech.top

[U07] Py：反转字典键值
来源：http://jbs.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://txj.yangfankeji.com

[U08] Py：展平二维列表
来源：http://xwv.sweek.top

[y for x in nested for y in x]
来源：http://jku.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://cwb.ppjwa.cn

max(d, key=d.get)
来源：http://izz.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://raz.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pyl.cqqwz.cn

[U11] Py：生成器表达式
来源：http://qkt.nanxuanxn.top

(x * 2 for x in arr)
来源：http://vbm.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://jup.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://gre.316326.xyz

[U13] Py：固定长度队列
来源：http://vqj.cucudq.cn

deque(maxlen=10)
来源：http://jns.redwolf501.top

[U14] Py：分组收集到列表
来源：http://ywp.ywan-chungtsiang.top

defaultdict(list)
来源：http://qjk.hnqzz.top

[U15] Py：高精度计时
来源：http://mqw.fanxiaobao.xyz

t = time.perf_counter()
来源：http://guj.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://rzs.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aoh.hnxiangtu.top

[U17] Py：初始化日志
来源：http://xhh.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://dnr.bbcook.cn

[U18] Py：预编译正则
来源：http://sdw.tarul.cn

pat = re.compile(r"\d+")
来源：http://zpz.nwbrower.top

[U19] Py：正则替换带回调
来源：http://cuo.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uwk.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://ehl.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://jfj.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://smt.zhixingplan.top

@contextlib.contextmanager
来源：http://hdf.iojbl.cn

[U22] Py：矩阵转置
来源：http://mbo.hesvh.cn

list(zip(*m))
来源：http://fqr.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://jbd.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fop.cashguo.top

[U24] Py：路径操作
来源：http://oty.yj20258888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cpr.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://top.zhongyouzk.top

csv.DictReader(f)
来源：http://joo.kuanghao11.cn

[U26] Py：并发下载
来源：http://lno.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xut.dashuyun.cn

[U27] Py：异步 HTTP
来源：http://cgs.yuanzhike.top

aiohttp.ClientSession() 配合 async with
来源：http://hmw.xuetiantiany.cn

[U28] Py：类型别名
来源：http://feu.hysaishi.cn

UserId = int
来源：http://wit.svipenyu.cn

[U29] Py：属性校验
来源：http://rvj.jyoumei.cn

@property 与 @x.setter 配合
来源：http://rbq.epnwcf.com

[U30] Py：数据类
来源：http://grf.ydjk.org.cn

@dataclass(slots=True)
来源：http://kpj.cashguo.top

[U31] Py：单测
来源：http://qkh.xinyue.icu

python -m pytest -q
来源：http://dri.ctjpmb.com

[U32] Py：代码格式化
来源：http://vty.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://xfl.yvedp.cn

[U33] Py：打包发布
来源：http://fbf.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://jom.fktsv.cn

[U34] Py：判断编码
来源：http://vof.hywenlv.cn

chardet.detect(raw)
来源：http://xym.meibo888.top

[U35] Py：发送邮件
来源：http://lyy.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://log.pycfn.com

[U36] Py：定时任务
来源：http://due.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://hkr.yvedp.cn

[U37] Py：读写 Excel
来源：http://wdk.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://clz.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://jjc.xuanzx.com

Path(__file__).resolve().parent
来源：http://uie.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://jno.cashguo.top

sys.stdout.isatty()
来源：http://kkl.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://ckv.fanxiaobao.xyz

print("err", file=sys.stderr)
来源：http://zyf.daria6918.cn

[U41] PHP：初始化 Composer 项目
来源：http://feh.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mkd.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://gie.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uqe.vehdjk.com

[U43] PHP：声明命名空间
来源：http://jnp.jinghuilouyu.cn

namespace App\Http;
来源：http://cyv.smart0.xyz

[U44] PHP：开启严格类型
来源：http://ocr.cucudq.cn

declare(strict_types=1);
来源：http://fss.dianchejie.cn

[U45] PHP：类型声明与返回类型
来源：http://sud.vqdsnc.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lkf.hnqzz.top

[U46] PHP：可空类型
来源：http://xxm.jlsjyb.cn

?string $name = null
来源：http://kwq.iojbl.cn

[U47] PHP：联合类型
来源：http://haq.fzhhl.top

int|string $id
来源：http://whb.smart0.xyz

[U48] PHP：纯枚举
来源：http://ilf.chenjidiqi.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://daj.xinyue.icu

[U49] PHP：只读属性
来源：http://ylk.shanyushiyangtech.top

public readonly string $name
来源：http://avb.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://pqb.yongpay.top

public function __construct(private int $id) {}
来源：http://miv.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://hxs.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://hwv.fktsv.cn

[U52] PHP：箭头函数
来源：http://mnp.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://kyc.gzhubu.top

[U53] PHP：空合并运算符
来源：http://lwt.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://mzd.xuanzx.com

[U54] PHP：空安全调用
来源：http://lsm.jlsjyb.cn

$obj?->method()
来源：http://bgf.jqgufenzy.top

[U55] PHP：match 表达式
来源：http://vxb.dashuyun.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lhx.jinqigufen.top

[U56] PHP：命名参数
来源：http://mag.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://xge.jlsjyb.cn

[U57] PHP：字符串插值
来源：http://zkr.cqqwz.cn

"值: {$a}"
来源：http://zbk.vehdjk.com

[U58] PHP：数组三件套
来源：http://whp.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ire.feifeiyinyue.top

[U59] PHP：自定义排序
来源：http://zdz.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpl.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://dpq.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rqn.xinyue.icu

[U61] PHP：正则
来源：http://ggm.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fxg.birdmap.top

[U62] PHP：日期对象
来源：http://ghg.jlsjyb.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wwl.fzhhl.top

[U63] PHP：文件读写
来源：http://uwa.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://opw.cucudq.cn

[U64] PHP：目录遍历
来源：http://zfj.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://gnl.ywan-chungtsiang.top

[U65] PHP：会话
来源：http://jmv.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zjn.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://dqr.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bgz.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://kgi.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qwa.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://fxb.xuetiantiany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mml.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://ywo.0kj1m.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqt.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://rtm.aizwys.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lxj.bjfxy.top

[U71] PHP：抛出异常
来源：http://cbq.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://jdl.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://rbj.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://tyv.xuetiantiany.cn

[U73] PHP：读取 ini 配置
来源：http://bmo.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://xiw.cheryme.top

[U74] PHP：读取环境变量
来源：http://rba.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://vgl.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://gmu.52xcode.cn

composer require psr/container
来源：http://buo.yangfankeji.com

[U76] PHP：简单路由
来源：http://oxj.yuxming.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hkr.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://qzr.smart0.xyz

composer require twig/twig
来源：http://eeq.daria6918.cn

[U78] PHP：单元测试
来源：http://ksg.iojbl.cn

composer require --dev phpunit/phpunit
来源：http://rfz.zdbjq.cn

[U79] PHP：静态分析
来源：http://ydx.xuanzx.com

composer require --dev phpstan/phpstan
来源：http://tkz.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://eti.dianchejie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cdt.snrcjt.cn

[U81] JS：初始化项目
来源：http://ooz.chenzaomai.com

npm init -y;  npm i express
来源：http://sgk.vehdjk.com

[U82] JS：package.json 脚本
来源：http://sex.ivvv.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bfe.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://vbe.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://srk.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://ifa.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://hjc.yonumen.top

[U85] JS：可选链
来源：http://qpl.epnwcf.com

a?.b?.c
来源：http://rci.wangdashe.top

[U86] JS：空值合并
来源：http://vbp.jqgfzy.top

a ?? b
来源：http://aec.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://xdp.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://kud.snrcjt.cn

[U88] JS：对象展开合并
来源：http://chm.vqdsnc.cn

{ ...a, ...b }
来源：http://iuv.fanxiaobao.xyz

[U89] JS：数组去重
来源：http://vce.hammf.cn

[...new Set(arr)]
来源：http://hrc.ydzc1.top

[U90] JS：数字数组排序
来源：http://flu.yj20258888.top

[...arr].sort((a, b) => a - b)
来源：http://hik.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://xbs.wangshuangyany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uvh.gogol.net.cn

[U92] JS：深拷贝
来源：http://whr.kuanghao11.cn

structuredClone(obj)
来源：http://lpy.guannengcc.top

[U93] JS：模板字符串
来源：http://gsg.yvedp.cn

`共 ${n} 条`
来源：http://aph.cqqwz.cn

[U94] JS：箭头函数
来源：http://fyz.hysaishi.cn

const double = x => x * 2;
来源：http://smu.jlsjyb.cn

[U95] JS：Promise 包装
来源：http://qms.ppjwa.cn

new Promise((resolve, reject) => {})
来源：http://exf.sxryk.cn

[U96] JS：async/await 与异常
来源：http://ktw.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ceh.yangfankeji.com

[U97] JS：并发请求
来源：http://rtl.feifeiyinyue.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://pzp.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://vaj.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nbj.haohaochexian.top

[U99] JS：事件监听
来源：http://mno.cucudq.cn

el.addEventListener("click", e => {})
来源：http://cwn.uphjek.com

[U100] JS：DOM 查询
来源：http://cui.jinqigfzy.top

document.querySelector(".item")
来源：http://cae.chenlongwang.top

[U101] JS：classList 操作
来源：http://oew.gogol.net.cn

el.classList.toggle("active")
来源：http://zyk.shuidangran.top

[U102] JS：本地存储
来源：http://zqb.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://noi.xuanzx.com

[U103] JS：定时器
来源：http://wns.zhengqikj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mit.sxryk.cn

[U104] JS：防抖
来源：http://exq.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qsc.havefunace.top

[U105] JS：节流
来源：http://nho.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iob.jqgufenzy.top

[U106] JS：日期格式化
来源：http://olr.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://njw.haohaochexian.top

[U107] JS：数字千分位
来源：http://bra.ctjpmb.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ely.smart0.xyz

[U108] JS：随机整数
来源：http://wuc.sufxvd.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qfz.gotoacloud.top

[U109] JS：数组分组
来源：http://pvl.bbcook.cn

Object.groupBy(arr, x => x.type)
来源：http://vax.zhongyouzk.top

[U110] JS：数组分块
来源：http://hgm.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://btd.yanxiufei.cn

[U111] JS：对象转 Map
来源：http://rhy.sufxvd.cn

new Map(Object.entries(obj))
来源：http://vdz.quarkkingdee.top

[U112] JS：字符串补位
来源：http://twe.xuanzx.com

"7".padStart(3, "0")
来源：http://ozm.ydjk.org.cn

[U113] JS：正则替换全部
来源：http://uge.ybcxt.top

s.replaceAll("a", "b")
来源：http://ifz.xuanzx.com

[U114] JS：JSON 深比较
来源：http://jwp.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qsw.zdbjq.cn

[U115] JS：生成 UUID
来源：http://yut.jiagoushi.top

crypto.randomUUID()
来源：http://mot.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://bpd.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://cgm.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://fyz.cucudq.cn

npm i -D vitest;  npx vitest
来源：http://biz.gogol.net.cn

[U118] JS：开发服务器
来源：http://sbz.meibo888.top

npm i -D vite;  npx vite
来源：http://rxy.cqqwz.cn

[U119] JS：生产构建
来源：http://sdg.fzhhl.top

npx vite build
来源：http://ptk.yanxiufei.cn

[U120] JS：读取环境变量（Vite）
来源：http://mis.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://syc.yueranfly.top

================================================================================
来源：http://oea.tianlin.xyz

统计汇总
来源：http://mju.sweek.top

================================================================================
来源：http://bsz.chenjidiqi.icu

按语言统计（条）：
来源：http://ojy.zhiwuduotai.top

Python ......... 252
来源：http://yja.cheryme.top

PHP ............ 252
来源：http://zwc.meibo888.top

JavaScript ..... 252
来源：http://rdv.daxiang520.top

TypeScript ..... 212
来源：http://hjy.kuanghao11.cn

Java ........... 212
来源：http://ggj.ehwqpu.com

Go ............. 212
来源：http://anv.tanke756.top

Ruby ........... 212
来源：http://pkx.jinqigufen.top

C# ............. 212
来源：http://agu.jinyuanbaomall.cn

C .............. 30
来源：http://qvv.zhongyouzk.top

C++ ............ 30
来源：http://jto.shanyushiyangtech.top

SQL ............ 90
来源：http://skj.vqdsnc.cn

Bash ........... 80
来源：http://vbh.ctjpmb.com

Kotlin ......... 15
来源：http://ens.cucudq.cn

Swift .......... 15
来源：http://cno.sxryk.cn

Lua ............ 10
来源：http://yau.c1oappe.top

Perl ........... 10
来源：http://ouk.wangshuangyany.cn

Scala .......... 10
来源：http://ykx.yj20258.top

------------------------------------
来源：http://msi.yj202588.top

合计 ........... 2106 条
来源：http://mku.sjlbkw.cn

按章节统计：
来源：http://wmp.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bsi.chenjidiqi.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wjp.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ezm.gotoacloud.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://eht.shanyushiyangkeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lyt.ehwqpu.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://unj.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xin.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oqa.hysaishi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nuw.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qvt.nwbrower.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qef.meibo888.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hsx.epnwcf.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fnl.sweek.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://umu.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zii.hcnkem.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://abc.kuanghao11.cn

Q SQL 专题                              90
来源：http://hga.hnqzz.top

R Bash 专题                             80
来源：http://wof.nwbrower.top

S C / C++ 专题                          60
来源：http://der.pengpengdd.cyou

T 其他语言补充                          60
来源：http://mrf.xuetiantiany.cn


<!-- 参考信息 -->