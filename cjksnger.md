代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://dgr.zhixingplan.top

[T59] Scala：循环
来源：http://yuy.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://azl.sweek.top

[T60] Scala：折叠
来源：http://vmt.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qwa.zycfv.cn

================================================================================
来源：http://tmc.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oat.fehbvm.com

================================================================================
来源：http://zqo.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://ras.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cvt.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://dpg.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rkx.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://voa.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dvd.epnwcf.com

[U04] Py：变量调试打印
来源：http://smb.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qtb.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://taa.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://eat.xylfe.cn

[U06] Py：合并两个字典
来源：http://zam.hammf.cn

{**a, **b}
来源：http://svz.316326.xyz

[U07] Py：反转字典键值
来源：http://uqf.aizwys.cn

{v: k for k, v in d.items()}
来源：http://ibl.ydzc1.top

[U08] Py：展平二维列表
来源：http://vib.guannengcc.top

[y for x in nested for y in x]
来源：http://eij.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://lxt.uphjek.com

max(d, key=d.get)
来源：http://tcv.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://ppb.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hek.daxiang520.top

[U11] Py：生成器表达式
来源：http://sim.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://ate.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://pgy.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://zkt.zdbjq.cn

[U13] Py：固定长度队列
来源：http://koh.ydjk.org.cn

deque(maxlen=10)
来源：http://odi.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://vxs.sweek.top

defaultdict(list)
来源：http://imu.hfpthk.cn

[U15] Py：高精度计时
来源：http://fbp.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://xma.ybcxt.top

[U16] Py：命令行参数解析
来源：http://iqn.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iic.snrcjt.cn

[U17] Py：初始化日志
来源：http://zrz.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://cxg.nanxuanxn.top

[U18] Py：预编译正则
来源：http://kox.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://xxl.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://irv.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vsf.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://hcy.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://eve.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://uke.yonumen.top

@contextlib.contextmanager
来源：http://ons.ivvv.top

[U22] Py：矩阵转置
来源：http://btr.yj202588.top

list(zip(*m))
来源：http://krs.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://ekz.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gtx.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://swr.hongshengwenyu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jzd.jqgufenzy.top

[U25] Py：CSV 按字典读
来源：http://eyf.fehbvm.com

csv.DictReader(f)
来源：http://xue.tianlin.xyz

[U26] Py：并发下载
来源：http://gve.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ppd.tian-w.cn

[U27] Py：异步 HTTP
来源：http://aho.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://bhi.zhengqikj.top

[U28] Py：类型别名
来源：http://ptf.wangdashe.top

UserId = int
来源：http://qiu.yanxiufei.cn

[U29] Py：属性校验
来源：http://oyc.chenjidiqi.icu

@property 与 @x.setter 配合
来源：http://ysk.yj20258.top

[U30] Py：数据类
来源：http://njs.jyoumei.cn

@dataclass(slots=True)
来源：http://jad.ywan-chungtsiang.top

[U31] Py：单测
来源：http://dsa.cashguo.top

python -m pytest -q
来源：http://vdr.0kj1m.cn

[U32] Py：代码格式化
来源：http://pcm.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://gxh.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://jng.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://chc.ivvv.top

[U34] Py：判断编码
来源：http://fka.shangyingyoupin.top

chardet.detect(raw)
来源：http://hog.jinqigfzy.top

[U35] Py：发送邮件
来源：http://jaa.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ctk.chenzaomai.com

[U36] Py：定时任务
来源：http://rbv.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://xdj.fktsv.cn

[U37] Py：读写 Excel
来源：http://kka.xziqi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nho.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://amg.vehdjk.com

Path(__file__).resolve().parent
来源：http://bdn.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://mek.yuxming.cn

sys.stdout.isatty()
来源：http://fpn.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://dbg.cucudq.cn

print("err", file=sys.stderr)
来源：http://uja.ybcxt.top

[U41] PHP：初始化 Composer 项目
来源：http://grs.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gfj.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://qul.gogol.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://arc.guannengcc.top

[U43] PHP：声明命名空间
来源：http://wzc.shuidangran.top

namespace App\Http;
来源：http://gnx.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://bex.zdqjudy.top

declare(strict_types=1);
来源：http://otc.fengsongda.top

[U45] PHP：类型声明与返回类型
来源：http://zjx.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jnm.hammf.cn

[U46] PHP：可空类型
来源：http://enp.zhaomingkeji.xyz

?string $name = null
来源：http://vde.hesvh.cn

[U47] PHP：联合类型
来源：http://gaj.52xcode.cn

int|string $id
来源：http://ahr.haohaochexian.top

[U48] PHP：纯枚举
来源：http://uuz.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mpb.zhengqikj.top

[U49] PHP：只读属性
来源：http://yit.jyoumei.cn

public readonly string $name
来源：http://ryj.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://cna.guannengcc.top

public function __construct(private int $id) {}
来源：http://gml.havefunace.top

[U51] PHP：数组解构
来源：http://cof.mhx1999.top

[$a, $b] = $arr;
来源：http://aso.bbcook.cn

[U52] PHP：箭头函数
来源：http://ope.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://ldw.svipenyu.cn

[U53] PHP：空合并运算符
来源：http://dln.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://kbj.hcnkem.com

[U54] PHP：空安全调用
来源：http://pza.birdmap.top

$obj?->method()
来源：http://doe.hnxiangtu.top

[U55] PHP：match 表达式
来源：http://kgk.chenlongwang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://euu.hywenlv.cn

[U56] PHP：命名参数
来源：http://ayw.meibo888.top

f(a: 1, b: 2)
来源：http://rvf.316326.xyz

[U57] PHP：字符串插值
来源：http://xca.chenzaomai.com

"值: {$a}"
来源：http://cmg.chenzaomai.com

[U58] PHP：数组三件套
来源：http://yvq.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://voj.jiagoushi.top

[U59] PHP：自定义排序
来源：http://lkw.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dod.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://lpo.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bbe.zycfv.cn

[U61] PHP：正则
来源：http://ohw.chenzaomai.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sag.cashguo.top

[U62] PHP：日期对象
来源：http://zmt.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nlp.yfazqb.com

[U63] PHP：文件读写
来源：http://mok.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ofa.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://cdt.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://ypk.sufxvd.cn

[U65] PHP：会话
来源：http://snp.shangyingyoupin.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jpb.fanxiaobao.xyz

[U66] PHP：设置 Cookie
来源：http://mvt.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fff.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://opo.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mnd.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://pes.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mvl.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://vpb.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cji.ywan-chungtsiang.top

[U70] PHP：PDO 事务
来源：http://ooj.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bxb.c1oappe.top

[U71] PHP：抛出异常
来源：http://isg.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://ccy.xuanzx.com

[U72] PHP：写错误日志
来源：http://hof.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://zgn.zhoulong.xyz

[U73] PHP：读取 ini 配置
来源：http://rej.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://lxb.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://shr.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://jtz.yongpay.top

[U75] PHP：依赖注入
来源：http://awb.smart0.xyz

composer require psr/container
来源：http://muv.sweek.top

[U76] PHP：简单路由
来源：http://evw.hammf.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zza.jiagoushi.top

[U77] PHP：模板渲染
来源：http://ath.hammf.cn

composer require twig/twig
来源：http://rir.gogol.net.cn

[U78] PHP：单元测试
来源：http://ptg.yonumen.top

composer require --dev phpunit/phpunit
来源：http://anf.tarul.cn

[U79] PHP：静态分析
来源：http://sjt.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://gzs.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://fos.yfazqb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://eer.meibo888.top

[U81] JS：初始化项目
来源：http://ovu.epnwcf.com

npm init -y;  npm i express
来源：http://qdm.hywenlv.cn

[U82] JS：package.json 脚本
来源：http://xds.smart0.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://puv.ppjwa.cn

[U83] JS：ES Module 导入导出
来源：http://bjt.dianchejie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tbc.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://wxh.wangdashe.top

module.exports = { a };  const { a } = require("./m");
来源：http://nqh.havefunace.top

[U85] JS：可选链
来源：http://qrl.guannengcc.top

a?.b?.c
来源：http://lhg.pengpengdd.cyou

[U86] JS：空值合并
来源：http://fzl.guowangkeji.top

a ?? b
来源：http://eaa.hnxiangtu.top

[U87] JS：解构默认值
来源：http://ous.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://fns.jinqigufen.top

[U88] JS：对象展开合并
来源：http://dqe.hysaishi.cn

{ ...a, ...b }
来源：http://wpg.yangfankeji.com

[U89] JS：数组去重
来源：http://piw.nwbrower.top

[...new Set(arr)]
来源：http://yqr.jinghuilouyu.cn

[U90] JS：数字数组排序
来源：http://ywr.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://qlc.yj20258.top

[U91] JS：对象键值遍历
来源：http://koh.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ysr.yj20258.top

[U92] JS：深拷贝
来源：http://gzb.zhijiandao.cn

structuredClone(obj)
来源：http://idh.sxryk.cn

[U93] JS：模板字符串
来源：http://pte.52xcode.cn

`共 ${n} 条`
来源：http://tye.jinqigufen.top

[U94] JS：箭头函数
来源：http://kqs.fanxiaobao.xyz

const double = x => x * 2;
来源：http://jao.zycfv.cn

[U95] JS：Promise 包装
来源：http://eso.yj20258.top

new Promise((resolve, reject) => {})
来源：http://kqa.vehdjk.com

[U96] JS：async/await 与异常
来源：http://izv.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yxt.sufxvd.cn

[U97] JS：并发请求
来源：http://cse.ybcxt.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gqw.iojbl.cn

[U98] JS：fetch 带 JSON
来源：http://lgs.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hto.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://ane.yuxming.cn

el.addEventListener("click", e => {})
来源：http://uec.nwbrower.top

[U100] JS：DOM 查询
来源：http://dow.jyoumei.cn

document.querySelector(".item")
来源：http://dgm.snrcjt.cn

[U101] JS：classList 操作
来源：http://xrc.hammf.cn

el.classList.toggle("active")
来源：http://wce.cheryme.top

[U102] JS：本地存储
来源：http://mpi.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://cvx.jinqigufen.top

[U103] JS：定时器
来源：http://trw.fktsv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tvi.aibaodan.cn

[U104] JS：防抖
来源：http://mpe.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dzf.yuxming.cn

[U105] JS：节流
来源：http://aqp.yongpay.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wvv.fehbvm.com

[U106] JS：日期格式化
来源：http://htn.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oku.yongpay.top

[U107] JS：数字千分位
来源：http://lvc.fktsv.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://drp.hysaishi.cn

[U108] JS：随机整数
来源：http://jfz.hesvh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gtl.hnqzz.top

[U109] JS：数组分组
来源：http://cha.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://lyy.guannengcc.top

[U110] JS：数组分块
来源：http://wob.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lop.iojbl.cn

[U111] JS：对象转 Map
来源：http://rja.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://dpm.dianchejie.cn

[U112] JS：字符串补位
来源：http://igr.jinqigufen.top

"7".padStart(3, "0")
来源：http://tjq.cucudq.cn

[U113] JS：正则替换全部
来源：http://ttc.meibo888.top

s.replaceAll("a", "b")
来源：http://zyf.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://bxa.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://etx.hysaishi.cn

[U115] JS：生成 UUID
来源：http://lig.ybcxt.top

crypto.randomUUID()
来源：http://pui.yvedp.cn

[U116] JS：类型检查（JSDoc）
来源：http://yue.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://vao.jinqigfzy.top

[U117] JS：单元测试
来源：http://hob.iojbl.cn

npm i -D vitest;  npx vitest
来源：http://upm.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://yhg.hfpthk.cn

npm i -D vite;  npx vite
来源：http://sqy.sxryk.cn

[U119] JS：生产构建
来源：http://ron.fanxiaobao.xyz

npx vite build
来源：http://hua.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://vrw.yonumen.top

import.meta.env.VITE_API_URL
来源：http://ubr.hnxiangtu.top

================================================================================
来源：http://pzu.yj202588.top

统计汇总
来源：http://jsm.cdnleiting.top

================================================================================
来源：http://keb.zhongyouzk.top

按语言统计（条）：
来源：http://kiq.mhx1999.top

Python ......... 252
来源：http://knd.bbcook.cn

PHP ............ 252
来源：http://ctu.yuanzhike.top

JavaScript ..... 252
来源：http://bjx.cashguo.top

TypeScript ..... 212
来源：http://nhk.zhiwuduotai.top

Java ........... 212
来源：http://smn.fengsongda.top

Go ............. 212
来源：http://vuc.sweek.top

Ruby ........... 212
来源：http://ksk.fengsongda.top

C# ............. 212
来源：http://zwi.guannengcc.top

C .............. 30
来源：http://pxi.cashguo.top

C++ ............ 30
来源：http://uiu.cashguo.top

SQL ............ 90
来源：http://lmg.316326.xyz

Bash ........... 80
来源：http://eda.fengsongda.top

Kotlin ......... 15
来源：http://zye.zhixingplan.top

Swift .......... 15
来源：http://fbh.ydzc1.top

Lua ............ 10
来源：http://cvx.guannengcc.top

Perl ........... 10
来源：http://buo.svipenyu.cn

Scala .......... 10
来源：http://bnd.cashguo.top

------------------------------------
来源：http://rfa.bbcook.cn

合计 ........... 2106 条
来源：http://rhl.tian-w.cn

按章节统计：
来源：http://mru.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lof.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ogc.zdqjudy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xzx.mhx1999.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aog.zhoulong.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bwq.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vrk.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oos.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ffd.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gnb.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://eaj.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sjm.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://elj.gotoacloud.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jrn.jianghu66.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ehx.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vda.uphjek.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vhg.nanxuanxn.top

Q SQL 专题                              90
来源：http://bew.zhijiandao.cn

R Bash 专题                             80
来源：http://vmf.9152youxi.cn

S C / C++ 专题                          60
来源：http://mdn.sjlbkw.cn

T 其他语言补充                          60
来源：http://eal.zhoulong.xyz

U 高频实用片段                         120
来源：http://xbn.andypj.xyz

------------------------------------
来源：http://kqo.jiagoushi.top

合计                                  2106 条
来源：http://vii.guannengcc.top

--------------------------------------------------------------------------------
来源：http://ksu.sxryk.cn

使用提醒
来源：http://vlz.pycfn.com

--------------------------------------------------------------------------------
来源：http://cpl.jlsjyb.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pee.haohaochexian.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ihr.zdbjq.cn


<!-- 参考信息 -->