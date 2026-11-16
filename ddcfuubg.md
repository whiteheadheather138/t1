代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://krn.ehwqpu.com

[T59] Scala：循环
来源：http://djs.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://bqb.uphjek.com

[T60] Scala：折叠
来源：http://zdi.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zly.jlsjyb.cn

================================================================================
来源：http://wuq.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jfp.tarul.cn

================================================================================
来源：http://wqz.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://owz.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tce.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://pmx.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jct.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://pnu.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cis.ybcxt.top

[U04] Py：变量调试打印
来源：http://qeg.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pex.hcnkem.com

[U05] Py：列表去重且保序
来源：http://ctn.hcnkem.com

list(dict.fromkeys(arr))
来源：http://qte.yj202588.top

[U06] Py：合并两个字典
来源：http://qia.jyoumei.cn

{**a, **b}
来源：http://ctu.vehdjk.com

[U07] Py：反转字典键值
来源：http://ldr.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://pks.ydjk.org.cn

[U08] Py：展平二维列表
来源：http://onf.shuidangran.top

[y for x in nested for y in x]
来源：http://bmk.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://awa.ehwqpu.com

max(d, key=d.get)
来源：http://tec.tanke756.top

[U10] Py：按值排序字典
来源：http://ftt.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xum.zdbjq.cn

[U11] Py：生成器表达式
来源：http://jmn.havefunace.top

(x * 2 for x in arr)
来源：http://mdw.guannengcc.top

[U12] Py：取出现最多的 3 个元素
来源：http://ffd.jinghuilouyu.cn

Counter(arr).most_common(3)
来源：http://lnu.yfazqb.com

[U13] Py：固定长度队列
来源：http://iwq.fengsongda.top

deque(maxlen=10)
来源：http://udt.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://zvb.hesvh.cn

defaultdict(list)
来源：http://whj.mhx1999.top

[U15] Py：高精度计时
来源：http://msm.ehwqpu.com

t = time.perf_counter()
来源：http://etn.yj20258888.top

[U16] Py：命令行参数解析
来源：http://atg.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zfi.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://siu.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://qom.yueranfly.top

[U18] Py：预编译正则
来源：http://jgl.yj20258.top

pat = re.compile(r"\d+")
来源：http://iok.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://gzu.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xgc.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://jwn.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://oir.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://qhl.xylfe.cn

@contextlib.contextmanager
来源：http://jgs.yj20258888.top

[U22] Py：矩阵转置
来源：http://ylq.zdbjq.cn

list(zip(*m))
来源：http://jtw.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://jjd.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gyr.vehdjk.com

[U24] Py：路径操作
来源：http://vor.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tbg.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://oku.52xcode.cn

csv.DictReader(f)
来源：http://jdu.yanxiufei.cn

[U26] Py：并发下载
来源：http://dgm.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://syt.xuetiantiany.cn

[U27] Py：异步 HTTP
来源：http://zdu.zhoulong.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zsr.xinyue.icu

[U28] Py：类型别名
来源：http://fox.pengpengdd.cyou

UserId = int
来源：http://wye.zhengqikj.top

[U29] Py：属性校验
来源：http://grr.guannengcc.top

@property 与 @x.setter 配合
来源：http://jcn.chenzaomai.com

[U30] Py：数据类
来源：http://yvw.yj20258.top

@dataclass(slots=True)
来源：http://ndh.nanxuanxn.top

[U31] Py：单测
来源：http://sqv.yfazqb.com

python -m pytest -q
来源：http://jph.sweek.top

[U32] Py：代码格式化
来源：http://rec.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://szd.tanke756.top

[U33] Py：打包发布
来源：http://fmq.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://uot.jqgufenzy.top

[U34] Py：判断编码
来源：http://tty.pycfn.com

chardet.detect(raw)
来源：http://cfd.zdqjudy.top

[U35] Py：发送邮件
来源：http://hqi.yuanzhike.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gmv.nanxuanxn.top

[U36] Py：定时任务
来源：http://pcj.ybcxt.top

schedule.every(10).minutes.do(job)
来源：http://kmn.hnqzz.top

[U37] Py：读写 Excel
来源：http://zal.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://dlb.aizwys.cn

[U38] Py：获取脚本所在目录
来源：http://dcj.meibo888.top

Path(__file__).resolve().parent
来源：http://pun.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://laa.hysaishi.cn

sys.stdout.isatty()
来源：http://aiq.ydzc1.top

[U40] Py：打印到标准错误
来源：http://qkf.yj202588.top

print("err", file=sys.stderr)
来源：http://zdw.pengpengdd.cyou

[U41] PHP：初始化 Composer 项目
来源：http://kzq.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vrc.quarkkingdee.top

[U42] PHP：PSR-4 自动加载
来源：http://pcf.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fej.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://mtw.guannengcc.top

namespace App\Http;
来源：http://dtx.nanxinkj.top

[U44] PHP：开启严格类型
来源：http://cxy.sweek.top

declare(strict_types=1);
来源：http://jri.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://skj.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nlq.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://tmx.pycfn.com

?string $name = null
来源：http://nxf.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://idq.daria6918.cn

int|string $id
来源：http://jbc.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://sxe.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jyh.jiagoushi.top

[U49] PHP：只读属性
来源：http://jcl.jinghuilouyu.cn

public readonly string $name
来源：http://rej.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://abm.chenlongwang.top

public function __construct(private int $id) {}
来源：http://kxx.xziqi.cn

[U51] PHP：数组解构
来源：http://iaf.jqgufenzy.top

[$a, $b] = $arr;
来源：http://fmj.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://miw.jinyuanbaomall.cn

$double = fn($x) => $x * 2;
来源：http://vmw.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://cib.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://svz.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://cfz.hcnkem.com

$obj?->method()
来源：http://wls.fehbvm.com

[U55] PHP：match 表达式
来源：http://fgc.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qsu.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://qwe.shuidangran.top

f(a: 1, b: 2)
来源：http://sxk.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://kqw.jinyuanbaomall.cn

"值: {$a}"
来源：http://hqh.fengsongda.top

[U58] PHP：数组三件套
来源：http://cnx.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://giz.ybcxt.top

[U59] PHP：自定义排序
来源：http://cca.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pfz.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://gqr.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gmt.yuxming.cn

[U61] PHP：正则
来源：http://eyi.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://obs.epnwcf.com

[U62] PHP：日期对象
来源：http://pke.jqgfzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eoc.quarkkingdee.top

[U63] PHP：文件读写
来源：http://iqf.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bqb.havefunace.top

[U64] PHP：目录遍历
来源：http://dab.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://zcd.tanke756.top

[U65] PHP：会话
来源：http://kha.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://mbf.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://eij.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ycl.havefunace.top

[U67] PHP：处理文件上传
来源：http://vba.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mlf.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://jmp.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kgm.meibo888.top

[U69] PHP：PDO 预处理
来源：http://rib.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zdy.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://ung.cheryme.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xgy.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://sck.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://yex.zycfv.cn

[U72] PHP：写错误日志
来源：http://cyz.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://yxf.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://pqg.ybcxt.top

parse_ini_file("config.ini", true)
来源：http://dcd.hesvh.cn

[U74] PHP：读取环境变量
来源：http://vay.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://jou.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://qvy.nwbrower.top

composer require psr/container
来源：http://wum.ivvv.top

[U76] PHP：简单路由
来源：http://qyj.yj20258888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://afm.sweek.top

[U77] PHP：模板渲染
来源：http://xmi.iojbl.cn

composer require twig/twig
来源：http://xfd.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://fko.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://bwm.zhoulong.xyz

[U79] PHP：静态分析
来源：http://qlo.uphjek.com

composer require --dev phpstan/phpstan
来源：http://tqv.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://zxi.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nrl.dianchejie.cn

[U81] JS：初始化项目
来源：http://qyk.hongshengwenyu.top

npm init -y;  npm i express
来源：http://anf.xuanzx.com

[U82] JS：package.json 脚本
来源：http://kqk.yongpay.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rfg.sxryk.cn

[U83] JS：ES Module 导入导出
来源：http://jif.cucudq.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pbq.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://htt.havefunace.top

module.exports = { a };  const { a } = require("./m");
来源：http://ceo.xziqi.cn

[U85] JS：可选链
来源：http://qps.guowangkeji.top

a?.b?.c
来源：http://iyc.daria6918.cn

[U86] JS：空值合并
来源：http://whp.havefunace.top

a ?? b
来源：http://jce.zhongyouzk.top

[U87] JS：解构默认值
来源：http://mes.uphjek.com

const { a = 1, b = 2 } = obj;
来源：http://shn.nwbrower.top

[U88] JS：对象展开合并
来源：http://ykg.hongshengwenyu.top

{ ...a, ...b }
来源：http://zii.feifeiyinyue.top

[U89] JS：数组去重
来源：http://lmb.zhijiandao.cn

[...new Set(arr)]
来源：http://fsm.nanxuanxn.top

[U90] JS：数字数组排序
来源：http://jzq.yj202588.top

[...arr].sort((a, b) => a - b)
来源：http://bdb.guannengcc.top

[U91] JS：对象键值遍历
来源：http://jdm.cdnleiting.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eao.dashuyun.cn

[U92] JS：深拷贝
来源：http://ajp.tianlin.xyz

structuredClone(obj)
来源：http://ytm.xuanzx.com

[U93] JS：模板字符串
来源：http://bki.ivvv.top

`共 ${n} 条`
来源：http://puw.jlsjyb.cn

[U94] JS：箭头函数
来源：http://zyr.jiagoushi.top

const double = x => x * 2;
来源：http://itc.epnwcf.com

[U95] JS：Promise 包装
来源：http://nqf.jyoumei.cn

new Promise((resolve, reject) => {})
来源：http://qfh.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://jfw.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gng.cucudq.cn

[U97] JS：并发请求
来源：http://tew.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://hjx.shuidangran.top

[U98] JS：fetch 带 JSON
来源：http://hbn.hnqzz.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pij.sufxvd.cn

[U99] JS：事件监听
来源：http://brm.guannengcc.top

el.addEventListener("click", e => {})
来源：http://rpi.sysykeji.top

[U100] JS：DOM 查询
来源：http://kod.nanxuanxn.top

document.querySelector(".item")
来源：http://bos.hnxiangtu.top

[U101] JS：classList 操作
来源：http://zdn.redwolf501.top

el.classList.toggle("active")
来源：http://kqi.yueranfly.top

[U102] JS：本地存储
来源：http://bwm.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uyj.hnqzz.top

[U103] JS：定时器
来源：http://bhr.hywenlv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rti.shanyushiyangtech.top

[U104] JS：防抖
来源：http://cho.xuetiantiany.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvi.zhixingplan.top

[U105] JS：节流
来源：http://glq.chenlongwang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eag.sweek.top

[U106] JS：日期格式化
来源：http://cvn.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://skq.zhoulong.xyz

[U107] JS：数字千分位
来源：http://zgr.xuanzx.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zjv.daria6918.cn

[U108] JS：随机整数
来源：http://fsl.zhiwuduotai.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ryi.dianchejie.cn

[U109] JS：数组分组
来源：http://zhd.bjfxy.top

Object.groupBy(arr, x => x.type)
来源：http://oud.ywan-chungtsiang.top

[U110] JS：数组分块
来源：http://pws.c1oappe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gqi.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://yyw.daria6918.cn

new Map(Object.entries(obj))
来源：http://hmc.guowangkeji.top

[U112] JS：字符串补位
来源：http://yua.xylfe.cn

"7".padStart(3, "0")
来源：http://hqz.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://vvx.dashuyun.cn

s.replaceAll("a", "b")
来源：http://sfa.sxryk.cn

[U114] JS：JSON 深比较
来源：http://wcv.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://yzk.hnxiangtu.top

[U115] JS：生成 UUID
来源：http://pig.meibo888.top

crypto.randomUUID()
来源：http://tii.zhengqikj.top

[U116] JS：类型检查（JSDoc）
来源：http://sfn.bjfxy.top

/** @param {string} name */ function f(name) {}
来源：http://ivg.quarkkingdee.top

[U117] JS：单元测试
来源：http://zvh.guowangkeji.top

npm i -D vitest;  npx vitest
来源：http://ljw.sxryk.cn

[U118] JS：开发服务器
来源：http://amk.cashguo.top

npm i -D vite;  npx vite
来源：http://vmc.chenlongwang.top

[U119] JS：生产构建
来源：http://pjm.hcnkem.com

npx vite build
来源：http://gei.hfpthk.cn

[U120] JS：读取环境变量（Vite）
来源：http://yit.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://bdi.sysykeji.top

================================================================================
来源：http://abv.yangfankeji.com

统计汇总
来源：http://aci.ybcxt.top

================================================================================
来源：http://wke.nanxinkj.top

按语言统计（条）：
来源：http://hdi.uphjek.com

Python ......... 252
来源：http://mdw.jianghu66.top

PHP ............ 252
来源：http://fwm.ybcxt.top

JavaScript ..... 252
来源：http://udv.ctjpmb.com

TypeScript ..... 212
来源：http://cow.cucudq.cn

Java ........... 212
来源：http://phu.pengpengdd.cyou

Go ............. 212
来源：http://snh.quarkkingdee.top

Ruby ........... 212
来源：http://gmv.yangfankeji.com

C# ............. 212
来源：http://byv.pengpengdd.cyou

C .............. 30
来源：http://lxv.shzxlz.cn

C++ ............ 30
来源：http://nce.smart0.xyz

SQL ............ 90
来源：http://ogj.chenjidiqi.icu

Bash ........... 80
来源：http://bhx.yonumen.top

Kotlin ......... 15
来源：http://qzw.yj20258888.top

Swift .......... 15
来源：http://wvb.shzxlz.cn

Lua ............ 10
来源：http://fzr.aizwys.cn

Perl ........... 10
来源：http://trq.svipenyu.cn

Scala .......... 10
来源：http://xye.yuanzhike.top

------------------------------------
来源：http://eou.feifeiyinyue.top

合计 ........... 2106 条
来源：http://gmz.chenjidiqi.icu

按章节统计：
来源：http://fxm.sufxvd.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kwk.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xfy.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://tgh.sysykeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://teo.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tdg.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mib.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oni.xuanzx.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cru.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qnu.sufxvd.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lga.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ocw.zhijiandao.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ntw.fanxiaobao.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rdo.zhiwuduotai.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://khc.sxryk.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xij.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ifp.zhoulong.xyz

Q SQL 专题                              90
来源：http://myn.zhixingplan.top

R Bash 专题                             80
来源：http://swd.pycfn.com

S C / C++ 专题                          60
来源：http://kqs.cucudq.cn

T 其他语言补充                          60
来源：http://opl.jinyuanbaomall.cn

U 高频实用片段                         120
来源：http://rdx.chenzaomai.com

------------------------------------
来源：http://tlz.ywan-chungtsiang.top

合计                                  2106 条
来源：http://mjp.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://gte.jlsjyb.cn

使用提醒
来源：http://hvl.guannengcc.top

--------------------------------------------------------------------------------
来源：http://dzg.cucudq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qpa.zhengqikj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ujk.sysykeji.top


<!-- 参考信息 -->