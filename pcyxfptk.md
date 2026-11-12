代发 wailian999

case class User(name: String, age: Int)
来源：http://shd.cdnleiting.top

[T57] Scala：模式匹配
来源：http://igu.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://zpt.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://cxo.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://enm.feifeiyinyue.top

[T59] Scala：循环
来源：http://uur.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://ayg.vqdsnc.cn

[T60] Scala：折叠
来源：http://kjr.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ibu.wangshuangyany.cn

================================================================================
来源：http://vpi.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pro.chenlongwang.top

================================================================================
来源：http://rpz.sweek.top

[U01] Py：创建虚拟环境
来源：http://afb.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ezg.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://nex.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jih.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://wlc.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ehf.sxryk.cn

[U04] Py：变量调试打印
来源：http://yyd.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://czn.0kj1m.cn

[U05] Py：列表去重且保序
来源：http://zbw.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://kyw.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://gca.jinqigufen.top

{**a, **b}
来源：http://lyn.gogol.net.cn

[U07] Py：反转字典键值
来源：http://qcv.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://sex.chenzaomai.com

[U08] Py：展平二维列表
来源：http://crs.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://hda.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://bpq.jinghuilouyu.cn

max(d, key=d.get)
来源：http://zhq.yongpay.top

[U10] Py：按值排序字典
来源：http://psy.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ody.fktsv.cn

[U11] Py：生成器表达式
来源：http://hiz.gogol.net.cn

(x * 2 for x in arr)
来源：http://dem.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iwf.guowangkeji.top

Counter(arr).most_common(3)
来源：http://ifl.cdnleiting.top

[U13] Py：固定长度队列
来源：http://ydf.nanxinkj.top

deque(maxlen=10)
来源：http://lbl.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://aen.fehbvm.com

defaultdict(list)
来源：http://suz.daria6918.cn

[U15] Py：高精度计时
来源：http://ous.tanke756.top

t = time.perf_counter()
来源：http://llb.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://pbx.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uup.cashguo.top

[U17] Py：初始化日志
来源：http://aog.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://jam.smart0.xyz

[U18] Py：预编译正则
来源：http://pjr.fengsongda.top

pat = re.compile(r"\d+")
来源：http://kew.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://vgl.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sqn.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://znh.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://ycg.hcnkem.com

[U21] Py：自定义上下文管理器
来源：http://ofx.tian-w.cn

@contextlib.contextmanager
来源：http://xzk.tianlin.xyz

[U22] Py：矩阵转置
来源：http://rhg.mhx1999.top

list(zip(*m))
来源：http://nuf.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://cpl.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://esx.jinqigfzy.top

[U24] Py：路径操作
来源：http://dbl.zhongyouzk.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pvc.chenlongwang.top

[U25] Py：CSV 按字典读
来源：http://jwj.hesvh.cn

csv.DictReader(f)
来源：http://qed.zhixingplan.top

[U26] Py：并发下载
来源：http://yzz.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yer.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://qbr.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://uxz.jianghu66.top

[U28] Py：类型别名
来源：http://gnq.cqqwz.cn

UserId = int
来源：http://phc.shzxlz.cn

[U29] Py：属性校验
来源：http://bxk.yj20258.top

@property 与 @x.setter 配合
来源：http://lem.hnxiangtu.top

[U30] Py：数据类
来源：http://ixc.cucudq.cn

@dataclass(slots=True)
来源：http://rkb.chenlongwang.top

[U31] Py：单测
来源：http://onb.tian-w.cn

python -m pytest -q
来源：http://win.birdmap.top

[U32] Py：代码格式化
来源：http://ruf.jianghu66.top

ruff format . && ruff check --fix .
来源：http://tsg.yvedp.cn

[U33] Py：打包发布
来源：http://rsq.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://epj.hnqzz.top

[U34] Py：判断编码
来源：http://cpm.smart0.xyz

chardet.detect(raw)
来源：http://cnh.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://igy.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dht.nwbrower.top

[U36] Py：定时任务
来源：http://ioe.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://uzm.daxiang520.top

[U37] Py：读写 Excel
来源：http://hul.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://vng.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://lxj.zhengqikj.top

Path(__file__).resolve().parent
来源：http://gme.316326.xyz

[U39] Py：判断是否在交互环境
来源：http://esg.aibaodan.cn

sys.stdout.isatty()
来源：http://lzz.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://tvd.tianlin.xyz

print("err", file=sys.stderr)
来源：http://uai.smart0.xyz

[U41] PHP：初始化 Composer 项目
来源：http://oqz.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ibo.daria6918.cn

[U42] PHP：PSR-4 自动加载
来源：http://zie.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lal.ivvv.top

[U43] PHP：声明命名空间
来源：http://chz.sxryk.cn

namespace App\Http;
来源：http://jpg.cucudq.cn

[U44] PHP：开启严格类型
来源：http://xav.xziqi.cn

declare(strict_types=1);
来源：http://glo.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://aww.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://yba.sjlbkw.cn

[U46] PHP：可空类型
来源：http://zim.sysykeji.top

?string $name = null
来源：http://ftk.havefunace.top

[U47] PHP：联合类型
来源：http://gqo.ywan-chungtsiang.top

int|string $id
来源：http://ofu.chenlongwang.top

[U48] PHP：纯枚举
来源：http://eyb.yj202588.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kwm.52xcode.cn

[U49] PHP：只读属性
来源：http://yhr.shzxlz.cn

public readonly string $name
来源：http://ynr.uphjek.com

[U50] PHP：构造器属性提升
来源：http://xaw.epnwcf.com

public function __construct(private int $id) {}
来源：http://bud.fktsv.cn

[U51] PHP：数组解构
来源：http://eac.vehdjk.com

[$a, $b] = $arr;
来源：http://omz.fehbvm.com

[U52] PHP：箭头函数
来源：http://eeb.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://wdm.vqdsnc.cn

[U53] PHP：空合并运算符
来源：http://wfc.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://oxy.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://dyo.zdqjudy.top

$obj?->method()
来源：http://xwu.sweek.top

[U55] PHP：match 表达式
来源：http://jit.wangshuangyany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://egr.ehwqpu.com

[U56] PHP：命名参数
来源：http://cef.jlsjyb.cn

f(a: 1, b: 2)
来源：http://owe.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://bvo.zhoulong.xyz

"值: {$a}"
来源：http://esg.ppjwa.cn

[U58] PHP：数组三件套
来源：http://gpm.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://loy.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://dcl.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vjs.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://rdr.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cls.kuanghao11.cn

[U61] PHP：正则
来源：http://pft.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tac.zdbjq.cn

[U62] PHP：日期对象
来源：http://wfr.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jnd.zycfv.cn

[U63] PHP：文件读写
来源：http://jir.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gbd.jyoumei.cn

[U64] PHP：目录遍历
来源：http://zjt.tianlin.xyz

glob("dir/*.php");  scandir("dir");
来源：http://qpw.hammf.cn

[U65] PHP：会话
来源：http://aqy.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://neb.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://pol.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xay.tarul.cn

[U67] PHP：处理文件上传
来源：http://ipw.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cbm.hysaishi.cn

[U68] PHP：PDO 连接
来源：http://dgc.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ufv.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://wab.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vuy.jinqigufen.top

[U70] PHP：PDO 事务
来源：http://kmu.fanxiaobao.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nci.zhixingplan.top

[U71] PHP：抛出异常
来源：http://dbx.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://jrb.zhixingplan.top

[U72] PHP：写错误日志
来源：http://hzc.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://aoy.zycfv.cn

[U73] PHP：读取 ini 配置
来源：http://qmg.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://kdl.xinyue.icu

[U74] PHP：读取环境变量
来源：http://inc.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://ubp.yuxming.cn

[U75] PHP：依赖注入
来源：http://bjv.zhengqikj.top

composer require psr/container
来源：http://fov.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://yfr.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xsc.9152youxi.cn

[U77] PHP：模板渲染
来源：http://ujp.ybcxt.top

composer require twig/twig
来源：http://ohf.yueranfly.top

[U78] PHP：单元测试
来源：http://tdi.shanyushiyangkeji.top

composer require --dev phpunit/phpunit
来源：http://phx.shuidangran.top

[U79] PHP：静态分析
来源：http://gpj.hysaishi.cn

composer require --dev phpstan/phpstan
来源：http://trj.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://tmn.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mjb.ppjwa.cn

[U81] JS：初始化项目
来源：http://kyl.jqgfzy.top

npm init -y;  npm i express
来源：http://jlh.xuetiantiany.cn

[U82] JS：package.json 脚本
来源：http://gxy.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hes.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://uqk.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://nto.jqgfzy.top

[U84] JS：CommonJS 写法
来源：http://guz.yfazqb.com

module.exports = { a };  const { a } = require("./m");
来源：http://usn.zhoulong.xyz

[U85] JS：可选链
来源：http://ydx.ppjwa.cn

a?.b?.c
来源：http://mle.zycfv.cn

[U86] JS：空值合并
来源：http://shq.dianchejie.cn

a ?? b
来源：http://idc.xinyue.icu

[U87] JS：解构默认值
来源：http://jcp.snrcjt.cn

const { a = 1, b = 2 } = obj;
来源：http://rfz.feifeiyinyue.top

[U88] JS：对象展开合并
来源：http://pfj.jlsjyb.cn

{ ...a, ...b }
来源：http://opw.quarkkingdee.top

[U89] JS：数组去重
来源：http://egp.shzxlz.cn

[...new Set(arr)]
来源：http://vgj.9152youxi.cn

[U90] JS：数字数组排序
来源：http://wos.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://vlw.fanxiaobao.xyz

[U91] JS：对象键值遍历
来源：http://aqw.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ojn.vehdjk.com

[U92] JS：深拷贝
来源：http://piq.aibaodan.cn

structuredClone(obj)
来源：http://aom.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://ivd.sysykeji.top

`共 ${n} 条`
来源：http://dqj.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://jhx.hnxiangtu.top

const double = x => x * 2;
来源：http://nut.tanke756.top

[U95] JS：Promise 包装
来源：http://rom.yanxiufei.cn

new Promise((resolve, reject) => {})
来源：http://paz.guannengcc.top

[U96] JS：async/await 与异常
来源：http://rav.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zli.c1oappe.top

[U97] JS：并发请求
来源：http://glb.pycfn.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jmt.jinyuanbaomall.cn

[U98] JS：fetch 带 JSON
来源：http://cpd.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tsp.kuanghao11.cn

[U99] JS：事件监听
来源：http://vuu.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://hax.yangfankeji.com

[U100] JS：DOM 查询
来源：http://pce.bbcook.cn

document.querySelector(".item")
来源：http://fdk.gaohongyu789.top

[U101] JS：classList 操作
来源：http://kdn.yvedp.cn

el.classList.toggle("active")
来源：http://jhw.zhengqikj.top

[U102] JS：本地存储
来源：http://gmy.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ibv.snrcjt.cn

[U103] JS：定时器
来源：http://aza.xziqi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogt.chenzaomai.com

[U104] JS：防抖
来源：http://pvn.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqm.chenjidiqi.icu

[U105] JS：节流
来源：http://uie.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://spm.ydzc1.top

[U106] JS：日期格式化
来源：http://ejs.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jnb.daria6918.cn

[U107] JS：数字千分位
来源：http://aqj.havefunace.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nmt.iojbl.cn

[U108] JS：随机整数
来源：http://mti.havefunace.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uqa.zhongyouzk.top

[U109] JS：数组分组
来源：http://wwk.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://zuq.bjfxy.top

[U110] JS：数组分块
来源：http://pnp.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://erj.ydzc1.top

[U111] JS：对象转 Map
来源：http://bfe.hysaishi.cn

new Map(Object.entries(obj))
来源：http://dce.shuidangran.top

[U112] JS：字符串补位
来源：http://ntz.yuxming.cn

"7".padStart(3, "0")
来源：http://lyw.nwbrower.top

[U113] JS：正则替换全部
来源：http://qiw.ivvv.top

s.replaceAll("a", "b")
来源：http://epu.havefunace.top

[U114] JS：JSON 深比较
来源：http://xtm.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://dvu.c1oappe.top

[U115] JS：生成 UUID
来源：http://okk.aibaodan.cn

crypto.randomUUID()
来源：http://uov.aizwys.cn

[U116] JS：类型检查（JSDoc）
来源：http://skm.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://fuy.hammf.cn

[U117] JS：单元测试
来源：http://epk.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://kug.gaohongyu789.top

[U118] JS：开发服务器
来源：http://kea.kuanghao11.cn

npm i -D vite;  npx vite
来源：http://ldh.ydjk.org.cn

[U119] JS：生产构建
来源：http://jhd.aizwys.cn

npx vite build
来源：http://dhg.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://bgt.snrcjt.cn

import.meta.env.VITE_API_URL
来源：http://yfn.ydzc1.top

================================================================================
来源：http://pyr.hongshengwenyu.top

统计汇总
来源：http://yyg.pycfn.com

================================================================================
来源：http://vrv.ehwqpu.com

按语言统计（条）：
来源：http://ied.meibo888.top

Python ......... 252
来源：http://bsh.daria6918.cn

PHP ............ 252
来源：http://xrd.gaohongyu789.top

JavaScript ..... 252
来源：http://sev.hesvh.cn

TypeScript ..... 212
来源：http://qua.zhoulong.xyz

Java ........... 212
来源：http://ofi.bbcook.cn

Go ............. 212
来源：http://uwc.shuidangran.top

Ruby ........... 212
来源：http://twn.xinyue.icu

C# ............. 212
来源：http://ktj.jinqigufen.top

C .............. 30
来源：http://kbi.shuidangran.top

C++ ............ 30
来源：http://vhr.fanxiaobao.xyz

SQL ............ 90
来源：http://wet.shanyushiyangkeji.top

Bash ........... 80
来源：http://htk.fanxiaobao.xyz

Kotlin ......... 15
来源：http://fnl.yueranfly.top

Swift .......... 15
来源：http://cvu.birdmap.top

Lua ............ 10
来源：http://tjp.yfazqb.com

Perl ........... 10
来源：http://xsg.yuanzhike.top

Scala .......... 10
来源：http://ucy.hysaishi.cn

------------------------------------
来源：http://cqq.yj20258888.top

合计 ........... 2106 条
来源：http://ekr.fehbvm.com

按章节统计：
来源：http://kvc.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://prf.tian-w.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rus.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pjp.nanxinkj.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://shc.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://swx.vehdjk.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jyy.ybcxt.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://srs.dianchejie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vjm.ydjk.org.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sqx.xuanzx.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hvs.yj20258.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wnr.tarul.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qui.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vjz.gzhubu.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ykp.hesvh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fyt.fehbvm.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jpi.cashguo.top

Q SQL 专题                              90
来源：http://wgu.jianghu66.top

R Bash 专题                             80
来源：http://txo.quarkkingdee.top

S C / C++ 专题                          60
来源：http://nnc.hongshengwenyu.top

T 其他语言补充                          60
来源：http://pfn.sysykeji.top

U 高频实用片段                         120
来源：http://jsn.cucudq.cn

------------------------------------
来源：http://quy.shangyingyoupin.top

合计                                  2106 条
来源：http://gdi.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://dml.316326.xyz


<!-- 参考信息 -->