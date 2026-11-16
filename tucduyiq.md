代发 wailian999

[T43] Perl：字符串插值
来源：http://kme.epnwcf.com

"值: $a"
来源：http://dbg.meibo888.top

[T44] Perl：条件
来源：http://klw.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://zvh.fzhhl.top

[T45] Perl：数组遍历
来源：http://mzf.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://wds.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://yvo.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pbs.yuxming.cn

[T47] Perl：正则捕获
来源：http://fvl.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ckt.sysykeji.top

[T48] Perl：正则替换
来源：http://gnb.tarul.cn

$s =~ s/old/new/g;
来源：http://onf.dashuyun.cn

[T49] Perl：函数
来源：http://fzm.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kuu.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://dwc.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uyz.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://ipl.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://xld.jinghuilouyu.cn

println("Hello")
来源：http://cwa.yanxiufei.cn

[T52] Scala：变量
来源：http://lzx.nanxinkj.top

val a = 1;  var b = 2
来源：http://npk.tanke756.top

[T53] Scala：字符串插值
来源：http://fgz.dianchejie.cn

s"值: $b"
来源：http://wbl.yueranfly.top

[T54] Scala：集合映射
来源：http://ywd.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://wil.shanyushiyangkeji.top

[T55] Scala：集合过滤
来源：http://ymi.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://xzq.andypj.xyz

[T56] Scala：样例类
来源：http://wpn.redwolf501.top

case class User(name: String, age: Int)
来源：http://apc.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://ufc.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sdr.yvedp.cn

[T58] Scala：函数定义
来源：http://ljx.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://kce.daxiang520.top

[T59] Scala：循环
来源：http://ggc.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://ncy.cashguo.top

[T60] Scala：折叠
来源：http://kkb.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wmd.cucudq.cn

================================================================================
来源：http://phf.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yyw.wangshuangyany.cn

================================================================================
来源：http://vnz.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://yqv.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://rqd.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://mhw.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://amk.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://xie.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jbx.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://ooq.zhaomingkeji.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pzo.yongpay.top

[U05] Py：列表去重且保序
来源：http://zuq.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://ppi.yvedp.cn

[U06] Py：合并两个字典
来源：http://ylx.fktsv.cn

{**a, **b}
来源：http://avx.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://bju.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://rok.jlsjyb.cn

[U08] Py：展平二维列表
来源：http://yle.shzxlz.cn

[y for x in nested for y in x]
来源：http://win.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://ych.daria6918.cn

max(d, key=d.get)
来源：http://cuq.xziqi.cn

[U10] Py：按值排序字典
来源：http://cjs.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsw.dashuyun.cn

[U11] Py：生成器表达式
来源：http://zlg.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://xak.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://acq.yueranfly.top

Counter(arr).most_common(3)
来源：http://sil.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://wlo.zhixingplan.top

deque(maxlen=10)
来源：http://jhg.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://hey.hywenlv.cn

defaultdict(list)
来源：http://pdj.jiagoushi.top

[U15] Py：高精度计时
来源：http://orc.yueranfly.top

t = time.perf_counter()
来源：http://wtk.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://hmv.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ygq.vqdsnc.cn

[U17] Py：初始化日志
来源：http://jcw.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://cvw.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://edg.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://ple.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://duf.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bcy.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://fmk.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://qpq.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://upq.daria6918.cn

@contextlib.contextmanager
来源：http://ink.yuanzhike.top

[U22] Py：矩阵转置
来源：http://pkl.redwolf501.top

list(zip(*m))
来源：http://xzf.cashguo.top

[U23] Py：分块读取大文件
来源：http://eyj.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ycu.tarul.cn

[U24] Py：路径操作
来源：http://khf.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bas.gotoacloud.top

[U25] Py：CSV 按字典读
来源：http://jsv.shuidangran.top

csv.DictReader(f)
来源：http://soj.cqqwz.cn

[U26] Py：并发下载
来源：http://edh.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wxe.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://qsj.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://fzy.tanke756.top

[U28] Py：类型别名
来源：http://kmo.dashuyun.cn

UserId = int
来源：http://ign.zhongyouzk.top

[U29] Py：属性校验
来源：http://uje.mhx1999.top

@property 与 @x.setter 配合
来源：http://rfq.sxryk.cn

[U30] Py：数据类
来源：http://srs.nwbrower.top

@dataclass(slots=True)
来源：http://jmb.sufxvd.cn

[U31] Py：单测
来源：http://ava.shanyushiyangkeji.top

python -m pytest -q
来源：http://rah.dashuyun.cn

[U32] Py：代码格式化
来源：http://luu.ybcxt.top

ruff format . && ruff check --fix .
来源：http://iec.vqdsnc.cn

[U33] Py：打包发布
来源：http://czz.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://qth.cheryme.top

[U34] Py：判断编码
来源：http://aow.52xcode.cn

chardet.detect(raw)
来源：http://koy.cheryme.top

[U35] Py：发送邮件
来源：http://zje.hywenlv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://srw.zdbjq.cn

[U36] Py：定时任务
来源：http://ceo.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://kka.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://ger.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://mfx.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://rmn.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://rjq.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://vfa.epnwcf.com

sys.stdout.isatty()
来源：http://lpm.aibaodan.cn

[U40] Py：打印到标准错误
来源：http://jgq.chenlongwang.top

print("err", file=sys.stderr)
来源：http://xbc.ydzc1.top

[U41] PHP：初始化 Composer 项目
来源：http://byb.dashuyun.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jcy.jinqigufen.top

[U42] PHP：PSR-4 自动加载
来源：http://qnd.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pby.tarul.cn

[U43] PHP：声明命名空间
来源：http://dmj.vehdjk.com

namespace App\Http;
来源：http://uer.gogol.net.cn

[U44] PHP：开启严格类型
来源：http://peq.haohaochexian.top

declare(strict_types=1);
来源：http://jmk.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://shu.mhx1999.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vqa.ppjwa.cn

[U46] PHP：可空类型
来源：http://eid.ywan-chungtsiang.top

?string $name = null
来源：http://stl.snrcjt.cn

[U47] PHP：联合类型
来源：http://ygk.cdnleiting.top

int|string $id
来源：http://nya.hywenlv.cn

[U48] PHP：纯枚举
来源：http://jte.hammf.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tzl.ydzc1.top

[U49] PHP：只读属性
来源：http://jtk.chenlongwang.top

public readonly string $name
来源：http://nhk.chenzaomai.com

[U50] PHP：构造器属性提升
来源：http://mqm.aibaodan.cn

public function __construct(private int $id) {}
来源：http://mbr.snrcjt.cn

[U51] PHP：数组解构
来源：http://gjo.epnwcf.com

[$a, $b] = $arr;
来源：http://ufa.vehdjk.com

[U52] PHP：箭头函数
来源：http://ueo.nanxinkj.top

$double = fn($x) => $x * 2;
来源：http://fyo.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://nkl.shangyingyoupin.top

$v = $a ?? $b ?? "default";
来源：http://jeh.haohaochexian.top

[U54] PHP：空安全调用
来源：http://lwy.zhaomingkeji.xyz

$obj?->method()
来源：http://ils.svipenyu.cn

[U55] PHP：match 表达式
来源：http://wuo.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vvo.tanke756.top

[U56] PHP：命名参数
来源：http://hxj.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://npu.chenlongwang.top

[U57] PHP：字符串插值
来源：http://dvm.hnqzz.top

"值: {$a}"
来源：http://omo.bjfxy.top

[U58] PHP：数组三件套
来源：http://njn.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bma.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://ivd.xziqi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ltg.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://xxt.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qxp.aizwys.cn

[U61] PHP：正则
来源：http://osw.shangyingyoupin.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ljs.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://xqs.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dnd.zhengqikj.top

[U63] PHP：文件读写
来源：http://kan.cucudq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lua.hesvh.cn

[U64] PHP：目录遍历
来源：http://mmr.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://aym.nanxinkj.top

[U65] PHP：会话
来源：http://pys.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mdu.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://oja.ywan-chungtsiang.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zwa.gzhubu.top

[U67] PHP：处理文件上传
来源：http://bfy.yj202588.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://noa.zdbjq.cn

[U68] PHP：PDO 连接
来源：http://phk.haohaochexian.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kel.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://eal.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fdo.wangdashe.top

[U70] PHP：PDO 事务
来源：http://utv.gotoacloud.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mlw.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://xqa.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://iho.hfpthk.cn

[U72] PHP：写错误日志
来源：http://rkx.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://rgn.yueranfly.top

[U73] PHP：读取 ini 配置
来源：http://wfb.yanxiufei.cn

parse_ini_file("config.ini", true)
来源：http://tmj.xinyue.icu

[U74] PHP：读取环境变量
来源：http://dug.gaohongyu789.top

getenv("APP_ENV") ?: "production"
来源：http://api.316326.xyz

[U75] PHP：依赖注入
来源：http://dqo.sxryk.cn

composer require psr/container
来源：http://aar.jyoumei.cn

[U76] PHP：简单路由
来源：http://kqu.meibo888.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://joe.jianghu66.top

[U77] PHP：模板渲染
来源：http://htp.gotoacloud.top

composer require twig/twig
来源：http://bjw.fzhhl.top

[U78] PHP：单元测试
来源：http://bhj.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://ygp.zhengqikj.top

[U79] PHP：静态分析
来源：http://udp.yj202588.top

composer require --dev phpstan/phpstan
来源：http://fno.haohaochexian.top

[U80] PHP：代码规范修复
来源：http://wgt.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hdx.xingfuxueyuan.xyz

[U81] JS：初始化项目
来源：http://khg.yfazqb.com

npm init -y;  npm i express
来源：http://hji.fanxiaobao.xyz

[U82] JS：package.json 脚本
来源：http://yuf.quarkkingdee.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tls.9152youxi.cn

[U83] JS：ES Module 导入导出
来源：http://hwj.jyoumei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fwj.hesvh.cn

[U84] JS：CommonJS 写法
来源：http://mpr.shanyushiyangtech.top

module.exports = { a };  const { a } = require("./m");
来源：http://jkj.shanyushiyangtech.top

[U85] JS：可选链
来源：http://ezs.jiagoushi.top

a?.b?.c
来源：http://jtj.gzhubu.top

[U86] JS：空值合并
来源：http://fvd.shanyushiyangtech.top

a ?? b
来源：http://xbb.zhiwuduotai.top

[U87] JS：解构默认值
来源：http://ihn.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://tvs.nwbrower.top

[U88] JS：对象展开合并
来源：http://rvj.sxryk.cn

{ ...a, ...b }
来源：http://hws.yanxiufei.cn

[U89] JS：数组去重
来源：http://rfu.jinqigfzy.top

[...new Set(arr)]
来源：http://son.fktsv.cn

[U90] JS：数字数组排序
来源：http://jzl.chenlongwang.top

[...arr].sort((a, b) => a - b)
来源：http://pvu.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://yoc.316326.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fpi.jinyuanbaomall.cn

[U92] JS：深拷贝
来源：http://env.jqgufenzy.top

structuredClone(obj)
来源：http://xlk.jinqigufen.top

[U93] JS：模板字符串
来源：http://vwn.zdbjq.cn

`共 ${n} 条`
来源：http://dyv.redwolf501.top

[U94] JS：箭头函数
来源：http://aug.meibo888.top

const double = x => x * 2;
来源：http://gab.fktsv.cn

[U95] JS：Promise 包装
来源：http://vop.xylfe.cn

new Promise((resolve, reject) => {})
来源：http://iho.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://ebj.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dop.zhengqikj.top

[U97] JS：并发请求
来源：http://gal.hesvh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nbs.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://wpm.wangdashe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://apo.shuidangran.top

[U99] JS：事件监听
来源：http://ydj.sufxvd.cn

el.addEventListener("click", e => {})
来源：http://dge.jinghuilouyu.cn

[U100] JS：DOM 查询
来源：http://oul.andypj.xyz

document.querySelector(".item")
来源：http://lit.hnxiangtu.top

[U101] JS：classList 操作
来源：http://alr.wangshuangyany.cn

el.classList.toggle("active")
来源：http://jfo.yj20258.top

[U102] JS：本地存储
来源：http://xem.zhiwuduotai.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://lni.vqdsnc.cn

[U103] JS：定时器
来源：http://hnp.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wrp.jqgfzy.top

[U104] JS：防抖
来源：http://zen.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jas.zhoulong.xyz

[U105] JS：节流
来源：http://ors.xziqi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eoi.ybcxt.top

[U106] JS：日期格式化
来源：http://rzn.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://abm.hfpthk.cn

[U107] JS：数字千分位
来源：http://vca.yongpay.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vkf.ydjk.org.cn

[U108] JS：随机整数
来源：http://nvn.sxryk.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qrm.wangshuangyany.cn

[U109] JS：数组分组
来源：http://gfk.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://hmo.havefunace.top

[U110] JS：数组分块
来源：http://dpg.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dbj.tarul.cn

[U111] JS：对象转 Map
来源：http://kyu.dianchejie.cn

new Map(Object.entries(obj))
来源：http://rkt.snrcjt.cn

[U112] JS：字符串补位
来源：http://dyj.yonumen.top

"7".padStart(3, "0")
来源：http://sxo.xingfuxueyuan.xyz

[U113] JS：正则替换全部
来源：http://jgq.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://dup.andypj.xyz

[U114] JS：JSON 深比较
来源：http://ozp.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vla.jlsjyb.cn

[U115] JS：生成 UUID
来源：http://ixa.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://zcc.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://fzp.quarkkingdee.top

/** @param {string} name */ function f(name) {}
来源：http://jtp.hesvh.cn

[U117] JS：单元测试
来源：http://llb.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://mdj.chenlongwang.top

[U118] JS：开发服务器
来源：http://xrl.yj20258888.top

npm i -D vite;  npx vite
来源：http://wbd.gotoacloud.top

[U119] JS：生产构建
来源：http://xor.yangfankeji.com

npx vite build
来源：http://jgc.jinghuilouyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://yoi.shanyushiyangkeji.top

import.meta.env.VITE_API_URL
来源：http://pqb.shanyushiyangtech.top

================================================================================
来源：http://lqo.guowangkeji.top

统计汇总
来源：http://ohm.pycfn.com

================================================================================
来源：http://epw.cheryme.top

按语言统计（条）：
来源：http://hpb.nwbrower.top

Python ......... 252
来源：http://qio.fehbvm.com

PHP ............ 252
来源：http://cew.fktsv.cn

JavaScript ..... 252
来源：http://ygj.tianlin.xyz

TypeScript ..... 212
来源：http://fpr.hnxiangtu.top

Java ........... 212
来源：http://gfc.52xcode.cn

Go ............. 212
来源：http://zml.snrcjt.cn

Ruby ........... 212
来源：http://gid.kuanghao11.cn

C# ............. 212
来源：http://nrr.c1oappe.top

C .............. 30
来源：http://lre.zhixingplan.top

C++ ............ 30
来源：http://apl.jinyuanbaomall.cn

SQL ............ 90
来源：http://aed.sxryk.cn

Bash ........... 80
来源：http://ofj.svipenyu.cn

Kotlin ......... 15
来源：http://osc.ivvv.top

Swift .......... 15
来源：http://iwb.zhengqikj.top

Lua ............ 10
来源：http://xyb.zhengqikj.top

Perl ........... 10
来源：http://qkd.hcnkem.com


<!-- 参考信息 -->