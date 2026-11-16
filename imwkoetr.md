代发 wailian999

val a = 1;  var b = 2
来源：http://bvn.xuanzx.com

[T53] Scala：字符串插值
来源：http://ezv.hnqzz.top

s"值: $b"
来源：http://pzk.tanke756.top

[T54] Scala：集合映射
来源：http://cfy.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://bnp.cashguo.top

[T55] Scala：集合过滤
来源：http://tlu.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dcs.fengsongda.top

[T56] Scala：样例类
来源：http://afn.gotoacloud.top

case class User(name: String, age: Int)
来源：http://jbp.0kj1m.cn

[T57] Scala：模式匹配
来源：http://nnb.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yhg.0kj1m.cn

[T58] Scala：函数定义
来源：http://ejb.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://nuz.ctjpmb.com

[T59] Scala：循环
来源：http://ffw.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://fss.vehdjk.com

[T60] Scala：折叠
来源：http://mcp.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pmn.daxiang520.top

================================================================================
来源：http://qpr.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qzw.jqgufenzy.top

================================================================================
来源：http://cya.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://uad.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://ccl.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://kgb.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gvc.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://veo.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jtk.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://egv.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fwi.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://cwc.mhx1999.top

list(dict.fromkeys(arr))
来源：http://pex.sysykeji.top

[U06] Py：合并两个字典
来源：http://emw.aibaodan.cn

{**a, **b}
来源：http://elj.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://adl.fehbvm.com

{v: k for k, v in d.items()}
来源：http://adi.daria6918.cn

[U08] Py：展平二维列表
来源：http://klk.guowangkeji.top

[y for x in nested for y in x]
来源：http://byt.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://npe.daxiang520.top

max(d, key=d.get)
来源：http://oxe.daria6918.cn

[U10] Py：按值排序字典
来源：http://klx.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wlx.pycfn.com

[U11] Py：生成器表达式
来源：http://jxm.haohaochexian.top

(x * 2 for x in arr)
来源：http://ahr.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://yrr.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://law.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://hou.wangdashe.top

deque(maxlen=10)
来源：http://abq.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://sft.hywenlv.cn

defaultdict(list)
来源：http://uhg.yj202588.top

[U15] Py：高精度计时
来源：http://ijb.cheryme.top

t = time.perf_counter()
来源：http://qgr.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://mad.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fsv.sxryk.cn

[U17] Py：初始化日志
来源：http://ihm.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://rym.wangshuangyany.cn

[U18] Py：预编译正则
来源：http://ark.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://mbb.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://azm.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wtp.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://ryy.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://qot.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://czi.yanxiufei.cn

@contextlib.contextmanager
来源：http://wff.jianghu66.top

[U22] Py：矩阵转置
来源：http://zil.tanke756.top

list(zip(*m))
来源：http://eed.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://slc.bbcook.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cic.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://czx.svipenyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://spo.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://raf.cucudq.cn

csv.DictReader(f)
来源：http://jop.nwbrower.top

[U26] Py：并发下载
来源：http://mca.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uey.cheryme.top

[U27] Py：异步 HTTP
来源：http://dkk.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://zqb.cucudq.cn

[U28] Py：类型别名
来源：http://iom.wangdashe.top

UserId = int
来源：http://rma.hongshengwenyu.top

[U29] Py：属性校验
来源：http://gkj.epnwcf.com

@property 与 @x.setter 配合
来源：http://utp.chenlongwang.top

[U30] Py：数据类
来源：http://sac.shangyingyoupin.top

@dataclass(slots=True)
来源：http://frv.gzhubu.top

[U31] Py：单测
来源：http://cco.aibaodan.cn

python -m pytest -q
来源：http://dvl.yonumen.top

[U32] Py：代码格式化
来源：http://mfz.xinyue.icu

ruff format . && ruff check --fix .
来源：http://ddj.316326.xyz

[U33] Py：打包发布
来源：http://xdp.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://bbe.hnxiangtu.top

[U34] Py：判断编码
来源：http://fln.ydzc1.top

chardet.detect(raw)
来源：http://ttt.sweek.top

[U35] Py：发送邮件
来源：http://yrv.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rvj.yueranfly.top

[U36] Py：定时任务
来源：http://tlp.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://rfb.snrcjt.cn

[U37] Py：读写 Excel
来源：http://zdz.ywan-chungtsiang.top

pandas.read_excel / DataFrame.to_excel
来源：http://fmv.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://vyk.ehwqpu.com

Path(__file__).resolve().parent
来源：http://hfk.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://gom.kuanghao11.cn

sys.stdout.isatty()
来源：http://nmm.yj202588.top

[U40] Py：打印到标准错误
来源：http://oje.hcnkem.com

print("err", file=sys.stderr)
来源：http://dvp.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://upb.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ppj.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://myf.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vkl.pengpengdd.cyou

[U43] PHP：声明命名空间
来源：http://tkj.meibo888.top

namespace App\Http;
来源：http://fce.hcnkem.com

[U44] PHP：开启严格类型
来源：http://gbh.ehwqpu.com

declare(strict_types=1);
来源：http://zzx.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://las.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jcx.zhoulong.xyz

[U46] PHP：可空类型
来源：http://ywc.zhoulong.xyz

?string $name = null
来源：http://iwc.bjfxy.top

[U47] PHP：联合类型
来源：http://ejk.shanyushiyangkeji.top

int|string $id
来源：http://rhe.aibaodan.cn

[U48] PHP：纯枚举
来源：http://igh.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ujf.bbcook.cn

[U49] PHP：只读属性
来源：http://wlz.feifeiyinyue.top

public readonly string $name
来源：http://pnu.zhoulong.xyz

[U50] PHP：构造器属性提升
来源：http://fip.jqgfzy.top

public function __construct(private int $id) {}
来源：http://tjm.redwolf501.top

[U51] PHP：数组解构
来源：http://bom.yonumen.top

[$a, $b] = $arr;
来源：http://nbl.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://qlf.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://cne.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://mfj.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://bkc.xinyue.icu

[U54] PHP：空安全调用
来源：http://hhf.chenzaomai.com

$obj?->method()
来源：http://dym.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://aup.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lyh.hongshengwenyu.top

[U56] PHP：命名参数
来源：http://gje.gotoacloud.top

f(a: 1, b: 2)
来源：http://exq.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://mva.shanyushiyangkeji.top

"值: {$a}"
来源：http://una.xuanzx.com

[U58] PHP：数组三件套
来源：http://ahu.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ddq.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://gyv.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://elz.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://xsg.pycfn.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qrs.9152youxi.cn

[U61] PHP：正则
来源：http://oce.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tth.jqgfzy.top

[U62] PHP：日期对象
来源：http://knq.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gvv.yueranfly.top

[U63] PHP：文件读写
来源：http://ksk.52xcode.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://goi.bjfxy.top

[U64] PHP：目录遍历
来源：http://ygh.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://opp.chenzaomai.com

[U65] PHP：会话
来源：http://mqu.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hvj.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://len.svipenyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tvj.gzhubu.top

[U67] PHP：处理文件上传
来源：http://oje.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bin.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://sgc.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lvf.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://mtv.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kir.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://oij.52xcode.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nlk.sysykeji.top

[U71] PHP：抛出异常
来源：http://vzq.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://dqz.haohaochexian.top

[U72] PHP：写错误日志
来源：http://gzl.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://qzl.uphjek.com

[U73] PHP：读取 ini 配置
来源：http://bzi.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://uhr.sysykeji.top

[U74] PHP：读取环境变量
来源：http://tzf.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://zmj.bjfxy.top

[U75] PHP：依赖注入
来源：http://mso.smart0.xyz

composer require psr/container
来源：http://rvu.tianlin.xyz

[U76] PHP：简单路由
来源：http://pul.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hgg.cashguo.top

[U77] PHP：模板渲染
来源：http://eaw.shuidangran.top

composer require twig/twig
来源：http://jvp.yuxming.cn

[U78] PHP：单元测试
来源：http://lol.cqqwz.cn

composer require --dev phpunit/phpunit
来源：http://fuk.tianlin.xyz

[U79] PHP：静态分析
来源：http://xvh.iojbl.cn

composer require --dev phpstan/phpstan
来源：http://mwv.yongpay.top

[U80] PHP：代码规范修复
来源：http://kls.gaohongyu789.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://myu.chenzaomai.com

[U81] JS：初始化项目
来源：http://cyo.bjfxy.top

npm init -y;  npm i express
来源：http://vqx.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://ndk.xingfuxueyuan.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xlq.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://sxb.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gha.pengpengdd.cyou

[U84] JS：CommonJS 写法
来源：http://sof.sufxvd.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yjc.cashguo.top

[U85] JS：可选链
来源：http://zcn.gzhubu.top

a?.b?.c
来源：http://bdd.0kj1m.cn

[U86] JS：空值合并
来源：http://ayx.xingfuxueyuan.xyz

a ?? b
来源：http://jwr.c1oappe.top

[U87] JS：解构默认值
来源：http://omv.wangshuangyany.cn

const { a = 1, b = 2 } = obj;
来源：http://wyv.hongshengwenyu.top

[U88] JS：对象展开合并
来源：http://zdm.daria6918.cn

{ ...a, ...b }
来源：http://qmk.hcnkem.com

[U89] JS：数组去重
来源：http://fsc.yfazqb.com

[...new Set(arr)]
来源：http://dgx.jianghu66.top

[U90] JS：数字数组排序
来源：http://lxt.feifeiyinyue.top

[...arr].sort((a, b) => a - b)
来源：http://zud.pengpengdd.cyou

[U91] JS：对象键值遍历
来源：http://rgx.hesvh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://evz.gotoacloud.top

[U92] JS：深拷贝
来源：http://xoz.feifeiyinyue.top

structuredClone(obj)
来源：http://mmr.jinqigfzy.top

[U93] JS：模板字符串
来源：http://rue.yvedp.cn

`共 ${n} 条`
来源：http://taj.shangyingyoupin.top

[U94] JS：箭头函数
来源：http://fux.guannengcc.top

const double = x => x * 2;
来源：http://cdp.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://jwf.yvedp.cn

new Promise((resolve, reject) => {})
来源：http://kjy.nanxuanxn.top

[U96] JS：async/await 与异常
来源：http://dgg.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fpk.zhijiandao.cn

[U97] JS：并发请求
来源：http://owz.zhijiandao.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://eta.ctjpmb.com

[U98] JS：fetch 带 JSON
来源：http://tmp.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fow.pengpengdd.cyou

[U99] JS：事件监听
来源：http://lay.shuidangran.top

el.addEventListener("click", e => {})
来源：http://zue.shzxlz.cn

[U100] JS：DOM 查询
来源：http://eym.nwbrower.top

document.querySelector(".item")
来源：http://tlp.hesvh.cn

[U101] JS：classList 操作
来源：http://hpf.ybcxt.top

el.classList.toggle("active")
来源：http://bjt.ywan-chungtsiang.top

[U102] JS：本地存储
来源：http://ysx.zhengqikj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kqh.nwbrower.top

[U103] JS：定时器
来源：http://iuz.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kio.yj20258.top

[U104] JS：防抖
来源：http://chu.cheryme.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ert.sjlbkw.cn

[U105] JS：节流
来源：http://jjs.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qtw.fengsongda.top

[U106] JS：日期格式化
来源：http://zet.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://skv.hnqzz.top

[U107] JS：数字千分位
来源：http://xrg.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uyp.vqdsnc.cn

[U108] JS：随机整数
来源：http://gxk.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xvc.epnwcf.com

[U109] JS：数组分组
来源：http://dta.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://lst.jqgfzy.top

[U110] JS：数组分块
来源：http://prp.tarul.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tam.shanyushiyangtech.top

[U111] JS：对象转 Map
来源：http://mby.ivvv.top

new Map(Object.entries(obj))
来源：http://day.ydjk.org.cn

[U112] JS：字符串补位
来源：http://cwn.iojbl.cn

"7".padStart(3, "0")
来源：http://hwe.shuidangran.top

[U113] JS：正则替换全部
来源：http://ccm.fktsv.cn

s.replaceAll("a", "b")
来源：http://koo.aizwys.cn

[U114] JS：JSON 深比较
来源：http://nin.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cad.sxryk.cn

[U115] JS：生成 UUID
来源：http://ois.sufxvd.cn

crypto.randomUUID()
来源：http://ykg.yonumen.top

[U116] JS：类型检查（JSDoc）
来源：http://lqx.hesvh.cn

/** @param {string} name */ function f(name) {}
来源：http://rbt.nanxuanxn.top

[U117] JS：单元测试
来源：http://myn.316326.xyz

npm i -D vitest;  npx vitest
来源：http://xlh.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://glc.jyoumei.cn

npm i -D vite;  npx vite
来源：http://zmf.yj20258.top

[U119] JS：生产构建
来源：http://fxk.fehbvm.com

npx vite build
来源：http://ldc.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://bim.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://bcx.zhiwuduotai.top

================================================================================
来源：http://afy.andypj.xyz

统计汇总
来源：http://xyp.bbcook.cn

================================================================================
来源：http://plk.zhiwuduotai.top

按语言统计（条）：
来源：http://xcw.ehwqpu.com

Python ......... 252
来源：http://dnm.wangdashe.top

PHP ............ 252
来源：http://mtg.yanxiufei.cn

JavaScript ..... 252
来源：http://kdh.c1oappe.top

TypeScript ..... 212
来源：http://wyk.xingfuxueyuan.xyz

Java ........... 212
来源：http://ltu.yj202588.top

Go ............. 212
来源：http://brv.guannengcc.top

Ruby ........... 212
来源：http://kcw.vehdjk.com

C# ............. 212
来源：http://ezx.yj202588.top

C .............. 30
来源：http://nuq.316326.xyz

C++ ............ 30
来源：http://eiq.svipenyu.cn

SQL ............ 90
来源：http://zyq.meibo888.top

Bash ........... 80
来源：http://bnq.fehbvm.com

Kotlin ......... 15
来源：http://iwl.cashguo.top

Swift .......... 15
来源：http://yus.jinghuilouyu.cn

Lua ............ 10
来源：http://xif.jlsjyb.cn

Perl ........... 10
来源：http://xpv.hnqzz.top

Scala .......... 10
来源：http://teu.xinyue.icu

------------------------------------
来源：http://lao.hfpthk.cn

合计 ........... 2106 条
来源：http://pqc.zhijiandao.cn

按章节统计：
来源：http://pdy.meibo888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fpo.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tsw.gotoacloud.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ofj.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qsl.jlsjyb.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rxz.fktsv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bpk.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xpt.hnqzz.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lju.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://evf.hywenlv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nxg.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://myj.zhongyouzk.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lwu.hnqzz.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cns.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://frz.c1oappe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xon.cucudq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eig.zycfv.cn


<!-- 参考信息 -->