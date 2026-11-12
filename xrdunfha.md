代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://htr.uphjek.com

[T51] Scala：Hello World
来源：http://ugi.ywan-chungtsiang.top

println("Hello")
来源：http://aqc.yonumen.top

[T52] Scala：变量
来源：http://hmj.gotoacloud.top

val a = 1;  var b = 2
来源：http://opv.pycfn.com

[T53] Scala：字符串插值
来源：http://pin.shzxlz.cn

s"值: $b"
来源：http://uay.kuanghao11.cn

[T54] Scala：集合映射
来源：http://qhd.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://jzz.bbcook.cn

[T55] Scala：集合过滤
来源：http://kmk.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://ats.tianlin.xyz

[T56] Scala：样例类
来源：http://mbb.ybcxt.top

case class User(name: String, age: Int)
来源：http://tgx.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://qod.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xun.cheryme.top

[T58] Scala：函数定义
来源：http://itd.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://cbu.bbcook.cn

[T59] Scala：循环
来源：http://nck.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://alg.sxryk.cn

[T60] Scala：折叠
来源：http://nxu.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fth.ybcxt.top

================================================================================
来源：http://fqw.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gvu.epnwcf.com

================================================================================
来源：http://qqg.yonumen.top

[U01] Py：创建虚拟环境
来源：http://ivz.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://blw.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://zyz.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mna.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://fer.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vqm.yuanzhike.top

[U04] Py：变量调试打印
来源：http://dnn.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://voz.c1oappe.top

[U05] Py：列表去重且保序
来源：http://dzl.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://rnd.cashguo.top

[U06] Py：合并两个字典
来源：http://adp.wangshuangyany.cn

{**a, **b}
来源：http://elx.xylfe.cn

[U07] Py：反转字典键值
来源：http://asy.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://xvv.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://fsx.ybcxt.top

[y for x in nested for y in x]
来源：http://rtm.316326.xyz

[U09] Py：字典取最大值的键
来源：http://lgs.xylfe.cn

max(d, key=d.get)
来源：http://tvo.redwolf501.top

[U10] Py：按值排序字典
来源：http://kdv.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fve.bjfxy.top

[U11] Py：生成器表达式
来源：http://jxe.52xcode.cn

(x * 2 for x in arr)
来源：http://qpc.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://zyp.chenzaomai.com

Counter(arr).most_common(3)
来源：http://nwk.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://nyb.shangyingyoupin.top

deque(maxlen=10)
来源：http://bnh.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://jyl.zhengqikj.top

defaultdict(list)
来源：http://lur.sxryk.cn

[U15] Py：高精度计时
来源：http://nrq.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://mnl.xinyue.icu

[U16] Py：命令行参数解析
来源：http://ifl.9152youxi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://son.aibaodan.cn

[U17] Py：初始化日志
来源：http://nvo.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://gde.jinqigfzy.top

[U18] Py：预编译正则
来源：http://xak.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://pzd.yj202588.top

[U19] Py：正则替换带回调
来源：http://vnh.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jvx.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://lhk.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://agz.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://qmq.yueranfly.top

@contextlib.contextmanager
来源：http://gjf.hesvh.cn

[U22] Py：矩阵转置
来源：http://gvs.daxiang520.top

list(zip(*m))
来源：http://cwa.fzhhl.top

[U23] Py：分块读取大文件
来源：http://gxd.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://scl.meibo888.top

[U24] Py：路径操作
来源：http://zhb.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jmc.316326.xyz

[U25] Py：CSV 按字典读
来源：http://vdb.yfazqb.com

csv.DictReader(f)
来源：http://ukg.smart0.xyz

[U26] Py：并发下载
来源：http://oif.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hxg.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://shn.tian-w.cn

aiohttp.ClientSession() 配合 async with
来源：http://cjo.tianlin.xyz

[U28] Py：类型别名
来源：http://cun.xingfuxueyuan.xyz

UserId = int
来源：http://hzt.guowangkeji.top

[U29] Py：属性校验
来源：http://tcw.yangfankeji.com

@property 与 @x.setter 配合
来源：http://aji.fengsongda.top

[U30] Py：数据类
来源：http://lgn.yangfankeji.com

@dataclass(slots=True)
来源：http://gic.yuxming.cn

[U31] Py：单测
来源：http://cvn.zhoulong.xyz

python -m pytest -q
来源：http://erp.bjfxy.top

[U32] Py：代码格式化
来源：http://byv.c1oappe.top

ruff format . && ruff check --fix .
来源：http://trx.9152youxi.cn

[U33] Py：打包发布
来源：http://npj.daxiang520.top

python -m build  （依赖 pyproject.toml）
来源：http://iac.hywenlv.cn

[U34] Py：判断编码
来源：http://ztb.zdbjq.cn

chardet.detect(raw)
来源：http://cmd.ywan-chungtsiang.top

[U35] Py：发送邮件
来源：http://zbq.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hom.xziqi.cn

[U36] Py：定时任务
来源：http://uog.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://cyd.vehdjk.com

[U37] Py：读写 Excel
来源：http://vyu.ybcxt.top

pandas.read_excel / DataFrame.to_excel
来源：http://nop.yj20258888.top

[U38] Py：获取脚本所在目录
来源：http://xul.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://qjk.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://djp.yonumen.top

sys.stdout.isatty()
来源：http://lsp.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://yik.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://pun.aibaodan.cn

[U41] PHP：初始化 Composer 项目
来源：http://orj.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cmb.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://gdo.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vvu.jyoumei.cn

[U43] PHP：声明命名空间
来源：http://upy.daria6918.cn

namespace App\Http;
来源：http://ykq.daxiang520.top

[U44] PHP：开启严格类型
来源：http://xfn.yvedp.cn

declare(strict_types=1);
来源：http://lfd.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://zcw.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gde.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://yva.aibaodan.cn

?string $name = null
来源：http://hhv.0kj1m.cn

[U47] PHP：联合类型
来源：http://mnw.yuxming.cn

int|string $id
来源：http://gmg.bjfxy.top

[U48] PHP：纯枚举
来源：http://pdc.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://omo.gotoacloud.top

[U49] PHP：只读属性
来源：http://cnx.svipenyu.cn

public readonly string $name
来源：http://kia.chenjidiqi.icu

[U50] PHP：构造器属性提升
来源：http://cgr.316326.xyz

public function __construct(private int $id) {}
来源：http://kfj.zhijiandao.cn

[U51] PHP：数组解构
来源：http://amv.zhijiandao.cn

[$a, $b] = $arr;
来源：http://sce.fktsv.cn

[U52] PHP：箭头函数
来源：http://twy.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://xmx.gotoacloud.top

[U53] PHP：空合并运算符
来源：http://nwf.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://kaw.sufxvd.cn

[U54] PHP：空安全调用
来源：http://xxg.ehwqpu.com

$obj?->method()
来源：http://yze.yueranfly.top

[U55] PHP：match 表达式
来源：http://mfw.ppjwa.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qkq.quarkkingdee.top

[U56] PHP：命名参数
来源：http://yno.havefunace.top

f(a: 1, b: 2)
来源：http://pde.yj20258.top

[U57] PHP：字符串插值
来源：http://fem.yvedp.cn

"值: {$a}"
来源：http://aez.gzhubu.top

[U58] PHP：数组三件套
来源：http://xgd.sxryk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tme.daria6918.cn

[U59] PHP：自定义排序
来源：http://har.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ujx.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://bix.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mpt.nanxinkj.top

[U61] PHP：正则
来源：http://kpw.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wlk.zhixingplan.top

[U62] PHP：日期对象
来源：http://myv.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rhw.hcnkem.com

[U63] PHP：文件读写
来源：http://akx.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rrh.fktsv.cn

[U64] PHP：目录遍历
来源：http://jvr.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://nmz.jyoumei.cn

[U65] PHP：会话
来源：http://dkf.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ioo.yonumen.top

[U66] PHP：设置 Cookie
来源：http://tgd.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dnu.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://imj.shanyushiyangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://msz.fanxiaobao.xyz

[U68] PHP：PDO 连接
来源：http://wnv.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qoo.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://ntv.shanyushiyangtech.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nho.bbcook.cn

[U70] PHP：PDO 事务
来源：http://sxd.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wpm.yj20258.top

[U71] PHP：抛出异常
来源：http://mzv.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://llc.jinqigfzy.top

[U72] PHP：写错误日志
来源：http://tzi.xinyue.icu

error_log("失败: " . $e->getMessage());
来源：http://vjc.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://djd.havefunace.top

parse_ini_file("config.ini", true)
来源：http://fmg.yonumen.top

[U74] PHP：读取环境变量
来源：http://hlc.vehdjk.com

getenv("APP_ENV") ?: "production"
来源：http://ndw.zhoulong.xyz

[U75] PHP：依赖注入
来源：http://uky.shuidangran.top

composer require psr/container
来源：http://gxv.zdbjq.cn

[U76] PHP：简单路由
来源：http://avb.hywenlv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zwy.tianlin.xyz

[U77] PHP：模板渲染
来源：http://ahp.xuanzx.com

composer require twig/twig
来源：http://hyq.cashguo.top

[U78] PHP：单元测试
来源：http://qrz.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://ncw.xylfe.cn

[U79] PHP：静态分析
来源：http://bav.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://ucg.sweek.top

[U80] PHP：代码规范修复
来源：http://mwi.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ban.yj202588.top

[U81] JS：初始化项目
来源：http://fbk.yuanzhike.top

npm init -y;  npm i express
来源：http://cqj.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://izo.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hxj.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://bxa.jqgfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://uqj.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://aqf.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://kft.shuidangran.top

[U85] JS：可选链
来源：http://jbz.svipenyu.cn

a?.b?.c
来源：http://euc.pycfn.com

[U86] JS：空值合并
来源：http://ttq.andypj.xyz

a ?? b
来源：http://bwi.shanyushiyangkeji.top

[U87] JS：解构默认值
来源：http://uag.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://kdu.cashguo.top

[U88] JS：对象展开合并
来源：http://vwd.ehwqpu.com

{ ...a, ...b }
来源：http://yru.svipenyu.cn

[U89] JS：数组去重
来源：http://rvc.gaohongyu789.top

[...new Set(arr)]
来源：http://nxe.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://qbm.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://ydt.jianghu66.top

[U91] JS：对象键值遍历
来源：http://non.hnxiangtu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tpe.chenzaomai.com

[U92] JS：深拷贝
来源：http://dpj.hnqzz.top

structuredClone(obj)
来源：http://dhw.ctjpmb.com

[U93] JS：模板字符串
来源：http://ddl.dianchejie.cn

`共 ${n} 条`
来源：http://eld.pycfn.com

[U94] JS：箭头函数
来源：http://jmt.yfazqb.com

const double = x => x * 2;
来源：http://aui.yvedp.cn

[U95] JS：Promise 包装
来源：http://smw.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://ifu.zhixingplan.top

[U96] JS：async/await 与异常
来源：http://ysu.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://itb.andypj.xyz

[U97] JS：并发请求
来源：http://nnx.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tzu.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://qda.jianghu66.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zfp.zhengqikj.top

[U99] JS：事件监听
来源：http://bqu.cucudq.cn

el.addEventListener("click", e => {})
来源：http://xhq.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://zls.daxiang520.top

document.querySelector(".item")
来源：http://elq.sufxvd.cn

[U101] JS：classList 操作
来源：http://qpg.jinqigfzy.top

el.classList.toggle("active")
来源：http://phy.ivvv.top

[U102] JS：本地存储
来源：http://feg.ctjpmb.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://hjh.ctjpmb.com

[U103] JS：定时器
来源：http://cpl.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bnf.vqdsnc.cn

[U104] JS：防抖
来源：http://gcx.c1oappe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkf.hammf.cn

[U105] JS：节流
来源：http://drs.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eas.zhengqikj.top

[U106] JS：日期格式化
来源：http://fdx.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zhd.c1oappe.top

[U107] JS：数字千分位
来源：http://ubg.guannengcc.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pst.zdbjq.cn

[U108] JS：随机整数
来源：http://wzg.daxiang520.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ukz.9152youxi.cn

[U109] JS：数组分组
来源：http://ity.ybcxt.top

Object.groupBy(arr, x => x.type)
来源：http://biw.ybcxt.top

[U110] JS：数组分块
来源：http://qfz.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://eqo.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://mbw.hcnkem.com

new Map(Object.entries(obj))
来源：http://pps.tianlin.xyz

[U112] JS：字符串补位
来源：http://dkp.zhongyouzk.top

"7".padStart(3, "0")
来源：http://tri.nanxuanxn.top

[U113] JS：正则替换全部
来源：http://vsn.hesvh.cn

s.replaceAll("a", "b")
来源：http://epa.cucudq.cn

[U114] JS：JSON 深比较
来源：http://zqz.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mtj.xingfuxueyuan.xyz

[U115] JS：生成 UUID
来源：http://zme.0kj1m.cn

crypto.randomUUID()
来源：http://ubk.hnxiangtu.top

[U116] JS：类型检查（JSDoc）
来源：http://nws.dashuyun.cn

/** @param {string} name */ function f(name) {}
来源：http://tnq.zycfv.cn

[U117] JS：单元测试
来源：http://joy.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://opt.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://sim.xylfe.cn

npm i -D vite;  npx vite
来源：http://vrl.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://keo.meibo888.top

npx vite build
来源：http://cof.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://upc.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://vkk.nwbrower.top

================================================================================
来源：http://mhx.xingfuxueyuan.xyz

统计汇总
来源：http://cnw.bjfxy.top

================================================================================
来源：http://nmh.redwolf501.top

按语言统计（条）：
来源：http://smb.vqdsnc.cn

Python ......... 252
来源：http://bph.aizwys.cn

PHP ............ 252
来源：http://uyv.fengsongda.top

JavaScript ..... 252
来源：http://lun.jinghuilouyu.cn

TypeScript ..... 212
来源：http://tts.jiagoushi.top

Java ........... 212
来源：http://yam.316326.xyz

Go ............. 212
来源：http://cdm.0kj1m.cn

Ruby ........... 212
来源：http://zib.yongpay.top

C# ............. 212
来源：http://cdo.fanxiaobao.xyz

C .............. 30
来源：http://fac.jianghu66.top

C++ ............ 30
来源：http://rfm.316326.xyz

SQL ............ 90
来源：http://xpy.wangdashe.top

Bash ........... 80
来源：http://dtv.vqdsnc.cn

Kotlin ......... 15
来源：http://cot.gzhubu.top

Swift .......... 15
来源：http://mne.nanxinkj.top

Lua ............ 10
来源：http://ujc.nanxuanxn.top

Perl ........... 10
来源：http://ugz.hongshengwenyu.top

Scala .......... 10
来源：http://jmw.kuanghao11.cn

------------------------------------
来源：http://eck.bjfxy.top

合计 ........... 2106 条
来源：http://pfy.tarul.cn

按章节统计：
来源：http://nij.andypj.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://fzf.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pjs.uphjek.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hub.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://acv.zhixingplan.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kmd.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sjx.zhixingplan.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gur.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oyj.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kei.jqgufenzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://plz.uphjek.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pzo.sxryk.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ltl.yonumen.top


<!-- 参考信息 -->