代发 wailian999

[T43] Perl：字符串插值
来源：http://rsl.shanyushiyangkeji.top

"值: $a"
来源：http://rwu.gogol.net.cn

[T44] Perl：条件
来源：http://ysp.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://yxo.shzxlz.cn

[T45] Perl：数组遍历
来源：http://lup.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://vib.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://hru.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://isj.bbcook.cn

[T47] Perl：正则捕获
来源：http://aij.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hjc.guowangkeji.top

[T48] Perl：正则替换
来源：http://pas.ctjpmb.com

$s =~ s/old/new/g;
来源：http://kht.shzxlz.cn

[T49] Perl：函数
来源：http://sjq.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mme.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://cgm.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qka.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://lnx.hysaishi.cn

[T51] Scala：Hello World
来源：http://khz.yvedp.cn

println("Hello")
来源：http://ugr.havefunace.top

[T52] Scala：变量
来源：http://hsj.jiagoushi.top

val a = 1;  var b = 2
来源：http://ylt.bjfxy.top

[T53] Scala：字符串插值
来源：http://kyc.shanyushiyangtech.top

s"值: $b"
来源：http://djy.andypj.xyz

[T54] Scala：集合映射
来源：http://smg.chenlongwang.top

List(1, 2, 3).map(_ * 2)
来源：http://mbg.jianghu66.top

[T55] Scala：集合过滤
来源：http://gzo.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ofh.hcnkem.com

[T56] Scala：样例类
来源：http://lai.52xcode.cn

case class User(name: String, age: Int)
来源：http://xmd.xziqi.cn

[T57] Scala：模式匹配
来源：http://moi.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://iij.yanxiufei.cn

[T58] Scala：函数定义
来源：http://twh.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://fig.wangdashe.top

[T59] Scala：循环
来源：http://wug.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://yjr.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://arx.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zgl.mhx1999.top

================================================================================
来源：http://xsu.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pyy.yuanzhike.top

================================================================================
来源：http://het.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://ivt.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hpp.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://gjk.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://doc.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://woj.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wnj.zhaomingkeji.xyz

[U04] Py：变量调试打印
来源：http://eeg.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xij.bbcook.cn

[U05] Py：列表去重且保序
来源：http://gfz.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://psd.tian-w.cn

[U06] Py：合并两个字典
来源：http://xcq.andypj.xyz

{**a, **b}
来源：http://qrv.jinqigufen.top

[U07] Py：反转字典键值
来源：http://ber.zhongyouzk.top

{v: k for k, v in d.items()}
来源：http://iki.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://bvd.gaohongyu789.top

[y for x in nested for y in x]
来源：http://ewv.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://bfb.guowangkeji.top

max(d, key=d.get)
来源：http://vjd.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://egz.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iqd.epnwcf.com

[U11] Py：生成器表达式
来源：http://amp.nwbrower.top

(x * 2 for x in arr)
来源：http://qye.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qfg.redwolf501.top

Counter(arr).most_common(3)
来源：http://qls.pycfn.com

[U13] Py：固定长度队列
来源：http://ccu.zycfv.cn

deque(maxlen=10)
来源：http://vra.sxryk.cn

[U14] Py：分组收集到列表
来源：http://vgy.meibo888.top

defaultdict(list)
来源：http://rpc.gaohongyu789.top

[U15] Py：高精度计时
来源：http://rdm.ppjwa.cn

t = time.perf_counter()
来源：http://yte.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://pvp.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uin.shuidangran.top

[U17] Py：初始化日志
来源：http://uuq.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://eow.jinqigufen.top

[U18] Py：预编译正则
来源：http://apa.fktsv.cn

pat = re.compile(r"\d+")
来源：http://yhv.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://wap.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://irj.yongpay.top

[U20] Py：缓存函数结果
来源：http://vrg.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://shh.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://pmr.yj202588.top

@contextlib.contextmanager
来源：http://flf.shangyingyoupin.top

[U22] Py：矩阵转置
来源：http://ylv.wangshuangyany.cn

list(zip(*m))
来源：http://xxn.fengsongda.top

[U23] Py：分块读取大文件
来源：http://jxq.mhx1999.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gvn.zhengqikj.top

[U24] Py：路径操作
来源：http://qfo.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mvu.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://hyu.zhengqikj.top

csv.DictReader(f)
来源：http://lay.zycfv.cn

[U26] Py：并发下载
来源：http://veo.yfazqb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tym.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://yov.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://sfz.jqgfzy.top

[U28] Py：类型别名
来源：http://qki.yanxiufei.cn

UserId = int
来源：http://aav.gaohongyu789.top

[U29] Py：属性校验
来源：http://imk.ctjpmb.com

@property 与 @x.setter 配合
来源：http://luz.epnwcf.com

[U30] Py：数据类
来源：http://wjl.fzhhl.top

@dataclass(slots=True)
来源：http://lwv.zhongyouzk.top

[U31] Py：单测
来源：http://auq.cheryme.top

python -m pytest -q
来源：http://odv.ehwqpu.com

[U32] Py：代码格式化
来源：http://mfd.daxiang520.top

ruff format . && ruff check --fix .
来源：http://smb.yonumen.top

[U33] Py：打包发布
来源：http://eyo.kuanghao11.cn

python -m build  （依赖 pyproject.toml）
来源：http://gew.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://qli.svipenyu.cn

chardet.detect(raw)
来源：http://bym.daria6918.cn

[U35] Py：发送邮件
来源：http://zws.jlsjyb.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xmb.jyoumei.cn

[U36] Py：定时任务
来源：http://gtc.jinyuanbaomall.cn

schedule.every(10).minutes.do(job)
来源：http://tou.svipenyu.cn

[U37] Py：读写 Excel
来源：http://fpi.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qek.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://aib.yfazqb.com

Path(__file__).resolve().parent
来源：http://yft.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://sry.jianghu66.top

sys.stdout.isatty()
来源：http://yvg.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://ucr.hammf.cn

print("err", file=sys.stderr)
来源：http://sav.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://lwg.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://xnb.tian-w.cn

[U42] PHP：PSR-4 自动加载
来源：http://ett.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hyf.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://mit.zhongyouzk.top

namespace App\Http;
来源：http://lcf.cqqwz.cn

[U44] PHP：开启严格类型
来源：http://cvq.sjlbkw.cn

declare(strict_types=1);
来源：http://hde.feifeiyinyue.top

[U45] PHP：类型声明与返回类型
来源：http://dvd.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://xob.hywenlv.cn

[U46] PHP：可空类型
来源：http://bpq.ctjpmb.com

?string $name = null
来源：http://kyv.yanxiufei.cn

[U47] PHP：联合类型
来源：http://brq.sysykeji.top

int|string $id
来源：http://akz.shangyingyoupin.top

[U48] PHP：纯枚举
来源：http://kdd.kuanghao11.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lnx.ivvv.top

[U49] PHP：只读属性
来源：http://nvg.yuxming.cn

public readonly string $name
来源：http://dwn.andypj.xyz

[U50] PHP：构造器属性提升
来源：http://mww.gzhubu.top

public function __construct(private int $id) {}
来源：http://sbf.redwolf501.top

[U51] PHP：数组解构
来源：http://fys.hnxiangtu.top

[$a, $b] = $arr;
来源：http://ipz.cdnleiting.top

[U52] PHP：箭头函数
来源：http://lyu.tanke756.top

$double = fn($x) => $x * 2;
来源：http://dvj.yvedp.cn

[U53] PHP：空合并运算符
来源：http://mvn.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://zdi.svipenyu.cn

[U54] PHP：空安全调用
来源：http://sai.gzhubu.top

$obj?->method()
来源：http://cha.hammf.cn

[U55] PHP：match 表达式
来源：http://aek.hongshengwenyu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tdq.tian-w.cn

[U56] PHP：命名参数
来源：http://tts.ivvv.top

f(a: 1, b: 2)
来源：http://sri.gotoacloud.top

[U57] PHP：字符串插值
来源：http://qpm.birdmap.top

"值: {$a}"
来源：http://ofy.tianlin.xyz

[U58] PHP：数组三件套
来源：http://beg.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://obw.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://srx.zhengqikj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bix.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://bha.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qkn.xziqi.cn

[U61] PHP：正则
来源：http://oge.9152youxi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://puf.gogol.net.cn

[U62] PHP：日期对象
来源：http://azg.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zyf.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://eta.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nbo.zhijiandao.cn

[U64] PHP：目录遍历
来源：http://hyl.havefunace.top

glob("dir/*.php");  scandir("dir");
来源：http://iou.quarkkingdee.top

[U65] PHP：会话
来源：http://zkt.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://twn.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://prz.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wac.fktsv.cn

[U67] PHP：处理文件上传
来源：http://cbf.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rot.meibo888.top

[U68] PHP：PDO 连接
来源：http://dbs.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xlg.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://but.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ble.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://zue.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcp.gaohongyu789.top

[U71] PHP：抛出异常
来源：http://enu.pycfn.com

throw new RuntimeException("失败", 500);
来源：http://gni.pycfn.com

[U72] PHP：写错误日志
来源：http://igy.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://bzx.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://bzu.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://puq.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://oue.shanyushiyangtech.top

getenv("APP_ENV") ?: "production"
来源：http://qnf.9152youxi.cn

[U75] PHP：依赖注入
来源：http://htq.zhiwuduotai.top

composer require psr/container
来源：http://dxj.zhijiandao.cn

[U76] PHP：简单路由
来源：http://yyl.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://exj.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://ytu.zdqjudy.top

composer require twig/twig
来源：http://vnh.hcnkem.com

[U78] PHP：单元测试
来源：http://bau.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://ozu.wangdashe.top

[U79] PHP：静态分析
来源：http://lhk.pycfn.com

composer require --dev phpstan/phpstan
来源：http://cfi.yuxming.cn

[U80] PHP：代码规范修复
来源：http://ajx.birdmap.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tym.tarul.cn

[U81] JS：初始化项目
来源：http://ufd.wangshuangyany.cn

npm init -y;  npm i express
来源：http://ayk.uphjek.com

[U82] JS：package.json 脚本
来源：http://hmh.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lhx.ywan-chungtsiang.top

[U83] JS：ES Module 导入导出
来源：http://dkd.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://zlm.gotoacloud.top

[U84] JS：CommonJS 写法
来源：http://rip.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://asf.iojbl.cn

[U85] JS：可选链
来源：http://mlo.cashguo.top

a?.b?.c
来源：http://xgg.ybcxt.top

[U86] JS：空值合并
来源：http://upa.daxiang520.top

a ?? b
来源：http://zzx.zhongyouzk.top

[U87] JS：解构默认值
来源：http://tax.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://jlr.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://pwe.sjlbkw.cn

{ ...a, ...b }
来源：http://bwz.redwolf501.top

[U89] JS：数组去重
来源：http://iwi.zdbjq.cn

[...new Set(arr)]
来源：http://cmz.zdqjudy.top

[U90] JS：数字数组排序
来源：http://seq.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://xrb.yvedp.cn

[U91] JS：对象键值遍历
来源：http://kqo.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://txy.yongpay.top

[U92] JS：深拷贝
来源：http://cbx.gotoacloud.top

structuredClone(obj)
来源：http://pqm.vqdsnc.cn

[U93] JS：模板字符串
来源：http://fgt.zhengqikj.top

`共 ${n} 条`
来源：http://ozk.gogol.net.cn

[U94] JS：箭头函数
来源：http://rsc.jianghu66.top

const double = x => x * 2;
来源：http://imi.fanxiaobao.xyz

[U95] JS：Promise 包装
来源：http://ccu.nwbrower.top

new Promise((resolve, reject) => {})
来源：http://iat.yuxming.cn

[U96] JS：async/await 与异常
来源：http://hni.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ymb.andypj.xyz

[U97] JS：并发请求
来源：http://evv.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jfi.shanyushiyangkeji.top

[U98] JS：fetch 带 JSON
来源：http://scr.ctjpmb.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ttd.jqgfzy.top

[U99] JS：事件监听
来源：http://loa.yvedp.cn

el.addEventListener("click", e => {})
来源：http://iop.xuetiantiany.cn

[U100] JS：DOM 查询
来源：http://jor.52xcode.cn

document.querySelector(".item")
来源：http://iuh.zhixingplan.top

[U101] JS：classList 操作
来源：http://jym.mhx1999.top

el.classList.toggle("active")
来源：http://rpb.gotoacloud.top

[U102] JS：本地存储
来源：http://olw.xylfe.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jgl.meibo888.top

[U103] JS：定时器
来源：http://rah.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iib.yj20258.top

[U104] JS：防抖
来源：http://avx.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gvd.yfazqb.com

[U105] JS：节流
来源：http://yww.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://daj.zdbjq.cn

[U106] JS：日期格式化
来源：http://nvr.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yoh.zhengqikj.top

[U107] JS：数字千分位
来源：http://qrx.yj20258888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://miz.wangshuangyany.cn

[U108] JS：随机整数
来源：http://ssh.ydzc1.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xxj.daxiang520.top

[U109] JS：数组分组
来源：http://qhy.ppjwa.cn

Object.groupBy(arr, x => x.type)
来源：http://jwt.zdbjq.cn

[U110] JS：数组分块
来源：http://wlo.ctjpmb.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lxd.zycfv.cn

[U111] JS：对象转 Map
来源：http://mpm.yvedp.cn

new Map(Object.entries(obj))
来源：http://hrz.cheryme.top

[U112] JS：字符串补位
来源：http://umn.yvedp.cn

"7".padStart(3, "0")
来源：http://bwt.uphjek.com

[U113] JS：正则替换全部
来源：http://anr.ivvv.top

s.replaceAll("a", "b")
来源：http://brc.vqdsnc.cn

[U114] JS：JSON 深比较
来源：http://sbv.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://kdp.yj20258.top

[U115] JS：生成 UUID
来源：http://csl.nwbrower.top

crypto.randomUUID()
来源：http://azr.yuxming.cn

[U116] JS：类型检查（JSDoc）
来源：http://zcr.zhoulong.xyz

/** @param {string} name */ function f(name) {}
来源：http://yyu.hywenlv.cn

[U117] JS：单元测试
来源：http://xyn.yj202588.top

npm i -D vitest;  npx vitest
来源：http://hmu.gotoacloud.top

[U118] JS：开发服务器
来源：http://jie.shzxlz.cn

npm i -D vite;  npx vite
来源：http://air.chenlongwang.top

[U119] JS：生产构建
来源：http://pkm.c1oappe.top

npx vite build
来源：http://uwg.mhx1999.top

[U120] JS：读取环境变量（Vite）
来源：http://fvf.xylfe.cn

import.meta.env.VITE_API_URL
来源：http://vcm.shanyushiyangkeji.top

================================================================================
来源：http://uwc.dianchejie.cn

统计汇总
来源：http://iab.dianchejie.cn

================================================================================
来源：http://kix.fanxiaobao.xyz

按语言统计（条）：
来源：http://emn.zhijiandao.cn

Python ......... 252
来源：http://urc.jinyuanbaomall.cn

PHP ............ 252
来源：http://rhq.sjlbkw.cn

JavaScript ..... 252
来源：http://dpz.fktsv.cn

TypeScript ..... 212
来源：http://aup.vehdjk.com

Java ........... 212
来源：http://cnq.gotoacloud.top

Go ............. 212
来源：http://bhy.redwolf501.top

Ruby ........... 212
来源：http://dwf.jiagoushi.top

C# ............. 212
来源：http://hrh.snrcjt.cn

C .............. 30
来源：http://wkn.ivvv.top

C++ ............ 30
来源：http://rns.nanxinkj.top

SQL ............ 90
来源：http://bpq.sufxvd.cn

Bash ........... 80
来源：http://alm.zhengqikj.top

Kotlin ......... 15
来源：http://asm.meibo888.top

Swift .......... 15
来源：http://beq.chenzaomai.com

Lua ............ 10
来源：http://xgy.pengpengdd.cyou

Perl ........... 10
来源：http://ylu.feifeiyinyue.top


<!-- 参考信息 -->