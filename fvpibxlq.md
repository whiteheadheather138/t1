代发 wailian999

[T45] Perl：数组遍历
来源：http://zfd.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://hze.fehbvm.com

[T46] Perl：哈希操作
来源：http://cwg.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hpb.zdqjudy.top

[T47] Perl：正则捕获
来源：http://eeh.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jry.cdnleiting.top

[T48] Perl：正则替换
来源：http://iri.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://bui.xziqi.cn

[T49] Perl：函数
来源：http://xxw.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rno.xziqi.cn

[T50] Perl：逐行读文件
来源：http://ebn.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vmp.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://asw.sjlbkw.cn

[T51] Scala：Hello World
来源：http://ziw.shanyushiyangkeji.top

println("Hello")
来源：http://pja.wangshuangyany.cn

[T52] Scala：变量
来源：http://dfi.iojbl.cn

val a = 1;  var b = 2
来源：http://rhn.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://ggs.fengsongda.top

s"值: $b"
来源：http://brl.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://tpx.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://lor.zdbjq.cn

[T55] Scala：集合过滤
来源：http://gbk.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://xat.nwbrower.top

[T56] Scala：样例类
来源：http://joi.iojbl.cn

case class User(name: String, age: Int)
来源：http://zbk.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://kza.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cnt.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://mss.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://hno.andypj.xyz

[T59] Scala：循环
来源：http://jar.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://scn.bbcook.cn

[T60] Scala：折叠
来源：http://snq.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://byo.sysykeji.top

================================================================================
来源：http://yrg.andypj.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://udg.xylfe.cn

================================================================================
来源：http://tde.fanxiaobao.xyz

[U01] Py：创建虚拟环境
来源：http://urg.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://jii.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://fvk.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yqf.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://vcd.yanxiufei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gny.hongshengwenyu.top

[U04] Py：变量调试打印
来源：http://lko.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jtp.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://stg.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://rtt.bbcook.cn

[U06] Py：合并两个字典
来源：http://zbb.c1oappe.top

{**a, **b}
来源：http://uzf.bjfxy.top

[U07] Py：反转字典键值
来源：http://pvc.c1oappe.top

{v: k for k, v in d.items()}
来源：http://pye.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://ukz.shangyingyoupin.top

[y for x in nested for y in x]
来源：http://ffm.yfazqb.com

[U09] Py：字典取最大值的键
来源：http://ypr.hcnkem.com

max(d, key=d.get)
来源：http://yws.ybcxt.top

[U10] Py：按值排序字典
来源：http://zwt.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xpq.tian-w.cn

[U11] Py：生成器表达式
来源：http://zfr.guannengcc.top

(x * 2 for x in arr)
来源：http://xhg.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://waj.nanxinkj.top

Counter(arr).most_common(3)
来源：http://fiz.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://fbz.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://hby.shangyingyoupin.top

[U14] Py：分组收集到列表
来源：http://dsx.cdnleiting.top

defaultdict(list)
来源：http://jzu.ppjwa.cn

[U15] Py：高精度计时
来源：http://cxm.hfpthk.cn

t = time.perf_counter()
来源：http://eiq.zhoulong.xyz

[U16] Py：命令行参数解析
来源：http://aex.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rjl.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://eyq.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://gen.daxiang520.top

[U18] Py：预编译正则
来源：http://ohi.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://grf.fehbvm.com

[U19] Py：正则替换带回调
来源：http://suq.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://upl.9152youxi.cn

[U20] Py：缓存函数结果
来源：http://stl.kuanghao11.cn

@functools.lru_cache(maxsize=None)
来源：http://tov.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://shn.hesvh.cn

@contextlib.contextmanager
来源：http://fnc.gzhubu.top

[U22] Py：矩阵转置
来源：http://wur.daxiang520.top

list(zip(*m))
来源：http://lsl.tarul.cn

[U23] Py：分块读取大文件
来源：http://wdb.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qhu.meibo888.top

[U24] Py：路径操作
来源：http://cux.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zxd.ywan-chungtsiang.top

[U25] Py：CSV 按字典读
来源：http://dqq.gotoacloud.top

csv.DictReader(f)
来源：http://gxo.cashguo.top

[U26] Py：并发下载
来源：http://jjj.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ajr.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://owq.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://hms.pengpengdd.cyou

[U28] Py：类型别名
来源：http://svv.shzxlz.cn

UserId = int
来源：http://her.ywan-chungtsiang.top

[U29] Py：属性校验
来源：http://bqr.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://wto.dianchejie.cn

[U30] Py：数据类
来源：http://eqz.guowangkeji.top

@dataclass(slots=True)
来源：http://wjv.fehbvm.com

[U31] Py：单测
来源：http://dte.dashuyun.cn

python -m pytest -q
来源：http://yhy.jinghuilouyu.cn

[U32] Py：代码格式化
来源：http://twn.c1oappe.top

ruff format . && ruff check --fix .
来源：http://baa.c1oappe.top

[U33] Py：打包发布
来源：http://xjy.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://qsj.shzxlz.cn

[U34] Py：判断编码
来源：http://xzl.hysaishi.cn

chardet.detect(raw)
来源：http://crk.ybcxt.top

[U35] Py：发送邮件
来源：http://jat.zhaomingkeji.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fwj.hammf.cn

[U36] Py：定时任务
来源：http://hhh.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ojz.sysykeji.top

[U37] Py：读写 Excel
来源：http://mim.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://kgx.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://jan.jyoumei.cn

Path(__file__).resolve().parent
来源：http://xbw.zhiwuduotai.top

[U39] Py：判断是否在交互环境
来源：http://taw.xinyue.icu

sys.stdout.isatty()
来源：http://xuh.dashuyun.cn

[U40] Py：打印到标准错误
来源：http://jao.52xcode.cn

print("err", file=sys.stderr)
来源：http://czm.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://cfe.hywenlv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pko.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://ate.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ytd.jinqigufen.top

[U43] PHP：声明命名空间
来源：http://ucn.quarkkingdee.top

namespace App\Http;
来源：http://qeh.0kj1m.cn

[U44] PHP：开启严格类型
来源：http://ykj.zhiwuduotai.top

declare(strict_types=1);
来源：http://sgv.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://zld.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aqk.pycfn.com

[U46] PHP：可空类型
来源：http://uns.sxryk.cn

?string $name = null
来源：http://png.hysaishi.cn

[U47] PHP：联合类型
来源：http://fqg.gogol.net.cn

int|string $id
来源：http://ihq.xylfe.cn

[U48] PHP：纯枚举
来源：http://foa.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ohv.meibo888.top

[U49] PHP：只读属性
来源：http://jeq.zhaomingkeji.xyz

public readonly string $name
来源：http://qtq.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://xao.sysykeji.top

public function __construct(private int $id) {}
来源：http://wkb.iojbl.cn

[U51] PHP：数组解构
来源：http://vql.9152youxi.cn

[$a, $b] = $arr;
来源：http://hph.c1oappe.top

[U52] PHP：箭头函数
来源：http://cyf.guowangkeji.top

$double = fn($x) => $x * 2;
来源：http://vur.hammf.cn

[U53] PHP：空合并运算符
来源：http://cgn.sxryk.cn

$v = $a ?? $b ?? "default";
来源：http://nfv.0kj1m.cn

[U54] PHP：空安全调用
来源：http://ecc.epnwcf.com

$obj?->method()
来源：http://qqx.hnqzz.top

[U55] PHP：match 表达式
来源：http://ipj.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fjj.feifeiyinyue.top

[U56] PHP：命名参数
来源：http://nse.yangfankeji.com

f(a: 1, b: 2)
来源：http://nzb.xuetiantiany.cn

[U57] PHP：字符串插值
来源：http://hos.jinghuilouyu.cn

"值: {$a}"
来源：http://cro.fktsv.cn

[U58] PHP：数组三件套
来源：http://dqb.yuxming.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mxc.vqdsnc.cn

[U59] PHP：自定义排序
来源：http://ssr.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pju.yonumen.top

[U60] PHP：JSON 编解码
来源：http://djw.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tvm.wangshuangyany.cn

[U61] PHP：正则
来源：http://hws.hfpthk.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ehm.ydzc1.top

[U62] PHP：日期对象
来源：http://syj.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qfe.hnxiangtu.top

[U63] PHP：文件读写
来源：http://tsg.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fpq.wangdashe.top

[U64] PHP：目录遍历
来源：http://mdm.zhengqikj.top

glob("dir/*.php");  scandir("dir");
来源：http://cxi.yj202588.top

[U65] PHP：会话
来源：http://ted.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lle.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://pne.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://huy.yanxiufei.cn

[U67] PHP：处理文件上传
来源：http://zrr.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yhj.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://wnd.jlsjyb.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wou.hfpthk.cn

[U69] PHP：PDO 预处理
来源：http://cub.zhengqikj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pdp.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://fzg.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lrr.zhengqikj.top

[U71] PHP：抛出异常
来源：http://myo.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://jkm.yuxming.cn

[U72] PHP：写错误日志
来源：http://ogt.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://ebf.ctjpmb.com

[U73] PHP：读取 ini 配置
来源：http://qtl.jinyuanbaomall.cn

parse_ini_file("config.ini", true)
来源：http://yvh.uphjek.com

[U74] PHP：读取环境变量
来源：http://akh.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://xen.xylfe.cn

[U75] PHP：依赖注入
来源：http://qbx.nanxinkj.top

composer require psr/container
来源：http://uhg.vehdjk.com

[U76] PHP：简单路由
来源：http://ooo.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dof.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://tzj.pycfn.com

composer require twig/twig
来源：http://cjh.zdqjudy.top

[U78] PHP：单元测试
来源：http://puc.wangshuangyany.cn

composer require --dev phpunit/phpunit
来源：http://qnu.zhixingplan.top

[U79] PHP：静态分析
来源：http://kua.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://zhq.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://ket.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lsc.yuxming.cn

[U81] JS：初始化项目
来源：http://obf.zhijiandao.cn

npm init -y;  npm i express
来源：http://hfs.jqgufenzy.top

[U82] JS：package.json 脚本
来源：http://ubt.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://asq.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://lvf.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nus.daxiang520.top

[U84] JS：CommonJS 写法
来源：http://rcv.haohaochexian.top

module.exports = { a };  const { a } = require("./m");
来源：http://boj.fengsongda.top

[U85] JS：可选链
来源：http://gll.feifeiyinyue.top

a?.b?.c
来源：http://ouf.gogol.net.cn

[U86] JS：空值合并
来源：http://arn.jinyuanbaomall.cn

a ?? b
来源：http://etc.yuanzhike.top

[U87] JS：解构默认值
来源：http://dml.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://uqc.daria6918.cn

[U88] JS：对象展开合并
来源：http://gug.jinqigufen.top

{ ...a, ...b }
来源：http://tzr.zycfv.cn

[U89] JS：数组去重
来源：http://qnn.pengpengdd.cyou

[...new Set(arr)]
来源：http://cma.zhoulong.xyz

[U90] JS：数字数组排序
来源：http://bwt.zdqjudy.top

[...arr].sort((a, b) => a - b)
来源：http://pjv.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://pui.hammf.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vqm.hesvh.cn

[U92] JS：深拷贝
来源：http://kvy.sweek.top

structuredClone(obj)
来源：http://ecr.aizwys.cn

[U93] JS：模板字符串
来源：http://kzs.wangdashe.top

`共 ${n} 条`
来源：http://wxt.yj20258.top

[U94] JS：箭头函数
来源：http://qml.quarkkingdee.top

const double = x => x * 2;
来源：http://krn.tanke756.top

[U95] JS：Promise 包装
来源：http://ann.ehwqpu.com

new Promise((resolve, reject) => {})
来源：http://osh.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://qoj.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dkv.snrcjt.cn

[U97] JS：并发请求
来源：http://jby.xylfe.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://abu.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://eza.sufxvd.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ufr.aibaodan.cn

[U99] JS：事件监听
来源：http://dzw.shanyushiyangkeji.top

el.addEventListener("click", e => {})
来源：http://hnd.xziqi.cn

[U100] JS：DOM 查询
来源：http://umk.zhoulong.xyz

document.querySelector(".item")
来源：http://apg.yanxiufei.cn

[U101] JS：classList 操作
来源：http://xsx.hywenlv.cn

el.classList.toggle("active")
来源：http://jcv.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://dwb.hongshengwenyu.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wnn.cashguo.top

[U103] JS：定时器
来源：http://hjg.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uva.dianchejie.cn

[U104] JS：防抖
来源：http://cah.yanxiufei.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlg.nwbrower.top

[U105] JS：节流
来源：http://azk.yangfankeji.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xtt.316326.xyz

[U106] JS：日期格式化
来源：http://rbo.fktsv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qdp.svipenyu.cn

[U107] JS：数字千分位
来源：http://gjc.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ldk.zdbjq.cn

[U108] JS：随机整数
来源：http://xbw.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qym.shanyushiyangkeji.top

[U109] JS：数组分组
来源：http://iuw.wangshuangyany.cn

Object.groupBy(arr, x => x.type)
来源：http://aan.haohaochexian.top

[U110] JS：数组分块
来源：http://ila.dashuyun.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xrh.ybcxt.top

[U111] JS：对象转 Map
来源：http://oov.fehbvm.com

new Map(Object.entries(obj))
来源：http://cdz.haohaochexian.top

[U112] JS：字符串补位
来源：http://lwb.ehwqpu.com

"7".padStart(3, "0")
来源：http://olk.wangdashe.top

[U113] JS：正则替换全部
来源：http://bwr.yanxiufei.cn

s.replaceAll("a", "b")
来源：http://tao.yvedp.cn

[U114] JS：JSON 深比较
来源：http://fap.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://chn.cqqwz.cn

[U115] JS：生成 UUID
来源：http://phk.daxiang520.top

crypto.randomUUID()
来源：http://vgo.zycfv.cn

[U116] JS：类型检查（JSDoc）
来源：http://xzv.hysaishi.cn

/** @param {string} name */ function f(name) {}
来源：http://mlf.c1oappe.top

[U117] JS：单元测试
来源：http://kbq.kuanghao11.cn

npm i -D vitest;  npx vitest
来源：http://rju.hcnkem.com

[U118] JS：开发服务器
来源：http://obv.dashuyun.cn

npm i -D vite;  npx vite
来源：http://mmx.yanxiufei.cn

[U119] JS：生产构建
来源：http://ous.ehwqpu.com

npx vite build
来源：http://zqv.fengsongda.top

[U120] JS：读取环境变量（Vite）
来源：http://jqz.zhixingplan.top

import.meta.env.VITE_API_URL
来源：http://wkm.316326.xyz

================================================================================
来源：http://pch.sysykeji.top

统计汇总
来源：http://jiw.chenzaomai.com

================================================================================
来源：http://ale.fengsongda.top

按语言统计（条）：
来源：http://kja.daxiang520.top

Python ......... 252
来源：http://lxd.uphjek.com

PHP ............ 252
来源：http://hmu.sxryk.cn

JavaScript ..... 252
来源：http://dnn.shuidangran.top

TypeScript ..... 212
来源：http://rvb.wangshuangyany.cn

Java ........... 212
来源：http://yfr.feifeiyinyue.top

Go ............. 212
来源：http://mri.zycfv.cn

Ruby ........... 212
来源：http://nnn.zdbjq.cn

C# ............. 212
来源：http://cqr.shangyingyoupin.top

C .............. 30
来源：http://shu.pengpengdd.cyou

C++ ............ 30
来源：http://ycg.xuetiantiany.cn

SQL ............ 90
来源：http://utj.yueranfly.top

Bash ........... 80
来源：http://eca.fktsv.cn

Kotlin ......... 15
来源：http://hia.316326.xyz

Swift .......... 15
来源：http://rbc.fehbvm.com

Lua ............ 10
来源：http://jhs.daria6918.cn

Perl ........... 10
来源：http://fcy.gaohongyu789.top

Scala .......... 10
来源：http://iof.jiagoushi.top

------------------------------------
来源：http://vwq.zdqjudy.top

合计 ........... 2106 条
来源：http://wmv.cashguo.top

按章节统计：
来源：http://gfr.shanyushiyangtech.top


<!-- 参考信息 -->