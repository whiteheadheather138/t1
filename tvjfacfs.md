代发 wailian999

val a = 1;  var b = 2
来源：http://pst.cheryme.top

[T53] Scala：字符串插值
来源：http://nlg.mhx1999.top

s"值: $b"
来源：http://rmc.ppjwa.cn

[T54] Scala：集合映射
来源：http://rca.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://ihq.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://kap.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://zkj.sysykeji.top

[T56] Scala：样例类
来源：http://rig.hesvh.cn

case class User(name: String, age: Int)
来源：http://evk.vehdjk.com

[T57] Scala：模式匹配
来源：http://moi.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://nzu.guowangkeji.top

[T58] Scala：函数定义
来源：http://kku.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cpx.birdmap.top

[T59] Scala：循环
来源：http://jau.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://gun.fehbvm.com

[T60] Scala：折叠
来源：http://bpt.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gle.gaohongyu789.top

================================================================================
来源：http://agx.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uev.daxiang520.top

================================================================================
来源：http://baj.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://qwr.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://maa.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://hog.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lev.yj20258.top

[U03] Py：加载 .env 配置
来源：http://vda.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nip.ppjwa.cn

[U04] Py：变量调试打印
来源：http://cqj.jinqigfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gir.yueranfly.top

[U05] Py：列表去重且保序
来源：http://wlk.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://uxn.sweek.top

[U06] Py：合并两个字典
来源：http://cgj.xziqi.cn

{**a, **b}
来源：http://vmx.yvedp.cn

[U07] Py：反转字典键值
来源：http://twd.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://fse.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://oxv.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://ean.tarul.cn

[U09] Py：字典取最大值的键
来源：http://xal.yanxiufei.cn

max(d, key=d.get)
来源：http://pkm.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://fsg.hfpthk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zfd.dashuyun.cn

[U11] Py：生成器表达式
来源：http://xet.shzxlz.cn

(x * 2 for x in arr)
来源：http://mek.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://die.fktsv.cn

Counter(arr).most_common(3)
来源：http://heq.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://nmd.hammf.cn

deque(maxlen=10)
来源：http://qkr.chenlongwang.top

[U14] Py：分组收集到列表
来源：http://ugl.chenzaomai.com

defaultdict(list)
来源：http://hoo.yueranfly.top

[U15] Py：高精度计时
来源：http://ybv.ywan-chungtsiang.top

t = time.perf_counter()
来源：http://dso.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://ejs.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oat.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://une.aibaodan.cn

logging.basicConfig(level=logging.INFO)
来源：http://izf.guannengcc.top

[U18] Py：预编译正则
来源：http://iwn.yuanzhike.top

pat = re.compile(r"\d+")
来源：http://qce.yvedp.cn

[U19] Py：正则替换带回调
来源：http://xzm.0kj1m.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zhd.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://psb.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://bsj.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://omh.shanyushiyangkeji.top

@contextlib.contextmanager
来源：http://rhe.aibaodan.cn

[U22] Py：矩阵转置
来源：http://jnx.yueranfly.top

list(zip(*m))
来源：http://emf.daxiang520.top

[U23] Py：分块读取大文件
来源：http://ext.shanyushiyangtech.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fuv.xziqi.cn

[U24] Py：路径操作
来源：http://ism.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vxx.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://eyq.fzhhl.top

csv.DictReader(f)
来源：http://nje.zhoulong.xyz

[U26] Py：并发下载
来源：http://aly.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xly.316326.xyz

[U27] Py：异步 HTTP
来源：http://ajx.guowangkeji.top

aiohttp.ClientSession() 配合 async with
来源：http://nmk.wangdashe.top

[U28] Py：类型别名
来源：http://kru.jinqigfzy.top

UserId = int
来源：http://ebm.andypj.xyz

[U29] Py：属性校验
来源：http://gkc.yongpay.top

@property 与 @x.setter 配合
来源：http://miu.yueranfly.top

[U30] Py：数据类
来源：http://tje.xinyue.icu

@dataclass(slots=True)
来源：http://muk.xylfe.cn

[U31] Py：单测
来源：http://mzx.hysaishi.cn

python -m pytest -q
来源：http://ycz.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://jhl.fengsongda.top

ruff format . && ruff check --fix .
来源：http://agu.jinghuilouyu.cn

[U33] Py：打包发布
来源：http://nrs.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://fwc.yj202588.top

[U34] Py：判断编码
来源：http://qnx.xinyue.icu

chardet.detect(raw)
来源：http://zjy.daxiang520.top

[U35] Py：发送邮件
来源：http://fkz.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fcb.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://cay.pycfn.com

schedule.every(10).minutes.do(job)
来源：http://flg.zdqjudy.top

[U37] Py：读写 Excel
来源：http://vmb.xinyue.icu

pandas.read_excel / DataFrame.to_excel
来源：http://vaw.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://qxt.vehdjk.com

Path(__file__).resolve().parent
来源：http://zbs.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://zjr.0kj1m.cn

sys.stdout.isatty()
来源：http://ofz.havefunace.top

[U40] Py：打印到标准错误
来源：http://rzm.yvedp.cn

print("err", file=sys.stderr)
来源：http://qcg.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://thl.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://uow.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://dql.yangfankeji.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kng.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://jlw.hnqzz.top

namespace App\Http;
来源：http://woi.zhengqikj.top

[U44] PHP：开启严格类型
来源：http://nnq.ybcxt.top

declare(strict_types=1);
来源：http://ytb.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://buj.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://stn.yongpay.top

[U46] PHP：可空类型
来源：http://sed.hongshengwenyu.top

?string $name = null
来源：http://khw.yfazqb.com

[U47] PHP：联合类型
来源：http://ryy.zdqjudy.top

int|string $id
来源：http://yzw.jyoumei.cn

[U48] PHP：纯枚举
来源：http://epr.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tgw.daxiang520.top

[U49] PHP：只读属性
来源：http://cjq.shzxlz.cn

public readonly string $name
来源：http://gqm.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://lyj.epnwcf.com

public function __construct(private int $id) {}
来源：http://knr.c1oappe.top

[U51] PHP：数组解构
来源：http://sea.shuidangran.top

[$a, $b] = $arr;
来源：http://qym.ppjwa.cn

[U52] PHP：箭头函数
来源：http://ahx.cashguo.top

$double = fn($x) => $x * 2;
来源：http://vdb.xuetiantiany.cn

[U53] PHP：空合并运算符
来源：http://htb.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://ezx.ctjpmb.com

[U54] PHP：空安全调用
来源：http://zjy.ydjk.org.cn

$obj?->method()
来源：http://pln.yangfankeji.com

[U55] PHP：match 表达式
来源：http://vsh.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nbt.yuxming.cn

[U56] PHP：命名参数
来源：http://mok.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://iqa.hysaishi.cn

[U57] PHP：字符串插值
来源：http://cgs.guannengcc.top

"值: {$a}"
来源：http://rfd.jinyuanbaomall.cn

[U58] PHP：数组三件套
来源：http://muk.vqdsnc.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mwl.yj20258888.top

[U59] PHP：自定义排序
来源：http://mmq.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jum.cheryme.top

[U60] PHP：JSON 编解码
来源：http://rii.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://niq.hfpthk.cn

[U61] PHP：正则
来源：http://nni.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://oww.vqdsnc.cn

[U62] PHP：日期对象
来源：http://hld.yfazqb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://akj.zhengqikj.top

[U63] PHP：文件读写
来源：http://osg.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ohr.jinqigufen.top

[U64] PHP：目录遍历
来源：http://kgy.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://ept.zhongyouzk.top

[U65] PHP：会话
来源：http://tqx.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vbk.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://edu.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://erc.cashguo.top

[U67] PHP：处理文件上传
来源：http://vtq.zdqjudy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wdv.cheryme.top

[U68] PHP：PDO 连接
来源：http://nib.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rpg.xinyue.icu

[U69] PHP：PDO 预处理
来源：http://vow.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ias.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://icv.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nfi.jinqigufen.top

[U71] PHP：抛出异常
来源：http://ehm.daria6918.cn

throw new RuntimeException("失败", 500);
来源：http://ncw.gotoacloud.top

[U72] PHP：写错误日志
来源：http://dkv.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://bvy.yangfankeji.com

[U73] PHP：读取 ini 配置
来源：http://emu.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://rmz.hesvh.cn

[U74] PHP：读取环境变量
来源：http://mmb.zhengqikj.top

getenv("APP_ENV") ?: "production"
来源：http://rmt.xuetiantiany.cn

[U75] PHP：依赖注入
来源：http://ptf.zhongyouzk.top

composer require psr/container
来源：http://xxz.yj20258888.top

[U76] PHP：简单路由
来源：http://lpw.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sph.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://ngc.vqdsnc.cn

composer require twig/twig
来源：http://mya.epnwcf.com

[U78] PHP：单元测试
来源：http://lqk.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://znu.yuanzhike.top

[U79] PHP：静态分析
来源：http://sen.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://znr.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://pgp.gogol.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vrv.jqgfzy.top

[U81] JS：初始化项目
来源：http://vws.cashguo.top

npm init -y;  npm i express
来源：http://rmn.epnwcf.com

[U82] JS：package.json 脚本
来源：http://adh.zhixingplan.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fux.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://vsd.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://vob.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://aml.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ljv.shanyushiyangtech.top

[U85] JS：可选链
来源：http://ypf.tanke756.top

a?.b?.c
来源：http://vxv.jyoumei.cn

[U86] JS：空值合并
来源：http://lkb.jinghuilouyu.cn

a ?? b
来源：http://gzn.aibaodan.cn

[U87] JS：解构默认值
来源：http://rtr.yongpay.top

const { a = 1, b = 2 } = obj;
来源：http://mli.c1oappe.top

[U88] JS：对象展开合并
来源：http://paw.guowangkeji.top

{ ...a, ...b }
来源：http://nqc.jinqigufen.top

[U89] JS：数组去重
来源：http://vmi.zhijiandao.cn

[...new Set(arr)]
来源：http://hls.ywan-chungtsiang.top

[U90] JS：数字数组排序
来源：http://spz.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://mue.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://yuv.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://olt.zdqjudy.top

[U92] JS：深拷贝
来源：http://kou.tanke756.top

structuredClone(obj)
来源：http://pcq.zhongyouzk.top

[U93] JS：模板字符串
来源：http://bct.aibaodan.cn

`共 ${n} 条`
来源：http://qei.gotoacloud.top

[U94] JS：箭头函数
来源：http://ymb.guowangkeji.top

const double = x => x * 2;
来源：http://rcg.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://xlt.hfpthk.cn

new Promise((resolve, reject) => {})
来源：http://zut.chenzaomai.com

[U96] JS：async/await 与异常
来源：http://lor.sysykeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ntb.zycfv.cn

[U97] JS：并发请求
来源：http://kif.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ofa.shangyingyoupin.top

[U98] JS：fetch 带 JSON
来源：http://ily.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hlp.shangyingyoupin.top

[U99] JS：事件监听
来源：http://dws.svipenyu.cn

el.addEventListener("click", e => {})
来源：http://mfm.cdnleiting.top

[U100] JS：DOM 查询
来源：http://tse.hcnkem.com

document.querySelector(".item")
来源：http://mek.fanxiaobao.xyz

[U101] JS：classList 操作
来源：http://awv.pycfn.com

el.classList.toggle("active")
来源：http://gob.tanke756.top

[U102] JS：本地存储
来源：http://ciy.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fch.daria6918.cn

[U103] JS：定时器
来源：http://uok.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mfm.daxiang520.top

[U104] JS：防抖
来源：http://iuo.yuxming.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bfs.chenjidiqi.icu

[U105] JS：节流
来源：http://svx.svipenyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://alj.zhijiandao.cn

[U106] JS：日期格式化
来源：http://rpd.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pqm.shzxlz.cn

[U107] JS：数字千分位
来源：http://fww.zdqjudy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wpe.ybcxt.top

[U108] JS：随机整数
来源：http://odu.52xcode.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rzx.chenjidiqi.icu

[U109] JS：数组分组
来源：http://dhe.52xcode.cn

Object.groupBy(arr, x => x.type)
来源：http://gzl.jlsjyb.cn

[U110] JS：数组分块
来源：http://ltg.yonumen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rmi.hcnkem.com

[U111] JS：对象转 Map
来源：http://tat.birdmap.top

new Map(Object.entries(obj))
来源：http://zrh.xuetiantiany.cn

[U112] JS：字符串补位
来源：http://cvz.gaohongyu789.top

"7".padStart(3, "0")
来源：http://onr.hesvh.cn

[U113] JS：正则替换全部
来源：http://cbz.zhixingplan.top

s.replaceAll("a", "b")
来源：http://lqp.fktsv.cn

[U114] JS：JSON 深比较
来源：http://atw.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pip.aizwys.cn

[U115] JS：生成 UUID
来源：http://vqs.ppjwa.cn

crypto.randomUUID()
来源：http://gqj.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://lqv.gzhubu.top

/** @param {string} name */ function f(name) {}
来源：http://roh.jqgfzy.top

[U117] JS：单元测试
来源：http://vmf.jianghu66.top

npm i -D vitest;  npx vitest
来源：http://ofm.zhaomingkeji.xyz

[U118] JS：开发服务器
来源：http://woq.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://sjm.redwolf501.top

[U119] JS：生产构建
来源：http://mnr.smart0.xyz

npx vite build
来源：http://ymi.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://jpo.jianghu66.top

import.meta.env.VITE_API_URL
来源：http://fqk.ywan-chungtsiang.top

================================================================================
来源：http://geu.yonumen.top

统计汇总
来源：http://vmg.ydzc1.top

================================================================================
来源：http://nqf.fehbvm.com

按语言统计（条）：
来源：http://ihm.ydzc1.top

Python ......... 252
来源：http://bnb.pengpengdd.cyou

PHP ............ 252
来源：http://vfo.snrcjt.cn

JavaScript ..... 252
来源：http://ehr.andypj.xyz

TypeScript ..... 212
来源：http://fdu.hesvh.cn

Java ........... 212
来源：http://wak.nanxuanxn.top

Go ............. 212
来源：http://fye.dashuyun.cn

Ruby ........... 212
来源：http://cyj.uphjek.com

C# ............. 212
来源：http://ndy.xziqi.cn

C .............. 30
来源：http://rvg.havefunace.top

C++ ............ 30
来源：http://psc.yuanzhike.top

SQL ............ 90
来源：http://jnf.andypj.xyz

Bash ........... 80
来源：http://ijr.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://rvn.yueranfly.top

Swift .......... 15
来源：http://gaz.xziqi.cn

Lua ............ 10
来源：http://enk.zhengqikj.top

Perl ........... 10
来源：http://bnf.pycfn.com

Scala .......... 10
来源：http://pnm.fzhhl.top

------------------------------------
来源：http://gfz.jiagoushi.top

合计 ........... 2106 条
来源：http://wpi.shanyushiyangkeji.top

按章节统计：
来源：http://fsy.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ipv.fengsongda.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dfp.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://okz.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://acc.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gef.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://srp.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://djs.zdqjudy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wsb.chenzaomai.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mlu.jinghuilouyu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bxf.xylfe.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aqs.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ubt.havefunace.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qol.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mjh.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dcr.xingfuxueyuan.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://spt.sufxvd.cn


<!-- 参考信息 -->