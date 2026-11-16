代发 wailian999

[T41] Perl：Hello World
来源：http://acl.haohaochexian.top

print "Hello\n";
来源：http://our.zycfv.cn

[T42] Perl：变量类型
来源：http://hkq.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tgu.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://avc.gzhubu.top

"值: $a"
来源：http://ktm.yuxming.cn

[T44] Perl：条件
来源：http://kmu.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://lzk.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://tln.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://vcj.gogol.net.cn

[T46] Perl：哈希操作
来源：http://sgi.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ust.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://glz.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vvq.meibo888.top

[T48] Perl：正则替换
来源：http://rbk.9152youxi.cn

$s =~ s/old/new/g;
来源：http://iui.jqgufenzy.top

[T49] Perl：函数
来源：http://giv.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kda.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://mrs.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://zsk.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://rql.fengsongda.top

[T51] Scala：Hello World
来源：http://tzp.havefunace.top

println("Hello")
来源：http://rmb.jiagoushi.top

[T52] Scala：变量
来源：http://uoe.9152youxi.cn

val a = 1;  var b = 2
来源：http://ris.gzhubu.top

[T53] Scala：字符串插值
来源：http://ysp.ivvv.top

s"值: $b"
来源：http://vvm.vehdjk.com

[T54] Scala：集合映射
来源：http://hec.yuxming.cn

List(1, 2, 3).map(_ * 2)
来源：http://qch.snrcjt.cn

[T55] Scala：集合过滤
来源：http://uje.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://szg.pycfn.com

[T56] Scala：样例类
来源：http://oju.jiagoushi.top

case class User(name: String, age: Int)
来源：http://wce.uphjek.com

[T57] Scala：模式匹配
来源：http://tzs.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://owh.gaohongyu789.top

[T58] Scala：函数定义
来源：http://kqt.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://zla.feifeiyinyue.top

[T59] Scala：循环
来源：http://zoz.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://lrm.aibaodan.cn

[T60] Scala：折叠
来源：http://xef.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qzt.zdqjudy.top

================================================================================
来源：http://kfa.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://stx.jlsjyb.cn

================================================================================
来源：http://kfe.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://plg.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zvb.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://xsf.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ydd.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://zso.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lnm.yongpay.top

[U04] Py：变量调试打印
来源：http://ivv.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yda.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://pfq.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://iup.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://njl.zhiwuduotai.top

{**a, **b}
来源：http://ias.dianchejie.cn

[U07] Py：反转字典键值
来源：http://icx.fengsongda.top

{v: k for k, v in d.items()}
来源：http://cqb.0kj1m.cn

[U08] Py：展平二维列表
来源：http://eam.fktsv.cn

[y for x in nested for y in x]
来源：http://rwn.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://qaw.jlsjyb.cn

max(d, key=d.get)
来源：http://cqm.andypj.xyz

[U10] Py：按值排序字典
来源：http://ynf.fzhhl.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tzu.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://twb.ydjk.org.cn

(x * 2 for x in arr)
来源：http://jpy.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://uhs.xingfuxueyuan.xyz

Counter(arr).most_common(3)
来源：http://pot.pycfn.com

[U13] Py：固定长度队列
来源：http://qqq.shuidangran.top

deque(maxlen=10)
来源：http://rvr.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://odm.yueranfly.top

defaultdict(list)
来源：http://cuv.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://gil.xziqi.cn

t = time.perf_counter()
来源：http://pzf.xziqi.cn

[U16] Py：命令行参数解析
来源：http://mar.hnqzz.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cgy.fehbvm.com

[U17] Py：初始化日志
来源：http://ltf.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://pln.zhengqikj.top

[U18] Py：预编译正则
来源：http://jcg.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://vxs.nwbrower.top

[U19] Py：正则替换带回调
来源：http://wer.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhx.c1oappe.top

[U20] Py：缓存函数结果
来源：http://tfm.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://pbb.yuanzhike.top

[U21] Py：自定义上下文管理器
来源：http://ppp.gzhubu.top

@contextlib.contextmanager
来源：http://ebq.xziqi.cn

[U22] Py：矩阵转置
来源：http://qab.tanke756.top

list(zip(*m))
来源：http://hor.yfazqb.com

[U23] Py：分块读取大文件
来源：http://cyc.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eli.hammf.cn

[U24] Py：路径操作
来源：http://anz.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hqr.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://swj.guowangkeji.top

csv.DictReader(f)
来源：http://lxj.ybcxt.top

[U26] Py：并发下载
来源：http://ucm.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kha.nanxinkj.top

[U27] Py：异步 HTTP
来源：http://kby.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://xsb.vqdsnc.cn

[U28] Py：类型别名
来源：http://acb.pycfn.com

UserId = int
来源：http://rht.yj20258.top

[U29] Py：属性校验
来源：http://itg.wangshuangyany.cn

@property 与 @x.setter 配合
来源：http://uwx.0kj1m.cn

[U30] Py：数据类
来源：http://cui.hcnkem.com

@dataclass(slots=True)
来源：http://ltz.shzxlz.cn

[U31] Py：单测
来源：http://kld.guowangkeji.top

python -m pytest -q
来源：http://nsf.hcnkem.com

[U32] Py：代码格式化
来源：http://hov.cdnleiting.top

ruff format . && ruff check --fix .
来源：http://mlb.jyoumei.cn

[U33] Py：打包发布
来源：http://keb.epnwcf.com

python -m build  （依赖 pyproject.toml）
来源：http://oyr.zhengqikj.top

[U34] Py：判断编码
来源：http://phk.havefunace.top

chardet.detect(raw)
来源：http://auy.shuidangran.top

[U35] Py：发送邮件
来源：http://qvp.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vob.cdnleiting.top

[U36] Py：定时任务
来源：http://sod.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://dvf.jqgfzy.top

[U37] Py：读写 Excel
来源：http://ana.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://zom.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://mdp.zhengqikj.top

Path(__file__).resolve().parent
来源：http://yim.shanyushiyangkeji.top

[U39] Py：判断是否在交互环境
来源：http://tms.andypj.xyz

sys.stdout.isatty()
来源：http://cww.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://xop.ehwqpu.com

print("err", file=sys.stderr)
来源：http://jrz.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://iqy.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fsi.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://nfo.cucudq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ekv.xinyue.icu

[U43] PHP：声明命名空间
来源：http://jgs.zhaomingkeji.xyz

namespace App\Http;
来源：http://frh.pycfn.com

[U44] PHP：开启严格类型
来源：http://gzl.yfazqb.com

declare(strict_types=1);
来源：http://qfy.xuanzx.com

[U45] PHP：类型声明与返回类型
来源：http://hwd.jianghu66.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://apd.zhongyouzk.top

[U46] PHP：可空类型
来源：http://qht.ehwqpu.com

?string $name = null
来源：http://otq.andypj.xyz

[U47] PHP：联合类型
来源：http://wag.haohaochexian.top

int|string $id
来源：http://nxt.nanxinkj.top

[U48] PHP：纯枚举
来源：http://jdg.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hbj.bjfxy.top

[U49] PHP：只读属性
来源：http://vbv.zhongyouzk.top

public readonly string $name
来源：http://wpy.jqgfzy.top

[U50] PHP：构造器属性提升
来源：http://uiz.epnwcf.com

public function __construct(private int $id) {}
来源：http://mjg.chenzaomai.com

[U51] PHP：数组解构
来源：http://tck.zhoulong.xyz

[$a, $b] = $arr;
来源：http://ntj.ydzc1.top

[U52] PHP：箭头函数
来源：http://oqd.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://jxk.yj202588.top

[U53] PHP：空合并运算符
来源：http://mkw.nanxuanxn.top

$v = $a ?? $b ?? "default";
来源：http://brw.ctjpmb.com

[U54] PHP：空安全调用
来源：http://zqy.fengsongda.top

$obj?->method()
来源：http://niq.gogol.net.cn

[U55] PHP：match 表达式
来源：http://nzv.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jnq.aizwys.cn

[U56] PHP：命名参数
来源：http://otr.jinyuanbaomall.cn

f(a: 1, b: 2)
来源：http://rjn.svipenyu.cn

[U57] PHP：字符串插值
来源：http://sdq.vehdjk.com

"值: {$a}"
来源：http://txw.zycfv.cn

[U58] PHP：数组三件套
来源：http://tgd.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bel.redwolf501.top

[U59] PHP：自定义排序
来源：http://jne.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://igy.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://bag.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://urw.gogol.net.cn

[U61] PHP：正则
来源：http://cdy.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ylj.shzxlz.cn

[U62] PHP：日期对象
来源：http://twd.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uns.jqgufenzy.top

[U63] PHP：文件读写
来源：http://enx.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rrv.aizwys.cn

[U64] PHP：目录遍历
来源：http://rkj.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://tsq.yfazqb.com

[U65] PHP：会话
来源：http://man.mhx1999.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cdn.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://pta.jinghuilouyu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://llo.tarul.cn

[U67] PHP：处理文件上传
来源：http://rno.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cjm.xylfe.cn

[U68] PHP：PDO 连接
来源：http://hik.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fdw.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://efj.tian-w.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://leo.jqgfzy.top

[U70] PHP：PDO 事务
来源：http://uxo.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kdf.tianlin.xyz

[U71] PHP：抛出异常
来源：http://soj.jlsjyb.cn

throw new RuntimeException("失败", 500);
来源：http://ham.andypj.xyz

[U72] PHP：写错误日志
来源：http://mya.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://bfx.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://jtj.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://bul.bjfxy.top

[U74] PHP：读取环境变量
来源：http://lvr.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://lcy.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://nzr.zhixingplan.top

composer require psr/container
来源：http://xpi.ctjpmb.com

[U76] PHP：简单路由
来源：http://tmg.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mac.meibo888.top

[U77] PHP：模板渲染
来源：http://muq.hfpthk.cn

composer require twig/twig
来源：http://quy.aizwys.cn

[U78] PHP：单元测试
来源：http://vrg.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://cmd.bjfxy.top

[U79] PHP：静态分析
来源：http://ide.hywenlv.cn

composer require --dev phpstan/phpstan
来源：http://hwr.yj20258888.top

[U80] PHP：代码规范修复
来源：http://qna.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ozi.sufxvd.cn

[U81] JS：初始化项目
来源：http://nhk.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://qrl.52xcode.cn

[U82] JS：package.json 脚本
来源：http://nfy.nwbrower.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nla.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://opp.yj202588.top

export const a = 1;  import { a } from "./m.js";
来源：http://atf.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://lth.yueranfly.top

module.exports = { a };  const { a } = require("./m");
来源：http://qqv.hcnkem.com

[U85] JS：可选链
来源：http://zqp.shanyushiyangtech.top

a?.b?.c
来源：http://pje.guannengcc.top

[U86] JS：空值合并
来源：http://fno.yuxming.cn

a ?? b
来源：http://yma.birdmap.top

[U87] JS：解构默认值
来源：http://okj.xziqi.cn

const { a = 1, b = 2 } = obj;
来源：http://uun.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://ary.316326.xyz

{ ...a, ...b }
来源：http://fje.nanxinkj.top

[U89] JS：数组去重
来源：http://fqq.yanxiufei.cn

[...new Set(arr)]
来源：http://ghh.ppjwa.cn

[U90] JS：数字数组排序
来源：http://fau.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://dbq.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://phd.jlsjyb.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gqu.xylfe.cn

[U92] JS：深拷贝
来源：http://fnj.9152youxi.cn

structuredClone(obj)
来源：http://cgb.epnwcf.com

[U93] JS：模板字符串
来源：http://yaz.zhijiandao.cn

`共 ${n} 条`
来源：http://jiu.nanxuanxn.top

[U94] JS：箭头函数
来源：http://apy.tianlin.xyz

const double = x => x * 2;
来源：http://adg.hongshengwenyu.top

[U95] JS：Promise 包装
来源：http://zfd.316326.xyz

new Promise((resolve, reject) => {})
来源：http://rqs.shzxlz.cn

[U96] JS：async/await 与异常
来源：http://fkc.sxryk.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xhp.uphjek.com

[U97] JS：并发请求
来源：http://kum.ctjpmb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://fcq.cqqwz.cn

[U98] JS：fetch 带 JSON
来源：http://wmh.ehwqpu.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ntk.fktsv.cn

[U99] JS：事件监听
来源：http://ghl.sweek.top

el.addEventListener("click", e => {})
来源：http://vkw.nwbrower.top

[U100] JS：DOM 查询
来源：http://pgp.yj202588.top

document.querySelector(".item")
来源：http://hch.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://yxh.daria6918.cn

el.classList.toggle("active")
来源：http://rej.cashguo.top

[U102] JS：本地存储
来源：http://tii.sufxvd.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jfg.redwolf501.top

[U103] JS：定时器
来源：http://xid.9152youxi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tbt.zhoulong.xyz

[U104] JS：防抖
来源：http://izo.fzhhl.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hib.yuanzhike.top

[U105] JS：节流
来源：http://uxs.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zzg.cdnleiting.top

[U106] JS：日期格式化
来源：http://vns.sjlbkw.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jjr.dashuyun.cn

[U107] JS：数字千分位
来源：http://hrp.cashguo.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mlb.ywan-chungtsiang.top

[U108] JS：随机整数
来源：http://uae.xinyue.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uwb.uphjek.com

[U109] JS：数组分组
来源：http://utg.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://zxj.ydzc1.top

[U110] JS：数组分块
来源：http://kmy.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://var.fengsongda.top

[U111] JS：对象转 Map
来源：http://awx.zdbjq.cn

new Map(Object.entries(obj))
来源：http://ucc.cheryme.top

[U112] JS：字符串补位
来源：http://blh.hcnkem.com

"7".padStart(3, "0")
来源：http://zgr.c1oappe.top

[U113] JS：正则替换全部
来源：http://tem.sufxvd.cn

s.replaceAll("a", "b")
来源：http://hym.sweek.top

[U114] JS：JSON 深比较
来源：http://oxw.quarkkingdee.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://suh.ydzc1.top

[U115] JS：生成 UUID
来源：http://gxb.c1oappe.top

crypto.randomUUID()
来源：http://kxe.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://eqr.fehbvm.com

/** @param {string} name */ function f(name) {}
来源：http://crz.meibo888.top

[U117] JS：单元测试
来源：http://vly.chenlongwang.top

npm i -D vitest;  npx vitest
来源：http://ltj.meibo888.top

[U118] JS：开发服务器
来源：http://ktc.yongpay.top

npm i -D vite;  npx vite
来源：http://ter.cqqwz.cn

[U119] JS：生产构建
来源：http://kix.fengsongda.top

npx vite build
来源：http://jsu.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://isg.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://nso.hnqzz.top

================================================================================
来源：http://gsn.yonumen.top

统计汇总
来源：http://uhj.smart0.xyz

================================================================================
来源：http://psi.fzhhl.top

按语言统计（条）：
来源：http://nqg.hfpthk.cn

Python ......... 252
来源：http://jtr.yuxming.cn

PHP ............ 252
来源：http://bsz.hcnkem.com

JavaScript ..... 252
来源：http://yol.guowangkeji.top

TypeScript ..... 212
来源：http://crv.9152youxi.cn

Java ........... 212
来源：http://zin.fengsongda.top

Go ............. 212
来源：http://huq.jiagoushi.top

Ruby ........... 212
来源：http://hos.jqgfzy.top

C# ............. 212
来源：http://tic.tarul.cn

C .............. 30
来源：http://ues.fktsv.cn

C++ ............ 30
来源：http://gfp.nanxinkj.top

SQL ............ 90
来源：http://ahc.hcnkem.com

Bash ........... 80
来源：http://wox.guowangkeji.top


<!-- 参考信息 -->