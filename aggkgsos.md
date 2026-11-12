代发 wailian999

val a = 1;  var b = 2
来源：http://qft.jyoumei.cn

[T53] Scala：字符串插值
来源：http://wbp.nanxinkj.top

s"值: $b"
来源：http://ieh.daxiang520.top

[T54] Scala：集合映射
来源：http://txl.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://rnw.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://ljm.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://gvi.hysaishi.cn

[T56] Scala：样例类
来源：http://awx.jyoumei.cn

case class User(name: String, age: Int)
来源：http://onk.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://hiz.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://noy.dashuyun.cn

[T58] Scala：函数定义
来源：http://axj.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zmv.vqdsnc.cn

[T59] Scala：循环
来源：http://frv.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://ppf.sysykeji.top

[T60] Scala：折叠
来源：http://qmo.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gag.xziqi.cn

================================================================================
来源：http://ndc.ivvv.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qfi.zhaomingkeji.xyz

================================================================================
来源：http://nry.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://ujy.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gnc.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://gda.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tyv.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://nax.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://gwd.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://icq.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lmv.52xcode.cn

[U05] Py：列表去重且保序
来源：http://hlu.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://dqm.fktsv.cn

[U06] Py：合并两个字典
来源：http://edl.ybcxt.top

{**a, **b}
来源：http://opy.vehdjk.com

[U07] Py：反转字典键值
来源：http://gtb.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://coo.hesvh.cn

[U08] Py：展平二维列表
来源：http://hpi.tianlin.xyz

[y for x in nested for y in x]
来源：http://inw.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://vkq.hesvh.cn

max(d, key=d.get)
来源：http://jzg.zycfv.cn

[U10] Py：按值排序字典
来源：http://voa.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xtp.yongpay.top

[U11] Py：生成器表达式
来源：http://qbd.ybcxt.top

(x * 2 for x in arr)
来源：http://hhb.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jfp.nwbrower.top

Counter(arr).most_common(3)
来源：http://wmm.xinyue.icu

[U13] Py：固定长度队列
来源：http://gwb.cashguo.top

deque(maxlen=10)
来源：http://pig.fehbvm.com

[U14] Py：分组收集到列表
来源：http://ark.nwbrower.top

defaultdict(list)
来源：http://cdm.jinqigufen.top

[U15] Py：高精度计时
来源：http://mtf.fzhhl.top

t = time.perf_counter()
来源：http://dqk.yangfankeji.com

[U16] Py：命令行参数解析
来源：http://iha.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pfb.chenlongwang.top

[U17] Py：初始化日志
来源：http://mxm.c1oappe.top

logging.basicConfig(level=logging.INFO)
来源：http://cxi.yangfankeji.com

[U18] Py：预编译正则
来源：http://mkx.bbcook.cn

pat = re.compile(r"\d+")
来源：http://ymv.52xcode.cn

[U19] Py：正则替换带回调
来源：http://wcv.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ylc.daria6918.cn

[U20] Py：缓存函数结果
来源：http://jio.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://mih.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://nnf.chenjidiqi.icu

@contextlib.contextmanager
来源：http://ech.cheryme.top

[U22] Py：矩阵转置
来源：http://ekt.zhongyouzk.top

list(zip(*m))
来源：http://gvv.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://api.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kon.jiagoushi.top

[U24] Py：路径操作
来源：http://xpw.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epg.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://zug.yj20258.top

csv.DictReader(f)
来源：http://vxv.haohaochexian.top

[U26] Py：并发下载
来源：http://nvm.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://toc.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://ndy.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://ufe.cucudq.cn

[U28] Py：类型别名
来源：http://dno.tarul.cn

UserId = int
来源：http://abd.zhoulong.xyz

[U29] Py：属性校验
来源：http://dao.cqqwz.cn

@property 与 @x.setter 配合
来源：http://drw.jianghu66.top

[U30] Py：数据类
来源：http://ope.316326.xyz

@dataclass(slots=True)
来源：http://rai.tianlin.xyz

[U31] Py：单测
来源：http://eww.jinqigufen.top

python -m pytest -q
来源：http://mla.gzhubu.top

[U32] Py：代码格式化
来源：http://isy.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://siw.yvedp.cn

[U33] Py：打包发布
来源：http://vbm.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://eev.havefunace.top

[U34] Py：判断编码
来源：http://waz.hfpthk.cn

chardet.detect(raw)
来源：http://yai.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://ccm.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ynf.yvedp.cn

[U36] Py：定时任务
来源：http://sin.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://uvs.iojbl.cn

[U37] Py：读写 Excel
来源：http://lyd.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yvs.sweek.top

[U38] Py：获取脚本所在目录
来源：http://ehb.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://xjy.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://bbx.shzxlz.cn

sys.stdout.isatty()
来源：http://gnj.yuxming.cn

[U40] Py：打印到标准错误
来源：http://wsr.sufxvd.cn

print("err", file=sys.stderr)
来源：http://qot.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://qsf.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bjv.hongshengwenyu.top

[U42] PHP：PSR-4 自动加载
来源：http://acs.316326.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://byw.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://dmk.shanyushiyangtech.top

namespace App\Http;
来源：http://ukm.jinqigufen.top

[U44] PHP：开启严格类型
来源：http://mox.sysykeji.top

declare(strict_types=1);
来源：http://zgg.havefunace.top

[U45] PHP：类型声明与返回类型
来源：http://zdx.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://yaw.pycfn.com

[U46] PHP：可空类型
来源：http://chy.9152youxi.cn

?string $name = null
来源：http://pwe.jianghu66.top

[U47] PHP：联合类型
来源：http://vpb.cashguo.top

int|string $id
来源：http://vvx.iojbl.cn

[U48] PHP：纯枚举
来源：http://gjc.bbcook.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gex.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://xfp.epnwcf.com

public readonly string $name
来源：http://rtx.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://nwa.fktsv.cn

public function __construct(private int $id) {}
来源：http://viq.pycfn.com

[U51] PHP：数组解构
来源：http://gfz.sweek.top

[$a, $b] = $arr;
来源：http://dzh.svipenyu.cn

[U52] PHP：箭头函数
来源：http://pdg.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://hkg.sysykeji.top

[U53] PHP：空合并运算符
来源：http://xxd.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://qqy.yj20258888.top

[U54] PHP：空安全调用
来源：http://srb.hammf.cn

$obj?->method()
来源：http://sog.yonumen.top

[U55] PHP：match 表达式
来源：http://jss.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jnv.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://byz.chenlongwang.top

f(a: 1, b: 2)
来源：http://ooa.svipenyu.cn

[U57] PHP：字符串插值
来源：http://irh.sweek.top

"值: {$a}"
来源：http://cfl.uphjek.com

[U58] PHP：数组三件套
来源：http://rtf.daxiang520.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ojq.sweek.top

[U59] PHP：自定义排序
来源：http://pto.quarkkingdee.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mpv.chenzaomai.com

[U60] PHP：JSON 编解码
来源：http://mqc.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ufo.yvedp.cn

[U61] PHP：正则
来源：http://ptr.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://myi.zdbjq.cn

[U62] PHP：日期对象
来源：http://cow.zhengqikj.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yqw.hywenlv.cn

[U63] PHP：文件读写
来源：http://yig.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dso.haohaochexian.top

[U64] PHP：目录遍历
来源：http://pec.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://hkl.jinghuilouyu.cn

[U65] PHP：会话
来源：http://kzu.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ijd.yueranfly.top

[U66] PHP：设置 Cookie
来源：http://cgf.hywenlv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://whh.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://mib.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qbn.shuidangran.top

[U68] PHP：PDO 连接
来源：http://sfx.cashguo.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mbm.dashuyun.cn

[U69] PHP：PDO 预处理
来源：http://tmu.bjfxy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://szl.fehbvm.com

[U70] PHP：PDO 事务
来源：http://vgo.chenlongwang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wvk.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://vog.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://mul.ehwqpu.com

[U72] PHP：写错误日志
来源：http://ghh.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://rid.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://ofh.yuxming.cn

parse_ini_file("config.ini", true)
来源：http://zrw.sysykeji.top

[U74] PHP：读取环境变量
来源：http://qzi.jinghuilouyu.cn

getenv("APP_ENV") ?: "production"
来源：http://sjb.zhaomingkeji.xyz

[U75] PHP：依赖注入
来源：http://hww.aibaodan.cn

composer require psr/container
来源：http://moj.aizwys.cn

[U76] PHP：简单路由
来源：http://sae.shzxlz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wob.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://jts.fzhhl.top

composer require twig/twig
来源：http://vom.chenzaomai.com

[U78] PHP：单元测试
来源：http://ila.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://ptu.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://ftr.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://cku.xuanzx.com

[U80] PHP：代码规范修复
来源：http://hhq.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://aph.hcnkem.com

[U81] JS：初始化项目
来源：http://mso.sufxvd.cn

npm init -y;  npm i express
来源：http://xdh.xuanzx.com

[U82] JS：package.json 脚本
来源：http://swd.meibo888.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://czw.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://qwe.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://ikm.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://ghw.xinyue.icu

module.exports = { a };  const { a } = require("./m");
来源：http://tkn.chenzaomai.com

[U85] JS：可选链
来源：http://bvz.c1oappe.top

a?.b?.c
来源：http://vgm.cdnleiting.top

[U86] JS：空值合并
来源：http://uwy.ctjpmb.com

a ?? b
来源：http://ivb.yonumen.top

[U87] JS：解构默认值
来源：http://wnr.gogol.net.cn

const { a = 1, b = 2 } = obj;
来源：http://wge.ydzc1.top

[U88] JS：对象展开合并
来源：http://blf.quarkkingdee.top

{ ...a, ...b }
来源：http://awb.cqqwz.cn

[U89] JS：数组去重
来源：http://qez.wangshuangyany.cn

[...new Set(arr)]
来源：http://suf.ppjwa.cn

[U90] JS：数字数组排序
来源：http://cjj.zhengqikj.top

[...arr].sort((a, b) => a - b)
来源：http://zur.nanxinkj.top

[U91] JS：对象键值遍历
来源：http://zwp.svipenyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ikj.52xcode.cn

[U92] JS：深拷贝
来源：http://kdp.zdbjq.cn

structuredClone(obj)
来源：http://glb.snrcjt.cn

[U93] JS：模板字符串
来源：http://med.fzhhl.top

`共 ${n} 条`
来源：http://orl.birdmap.top

[U94] JS：箭头函数
来源：http://uez.hysaishi.cn

const double = x => x * 2;
来源：http://xwt.meibo888.top

[U95] JS：Promise 包装
来源：http://xqt.snrcjt.cn

new Promise((resolve, reject) => {})
来源：http://hlh.316326.xyz

[U96] JS：async/await 与异常
来源：http://swx.birdmap.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zce.316326.xyz

[U97] JS：并发请求
来源：http://ddb.aizwys.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uge.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://ptx.cheryme.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kwv.daxiang520.top

[U99] JS：事件监听
来源：http://hrs.epnwcf.com

el.addEventListener("click", e => {})
来源：http://mqx.shanyushiyangkeji.top

[U100] JS：DOM 查询
来源：http://nsp.hnqzz.top

document.querySelector(".item")
来源：http://sfl.shanyushiyangkeji.top

[U101] JS：classList 操作
来源：http://qos.ybcxt.top

el.classList.toggle("active")
来源：http://yqw.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://iuw.hesvh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://qil.aizwys.cn

[U103] JS：定时器
来源：http://sbp.fanxiaobao.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ieg.pycfn.com

[U104] JS：防抖
来源：http://jbh.9152youxi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwg.9152youxi.cn

[U105] JS：节流
来源：http://ebt.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mps.vehdjk.com

[U106] JS：日期格式化
来源：http://csj.guannengcc.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://iog.feifeiyinyue.top

[U107] JS：数字千分位
来源：http://nqp.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jpp.cdnleiting.top

[U108] JS：随机整数
来源：http://ggn.sjlbkw.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://haj.iojbl.cn

[U109] JS：数组分组
来源：http://lyp.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://jlg.yonumen.top

[U110] JS：数组分块
来源：http://zbm.316326.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dvt.zdbjq.cn

[U111] JS：对象转 Map
来源：http://sui.yanxiufei.cn

new Map(Object.entries(obj))
来源：http://ies.aizwys.cn

[U112] JS：字符串补位
来源：http://mfb.vqdsnc.cn

"7".padStart(3, "0")
来源：http://ovt.redwolf501.top

[U113] JS：正则替换全部
来源：http://mcv.feifeiyinyue.top

s.replaceAll("a", "b")
来源：http://xcb.smart0.xyz

[U114] JS：JSON 深比较
来源：http://jet.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yfn.guowangkeji.top

[U115] JS：生成 UUID
来源：http://hqx.ydzc1.top

crypto.randomUUID()
来源：http://onx.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://uiu.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://szr.dashuyun.cn

[U117] JS：单元测试
来源：http://usu.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://mpu.shuidangran.top

[U118] JS：开发服务器
来源：http://egu.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://hpj.yueranfly.top

[U119] JS：生产构建
来源：http://spi.guowangkeji.top

npx vite build
来源：http://fir.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://nre.sweek.top

import.meta.env.VITE_API_URL
来源：http://ksu.aizwys.cn

================================================================================
来源：http://zdi.sysykeji.top

统计汇总
来源：http://bjm.ppjwa.cn

================================================================================
来源：http://jju.andypj.xyz

按语言统计（条）：
来源：http://heq.daxiang520.top

Python ......... 252
来源：http://gom.sweek.top

PHP ............ 252
来源：http://mmo.jiagoushi.top

JavaScript ..... 252
来源：http://rhu.gzhubu.top

TypeScript ..... 212
来源：http://evq.yongpay.top

Java ........... 212
来源：http://sdm.52xcode.cn

Go ............. 212
来源：http://las.zhengqikj.top

Ruby ........... 212
来源：http://naa.pycfn.com

C# ............. 212
来源：http://jrx.feifeiyinyue.top

C .............. 30
来源：http://awp.zdbjq.cn

C++ ............ 30
来源：http://qwq.bbcook.cn

SQL ............ 90
来源：http://roc.hysaishi.cn

Bash ........... 80
来源：http://pob.chenlongwang.top

Kotlin ......... 15
来源：http://gqs.nanxuanxn.top

Swift .......... 15
来源：http://ibt.hesvh.cn

Lua ............ 10
来源：http://lcr.jiagoushi.top

Perl ........... 10
来源：http://hck.wangdashe.top

Scala .......... 10
来源：http://jjn.xylfe.cn

------------------------------------
来源：http://mra.jqgufenzy.top

合计 ........... 2106 条
来源：http://wjm.cheryme.top

按章节统计：
来源：http://lkp.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vgz.jqgfzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://luy.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fdg.nanxuanxn.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hyk.wangshuangyany.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jsu.sufxvd.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://efh.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tdq.mhx1999.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kvo.tianlin.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qqf.sxryk.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tln.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dfm.iojbl.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fak.feifeiyinyue.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jbk.tian-w.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://udz.kuanghao11.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://egw.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kbz.guowangkeji.top


<!-- 参考信息 -->