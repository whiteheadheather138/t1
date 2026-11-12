代发 wailian999

[U03] Py：加载 .env 配置
来源：http://dmc.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vow.iojbl.cn

[U04] Py：变量调试打印
来源：http://onc.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wfe.gzhubu.top

[U05] Py：列表去重且保序
来源：http://zyi.xylfe.cn

list(dict.fromkeys(arr))
来源：http://bxh.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://aiv.fanxiaobao.xyz

{**a, **b}
来源：http://gke.haohaochexian.top

[U07] Py：反转字典键值
来源：http://ull.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://ksx.dianchejie.cn

[U08] Py：展平二维列表
来源：http://uvt.tarul.cn

[y for x in nested for y in x]
来源：http://xcp.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://fex.cucudq.cn

max(d, key=d.get)
来源：http://rwr.vehdjk.com

[U10] Py：按值排序字典
来源：http://rom.ywan-chungtsiang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oaa.fktsv.cn

[U11] Py：生成器表达式
来源：http://ecc.yj20258.top

(x * 2 for x in arr)
来源：http://wko.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://myz.xziqi.cn

Counter(arr).most_common(3)
来源：http://plm.aibaodan.cn

[U13] Py：固定长度队列
来源：http://squ.tanke756.top

deque(maxlen=10)
来源：http://owv.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://mzt.jqgfzy.top

defaultdict(list)
来源：http://fvw.hesvh.cn

[U15] Py：高精度计时
来源：http://kpv.dashuyun.cn

t = time.perf_counter()
来源：http://ntp.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://mwo.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kmc.zhoulong.xyz

[U17] Py：初始化日志
来源：http://pte.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://fto.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://mrg.zycfv.cn

pat = re.compile(r"\d+")
来源：http://lhk.shuidangran.top

[U19] Py：正则替换带回调
来源：http://zvn.9152youxi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iel.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://ury.nanxinkj.top

@functools.lru_cache(maxsize=None)
来源：http://cjv.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://tjt.yfazqb.com

@contextlib.contextmanager
来源：http://kbi.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://bsl.sufxvd.cn

list(zip(*m))
来源：http://imn.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://jyz.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xpw.jlsjyb.cn

[U24] Py：路径操作
来源：http://zsh.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wlf.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://qnc.xuanzx.com

csv.DictReader(f)
来源：http://czn.0kj1m.cn

[U26] Py：并发下载
来源：http://kor.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zbg.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://axc.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://syl.zdqjudy.top

[U28] Py：类型别名
来源：http://ssg.yj20258.top

UserId = int
来源：http://kvu.hnqzz.top

[U29] Py：属性校验
来源：http://nje.nanxuanxn.top

@property 与 @x.setter 配合
来源：http://hdj.jinghuilouyu.cn

[U30] Py：数据类
来源：http://lle.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://zer.cdnleiting.top

[U31] Py：单测
来源：http://pmm.zdbjq.cn

python -m pytest -q
来源：http://iwa.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://vjw.meibo888.top

ruff format . && ruff check --fix .
来源：http://qbf.yj202588.top

[U33] Py：打包发布
来源：http://prc.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://cxm.yj20258888.top

[U34] Py：判断编码
来源：http://kmu.cdnleiting.top

chardet.detect(raw)
来源：http://jmm.xuanzx.com

[U35] Py：发送邮件
来源：http://ili.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uxc.tarul.cn

[U36] Py：定时任务
来源：http://dup.sweek.top

schedule.every(10).minutes.do(job)
来源：http://baa.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://vec.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://jrr.316326.xyz

[U38] Py：获取脚本所在目录
来源：http://mog.iojbl.cn

Path(__file__).resolve().parent
来源：http://dvk.aibaodan.cn

[U39] Py：判断是否在交互环境
来源：http://iue.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://tfm.uphjek.com

[U40] Py：打印到标准错误
来源：http://mdj.hysaishi.cn

print("err", file=sys.stderr)
来源：http://rez.hywenlv.cn

[U41] PHP：初始化 Composer 项目
来源：http://evi.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wjj.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://avn.hcnkem.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ssj.gzhubu.top

[U43] PHP：声明命名空间
来源：http://dgb.snrcjt.cn

namespace App\Http;
来源：http://mqe.bbcook.cn

[U44] PHP：开启严格类型
来源：http://jmv.vqdsnc.cn

declare(strict_types=1);
来源：http://ifs.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://xta.xylfe.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dyb.ehwqpu.com

[U46] PHP：可空类型
来源：http://fij.hfpthk.cn

?string $name = null
来源：http://mgw.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://zbs.dashuyun.cn

int|string $id
来源：http://amk.yongpay.top

[U48] PHP：纯枚举
来源：http://xgv.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://meh.sxryk.cn

[U49] PHP：只读属性
来源：http://dmm.bbcook.cn

public readonly string $name
来源：http://vrk.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://aow.jianghu66.top

public function __construct(private int $id) {}
来源：http://vio.jiagoushi.top

[U51] PHP：数组解构
来源：http://yfq.hcnkem.com

[$a, $b] = $arr;
来源：http://dny.chenzaomai.com

[U52] PHP：箭头函数
来源：http://val.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://gpl.haohaochexian.top

[U53] PHP：空合并运算符
来源：http://brd.bbcook.cn

$v = $a ?? $b ?? "default";
来源：http://qam.mhx1999.top

[U54] PHP：空安全调用
来源：http://nfd.yj20258.top

$obj?->method()
来源：http://qbl.shanyushiyangkeji.top

[U55] PHP：match 表达式
来源：http://lvg.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://efe.zdbjq.cn

[U56] PHP：命名参数
来源：http://wrg.yuxming.cn

f(a: 1, b: 2)
来源：http://stw.yj20258.top

[U57] PHP：字符串插值
来源：http://jpt.nanxuanxn.top

"值: {$a}"
来源：http://rax.hywenlv.cn

[U58] PHP：数组三件套
来源：http://bkb.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yfj.fktsv.cn

[U59] PHP：自定义排序
来源：http://jnl.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://acg.zhijiandao.cn

[U60] PHP：JSON 编解码
来源：http://oxq.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://whr.yueranfly.top

[U61] PHP：正则
来源：http://bsb.ybcxt.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yez.zhijiandao.cn

[U62] PHP：日期对象
来源：http://gjw.gotoacloud.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ssm.cdnleiting.top

[U63] PHP：文件读写
来源：http://lwm.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mdr.hysaishi.cn

[U64] PHP：目录遍历
来源：http://peb.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://slb.bjfxy.top

[U65] PHP：会话
来源：http://stb.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jwy.hammf.cn

[U66] PHP：设置 Cookie
来源：http://nsw.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nmf.zycfv.cn

[U67] PHP：处理文件上传
来源：http://axx.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://giu.vehdjk.com

[U68] PHP：PDO 连接
来源：http://unr.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iip.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://vwt.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ilb.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://ofa.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fxw.hongshengwenyu.top

[U71] PHP：抛出异常
来源：http://bxu.shanyushiyangtech.top

throw new RuntimeException("失败", 500);
来源：http://eco.hammf.cn

[U72] PHP：写错误日志
来源：http://fub.gaohongyu789.top

error_log("失败: " . $e->getMessage());
来源：http://hxt.guannengcc.top

[U73] PHP：读取 ini 配置
来源：http://mrj.nanxinkj.top

parse_ini_file("config.ini", true)
来源：http://efd.vehdjk.com

[U74] PHP：读取环境变量
来源：http://uxq.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://vcs.xinyue.icu

[U75] PHP：依赖注入
来源：http://xuj.havefunace.top

composer require psr/container
来源：http://rvl.fzhhl.top

[U76] PHP：简单路由
来源：http://vii.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wfq.sjlbkw.cn

[U77] PHP：模板渲染
来源：http://nan.yfazqb.com

composer require twig/twig
来源：http://xzd.chenlongwang.top

[U78] PHP：单元测试
来源：http://kwp.sysykeji.top

composer require --dev phpunit/phpunit
来源：http://dsg.chenlongwang.top

[U79] PHP：静态分析
来源：http://blg.jianghu66.top

composer require --dev phpstan/phpstan
来源：http://dhi.c1oappe.top

[U80] PHP：代码规范修复
来源：http://osu.fehbvm.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://uqm.bjfxy.top

[U81] JS：初始化项目
来源：http://qdp.shuidangran.top

npm init -y;  npm i express
来源：http://wrg.xinyue.icu

[U82] JS：package.json 脚本
来源：http://dar.tanke756.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vql.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://fqi.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://frf.birdmap.top

[U84] JS：CommonJS 写法
来源：http://ilt.nwbrower.top

module.exports = { a };  const { a } = require("./m");
来源：http://fad.ehwqpu.com

[U85] JS：可选链
来源：http://vki.smart0.xyz

a?.b?.c
来源：http://aol.jqgfzy.top

[U86] JS：空值合并
来源：http://uhi.yfazqb.com

a ?? b
来源：http://cqq.nanxinkj.top

[U87] JS：解构默认值
来源：http://rsc.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://irm.ybcxt.top

[U88] JS：对象展开合并
来源：http://fzn.tarul.cn

{ ...a, ...b }
来源：http://wqk.birdmap.top

[U89] JS：数组去重
来源：http://eoq.jlsjyb.cn

[...new Set(arr)]
来源：http://hyr.52xcode.cn

[U90] JS：数字数组排序
来源：http://trx.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://ghk.xuanzx.com

[U91] JS：对象键值遍历
来源：http://ept.ctjpmb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://efj.shuidangran.top

[U92] JS：深拷贝
来源：http://riv.dianchejie.cn

structuredClone(obj)
来源：http://zfm.yj20258.top

[U93] JS：模板字符串
来源：http://jht.fengsongda.top

`共 ${n} 条`
来源：http://nwl.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://bvk.mhx1999.top

const double = x => x * 2;
来源：http://nzp.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://lwg.jianghu66.top

new Promise((resolve, reject) => {})
来源：http://vxc.yvedp.cn

[U96] JS：async/await 与异常
来源：http://uhe.jiagoushi.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://abo.aizwys.cn

[U97] JS：并发请求
来源：http://qls.yuxming.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zcd.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://brf.aibaodan.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://meu.yangfankeji.com

[U99] JS：事件监听
来源：http://fzs.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://lyx.cqqwz.cn

[U100] JS：DOM 查询
来源：http://vga.9152youxi.cn

document.querySelector(".item")
来源：http://cul.dianchejie.cn

[U101] JS：classList 操作
来源：http://zxi.gogol.net.cn

el.classList.toggle("active")
来源：http://adc.cheryme.top

[U102] JS：本地存储
来源：http://xgz.zdbjq.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gaj.epnwcf.com

[U103] JS：定时器
来源：http://ftg.yangfankeji.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ydu.redwolf501.top

[U104] JS：防抖
来源：http://mgu.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eue.kuanghao11.cn

[U105] JS：节流
来源：http://ooj.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://quy.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://gcg.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jai.ybcxt.top

[U107] JS：数字千分位
来源：http://fni.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pst.yj20258.top

[U108] JS：随机整数
来源：http://fce.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fmg.guowangkeji.top

[U109] JS：数组分组
来源：http://qlp.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://kly.birdmap.top

[U110] JS：数组分块
来源：http://ypo.epnwcf.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kdy.sufxvd.cn

[U111] JS：对象转 Map
来源：http://loh.9152youxi.cn

new Map(Object.entries(obj))
来源：http://wmi.haohaochexian.top

[U112] JS：字符串补位
来源：http://agb.tianlin.xyz

"7".padStart(3, "0")
来源：http://npo.guannengcc.top

[U113] JS：正则替换全部
来源：http://dcc.sxryk.cn

s.replaceAll("a", "b")
来源：http://jty.c1oappe.top

[U114] JS：JSON 深比较
来源：http://tex.bbcook.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qjc.epnwcf.com

[U115] JS：生成 UUID
来源：http://fcq.hammf.cn

crypto.randomUUID()
来源：http://kjv.jinqigfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://xxf.ydzc1.top

/** @param {string} name */ function f(name) {}
来源：http://wzx.yj20258.top

[U117] JS：单元测试
来源：http://zph.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://nay.chenzaomai.com

[U118] JS：开发服务器
来源：http://mdq.52xcode.cn

npm i -D vite;  npx vite
来源：http://mhp.yanxiufei.cn

[U119] JS：生产构建
来源：http://lim.xziqi.cn

npx vite build
来源：http://amy.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://kzt.mhx1999.top

import.meta.env.VITE_API_URL
来源：http://kpv.hnqzz.top

================================================================================
来源：http://fwx.yvedp.cn

统计汇总
来源：http://shv.hammf.cn

================================================================================
来源：http://zry.xuetiantiany.cn

按语言统计（条）：
来源：http://dau.fanxiaobao.xyz

Python ......... 252
来源：http://bov.hfpthk.cn

PHP ............ 252
来源：http://nep.svipenyu.cn

JavaScript ..... 252
来源：http://any.52xcode.cn

TypeScript ..... 212
来源：http://rzb.pycfn.com

Java ........... 212
来源：http://wtb.shanyushiyangkeji.top

Go ............. 212
来源：http://kht.yuxming.cn

Ruby ........... 212
来源：http://lpv.chenzaomai.com

C# ............. 212
来源：http://bxv.bjfxy.top

C .............. 30
来源：http://esu.uphjek.com

C++ ............ 30
来源：http://abn.fehbvm.com

SQL ............ 90
来源：http://rjg.zhongyouzk.top

Bash ........... 80
来源：http://muc.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://ujn.hesvh.cn

Swift .......... 15
来源：http://huw.yanxiufei.cn

Lua ............ 10
来源：http://hdt.bbcook.cn

Perl ........... 10
来源：http://gaa.fengsongda.top

Scala .......... 10
来源：http://pjp.pengpengdd.cyou

------------------------------------
来源：http://toz.ctjpmb.com

合计 ........... 2106 条
来源：http://omt.xinyue.icu

按章节统计：
来源：http://xcq.zhaomingkeji.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vmz.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hlg.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://csw.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zls.jinyuanbaomall.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ras.shzxlz.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iac.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ncv.yj20258888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xoc.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xtr.shuidangran.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rns.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eej.xylfe.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://djo.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://edh.shuidangran.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gpa.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qze.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tkn.yuxming.cn

Q SQL 专题                              90
来源：http://zgh.andypj.xyz

R Bash 专题                             80
来源：http://cdd.xinyue.icu

S C / C++ 专题                          60
来源：http://rdm.mhx1999.top

T 其他语言补充                          60
来源：http://rxa.chenlongwang.top

U 高频实用片段                         120
来源：http://djp.shanyushiyangkeji.top

------------------------------------
来源：http://yof.bjfxy.top

合计                                  2106 条
来源：http://hqz.aibaodan.cn

--------------------------------------------------------------------------------
来源：http://qyk.sweek.top

使用提醒
来源：http://gss.pycfn.com

--------------------------------------------------------------------------------
来源：http://oyb.hnqzz.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://knt.vehdjk.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://alu.hnqzz.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://icf.zhaomingkeji.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://rbq.smart0.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lve.jiagoushi.top

—— 文件结束 ——
来源：http://coe.shanyushiyangtech.top

================================================================================
来源：http://tsk.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://bjn.daxiang520.top

Common Programming Examples Cheat Book
来源：http://ztn.jinqigfzy.top

================================================================================
来源：http://goh.shangyingyoupin.top

【收录内容】
来源：http://pyl.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://oex.uphjek.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://toi.ydzc1.top

SQL · Bash · C · C++
来源：http://wcp.mhx1999.top


<!-- 参考信息 -->