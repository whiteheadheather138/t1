代发 wailian999

case class User(name: String, age: Int)
来源：http://hzx.ehwqpu.com

[T57] Scala：模式匹配
来源：http://izy.meibo888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sxd.daxiang520.top

[T58] Scala：函数定义
来源：http://kqu.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://gzw.snrcjt.cn

[T59] Scala：循环
来源：http://lbn.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://pru.tanke756.top

[T60] Scala：折叠
来源：http://zst.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gqa.feifeiyinyue.top

================================================================================
来源：http://kqe.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qsw.gotoacloud.top

================================================================================
来源：http://ooq.cashguo.top

[U01] Py：创建虚拟环境
来源：http://lvb.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://fdh.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://gnt.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xji.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://xxd.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hxu.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://pco.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://meo.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://nom.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://cbz.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://jkz.yanxiufei.cn

{**a, **b}
来源：http://mvj.cashguo.top

[U07] Py：反转字典键值
来源：http://mup.c1oappe.top

{v: k for k, v in d.items()}
来源：http://fgc.ctjpmb.com

[U08] Py：展平二维列表
来源：http://wjq.chenjidiqi.icu

[y for x in nested for y in x]
来源：http://zzi.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://rpg.tarul.cn

max(d, key=d.get)
来源：http://abl.jqgfzy.top

[U10] Py：按值排序字典
来源：http://lds.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yno.mhx1999.top

[U11] Py：生成器表达式
来源：http://knr.xylfe.cn

(x * 2 for x in arr)
来源：http://fyr.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hnq.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://lnd.hcnkem.com

[U13] Py：固定长度队列
来源：http://cqw.xuetiantiany.cn

deque(maxlen=10)
来源：http://zct.ehwqpu.com

[U14] Py：分组收集到列表
来源：http://ogl.hnqzz.top

defaultdict(list)
来源：http://erh.kuanghao11.cn

[U15] Py：高精度计时
来源：http://jmn.cashguo.top

t = time.perf_counter()
来源：http://dzx.xinyue.icu

[U16] Py：命令行参数解析
来源：http://gar.gzhubu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rhb.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://cbs.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://ezl.zhixingplan.top

[U18] Py：预编译正则
来源：http://qkm.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://dzi.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://ayp.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://moy.wangdashe.top

[U20] Py：缓存函数结果
来源：http://gzf.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://wkf.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://cnr.meibo888.top

@contextlib.contextmanager
来源：http://xvy.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://ost.epnwcf.com

list(zip(*m))
来源：http://kox.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://bgo.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dwt.ybcxt.top

[U24] Py：路径操作
来源：http://zuc.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vyw.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://pjb.ppjwa.cn

csv.DictReader(f)
来源：http://cef.shuidangran.top

[U26] Py：并发下载
来源：http://scz.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gqy.meibo888.top

[U27] Py：异步 HTTP
来源：http://dmh.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://dwg.zhijiandao.cn

[U28] Py：类型别名
来源：http://clh.birdmap.top

UserId = int
来源：http://kfy.haohaochexian.top

[U29] Py：属性校验
来源：http://nym.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://stz.xuanzx.com

[U30] Py：数据类
来源：http://nkw.haohaochexian.top

@dataclass(slots=True)
来源：http://ccs.daxiang520.top

[U31] Py：单测
来源：http://zej.hnxiangtu.top

python -m pytest -q
来源：http://ycb.zhijiandao.cn

[U32] Py：代码格式化
来源：http://hvx.fktsv.cn

ruff format . && ruff check --fix .
来源：http://mvl.chenzaomai.com

[U33] Py：打包发布
来源：http://glu.gotoacloud.top

python -m build  （依赖 pyproject.toml）
来源：http://qbv.zhiwuduotai.top

[U34] Py：判断编码
来源：http://efo.zdqjudy.top

chardet.detect(raw)
来源：http://bmq.aibaodan.cn

[U35] Py：发送邮件
来源：http://qfo.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tpb.havefunace.top

[U36] Py：定时任务
来源：http://wqz.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://fhq.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://mjj.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eti.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://ioz.dashuyun.cn

Path(__file__).resolve().parent
来源：http://roj.svipenyu.cn

[U39] Py：判断是否在交互环境
来源：http://rac.ctjpmb.com

sys.stdout.isatty()
来源：http://mli.wangdashe.top

[U40] Py：打印到标准错误
来源：http://wyv.daxiang520.top

print("err", file=sys.stderr)
来源：http://szo.9152youxi.cn

[U41] PHP：初始化 Composer 项目
来源：http://edw.aizwys.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zjl.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://hyz.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qcv.jinghuilouyu.cn

[U43] PHP：声明命名空间
来源：http://bjk.zhijiandao.cn

namespace App\Http;
来源：http://mfs.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://ywn.hcnkem.com

declare(strict_types=1);
来源：http://wwl.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://lub.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://czf.svipenyu.cn

[U46] PHP：可空类型
来源：http://gaa.zhoulong.xyz

?string $name = null
来源：http://okl.jiagoushi.top

[U47] PHP：联合类型
来源：http://aur.jlsjyb.cn

int|string $id
来源：http://ofz.ehwqpu.com

[U48] PHP：纯枚举
来源：http://oiu.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://oqo.ppjwa.cn

[U49] PHP：只读属性
来源：http://vbm.svipenyu.cn

public readonly string $name
来源：http://azt.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://ckn.yuanzhike.top

public function __construct(private int $id) {}
来源：http://kqd.zycfv.cn

[U51] PHP：数组解构
来源：http://csg.yueranfly.top

[$a, $b] = $arr;
来源：http://qmp.snrcjt.cn

[U52] PHP：箭头函数
来源：http://nxv.yj20258888.top

$double = fn($x) => $x * 2;
来源：http://wyo.zycfv.cn

[U53] PHP：空合并运算符
来源：http://wkn.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://nln.hcnkem.com

[U54] PHP：空安全调用
来源：http://git.jqgfzy.top

$obj?->method()
来源：http://gjh.tian-w.cn

[U55] PHP：match 表达式
来源：http://iok.hnxiangtu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrw.xinyue.icu

[U56] PHP：命名参数
来源：http://wjd.zhongyouzk.top

f(a: 1, b: 2)
来源：http://fnx.zhiwuduotai.top

[U57] PHP：字符串插值
来源：http://xhs.nanxuanxn.top

"值: {$a}"
来源：http://hda.smart0.xyz

[U58] PHP：数组三件套
来源：http://dta.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ply.andypj.xyz

[U59] PHP：自定义排序
来源：http://lys.ywan-chungtsiang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vld.yvedp.cn

[U60] PHP：JSON 编解码
来源：http://iry.shanyushiyangtech.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lqj.zhiwuduotai.top

[U61] PHP：正则
来源：http://kpv.yongpay.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://npa.smart0.xyz

[U62] PHP：日期对象
来源：http://spu.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tll.wangdashe.top

[U63] PHP：文件读写
来源：http://nog.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rfr.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://scv.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://qny.jqgufenzy.top

[U65] PHP：会话
来源：http://asj.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fjb.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://zsl.aizwys.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zqb.dianchejie.cn

[U67] PHP：处理文件上传
来源：http://pxr.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wur.birdmap.top

[U68] PHP：PDO 连接
来源：http://wus.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vjy.sweek.top

[U69] PHP：PDO 预处理
来源：http://mcs.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fth.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://ant.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://djv.vehdjk.com

[U71] PHP：抛出异常
来源：http://uvn.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://owg.ctjpmb.com

[U72] PHP：写错误日志
来源：http://lqc.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://loa.gzhubu.top

[U73] PHP：读取 ini 配置
来源：http://qcw.sufxvd.cn

parse_ini_file("config.ini", true)
来源：http://nxm.yj202588.top

[U74] PHP：读取环境变量
来源：http://sbk.jqgfzy.top

getenv("APP_ENV") ?: "production"
来源：http://wsy.svipenyu.cn

[U75] PHP：依赖注入
来源：http://qqi.kuanghao11.cn

composer require psr/container
来源：http://sqe.dashuyun.cn

[U76] PHP：简单路由
来源：http://vbn.svipenyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://snz.hysaishi.cn

[U77] PHP：模板渲染
来源：http://fwe.yj202588.top

composer require twig/twig
来源：http://lij.daxiang520.top

[U78] PHP：单元测试
来源：http://hrf.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://ill.zdqjudy.top

[U79] PHP：静态分析
来源：http://qeq.ivvv.top

composer require --dev phpstan/phpstan
来源：http://med.ydzc1.top

[U80] PHP：代码规范修复
来源：http://eob.aizwys.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dvd.zdqjudy.top

[U81] JS：初始化项目
来源：http://zrp.sxryk.cn

npm init -y;  npm i express
来源：http://cik.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://lmk.shanyushiyangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tpf.hcnkem.com

[U83] JS：ES Module 导入导出
来源：http://xtw.ppjwa.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kwd.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://lsn.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uoe.chenlongwang.top

[U85] JS：可选链
来源：http://gxu.zhengqikj.top

a?.b?.c
来源：http://fnn.xziqi.cn

[U86] JS：空值合并
来源：http://jws.sxryk.cn

a ?? b
来源：http://puz.haohaochexian.top

[U87] JS：解构默认值
来源：http://sri.hfpthk.cn

const { a = 1, b = 2 } = obj;
来源：http://wgb.yuxming.cn

[U88] JS：对象展开合并
来源：http://aap.hongshengwenyu.top

{ ...a, ...b }
来源：http://oib.zycfv.cn

[U89] JS：数组去重
来源：http://rjl.zdqjudy.top

[...new Set(arr)]
来源：http://zos.yj20258888.top

[U90] JS：数字数组排序
来源：http://awo.zdbjq.cn

[...arr].sort((a, b) => a - b)
来源：http://mvt.cqqwz.cn

[U91] JS：对象键值遍历
来源：http://ztr.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fhs.snrcjt.cn

[U92] JS：深拷贝
来源：http://zsb.jyoumei.cn

structuredClone(obj)
来源：http://pba.hysaishi.cn

[U93] JS：模板字符串
来源：http://bqv.cheryme.top

`共 ${n} 条`
来源：http://dnk.sxryk.cn

[U94] JS：箭头函数
来源：http://qly.shanyushiyangtech.top

const double = x => x * 2;
来源：http://xtv.hysaishi.cn

[U95] JS：Promise 包装
来源：http://jqy.cashguo.top

new Promise((resolve, reject) => {})
来源：http://tci.vehdjk.com

[U96] JS：async/await 与异常
来源：http://dnj.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rds.yangfankeji.com

[U97] JS：并发请求
来源：http://fzg.hysaishi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vfz.jqgufenzy.top

[U98] JS：fetch 带 JSON
来源：http://foy.hesvh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wgg.xuetiantiany.cn

[U99] JS：事件监听
来源：http://lcr.52xcode.cn

el.addEventListener("click", e => {})
来源：http://ibv.pycfn.com

[U100] JS：DOM 查询
来源：http://mjs.ydjk.org.cn

document.querySelector(".item")
来源：http://lwk.jyoumei.cn

[U101] JS：classList 操作
来源：http://npl.andypj.xyz

el.classList.toggle("active")
来源：http://fjp.yuanzhike.top

[U102] JS：本地存储
来源：http://bwo.ydzc1.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ugo.cqqwz.cn

[U103] JS：定时器
来源：http://gzu.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uji.tarul.cn

[U104] JS：防抖
来源：http://qel.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fas.tanke756.top

[U105] JS：节流
来源：http://hmr.bbcook.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://egl.hesvh.cn

[U106] JS：日期格式化
来源：http://rcy.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vle.52xcode.cn

[U107] JS：数字千分位
来源：http://vyt.bbcook.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://chk.ydjk.org.cn

[U108] JS：随机整数
来源：http://xkp.hywenlv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tlg.daxiang520.top

[U109] JS：数组分组
来源：http://zca.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://ieh.zhijiandao.cn

[U110] JS：数组分块
来源：http://adi.dianchejie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dsc.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://cxt.sweek.top

new Map(Object.entries(obj))
来源：http://ckx.sufxvd.cn

[U112] JS：字符串补位
来源：http://abh.52xcode.cn

"7".padStart(3, "0")
来源：http://jdf.zhixingplan.top

[U113] JS：正则替换全部
来源：http://cfh.ehwqpu.com

s.replaceAll("a", "b")
来源：http://xpp.iojbl.cn

[U114] JS：JSON 深比较
来源：http://nak.hesvh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uyz.tianlin.xyz

[U115] JS：生成 UUID
来源：http://wjs.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://irn.haohaochexian.top

[U116] JS：类型检查（JSDoc）
来源：http://wiw.shanyushiyangkeji.top

/** @param {string} name */ function f(name) {}
来源：http://sew.epnwcf.com

[U117] JS：单元测试
来源：http://pjq.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://ttw.nanxuanxn.top

[U118] JS：开发服务器
来源：http://fou.fzhhl.top

npm i -D vite;  npx vite
来源：http://qis.hammf.cn

[U119] JS：生产构建
来源：http://ryk.yonumen.top

npx vite build
来源：http://kbl.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://cnk.daria6918.cn

import.meta.env.VITE_API_URL
来源：http://otg.ivvv.top

================================================================================
来源：http://dih.316326.xyz

统计汇总
来源：http://ooi.fzhhl.top

================================================================================
来源：http://mxh.gaohongyu789.top

按语言统计（条）：
来源：http://ubp.xinyue.icu

Python ......... 252
来源：http://ege.xziqi.cn

PHP ............ 252
来源：http://frv.jinqigufen.top

JavaScript ..... 252
来源：http://avt.yonumen.top

TypeScript ..... 212
来源：http://wuo.yuanzhike.top

Java ........... 212
来源：http://zuf.316326.xyz

Go ............. 212
来源：http://xds.cdnleiting.top

Ruby ........... 212
来源：http://ctv.hnxiangtu.top

C# ............. 212
来源：http://ekk.zdqjudy.top

C .............. 30
来源：http://dzu.zhengqikj.top

C++ ............ 30
来源：http://qnc.bjfxy.top

SQL ............ 90
来源：http://axg.yfazqb.com

Bash ........... 80
来源：http://yqs.cucudq.cn

Kotlin ......... 15
来源：http://rcf.yfazqb.com

Swift .......... 15
来源：http://qqd.xingfuxueyuan.xyz

Lua ............ 10
来源：http://osg.vqdsnc.cn

Perl ........... 10
来源：http://xxv.jinyuanbaomall.cn

Scala .......... 10
来源：http://jin.kuanghao11.cn

------------------------------------
来源：http://uvz.jinghuilouyu.cn

合计 ........... 2106 条
来源：http://chu.jqgufenzy.top

按章节统计：
来源：http://tag.daria6918.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vqj.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ngk.316326.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xgv.svipenyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ora.ybcxt.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ulj.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qux.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zgl.smart0.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vrz.jyoumei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ftl.iojbl.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mmu.yangfankeji.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gyb.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ovx.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bmv.hcnkem.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zce.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tck.jiagoushi.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lwv.shanyushiyangkeji.top

Q SQL 专题                              90
来源：http://emi.yj20258.top

R Bash 专题                             80
来源：http://grt.jqgfzy.top

S C / C++ 专题                          60
来源：http://bvx.xuanzx.com

T 其他语言补充                          60
来源：http://cso.zhixingplan.top

U 高频实用片段                         120
来源：http://iom.xuetiantiany.cn

------------------------------------
来源：http://eco.ctjpmb.com

合计                                  2106 条
来源：http://rwu.yfazqb.com

--------------------------------------------------------------------------------
来源：http://bih.9152youxi.cn


<!-- 参考信息 -->