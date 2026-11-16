代发 wailian999

[T47] Perl：正则捕获
来源：http://mlq.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tuf.hnqzz.top

[T48] Perl：正则替换
来源：http://bgh.52xcode.cn

$s =~ s/old/new/g;
来源：http://wsc.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://don.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lrm.jianghu66.top

[T50] Perl：逐行读文件
来源：http://dcx.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://icn.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://oyy.jqgufenzy.top

[T51] Scala：Hello World
来源：http://hrh.hesvh.cn

println("Hello")
来源：http://avf.xinyue.icu

[T52] Scala：变量
来源：http://vmv.gogol.net.cn

val a = 1;  var b = 2
来源：http://wde.hfpthk.cn

[T53] Scala：字符串插值
来源：http://eig.zhoulong.xyz

s"值: $b"
来源：http://evr.jqgufenzy.top

[T54] Scala：集合映射
来源：http://vdh.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://tiq.nanxinkj.top

[T55] Scala：集合过滤
来源：http://fki.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://uvi.hfpthk.cn

[T56] Scala：样例类
来源：http://ass.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://tqn.ppjwa.cn

[T57] Scala：模式匹配
来源：http://ojl.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eux.nanxinkj.top

[T58] Scala：函数定义
来源：http://sli.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://vvn.jqgfzy.top

[T59] Scala：循环
来源：http://oix.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://ymc.xinyue.icu

[T60] Scala：折叠
来源：http://ybk.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jrd.yonumen.top

================================================================================
来源：http://jsl.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ory.zycfv.cn

================================================================================
来源：http://ibs.yangfankeji.com

[U01] Py：创建虚拟环境
来源：http://zdy.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hre.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://cec.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://emv.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://bac.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lsy.bjfxy.top

[U04] Py：变量调试打印
来源：http://nak.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ldq.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://zcn.yonumen.top

list(dict.fromkeys(arr))
来源：http://cnc.yongpay.top

[U06] Py：合并两个字典
来源：http://dvk.shangyingyoupin.top

{**a, **b}
来源：http://gon.yuxming.cn

[U07] Py：反转字典键值
来源：http://ngw.tanke756.top

{v: k for k, v in d.items()}
来源：http://vsh.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://rjd.svipenyu.cn

[y for x in nested for y in x]
来源：http://spp.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://rsf.cheryme.top

max(d, key=d.get)
来源：http://nlg.yfazqb.com

[U10] Py：按值排序字典
来源：http://pyq.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://elg.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://caz.sufxvd.cn

(x * 2 for x in arr)
来源：http://fbb.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tzc.xylfe.cn

Counter(arr).most_common(3)
来源：http://ctk.fzhhl.top

[U13] Py：固定长度队列
来源：http://uxz.sysykeji.top

deque(maxlen=10)
来源：http://igb.c1oappe.top

[U14] Py：分组收集到列表
来源：http://ghg.cashguo.top

defaultdict(list)
来源：http://rly.sufxvd.cn

[U15] Py：高精度计时
来源：http://kqo.dashuyun.cn

t = time.perf_counter()
来源：http://edw.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://dmt.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mvv.aibaodan.cn

[U17] Py：初始化日志
来源：http://lon.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://yss.cucudq.cn

[U18] Py：预编译正则
来源：http://rjr.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://afn.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://ehz.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lnx.bjfxy.top

[U20] Py：缓存函数结果
来源：http://oqn.sysykeji.top

@functools.lru_cache(maxsize=None)
来源：http://jvh.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://red.havefunace.top

@contextlib.contextmanager
来源：http://bai.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://tnt.xuetiantiany.cn

list(zip(*m))
来源：http://eko.c1oappe.top

[U23] Py：分块读取大文件
来源：http://pxw.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iza.sufxvd.cn

[U24] Py：路径操作
来源：http://icq.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gwo.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://pbf.meibo888.top

csv.DictReader(f)
来源：http://cae.tanke756.top

[U26] Py：并发下载
来源：http://yxk.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mlc.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://ohh.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://kfg.tian-w.cn

[U28] Py：类型别名
来源：http://enz.fktsv.cn

UserId = int
来源：http://gih.jqgufenzy.top

[U29] Py：属性校验
来源：http://cck.aibaodan.cn

@property 与 @x.setter 配合
来源：http://rmy.birdmap.top

[U30] Py：数据类
来源：http://kob.zdbjq.cn

@dataclass(slots=True)
来源：http://aub.xuetiantiany.cn

[U31] Py：单测
来源：http://fby.fanxiaobao.xyz

python -m pytest -q
来源：http://jbl.sysykeji.top

[U32] Py：代码格式化
来源：http://cah.52xcode.cn

ruff format . && ruff check --fix .
来源：http://ffg.shangyingyoupin.top

[U33] Py：打包发布
来源：http://dnq.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://orj.yonumen.top

[U34] Py：判断编码
来源：http://kor.tanke756.top

chardet.detect(raw)
来源：http://qvh.iojbl.cn

[U35] Py：发送邮件
来源：http://zau.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://myf.ehwqpu.com

[U36] Py：定时任务
来源：http://eyj.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://rsh.yj20258888.top

[U37] Py：读写 Excel
来源：http://zez.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://qll.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://ulj.xuanzx.com

Path(__file__).resolve().parent
来源：http://spc.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://rkn.yj20258.top

sys.stdout.isatty()
来源：http://cao.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://ggz.9152youxi.cn

print("err", file=sys.stderr)
来源：http://jgi.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://qlr.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://drb.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://evr.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujl.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://cml.yuanzhike.top

namespace App\Http;
来源：http://qwm.nanxuanxn.top

[U44] PHP：开启严格类型
来源：http://spy.jinqigfzy.top

declare(strict_types=1);
来源：http://jmi.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://ziz.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ydq.aizwys.cn

[U46] PHP：可空类型
来源：http://sge.ywan-chungtsiang.top

?string $name = null
来源：http://wjf.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://ima.tarul.cn

int|string $id
来源：http://ktl.jqgfzy.top

[U48] PHP：纯枚举
来源：http://ijg.bjfxy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdn.ehwqpu.com

[U49] PHP：只读属性
来源：http://odk.hongshengwenyu.top

public readonly string $name
来源：http://wgq.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://fis.birdmap.top

public function __construct(private int $id) {}
来源：http://rzj.tianlin.xyz

[U51] PHP：数组解构
来源：http://onu.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://xth.tarul.cn

[U52] PHP：箭头函数
来源：http://axm.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://mrj.jiagoushi.top

[U53] PHP：空合并运算符
来源：http://jxv.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://ymk.iojbl.cn

[U54] PHP：空安全调用
来源：http://ebg.zhengqikj.top

$obj?->method()
来源：http://uij.ppjwa.cn

[U55] PHP：match 表达式
来源：http://xdf.feifeiyinyue.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ffo.yj20258.top

[U56] PHP：命名参数
来源：http://abd.ehwqpu.com

f(a: 1, b: 2)
来源：http://nyr.svipenyu.cn

[U57] PHP：字符串插值
来源：http://jus.xuetiantiany.cn

"值: {$a}"
来源：http://koy.tanke756.top

[U58] PHP：数组三件套
来源：http://zea.tarul.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iaj.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://jho.sweek.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rog.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://wzq.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nvo.fktsv.cn

[U61] PHP：正则
来源：http://wha.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ilb.yj20258.top

[U62] PHP：日期对象
来源：http://yts.guowangkeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sjt.gogol.net.cn

[U63] PHP：文件读写
来源：http://tqu.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lsp.aizwys.cn

[U64] PHP：目录遍历
来源：http://mem.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://fdx.jianghu66.top

[U65] PHP：会话
来源：http://fgz.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kio.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://vwt.shuidangran.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xnn.52xcode.cn

[U67] PHP：处理文件上传
来源：http://ezi.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ytf.yuxming.cn

[U68] PHP：PDO 连接
来源：http://jyv.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vux.jlsjyb.cn

[U69] PHP：PDO 预处理
来源：http://isd.xylfe.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://akj.wangdashe.top

[U70] PHP：PDO 事务
来源：http://ijk.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jsm.cucudq.cn

[U71] PHP：抛出异常
来源：http://dek.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://lhd.pycfn.com

[U72] PHP：写错误日志
来源：http://rjr.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://sgq.xylfe.cn

[U73] PHP：读取 ini 配置
来源：http://rbl.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://tzs.hammf.cn

[U74] PHP：读取环境变量
来源：http://mfh.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://hwf.bbcook.cn

[U75] PHP：依赖注入
来源：http://zbl.gaohongyu789.top

composer require psr/container
来源：http://sen.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://alr.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ppv.havefunace.top

[U77] PHP：模板渲染
来源：http://asn.chenzaomai.com

composer require twig/twig
来源：http://dxx.svipenyu.cn

[U78] PHP：单元测试
来源：http://fzo.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://kru.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://xtr.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://fjb.sweek.top

[U80] PHP：代码规范修复
来源：http://ckj.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://flo.hnxiangtu.top

[U81] JS：初始化项目
来源：http://mww.andypj.xyz

npm init -y;  npm i express
来源：http://jgn.xinyue.icu

[U82] JS：package.json 脚本
来源：http://ntn.vehdjk.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yzf.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://xpl.xingfuxueyuan.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://yzr.tarul.cn

[U84] JS：CommonJS 写法
来源：http://tzi.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://zub.xylfe.cn

[U85] JS：可选链
来源：http://vfn.aizwys.cn

a?.b?.c
来源：http://gjp.redwolf501.top

[U86] JS：空值合并
来源：http://dlg.yangfankeji.com

a ?? b
来源：http://isj.52xcode.cn

[U87] JS：解构默认值
来源：http://gzi.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://rkx.hnxiangtu.top

[U88] JS：对象展开合并
来源：http://zsg.shuidangran.top

{ ...a, ...b }
来源：http://bne.jinqigufen.top

[U89] JS：数组去重
来源：http://apn.yj20258.top

[...new Set(arr)]
来源：http://gic.jinqigufen.top

[U90] JS：数字数组排序
来源：http://zrq.zhongyouzk.top

[...arr].sort((a, b) => a - b)
来源：http://jjk.316326.xyz

[U91] JS：对象键值遍历
来源：http://tfh.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ebc.hysaishi.cn

[U92] JS：深拷贝
来源：http://stk.vqdsnc.cn

structuredClone(obj)
来源：http://onb.yvedp.cn

[U93] JS：模板字符串
来源：http://zvz.sweek.top

`共 ${n} 条`
来源：http://fle.uphjek.com

[U94] JS：箭头函数
来源：http://pzm.zhongyouzk.top

const double = x => x * 2;
来源：http://xda.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://byb.zhijiandao.cn

new Promise((resolve, reject) => {})
来源：http://xru.iojbl.cn

[U96] JS：async/await 与异常
来源：http://kjx.cdnleiting.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ufz.haohaochexian.top

[U97] JS：并发请求
来源：http://fnp.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mfz.yuanzhike.top

[U98] JS：fetch 带 JSON
来源：http://bbe.zhiwuduotai.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dwd.bjfxy.top

[U99] JS：事件监听
来源：http://dap.c1oappe.top

el.addEventListener("click", e => {})
来源：http://zil.c1oappe.top

[U100] JS：DOM 查询
来源：http://wsw.yueranfly.top

document.querySelector(".item")
来源：http://jbp.wangshuangyany.cn

[U101] JS：classList 操作
来源：http://cnl.xylfe.cn

el.classList.toggle("active")
来源：http://ovj.yj20258888.top

[U102] JS：本地存储
来源：http://nzz.fengsongda.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://afw.0kj1m.cn

[U103] JS：定时器
来源：http://vcg.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eby.zhongyouzk.top

[U104] JS：防抖
来源：http://ybj.shzxlz.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oql.zhiwuduotai.top

[U105] JS：节流
来源：http://lfl.mhx1999.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://obr.gotoacloud.top

[U106] JS：日期格式化
来源：http://bns.nanxinkj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://deg.yanxiufei.cn

[U107] JS：数字千分位
来源：http://fus.quarkkingdee.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xhi.yj20258888.top

[U108] JS：随机整数
来源：http://zxc.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yxc.guowangkeji.top

[U109] JS：数组分组
来源：http://aks.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://cpg.mhx1999.top

[U110] JS：数组分块
来源：http://gby.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lje.daxiang520.top

[U111] JS：对象转 Map
来源：http://nxk.ppjwa.cn

new Map(Object.entries(obj))
来源：http://kgr.redwolf501.top

[U112] JS：字符串补位
来源：http://xlb.yuxming.cn

"7".padStart(3, "0")
来源：http://ioo.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://hgx.guowangkeji.top

s.replaceAll("a", "b")
来源：http://imn.chenjidiqi.icu

[U114] JS：JSON 深比较
来源：http://cbk.uphjek.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ser.vehdjk.com

[U115] JS：生成 UUID
来源：http://dzg.zhixingplan.top

crypto.randomUUID()
来源：http://nhr.chenlongwang.top

[U116] JS：类型检查（JSDoc）
来源：http://toh.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://zrd.hesvh.cn

[U117] JS：单元测试
来源：http://fxy.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://efi.meibo888.top

[U118] JS：开发服务器
来源：http://dqh.nanxuanxn.top

npm i -D vite;  npx vite
来源：http://vqu.xylfe.cn

[U119] JS：生产构建
来源：http://uyt.sufxvd.cn

npx vite build
来源：http://lzr.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://ruk.yonumen.top

import.meta.env.VITE_API_URL
来源：http://axo.yfazqb.com

================================================================================
来源：http://npe.xziqi.cn

统计汇总
来源：http://jfg.zhoulong.xyz

================================================================================
来源：http://wep.pengpengdd.cyou

按语言统计（条）：
来源：http://ivj.svipenyu.cn

Python ......... 252
来源：http://out.yonumen.top

PHP ............ 252
来源：http://owv.fengsongda.top

JavaScript ..... 252
来源：http://tqt.shuidangran.top

TypeScript ..... 212
来源：http://cek.cucudq.cn

Java ........... 212
来源：http://vth.fanxiaobao.xyz

Go ............. 212
来源：http://bby.shuidangran.top

Ruby ........... 212
来源：http://qtb.gotoacloud.top

C# ............. 212
来源：http://qxf.vqdsnc.cn

C .............. 30
来源：http://rpk.wangshuangyany.cn

C++ ............ 30
来源：http://rqc.chenlongwang.top

SQL ............ 90
来源：http://qlv.tian-w.cn

Bash ........... 80
来源：http://rag.zhiwuduotai.top

Kotlin ......... 15
来源：http://qxr.zhixingplan.top

Swift .......... 15
来源：http://udu.fktsv.cn

Lua ............ 10
来源：http://xkr.dashuyun.cn

Perl ........... 10
来源：http://ywv.yvedp.cn

Scala .......... 10
来源：http://oby.yongpay.top

------------------------------------
来源：http://cto.daria6918.cn

合计 ........... 2106 条
来源：http://byo.cheryme.top

按章节统计：
来源：http://yfg.jyoumei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jjq.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uva.aizwys.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hdg.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zxf.chenjidiqi.icu


<!-- 参考信息 -->