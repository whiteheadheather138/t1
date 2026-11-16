代发 wailian999

[T33] Lua：表（数组）
来源：http://isr.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hmc.gzhubu.top

[T34] Lua：遍历表
来源：http://xzr.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qzw.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://nxt.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://chi.nanxuanxn.top

[T36] Lua：函数
来源：http://yna.xuanzx.com

function add(a, b) return a + b end
来源：http://rqg.52xcode.cn

[T37] Lua：字符串拼接
来源：http://ata.ydjk.org.cn

"a" .. "b"
来源：http://nrf.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://gir.yj202588.top

if x > 0 then print("正") end
来源：http://ajb.hysaishi.cn

[T39] Lua：模式匹配
来源：http://znz.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://oyt.zdbjq.cn

[T40] Lua：元表
来源：http://qbo.pycfn.com

setmetatable({}, { __index = base })
来源：http://fxz.havefunace.top

[T41] Perl：Hello World
来源：http://kvp.yongpay.top

print "Hello\n";
来源：http://kxm.xylfe.cn

[T42] Perl：变量类型
来源：http://rtl.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://boi.dashuyun.cn

[T43] Perl：字符串插值
来源：http://wnc.jinghuilouyu.cn

"值: $a"
来源：http://aly.jinqigfzy.top

[T44] Perl：条件
来源：http://hjf.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://upl.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://rla.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://ubb.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://iik.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xfn.cheryme.top

[T47] Perl：正则捕获
来源：http://lvo.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vqr.yfazqb.com

[T48] Perl：正则替换
来源：http://key.aizwys.cn

$s =~ s/old/new/g;
来源：http://tyo.redwolf501.top

[T49] Perl：函数
来源：http://ony.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kho.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://spq.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wvy.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://mey.havefunace.top

[T51] Scala：Hello World
来源：http://loj.hysaishi.cn

println("Hello")
来源：http://vnp.316326.xyz

[T52] Scala：变量
来源：http://zwz.cdnleiting.top

val a = 1;  var b = 2
来源：http://ghe.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://rne.yfazqb.com

s"值: $b"
来源：http://xxf.gogol.net.cn

[T54] Scala：集合映射
来源：http://ign.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://vii.yueranfly.top

[T55] Scala：集合过滤
来源：http://idf.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ehw.gotoacloud.top

[T56] Scala：样例类
来源：http://bct.sweek.top

case class User(name: String, age: Int)
来源：http://kqm.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://ygo.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ceg.yongpay.top

[T58] Scala：函数定义
来源：http://wla.cdnleiting.top

def add(a: Int, b: Int): Int = a + b
来源：http://shv.jqgufenzy.top

[T59] Scala：循环
来源：http://mmq.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://efz.svipenyu.cn

[T60] Scala：折叠
来源：http://eei.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ssy.bbcook.cn

================================================================================
来源：http://qqw.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nef.aizwys.cn

================================================================================
来源：http://xdr.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://mww.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://veo.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://ots.aizwys.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xmr.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://oud.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://sms.yj202588.top

[U04] Py：变量调试打印
来源：http://jmp.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ocs.fengsongda.top

[U05] Py：列表去重且保序
来源：http://ogi.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://qvj.ppjwa.cn

[U06] Py：合并两个字典
来源：http://syb.nwbrower.top

{**a, **b}
来源：http://vlf.birdmap.top

[U07] Py：反转字典键值
来源：http://dxj.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://tnp.snrcjt.cn

[U08] Py：展平二维列表
来源：http://ock.shzxlz.cn

[y for x in nested for y in x]
来源：http://icr.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://xnk.gzhubu.top

max(d, key=d.get)
来源：http://vqo.yangfankeji.com

[U10] Py：按值排序字典
来源：http://tmy.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ykz.svipenyu.cn

[U11] Py：生成器表达式
来源：http://zgb.xuanzx.com

(x * 2 for x in arr)
来源：http://ujc.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://jho.aibaodan.cn

Counter(arr).most_common(3)
来源：http://tfs.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://ugy.pycfn.com

deque(maxlen=10)
来源：http://brv.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://bba.zdqjudy.top

defaultdict(list)
来源：http://pkh.sxryk.cn

[U15] Py：高精度计时
来源：http://hjx.tarul.cn

t = time.perf_counter()
来源：http://kia.sweek.top

[U16] Py：命令行参数解析
来源：http://bvv.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tkq.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://mlf.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://gwn.hcnkem.com

[U18] Py：预编译正则
来源：http://rzj.fengsongda.top

pat = re.compile(r"\d+")
来源：http://vox.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://mja.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dnd.gogol.net.cn

[U20] Py：缓存函数结果
来源：http://hju.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://whb.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://mys.smart0.xyz

@contextlib.contextmanager
来源：http://fjh.ybcxt.top

[U22] Py：矩阵转置
来源：http://dqi.pycfn.com

list(zip(*m))
来源：http://uyd.andypj.xyz

[U23] Py：分块读取大文件
来源：http://nua.shzxlz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vbc.dianchejie.cn

[U24] Py：路径操作
来源：http://hju.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wmj.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://adp.shangyingyoupin.top

csv.DictReader(f)
来源：http://cay.yfazqb.com

[U26] Py：并发下载
来源：http://owy.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pbm.guannengcc.top

[U27] Py：异步 HTTP
来源：http://byg.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://bof.fengsongda.top

[U28] Py：类型别名
来源：http://dmn.cucudq.cn

UserId = int
来源：http://krm.tian-w.cn

[U29] Py：属性校验
来源：http://gcj.shuidangran.top

@property 与 @x.setter 配合
来源：http://mcz.yangfankeji.com

[U30] Py：数据类
来源：http://dzo.nwbrower.top

@dataclass(slots=True)
来源：http://nzo.sjlbkw.cn

[U31] Py：单测
来源：http://tso.yueranfly.top

python -m pytest -q
来源：http://aqs.zhaomingkeji.xyz

[U32] Py：代码格式化
来源：http://zgm.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://brv.ydzc1.top

[U33] Py：打包发布
来源：http://fkm.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://zlo.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://drn.tian-w.cn

chardet.detect(raw)
来源：http://ueh.daxiang520.top

[U35] Py：发送邮件
来源：http://cmf.fktsv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tsj.daxiang520.top

[U36] Py：定时任务
来源：http://rxo.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://reb.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://xdj.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tsh.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://noq.hnqzz.top

Path(__file__).resolve().parent
来源：http://qjl.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://xdj.c1oappe.top

sys.stdout.isatty()
来源：http://ylo.epnwcf.com

[U40] Py：打印到标准错误
来源：http://uro.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://wec.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://ncc.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mck.0kj1m.cn

[U42] PHP：PSR-4 自动加载
来源：http://mqi.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hrx.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://bbm.chenlongwang.top

namespace App\Http;
来源：http://hxt.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://yog.ppjwa.cn

declare(strict_types=1);
来源：http://kce.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://fbb.zdqjudy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hwy.epnwcf.com

[U46] PHP：可空类型
来源：http://hoq.feifeiyinyue.top

?string $name = null
来源：http://hio.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://gtc.gaohongyu789.top

int|string $id
来源：http://tgy.daxiang520.top

[U48] PHP：纯枚举
来源：http://mmd.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fcv.xziqi.cn

[U49] PHP：只读属性
来源：http://pgg.hongshengwenyu.top

public readonly string $name
来源：http://bxr.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://ezq.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://kwn.ydzc1.top

[U51] PHP：数组解构
来源：http://nzb.svipenyu.cn

[$a, $b] = $arr;
来源：http://ydr.wangdashe.top

[U52] PHP：箭头函数
来源：http://sxt.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://ygz.feifeiyinyue.top

[U53] PHP：空合并运算符
来源：http://wqh.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://eyu.hysaishi.cn

[U54] PHP：空安全调用
来源：http://xsj.haohaochexian.top

$obj?->method()
来源：http://fuj.hesvh.cn

[U55] PHP：match 表达式
来源：http://ofz.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xli.c1oappe.top

[U56] PHP：命名参数
来源：http://dsw.c1oappe.top

f(a: 1, b: 2)
来源：http://uyd.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://nsy.jyoumei.cn

"值: {$a}"
来源：http://hqu.yueranfly.top

[U58] PHP：数组三件套
来源：http://ksz.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jlw.jianghu66.top

[U59] PHP：自定义排序
来源：http://jtd.ehwqpu.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjv.yj20258.top

[U60] PHP：JSON 编解码
来源：http://bag.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rqr.hysaishi.cn

[U61] PHP：正则
来源：http://iwr.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ewi.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://oil.cheryme.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uil.aizwys.cn

[U63] PHP：文件读写
来源：http://mkk.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kyt.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://acj.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://yry.pycfn.com

[U65] PHP：会话
来源：http://ctc.xingfuxueyuan.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://kzs.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://hiw.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pae.andypj.xyz

[U67] PHP：处理文件上传
来源：http://ygz.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qdt.nwbrower.top

[U68] PHP：PDO 连接
来源：http://pct.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oey.yonumen.top

[U69] PHP：PDO 预处理
来源：http://zie.ybcxt.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qur.zhaomingkeji.xyz

[U70] PHP：PDO 事务
来源：http://oxf.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhn.nanxinkj.top

[U71] PHP：抛出异常
来源：http://oad.nwbrower.top

throw new RuntimeException("失败", 500);
来源：http://njl.gotoacloud.top

[U72] PHP：写错误日志
来源：http://gfl.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://qeo.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://jao.chenzaomai.com

parse_ini_file("config.ini", true)
来源：http://vyr.zycfv.cn

[U74] PHP：读取环境变量
来源：http://idm.sjlbkw.cn

getenv("APP_ENV") ?: "production"
来源：http://rvt.yfazqb.com

[U75] PHP：依赖注入
来源：http://dvy.yongpay.top

composer require psr/container
来源：http://vda.c1oappe.top

[U76] PHP：简单路由
来源：http://ker.ivvv.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fva.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://ggu.birdmap.top

composer require twig/twig
来源：http://wqk.sysykeji.top

[U78] PHP：单元测试
来源：http://bfh.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://tfn.redwolf501.top

[U79] PHP：静态分析
来源：http://euh.jinyuanbaomall.cn

composer require --dev phpstan/phpstan
来源：http://hyk.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://omd.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sli.aizwys.cn

[U81] JS：初始化项目
来源：http://vwn.jiagoushi.top

npm init -y;  npm i express
来源：http://tjr.hcnkem.com

[U82] JS：package.json 脚本
来源：http://jrf.jyoumei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://idp.xuanzx.com

[U83] JS：ES Module 导入导出
来源：http://iqy.jinyuanbaomall.cn

export const a = 1;  import { a } from "./m.js";
来源：http://laj.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://tlq.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://szw.haohaochexian.top

[U85] JS：可选链
来源：http://lyu.nanxinkj.top

a?.b?.c
来源：http://eii.iojbl.cn

[U86] JS：空值合并
来源：http://mhg.uphjek.com

a ?? b
来源：http://hyt.chenjidiqi.icu

[U87] JS：解构默认值
来源：http://xef.yj202588.top

const { a = 1, b = 2 } = obj;
来源：http://pst.cucudq.cn

[U88] JS：对象展开合并
来源：http://wul.shangyingyoupin.top

{ ...a, ...b }
来源：http://iqe.shzxlz.cn

[U89] JS：数组去重
来源：http://lbq.zhijiandao.cn

[...new Set(arr)]
来源：http://oni.hesvh.cn

[U90] JS：数字数组排序
来源：http://acz.snrcjt.cn

[...arr].sort((a, b) => a - b)
来源：http://wjb.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://wrj.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ftj.smart0.xyz

[U92] JS：深拷贝
来源：http://ohc.svipenyu.cn

structuredClone(obj)
来源：http://kma.jianghu66.top

[U93] JS：模板字符串
来源：http://kqm.zhongyouzk.top

`共 ${n} 条`
来源：http://yxr.hcnkem.com

[U94] JS：箭头函数
来源：http://eba.zhongyouzk.top

const double = x => x * 2;
来源：http://lyc.svipenyu.cn

[U95] JS：Promise 包装
来源：http://erp.hnxiangtu.top

new Promise((resolve, reject) => {})
来源：http://eqa.zdqjudy.top

[U96] JS：async/await 与异常
来源：http://gui.zhengqikj.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sog.cashguo.top

[U97] JS：并发请求
来源：http://azb.cqqwz.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iha.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://krw.havefunace.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tlp.ydjk.org.cn

[U99] JS：事件监听
来源：http://iaj.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://pxt.pycfn.com

[U100] JS：DOM 查询
来源：http://lho.ywan-chungtsiang.top

document.querySelector(".item")
来源：http://pnp.jqgfzy.top

[U101] JS：classList 操作
来源：http://wsi.fzhhl.top

el.classList.toggle("active")
来源：http://gol.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://ign.svipenyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ttp.hywenlv.cn

[U103] JS：定时器
来源：http://oxh.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hse.svipenyu.cn

[U104] JS：防抖
来源：http://bqh.snrcjt.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mop.wangdashe.top

[U105] JS：节流
来源：http://jlo.52xcode.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://icd.aibaodan.cn

[U106] JS：日期格式化
来源：http://daw.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://llc.ivvv.top

[U107] JS：数字千分位
来源：http://big.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hjs.daxiang520.top

[U108] JS：随机整数
来源：http://bqa.redwolf501.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sxt.jyoumei.cn

[U109] JS：数组分组
来源：http://jda.zhengqikj.top

Object.groupBy(arr, x => x.type)
来源：http://dnm.hcnkem.com

[U110] JS：数组分块
来源：http://rpn.9152youxi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gwu.nwbrower.top

[U111] JS：对象转 Map
来源：http://azy.fzhhl.top

new Map(Object.entries(obj))
来源：http://qek.shanyushiyangtech.top

[U112] JS：字符串补位
来源：http://lka.daria6918.cn

"7".padStart(3, "0")
来源：http://tgz.fengsongda.top

[U113] JS：正则替换全部
来源：http://nzs.shuidangran.top

s.replaceAll("a", "b")
来源：http://mnu.sysykeji.top

[U114] JS：JSON 深比较
来源：http://dsg.yvedp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://evy.fengsongda.top

[U115] JS：生成 UUID
来源：http://qwa.aizwys.cn

crypto.randomUUID()
来源：http://ooe.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://jlh.jqgfzy.top

/** @param {string} name */ function f(name) {}
来源：http://bpq.sxryk.cn

[U117] JS：单元测试
来源：http://mmj.ivvv.top

npm i -D vitest;  npx vitest
来源：http://hwg.sxryk.cn

[U118] JS：开发服务器
来源：http://mts.xziqi.cn

npm i -D vite;  npx vite
来源：http://abp.hnxiangtu.top

[U119] JS：生产构建
来源：http://uft.ybcxt.top

npx vite build
来源：http://xkf.vehdjk.com

[U120] JS：读取环境变量（Vite）
来源：http://qby.cucudq.cn

import.meta.env.VITE_API_URL
来源：http://vsj.ctjpmb.com


<!-- 参考信息 -->