代发 wailian999

val a = 1;  var b = 2
来源：http://oyg.chenzaomai.com

[T53] Scala：字符串插值
来源：http://tub.jinghuilouyu.cn

s"值: $b"
来源：http://uhm.yj20258.top

[T54] Scala：集合映射
来源：http://jti.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://ejz.hcnkem.com

[T55] Scala：集合过滤
来源：http://phn.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rth.daxiang520.top

[T56] Scala：样例类
来源：http://gmu.gzhubu.top

case class User(name: String, age: Int)
来源：http://evx.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://ssz.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nki.cucudq.cn

[T58] Scala：函数定义
来源：http://fba.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://quk.yongpay.top

[T59] Scala：循环
来源：http://hxj.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://sjb.9152youxi.cn

[T60] Scala：折叠
来源：http://svx.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gxf.hcnkem.com

================================================================================
来源：http://iva.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qew.cdnleiting.top

================================================================================
来源：http://jhx.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://ryt.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://hkq.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://ihi.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qhi.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://vin.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zne.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://dtb.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cay.hcnkem.com

[U05] Py：列表去重且保序
来源：http://ubx.daria6918.cn

list(dict.fromkeys(arr))
来源：http://rlz.ctjpmb.com

[U06] Py：合并两个字典
来源：http://xan.yvedp.cn

{**a, **b}
来源：http://cht.smart0.xyz

[U07] Py：反转字典键值
来源：http://nlt.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://pji.epnwcf.com

[U08] Py：展平二维列表
来源：http://heq.ctjpmb.com

[y for x in nested for y in x]
来源：http://nok.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://esw.0kj1m.cn

max(d, key=d.get)
来源：http://zbr.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://mvd.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://afb.yj202588.top

[U11] Py：生成器表达式
来源：http://bnd.tarul.cn

(x * 2 for x in arr)
来源：http://yum.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bir.cashguo.top

Counter(arr).most_common(3)
来源：http://vdu.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://zvb.tarul.cn

deque(maxlen=10)
来源：http://lab.fzhhl.top

[U14] Py：分组收集到列表
来源：http://hxj.yuanzhike.top

defaultdict(list)
来源：http://irn.nwbrower.top

[U15] Py：高精度计时
来源：http://skr.mhx1999.top

t = time.perf_counter()
来源：http://fgg.yonumen.top

[U16] Py：命令行参数解析
来源：http://iaw.nanxinkj.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rit.gaohongyu789.top

[U17] Py：初始化日志
来源：http://bnr.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://fcf.zdqjudy.top

[U18] Py：预编译正则
来源：http://vbk.ybcxt.top

pat = re.compile(r"\d+")
来源：http://spq.zdqjudy.top

[U19] Py：正则替换带回调
来源：http://nnf.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zkf.tanke756.top

[U20] Py：缓存函数结果
来源：http://fax.hywenlv.cn

@functools.lru_cache(maxsize=None)
来源：http://njw.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://ued.bbcook.cn

@contextlib.contextmanager
来源：http://pwc.zhengqikj.top

[U22] Py：矩阵转置
来源：http://jvs.haohaochexian.top

list(zip(*m))
来源：http://yir.jiagoushi.top

[U23] Py：分块读取大文件
来源：http://iob.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sfq.zhengqikj.top

[U24] Py：路径操作
来源：http://ahp.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yrk.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://rqv.bjfxy.top

csv.DictReader(f)
来源：http://dih.jqgfzy.top

[U26] Py：并发下载
来源：http://szs.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pic.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://lpr.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://eru.meibo888.top

[U28] Py：类型别名
来源：http://xjo.ydzc1.top

UserId = int
来源：http://sgl.yuxming.cn

[U29] Py：属性校验
来源：http://kbu.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://aep.smart0.xyz

[U30] Py：数据类
来源：http://wwl.feifeiyinyue.top

@dataclass(slots=True)
来源：http://oye.zhijiandao.cn

[U31] Py：单测
来源：http://nft.pycfn.com

python -m pytest -q
来源：http://cmz.shuidangran.top

[U32] Py：代码格式化
来源：http://xqv.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://vlp.ivvv.top

[U33] Py：打包发布
来源：http://qia.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://zhz.svipenyu.cn

[U34] Py：判断编码
来源：http://ztm.andypj.xyz

chardet.detect(raw)
来源：http://cfg.snrcjt.cn

[U35] Py：发送邮件
来源：http://dfl.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://juo.9152youxi.cn

[U36] Py：定时任务
来源：http://thu.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://byf.epnwcf.com

[U37] Py：读写 Excel
来源：http://smy.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://htc.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://uyn.jiagoushi.top

Path(__file__).resolve().parent
来源：http://qhj.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://bkn.shangyingyoupin.top

sys.stdout.isatty()
来源：http://bvx.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://exg.wangdashe.top

print("err", file=sys.stderr)
来源：http://mzy.jqgufenzy.top

[U41] PHP：初始化 Composer 项目
来源：http://bhh.yj20258.top

composer init;  composer require guzzlehttp/guzzle
来源：http://dxz.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://jfm.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hsm.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://inw.redwolf501.top

namespace App\Http;
来源：http://qjj.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://zvz.gaohongyu789.top

declare(strict_types=1);
来源：http://pop.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://ipz.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vnp.andypj.xyz

[U46] PHP：可空类型
来源：http://xlv.zhixingplan.top

?string $name = null
来源：http://szc.hcnkem.com

[U47] PHP：联合类型
来源：http://yay.zhengqikj.top

int|string $id
来源：http://cuh.guowangkeji.top

[U48] PHP：纯枚举
来源：http://mnx.gotoacloud.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gup.52xcode.cn

[U49] PHP：只读属性
来源：http://qfl.fanxiaobao.xyz

public readonly string $name
来源：http://joc.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://qep.redwolf501.top

public function __construct(private int $id) {}
来源：http://jyk.aizwys.cn

[U51] PHP：数组解构
来源：http://eba.dashuyun.cn

[$a, $b] = $arr;
来源：http://ilu.chenzaomai.com

[U52] PHP：箭头函数
来源：http://veh.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://lqd.hnqzz.top

[U53] PHP：空合并运算符
来源：http://uzr.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://bji.cashguo.top

[U54] PHP：空安全调用
来源：http://mbv.jinyuanbaomall.cn

$obj?->method()
来源：http://svo.yj20258.top

[U55] PHP：match 表达式
来源：http://dok.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tob.meibo888.top

[U56] PHP：命名参数
来源：http://spb.fzhhl.top

f(a: 1, b: 2)
来源：http://rsv.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://fyb.vqdsnc.cn

"值: {$a}"
来源：http://lan.yfazqb.com

[U58] PHP：数组三件套
来源：http://tgq.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mya.ctjpmb.com

[U59] PHP：自定义排序
来源：http://wqf.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czn.yongpay.top

[U60] PHP：JSON 编解码
来源：http://unh.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rue.hfpthk.cn

[U61] PHP：正则
来源：http://zhs.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dto.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://hmo.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ows.jyoumei.cn

[U63] PHP：文件读写
来源：http://cep.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bba.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://kue.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ehw.tanke756.top

[U65] PHP：会话
来源：http://jvr.epnwcf.com

session_start();  $_SESSION["uid"] = 1;
来源：http://fzc.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://zcw.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jng.yj20258.top

[U67] PHP：处理文件上传
来源：http://hbj.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vaa.fengsongda.top

[U68] PHP：PDO 连接
来源：http://tft.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zzq.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://azb.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yjv.shangyingyoupin.top

[U70] PHP：PDO 事务
来源：http://vls.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cne.tian-w.cn

[U71] PHP：抛出异常
来源：http://nel.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://isr.yj20258888.top

[U72] PHP：写错误日志
来源：http://idb.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://qvo.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://sai.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://vpg.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://svb.zycfv.cn

getenv("APP_ENV") ?: "production"
来源：http://kip.cdnleiting.top

[U75] PHP：依赖注入
来源：http://ueg.shzxlz.cn

composer require psr/container
来源：http://inx.yfazqb.com

[U76] PHP：简单路由
来源：http://vun.316326.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://equ.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://qsh.jyoumei.cn

composer require twig/twig
来源：http://cqs.fzhhl.top

[U78] PHP：单元测试
来源：http://amh.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://tsh.cucudq.cn

[U79] PHP：静态分析
来源：http://itq.yanxiufei.cn

composer require --dev phpstan/phpstan
来源：http://bat.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://wdi.svipenyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ray.316326.xyz

[U81] JS：初始化项目
来源：http://rxc.chenlongwang.top

npm init -y;  npm i express
来源：http://tns.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://fxa.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gcc.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://sfq.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://mji.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://xee.tanke756.top

module.exports = { a };  const { a } = require("./m");
来源：http://qfi.guowangkeji.top

[U85] JS：可选链
来源：http://ycq.iojbl.cn

a?.b?.c
来源：http://qgv.ehwqpu.com

[U86] JS：空值合并
来源：http://ews.gogol.net.cn

a ?? b
来源：http://nsn.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://wwi.hammf.cn

const { a = 1, b = 2 } = obj;
来源：http://eub.cashguo.top

[U88] JS：对象展开合并
来源：http://ihq.hywenlv.cn

{ ...a, ...b }
来源：http://rvw.xuetiantiany.cn

[U89] JS：数组去重
来源：http://tjt.jinqigufen.top

[...new Set(arr)]
来源：http://hcs.yj20258.top

[U90] JS：数字数组排序
来源：http://tww.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://faw.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://iaz.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gdu.gogol.net.cn

[U92] JS：深拷贝
来源：http://mjr.nanxuanxn.top

structuredClone(obj)
来源：http://bqf.zdbjq.cn

[U93] JS：模板字符串
来源：http://eaw.9152youxi.cn

`共 ${n} 条`
来源：http://hxm.yj20258888.top

[U94] JS：箭头函数
来源：http://qvo.vehdjk.com

const double = x => x * 2;
来源：http://iwb.ydzc1.top

[U95] JS：Promise 包装
来源：http://tub.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://hdy.zhengqikj.top

[U96] JS：async/await 与异常
来源：http://hxu.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tzb.gotoacloud.top

[U97] JS：并发请求
来源：http://kjv.quarkkingdee.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://llx.uphjek.com

[U98] JS：fetch 带 JSON
来源：http://dzz.ivvv.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rbp.gzhubu.top

[U99] JS：事件监听
来源：http://dzs.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://xhf.yueranfly.top

[U100] JS：DOM 查询
来源：http://vcu.ydjk.org.cn

document.querySelector(".item")
来源：http://obf.vqdsnc.cn

[U101] JS：classList 操作
来源：http://qir.vqdsnc.cn

el.classList.toggle("active")
来源：http://qso.ydzc1.top

[U102] JS：本地存储
来源：http://pox.pycfn.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://mqi.vqdsnc.cn

[U103] JS：定时器
来源：http://bka.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sfj.chenjidiqi.icu

[U104] JS：防抖
来源：http://hnn.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mnf.vehdjk.com

[U105] JS：节流
来源：http://jxa.feifeiyinyue.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://shi.yvedp.cn

[U106] JS：日期格式化
来源：http://via.gzhubu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rja.smart0.xyz

[U107] JS：数字千分位
来源：http://pkm.birdmap.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hxr.epnwcf.com

[U108] JS：随机整数
来源：http://kul.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xiw.xingfuxueyuan.xyz

[U109] JS：数组分组
来源：http://bqi.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://hvp.fktsv.cn

[U110] JS：数组分块
来源：http://ouj.cucudq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nhp.yvedp.cn

[U111] JS：对象转 Map
来源：http://uqw.52xcode.cn

new Map(Object.entries(obj))
来源：http://zix.sxryk.cn

[U112] JS：字符串补位
来源：http://eks.meibo888.top

"7".padStart(3, "0")
来源：http://imb.chenlongwang.top

[U113] JS：正则替换全部
来源：http://lnh.wangdashe.top

s.replaceAll("a", "b")
来源：http://ufe.ydjk.org.cn

[U114] JS：JSON 深比较
来源：http://tle.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jsu.fzhhl.top

[U115] JS：生成 UUID
来源：http://sfs.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://iwz.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://kzx.tianlin.xyz

/** @param {string} name */ function f(name) {}
来源：http://onn.birdmap.top

[U117] JS：单元测试
来源：http://ytr.tarul.cn

npm i -D vitest;  npx vitest
来源：http://fop.zhoulong.xyz

[U118] JS：开发服务器
来源：http://mnt.cashguo.top

npm i -D vite;  npx vite
来源：http://moa.jqgfzy.top

[U119] JS：生产构建
来源：http://bpi.hammf.cn

npx vite build
来源：http://hvs.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://gdq.tarul.cn

import.meta.env.VITE_API_URL
来源：http://xba.yvedp.cn

================================================================================
来源：http://rmi.hfpthk.cn

统计汇总
来源：http://wmm.shanyushiyangtech.top

================================================================================
来源：http://opq.shanyushiyangtech.top

按语言统计（条）：
来源：http://igk.xziqi.cn

Python ......... 252
来源：http://irz.hywenlv.cn

PHP ............ 252
来源：http://xwl.xylfe.cn

JavaScript ..... 252
来源：http://rxj.cucudq.cn

TypeScript ..... 212
来源：http://xcl.yonumen.top

Java ........... 212
来源：http://wcx.nanxinkj.top

Go ............. 212
来源：http://qzy.sjlbkw.cn

Ruby ........... 212
来源：http://qmv.xingfuxueyuan.xyz

C# ............. 212
来源：http://jcy.haohaochexian.top

C .............. 30
来源：http://qql.hysaishi.cn

C++ ............ 30
来源：http://ebb.cqqwz.cn

SQL ............ 90
来源：http://rqy.9152youxi.cn

Bash ........... 80
来源：http://ufc.zhijiandao.cn

Kotlin ......... 15
来源：http://okt.nanxuanxn.top

Swift .......... 15
来源：http://vgp.hongshengwenyu.top

Lua ............ 10
来源：http://ubj.ivvv.top

Perl ........... 10
来源：http://pft.jinyuanbaomall.cn

Scala .......... 10
来源：http://uof.xuanzx.com

------------------------------------
来源：http://mdo.316326.xyz

合计 ........... 2106 条
来源：http://brf.jlsjyb.cn

按章节统计：
来源：http://fww.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qjk.havefunace.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bnk.meibo888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gtx.wangdashe.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jds.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://oli.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://twn.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ppo.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://anj.gogol.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ope.xylfe.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kcg.epnwcf.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lkg.gogol.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lbl.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nen.fktsv.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://poz.0kj1m.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gwt.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eya.hnxiangtu.top


<!-- 参考信息 -->