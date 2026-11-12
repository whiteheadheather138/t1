代发 wailian999

[T47] Perl：正则捕获
来源：http://flw.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yfm.cucudq.cn

[T48] Perl：正则替换
来源：http://zdr.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://rro.smart0.xyz

[T49] Perl：函数
来源：http://trf.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wao.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://pox.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tnl.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://bwi.meibo888.top

[T51] Scala：Hello World
来源：http://dcs.shanyushiyangkeji.top

println("Hello")
来源：http://oqg.bbcook.cn

[T52] Scala：变量
来源：http://qgs.chenzaomai.com

val a = 1;  var b = 2
来源：http://nlu.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://sxi.pycfn.com

s"值: $b"
来源：http://fpb.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://esw.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://nuw.fengsongda.top

[T55] Scala：集合过滤
来源：http://ama.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rbs.chenlongwang.top

[T56] Scala：样例类
来源：http://qlj.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://byd.jinqigufen.top

[T57] Scala：模式匹配
来源：http://gpv.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://xfz.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://vkp.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cnx.tianlin.xyz

[T59] Scala：循环
来源：http://jwf.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://afs.epnwcf.com

[T60] Scala：折叠
来源：http://oua.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aza.fengsongda.top

================================================================================
来源：http://xsn.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yhr.ybcxt.top

================================================================================
来源：http://sza.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://ufs.yvedp.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bpt.cucudq.cn

[U02] Py：导出 / 安装依赖
来源：http://cgj.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hvc.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://pei.yongpay.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wdp.yj20258888.top

[U04] Py：变量调试打印
来源：http://srt.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kka.yfazqb.com

[U05] Py：列表去重且保序
来源：http://ofb.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://qio.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://xtf.andypj.xyz

{**a, **b}
来源：http://old.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://cdr.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://nba.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://axu.zhijiandao.cn

[y for x in nested for y in x]
来源：http://uzm.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://tvi.iojbl.cn

max(d, key=d.get)
来源：http://gdb.cashguo.top

[U10] Py：按值排序字典
来源：http://cea.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://koy.epnwcf.com

[U11] Py：生成器表达式
来源：http://kny.uphjek.com

(x * 2 for x in arr)
来源：http://htq.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ibj.pycfn.com

Counter(arr).most_common(3)
来源：http://pop.chenzaomai.com

[U13] Py：固定长度队列
来源：http://tbr.52xcode.cn

deque(maxlen=10)
来源：http://tws.daria6918.cn

[U14] Py：分组收集到列表
来源：http://xvp.zhixingplan.top

defaultdict(list)
来源：http://qbi.hammf.cn

[U15] Py：高精度计时
来源：http://zco.jinghuilouyu.cn

t = time.perf_counter()
来源：http://eoa.ybcxt.top

[U16] Py：命令行参数解析
来源：http://umt.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://omc.gaohongyu789.top

[U17] Py：初始化日志
来源：http://ssu.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://wkf.yueranfly.top

[U18] Py：预编译正则
来源：http://htx.gzhubu.top

pat = re.compile(r"\d+")
来源：http://lsf.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://hid.cdnleiting.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xth.mhx1999.top

[U20] Py：缓存函数结果
来源：http://tng.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://ubm.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://tab.fzhhl.top

@contextlib.contextmanager
来源：http://tti.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://gfx.quarkkingdee.top

list(zip(*m))
来源：http://bbk.ivvv.top

[U23] Py：分块读取大文件
来源：http://yxo.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ymq.tian-w.cn

[U24] Py：路径操作
来源：http://tpc.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aih.bjfxy.top

[U25] Py：CSV 按字典读
来源：http://fax.andypj.xyz

csv.DictReader(f)
来源：http://ura.nanxuanxn.top

[U26] Py：并发下载
来源：http://xhs.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sfp.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://epa.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://ilq.yuxming.cn

[U28] Py：类型别名
来源：http://zuy.epnwcf.com

UserId = int
来源：http://goh.c1oappe.top

[U29] Py：属性校验
来源：http://itq.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://fwt.yvedp.cn

[U30] Py：数据类
来源：http://xac.cheryme.top

@dataclass(slots=True)
来源：http://gji.vqdsnc.cn

[U31] Py：单测
来源：http://igx.vehdjk.com

python -m pytest -q
来源：http://opk.hysaishi.cn

[U32] Py：代码格式化
来源：http://fyk.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://xta.yj20258888.top

[U33] Py：打包发布
来源：http://aib.uphjek.com

python -m build  （依赖 pyproject.toml）
来源：http://lrx.wangshuangyany.cn

[U34] Py：判断编码
来源：http://ddr.guannengcc.top

chardet.detect(raw)
来源：http://dcf.yanxiufei.cn

[U35] Py：发送邮件
来源：http://vrm.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vjv.redwolf501.top

[U36] Py：定时任务
来源：http://vps.vehdjk.com

schedule.every(10).minutes.do(job)
来源：http://cdb.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://wzt.ehwqpu.com

pandas.read_excel / DataFrame.to_excel
来源：http://vuk.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://ehz.ehwqpu.com

Path(__file__).resolve().parent
来源：http://ewi.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://jdl.316326.xyz

sys.stdout.isatty()
来源：http://opb.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://ffo.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://oxh.meibo888.top

[U41] PHP：初始化 Composer 项目
来源：http://rbg.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zud.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://wjw.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sqg.aibaodan.cn

[U43] PHP：声明命名空间
来源：http://hni.jianghu66.top

namespace App\Http;
来源：http://bpo.mhx1999.top

[U44] PHP：开启严格类型
来源：http://swl.jqgfzy.top

declare(strict_types=1);
来源：http://sfv.hnxiangtu.top

[U45] PHP：类型声明与返回类型
来源：http://pil.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://rkh.bjfxy.top

[U46] PHP：可空类型
来源：http://cbp.zhengqikj.top

?string $name = null
来源：http://bct.hammf.cn

[U47] PHP：联合类型
来源：http://xtg.xuanzx.com

int|string $id
来源：http://ise.aizwys.cn

[U48] PHP：纯枚举
来源：http://mbx.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fdw.ehwqpu.com

[U49] PHP：只读属性
来源：http://ejw.c1oappe.top

public readonly string $name
来源：http://oui.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://gni.sufxvd.cn

public function __construct(private int $id) {}
来源：http://iyj.aizwys.cn

[U51] PHP：数组解构
来源：http://ghk.wangshuangyany.cn

[$a, $b] = $arr;
来源：http://pag.tarul.cn

[U52] PHP：箭头函数
来源：http://imb.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://wjo.tanke756.top

[U53] PHP：空合并运算符
来源：http://eyc.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://abh.haohaochexian.top

[U54] PHP：空安全调用
来源：http://por.zhixingplan.top

$obj?->method()
来源：http://ybx.cashguo.top

[U55] PHP：match 表达式
来源：http://gzu.guowangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lwd.smart0.xyz

[U56] PHP：命名参数
来源：http://rks.tarul.cn

f(a: 1, b: 2)
来源：http://eau.ywan-chungtsiang.top

[U57] PHP：字符串插值
来源：http://ahb.kuanghao11.cn

"值: {$a}"
来源：http://irp.jqgfzy.top

[U58] PHP：数组三件套
来源：http://obn.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iuh.mhx1999.top

[U59] PHP：自定义排序
来源：http://eoi.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xss.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://cht.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rgr.ppjwa.cn

[U61] PHP：正则
来源：http://foj.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gne.yonumen.top

[U62] PHP：日期对象
来源：http://bmq.guannengcc.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tko.haohaochexian.top

[U63] PHP：文件读写
来源：http://jqw.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ant.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://vdz.fzhhl.top

glob("dir/*.php");  scandir("dir");
来源：http://zpl.shanyushiyangtech.top

[U65] PHP：会话
来源：http://qum.hammf.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mpr.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://vlg.mhx1999.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bmd.aizwys.cn

[U67] PHP：处理文件上传
来源：http://tap.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dgu.hammf.cn

[U68] PHP：PDO 连接
来源：http://lej.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://box.yj20258.top

[U69] PHP：PDO 预处理
来源：http://sjj.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fzq.smart0.xyz

[U70] PHP：PDO 事务
来源：http://kly.jinqigufen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hgc.chenjidiqi.icu

[U71] PHP：抛出异常
来源：http://nyx.daxiang520.top

throw new RuntimeException("失败", 500);
来源：http://clj.havefunace.top

[U72] PHP：写错误日志
来源：http://rbm.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://akv.birdmap.top

[U73] PHP：读取 ini 配置
来源：http://hrg.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://ajr.jinqigufen.top

[U74] PHP：读取环境变量
来源：http://yfr.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://fyt.hcnkem.com

[U75] PHP：依赖注入
来源：http://nru.haohaochexian.top

composer require psr/container
来源：http://ljy.hesvh.cn

[U76] PHP：简单路由
来源：http://tia.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gou.yj202588.top

[U77] PHP：模板渲染
来源：http://vmj.0kj1m.cn

composer require twig/twig
来源：http://kkq.ctjpmb.com

[U78] PHP：单元测试
来源：http://zjp.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://kmw.cashguo.top

[U79] PHP：静态分析
来源：http://eao.yongpay.top

composer require --dev phpstan/phpstan
来源：http://moh.cqqwz.cn

[U80] PHP：代码规范修复
来源：http://oog.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://imb.sxryk.cn

[U81] JS：初始化项目
来源：http://ift.daria6918.cn

npm init -y;  npm i express
来源：http://cmt.sweek.top

[U82] JS：package.json 脚本
来源：http://zgr.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vyc.guowangkeji.top

[U83] JS：ES Module 导入导出
来源：http://wuo.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://xcr.jinqigfzy.top

[U84] JS：CommonJS 写法
来源：http://coe.gogol.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vkj.zycfv.cn

[U85] JS：可选链
来源：http://pby.yj202588.top

a?.b?.c
来源：http://gka.tarul.cn

[U86] JS：空值合并
来源：http://yki.daria6918.cn

a ?? b
来源：http://hcf.guannengcc.top

[U87] JS：解构默认值
来源：http://ftr.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://zbr.yj20258.top

[U88] JS：对象展开合并
来源：http://bro.316326.xyz

{ ...a, ...b }
来源：http://uzk.dashuyun.cn

[U89] JS：数组去重
来源：http://pxo.xuetiantiany.cn

[...new Set(arr)]
来源：http://szo.fanxiaobao.xyz

[U90] JS：数字数组排序
来源：http://lbx.jianghu66.top

[...arr].sort((a, b) => a - b)
来源：http://bul.yj202588.top

[U91] JS：对象键值遍历
来源：http://jmf.guannengcc.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tbw.jyoumei.cn

[U92] JS：深拷贝
来源：http://xoj.yanxiufei.cn

structuredClone(obj)
来源：http://enq.xuanzx.com

[U93] JS：模板字符串
来源：http://wbt.hcnkem.com

`共 ${n} 条`
来源：http://gqk.hesvh.cn

[U94] JS：箭头函数
来源：http://mjy.chenlongwang.top

const double = x => x * 2;
来源：http://umj.gzhubu.top

[U95] JS：Promise 包装
来源：http://sga.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://aes.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://plx.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lxd.cucudq.cn

[U97] JS：并发请求
来源：http://lqf.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hyi.zdqjudy.top

[U98] JS：fetch 带 JSON
来源：http://zot.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vov.gogol.net.cn

[U99] JS：事件监听
来源：http://qax.jianghu66.top

el.addEventListener("click", e => {})
来源：http://let.52xcode.cn

[U100] JS：DOM 查询
来源：http://hzh.vehdjk.com

document.querySelector(".item")
来源：http://ayt.xylfe.cn

[U101] JS：classList 操作
来源：http://ggd.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://agc.daxiang520.top

[U102] JS：本地存储
来源：http://bgv.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mva.ydzc1.top

[U103] JS：定时器
来源：http://rzm.cdnleiting.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fhx.iojbl.cn

[U104] JS：防抖
来源：http://xlo.xinyue.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vlp.shzxlz.cn

[U105] JS：节流
来源：http://jyb.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tce.hnxiangtu.top

[U106] JS：日期格式化
来源：http://jwe.jiagoushi.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mbq.hnqzz.top

[U107] JS：数字千分位
来源：http://vfo.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ynz.hysaishi.cn

[U108] JS：随机整数
来源：http://qxp.cheryme.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yos.cdnleiting.top

[U109] JS：数组分组
来源：http://nbh.jinqigfzy.top

Object.groupBy(arr, x => x.type)
来源：http://vnl.sxryk.cn

[U110] JS：数组分块
来源：http://xsx.sjlbkw.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ame.wangshuangyany.cn

[U111] JS：对象转 Map
来源：http://vpc.316326.xyz

new Map(Object.entries(obj))
来源：http://ycv.meibo888.top

[U112] JS：字符串补位
来源：http://cwb.yj20258.top

"7".padStart(3, "0")
来源：http://hrj.shzxlz.cn

[U113] JS：正则替换全部
来源：http://eaf.wangdashe.top

s.replaceAll("a", "b")
来源：http://nwb.wangshuangyany.cn

[U114] JS：JSON 深比较
来源：http://bmk.jyoumei.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vez.guowangkeji.top

[U115] JS：生成 UUID
来源：http://lpv.ehwqpu.com

crypto.randomUUID()
来源：http://xoo.fktsv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ltl.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://nfo.cheryme.top

[U117] JS：单元测试
来源：http://yqy.sweek.top

npm i -D vitest;  npx vitest
来源：http://xkj.yuanzhike.top

[U118] JS：开发服务器
来源：http://euu.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://nmy.fehbvm.com

[U119] JS：生产构建
来源：http://mhn.daxiang520.top

npx vite build
来源：http://lag.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://xlz.chenjidiqi.icu

import.meta.env.VITE_API_URL
来源：http://uki.ivvv.top

================================================================================
来源：http://mmb.xinyue.icu

统计汇总
来源：http://kjv.yj202588.top

================================================================================
来源：http://urq.yonumen.top

按语言统计（条）：
来源：http://wur.haohaochexian.top

Python ......... 252
来源：http://ptd.feifeiyinyue.top

PHP ............ 252
来源：http://cje.daria6918.cn

JavaScript ..... 252
来源：http://cxd.zhoulong.xyz

TypeScript ..... 212
来源：http://cjw.316326.xyz

Java ........... 212
来源：http://ktp.fanxiaobao.xyz

Go ............. 212
来源：http://zhi.9152youxi.cn

Ruby ........... 212
来源：http://jxo.jinqigfzy.top

C# ............. 212
来源：http://ufi.smart0.xyz

C .............. 30
来源：http://fbf.tanke756.top

C++ ............ 30
来源：http://fhd.sxryk.cn

SQL ............ 90
来源：http://blc.uphjek.com

Bash ........... 80
来源：http://kob.gotoacloud.top

Kotlin ......... 15
来源：http://lyt.svipenyu.cn

Swift .......... 15
来源：http://ksd.0kj1m.cn

Lua ............ 10
来源：http://ule.nwbrower.top

Perl ........... 10
来源：http://hwg.nwbrower.top

Scala .......... 10
来源：http://uhr.yfazqb.com

------------------------------------
来源：http://byi.c1oappe.top

合计 ........... 2106 条
来源：http://oia.jiagoushi.top

按章节统计：
来源：http://wqs.316326.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jar.xylfe.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fvo.dashuyun.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://akm.316326.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cmc.gaohongyu789.top


<!-- 参考信息 -->