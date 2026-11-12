代发 wailian999

case class User(name: String, age: Int)
来源：http://ddu.jinqigufen.top

[T57] Scala：模式匹配
来源：http://rdr.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rpq.nanxinkj.top

[T58] Scala：函数定义
来源：http://nma.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://hld.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://iyq.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://xbi.bbcook.cn

[T60] Scala：折叠
来源：http://dme.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hyu.yangfankeji.com

================================================================================
来源：http://exh.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ubs.hysaishi.cn

================================================================================
来源：http://gyq.52xcode.cn

[U01] Py：创建虚拟环境
来源：http://vij.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nfr.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://qqk.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vhh.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://hjc.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://azs.gotoacloud.top

[U04] Py：变量调试打印
来源：http://tag.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oes.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://kia.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://yfy.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://jei.yj20258.top

{**a, **b}
来源：http://xok.hnqzz.top

[U07] Py：反转字典键值
来源：http://wcc.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://ndi.fktsv.cn

[U08] Py：展平二维列表
来源：http://lom.gogol.net.cn

[y for x in nested for y in x]
来源：http://hnl.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://yul.yfazqb.com

max(d, key=d.get)
来源：http://vcw.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://ebg.sysykeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zzi.pycfn.com

[U11] Py：生成器表达式
来源：http://umf.havefunace.top

(x * 2 for x in arr)
来源：http://wws.chenjidiqi.icu

[U12] Py：取出现最多的 3 个元素
来源：http://skj.zdqjudy.top

Counter(arr).most_common(3)
来源：http://dwm.aizwys.cn

[U13] Py：固定长度队列
来源：http://ajo.zhijiandao.cn

deque(maxlen=10)
来源：http://igg.316326.xyz

[U14] Py：分组收集到列表
来源：http://yog.ehwqpu.com

defaultdict(list)
来源：http://bcr.vqdsnc.cn

[U15] Py：高精度计时
来源：http://qzc.fktsv.cn

t = time.perf_counter()
来源：http://msd.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://nef.zhengqikj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://taw.hnxiangtu.top

[U17] Py：初始化日志
来源：http://hbz.kuanghao11.cn

logging.basicConfig(level=logging.INFO)
来源：http://tuf.daxiang520.top

[U18] Py：预编译正则
来源：http://rkz.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://atd.hnxiangtu.top

[U19] Py：正则替换带回调
来源：http://sdf.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tvw.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://gle.snrcjt.cn

@functools.lru_cache(maxsize=None)
来源：http://pbo.iojbl.cn

[U21] Py：自定义上下文管理器
来源：http://zgi.ybcxt.top

@contextlib.contextmanager
来源：http://eyp.jianghu66.top

[U22] Py：矩阵转置
来源：http://utl.hammf.cn

list(zip(*m))
来源：http://gpq.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://klm.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bqu.yonumen.top

[U24] Py：路径操作
来源：http://xmh.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zcp.havefunace.top

[U25] Py：CSV 按字典读
来源：http://wis.xinyue.icu

csv.DictReader(f)
来源：http://dsh.zhongyouzk.top

[U26] Py：并发下载
来源：http://mml.andypj.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hqa.snrcjt.cn

[U27] Py：异步 HTTP
来源：http://kze.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://utn.shangyingyoupin.top

[U28] Py：类型别名
来源：http://pph.sweek.top

UserId = int
来源：http://aww.mhx1999.top

[U29] Py：属性校验
来源：http://wbk.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://sqs.uphjek.com

[U30] Py：数据类
来源：http://qzr.ybcxt.top

@dataclass(slots=True)
来源：http://etk.bjfxy.top

[U31] Py：单测
来源：http://ydn.nwbrower.top

python -m pytest -q
来源：http://bqw.smart0.xyz

[U32] Py：代码格式化
来源：http://pfz.ydzc1.top

ruff format . && ruff check --fix .
来源：http://lun.sjlbkw.cn

[U33] Py：打包发布
来源：http://qup.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://haw.pengpengdd.cyou

[U34] Py：判断编码
来源：http://dlo.ctjpmb.com

chardet.detect(raw)
来源：http://obq.jlsjyb.cn

[U35] Py：发送邮件
来源：http://mqs.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pbk.yangfankeji.com

[U36] Py：定时任务
来源：http://mzz.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://ymt.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://nbt.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://zle.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://xne.smart0.xyz

Path(__file__).resolve().parent
来源：http://fdz.gzhubu.top

[U39] Py：判断是否在交互环境
来源：http://wjt.c1oappe.top

sys.stdout.isatty()
来源：http://nks.nwbrower.top

[U40] Py：打印到标准错误
来源：http://ous.tianlin.xyz

print("err", file=sys.stderr)
来源：http://vob.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://cbg.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gto.yj20258.top

[U42] PHP：PSR-4 自动加载
来源：http://kdp.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ijz.havefunace.top

[U43] PHP：声明命名空间
来源：http://ofz.hongshengwenyu.top

namespace App\Http;
来源：http://vrp.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://qot.ivvv.top

declare(strict_types=1);
来源：http://mhz.gaohongyu789.top

[U45] PHP：类型声明与返回类型
来源：http://arw.zhengqikj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://uqd.yj20258888.top

[U46] PHP：可空类型
来源：http://tkn.yj20258888.top

?string $name = null
来源：http://lke.tanke756.top

[U47] PHP：联合类型
来源：http://hld.zhongyouzk.top

int|string $id
来源：http://mac.fzhhl.top

[U48] PHP：纯枚举
来源：http://sfw.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://etf.snrcjt.cn

[U49] PHP：只读属性
来源：http://yse.shzxlz.cn

public readonly string $name
来源：http://vbx.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://mgt.nanxinkj.top

public function __construct(private int $id) {}
来源：http://pcq.yueranfly.top

[U51] PHP：数组解构
来源：http://mah.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://soh.dashuyun.cn

[U52] PHP：箭头函数
来源：http://lyr.hnqzz.top

$double = fn($x) => $x * 2;
来源：http://xfr.jqgufenzy.top

[U53] PHP：空合并运算符
来源：http://eku.pengpengdd.cyou

$v = $a ?? $b ?? "default";
来源：http://hhr.ctjpmb.com

[U54] PHP：空安全调用
来源：http://jgm.jinqigfzy.top

$obj?->method()
来源：http://uwd.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://pbh.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wbr.chenlongwang.top

[U56] PHP：命名参数
来源：http://fvz.gaohongyu789.top

f(a: 1, b: 2)
来源：http://ecx.redwolf501.top

[U57] PHP：字符串插值
来源：http://dbh.sufxvd.cn

"值: {$a}"
来源：http://mnd.yongpay.top

[U58] PHP：数组三件套
来源：http://vnh.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://flo.jqgufenzy.top

[U59] PHP：自定义排序
来源：http://usd.jqgufenzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hhb.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://mow.hfpthk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ldd.jianghu66.top

[U61] PHP：正则
来源：http://hvr.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://khy.pycfn.com

[U62] PHP：日期对象
来源：http://tsx.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ukk.zhixingplan.top

[U63] PHP：文件读写
来源：http://jar.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://azs.yangfankeji.com

[U64] PHP：目录遍历
来源：http://axj.ppjwa.cn

glob("dir/*.php");  scandir("dir");
来源：http://hfl.zhengqikj.top

[U65] PHP：会话
来源：http://tif.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qls.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://okw.yfazqb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fcx.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://juf.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rlt.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://guv.pycfn.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ahd.bjfxy.top

[U69] PHP：PDO 预处理
来源：http://kxm.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zfk.52xcode.cn

[U70] PHP：PDO 事务
来源：http://avo.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://obi.jinqigufen.top

[U71] PHP：抛出异常
来源：http://ygr.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://rvn.yj202588.top

[U72] PHP：写错误日志
来源：http://sci.shanyushiyangkeji.top

error_log("失败: " . $e->getMessage());
来源：http://kyi.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://ibq.gogol.net.cn

parse_ini_file("config.ini", true)
来源：http://yjt.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://fou.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://nft.redwolf501.top

[U75] PHP：依赖注入
来源：http://cvt.chenlongwang.top

composer require psr/container
来源：http://gwa.xylfe.cn

[U76] PHP：简单路由
来源：http://blf.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rsb.316326.xyz

[U77] PHP：模板渲染
来源：http://kmx.jyoumei.cn

composer require twig/twig
来源：http://qzu.nwbrower.top

[U78] PHP：单元测试
来源：http://mdl.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://ump.daria6918.cn

[U79] PHP：静态分析
来源：http://yut.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://uoh.epnwcf.com

[U80] PHP：代码规范修复
来源：http://dzl.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iis.jinqigfzy.top

[U81] JS：初始化项目
来源：http://zoh.andypj.xyz

npm init -y;  npm i express
来源：http://vhy.vehdjk.com

[U82] JS：package.json 脚本
来源：http://rbw.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wug.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://udv.9152youxi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zyd.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://goa.dianchejie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zum.9152youxi.cn

[U85] JS：可选链
来源：http://gqj.ydjk.org.cn

a?.b?.c
来源：http://fmm.hywenlv.cn

[U86] JS：空值合并
来源：http://chb.andypj.xyz

a ?? b
来源：http://yqr.jiagoushi.top

[U87] JS：解构默认值
来源：http://rqi.ybcxt.top

const { a = 1, b = 2 } = obj;
来源：http://dpb.xinyue.icu

[U88] JS：对象展开合并
来源：http://sts.cheryme.top

{ ...a, ...b }
来源：http://hje.aibaodan.cn

[U89] JS：数组去重
来源：http://vhp.haohaochexian.top

[...new Set(arr)]
来源：http://ogy.yfazqb.com

[U90] JS：数字数组排序
来源：http://odl.xuetiantiany.cn

[...arr].sort((a, b) => a - b)
来源：http://vys.xylfe.cn

[U91] JS：对象键值遍历
来源：http://hug.gzhubu.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uml.zhixingplan.top

[U92] JS：深拷贝
来源：http://uji.xingfuxueyuan.xyz

structuredClone(obj)
来源：http://dto.zhoulong.xyz

[U93] JS：模板字符串
来源：http://tfh.hysaishi.cn

`共 ${n} 条`
来源：http://tnr.pycfn.com

[U94] JS：箭头函数
来源：http://lgh.zhiwuduotai.top

const double = x => x * 2;
来源：http://hzw.jinghuilouyu.cn

[U95] JS：Promise 包装
来源：http://tqo.feifeiyinyue.top

new Promise((resolve, reject) => {})
来源：http://dvu.tian-w.cn

[U96] JS：async/await 与异常
来源：http://jgx.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cpe.dianchejie.cn

[U97] JS：并发请求
来源：http://upo.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://iqg.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://bac.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iuv.ybcxt.top

[U99] JS：事件监听
来源：http://vqe.guowangkeji.top

el.addEventListener("click", e => {})
来源：http://nlo.jinyuanbaomall.cn

[U100] JS：DOM 查询
来源：http://bff.xuanzx.com

document.querySelector(".item")
来源：http://wpe.xingfuxueyuan.xyz

[U101] JS：classList 操作
来源：http://nkd.feifeiyinyue.top

el.classList.toggle("active")
来源：http://snm.zhaomingkeji.xyz

[U102] JS：本地存储
来源：http://mse.aizwys.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rnl.hongshengwenyu.top

[U103] JS：定时器
来源：http://tlu.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://cxy.zhaomingkeji.xyz

[U104] JS：防抖
来源：http://oow.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ncq.yj202588.top

[U105] JS：节流
来源：http://poc.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jeh.tarul.cn

[U106] JS：日期格式化
来源：http://uaf.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sbr.yangfankeji.com

[U107] JS：数字千分位
来源：http://osc.ydzc1.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://opg.hfpthk.cn

[U108] JS：随机整数
来源：http://nrn.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qee.yvedp.cn

[U109] JS：数组分组
来源：http://xwk.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://gle.hnqzz.top

[U110] JS：数组分块
来源：http://ggi.shzxlz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cwx.xylfe.cn

[U111] JS：对象转 Map
来源：http://wmv.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://scy.52xcode.cn

[U112] JS：字符串补位
来源：http://qlf.9152youxi.cn

"7".padStart(3, "0")
来源：http://via.hysaishi.cn

[U113] JS：正则替换全部
来源：http://tao.yueranfly.top

s.replaceAll("a", "b")
来源：http://gai.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://agt.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wzy.tanke756.top

[U115] JS：生成 UUID
来源：http://bvq.jianghu66.top

crypto.randomUUID()
来源：http://gfw.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://kht.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://rmx.tian-w.cn

[U117] JS：单元测试
来源：http://hjf.meibo888.top

npm i -D vitest;  npx vitest
来源：http://bjb.wangshuangyany.cn

[U118] JS：开发服务器
来源：http://jcs.meibo888.top

npm i -D vite;  npx vite
来源：http://pio.xuanzx.com

[U119] JS：生产构建
来源：http://xfh.hongshengwenyu.top

npx vite build
来源：http://drb.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://avw.316326.xyz

import.meta.env.VITE_API_URL
来源：http://sew.guannengcc.top

================================================================================
来源：http://izn.shanyushiyangtech.top

统计汇总
来源：http://fhu.bjfxy.top

================================================================================
来源：http://dxv.yonumen.top

按语言统计（条）：
来源：http://yqu.nwbrower.top

Python ......... 252
来源：http://bwi.tian-w.cn

PHP ............ 252
来源：http://lza.hammf.cn

JavaScript ..... 252
来源：http://jzj.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://atk.yfazqb.com

Java ........... 212
来源：http://xyq.chenlongwang.top

Go ............. 212
来源：http://xoi.hcnkem.com

Ruby ........... 212
来源：http://frl.vqdsnc.cn

C# ............. 212
来源：http://mfj.yj20258888.top

C .............. 30
来源：http://odg.ydzc1.top

C++ ............ 30
来源：http://ebf.yuxming.cn

SQL ............ 90
来源：http://rvz.jiagoushi.top

Bash ........... 80
来源：http://fjl.shzxlz.cn

Kotlin ......... 15
来源：http://pon.dashuyun.cn

Swift .......... 15
来源：http://wse.yfazqb.com

Lua ............ 10
来源：http://eik.sysykeji.top

Perl ........... 10
来源：http://zaf.yanxiufei.cn

Scala .......... 10
来源：http://lsv.hcnkem.com

------------------------------------
来源：http://fit.shanyushiyangkeji.top

合计 ........... 2106 条
来源：http://rzd.gogol.net.cn

按章节统计：
来源：http://rfn.uphjek.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pwp.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ujh.ehwqpu.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kkl.vqdsnc.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bqz.feifeiyinyue.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fkr.yj202588.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ddd.yuanzhike.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sca.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vti.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://osw.fktsv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dkb.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tfs.yj202588.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ptz.jyoumei.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cog.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jrc.vqdsnc.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dyg.ctjpmb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vwn.nanxuanxn.top

Q SQL 专题                              90
来源：http://mvo.316326.xyz

R Bash 专题                             80
来源：http://hsw.hammf.cn

S C / C++ 专题                          60
来源：http://zkl.xingfuxueyuan.xyz

T 其他语言补充                          60
来源：http://eyg.nwbrower.top

U 高频实用片段                         120
来源：http://rku.0kj1m.cn

------------------------------------
来源：http://mux.0kj1m.cn

合计                                  2106 条
来源：http://vsj.fengsongda.top

--------------------------------------------------------------------------------
来源：http://lua.tarul.cn


<!-- 参考信息 -->