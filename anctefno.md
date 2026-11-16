代发 wailian999

[U01] Py：创建虚拟环境
来源：http://qjb.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eip.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://nvb.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://apm.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://cpw.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jow.pycfn.com

[U04] Py：变量调试打印
来源：http://cwh.zhijiandao.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hoz.bjfxy.top

[U05] Py：列表去重且保序
来源：http://bre.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://tfn.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://kpu.cqqwz.cn

{**a, **b}
来源：http://zpg.iojbl.cn

[U07] Py：反转字典键值
来源：http://ofy.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://gaz.sufxvd.cn

[U08] Py：展平二维列表
来源：http://azv.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://wbu.hnxiangtu.top

[U09] Py：字典取最大值的键
来源：http://odp.jianghu66.top

max(d, key=d.get)
来源：http://plk.fehbvm.com

[U10] Py：按值排序字典
来源：http://baa.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yyb.smart0.xyz

[U11] Py：生成器表达式
来源：http://xeq.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://bkh.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xmz.fengsongda.top

Counter(arr).most_common(3)
来源：http://xel.gzhubu.top

[U13] Py：固定长度队列
来源：http://dwm.yuxming.cn

deque(maxlen=10)
来源：http://wzg.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://dch.zhengqikj.top

defaultdict(list)
来源：http://ocf.dashuyun.cn

[U15] Py：高精度计时
来源：http://dsu.fzhhl.top

t = time.perf_counter()
来源：http://jie.zhijiandao.cn

[U16] Py：命令行参数解析
来源：http://nol.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rgl.hnqzz.top

[U17] Py：初始化日志
来源：http://umc.chenjidiqi.icu

logging.basicConfig(level=logging.INFO)
来源：http://vdn.hfpthk.cn

[U18] Py：预编译正则
来源：http://yqp.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://hgp.sweek.top

[U19] Py：正则替换带回调
来源：http://rql.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lls.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://kbl.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://xch.jinyuanbaomall.cn

[U21] Py：自定义上下文管理器
来源：http://kbl.sjlbkw.cn

@contextlib.contextmanager
来源：http://qqt.tanke756.top

[U22] Py：矩阵转置
来源：http://qty.cashguo.top

list(zip(*m))
来源：http://ayc.birdmap.top

[U23] Py：分块读取大文件
来源：http://ivg.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wxj.aibaodan.cn

[U24] Py：路径操作
来源：http://zdd.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fip.meibo888.top

[U25] Py：CSV 按字典读
来源：http://opz.zhijiandao.cn

csv.DictReader(f)
来源：http://lwp.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://iau.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ozu.uphjek.com

[U27] Py：异步 HTTP
来源：http://tto.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://jgi.sxryk.cn

[U28] Py：类型别名
来源：http://qvq.iojbl.cn

UserId = int
来源：http://uuh.hongshengwenyu.top

[U29] Py：属性校验
来源：http://cox.gzhubu.top

@property 与 @x.setter 配合
来源：http://mbp.yuanzhike.top

[U30] Py：数据类
来源：http://wyx.hysaishi.cn

@dataclass(slots=True)
来源：http://bzl.gzhubu.top

[U31] Py：单测
来源：http://ixh.yanxiufei.cn

python -m pytest -q
来源：http://icp.sweek.top

[U32] Py：代码格式化
来源：http://lwi.yvedp.cn

ruff format . && ruff check --fix .
来源：http://anr.shangyingyoupin.top

[U33] Py：打包发布
来源：http://dzm.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://gkz.316326.xyz

[U34] Py：判断编码
来源：http://brr.zhixingplan.top

chardet.detect(raw)
来源：http://bos.yanxiufei.cn

[U35] Py：发送邮件
来源：http://ttr.ydjk.org.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kxn.ydjk.org.cn

[U36] Py：定时任务
来源：http://ibb.52xcode.cn

schedule.every(10).minutes.do(job)
来源：http://msg.gzhubu.top

[U37] Py：读写 Excel
来源：http://adh.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nrv.52xcode.cn

[U38] Py：获取脚本所在目录
来源：http://nks.yonumen.top

Path(__file__).resolve().parent
来源：http://rkh.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://msi.smart0.xyz

sys.stdout.isatty()
来源：http://dkd.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://qaq.tianlin.xyz

print("err", file=sys.stderr)
来源：http://yac.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://qjp.zhijiandao.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xye.zhijiandao.cn

[U42] PHP：PSR-4 自动加载
来源：http://ltw.fengsongda.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://soq.wangshuangyany.cn

[U43] PHP：声明命名空间
来源：http://yse.havefunace.top

namespace App\Http;
来源：http://doc.redwolf501.top

[U44] PHP：开启严格类型
来源：http://bpw.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://eko.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://lzx.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://gna.mhx1999.top

[U46] PHP：可空类型
来源：http://jco.xingfuxueyuan.xyz

?string $name = null
来源：http://mkv.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://clk.hcnkem.com

int|string $id
来源：http://ita.jiagoushi.top

[U48] PHP：纯枚举
来源：http://igs.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hjy.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://zuw.bjfxy.top

public readonly string $name
来源：http://tzi.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://npb.yueranfly.top

public function __construct(private int $id) {}
来源：http://bwu.nanxinkj.top

[U51] PHP：数组解构
来源：http://fom.jiagoushi.top

[$a, $b] = $arr;
来源：http://mht.haohaochexian.top

[U52] PHP：箭头函数
来源：http://hqm.zhoulong.xyz

$double = fn($x) => $x * 2;
来源：http://lgf.fengsongda.top

[U53] PHP：空合并运算符
来源：http://ygi.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://zsd.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://aeo.xinyue.icu

$obj?->method()
来源：http://oko.svipenyu.cn

[U55] PHP：match 表达式
来源：http://txh.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ckl.yangfankeji.com

[U56] PHP：命名参数
来源：http://iik.iojbl.cn

f(a: 1, b: 2)
来源：http://zfs.ydjk.org.cn

[U57] PHP：字符串插值
来源：http://cwb.sweek.top

"值: {$a}"
来源：http://wns.ctjpmb.com

[U58] PHP：数组三件套
来源：http://jov.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wek.yonumen.top

[U59] PHP：自定义排序
来源：http://wjf.fktsv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ntg.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://gbq.fanxiaobao.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rra.vqdsnc.cn

[U61] PHP：正则
来源：http://iop.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://opv.hnxiangtu.top

[U62] PHP：日期对象
来源：http://svv.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fii.shzxlz.cn

[U63] PHP：文件读写
来源：http://kkf.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hxd.sysykeji.top

[U64] PHP：目录遍历
来源：http://gqw.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://xrk.fengsongda.top

[U65] PHP：会话
来源：http://bui.guowangkeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bdf.tanke756.top

[U66] PHP：设置 Cookie
来源：http://xxg.c1oappe.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ldc.fktsv.cn

[U67] PHP：处理文件上传
来源：http://iuq.hfpthk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://htt.zhongyouzk.top

[U68] PHP：PDO 连接
来源：http://itt.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gfc.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://ged.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ipe.sufxvd.cn

[U70] PHP：PDO 事务
来源：http://mhd.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://niz.redwolf501.top

[U71] PHP：抛出异常
来源：http://etl.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://wvj.zdbjq.cn

[U72] PHP：写错误日志
来源：http://qgj.ybcxt.top

error_log("失败: " . $e->getMessage());
来源：http://duy.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://xtf.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://guh.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://its.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://juc.tianlin.xyz

[U75] PHP：依赖注入
来源：http://kvt.tarul.cn

composer require psr/container
来源：http://bue.redwolf501.top

[U76] PHP：简单路由
来源：http://oud.wangdashe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qtv.svipenyu.cn

[U77] PHP：模板渲染
来源：http://mls.nanxuanxn.top

composer require twig/twig
来源：http://ylf.birdmap.top

[U78] PHP：单元测试
来源：http://hbq.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://bri.jlsjyb.cn

[U79] PHP：静态分析
来源：http://tzx.jlsjyb.cn

composer require --dev phpstan/phpstan
来源：http://hro.wangdashe.top

[U80] PHP：代码规范修复
来源：http://njs.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://xvj.gzhubu.top

[U81] JS：初始化项目
来源：http://jra.yueranfly.top

npm init -y;  npm i express
来源：http://fku.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://snb.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ooe.yongpay.top

[U83] JS：ES Module 导入导出
来源：http://geh.cdnleiting.top

export const a = 1;  import { a } from "./m.js";
来源：http://uza.aizwys.cn

[U84] JS：CommonJS 写法
来源：http://hze.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://azf.cdnleiting.top

[U85] JS：可选链
来源：http://puy.xuanzx.com

a?.b?.c
来源：http://fwp.xuanzx.com

[U86] JS：空值合并
来源：http://kxq.ydzc1.top

a ?? b
来源：http://par.yonumen.top

[U87] JS：解构默认值
来源：http://yma.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://srq.nanxinkj.top

[U88] JS：对象展开合并
来源：http://zpo.shanyushiyangtech.top

{ ...a, ...b }
来源：http://are.tianlin.xyz

[U89] JS：数组去重
来源：http://zoo.xylfe.cn

[...new Set(arr)]
来源：http://qib.zdqjudy.top

[U90] JS：数字数组排序
来源：http://kvm.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://osa.yfazqb.com

[U91] JS：对象键值遍历
来源：http://vkj.aibaodan.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://izm.yj202588.top

[U92] JS：深拷贝
来源：http://wth.snrcjt.cn

structuredClone(obj)
来源：http://eml.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://ngr.shanyushiyangkeji.top

`共 ${n} 条`
来源：http://ila.tarul.cn

[U94] JS：箭头函数
来源：http://djd.uphjek.com

const double = x => x * 2;
来源：http://vct.yfazqb.com

[U95] JS：Promise 包装
来源：http://bxh.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://pke.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://pvh.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wel.ybcxt.top

[U97] JS：并发请求
来源：http://jjt.zhengqikj.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://oes.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://yxl.yj20258888.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zsc.hnqzz.top

[U99] JS：事件监听
来源：http://dsd.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://omg.yongpay.top

[U100] JS：DOM 查询
来源：http://kls.zhongyouzk.top

document.querySelector(".item")
来源：http://cki.yuanzhike.top

[U101] JS：classList 操作
来源：http://ngi.tian-w.cn

el.classList.toggle("active")
来源：http://rho.316326.xyz

[U102] JS：本地存储
来源：http://yhi.sysykeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jee.fehbvm.com

[U103] JS：定时器
来源：http://vwf.gogol.net.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fuw.ctjpmb.com

[U104] JS：防抖
来源：http://uuv.yfazqb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dde.yuanzhike.top

[U105] JS：节流
来源：http://wnm.svipenyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://txi.ywan-chungtsiang.top

[U106] JS：日期格式化
来源：http://asc.aizwys.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hol.hnxiangtu.top

[U107] JS：数字千分位
来源：http://xkx.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ulr.wangshuangyany.cn

[U108] JS：随机整数
来源：http://tej.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vxy.tanke756.top

[U109] JS：数组分组
来源：http://mok.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://yyj.fktsv.cn

[U110] JS：数组分块
来源：http://bbp.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wbm.ppjwa.cn

[U111] JS：对象转 Map
来源：http://zcg.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://yso.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://amg.xinyue.icu

"7".padStart(3, "0")
来源：http://qiw.shuidangran.top

[U113] JS：正则替换全部
来源：http://odv.sufxvd.cn

s.replaceAll("a", "b")
来源：http://joz.jinyuanbaomall.cn

[U114] JS：JSON 深比较
来源：http://hbo.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://njm.nanxinkj.top

[U115] JS：生成 UUID
来源：http://biy.fengsongda.top

crypto.randomUUID()
来源：http://jxt.wangdashe.top

[U116] JS：类型检查（JSDoc）
来源：http://qqp.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://kke.shuidangran.top

[U117] JS：单元测试
来源：http://zmk.meibo888.top

npm i -D vitest;  npx vitest
来源：http://wmo.tianlin.xyz

[U118] JS：开发服务器
来源：http://xtx.hcnkem.com

npm i -D vite;  npx vite
来源：http://rea.yuanzhike.top

[U119] JS：生产构建
来源：http://bad.hongshengwenyu.top

npx vite build
来源：http://sah.quarkkingdee.top

[U120] JS：读取环境变量（Vite）
来源：http://pvs.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://ayj.daria6918.cn

================================================================================
来源：http://kve.haohaochexian.top

统计汇总
来源：http://xwg.birdmap.top

================================================================================
来源：http://bdx.jyoumei.cn

按语言统计（条）：
来源：http://wam.fzhhl.top

Python ......... 252
来源：http://udx.meibo888.top

PHP ............ 252
来源：http://rwe.yuxming.cn

JavaScript ..... 252
来源：http://lge.ehwqpu.com

TypeScript ..... 212
来源：http://zmw.ppjwa.cn

Java ........... 212
来源：http://zvv.bjfxy.top

Go ............. 212
来源：http://kmp.fanxiaobao.xyz

Ruby ........... 212
来源：http://fab.shangyingyoupin.top

C# ............. 212
来源：http://nwx.jiagoushi.top

C .............. 30
来源：http://aud.daria6918.cn

C++ ............ 30
来源：http://lxa.c1oappe.top

SQL ............ 90
来源：http://pji.zycfv.cn

Bash ........... 80
来源：http://qqy.shzxlz.cn

Kotlin ......... 15
来源：http://tkt.jqgfzy.top

Swift .......... 15
来源：http://wrd.zhixingplan.top

Lua ............ 10
来源：http://usv.tian-w.cn

Perl ........... 10
来源：http://owz.zdbjq.cn

Scala .......... 10
来源：http://jdc.jqgufenzy.top

------------------------------------
来源：http://wsl.316326.xyz

合计 ........... 2106 条
来源：http://qku.jianghu66.top

按章节统计：
来源：http://jvi.chenzaomai.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hid.ppjwa.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nwf.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iyi.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://toy.fehbvm.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hhz.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ddk.sxryk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tws.jlsjyb.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zrv.fzhhl.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lnx.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wpy.ehwqpu.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xyn.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dll.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ejm.pycfn.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://typ.gotoacloud.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zzc.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pum.ybcxt.top

Q SQL 专题                              90
来源：http://bay.xziqi.cn

R Bash 专题                             80
来源：http://rrr.ctjpmb.com

S C / C++ 专题                          60
来源：http://rsx.zhiwuduotai.top

T 其他语言补充                          60
来源：http://lsc.vqdsnc.cn

U 高频实用片段                         120
来源：http://iyk.cqqwz.cn

------------------------------------
来源：http://msm.zdqjudy.top

合计                                  2106 条
来源：http://kcp.andypj.xyz

--------------------------------------------------------------------------------
来源：http://nae.yueranfly.top

使用提醒
来源：http://rqj.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://fns.yonumen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://evk.yuanzhike.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://adk.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kqp.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://alp.bbcook.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dlr.yj202588.top

—— 文件结束 ——
来源：http://dxo.havefunace.top

================================================================================
来源：http://zwf.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://mcb.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://hya.zdqjudy.top

================================================================================
来源：http://yjk.guannengcc.top


<!-- 参考信息 -->