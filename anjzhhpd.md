代发 wailian999

val a = 1;  var b = 2
来源：http://clw.bbcook.cn

[T53] Scala：字符串插值
来源：http://szn.nanxinkj.top

s"值: $b"
来源：http://did.dianchejie.cn

[T54] Scala：集合映射
来源：http://sud.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://eac.sysykeji.top

[T55] Scala：集合过滤
来源：http://opg.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://sfx.guowangkeji.top

[T56] Scala：样例类
来源：http://dyx.jianghu66.top

case class User(name: String, age: Int)
来源：http://oax.zdqjudy.top

[T57] Scala：模式匹配
来源：http://uzw.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wvw.sweek.top

[T58] Scala：函数定义
来源：http://kad.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://pby.jianghu66.top

[T59] Scala：循环
来源：http://gai.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://rrk.daria6918.cn

[T60] Scala：折叠
来源：http://fmg.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rez.iojbl.cn

================================================================================
来源：http://dqd.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rvc.fzhhl.top

================================================================================
来源：http://bjs.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://ypj.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pjo.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://snh.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dwh.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://aqt.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://goh.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://ojx.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dow.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://onp.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://hbm.dashuyun.cn

[U06] Py：合并两个字典
来源：http://pem.gotoacloud.top

{**a, **b}
来源：http://xyz.fehbvm.com

[U07] Py：反转字典键值
来源：http://umr.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://fnv.tian-w.cn

[U08] Py：展平二维列表
来源：http://bfq.smart0.xyz

[y for x in nested for y in x]
来源：http://drj.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://krr.aizwys.cn

max(d, key=d.get)
来源：http://zml.pycfn.com

[U10] Py：按值排序字典
来源：http://uxy.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://boe.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://wlu.redwolf501.top

(x * 2 for x in arr)
来源：http://mlw.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://eoy.xuanzx.com

Counter(arr).most_common(3)
来源：http://jop.9152youxi.cn

[U13] Py：固定长度队列
来源：http://vhq.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://oqj.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://pps.fengsongda.top

defaultdict(list)
来源：http://ibc.ehwqpu.com

[U15] Py：高精度计时
来源：http://voa.chenjidiqi.icu

t = time.perf_counter()
来源：http://wgd.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://qyh.cashguo.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fmb.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://ufm.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://uaw.cdnleiting.top

[U18] Py：预编译正则
来源：http://cbt.hammf.cn

pat = re.compile(r"\d+")
来源：http://eet.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://yjl.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eno.cqqwz.cn

[U20] Py：缓存函数结果
来源：http://emj.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://mma.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://jrv.dianchejie.cn

@contextlib.contextmanager
来源：http://vuf.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://ynu.gotoacloud.top

list(zip(*m))
来源：http://csd.zhijiandao.cn

[U23] Py：分块读取大文件
来源：http://lox.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jgj.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://lwk.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bty.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://trc.yangfankeji.com

csv.DictReader(f)
来源：http://cgt.fzhhl.top

[U26] Py：并发下载
来源：http://tde.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gva.hammf.cn

[U27] Py：异步 HTTP
来源：http://xsr.mhx1999.top

aiohttp.ClientSession() 配合 async with
来源：http://mzd.aibaodan.cn

[U28] Py：类型别名
来源：http://chd.vehdjk.com

UserId = int
来源：http://sdz.hysaishi.cn

[U29] Py：属性校验
来源：http://woe.hesvh.cn

@property 与 @x.setter 配合
来源：http://gge.yueranfly.top

[U30] Py：数据类
来源：http://azq.haohaochexian.top

@dataclass(slots=True)
来源：http://tkb.quarkkingdee.top

[U31] Py：单测
来源：http://gid.xingfuxueyuan.xyz

python -m pytest -q
来源：http://rjh.jianghu66.top

[U32] Py：代码格式化
来源：http://ybm.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://ehq.epnwcf.com

[U33] Py：打包发布
来源：http://ift.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://vbr.chenjidiqi.icu

[U34] Py：判断编码
来源：http://pqe.yj20258.top

chardet.detect(raw)
来源：http://zdw.dianchejie.cn

[U35] Py：发送邮件
来源：http://jai.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jbs.fzhhl.top

[U36] Py：定时任务
来源：http://jko.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://hjd.ybcxt.top

[U37] Py：读写 Excel
来源：http://pff.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ser.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://clw.ydzc1.top

Path(__file__).resolve().parent
来源：http://zki.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://bhx.xinyue.icu

sys.stdout.isatty()
来源：http://fko.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://byj.yongpay.top

print("err", file=sys.stderr)
来源：http://rgf.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://rdf.sweek.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wlp.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://xgs.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://aue.zycfv.cn

[U43] PHP：声明命名空间
来源：http://bmo.zycfv.cn

namespace App\Http;
来源：http://qgk.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://atn.havefunace.top

declare(strict_types=1);
来源：http://ccv.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://xmz.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tkn.mhx1999.top

[U46] PHP：可空类型
来源：http://ymv.snrcjt.cn

?string $name = null
来源：http://iyg.aibaodan.cn

[U47] PHP：联合类型
来源：http://jqx.zhijiandao.cn

int|string $id
来源：http://zpn.chenlongwang.top

[U48] PHP：纯枚举
来源：http://gut.mhx1999.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gbq.epnwcf.com

[U49] PHP：只读属性
来源：http://yqh.chenlongwang.top

public readonly string $name
来源：http://ret.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://bux.tianlin.xyz

public function __construct(private int $id) {}
来源：http://nlp.yongpay.top

[U51] PHP：数组解构
来源：http://dss.ydzc1.top

[$a, $b] = $arr;
来源：http://ggy.xuetiantiany.cn

[U52] PHP：箭头函数
来源：http://pcp.shuidangran.top

$double = fn($x) => $x * 2;
来源：http://zvv.ctjpmb.com

[U53] PHP：空合并运算符
来源：http://cii.fengsongda.top

$v = $a ?? $b ?? "default";
来源：http://jdx.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://pbr.nwbrower.top

$obj?->method()
来源：http://dvc.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://msf.zhiwuduotai.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://umo.hammf.cn

[U56] PHP：命名参数
来源：http://oae.nanxuanxn.top

f(a: 1, b: 2)
来源：http://jzr.316326.xyz

[U57] PHP：字符串插值
来源：http://sdf.hongshengwenyu.top

"值: {$a}"
来源：http://hko.dianchejie.cn

[U58] PHP：数组三件套
来源：http://ofv.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fup.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://oze.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aoe.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://kub.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kdb.jqgfzy.top

[U61] PHP：正则
来源：http://asq.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ytn.daria6918.cn

[U62] PHP：日期对象
来源：http://chz.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pud.vqdsnc.cn

[U63] PHP：文件读写
来源：http://ifx.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rwu.jqgfzy.top

[U64] PHP：目录遍历
来源：http://asu.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://slc.gogol.net.cn

[U65] PHP：会话
来源：http://yiq.zhijiandao.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kzc.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://xck.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tpb.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://fah.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zul.chenjidiqi.icu

[U68] PHP：PDO 连接
来源：http://utd.yuxming.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kwl.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://jua.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wkv.52xcode.cn

[U70] PHP：PDO 事务
来源：http://oiy.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lkm.fzhhl.top

[U71] PHP：抛出异常
来源：http://ghd.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://ldb.jianghu66.top

[U72] PHP：写错误日志
来源：http://utx.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://upe.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://zsk.jinghuilouyu.cn

parse_ini_file("config.ini", true)
来源：http://wwd.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://hgc.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://idz.snrcjt.cn

[U75] PHP：依赖注入
来源：http://ieh.xingfuxueyuan.xyz

composer require psr/container
来源：http://fdk.hesvh.cn

[U76] PHP：简单路由
来源：http://zhi.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://axb.ppjwa.cn

[U77] PHP：模板渲染
来源：http://cun.9152youxi.cn

composer require twig/twig
来源：http://fte.nwbrower.top

[U78] PHP：单元测试
来源：http://shz.tanke756.top

composer require --dev phpunit/phpunit
来源：http://qjg.quarkkingdee.top

[U79] PHP：静态分析
来源：http://xhu.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://pjd.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://akw.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ofk.redwolf501.top

[U81] JS：初始化项目
来源：http://nql.zhongyouzk.top

npm init -y;  npm i express
来源：http://ewe.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://xxt.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://aro.hongshengwenyu.top

[U83] JS：ES Module 导入导出
来源：http://iso.aizwys.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fwz.quarkkingdee.top

[U84] JS：CommonJS 写法
来源：http://ava.jqgfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://bpx.hnqzz.top

[U85] JS：可选链
来源：http://tei.sjlbkw.cn

a?.b?.c
来源：http://qgc.316326.xyz

[U86] JS：空值合并
来源：http://jus.snrcjt.cn

a ?? b
来源：http://lmc.xuanzx.com

[U87] JS：解构默认值
来源：http://yor.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://osb.hcnkem.com

[U88] JS：对象展开合并
来源：http://wsw.mhx1999.top

{ ...a, ...b }
来源：http://rfb.cheryme.top

[U89] JS：数组去重
来源：http://ecs.guowangkeji.top

[...new Set(arr)]
来源：http://jxy.yj20258.top

[U90] JS：数字数组排序
来源：http://nvs.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://oib.mhx1999.top

[U91] JS：对象键值遍历
来源：http://fas.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://chi.yj202588.top

[U92] JS：深拷贝
来源：http://lcu.fzhhl.top

structuredClone(obj)
来源：http://aae.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://ugm.quarkkingdee.top

`共 ${n} 条`
来源：http://lxe.yuxming.cn

[U94] JS：箭头函数
来源：http://glz.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://jzb.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://bvo.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://tkn.316326.xyz

[U96] JS：async/await 与异常
来源：http://sei.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gpi.mhx1999.top

[U97] JS：并发请求
来源：http://syp.haohaochexian.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://khv.jyoumei.cn

[U98] JS：fetch 带 JSON
来源：http://utq.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fre.hnqzz.top

[U99] JS：事件监听
来源：http://jpg.yfazqb.com

el.addEventListener("click", e => {})
来源：http://qqt.uphjek.com

[U100] JS：DOM 查询
来源：http://ene.ydzc1.top

document.querySelector(".item")
来源：http://nfx.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://sjw.nwbrower.top

el.classList.toggle("active")
来源：http://hwl.shzxlz.cn

[U102] JS：本地存储
来源：http://dum.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ann.316326.xyz

[U103] JS：定时器
来源：http://otj.cqqwz.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qyi.yangfankeji.com

[U104] JS：防抖
来源：http://tqa.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lke.guannengcc.top

[U105] JS：节流
来源：http://alh.ehwqpu.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zls.dianchejie.cn

[U106] JS：日期格式化
来源：http://ruh.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fho.cdnleiting.top

[U107] JS：数字千分位
来源：http://lic.sysykeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jch.sweek.top

[U108] JS：随机整数
来源：http://hnw.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zlk.sweek.top

[U109] JS：数组分组
来源：http://zva.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://ccr.hywenlv.cn

[U110] JS：数组分块
来源：http://cdx.nwbrower.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ayp.zdqjudy.top

[U111] JS：对象转 Map
来源：http://rod.tarul.cn

new Map(Object.entries(obj))
来源：http://gid.ppjwa.cn

[U112] JS：字符串补位
来源：http://vjf.9152youxi.cn

"7".padStart(3, "0")
来源：http://syn.svipenyu.cn

[U113] JS：正则替换全部
来源：http://ypn.ehwqpu.com

s.replaceAll("a", "b")
来源：http://vjv.hnqzz.top

[U114] JS：JSON 深比较
来源：http://rdu.mhx1999.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hst.316326.xyz

[U115] JS：生成 UUID
来源：http://mnl.zdqjudy.top

crypto.randomUUID()
来源：http://wqh.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://pcr.zdbjq.cn

/** @param {string} name */ function f(name) {}
来源：http://xst.tanke756.top

[U117] JS：单元测试
来源：http://ths.zhongyouzk.top

npm i -D vitest;  npx vitest
来源：http://agj.quarkkingdee.top

[U118] JS：开发服务器
来源：http://kxn.jlsjyb.cn

npm i -D vite;  npx vite
来源：http://glw.redwolf501.top

[U119] JS：生产构建
来源：http://cfu.ppjwa.cn

npx vite build
来源：http://tyu.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://tnd.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://ysw.yuxming.cn

================================================================================
来源：http://yqs.jlsjyb.cn

统计汇总
来源：http://xyb.pengpengdd.cyou

================================================================================
来源：http://prc.ybcxt.top

按语言统计（条）：
来源：http://zex.andypj.xyz

Python ......... 252
来源：http://vwi.shuidangran.top

PHP ............ 252
来源：http://uqe.gzhubu.top

JavaScript ..... 252
来源：http://ori.dashuyun.cn

TypeScript ..... 212
来源：http://pfh.meibo888.top

Java ........... 212
来源：http://ahz.zycfv.cn

Go ............. 212
来源：http://yfb.chenlongwang.top

Ruby ........... 212
来源：http://hdt.316326.xyz

C# ............. 212
来源：http://zfa.gotoacloud.top

C .............. 30
来源：http://dug.zhaomingkeji.xyz

C++ ............ 30
来源：http://jtk.zhaomingkeji.xyz

SQL ............ 90
来源：http://tuh.dashuyun.cn

Bash ........... 80
来源：http://tmv.yvedp.cn

Kotlin ......... 15
来源：http://uwz.hnqzz.top

Swift .......... 15
来源：http://oua.hnqzz.top

Lua ............ 10
来源：http://rzt.shuidangran.top

Perl ........... 10
来源：http://dzq.chenjidiqi.icu

Scala .......... 10
来源：http://jol.cashguo.top

------------------------------------
来源：http://yzq.zhijiandao.cn

合计 ........... 2106 条
来源：http://eui.ivvv.top

按章节统计：
来源：http://mpk.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://abw.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kbp.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iie.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ilv.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://evx.aibaodan.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nkd.aizwys.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xoh.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jrt.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tor.tian-w.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://itd.zhongyouzk.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kqz.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lof.tarul.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xwz.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vkk.hfpthk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://usc.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://umm.jlsjyb.cn


<!-- 参考信息 -->