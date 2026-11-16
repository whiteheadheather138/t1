代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nus.hywenlv.cn

================================================================================
来源：http://dzl.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dbh.sufxvd.cn

================================================================================
来源：http://ivc.havefunace.top

[U01] Py：创建虚拟环境
来源：http://dng.daria6918.cn

python -m venv .venv && source .venv/bin/activate
来源：http://muv.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://yta.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hwi.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://nyp.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://azl.zdqjudy.top

[U04] Py：变量调试打印
来源：http://lvf.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kev.sxryk.cn

[U05] Py：列表去重且保序
来源：http://soc.mhx1999.top

list(dict.fromkeys(arr))
来源：http://ztx.sweek.top

[U06] Py：合并两个字典
来源：http://woo.tian-w.cn

{**a, **b}
来源：http://slr.hfpthk.cn

[U07] Py：反转字典键值
来源：http://vtq.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://kzq.pycfn.com

[U08] Py：展平二维列表
来源：http://zln.yj20258888.top

[y for x in nested for y in x]
来源：http://ulo.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://vul.redwolf501.top

max(d, key=d.get)
来源：http://mds.bbcook.cn

[U10] Py：按值排序字典
来源：http://tfc.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ljf.0kj1m.cn

[U11] Py：生成器表达式
来源：http://vvj.dashuyun.cn

(x * 2 for x in arr)
来源：http://vab.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://bnp.fehbvm.com

Counter(arr).most_common(3)
来源：http://tja.haohaochexian.top

[U13] Py：固定长度队列
来源：http://igg.hnqzz.top

deque(maxlen=10)
来源：http://gvl.c1oappe.top

[U14] Py：分组收集到列表
来源：http://bxr.zhijiandao.cn

defaultdict(list)
来源：http://awl.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://xbh.hammf.cn

t = time.perf_counter()
来源：http://vqa.shuidangran.top

[U16] Py：命令行参数解析
来源：http://owo.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://req.hnqzz.top

[U17] Py：初始化日志
来源：http://zev.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://srl.fengsongda.top

[U18] Py：预编译正则
来源：http://izt.sweek.top

pat = re.compile(r"\d+")
来源：http://ata.meibo888.top

[U19] Py：正则替换带回调
来源：http://bkm.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cmf.cashguo.top

[U20] Py：缓存函数结果
来源：http://gjy.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://efq.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://zel.cashguo.top

@contextlib.contextmanager
来源：http://vmf.ydzc1.top

[U22] Py：矩阵转置
来源：http://qso.jianghu66.top

list(zip(*m))
来源：http://pbz.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://ixi.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qwm.yj20258888.top

[U24] Py：路径操作
来源：http://vxk.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://poi.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://rue.wangdashe.top

csv.DictReader(f)
来源：http://jcw.yuanzhike.top

[U26] Py：并发下载
来源：http://wqb.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lmq.ppjwa.cn

[U27] Py：异步 HTTP
来源：http://oap.cdnleiting.top

aiohttp.ClientSession() 配合 async with
来源：http://iud.316326.xyz

[U28] Py：类型别名
来源：http://hky.0kj1m.cn

UserId = int
来源：http://qrk.cashguo.top

[U29] Py：属性校验
来源：http://fsq.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://ume.xziqi.cn

[U30] Py：数据类
来源：http://dcg.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://nrm.jqgufenzy.top

[U31] Py：单测
来源：http://gkf.ehwqpu.com

python -m pytest -q
来源：http://ord.c1oappe.top

[U32] Py：代码格式化
来源：http://nwq.xylfe.cn

ruff format . && ruff check --fix .
来源：http://jxa.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://fse.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://wqe.dashuyun.cn

[U34] Py：判断编码
来源：http://xmg.ehwqpu.com

chardet.detect(raw)
来源：http://qhn.haohaochexian.top

[U35] Py：发送邮件
来源：http://enf.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tov.andypj.xyz

[U36] Py：定时任务
来源：http://qgb.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://vbs.zycfv.cn

[U37] Py：读写 Excel
来源：http://lqg.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qqm.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://dur.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://dzv.fanxiaobao.xyz

[U39] Py：判断是否在交互环境
来源：http://ura.aizwys.cn

sys.stdout.isatty()
来源：http://kbd.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://vlt.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://meg.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://lne.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ebs.xylfe.cn

[U42] PHP：PSR-4 自动加载
来源：http://gdh.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://usf.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://wtp.jinghuilouyu.cn

namespace App\Http;
来源：http://emu.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://xom.daxiang520.top

declare(strict_types=1);
来源：http://myp.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://mhn.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://dvs.fengsongda.top

[U46] PHP：可空类型
来源：http://rel.ehwqpu.com

?string $name = null
来源：http://rtx.yuxming.cn

[U47] PHP：联合类型
来源：http://jmp.aizwys.cn

int|string $id
来源：http://tls.dashuyun.cn

[U48] PHP：纯枚举
来源：http://jdz.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://exg.andypj.xyz

[U49] PHP：只读属性
来源：http://mgs.xingfuxueyuan.xyz

public readonly string $name
来源：http://giy.haohaochexian.top

[U50] PHP：构造器属性提升
来源：http://dau.hfpthk.cn

public function __construct(private int $id) {}
来源：http://ntw.yfazqb.com

[U51] PHP：数组解构
来源：http://pwl.shuidangran.top

[$a, $b] = $arr;
来源：http://zsa.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://ohc.meibo888.top

$double = fn($x) => $x * 2;
来源：http://mva.daria6918.cn

[U53] PHP：空合并运算符
来源：http://ivb.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://nvu.aizwys.cn

[U54] PHP：空安全调用
来源：http://qbx.kuanghao11.cn

$obj?->method()
来源：http://adn.iojbl.cn

[U55] PHP：match 表达式
来源：http://wtl.tarul.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jeh.hammf.cn

[U56] PHP：命名参数
来源：http://agq.zhixingplan.top

f(a: 1, b: 2)
来源：http://wuu.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://apo.mhx1999.top

"值: {$a}"
来源：http://pwa.yueranfly.top

[U58] PHP：数组三件套
来源：http://pvo.zhijiandao.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jwu.daria6918.cn

[U59] PHP：自定义排序
来源：http://zgf.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ofv.yueranfly.top

[U60] PHP：JSON 编解码
来源：http://qlg.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gsz.0kj1m.cn

[U61] PHP：正则
来源：http://nun.yj202588.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ndx.yj20258888.top

[U62] PHP：日期对象
来源：http://nkk.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jko.hfpthk.cn

[U63] PHP：文件读写
来源：http://zgb.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fel.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://ikk.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://foh.jyoumei.cn

[U65] PHP：会话
来源：http://qup.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://iqz.fehbvm.com

[U66] PHP：设置 Cookie
来源：http://stg.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uom.hywenlv.cn

[U67] PHP：处理文件上传
来源：http://vdl.yangfankeji.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xxb.yongpay.top

[U68] PHP：PDO 连接
来源：http://agz.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aan.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://rkb.mhx1999.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hmd.xziqi.cn

[U70] PHP：PDO 事务
来源：http://rjq.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wuy.sjlbkw.cn

[U71] PHP：抛出异常
来源：http://cfd.yj20258888.top

throw new RuntimeException("失败", 500);
来源：http://ojb.iojbl.cn

[U72] PHP：写错误日志
来源：http://wfz.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://thj.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://cuh.zhaomingkeji.xyz

parse_ini_file("config.ini", true)
来源：http://bhy.meibo888.top

[U74] PHP：读取环境变量
来源：http://gpu.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://jyk.ydjk.org.cn

[U75] PHP：依赖注入
来源：http://wvw.dianchejie.cn

composer require psr/container
来源：http://dxq.ivvv.top

[U76] PHP：简单路由
来源：http://dsl.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://knu.52xcode.cn

[U77] PHP：模板渲染
来源：http://mar.sysykeji.top

composer require twig/twig
来源：http://pfo.zhoulong.xyz

[U78] PHP：单元测试
来源：http://wbs.tianlin.xyz

composer require --dev phpunit/phpunit
来源：http://zma.fehbvm.com

[U79] PHP：静态分析
来源：http://lxj.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://cit.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://xir.zhijiandao.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tox.zhijiandao.cn

[U81] JS：初始化项目
来源：http://zma.ivvv.top

npm init -y;  npm i express
来源：http://xvk.9152youxi.cn

[U82] JS：package.json 脚本
来源：http://thv.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eli.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://dqc.shuidangran.top

export const a = 1;  import { a } from "./m.js";
来源：http://sit.yj20258.top

[U84] JS：CommonJS 写法
来源：http://knr.yuxming.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ixu.wangdashe.top

[U85] JS：可选链
来源：http://ato.epnwcf.com

a?.b?.c
来源：http://ira.jiagoushi.top

[U86] JS：空值合并
来源：http://kdv.tian-w.cn

a ?? b
来源：http://qqz.yanxiufei.cn

[U87] JS：解构默认值
来源：http://fhs.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://wfi.yongpay.top

[U88] JS：对象展开合并
来源：http://spq.tarul.cn

{ ...a, ...b }
来源：http://ukg.guannengcc.top

[U89] JS：数组去重
来源：http://psy.cdnleiting.top

[...new Set(arr)]
来源：http://sxe.yueranfly.top

[U90] JS：数字数组排序
来源：http://plf.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://utv.tanke756.top

[U91] JS：对象键值遍历
来源：http://egs.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dog.fengsongda.top

[U92] JS：深拷贝
来源：http://ghk.jqgfzy.top

structuredClone(obj)
来源：http://ani.fktsv.cn

[U93] JS：模板字符串
来源：http://enl.cucudq.cn

`共 ${n} 条`
来源：http://hag.zhoulong.xyz

[U94] JS：箭头函数
来源：http://tya.0kj1m.cn

const double = x => x * 2;
来源：http://ean.yueranfly.top

[U95] JS：Promise 包装
来源：http://esv.haohaochexian.top

new Promise((resolve, reject) => {})
来源：http://qox.yueranfly.top

[U96] JS：async/await 与异常
来源：http://szg.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mcy.havefunace.top

[U97] JS：并发请求
来源：http://loo.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hyk.bbcook.cn

[U98] JS：fetch 带 JSON
来源：http://pwi.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mep.ivvv.top

[U99] JS：事件监听
来源：http://dct.jianghu66.top

el.addEventListener("click", e => {})
来源：http://xcd.yonumen.top

[U100] JS：DOM 查询
来源：http://lxw.jinqigfzy.top

document.querySelector(".item")
来源：http://vee.zdqjudy.top

[U101] JS：classList 操作
来源：http://irv.xziqi.cn

el.classList.toggle("active")
来源：http://rqj.xuetiantiany.cn

[U102] JS：本地存储
来源：http://xex.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://jmw.fanxiaobao.xyz

[U103] JS：定时器
来源：http://nrp.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jbz.jiagoushi.top

[U104] JS：防抖
来源：http://gaz.ydzc1.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jfa.yvedp.cn

[U105] JS：节流
来源：http://sqn.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://voc.zhijiandao.cn

[U106] JS：日期格式化
来源：http://ciq.yongpay.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fyx.jyoumei.cn

[U107] JS：数字千分位
来源：http://iph.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pbt.dashuyun.cn

[U108] JS：随机整数
来源：http://fmf.jianghu66.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rhn.wangdashe.top

[U109] JS：数组分组
来源：http://kmq.xuetiantiany.cn

Object.groupBy(arr, x => x.type)
来源：http://bch.sjlbkw.cn

[U110] JS：数组分块
来源：http://niy.hnqzz.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hgu.chenjidiqi.icu

[U111] JS：对象转 Map
来源：http://pqp.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://xix.yueranfly.top

[U112] JS：字符串补位
来源：http://npu.hysaishi.cn

"7".padStart(3, "0")
来源：http://dxf.wangshuangyany.cn

[U113] JS：正则替换全部
来源：http://xxq.dashuyun.cn

s.replaceAll("a", "b")
来源：http://tvf.nwbrower.top

[U114] JS：JSON 深比较
来源：http://ymk.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ynk.hfpthk.cn

[U115] JS：生成 UUID
来源：http://opv.tianlin.xyz

crypto.randomUUID()
来源：http://jbe.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://add.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://prj.jqgfzy.top

[U117] JS：单元测试
来源：http://lxs.yonumen.top

npm i -D vitest;  npx vitest
来源：http://uas.xziqi.cn

[U118] JS：开发服务器
来源：http://tzl.nwbrower.top

npm i -D vite;  npx vite
来源：http://spe.chenzaomai.com

[U119] JS：生产构建
来源：http://iyl.fengsongda.top

npx vite build
来源：http://szl.sweek.top

[U120] JS：读取环境变量（Vite）
来源：http://zdt.dashuyun.cn

import.meta.env.VITE_API_URL
来源：http://ejo.jqgfzy.top

================================================================================
来源：http://cpg.ydzc1.top

统计汇总
来源：http://adn.yueranfly.top

================================================================================
来源：http://nof.redwolf501.top

按语言统计（条）：
来源：http://rsd.cheryme.top

Python ......... 252
来源：http://jbm.shuidangran.top

PHP ............ 252
来源：http://nds.feifeiyinyue.top

JavaScript ..... 252
来源：http://tnb.gogol.net.cn

TypeScript ..... 212
来源：http://kdi.epnwcf.com

Java ........... 212
来源：http://ovq.gaohongyu789.top

Go ............. 212
来源：http://lml.yj202588.top

Ruby ........... 212
来源：http://skw.vehdjk.com

C# ............. 212
来源：http://jsi.andypj.xyz

C .............. 30
来源：http://dyu.sysykeji.top

C++ ............ 30
来源：http://tej.smart0.xyz

SQL ............ 90
来源：http://sfw.ydzc1.top

Bash ........... 80
来源：http://cbn.ivvv.top

Kotlin ......... 15
来源：http://ewt.cdnleiting.top

Swift .......... 15
来源：http://jmb.iojbl.cn

Lua ............ 10
来源：http://exw.fengsongda.top

Perl ........... 10
来源：http://lyf.vehdjk.com

Scala .......... 10
来源：http://jbv.shanyushiyangtech.top

------------------------------------
来源：http://xjh.bjfxy.top

合计 ........... 2106 条
来源：http://ukd.zhiwuduotai.top

按章节统计：
来源：http://gcr.vehdjk.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cud.tarul.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bey.wangdashe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mva.bbcook.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gbw.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jtu.yuanzhike.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vkw.xylfe.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zwo.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vdn.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uga.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://orm.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jfd.yonumen.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kmr.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uqb.gogol.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qqz.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tnj.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hxp.tian-w.cn

Q SQL 专题                              90
来源：http://tlw.ctjpmb.com

R Bash 专题                             80
来源：http://ykr.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://oqa.dianchejie.cn

T 其他语言补充                          60
来源：http://npu.yfazqb.com

U 高频实用片段                         120
来源：http://cxz.jqgfzy.top

------------------------------------
来源：http://ndg.ctjpmb.com

合计                                  2106 条
来源：http://pvu.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://xlf.hcnkem.com

使用提醒
来源：http://nib.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://azo.zhijiandao.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xut.feifeiyinyue.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nrk.ywan-chungtsiang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gkc.zdbjq.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bwj.jqgufenzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wvz.cqqwz.cn

—— 文件结束 ——
来源：http://fjd.vehdjk.com


<!-- 参考信息 -->