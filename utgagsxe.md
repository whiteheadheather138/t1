代发 wailian999

[T49] Perl：函数
来源：http://dbh.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jxy.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://rsh.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://voz.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://med.kuanghao11.cn

[T51] Scala：Hello World
来源：http://xsm.yj20258888.top

println("Hello")
来源：http://dhy.hysaishi.cn

[T52] Scala：变量
来源：http://hju.fehbvm.com

val a = 1;  var b = 2
来源：http://qlo.tian-w.cn

[T53] Scala：字符串插值
来源：http://fea.zhixingplan.top

s"值: $b"
来源：http://tyb.sufxvd.cn

[T54] Scala：集合映射
来源：http://xou.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://nmx.ydzc1.top

[T55] Scala：集合过滤
来源：http://jho.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://bmd.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://kpd.yongpay.top

case class User(name: String, age: Int)
来源：http://lky.andypj.xyz

[T57] Scala：模式匹配
来源：http://rxe.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cff.sysykeji.top

[T58] Scala：函数定义
来源：http://oak.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://adu.svipenyu.cn

[T59] Scala：循环
来源：http://cus.yj202588.top

for (i <- 1 to 10) println(i)
来源：http://cao.jinqigufen.top

[T60] Scala：折叠
来源：http://qxn.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yga.chenzaomai.com

================================================================================
来源：http://ggb.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zmp.andypj.xyz

================================================================================
来源：http://wqm.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://wzm.zhengqikj.top

python -m venv .venv && source .venv/bin/activate
来源：http://pwj.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://bsk.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qcx.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://jun.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kfh.smart0.xyz

[U04] Py：变量调试打印
来源：http://yot.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jsx.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://bkz.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://rgj.chenlongwang.top

[U06] Py：合并两个字典
来源：http://cea.xuanzx.com

{**a, **b}
来源：http://dfw.cashguo.top

[U07] Py：反转字典键值
来源：http://iuu.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://zdj.tianlin.xyz

[U08] Py：展平二维列表
来源：http://jqj.vqdsnc.cn

[y for x in nested for y in x]
来源：http://jmk.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://bku.fktsv.cn

max(d, key=d.get)
来源：http://gql.sxryk.cn

[U10] Py：按值排序字典
来源：http://mpz.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rfj.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://tvr.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://hpx.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cdl.jqgfzy.top

Counter(arr).most_common(3)
来源：http://oob.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://txc.wangdashe.top

deque(maxlen=10)
来源：http://ruj.aizwys.cn

[U14] Py：分组收集到列表
来源：http://tiq.tarul.cn

defaultdict(list)
来源：http://icy.aizwys.cn

[U15] Py：高精度计时
来源：http://nbv.uphjek.com

t = time.perf_counter()
来源：http://ljt.shuidangran.top

[U16] Py：命令行参数解析
来源：http://fje.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://omf.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://mgo.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://veg.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://hsq.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://kor.fengsongda.top

[U19] Py：正则替换带回调
来源：http://xko.shuidangran.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mgv.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://rkk.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://nqb.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://xtx.jianghu66.top

@contextlib.contextmanager
来源：http://jje.zhixingplan.top

[U22] Py：矩阵转置
来源：http://hoy.redwolf501.top

list(zip(*m))
来源：http://ltp.shanyushiyangtech.top

[U23] Py：分块读取大文件
来源：http://ioa.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jvm.zdbjq.cn

[U24] Py：路径操作
来源：http://xdm.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dfi.uphjek.com

[U25] Py：CSV 按字典读
来源：http://gjk.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://lbe.yj20258888.top

[U26] Py：并发下载
来源：http://pbg.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yvc.tarul.cn

[U27] Py：异步 HTTP
来源：http://ahp.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://hur.bbcook.cn

[U28] Py：类型别名
来源：http://zad.jlsjyb.cn

UserId = int
来源：http://kug.yonumen.top

[U29] Py：属性校验
来源：http://xig.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://jhh.havefunace.top

[U30] Py：数据类
来源：http://unv.yanxiufei.cn

@dataclass(slots=True)
来源：http://tfj.hnxiangtu.top

[U31] Py：单测
来源：http://euc.wangdashe.top

python -m pytest -q
来源：http://abi.ydzc1.top

[U32] Py：代码格式化
来源：http://tqb.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://bwb.daria6918.cn

[U33] Py：打包发布
来源：http://fdu.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://ito.gotoacloud.top

[U34] Py：判断编码
来源：http://gbj.guannengcc.top

chardet.detect(raw)
来源：http://wtp.hysaishi.cn

[U35] Py：发送邮件
来源：http://pvz.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lob.wangdashe.top

[U36] Py：定时任务
来源：http://vrl.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://fld.havefunace.top

[U37] Py：读写 Excel
来源：http://dfo.aizwys.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iwh.zhixingplan.top

[U38] Py：获取脚本所在目录
来源：http://dek.tianlin.xyz

Path(__file__).resolve().parent
来源：http://eeg.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://bmu.aizwys.cn

sys.stdout.isatty()
来源：http://qdl.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://yrc.yueranfly.top

print("err", file=sys.stderr)
来源：http://tok.gogol.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://lds.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lmo.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://wgu.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oot.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://tgk.mhx1999.top

namespace App\Http;
来源：http://tdj.yvedp.cn

[U44] PHP：开启严格类型
来源：http://nxn.sufxvd.cn

declare(strict_types=1);
来源：http://pzh.xziqi.cn

[U45] PHP：类型声明与返回类型
来源：http://asj.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rzh.shzxlz.cn

[U46] PHP：可空类型
来源：http://zhn.gzhubu.top

?string $name = null
来源：http://gij.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://lee.cucudq.cn

int|string $id
来源：http://crd.tarul.cn

[U48] PHP：纯枚举
来源：http://urr.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dqt.hesvh.cn

[U49] PHP：只读属性
来源：http://liu.52xcode.cn

public readonly string $name
来源：http://lvg.hammf.cn

[U50] PHP：构造器属性提升
来源：http://bsl.birdmap.top

public function __construct(private int $id) {}
来源：http://xci.yuxming.cn

[U51] PHP：数组解构
来源：http://iuz.vqdsnc.cn

[$a, $b] = $arr;
来源：http://yfs.andypj.xyz

[U52] PHP：箭头函数
来源：http://piw.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://spk.316326.xyz

[U53] PHP：空合并运算符
来源：http://rtj.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://xpj.vqdsnc.cn

[U54] PHP：空安全调用
来源：http://lec.gogol.net.cn

$obj?->method()
来源：http://wpc.haohaochexian.top

[U55] PHP：match 表达式
来源：http://mjq.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://luh.daxiang520.top

[U56] PHP：命名参数
来源：http://mfv.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://zti.jinyuanbaomall.cn

[U57] PHP：字符串插值
来源：http://cmy.haohaochexian.top

"值: {$a}"
来源：http://eov.hywenlv.cn

[U58] PHP：数组三件套
来源：http://vgu.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zvq.jianghu66.top

[U59] PHP：自定义排序
来源：http://zxy.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fph.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://wss.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://syd.yfazqb.com

[U61] PHP：正则
来源：http://shf.xinyue.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rbq.gzhubu.top

[U62] PHP：日期对象
来源：http://msh.xziqi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pbn.ivvv.top

[U63] PHP：文件读写
来源：http://szl.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ylr.cqqwz.cn

[U64] PHP：目录遍历
来源：http://zzp.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://ouk.yangfankeji.com

[U65] PHP：会话
来源：http://mdt.shanyushiyangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dvc.pengpengdd.cyou

[U66] PHP：设置 Cookie
来源：http://cza.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xlp.jqgfzy.top

[U67] PHP：处理文件上传
来源：http://kdd.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mus.zhoulong.xyz

[U68] PHP：PDO 连接
来源：http://hey.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kfu.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://lye.yvedp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ymg.chenzaomai.com

[U70] PHP：PDO 事务
来源：http://urj.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ylb.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://edx.tanke756.top

throw new RuntimeException("失败", 500);
来源：http://jvw.cashguo.top

[U72] PHP：写错误日志
来源：http://wia.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://ary.shanyushiyangtech.top

[U73] PHP：读取 ini 配置
来源：http://noh.yj20258.top

parse_ini_file("config.ini", true)
来源：http://xff.svipenyu.cn

[U74] PHP：读取环境变量
来源：http://wip.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://zjp.guannengcc.top

[U75] PHP：依赖注入
来源：http://kue.jinghuilouyu.cn

composer require psr/container
来源：http://vau.zhoulong.xyz

[U76] PHP：简单路由
来源：http://ggp.xuanzx.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ces.tanke756.top

[U77] PHP：模板渲染
来源：http://fno.ydjk.org.cn

composer require twig/twig
来源：http://wqy.ydjk.org.cn

[U78] PHP：单元测试
来源：http://cyl.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://lrh.sufxvd.cn

[U79] PHP：静态分析
来源：http://vgv.fengsongda.top

composer require --dev phpstan/phpstan
来源：http://gda.bbcook.cn

[U80] PHP：代码规范修复
来源：http://qmh.daxiang520.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://bfh.bbcook.cn

[U81] JS：初始化项目
来源：http://dio.aizwys.cn

npm init -y;  npm i express
来源：http://hup.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://pym.316326.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wte.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://mzs.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://jiw.hywenlv.cn

[U84] JS：CommonJS 写法
来源：http://tkr.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://evk.ydjk.org.cn

[U85] JS：可选链
来源：http://ixl.epnwcf.com

a?.b?.c
来源：http://vdi.jlsjyb.cn

[U86] JS：空值合并
来源：http://frx.ivvv.top

a ?? b
来源：http://pnb.yonumen.top

[U87] JS：解构默认值
来源：http://hnr.tanke756.top

const { a = 1, b = 2 } = obj;
来源：http://hsc.cashguo.top

[U88] JS：对象展开合并
来源：http://cty.jinyuanbaomall.cn

{ ...a, ...b }
来源：http://cmx.zhiwuduotai.top

[U89] JS：数组去重
来源：http://fuh.ybcxt.top

[...new Set(arr)]
来源：http://zvm.dianchejie.cn

[U90] JS：数字数组排序
来源：http://fqy.smart0.xyz

[...arr].sort((a, b) => a - b)
来源：http://xmf.pycfn.com

[U91] JS：对象键值遍历
来源：http://orm.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tci.xziqi.cn

[U92] JS：深拷贝
来源：http://tcx.mhx1999.top

structuredClone(obj)
来源：http://uua.xuanzx.com

[U93] JS：模板字符串
来源：http://ocy.yj202588.top

`共 ${n} 条`
来源：http://ngh.jlsjyb.cn

[U94] JS：箭头函数
来源：http://ffn.jinghuilouyu.cn

const double = x => x * 2;
来源：http://wmg.yongpay.top

[U95] JS：Promise 包装
来源：http://vgh.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://eua.jyoumei.cn

[U96] JS：async/await 与异常
来源：http://qjs.jlsjyb.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lvc.yongpay.top

[U97] JS：并发请求
来源：http://mpk.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://itq.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://xjw.cucudq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbs.hongshengwenyu.top

[U99] JS：事件监听
来源：http://qpg.hongshengwenyu.top

el.addEventListener("click", e => {})
来源：http://hxy.sufxvd.cn

[U100] JS：DOM 查询
来源：http://msk.hcnkem.com

document.querySelector(".item")
来源：http://yzb.hnxiangtu.top

[U101] JS：classList 操作
来源：http://prd.nanxinkj.top

el.classList.toggle("active")
来源：http://gyl.hongshengwenyu.top

[U102] JS：本地存储
来源：http://gpv.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ruz.hnxiangtu.top

[U103] JS：定时器
来源：http://yts.ydzc1.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vjs.fktsv.cn

[U104] JS：防抖
来源：http://emt.jinyuanbaomall.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqg.mhx1999.top

[U105] JS：节流
来源：http://syw.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://swa.tianlin.xyz

[U106] JS：日期格式化
来源：http://dru.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pol.meibo888.top

[U107] JS：数字千分位
来源：http://vhj.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qjq.zhongyouzk.top

[U108] JS：随机整数
来源：http://won.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hbe.wangdashe.top

[U109] JS：数组分组
来源：http://ogm.nanxuanxn.top

Object.groupBy(arr, x => x.type)
来源：http://eyg.yueranfly.top

[U110] JS：数组分块
来源：http://dag.wangshuangyany.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ryl.shzxlz.cn

[U111] JS：对象转 Map
来源：http://tca.xylfe.cn

new Map(Object.entries(obj))
来源：http://jos.yuanzhike.top

[U112] JS：字符串补位
来源：http://ukp.jiagoushi.top

"7".padStart(3, "0")
来源：http://swc.hywenlv.cn

[U113] JS：正则替换全部
来源：http://ubw.vqdsnc.cn

s.replaceAll("a", "b")
来源：http://hwe.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://ytl.hysaishi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ppv.fzhhl.top

[U115] JS：生成 UUID
来源：http://mpm.hywenlv.cn

crypto.randomUUID()
来源：http://vbm.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://xvz.tian-w.cn

/** @param {string} name */ function f(name) {}
来源：http://dun.sxryk.cn

[U117] JS：单元测试
来源：http://vth.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://tuv.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://eaq.tarul.cn

npm i -D vite;  npx vite
来源：http://zdo.yangfankeji.com

[U119] JS：生产构建
来源：http://wjc.yvedp.cn

npx vite build
来源：http://xou.sufxvd.cn

[U120] JS：读取环境变量（Vite）
来源：http://eog.yongpay.top

import.meta.env.VITE_API_URL
来源：http://xjs.jianghu66.top

================================================================================
来源：http://gdp.gotoacloud.top

统计汇总
来源：http://hen.0kj1m.cn

================================================================================
来源：http://wvo.haohaochexian.top

按语言统计（条）：
来源：http://cqt.shuidangran.top

Python ......... 252
来源：http://kbe.yfazqb.com

PHP ............ 252
来源：http://tvb.316326.xyz

JavaScript ..... 252
来源：http://pbq.xziqi.cn

TypeScript ..... 212
来源：http://bcy.yj20258.top

Java ........... 212
来源：http://acz.shanyushiyangkeji.top

Go ............. 212
来源：http://qnu.xingfuxueyuan.xyz

Ruby ........... 212
来源：http://hup.hysaishi.cn

C# ............. 212
来源：http://fyh.jinqigufen.top

C .............. 30
来源：http://adn.xziqi.cn

C++ ............ 30
来源：http://rma.zhengqikj.top

SQL ............ 90
来源：http://bxs.aizwys.cn

Bash ........... 80
来源：http://tqw.chenlongwang.top

Kotlin ......... 15
来源：http://uvf.316326.xyz

Swift .......... 15
来源：http://rle.hesvh.cn

Lua ............ 10
来源：http://hlb.yuxming.cn

Perl ........... 10
来源：http://tad.9152youxi.cn

Scala .......... 10
来源：http://bnl.yuxming.cn

------------------------------------
来源：http://hyc.nanxuanxn.top

合计 ........... 2106 条
来源：http://qsv.xziqi.cn

按章节统计：
来源：http://ccv.zhijiandao.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cbj.nwbrower.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xjh.yanxiufei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ghb.shanyushiyangtech.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://itc.daria6918.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nsc.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hat.xinyue.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wfm.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zbs.yj20258888.top


<!-- 参考信息 -->