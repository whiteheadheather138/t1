代发 wailian999

[T39] Lua：模式匹配
来源：http://zgs.shangyingyoupin.top

string.find(s, "%d+")
来源：http://yig.jinqigfzy.top

[T40] Lua：元表
来源：http://lon.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://mdn.hfpthk.cn

[T41] Perl：Hello World
来源：http://fsh.hnqzz.top

print "Hello\n";
来源：http://lay.c1oappe.top

[T42] Perl：变量类型
来源：http://pny.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gfz.c1oappe.top

[T43] Perl：字符串插值
来源：http://xqy.vehdjk.com

"值: $a"
来源：http://ejn.yueranfly.top

[T44] Perl：条件
来源：http://tke.ivvv.top

if ($a > 0) { print "正"; }
来源：http://ebi.epnwcf.com

[T45] Perl：数组遍历
来源：http://aij.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://uhq.daria6918.cn

[T46] Perl：哈希操作
来源：http://evc.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kit.hywenlv.cn

[T47] Perl：正则捕获
来源：http://yld.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bmb.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://bpa.fehbvm.com

$s =~ s/old/new/g;
来源：http://jsf.fehbvm.com

[T49] Perl：函数
来源：http://mgo.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tty.sysykeji.top

[T50] Perl：逐行读文件
来源：http://svv.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://frf.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://jrr.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://dnl.cheryme.top

println("Hello")
来源：http://cdm.chenzaomai.com

[T52] Scala：变量
来源：http://mnn.yangfankeji.com

val a = 1;  var b = 2
来源：http://dug.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://wcv.fehbvm.com

s"值: $b"
来源：http://lyv.yj202588.top

[T54] Scala：集合映射
来源：http://uxq.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://jqd.jianghu66.top

[T55] Scala：集合过滤
来源：http://jhc.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://rnn.cheryme.top

[T56] Scala：样例类
来源：http://jxj.sweek.top

case class User(name: String, age: Int)
来源：http://csn.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://jxj.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cai.cqqwz.cn

[T58] Scala：函数定义
来源：http://vgw.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://jxa.shangyingyoupin.top

[T59] Scala：循环
来源：http://txf.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://qdk.yonumen.top

[T60] Scala：折叠
来源：http://kta.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nxm.sxryk.cn

================================================================================
来源：http://kac.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cmv.nanxuanxn.top

================================================================================
来源：http://lxe.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://eya.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jzd.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://hjt.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://phu.tianlin.xyz

[U03] Py：加载 .env 配置
来源：http://tup.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zcz.zhixingplan.top

[U04] Py：变量调试打印
来源：http://urt.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zes.daxiang520.top

[U05] Py：列表去重且保序
来源：http://xxs.cucudq.cn

list(dict.fromkeys(arr))
来源：http://khg.jinqigufen.top

[U06] Py：合并两个字典
来源：http://ukc.yuanzhike.top

{**a, **b}
来源：http://nzm.gotoacloud.top

[U07] Py：反转字典键值
来源：http://jxl.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://eym.cdnleiting.top

[U08] Py：展平二维列表
来源：http://caa.yuxming.cn

[y for x in nested for y in x]
来源：http://req.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://ura.pycfn.com

max(d, key=d.get)
来源：http://phw.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://ndr.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fwy.ivvv.top

[U11] Py：生成器表达式
来源：http://ekr.uphjek.com

(x * 2 for x in arr)
来源：http://myk.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://exz.cashguo.top

Counter(arr).most_common(3)
来源：http://elf.0kj1m.cn

[U13] Py：固定长度队列
来源：http://teg.316326.xyz

deque(maxlen=10)
来源：http://sks.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://rgv.ywan-chungtsiang.top

defaultdict(list)
来源：http://izn.zdbjq.cn

[U15] Py：高精度计时
来源：http://qpa.zhongyouzk.top

t = time.perf_counter()
来源：http://ddw.yuanzhike.top

[U16] Py：命令行参数解析
来源：http://bbp.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bdk.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://drn.shanyushiyangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://cby.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://blc.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://hcd.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://skc.sjlbkw.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uiu.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://rxc.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://pff.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://xvx.ctjpmb.com

@contextlib.contextmanager
来源：http://vye.guannengcc.top

[U22] Py：矩阵转置
来源：http://lws.nanxinkj.top

list(zip(*m))
来源：http://iis.hnqzz.top

[U23] Py：分块读取大文件
来源：http://gtg.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmb.cqqwz.cn

[U24] Py：路径操作
来源：http://utt.ehwqpu.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zep.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://lvl.yuxming.cn

csv.DictReader(f)
来源：http://evk.zhaomingkeji.xyz

[U26] Py：并发下载
来源：http://muy.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hft.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://vvl.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://dzq.yj20258888.top

[U28] Py：类型别名
来源：http://vtj.nanxinkj.top

UserId = int
来源：http://cpk.zycfv.cn

[U29] Py：属性校验
来源：http://aqp.chenzaomai.com

@property 与 @x.setter 配合
来源：http://xru.xingfuxueyuan.xyz

[U30] Py：数据类
来源：http://rkp.vqdsnc.cn

@dataclass(slots=True)
来源：http://rav.ybcxt.top

[U31] Py：单测
来源：http://pbc.c1oappe.top

python -m pytest -q
来源：http://rqx.shuidangran.top

[U32] Py：代码格式化
来源：http://sxh.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://esb.zycfv.cn

[U33] Py：打包发布
来源：http://bzc.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://ofm.zdqjudy.top

[U34] Py：判断编码
来源：http://nuc.gogol.net.cn

chardet.detect(raw)
来源：http://qvc.hammf.cn

[U35] Py：发送邮件
来源：http://itp.hesvh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hmc.quarkkingdee.top

[U36] Py：定时任务
来源：http://szr.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://imf.52xcode.cn

[U37] Py：读写 Excel
来源：http://usm.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://myi.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://oty.birdmap.top

Path(__file__).resolve().parent
来源：http://zui.tian-w.cn

[U39] Py：判断是否在交互环境
来源：http://wpl.jianghu66.top

sys.stdout.isatty()
来源：http://huu.yueranfly.top

[U40] Py：打印到标准错误
来源：http://iwv.vehdjk.com

print("err", file=sys.stderr)
来源：http://wut.0kj1m.cn

[U41] PHP：初始化 Composer 项目
来源：http://kju.yvedp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://emp.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://gsw.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nvo.52xcode.cn

[U43] PHP：声明命名空间
来源：http://mwr.jyoumei.cn

namespace App\Http;
来源：http://ewg.yj20258888.top

[U44] PHP：开启严格类型
来源：http://nzf.yj202588.top

declare(strict_types=1);
来源：http://swy.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://vmb.vehdjk.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://tvb.vehdjk.com

[U46] PHP：可空类型
来源：http://tbv.tian-w.cn

?string $name = null
来源：http://xru.meibo888.top

[U47] PHP：联合类型
来源：http://pfa.jinqigfzy.top

int|string $id
来源：http://gnt.chenlongwang.top

[U48] PHP：纯枚举
来源：http://dub.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://and.jqgufenzy.top

[U49] PHP：只读属性
来源：http://rnx.hongshengwenyu.top

public readonly string $name
来源：http://nyp.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://rkt.ppjwa.cn

public function __construct(private int $id) {}
来源：http://cpr.yvedp.cn

[U51] PHP：数组解构
来源：http://dex.jiagoushi.top

[$a, $b] = $arr;
来源：http://byu.52xcode.cn

[U52] PHP：箭头函数
来源：http://oyj.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://tfb.epnwcf.com

[U53] PHP：空合并运算符
来源：http://gcf.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://buc.fengsongda.top

[U54] PHP：空安全调用
来源：http://gia.snrcjt.cn

$obj?->method()
来源：http://zeb.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://niq.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dsr.fengsongda.top

[U56] PHP：命名参数
来源：http://gqk.hysaishi.cn

f(a: 1, b: 2)
来源：http://wuw.hfpthk.cn

[U57] PHP：字符串插值
来源：http://ass.birdmap.top

"值: {$a}"
来源：http://oup.jiagoushi.top

[U58] PHP：数组三件套
来源：http://veu.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iap.iojbl.cn

[U59] PHP：自定义排序
来源：http://zcc.sjlbkw.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovz.316326.xyz

[U60] PHP：JSON 编解码
来源：http://jjj.jinghuilouyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mwv.yanxiufei.cn

[U61] PHP：正则
来源：http://cwg.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gne.ppjwa.cn

[U62] PHP：日期对象
来源：http://oro.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pmn.zhoulong.xyz

[U63] PHP：文件读写
来源：http://srb.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ywc.fehbvm.com

[U64] PHP：目录遍历
来源：http://ruh.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://flx.bjfxy.top

[U65] PHP：会话
来源：http://cza.gaohongyu789.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kkt.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://qme.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zyt.xuanzx.com

[U67] PHP：处理文件上传
来源：http://lmk.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://evw.chenzaomai.com

[U68] PHP：PDO 连接
来源：http://mne.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://diy.fehbvm.com

[U69] PHP：PDO 预处理
来源：http://dap.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eek.zdqjudy.top

[U70] PHP：PDO 事务
来源：http://lex.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yuk.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://jor.gotoacloud.top

throw new RuntimeException("失败", 500);
来源：http://ugc.gogol.net.cn

[U72] PHP：写错误日志
来源：http://ipc.pycfn.com

error_log("失败: " . $e->getMessage());
来源：http://uqf.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://bal.zhixingplan.top

parse_ini_file("config.ini", true)
来源：http://umr.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://hww.fehbvm.com

getenv("APP_ENV") ?: "production"
来源：http://vcl.aizwys.cn

[U75] PHP：依赖注入
来源：http://hze.fanxiaobao.xyz

composer require psr/container
来源：http://jar.hesvh.cn

[U76] PHP：简单路由
来源：http://ckf.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vce.zdbjq.cn

[U77] PHP：模板渲染
来源：http://qzw.hammf.cn

composer require twig/twig
来源：http://tvq.nanxuanxn.top

[U78] PHP：单元测试
来源：http://fhf.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://tun.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://euj.xinyue.icu

composer require --dev phpstan/phpstan
来源：http://kfo.yj20258.top

[U80] PHP：代码规范修复
来源：http://blh.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://foj.sxryk.cn

[U81] JS：初始化项目
来源：http://fiy.0kj1m.cn

npm init -y;  npm i express
来源：http://uqh.uphjek.com

[U82] JS：package.json 脚本
来源：http://nsa.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ytj.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://avy.gotoacloud.top

export const a = 1;  import { a } from "./m.js";
来源：http://zfb.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://gcr.ywan-chungtsiang.top

module.exports = { a };  const { a } = require("./m");
来源：http://tvu.yvedp.cn

[U85] JS：可选链
来源：http://ukc.hesvh.cn

a?.b?.c
来源：http://yqy.jlsjyb.cn

[U86] JS：空值合并
来源：http://uam.xuetiantiany.cn

a ?? b
来源：http://fdk.yfazqb.com

[U87] JS：解构默认值
来源：http://cay.ctjpmb.com

const { a = 1, b = 2 } = obj;
来源：http://scd.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://upn.yanxiufei.cn

{ ...a, ...b }
来源：http://rvk.ydjk.org.cn

[U89] JS：数组去重
来源：http://xza.xinyue.icu

[...new Set(arr)]
来源：http://roj.gaohongyu789.top

[U90] JS：数字数组排序
来源：http://chj.epnwcf.com

[...arr].sort((a, b) => a - b)
来源：http://arw.ivvv.top

[U91] JS：对象键值遍历
来源：http://vpb.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vvb.yj202588.top

[U92] JS：深拷贝
来源：http://tbh.nanxinkj.top

structuredClone(obj)
来源：http://bjn.yfazqb.com

[U93] JS：模板字符串
来源：http://nip.jqgfzy.top

`共 ${n} 条`
来源：http://mfl.jinyuanbaomall.cn

[U94] JS：箭头函数
来源：http://nai.hfpthk.cn

const double = x => x * 2;
来源：http://prx.feifeiyinyue.top

[U95] JS：Promise 包装
来源：http://mpv.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://qkq.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://oqt.wangshuangyany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oui.guannengcc.top

[U97] JS：并发请求
来源：http://jkk.uphjek.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://jcw.gotoacloud.top

[U98] JS：fetch 带 JSON
来源：http://mjk.redwolf501.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zwv.jinqigfzy.top

[U99] JS：事件监听
来源：http://xhq.yangfankeji.com

el.addEventListener("click", e => {})
来源：http://whd.daria6918.cn

[U100] JS：DOM 查询
来源：http://xow.havefunace.top

document.querySelector(".item")
来源：http://wgu.zhixingplan.top

[U101] JS：classList 操作
来源：http://yll.ppjwa.cn

el.classList.toggle("active")
来源：http://zju.fehbvm.com

[U102] JS：本地存储
来源：http://iir.xziqi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://djq.xuetiantiany.cn

[U103] JS：定时器
来源：http://xbn.pycfn.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kaa.jianghu66.top

[U104] JS：防抖
来源：http://pfb.316326.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yak.gotoacloud.top

[U105] JS：节流
来源：http://cem.yuxming.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://opc.guowangkeji.top

[U106] JS：日期格式化
来源：http://xtk.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gox.meibo888.top

[U107] JS：数字千分位
来源：http://kku.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mru.fanxiaobao.xyz

[U108] JS：随机整数
来源：http://xvx.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bvm.pengpengdd.cyou

[U109] JS：数组分组
来源：http://ehp.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://xfh.zhijiandao.cn

[U110] JS：数组分块
来源：http://vrl.hysaishi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bxb.xinyue.icu

[U111] JS：对象转 Map
来源：http://fgi.fktsv.cn

new Map(Object.entries(obj))
来源：http://qbr.tarul.cn

[U112] JS：字符串补位
来源：http://iiu.jinqigfzy.top

"7".padStart(3, "0")
来源：http://wyc.nanxinkj.top

[U113] JS：正则替换全部
来源：http://gzp.zhoulong.xyz

s.replaceAll("a", "b")
来源：http://pcr.9152youxi.cn

[U114] JS：JSON 深比较
来源：http://awt.yfazqb.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://wmr.dashuyun.cn

[U115] JS：生成 UUID
来源：http://gma.sjlbkw.cn

crypto.randomUUID()
来源：http://moo.52xcode.cn

[U116] JS：类型检查（JSDoc）
来源：http://jfb.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://ibe.zdqjudy.top

[U117] JS：单元测试
来源：http://hzt.jinghuilouyu.cn

npm i -D vitest;  npx vitest
来源：http://qit.shangyingyoupin.top

[U118] JS：开发服务器
来源：http://aqn.yongpay.top

npm i -D vite;  npx vite
来源：http://dlv.cashguo.top

[U119] JS：生产构建
来源：http://vmd.yuanzhike.top

npx vite build
来源：http://bgo.jianghu66.top

[U120] JS：读取环境变量（Vite）
来源：http://omx.andypj.xyz

import.meta.env.VITE_API_URL
来源：http://adl.zdqjudy.top

================================================================================
来源：http://uub.shuidangran.top

统计汇总
来源：http://eys.feifeiyinyue.top

================================================================================
来源：http://zgh.chenjidiqi.icu

按语言统计（条）：
来源：http://rvt.tianlin.xyz

Python ......... 252
来源：http://mpb.sweek.top

PHP ............ 252
来源：http://jre.ywan-chungtsiang.top

JavaScript ..... 252
来源：http://zrr.fehbvm.com

TypeScript ..... 212
来源：http://aov.c1oappe.top

Java ........... 212
来源：http://ooe.ydzc1.top

Go ............. 212
来源：http://qkl.andypj.xyz

Ruby ........... 212
来源：http://wjg.zdqjudy.top

C# ............. 212
来源：http://byo.cashguo.top


<!-- 参考信息 -->