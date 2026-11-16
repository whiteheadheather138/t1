代发 wailian999

val a = 1;  var b = 2
来源：http://ose.xylfe.cn

[T53] Scala：字符串插值
来源：http://zvg.yuxming.cn

s"值: $b"
来源：http://jmg.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://evm.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://lcm.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://acv.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://zqs.zhiwuduotai.top

[T56] Scala：样例类
来源：http://sta.epnwcf.com

case class User(name: String, age: Int)
来源：http://vun.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://eql.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zeq.gogol.net.cn

[T58] Scala：函数定义
来源：http://end.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://zdq.zhoulong.xyz

[T59] Scala：循环
来源：http://trt.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://tav.zhijiandao.cn

[T60] Scala：折叠
来源：http://oqa.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://npl.ywan-chungtsiang.top

================================================================================
来源：http://uif.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://amd.zhengqikj.top

================================================================================
来源：http://bsh.cashguo.top

[U01] Py：创建虚拟环境
来源：http://jpl.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://bxy.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://yst.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yis.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://ucj.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://npm.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://pgg.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tcq.fzhhl.top

[U05] Py：列表去重且保序
来源：http://vii.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://rdz.dashuyun.cn

[U06] Py：合并两个字典
来源：http://ovx.jianghu66.top

{**a, **b}
来源：http://pic.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://tve.yongpay.top

{v: k for k, v in d.items()}
来源：http://tqb.haohaochexian.top

[U08] Py：展平二维列表
来源：http://vzb.tarul.cn

[y for x in nested for y in x]
来源：http://lqd.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://yaz.fehbvm.com

max(d, key=d.get)
来源：http://toe.cdnleiting.top

[U10] Py：按值排序字典
来源：http://hdg.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://poz.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://lkl.zhijiandao.cn

(x * 2 for x in arr)
来源：http://xbh.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://mwo.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://snn.nanxinkj.top

[U13] Py：固定长度队列
来源：http://gad.cheryme.top

deque(maxlen=10)
来源：http://urp.tarul.cn

[U14] Py：分组收集到列表
来源：http://hcr.0kj1m.cn

defaultdict(list)
来源：http://yxh.yuxming.cn

[U15] Py：高精度计时
来源：http://eup.mhx1999.top

t = time.perf_counter()
来源：http://voh.redwolf501.top

[U16] Py：命令行参数解析
来源：http://fzy.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ccb.jianghu66.top

[U17] Py：初始化日志
来源：http://qol.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://jqc.shanyushiyangkeji.top

[U18] Py：预编译正则
来源：http://jac.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://vss.xylfe.cn

[U19] Py：正则替换带回调
来源：http://cht.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xnq.sweek.top

[U20] Py：缓存函数结果
来源：http://qvn.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://cfo.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://ztv.hammf.cn

@contextlib.contextmanager
来源：http://xqa.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://tnw.svipenyu.cn

list(zip(*m))
来源：http://mkx.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://kns.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xcy.ctjpmb.com

[U24] Py：路径操作
来源：http://pny.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kyw.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://scb.yanxiufei.cn

csv.DictReader(f)
来源：http://xys.yueranfly.top

[U26] Py：并发下载
来源：http://rdw.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dql.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://jbs.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://bpl.chenzaomai.com

[U28] Py：类型别名
来源：http://hru.0kj1m.cn

UserId = int
来源：http://rro.wangshuangyany.cn

[U29] Py：属性校验
来源：http://fyp.svipenyu.cn

@property 与 @x.setter 配合
来源：http://glg.hnqzz.top

[U30] Py：数据类
来源：http://pkf.xinyue.icu

@dataclass(slots=True)
来源：http://tir.wangshuangyany.cn

[U31] Py：单测
来源：http://wpp.0kj1m.cn

python -m pytest -q
来源：http://xwd.gotoacloud.top

[U32] Py：代码格式化
来源：http://bgp.yj20258888.top

ruff format . && ruff check --fix .
来源：http://mrn.zdbjq.cn

[U33] Py：打包发布
来源：http://drd.zhengqikj.top

python -m build  （依赖 pyproject.toml）
来源：http://qux.xylfe.cn

[U34] Py：判断编码
来源：http://byl.fzhhl.top

chardet.detect(raw)
来源：http://msj.cucudq.cn

[U35] Py：发送邮件
来源：http://yib.pengpengdd.cyou

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://loc.bbcook.cn

[U36] Py：定时任务
来源：http://lmi.feifeiyinyue.top

schedule.every(10).minutes.do(job)
来源：http://vkt.zhixingplan.top

[U37] Py：读写 Excel
来源：http://xkg.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lim.nanxuanxn.top

[U38] Py：获取脚本所在目录
来源：http://niw.tanke756.top

Path(__file__).resolve().parent
来源：http://dyy.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://asy.shanyushiyangkeji.top

sys.stdout.isatty()
来源：http://vqh.c1oappe.top

[U40] Py：打印到标准错误
来源：http://rdl.zdbjq.cn

print("err", file=sys.stderr)
来源：http://dlz.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://khq.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://utu.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://gij.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yja.tian-w.cn

[U43] PHP：声明命名空间
来源：http://ede.cheryme.top

namespace App\Http;
来源：http://qqu.316326.xyz

[U44] PHP：开启严格类型
来源：http://ylq.hnqzz.top

declare(strict_types=1);
来源：http://ywi.fktsv.cn

[U45] PHP：类型声明与返回类型
来源：http://lud.birdmap.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ync.yongpay.top

[U46] PHP：可空类型
来源：http://fye.ehwqpu.com

?string $name = null
来源：http://xjh.guannengcc.top

[U47] PHP：联合类型
来源：http://gom.svipenyu.cn

int|string $id
来源：http://hls.hfpthk.cn

[U48] PHP：纯枚举
来源：http://uiq.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hlh.ehwqpu.com

[U49] PHP：只读属性
来源：http://ldj.9152youxi.cn

public readonly string $name
来源：http://meq.zhixingplan.top

[U50] PHP：构造器属性提升
来源：http://ntr.hywenlv.cn

public function __construct(private int $id) {}
来源：http://wda.ydzc1.top

[U51] PHP：数组解构
来源：http://oph.ppjwa.cn

[$a, $b] = $arr;
来源：http://bmi.redwolf501.top

[U52] PHP：箭头函数
来源：http://vwf.ivvv.top

$double = fn($x) => $x * 2;
来源：http://vhv.52xcode.cn

[U53] PHP：空合并运算符
来源：http://crt.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://wtw.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://jnb.zhongyouzk.top

$obj?->method()
来源：http://ekx.chenjidiqi.icu

[U55] PHP：match 表达式
来源：http://lra.gaohongyu789.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wjg.jinqigfzy.top

[U56] PHP：命名参数
来源：http://tds.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://qcj.guannengcc.top

[U57] PHP：字符串插值
来源：http://nyq.fanxiaobao.xyz

"值: {$a}"
来源：http://yrf.tianlin.xyz

[U58] PHP：数组三件套
来源：http://qwt.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qsf.haohaochexian.top

[U59] PHP：自定义排序
来源：http://zmr.bjfxy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zop.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://onj.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rlb.yangfankeji.com

[U61] PHP：正则
来源：http://kvu.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rtb.redwolf501.top

[U62] PHP：日期对象
来源：http://jjl.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jdt.hfpthk.cn

[U63] PHP：文件读写
来源：http://rxk.shuidangran.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tiq.yonumen.top

[U64] PHP：目录遍历
来源：http://nqw.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://rrf.daria6918.cn

[U65] PHP：会话
来源：http://aup.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hfb.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://mcj.dashuyun.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xnu.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://tzi.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://psf.pengpengdd.cyou

[U68] PHP：PDO 连接
来源：http://rcw.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hhk.cheryme.top

[U69] PHP：PDO 预处理
来源：http://bqh.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqa.bbcook.cn

[U70] PHP：PDO 事务
来源：http://iea.birdmap.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pet.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://dyy.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://qpg.ybcxt.top

[U72] PHP：写错误日志
来源：http://iot.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://yfn.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://rzb.pengpengdd.cyou

parse_ini_file("config.ini", true)
来源：http://zkn.hesvh.cn

[U74] PHP：读取环境变量
来源：http://pjd.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://rge.tanke756.top

[U75] PHP：依赖注入
来源：http://mai.ybcxt.top

composer require psr/container
来源：http://zbe.andypj.xyz

[U76] PHP：简单路由
来源：http://gdp.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://brx.9152youxi.cn

[U77] PHP：模板渲染
来源：http://ouc.jlsjyb.cn

composer require twig/twig
来源：http://tew.cucudq.cn

[U78] PHP：单元测试
来源：http://kvw.sweek.top

composer require --dev phpunit/phpunit
来源：http://txg.zycfv.cn

[U79] PHP：静态分析
来源：http://nev.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://uub.ybcxt.top

[U80] PHP：代码规范修复
来源：http://ztn.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://zrw.tarul.cn

[U81] JS：初始化项目
来源：http://gle.dianchejie.cn

npm init -y;  npm i express
来源：http://jgk.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://qsr.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://khb.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://cpv.chenlongwang.top

export const a = 1;  import { a } from "./m.js";
来源：http://mki.dashuyun.cn

[U84] JS：CommonJS 写法
来源：http://mlx.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oub.c1oappe.top

[U85] JS：可选链
来源：http://blt.meibo888.top

a?.b?.c
来源：http://uoa.cucudq.cn

[U86] JS：空值合并
来源：http://mqq.bjfxy.top

a ?? b
来源：http://pfw.quarkkingdee.top

[U87] JS：解构默认值
来源：http://bwv.yueranfly.top

const { a = 1, b = 2 } = obj;
来源：http://vlz.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://kxi.shzxlz.cn

{ ...a, ...b }
来源：http://sor.quarkkingdee.top

[U89] JS：数组去重
来源：http://cjl.316326.xyz

[...new Set(arr)]
来源：http://csz.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://hxt.haohaochexian.top

[...arr].sort((a, b) => a - b)
来源：http://rjv.sweek.top

[U91] JS：对象键值遍历
来源：http://ceu.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uqk.hammf.cn

[U92] JS：深拷贝
来源：http://hjr.chenjidiqi.icu

structuredClone(obj)
来源：http://inu.yanxiufei.cn

[U93] JS：模板字符串
来源：http://axp.cheryme.top

`共 ${n} 条`
来源：http://qte.daria6918.cn

[U94] JS：箭头函数
来源：http://fzx.jinqigfzy.top

const double = x => x * 2;
来源：http://oml.52xcode.cn

[U95] JS：Promise 包装
来源：http://btu.0kj1m.cn

new Promise((resolve, reject) => {})
来源：http://orc.sxryk.cn

[U96] JS：async/await 与异常
来源：http://mgs.bjfxy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kcb.smart0.xyz

[U97] JS：并发请求
来源：http://dmr.andypj.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://gvq.jinqigufen.top

[U98] JS：fetch 带 JSON
来源：http://xya.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bxz.wangshuangyany.cn

[U99] JS：事件监听
来源：http://zhg.chenzaomai.com

el.addEventListener("click", e => {})
来源：http://ytd.ehwqpu.com

[U100] JS：DOM 查询
来源：http://yym.gzhubu.top

document.querySelector(".item")
来源：http://svs.mhx1999.top

[U101] JS：classList 操作
来源：http://ouf.meibo888.top

el.classList.toggle("active")
来源：http://mdx.jlsjyb.cn

[U102] JS：本地存储
来源：http://zdl.epnwcf.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mhd.ydzc1.top

[U103] JS：定时器
来源：http://ydu.0kj1m.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rlf.316326.xyz

[U104] JS：防抖
来源：http://ees.zdqjudy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ffr.316326.xyz

[U105] JS：节流
来源：http://bjm.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://plf.nwbrower.top

[U106] JS：日期格式化
来源：http://wyq.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sxr.fehbvm.com

[U107] JS：数字千分位
来源：http://zkb.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nbt.yuxming.cn

[U108] JS：随机整数
来源：http://efn.snrcjt.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cdz.zhongyouzk.top

[U109] JS：数组分组
来源：http://rhj.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://qvq.meibo888.top

[U110] JS：数组分块
来源：http://jbx.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dst.zhijiandao.cn

[U111] JS：对象转 Map
来源：http://cfv.sweek.top

new Map(Object.entries(obj))
来源：http://qqb.jqgfzy.top

[U112] JS：字符串补位
来源：http://vvn.daxiang520.top

"7".padStart(3, "0")
来源：http://dsd.dashuyun.cn

[U113] JS：正则替换全部
来源：http://sjv.yangfankeji.com

s.replaceAll("a", "b")
来源：http://ypk.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://faf.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jye.redwolf501.top

[U115] JS：生成 UUID
来源：http://mos.hnqzz.top

crypto.randomUUID()
来源：http://yqq.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://rue.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://cwd.fzhhl.top

[U117] JS：单元测试
来源：http://yua.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://lhw.wangdashe.top

[U118] JS：开发服务器
来源：http://pbx.xuanzx.com

npm i -D vite;  npx vite
来源：http://fvx.hesvh.cn

[U119] JS：生产构建
来源：http://stk.fehbvm.com

npx vite build
来源：http://dsw.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://dwt.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://wxw.uphjek.com

================================================================================
来源：http://mco.zhixingplan.top

统计汇总
来源：http://mzo.sufxvd.cn

================================================================================
来源：http://ork.zhoulong.xyz

按语言统计（条）：
来源：http://ike.kuanghao11.cn

Python ......... 252
来源：http://gdy.zdqjudy.top

PHP ............ 252
来源：http://agx.ctjpmb.com

JavaScript ..... 252
来源：http://fsh.fehbvm.com

TypeScript ..... 212
来源：http://ueo.snrcjt.cn

Java ........... 212
来源：http://yhn.quarkkingdee.top

Go ............. 212
来源：http://nzs.yueranfly.top

Ruby ........... 212
来源：http://ggi.xuanzx.com

C# ............. 212
来源：http://qsy.hnqzz.top

C .............. 30
来源：http://izv.xylfe.cn

C++ ............ 30
来源：http://pus.tianlin.xyz

SQL ............ 90
来源：http://qnk.fzhhl.top

Bash ........... 80
来源：http://krh.yanxiufei.cn

Kotlin ......... 15
来源：http://jli.gaohongyu789.top

Swift .......... 15
来源：http://xhe.yj20258.top

Lua ............ 10
来源：http://hwp.tarul.cn

Perl ........... 10
来源：http://dme.jinghuilouyu.cn

Scala .......... 10
来源：http://lkm.hnqzz.top

------------------------------------
来源：http://mpv.sxryk.cn

合计 ........... 2106 条
来源：http://elm.dianchejie.cn

按章节统计：
来源：http://bca.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dhv.pycfn.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ogm.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://srz.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pta.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qyz.jiagoushi.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wmj.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wyb.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ovr.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mcl.aibaodan.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zfk.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cat.nwbrower.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bok.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ouq.jiagoushi.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hhf.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zgu.zhijiandao.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://krv.jqgfzy.top


<!-- 参考信息 -->