代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ssc.pengpengdd.cyou

================================================================================
来源：http://gli.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gib.cqqwz.cn

================================================================================
来源：http://hzn.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://qxo.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://iqt.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://fra.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fog.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://lme.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ubz.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://fuc.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lcb.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://qrb.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://cxf.zycfv.cn

[U06] Py：合并两个字典
来源：http://rkb.xziqi.cn

{**a, **b}
来源：http://yqr.dashuyun.cn

[U07] Py：反转字典键值
来源：http://bzk.meibo888.top

{v: k for k, v in d.items()}
来源：http://xyr.aibaodan.cn

[U08] Py：展平二维列表
来源：http://imp.fktsv.cn

[y for x in nested for y in x]
来源：http://eva.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://qkv.ydzc1.top

max(d, key=d.get)
来源：http://xau.xuetiantiany.cn

[U10] Py：按值排序字典
来源：http://gxy.yanxiufei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wej.ivvv.top

[U11] Py：生成器表达式
来源：http://rhm.hywenlv.cn

(x * 2 for x in arr)
来源：http://znh.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ega.ppjwa.cn

Counter(arr).most_common(3)
来源：http://uim.0kj1m.cn

[U13] Py：固定长度队列
来源：http://tqa.uphjek.com

deque(maxlen=10)
来源：http://xqc.xziqi.cn

[U14] Py：分组收集到列表
来源：http://gyi.hesvh.cn

defaultdict(list)
来源：http://cud.gotoacloud.top

[U15] Py：高精度计时
来源：http://fez.yj20258888.top

t = time.perf_counter()
来源：http://icz.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://acx.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://knd.nwbrower.top

[U17] Py：初始化日志
来源：http://sjr.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://xlt.tanke756.top

[U18] Py：预编译正则
来源：http://zba.hcnkem.com

pat = re.compile(r"\d+")
来源：http://ihb.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://bwn.chenlongwang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lxu.cashguo.top

[U20] Py：缓存函数结果
来源：http://urc.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://ypx.guannengcc.top

[U21] Py：自定义上下文管理器
来源：http://poe.cqqwz.cn

@contextlib.contextmanager
来源：http://xsf.cashguo.top

[U22] Py：矩阵转置
来源：http://qpc.hysaishi.cn

list(zip(*m))
来源：http://kzq.yonumen.top

[U23] Py：分块读取大文件
来源：http://etf.chenlongwang.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://taj.tianlin.xyz

[U24] Py：路径操作
来源：http://hes.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wyo.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://gtg.yvedp.cn

csv.DictReader(f)
来源：http://eog.gaohongyu789.top

[U26] Py：并发下载
来源：http://nza.pengpengdd.cyou

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nlv.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://wgt.yanxiufei.cn

aiohttp.ClientSession() 配合 async with
来源：http://chd.quarkkingdee.top

[U28] Py：类型别名
来源：http://neq.chenjidiqi.icu

UserId = int
来源：http://yhj.andypj.xyz

[U29] Py：属性校验
来源：http://khy.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://lkh.hywenlv.cn

[U30] Py：数据类
来源：http://axt.nwbrower.top

@dataclass(slots=True)
来源：http://wcs.ybcxt.top

[U31] Py：单测
来源：http://bnz.fengsongda.top

python -m pytest -q
来源：http://qwb.cashguo.top

[U32] Py：代码格式化
来源：http://uhs.pycfn.com

ruff format . && ruff check --fix .
来源：http://mpo.zhixingplan.top

[U33] Py：打包发布
来源：http://krc.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://iut.hywenlv.cn

[U34] Py：判断编码
来源：http://ttf.gzhubu.top

chardet.detect(raw)
来源：http://dag.kuanghao11.cn

[U35] Py：发送邮件
来源：http://rbs.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vpf.bbcook.cn

[U36] Py：定时任务
来源：http://yzu.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://xfp.smart0.xyz

[U37] Py：读写 Excel
来源：http://ufh.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kpd.shanyushiyangtech.top

[U38] Py：获取脚本所在目录
来源：http://kji.chenzaomai.com

Path(__file__).resolve().parent
来源：http://qed.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://owy.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://loh.316326.xyz

[U40] Py：打印到标准错误
来源：http://ufz.yangfankeji.com

print("err", file=sys.stderr)
来源：http://zgs.ppjwa.cn

[U41] PHP：初始化 Composer 项目
来源：http://icx.fanxiaobao.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://bqm.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://uxc.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://uyi.cashguo.top

[U43] PHP：声明命名空间
来源：http://asp.redwolf501.top

namespace App\Http;
来源：http://ith.tanke756.top

[U44] PHP：开启严格类型
来源：http://hbl.cqqwz.cn

declare(strict_types=1);
来源：http://olb.smart0.xyz

[U45] PHP：类型声明与返回类型
来源：http://yeb.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://czc.ehwqpu.com

[U46] PHP：可空类型
来源：http://rnt.hysaishi.cn

?string $name = null
来源：http://pzj.52xcode.cn

[U47] PHP：联合类型
来源：http://xnz.c1oappe.top

int|string $id
来源：http://qjm.zhengqikj.top

[U48] PHP：纯枚举
来源：http://fty.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://msv.epnwcf.com

[U49] PHP：只读属性
来源：http://uwy.redwolf501.top

public readonly string $name
来源：http://taw.cheryme.top

[U50] PHP：构造器属性提升
来源：http://aps.epnwcf.com

public function __construct(private int $id) {}
来源：http://hmi.guannengcc.top

[U51] PHP：数组解构
来源：http://bve.ydjk.org.cn

[$a, $b] = $arr;
来源：http://afb.daria6918.cn

[U52] PHP：箭头函数
来源：http://srd.yongpay.top

$double = fn($x) => $x * 2;
来源：http://qdq.shangyingyoupin.top

[U53] PHP：空合并运算符
来源：http://zyt.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://nzc.meibo888.top

[U54] PHP：空安全调用
来源：http://pih.9152youxi.cn

$obj?->method()
来源：http://ban.daxiang520.top

[U55] PHP：match 表达式
来源：http://wti.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wpq.bbcook.cn

[U56] PHP：命名参数
来源：http://ken.yangfankeji.com

f(a: 1, b: 2)
来源：http://vnv.fengsongda.top

[U57] PHP：字符串插值
来源：http://cqt.svipenyu.cn

"值: {$a}"
来源：http://yko.epnwcf.com

[U58] PHP：数组三件套
来源：http://qlj.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uir.zhijiandao.cn

[U59] PHP：自定义排序
来源：http://yis.jianghu66.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aiu.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://ewe.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dbl.gogol.net.cn

[U61] PHP：正则
来源：http://yto.havefunace.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tew.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://vjt.cashguo.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jah.gaohongyu789.top

[U63] PHP：文件读写
来源：http://iwh.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://may.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://fkf.316326.xyz

glob("dir/*.php");  scandir("dir");
来源：http://hyr.yj20258.top

[U65] PHP：会话
来源：http://csq.zycfv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xxs.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://dwj.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://psz.shanyushiyangkeji.top

[U67] PHP：处理文件上传
来源：http://neu.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kwd.smart0.xyz

[U68] PHP：PDO 连接
来源：http://pkh.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ofh.ydjk.org.cn

[U69] PHP：PDO 预处理
来源：http://fjz.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wsp.yongpay.top

[U70] PHP：PDO 事务
来源：http://rvo.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kic.zycfv.cn

[U71] PHP：抛出异常
来源：http://yzw.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://fbf.meibo888.top

[U72] PHP：写错误日志
来源：http://cdq.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://zwu.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://wek.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://krx.sysykeji.top

[U74] PHP：读取环境变量
来源：http://ewn.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://utt.ydzc1.top

[U75] PHP：依赖注入
来源：http://ljp.jyoumei.cn

composer require psr/container
来源：http://izz.svipenyu.cn

[U76] PHP：简单路由
来源：http://yus.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tgh.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://wvu.hnqzz.top

composer require twig/twig
来源：http://grp.daria6918.cn

[U78] PHP：单元测试
来源：http://fnc.jinqigufen.top

composer require --dev phpunit/phpunit
来源：http://wvy.epnwcf.com

[U79] PHP：静态分析
来源：http://uqt.chenlongwang.top

composer require --dev phpstan/phpstan
来源：http://nvk.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://ask.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qyh.jlsjyb.cn

[U81] JS：初始化项目
来源：http://uxt.smart0.xyz

npm init -y;  npm i express
来源：http://byo.jianghu66.top

[U82] JS：package.json 脚本
来源：http://nwo.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qjr.tanke756.top

[U83] JS：ES Module 导入导出
来源：http://scl.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://kek.ydjk.org.cn

[U84] JS：CommonJS 写法
来源：http://pzg.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gnk.ctjpmb.com

[U85] JS：可选链
来源：http://dpj.bbcook.cn

a?.b?.c
来源：http://oca.yongpay.top

[U86] JS：空值合并
来源：http://bkv.chenjidiqi.icu

a ?? b
来源：http://tpc.xziqi.cn

[U87] JS：解构默认值
来源：http://cvn.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://djk.quarkkingdee.top

[U88] JS：对象展开合并
来源：http://ejz.sjlbkw.cn

{ ...a, ...b }
来源：http://cbx.chenzaomai.com

[U89] JS：数组去重
来源：http://yrl.c1oappe.top

[...new Set(arr)]
来源：http://anh.fehbvm.com

[U90] JS：数字数组排序
来源：http://tan.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://tqr.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://jpl.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://oos.daria6918.cn

[U92] JS：深拷贝
来源：http://qkj.cashguo.top

structuredClone(obj)
来源：http://gkw.zycfv.cn

[U93] JS：模板字符串
来源：http://los.hnqzz.top

`共 ${n} 条`
来源：http://kqb.hywenlv.cn

[U94] JS：箭头函数
来源：http://jxr.epnwcf.com

const double = x => x * 2;
来源：http://uuy.ybcxt.top

[U95] JS：Promise 包装
来源：http://xxj.hammf.cn

new Promise((resolve, reject) => {})
来源：http://gmm.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://itp.xziqi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qdm.daxiang520.top

[U97] JS：并发请求
来源：http://hhg.yanxiufei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yww.epnwcf.com

[U98] JS：fetch 带 JSON
来源：http://tkf.hongshengwenyu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fkw.havefunace.top

[U99] JS：事件监听
来源：http://sqe.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://iap.svipenyu.cn

[U100] JS：DOM 查询
来源：http://kcw.zhongyouzk.top

document.querySelector(".item")
来源：http://ufi.nanxuanxn.top

[U101] JS：classList 操作
来源：http://fmv.ywan-chungtsiang.top

el.classList.toggle("active")
来源：http://eta.jinyuanbaomall.cn

[U102] JS：本地存储
来源：http://hhf.yvedp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://mpc.zhijiandao.cn

[U103] JS：定时器
来源：http://ogb.daria6918.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wum.ivvv.top

[U104] JS：防抖
来源：http://cvi.sysykeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhn.daxiang520.top

[U105] JS：节流
来源：http://ydp.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iqa.daxiang520.top

[U106] JS：日期格式化
来源：http://cfr.xylfe.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lzu.vqdsnc.cn

[U107] JS：数字千分位
来源：http://bxc.yonumen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qvn.yueranfly.top

[U108] JS：随机整数
来源：http://mka.zhaomingkeji.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ovn.hnqzz.top

[U109] JS：数组分组
来源：http://inw.cdnleiting.top

Object.groupBy(arr, x => x.type)
来源：http://zag.yfazqb.com

[U110] JS：数组分块
来源：http://dkt.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gdm.yueranfly.top

[U111] JS：对象转 Map
来源：http://ycf.cqqwz.cn

new Map(Object.entries(obj))
来源：http://pal.cashguo.top

[U112] JS：字符串补位
来源：http://jxg.hammf.cn

"7".padStart(3, "0")
来源：http://kzc.jqgfzy.top

[U113] JS：正则替换全部
来源：http://zdw.tian-w.cn

s.replaceAll("a", "b")
来源：http://xgg.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://ypb.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ntv.yuxming.cn

[U115] JS：生成 UUID
来源：http://spc.yvedp.cn

crypto.randomUUID()
来源：http://xdu.sufxvd.cn

[U116] JS：类型检查（JSDoc）
来源：http://cyh.meibo888.top

/** @param {string} name */ function f(name) {}
来源：http://vyo.ppjwa.cn

[U117] JS：单元测试
来源：http://iei.bbcook.cn

npm i -D vitest;  npx vitest
来源：http://mde.guannengcc.top

[U118] JS：开发服务器
来源：http://bdp.jinyuanbaomall.cn

npm i -D vite;  npx vite
来源：http://tgi.quarkkingdee.top

[U119] JS：生产构建
来源：http://pqu.yonumen.top

npx vite build
来源：http://ylb.ctjpmb.com

[U120] JS：读取环境变量（Vite）
来源：http://buz.yj20258888.top

import.meta.env.VITE_API_URL
来源：http://zwa.yj20258.top

================================================================================
来源：http://ztr.daria6918.cn

统计汇总
来源：http://uth.hfpthk.cn

================================================================================
来源：http://sse.chenlongwang.top

按语言统计（条）：
来源：http://yju.quarkkingdee.top

Python ......... 252
来源：http://cji.jianghu66.top

PHP ............ 252
来源：http://vhf.nanxinkj.top

JavaScript ..... 252
来源：http://xzh.sxryk.cn

TypeScript ..... 212
来源：http://cei.zdqjudy.top

Java ........... 212
来源：http://fzr.gogol.net.cn

Go ............. 212
来源：http://ysn.nwbrower.top

Ruby ........... 212
来源：http://zcf.yj202588.top

C# ............. 212
来源：http://imt.gotoacloud.top

C .............. 30
来源：http://ioi.yangfankeji.com

C++ ............ 30
来源：http://oig.cdnleiting.top

SQL ............ 90
来源：http://nxk.epnwcf.com

Bash ........... 80
来源：http://ahp.dianchejie.cn

Kotlin ......... 15
来源：http://gpm.chenlongwang.top

Swift .......... 15
来源：http://utl.jinqigufen.top

Lua ............ 10
来源：http://cfj.epnwcf.com

Perl ........... 10
来源：http://uvy.bjfxy.top

Scala .......... 10
来源：http://hfs.cqqwz.cn

------------------------------------
来源：http://uhz.cheryme.top

合计 ........... 2106 条
来源：http://wob.zhijiandao.cn

按章节统计：
来源：http://nok.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vqj.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ktf.mhx1999.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dal.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fcy.iojbl.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjh.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gmk.ehwqpu.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vlm.xylfe.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qsm.cqqwz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://oav.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://slz.jinqigfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zbd.vehdjk.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qir.yueranfly.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kul.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yib.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cav.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://den.xuetiantiany.cn

Q SQL 专题                              90
来源：http://num.yvedp.cn

R Bash 专题                             80
来源：http://beh.nwbrower.top

S C / C++ 专题                          60
来源：http://hfy.hesvh.cn

T 其他语言补充                          60
来源：http://vol.yongpay.top

U 高频实用片段                         120
来源：http://bhi.zhijiandao.cn

------------------------------------
来源：http://asq.guowangkeji.top

合计                                  2106 条
来源：http://zuu.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://jax.cashguo.top

使用提醒
来源：http://auq.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://mzk.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ypa.guowangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cjq.xziqi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eiu.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qwk.yuanzhike.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://odw.shanyushiyangkeji.top

—— 文件结束 ——
来源：http://yly.jiagoushi.top


<!-- 参考信息 -->