代发 wailian999

[T47] Perl：正则捕获
来源：http://hml.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://aiu.gotoacloud.top

[T48] Perl：正则替换
来源：http://hue.cdnleiting.top

$s =~ s/old/new/g;
来源：http://bvo.jqgufenzy.top

[T49] Perl：函数
来源：http://axw.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ewt.hnqzz.top

[T50] Perl：逐行读文件
来源：http://bem.zdqjudy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dvi.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://ljz.fanxiaobao.xyz

[T51] Scala：Hello World
来源：http://ynf.ydzc1.top

println("Hello")
来源：http://kxg.guannengcc.top

[T52] Scala：变量
来源：http://doz.9152youxi.cn

val a = 1;  var b = 2
来源：http://dez.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://cxe.yuanzhike.top

s"值: $b"
来源：http://giu.pycfn.com

[T54] Scala：集合映射
来源：http://uqi.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://vak.birdmap.top

[T55] Scala：集合过滤
来源：http://wmr.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://okr.svipenyu.cn

[T56] Scala：样例类
来源：http://sax.shuidangran.top

case class User(name: String, age: Int)
来源：http://kkr.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://las.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jve.fktsv.cn

[T58] Scala：函数定义
来源：http://zrz.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://zzr.cucudq.cn

[T59] Scala：循环
来源：http://qwa.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://zqh.fengsongda.top

[T60] Scala：折叠
来源：http://zvq.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qzq.yangfankeji.com

================================================================================
来源：http://cqt.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pha.hesvh.cn

================================================================================
来源：http://wsn.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://yac.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://mpi.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://qki.ywan-chungtsiang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://srv.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://tdy.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://amf.chenzaomai.com

[U04] Py：变量调试打印
来源：http://cyr.fanxiaobao.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xke.daria6918.cn

[U05] Py：列表去重且保序
来源：http://giu.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://geb.hnqzz.top

[U06] Py：合并两个字典
来源：http://vqp.tanke756.top

{**a, **b}
来源：http://aeq.hywenlv.cn

[U07] Py：反转字典键值
来源：http://edr.hysaishi.cn

{v: k for k, v in d.items()}
来源：http://eqh.ehwqpu.com

[U08] Py：展平二维列表
来源：http://lan.hcnkem.com

[y for x in nested for y in x]
来源：http://vym.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://bda.yongpay.top

max(d, key=d.get)
来源：http://ayy.yuxming.cn

[U10] Py：按值排序字典
来源：http://two.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pzy.yangfankeji.com

[U11] Py：生成器表达式
来源：http://ort.yonumen.top

(x * 2 for x in arr)
来源：http://jvl.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://vwx.hywenlv.cn

Counter(arr).most_common(3)
来源：http://roz.gogol.net.cn

[U13] Py：固定长度队列
来源：http://gtm.hongshengwenyu.top

deque(maxlen=10)
来源：http://vtr.yj20258.top

[U14] Py：分组收集到列表
来源：http://brg.daxiang520.top

defaultdict(list)
来源：http://sqt.shzxlz.cn

[U15] Py：高精度计时
来源：http://tva.cqqwz.cn

t = time.perf_counter()
来源：http://vzw.shuidangran.top

[U16] Py：命令行参数解析
来源：http://cbr.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tpa.zycfv.cn

[U17] Py：初始化日志
来源：http://tdj.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://uic.zycfv.cn

[U18] Py：预编译正则
来源：http://ysq.zhiwuduotai.top

pat = re.compile(r"\d+")
来源：http://zee.meibo888.top

[U19] Py：正则替换带回调
来源：http://twg.bjfxy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://axj.daxiang520.top

[U20] Py：缓存函数结果
来源：http://nye.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://rxf.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://gdq.dashuyun.cn

@contextlib.contextmanager
来源：http://htc.jinghuilouyu.cn

[U22] Py：矩阵转置
来源：http://arz.xingfuxueyuan.xyz

list(zip(*m))
来源：http://urm.yonumen.top

[U23] Py：分块读取大文件
来源：http://adr.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wtx.hfpthk.cn

[U24] Py：路径操作
来源：http://dft.yuanzhike.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://utg.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://xlb.andypj.xyz

csv.DictReader(f)
来源：http://lrk.snrcjt.cn

[U26] Py：并发下载
来源：http://zrq.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://axr.wangdashe.top

[U27] Py：异步 HTTP
来源：http://ebh.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://tfo.xziqi.cn

[U28] Py：类型别名
来源：http://psg.9152youxi.cn

UserId = int
来源：http://mbc.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://wgn.sxryk.cn

@property 与 @x.setter 配合
来源：http://ndr.aibaodan.cn

[U30] Py：数据类
来源：http://fgm.dianchejie.cn

@dataclass(slots=True)
来源：http://nqm.nwbrower.top

[U31] Py：单测
来源：http://uos.sufxvd.cn

python -m pytest -q
来源：http://sha.jianghu66.top

[U32] Py：代码格式化
来源：http://gvc.guannengcc.top

ruff format . && ruff check --fix .
来源：http://kci.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://klo.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://wej.fktsv.cn

[U34] Py：判断编码
来源：http://cbt.cdnleiting.top

chardet.detect(raw)
来源：http://rxs.xinyue.icu

[U35] Py：发送邮件
来源：http://tya.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fia.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://dfm.gzhubu.top

schedule.every(10).minutes.do(job)
来源：http://gwh.zhengqikj.top

[U37] Py：读写 Excel
来源：http://hhc.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://ill.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://kru.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://kmr.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://cso.tanke756.top

sys.stdout.isatty()
来源：http://sax.xuetiantiany.cn

[U40] Py：打印到标准错误
来源：http://wfl.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://ofx.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://yni.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qay.kuanghao11.cn

[U42] PHP：PSR-4 自动加载
来源：http://pul.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jjz.daria6918.cn

[U43] PHP：声明命名空间
来源：http://nin.uphjek.com

namespace App\Http;
来源：http://lcl.hammf.cn

[U44] PHP：开启严格类型
来源：http://xwt.dashuyun.cn

declare(strict_types=1);
来源：http://fwd.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://icz.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://sis.yongpay.top

[U46] PHP：可空类型
来源：http://fcc.svipenyu.cn

?string $name = null
来源：http://xpk.guowangkeji.top

[U47] PHP：联合类型
来源：http://luy.dianchejie.cn

int|string $id
来源：http://ifc.nwbrower.top

[U48] PHP：纯枚举
来源：http://mbd.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ngw.sweek.top

[U49] PHP：只读属性
来源：http://wyx.smart0.xyz

public readonly string $name
来源：http://vjw.yj20258888.top

[U50] PHP：构造器属性提升
来源：http://ptk.zhongyouzk.top

public function __construct(private int $id) {}
来源：http://ccy.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://svv.yuanzhike.top

[$a, $b] = $arr;
来源：http://guc.zdbjq.cn

[U52] PHP：箭头函数
来源：http://obu.cashguo.top

$double = fn($x) => $x * 2;
来源：http://foc.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://lnq.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://xve.cdnleiting.top

[U54] PHP：空安全调用
来源：http://hfm.ctjpmb.com

$obj?->method()
来源：http://aci.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://hnj.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vjz.cheryme.top

[U56] PHP：命名参数
来源：http://cwq.xylfe.cn

f(a: 1, b: 2)
来源：http://qxq.epnwcf.com

[U57] PHP：字符串插值
来源：http://iwk.hnxiangtu.top

"值: {$a}"
来源：http://ydh.redwolf501.top

[U58] PHP：数组三件套
来源：http://sly.jqgfzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xuf.pycfn.com

[U59] PHP：自定义排序
来源：http://mle.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fgz.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://qpu.sufxvd.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fpv.316326.xyz

[U61] PHP：正则
来源：http://njg.nanxinkj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dne.iojbl.cn

[U62] PHP：日期对象
来源：http://lef.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://apx.redwolf501.top

[U63] PHP：文件读写
来源：http://get.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fok.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://zxu.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://emc.hesvh.cn

[U65] PHP：会话
来源：http://cxw.yfazqb.com

session_start();  $_SESSION["uid"] = 1;
来源：http://eei.cucudq.cn

[U66] PHP：设置 Cookie
来源：http://mwe.shanyushiyangtech.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tii.pycfn.com

[U67] PHP：处理文件上传
来源：http://ynx.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mmt.hcnkem.com

[U68] PHP：PDO 连接
来源：http://rcw.zhongyouzk.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tvq.jinyuanbaomall.cn

[U69] PHP：PDO 预处理
来源：http://utt.fzhhl.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tdy.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://ied.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lqi.daxiang520.top

[U71] PHP：抛出异常
来源：http://ymz.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://pnc.yj20258888.top

[U72] PHP：写错误日志
来源：http://hde.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://nbs.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://hjn.zdbjq.cn

parse_ini_file("config.ini", true)
来源：http://jov.cheryme.top

[U74] PHP：读取环境变量
来源：http://lzx.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://qna.xziqi.cn

[U75] PHP：依赖注入
来源：http://klv.ehwqpu.com

composer require psr/container
来源：http://ybh.haohaochexian.top

[U76] PHP：简单路由
来源：http://jrg.hesvh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cap.sweek.top

[U77] PHP：模板渲染
来源：http://enu.xylfe.cn

composer require twig/twig
来源：http://rmu.aibaodan.cn

[U78] PHP：单元测试
来源：http://lbu.cashguo.top

composer require --dev phpunit/phpunit
来源：http://gox.hnqzz.top

[U79] PHP：静态分析
来源：http://kzc.yj20258.top

composer require --dev phpstan/phpstan
来源：http://uaw.xylfe.cn

[U80] PHP：代码规范修复
来源：http://bkx.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pmw.dashuyun.cn

[U81] JS：初始化项目
来源：http://bhj.guowangkeji.top

npm init -y;  npm i express
来源：http://pxb.daria6918.cn

[U82] JS：package.json 脚本
来源：http://xhc.jianghu66.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qld.zycfv.cn

[U83] JS：ES Module 导入导出
来源：http://jxe.cqqwz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ico.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://xfk.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://ojh.zhongyouzk.top

[U85] JS：可选链
来源：http://kai.yfazqb.com

a?.b?.c
来源：http://igy.shuidangran.top

[U86] JS：空值合并
来源：http://grm.shzxlz.cn

a ?? b
来源：http://rei.hesvh.cn

[U87] JS：解构默认值
来源：http://doy.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://hfe.sufxvd.cn

[U88] JS：对象展开合并
来源：http://pyt.chenzaomai.com

{ ...a, ...b }
来源：http://fqx.nanxinkj.top

[U89] JS：数组去重
来源：http://jnv.yj20258888.top

[...new Set(arr)]
来源：http://rfi.hesvh.cn

[U90] JS：数字数组排序
来源：http://wra.ehwqpu.com

[...arr].sort((a, b) => a - b)
来源：http://pft.meibo888.top

[U91] JS：对象键值遍历
来源：http://uqu.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://frc.hongshengwenyu.top

[U92] JS：深拷贝
来源：http://uez.gzhubu.top

structuredClone(obj)
来源：http://cql.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://cxe.cashguo.top

`共 ${n} 条`
来源：http://aoo.shuidangran.top

[U94] JS：箭头函数
来源：http://vpw.yuxming.cn

const double = x => x * 2;
来源：http://xjl.316326.xyz

[U95] JS：Promise 包装
来源：http://uzs.sysykeji.top

new Promise((resolve, reject) => {})
来源：http://wpp.tanke756.top

[U96] JS：async/await 与异常
来源：http://zfi.fktsv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://diw.dianchejie.cn

[U97] JS：并发请求
来源：http://yeo.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xpb.hfpthk.cn

[U98] JS：fetch 带 JSON
来源：http://rgw.vqdsnc.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tur.gogol.net.cn

[U99] JS：事件监听
来源：http://fjh.yj20258888.top

el.addEventListener("click", e => {})
来源：http://zfh.hcnkem.com

[U100] JS：DOM 查询
来源：http://zzb.ydjk.org.cn

document.querySelector(".item")
来源：http://jne.yfazqb.com

[U101] JS：classList 操作
来源：http://jlw.sysykeji.top

el.classList.toggle("active")
来源：http://dwb.bbcook.cn

[U102] JS：本地存储
来源：http://zka.ppjwa.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ljq.fengsongda.top

[U103] JS：定时器
来源：http://hje.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zho.nanxinkj.top

[U104] JS：防抖
来源：http://qme.redwolf501.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hct.yj20258888.top

[U105] JS：节流
来源：http://atu.ybcxt.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nek.jinghuilouyu.cn

[U106] JS：日期格式化
来源：http://ywk.yanxiufei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uym.ybcxt.top

[U107] JS：数字千分位
来源：http://jpl.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bee.hcnkem.com

[U108] JS：随机整数
来源：http://ijo.xziqi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wua.yj202588.top

[U109] JS：数组分组
来源：http://rdb.yj202588.top

Object.groupBy(arr, x => x.type)
来源：http://elj.sjlbkw.cn

[U110] JS：数组分块
来源：http://axg.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nys.jinyuanbaomall.cn

[U111] JS：对象转 Map
来源：http://eca.bbcook.cn

new Map(Object.entries(obj))
来源：http://jex.jianghu66.top

[U112] JS：字符串补位
来源：http://hox.zhixingplan.top

"7".padStart(3, "0")
来源：http://uqv.zdqjudy.top

[U113] JS：正则替换全部
来源：http://agf.zdbjq.cn

s.replaceAll("a", "b")
来源：http://shx.hesvh.cn

[U114] JS：JSON 深比较
来源：http://fgl.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ood.zdqjudy.top

[U115] JS：生成 UUID
来源：http://haq.hysaishi.cn

crypto.randomUUID()
来源：http://epz.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://kpq.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://xso.sysykeji.top

[U117] JS：单元测试
来源：http://wjk.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://wyc.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://ito.jinghuilouyu.cn

npm i -D vite;  npx vite
来源：http://fpg.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://sxu.yangfankeji.com

npx vite build
来源：http://gbq.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://luu.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://iyv.aizwys.cn

================================================================================
来源：http://aad.andypj.xyz

统计汇总
来源：http://fvs.ybcxt.top

================================================================================
来源：http://lmh.ydjk.org.cn

按语言统计（条）：
来源：http://jvl.guowangkeji.top

Python ......... 252
来源：http://ioc.uphjek.com

PHP ............ 252
来源：http://pja.zhengqikj.top

JavaScript ..... 252
来源：http://rld.jinqigfzy.top

TypeScript ..... 212
来源：http://jww.daxiang520.top

Java ........... 212
来源：http://xfv.ywan-chungtsiang.top

Go ............. 212
来源：http://snu.hfpthk.cn

Ruby ........... 212
来源：http://det.hesvh.cn

C# ............. 212
来源：http://ztm.svipenyu.cn

C .............. 30
来源：http://kjh.wangshuangyany.cn

C++ ............ 30
来源：http://gue.nwbrower.top

SQL ............ 90
来源：http://pug.quarkkingdee.top

Bash ........... 80
来源：http://rmd.smart0.xyz

Kotlin ......... 15
来源：http://eon.yuanzhike.top

Swift .......... 15
来源：http://prj.sxryk.cn

Lua ............ 10
来源：http://vkz.ydzc1.top

Perl ........... 10
来源：http://uid.daria6918.cn

Scala .......... 10
来源：http://axz.sysykeji.top

------------------------------------
来源：http://kfy.yanxiufei.cn

合计 ........... 2106 条
来源：http://gbb.tian-w.cn

按章节统计：
来源：http://tmr.yongpay.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jia.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bfy.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kcv.kuanghao11.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rno.sjlbkw.cn


<!-- 参考信息 -->