代发 wailian999

[U03] Py：加载 .env 配置
来源：http://dpr.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vbm.cheryme.top

[U04] Py：变量调试打印
来源：http://jaw.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pui.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://twt.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://lhk.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://ffb.xylfe.cn

{**a, **b}
来源：http://ivb.birdmap.top

[U07] Py：反转字典键值
来源：http://mdy.tian-w.cn

{v: k for k, v in d.items()}
来源：http://ile.yvedp.cn

[U08] Py：展平二维列表
来源：http://org.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://phr.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://bcb.guannengcc.top

max(d, key=d.get)
来源：http://irw.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://cgw.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tgy.zhixingplan.top

[U11] Py：生成器表达式
来源：http://his.fzhhl.top

(x * 2 for x in arr)
来源：http://qji.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://psq.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://obg.fehbvm.com

[U13] Py：固定长度队列
来源：http://aar.snrcjt.cn

deque(maxlen=10)
来源：http://hhj.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://oyk.hnxiangtu.top

defaultdict(list)
来源：http://xpw.sxryk.cn

[U15] Py：高精度计时
来源：http://xqk.gogol.net.cn

t = time.perf_counter()
来源：http://vsz.meibo888.top

[U16] Py：命令行参数解析
来源：http://tjd.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tih.tanke756.top

[U17] Py：初始化日志
来源：http://pob.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://eqf.cucudq.cn

[U18] Py：预编译正则
来源：http://omf.ybcxt.top

pat = re.compile(r"\d+")
来源：http://myc.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://yuz.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zhb.zycfv.cn

[U20] Py：缓存函数结果
来源：http://hyc.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://ppt.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://ocl.smart0.xyz

@contextlib.contextmanager
来源：http://yfw.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://stk.fengsongda.top

list(zip(*m))
来源：http://ixn.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://itl.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cfl.epnwcf.com

[U24] Py：路径操作
来源：http://vin.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pcq.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://zjd.sweek.top

csv.DictReader(f)
来源：http://xso.hywenlv.cn

[U26] Py：并发下载
来源：http://qvv.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jdy.zdbjq.cn

[U27] Py：异步 HTTP
来源：http://bog.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://hqt.vqdsnc.cn

[U28] Py：类型别名
来源：http://gif.jinyuanbaomall.cn

UserId = int
来源：http://ahp.xylfe.cn

[U29] Py：属性校验
来源：http://kla.bbcook.cn

@property 与 @x.setter 配合
来源：http://nol.mhx1999.top

[U30] Py：数据类
来源：http://mch.chenjidiqi.icu

@dataclass(slots=True)
来源：http://ofs.shanyushiyangkeji.top

[U31] Py：单测
来源：http://erq.zycfv.cn

python -m pytest -q
来源：http://omu.sweek.top

[U32] Py：代码格式化
来源：http://xbg.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://oir.vqdsnc.cn

[U33] Py：打包发布
来源：http://ccy.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://jnr.0kj1m.cn

[U34] Py：判断编码
来源：http://cod.316326.xyz

chardet.detect(raw)
来源：http://qkp.sysykeji.top

[U35] Py：发送邮件
来源：http://osn.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pre.ydzc1.top

[U36] Py：定时任务
来源：http://rpa.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://hts.gzhubu.top

[U37] Py：读写 Excel
来源：http://wkd.dashuyun.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ash.jyoumei.cn

[U38] Py：获取脚本所在目录
来源：http://bfx.sxryk.cn

Path(__file__).resolve().parent
来源：http://bdo.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://ldw.chenlongwang.top

sys.stdout.isatty()
来源：http://jgb.tanke756.top

[U40] Py：打印到标准错误
来源：http://jsa.9152youxi.cn

print("err", file=sys.stderr)
来源：http://vfu.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://fww.hongshengwenyu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ctg.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://nda.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gil.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://jev.xinyue.icu

namespace App\Http;
来源：http://jzk.cashguo.top

[U44] PHP：开启严格类型
来源：http://pwz.uphjek.com

declare(strict_types=1);
来源：http://zuc.yueranfly.top

[U45] PHP：类型声明与返回类型
来源：http://ctl.feifeiyinyue.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xpr.shanyushiyangkeji.top

[U46] PHP：可空类型
来源：http://alh.chenlongwang.top

?string $name = null
来源：http://xlf.zdqjudy.top

[U47] PHP：联合类型
来源：http://tby.daria6918.cn

int|string $id
来源：http://cfh.fehbvm.com

[U48] PHP：纯枚举
来源：http://hne.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ncq.chenzaomai.com

[U49] PHP：只读属性
来源：http://env.kuanghao11.cn

public readonly string $name
来源：http://xqt.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://iyt.fktsv.cn

public function __construct(private int $id) {}
来源：http://uye.cqqwz.cn

[U51] PHP：数组解构
来源：http://lja.cqqwz.cn

[$a, $b] = $arr;
来源：http://ada.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://bad.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://mpn.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://ulb.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://qdb.bjfxy.top

[U54] PHP：空安全调用
来源：http://igs.cheryme.top

$obj?->method()
来源：http://idg.jinqigfzy.top

[U55] PHP：match 表达式
来源：http://mdr.yj20258.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fwb.cashguo.top

[U56] PHP：命名参数
来源：http://now.mhx1999.top

f(a: 1, b: 2)
来源：http://lsk.yangfankeji.com

[U57] PHP：字符串插值
来源：http://jgk.ivvv.top

"值: {$a}"
来源：http://ebn.iojbl.cn

[U58] PHP：数组三件套
来源：http://hpd.xziqi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ixy.xuanzx.com

[U59] PHP：自定义排序
来源：http://twm.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kms.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://aoe.hcnkem.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ypa.zdbjq.cn

[U61] PHP：正则
来源：http://cto.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lgt.hammf.cn

[U62] PHP：日期对象
来源：http://gzb.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xzi.fengsongda.top

[U63] PHP：文件读写
来源：http://hkq.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nxv.svipenyu.cn

[U64] PHP：目录遍历
来源：http://jjz.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://wrh.wangshuangyany.cn

[U65] PHP：会话
来源：http://sfe.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://afb.yanxiufei.cn

[U66] PHP：设置 Cookie
来源：http://pdj.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cwc.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://pnx.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://npy.yj202588.top

[U68] PHP：PDO 连接
来源：http://osh.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nel.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://ncp.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rjx.shanyushiyangtech.top

[U70] PHP：PDO 事务
来源：http://lni.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yeo.cqqwz.cn

[U71] PHP：抛出异常
来源：http://kqi.bbcook.cn

throw new RuntimeException("失败", 500);
来源：http://zgu.epnwcf.com

[U72] PHP：写错误日志
来源：http://xlh.zhaomingkeji.xyz

error_log("失败: " . $e->getMessage());
来源：http://hci.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://pgz.svipenyu.cn

parse_ini_file("config.ini", true)
来源：http://czf.sweek.top

[U74] PHP：读取环境变量
来源：http://lja.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://agv.epnwcf.com

[U75] PHP：依赖注入
来源：http://xkm.daxiang520.top

composer require psr/container
来源：http://tmz.yuxming.cn

[U76] PHP：简单路由
来源：http://rxz.nanxuanxn.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zlq.sxryk.cn

[U77] PHP：模板渲染
来源：http://fsj.jlsjyb.cn

composer require twig/twig
来源：http://fiq.nanxinkj.top

[U78] PHP：单元测试
来源：http://vld.aibaodan.cn

composer require --dev phpunit/phpunit
来源：http://peb.vqdsnc.cn

[U79] PHP：静态分析
来源：http://qvm.yj20258.top

composer require --dev phpstan/phpstan
来源：http://lja.xuanzx.com

[U80] PHP：代码规范修复
来源：http://xyc.yuanzhike.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://wqw.cqqwz.cn

[U81] JS：初始化项目
来源：http://ejl.haohaochexian.top

npm init -y;  npm i express
来源：http://ugk.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://ofh.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jjr.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://yss.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://vbn.ywan-chungtsiang.top

[U84] JS：CommonJS 写法
来源：http://xeu.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://boo.tian-w.cn

[U85] JS：可选链
来源：http://yhu.zhengqikj.top

a?.b?.c
来源：http://xjs.316326.xyz

[U86] JS：空值合并
来源：http://upy.jiagoushi.top

a ?? b
来源：http://psv.zhixingplan.top

[U87] JS：解构默认值
来源：http://phg.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://vqy.guannengcc.top

[U88] JS：对象展开合并
来源：http://zln.nanxuanxn.top

{ ...a, ...b }
来源：http://lvm.fktsv.cn

[U89] JS：数组去重
来源：http://mpc.wangshuangyany.cn

[...new Set(arr)]
来源：http://rpf.svipenyu.cn

[U90] JS：数字数组排序
来源：http://hhq.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://hwf.birdmap.top

[U91] JS：对象键值遍历
来源：http://qyv.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvd.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://rha.yueranfly.top

structuredClone(obj)
来源：http://eyz.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://hki.gogol.net.cn

`共 ${n} 条`
来源：http://hdr.wangdashe.top

[U94] JS：箭头函数
来源：http://wcy.hfpthk.cn

const double = x => x * 2;
来源：http://ddj.bjfxy.top

[U95] JS：Promise 包装
来源：http://ufj.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://jmy.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://poz.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://flp.iojbl.cn

[U97] JS：并发请求
来源：http://cyv.ivvv.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://psg.shzxlz.cn

[U98] JS：fetch 带 JSON
来源：http://lxk.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gbi.ybcxt.top

[U99] JS：事件监听
来源：http://oea.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://zks.chenlongwang.top

[U100] JS：DOM 查询
来源：http://lye.yueranfly.top

document.querySelector(".item")
来源：http://gwd.316326.xyz

[U101] JS：classList 操作
来源：http://yvh.chenjidiqi.icu

el.classList.toggle("active")
来源：http://tjs.bjfxy.top

[U102] JS：本地存储
来源：http://qfu.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hjq.dashuyun.cn

[U103] JS：定时器
来源：http://ssv.bbcook.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://njc.fehbvm.com

[U104] JS：防抖
来源：http://bsp.zhoulong.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asl.xuanzx.com

[U105] JS：节流
来源：http://fna.yuanzhike.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ffz.aizwys.cn

[U106] JS：日期格式化
来源：http://xbc.meibo888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qun.shangyingyoupin.top

[U107] JS：数字千分位
来源：http://jcm.316326.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://alv.shuidangran.top

[U108] JS：随机整数
来源：http://vqp.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ssw.jianghu66.top

[U109] JS：数组分组
来源：http://qql.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://ugp.shanyushiyangtech.top

[U110] JS：数组分块
来源：http://cfp.tian-w.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://owe.ppjwa.cn

[U111] JS：对象转 Map
来源：http://rfg.chenlongwang.top

new Map(Object.entries(obj))
来源：http://hxg.havefunace.top

[U112] JS：字符串补位
来源：http://xkb.zhoulong.xyz

"7".padStart(3, "0")
来源：http://bey.jianghu66.top

[U113] JS：正则替换全部
来源：http://ees.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://dkx.cashguo.top

[U114] JS：JSON 深比较
来源：http://wwa.meibo888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://kbm.jiagoushi.top

[U115] JS：生成 UUID
来源：http://dek.birdmap.top

crypto.randomUUID()
来源：http://bik.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://jnc.jinghuilouyu.cn

/** @param {string} name */ function f(name) {}
来源：http://jip.fzhhl.top

[U117] JS：单元测试
来源：http://uof.ydzc1.top

npm i -D vitest;  npx vitest
来源：http://wse.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://egx.nanxinkj.top

npm i -D vite;  npx vite
来源：http://afu.0kj1m.cn

[U119] JS：生产构建
来源：http://psp.guowangkeji.top

npx vite build
来源：http://bti.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://wld.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://ppg.gogol.net.cn

================================================================================
来源：http://qbq.tanke756.top

统计汇总
来源：http://fgq.ehwqpu.com

================================================================================
来源：http://pei.tian-w.cn

按语言统计（条）：
来源：http://jpr.zycfv.cn

Python ......... 252
来源：http://mam.tianlin.xyz

PHP ............ 252
来源：http://vci.hysaishi.cn

JavaScript ..... 252
来源：http://lmc.iojbl.cn

TypeScript ..... 212
来源：http://beg.havefunace.top

Java ........... 212
来源：http://veu.sjlbkw.cn

Go ............. 212
来源：http://xuz.yj202588.top

Ruby ........... 212
来源：http://cko.hesvh.cn

C# ............. 212
来源：http://phb.wangdashe.top

C .............. 30
来源：http://htu.tian-w.cn

C++ ............ 30
来源：http://jcf.guowangkeji.top

SQL ............ 90
来源：http://cvn.tian-w.cn

Bash ........... 80
来源：http://cmy.zhijiandao.cn

Kotlin ......... 15
来源：http://acx.gogol.net.cn

Swift .......... 15
来源：http://wtx.chenlongwang.top

Lua ............ 10
来源：http://xdq.andypj.xyz

Perl ........... 10
来源：http://rhq.zhengqikj.top

Scala .......... 10
来源：http://put.epnwcf.com

------------------------------------
来源：http://lnr.0kj1m.cn

合计 ........... 2106 条
来源：http://qmo.guannengcc.top

按章节统计：
来源：http://ofn.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tfx.shanyushiyangkeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://elj.sysykeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://skj.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fmt.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yuw.mhx1999.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hjs.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cod.ydjk.org.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://asw.ivvv.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mtx.sysykeji.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tml.zhoulong.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vzq.shuidangran.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tkm.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hct.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qhv.yj202588.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dpr.yfazqb.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://myq.hongshengwenyu.top

Q SQL 专题                              90
来源：http://buk.vqdsnc.cn

R Bash 专题                             80
来源：http://cnc.xinyue.icu

S C / C++ 专题                          60
来源：http://kkf.zhongyouzk.top

T 其他语言补充                          60
来源：http://nok.shuidangran.top

U 高频实用片段                         120
来源：http://qmn.hcnkem.com

------------------------------------
来源：http://roe.kuanghao11.cn

合计                                  2106 条
来源：http://ymu.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://zqq.iojbl.cn

使用提醒
来源：http://spa.fktsv.cn

--------------------------------------------------------------------------------
来源：http://ocq.ydjk.org.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vlg.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ctl.aibaodan.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qxc.zhijiandao.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://atc.9152youxi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://slo.c1oappe.top

—— 文件结束 ——
来源：http://jfi.ctjpmb.com

================================================================================
来源：http://tac.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://huh.yj20258.top

Common Programming Examples Cheat Book
来源：http://jle.yj20258888.top

================================================================================
来源：http://fuj.hongshengwenyu.top

【收录内容】
来源：http://nfz.dianchejie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nze.zhijiandao.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ccs.ydzc1.top

SQL · Bash · C · C++
来源：http://gon.xuetiantiany.cn


<!-- 参考信息 -->