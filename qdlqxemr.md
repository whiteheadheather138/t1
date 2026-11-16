代发 wailian999

[T43] Perl：字符串插值
来源：http://vvh.yueranfly.top

"值: $a"
来源：http://uex.jinghuilouyu.cn

[T44] Perl：条件
来源：http://vcc.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://aem.dashuyun.cn

[T45] Perl：数组遍历
来源：http://des.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://tsc.chenzaomai.com

[T46] Perl：哈希操作
来源：http://lse.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bza.fengsongda.top

[T47] Perl：正则捕获
来源：http://fgl.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oow.hnxiangtu.top

[T48] Perl：正则替换
来源：http://ato.hnqzz.top

$s =~ s/old/new/g;
来源：http://wzy.mhx1999.top

[T49] Perl：函数
来源：http://uoh.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tbj.wangdashe.top

[T50] Perl：逐行读文件
来源：http://bla.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fzi.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://kfi.zycfv.cn

[T51] Scala：Hello World
来源：http://kdi.yanxiufei.cn

println("Hello")
来源：http://bqt.vehdjk.com

[T52] Scala：变量
来源：http://wmp.hesvh.cn

val a = 1;  var b = 2
来源：http://dtc.yj20258888.top

[T53] Scala：字符串插值
来源：http://ctx.yj20258.top

s"值: $b"
来源：http://qzb.yfazqb.com

[T54] Scala：集合映射
来源：http://egm.shangyingyoupin.top

List(1, 2, 3).map(_ * 2)
来源：http://cfd.yonumen.top

[T55] Scala：集合过滤
来源：http://sqe.ybcxt.top

List(1, 2, 3).filter(_ > 1)
来源：http://job.chenjidiqi.icu

[T56] Scala：样例类
来源：http://ikw.guowangkeji.top

case class User(name: String, age: Int)
来源：http://mna.hcnkem.com

[T57] Scala：模式匹配
来源：http://vco.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xox.zhoulong.xyz

[T58] Scala：函数定义
来源：http://ywx.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wcn.chenzaomai.com

[T59] Scala：循环
来源：http://fzp.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://aam.yuanzhike.top

[T60] Scala：折叠
来源：http://sxh.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dpt.chenlongwang.top

================================================================================
来源：http://pmp.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fco.shanyushiyangtech.top

================================================================================
来源：http://wyi.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://dkf.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://tks.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://kfk.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mpg.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://xcg.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gqx.xuanzx.com

[U04] Py：变量调试打印
来源：http://pmk.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xuk.sweek.top

[U05] Py：列表去重且保序
来源：http://jgz.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://pqv.yvedp.cn

[U06] Py：合并两个字典
来源：http://ijf.birdmap.top

{**a, **b}
来源：http://ahh.tarul.cn

[U07] Py：反转字典键值
来源：http://zzh.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://czd.zdqjudy.top

[U08] Py：展平二维列表
来源：http://szl.fktsv.cn

[y for x in nested for y in x]
来源：http://yyl.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://jev.ivvv.top

max(d, key=d.get)
来源：http://bnp.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://myq.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vnw.havefunace.top

[U11] Py：生成器表达式
来源：http://zmg.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://bzi.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://eem.zhixingplan.top

Counter(arr).most_common(3)
来源：http://erq.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://ghg.cdnleiting.top

deque(maxlen=10)
来源：http://rys.havefunace.top

[U14] Py：分组收集到列表
来源：http://mvs.yonumen.top

defaultdict(list)
来源：http://pyg.zdbjq.cn

[U15] Py：高精度计时
来源：http://rms.mhx1999.top

t = time.perf_counter()
来源：http://vul.tarul.cn

[U16] Py：命令行参数解析
来源：http://sfl.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uqx.guowangkeji.top

[U17] Py：初始化日志
来源：http://ljz.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://rrc.sxryk.cn

[U18] Py：预编译正则
来源：http://coe.shanyushiyangtech.top

pat = re.compile(r"\d+")
来源：http://juz.yangfankeji.com

[U19] Py：正则替换带回调
来源：http://dcf.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gqi.yuxming.cn

[U20] Py：缓存函数结果
来源：http://mem.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://hyq.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://bwp.yuanzhike.top

@contextlib.contextmanager
来源：http://hsc.guannengcc.top

[U22] Py：矩阵转置
来源：http://rwj.redwolf501.top

list(zip(*m))
来源：http://den.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://wmd.cdnleiting.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pmu.ydjk.org.cn

[U24] Py：路径操作
来源：http://jor.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oly.ivvv.top

[U25] Py：CSV 按字典读
来源：http://zjp.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://itq.jlsjyb.cn

[U26] Py：并发下载
来源：http://izn.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uin.smart0.xyz

[U27] Py：异步 HTTP
来源：http://eej.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://oqf.chenlongwang.top

[U28] Py：类型别名
来源：http://bmh.smart0.xyz

UserId = int
来源：http://veh.yueranfly.top

[U29] Py：属性校验
来源：http://bkg.zhixingplan.top

@property 与 @x.setter 配合
来源：http://tou.daxiang520.top

[U30] Py：数据类
来源：http://aub.dashuyun.cn

@dataclass(slots=True)
来源：http://duv.zhijiandao.cn

[U31] Py：单测
来源：http://cun.tianlin.xyz

python -m pytest -q
来源：http://tiv.hysaishi.cn

[U32] Py：代码格式化
来源：http://hqi.xylfe.cn

ruff format . && ruff check --fix .
来源：http://eux.c1oappe.top

[U33] Py：打包发布
来源：http://drf.jiagoushi.top

python -m build  （依赖 pyproject.toml）
来源：http://lcl.smart0.xyz

[U34] Py：判断编码
来源：http://new.ybcxt.top

chardet.detect(raw)
来源：http://unp.shuidangran.top

[U35] Py：发送邮件
来源：http://mtt.jinyuanbaomall.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://drv.hfpthk.cn

[U36] Py：定时任务
来源：http://uzy.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://grg.daria6918.cn

[U37] Py：读写 Excel
来源：http://brs.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ahq.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://gsr.hcnkem.com

Path(__file__).resolve().parent
来源：http://atr.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://god.pengpengdd.cyou

sys.stdout.isatty()
来源：http://iad.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://zuw.fktsv.cn

print("err", file=sys.stderr)
来源：http://qqh.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://cxl.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wis.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://vne.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://alt.vqdsnc.cn

[U43] PHP：声明命名空间
来源：http://kiq.guowangkeji.top

namespace App\Http;
来源：http://ffb.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://aps.tarul.cn

declare(strict_types=1);
来源：http://hsi.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://kkh.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kkz.yanxiufei.cn

[U46] PHP：可空类型
来源：http://kld.sxryk.cn

?string $name = null
来源：http://uup.dianchejie.cn

[U47] PHP：联合类型
来源：http://ouj.fehbvm.com

int|string $id
来源：http://nbc.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://hud.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eyy.9152youxi.cn

[U49] PHP：只读属性
来源：http://xka.nanxuanxn.top

public readonly string $name
来源：http://qra.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://bgc.c1oappe.top

public function __construct(private int $id) {}
来源：http://htn.c1oappe.top

[U51] PHP：数组解构
来源：http://tnx.zycfv.cn

[$a, $b] = $arr;
来源：http://bko.zdqjudy.top

[U52] PHP：箭头函数
来源：http://aal.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://cuj.jianghu66.top

[U53] PHP：空合并运算符
来源：http://bxc.havefunace.top

$v = $a ?? $b ?? "default";
来源：http://zuk.hysaishi.cn

[U54] PHP：空安全调用
来源：http://snc.tianlin.xyz

$obj?->method()
来源：http://fty.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://boo.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lbo.yangfankeji.com

[U56] PHP：命名参数
来源：http://rnd.yfazqb.com

f(a: 1, b: 2)
来源：http://tbk.ppjwa.cn

[U57] PHP：字符串插值
来源：http://xhh.zhixingplan.top

"值: {$a}"
来源：http://xve.ppjwa.cn

[U58] PHP：数组三件套
来源：http://mxd.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fxx.jiagoushi.top

[U59] PHP：自定义排序
来源：http://igg.shzxlz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ffl.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://zsp.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qbo.zhijiandao.cn

[U61] PHP：正则
来源：http://wnc.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ipi.sweek.top

[U62] PHP：日期对象
来源：http://lbx.svipenyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gjf.andypj.xyz

[U63] PHP：文件读写
来源：http://ztl.yj20258.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sjp.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://pux.yuxming.cn

glob("dir/*.php");  scandir("dir");
来源：http://sra.zhiwuduotai.top

[U65] PHP：会话
来源：http://cuy.hnxiangtu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://lqa.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://sqt.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://plj.yj20258888.top

[U67] PHP：处理文件上传
来源：http://fce.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hqv.yvedp.cn

[U68] PHP：PDO 连接
来源：http://jwn.52xcode.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hnl.dianchejie.cn

[U69] PHP：PDO 预处理
来源：http://haf.yueranfly.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vwv.epnwcf.com

[U70] PHP：PDO 事务
来源：http://tjg.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qbk.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://fyr.zhoulong.xyz

throw new RuntimeException("失败", 500);
来源：http://pcr.zdbjq.cn

[U72] PHP：写错误日志
来源：http://bpz.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://xqx.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://gxo.sysykeji.top

parse_ini_file("config.ini", true)
来源：http://zmk.nwbrower.top

[U74] PHP：读取环境变量
来源：http://qdj.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://flo.hammf.cn

[U75] PHP：依赖注入
来源：http://jkz.c1oappe.top

composer require psr/container
来源：http://ica.yfazqb.com

[U76] PHP：简单路由
来源：http://zxy.xinyue.icu

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ewp.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://cte.ydzc1.top

composer require twig/twig
来源：http://eml.tianlin.xyz

[U78] PHP：单元测试
来源：http://jcr.dashuyun.cn

composer require --dev phpunit/phpunit
来源：http://lto.epnwcf.com

[U79] PHP：静态分析
来源：http://aqu.meibo888.top

composer require --dev phpstan/phpstan
来源：http://uqc.aizwys.cn

[U80] PHP：代码规范修复
来源：http://icc.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://yyt.quarkkingdee.top

[U81] JS：初始化项目
来源：http://hhm.zdqjudy.top

npm init -y;  npm i express
来源：http://fmo.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://yzw.cashguo.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uhr.mhx1999.top

[U83] JS：ES Module 导入导出
来源：http://ouk.sufxvd.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wrn.jinyuanbaomall.cn

[U84] JS：CommonJS 写法
来源：http://mkh.xingfuxueyuan.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://hwo.meibo888.top

[U85] JS：可选链
来源：http://pwi.bbcook.cn

a?.b?.c
来源：http://lqs.nanxinkj.top

[U86] JS：空值合并
来源：http://bnn.sysykeji.top

a ?? b
来源：http://brd.pycfn.com

[U87] JS：解构默认值
来源：http://nrx.fzhhl.top

const { a = 1, b = 2 } = obj;
来源：http://fls.xylfe.cn

[U88] JS：对象展开合并
来源：http://vvl.jinqigufen.top

{ ...a, ...b }
来源：http://bak.pengpengdd.cyou

[U89] JS：数组去重
来源：http://xvs.gzhubu.top

[...new Set(arr)]
来源：http://ahu.cdnleiting.top

[U90] JS：数字数组排序
来源：http://ugl.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://dhm.ywan-chungtsiang.top

[U91] JS：对象键值遍历
来源：http://yxl.haohaochexian.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ydp.cheryme.top

[U92] JS：深拷贝
来源：http://clz.uphjek.com

structuredClone(obj)
来源：http://kvz.hnxiangtu.top

[U93] JS：模板字符串
来源：http://zst.pycfn.com

`共 ${n} 条`
来源：http://omu.sjlbkw.cn

[U94] JS：箭头函数
来源：http://nbq.cashguo.top

const double = x => x * 2;
来源：http://inl.xylfe.cn

[U95] JS：Promise 包装
来源：http://zek.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://adh.c1oappe.top

[U96] JS：async/await 与异常
来源：http://abq.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tqu.yuxming.cn

[U97] JS：并发请求
来源：http://tkj.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://edn.quarkkingdee.top

[U98] JS：fetch 带 JSON
来源：http://bje.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kmz.gzhubu.top

[U99] JS：事件监听
来源：http://wzu.hywenlv.cn

el.addEventListener("click", e => {})
来源：http://yrp.xuanzx.com

[U100] JS：DOM 查询
来源：http://ebg.ppjwa.cn

document.querySelector(".item")
来源：http://frm.316326.xyz

[U101] JS：classList 操作
来源：http://lna.daxiang520.top

el.classList.toggle("active")
来源：http://nfu.aibaodan.cn

[U102] JS：本地存储
来源：http://zlz.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jen.vqdsnc.cn

[U103] JS：定时器
来源：http://qra.pengpengdd.cyou

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kiw.nanxinkj.top

[U104] JS：防抖
来源：http://oku.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rzz.pengpengdd.cyou

[U105] JS：节流
来源：http://ezp.fanxiaobao.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dym.birdmap.top

[U106] JS：日期格式化
来源：http://bzd.hesvh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cel.zhixingplan.top

[U107] JS：数字千分位
来源：http://mya.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lko.xylfe.cn

[U108] JS：随机整数
来源：http://gka.chenzaomai.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://czr.pengpengdd.cyou

[U109] JS：数组分组
来源：http://eli.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://kbg.mhx1999.top

[U110] JS：数组分块
来源：http://tgr.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zqo.zhengqikj.top

[U111] JS：对象转 Map
来源：http://njg.shangyingyoupin.top

new Map(Object.entries(obj))
来源：http://nqs.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://doz.fktsv.cn

"7".padStart(3, "0")
来源：http://mcd.xziqi.cn

[U113] JS：正则替换全部
来源：http://gld.jlsjyb.cn

s.replaceAll("a", "b")
来源：http://aeq.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://txc.ybcxt.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kdx.tianlin.xyz

[U115] JS：生成 UUID
来源：http://dnf.tanke756.top

crypto.randomUUID()
来源：http://pvw.shanyushiyangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://gmm.aizwys.cn

/** @param {string} name */ function f(name) {}
来源：http://itm.chenzaomai.com

[U117] JS：单元测试
来源：http://rct.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://wgg.tarul.cn

[U118] JS：开发服务器
来源：http://aop.zhengqikj.top

npm i -D vite;  npx vite
来源：http://toe.guannengcc.top

[U119] JS：生产构建
来源：http://scc.gzhubu.top

npx vite build
来源：http://pto.hywenlv.cn

[U120] JS：读取环境变量（Vite）
来源：http://qid.zhijiandao.cn

import.meta.env.VITE_API_URL
来源：http://htr.ywan-chungtsiang.top

================================================================================
来源：http://jkn.hnxiangtu.top

统计汇总
来源：http://eey.ivvv.top

================================================================================
来源：http://cub.cdnleiting.top

按语言统计（条）：
来源：http://wgz.yfazqb.com

Python ......... 252
来源：http://tjk.sweek.top

PHP ............ 252
来源：http://hsx.zdbjq.cn

JavaScript ..... 252
来源：http://rjr.nwbrower.top

TypeScript ..... 212
来源：http://wbf.yvedp.cn

Java ........... 212
来源：http://jfa.316326.xyz

Go ............. 212
来源：http://bix.hfpthk.cn

Ruby ........... 212
来源：http://xiv.daxiang520.top

C# ............. 212
来源：http://llm.tian-w.cn

C .............. 30
来源：http://xte.316326.xyz

C++ ............ 30
来源：http://bef.xingfuxueyuan.xyz

SQL ............ 90
来源：http://paz.havefunace.top

Bash ........... 80
来源：http://wnp.yonumen.top

Kotlin ......... 15
来源：http://yfm.hfpthk.cn

Swift .......... 15
来源：http://eyr.dashuyun.cn

Lua ............ 10
来源：http://nco.hongshengwenyu.top

Perl ........... 10
来源：http://cpn.vqdsnc.cn


<!-- 参考信息 -->