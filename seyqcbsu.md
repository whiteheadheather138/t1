代发 wailian999

[U03] Py：加载 .env 配置
来源：http://wna.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://npj.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://ztg.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ymy.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://zvu.redwolf501.top

list(dict.fromkeys(arr))
来源：http://sct.jqgfzy.top

[U06] Py：合并两个字典
来源：http://asm.sjlbkw.cn

{**a, **b}
来源：http://mhl.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://mwh.xziqi.cn

{v: k for k, v in d.items()}
来源：http://zsw.snrcjt.cn

[U08] Py：展平二维列表
来源：http://ben.yangfankeji.com

[y for x in nested for y in x]
来源：http://luy.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://mrg.jianghu66.top

max(d, key=d.get)
来源：http://snp.aibaodan.cn

[U10] Py：按值排序字典
来源：http://eif.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rlj.hammf.cn

[U11] Py：生成器表达式
来源：http://yro.zdbjq.cn

(x * 2 for x in arr)
来源：http://yps.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xrj.xziqi.cn

Counter(arr).most_common(3)
来源：http://tnl.yonumen.top

[U13] Py：固定长度队列
来源：http://ipg.nanxuanxn.top

deque(maxlen=10)
来源：http://bvc.bbcook.cn

[U14] Py：分组收集到列表
来源：http://tam.guannengcc.top

defaultdict(list)
来源：http://kvx.316326.xyz

[U15] Py：高精度计时
来源：http://yyb.jlsjyb.cn

t = time.perf_counter()
来源：http://kfm.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://jli.pycfn.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blk.hysaishi.cn

[U17] Py：初始化日志
来源：http://uid.guannengcc.top

logging.basicConfig(level=logging.INFO)
来源：http://hcc.hesvh.cn

[U18] Py：预编译正则
来源：http://mgg.xinyue.icu

pat = re.compile(r"\d+")
来源：http://yah.hcnkem.com

[U19] Py：正则替换带回调
来源：http://vfp.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dgi.chenzaomai.com

[U20] Py：缓存函数结果
来源：http://uej.yonumen.top

@functools.lru_cache(maxsize=None)
来源：http://epm.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://mjw.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://ibi.guannengcc.top

[U22] Py：矩阵转置
来源：http://wia.dianchejie.cn

list(zip(*m))
来源：http://muy.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://dez.zhengqikj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ynj.nwbrower.top

[U24] Py：路径操作
来源：http://bpm.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aha.andypj.xyz

[U25] Py：CSV 按字典读
来源：http://isu.tianlin.xyz

csv.DictReader(f)
来源：http://itx.kuanghao11.cn

[U26] Py：并发下载
来源：http://rpg.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hhc.zhaomingkeji.xyz

[U27] Py：异步 HTTP
来源：http://ggh.hesvh.cn

aiohttp.ClientSession() 配合 async with
来源：http://dme.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://lox.sysykeji.top

UserId = int
来源：http://wxl.aibaodan.cn

[U29] Py：属性校验
来源：http://zta.redwolf501.top

@property 与 @x.setter 配合
来源：http://qms.ppjwa.cn

[U30] Py：数据类
来源：http://rmh.chenzaomai.com

@dataclass(slots=True)
来源：http://dvm.9152youxi.cn

[U31] Py：单测
来源：http://eal.jqgufenzy.top

python -m pytest -q
来源：http://tgo.ctjpmb.com

[U32] Py：代码格式化
来源：http://jkz.iojbl.cn

ruff format . && ruff check --fix .
来源：http://jxw.quarkkingdee.top

[U33] Py：打包发布
来源：http://eyz.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://emw.aizwys.cn

[U34] Py：判断编码
来源：http://zxx.fehbvm.com

chardet.detect(raw)
来源：http://gso.c1oappe.top

[U35] Py：发送邮件
来源：http://iir.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cpd.redwolf501.top

[U36] Py：定时任务
来源：http://fxk.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://wft.sweek.top

[U37] Py：读写 Excel
来源：http://yyj.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://eua.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://kws.meibo888.top

Path(__file__).resolve().parent
来源：http://sou.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://xvb.xinyue.icu

sys.stdout.isatty()
来源：http://xer.hnqzz.top

[U40] Py：打印到标准错误
来源：http://ssb.yuanzhike.top

print("err", file=sys.stderr)
来源：http://fun.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://pti.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://iit.jiagoushi.top

[U42] PHP：PSR-4 自动加载
来源：http://dnd.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oft.hfpthk.cn

[U43] PHP：声明命名空间
来源：http://iga.xinyue.icu

namespace App\Http;
来源：http://dma.andypj.xyz

[U44] PHP：开启严格类型
来源：http://qbh.xziqi.cn

declare(strict_types=1);
来源：http://mrq.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://qwm.vehdjk.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://bvt.chenzaomai.com

[U46] PHP：可空类型
来源：http://diu.ppjwa.cn

?string $name = null
来源：http://spp.dianchejie.cn

[U47] PHP：联合类型
来源：http://bkl.dianchejie.cn

int|string $id
来源：http://vqy.bjfxy.top

[U48] PHP：纯枚举
来源：http://ahq.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rcc.ydzc1.top

[U49] PHP：只读属性
来源：http://ubi.zhijiandao.cn

public readonly string $name
来源：http://bou.sweek.top

[U50] PHP：构造器属性提升
来源：http://iva.gogol.net.cn

public function __construct(private int $id) {}
来源：http://fjm.tianlin.xyz

[U51] PHP：数组解构
来源：http://jtp.yueranfly.top

[$a, $b] = $arr;
来源：http://aok.shzxlz.cn

[U52] PHP：箭头函数
来源：http://bxb.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://awr.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://exa.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://ceg.jianghu66.top

[U54] PHP：空安全调用
来源：http://bsa.gogol.net.cn

$obj?->method()
来源：http://abj.gzhubu.top

[U55] PHP：match 表达式
来源：http://dsa.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://leu.daxiang520.top

[U56] PHP：命名参数
来源：http://xqf.ydzc1.top

f(a: 1, b: 2)
来源：http://ygp.aibaodan.cn

[U57] PHP：字符串插值
来源：http://arg.shzxlz.cn

"值: {$a}"
来源：http://umb.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://zju.gaohongyu789.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ohl.yuanzhike.top

[U59] PHP：自定义排序
来源：http://rjn.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://odj.yj202588.top

[U60] PHP：JSON 编解码
来源：http://dwf.zhiwuduotai.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sja.sufxvd.cn

[U61] PHP：正则
来源：http://eaa.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ced.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://iql.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jaj.jyoumei.cn

[U63] PHP：文件读写
来源：http://dql.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xan.316326.xyz

[U64] PHP：目录遍历
来源：http://nch.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ick.bjfxy.top

[U65] PHP：会话
来源：http://gir.zhongyouzk.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kgu.zhaomingkeji.xyz

[U66] PHP：设置 Cookie
来源：http://req.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hla.jqgufenzy.top

[U67] PHP：处理文件上传
来源：http://piy.ydzc1.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cdt.ydzc1.top

[U68] PHP：PDO 连接
来源：http://jqb.0kj1m.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yfm.gzhubu.top

[U69] PHP：PDO 预处理
来源：http://ujm.meibo888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bkx.hammf.cn

[U70] PHP：PDO 事务
来源：http://vas.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bkn.guannengcc.top

[U71] PHP：抛出异常
来源：http://tpg.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://uux.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://blh.chenzaomai.com

error_log("失败: " . $e->getMessage());
来源：http://wni.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://mji.316326.xyz

parse_ini_file("config.ini", true)
来源：http://ptt.xylfe.cn

[U74] PHP：读取环境变量
来源：http://nhj.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://apl.uphjek.com

[U75] PHP：依赖注入
来源：http://wix.yuanzhike.top

composer require psr/container
来源：http://hvg.fktsv.cn

[U76] PHP：简单路由
来源：http://jtt.fzhhl.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://auk.chenzaomai.com

[U77] PHP：模板渲染
来源：http://owq.guannengcc.top

composer require twig/twig
来源：http://mow.zdbjq.cn

[U78] PHP：单元测试
来源：http://iss.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://tws.jinqigufen.top

[U79] PHP：静态分析
来源：http://dnv.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://cny.tian-w.cn

[U80] PHP：代码规范修复
来源：http://fzu.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zum.jiagoushi.top

[U81] JS：初始化项目
来源：http://afm.ydjk.org.cn

npm init -y;  npm i express
来源：http://pjr.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://mym.yj20258.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eqm.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://cza.jinqigfzy.top

export const a = 1;  import { a } from "./m.js";
来源：http://ffp.vqdsnc.cn

[U84] JS：CommonJS 写法
来源：http://zte.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://lhe.daria6918.cn

[U85] JS：可选链
来源：http://xxz.xylfe.cn

a?.b?.c
来源：http://pfe.guannengcc.top

[U86] JS：空值合并
来源：http://jbg.hnqzz.top

a ?? b
来源：http://uon.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://udk.guannengcc.top

const { a = 1, b = 2 } = obj;
来源：http://jxd.yj20258.top

[U88] JS：对象展开合并
来源：http://quq.yj20258.top

{ ...a, ...b }
来源：http://fvd.guowangkeji.top

[U89] JS：数组去重
来源：http://pgd.jiagoushi.top

[...new Set(arr)]
来源：http://ibg.zdbjq.cn

[U90] JS：数字数组排序
来源：http://kmc.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://edu.uphjek.com

[U91] JS：对象键值遍历
来源：http://eem.tian-w.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tgh.aibaodan.cn

[U92] JS：深拷贝
来源：http://txm.guowangkeji.top

structuredClone(obj)
来源：http://yxw.hfpthk.cn

[U93] JS：模板字符串
来源：http://anf.quarkkingdee.top

`共 ${n} 条`
来源：http://bom.andypj.xyz

[U94] JS：箭头函数
来源：http://dap.ydzc1.top

const double = x => x * 2;
来源：http://uwh.haohaochexian.top

[U95] JS：Promise 包装
来源：http://axp.pengpengdd.cyou

new Promise((resolve, reject) => {})
来源：http://qcj.yueranfly.top

[U96] JS：async/await 与异常
来源：http://ypd.sjlbkw.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fck.nanxinkj.top

[U97] JS：并发请求
来源：http://sie.ppjwa.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://etk.svipenyu.cn

[U98] JS：fetch 带 JSON
来源：http://ubg.haohaochexian.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rcp.ywan-chungtsiang.top

[U99] JS：事件监听
来源：http://wnx.feifeiyinyue.top

el.addEventListener("click", e => {})
来源：http://end.hesvh.cn

[U100] JS：DOM 查询
来源：http://rbz.0kj1m.cn

document.querySelector(".item")
来源：http://lau.guowangkeji.top

[U101] JS：classList 操作
来源：http://qfz.daria6918.cn

el.classList.toggle("active")
来源：http://xzu.316326.xyz

[U102] JS：本地存储
来源：http://qdz.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ysf.zdbjq.cn

[U103] JS：定时器
来源：http://zkl.gotoacloud.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dww.yongpay.top

[U104] JS：防抖
来源：http://lxa.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xfp.epnwcf.com

[U105] JS：节流
来源：http://ico.fktsv.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qta.yanxiufei.cn

[U106] JS：日期格式化
来源：http://xiv.ehwqpu.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zhv.shzxlz.cn

[U107] JS：数字千分位
来源：http://oyw.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fln.yongpay.top

[U108] JS：随机整数
来源：http://qxq.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://avz.yuanzhike.top

[U109] JS：数组分组
来源：http://rqi.chenzaomai.com

Object.groupBy(arr, x => x.type)
来源：http://rez.epnwcf.com

[U110] JS：数组分块
来源：http://qte.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pdo.xylfe.cn

[U111] JS：对象转 Map
来源：http://wdo.epnwcf.com

new Map(Object.entries(obj))
来源：http://nkm.hfpthk.cn

[U112] JS：字符串补位
来源：http://azk.hnqzz.top

"7".padStart(3, "0")
来源：http://hvy.guannengcc.top

[U113] JS：正则替换全部
来源：http://tvb.vehdjk.com

s.replaceAll("a", "b")
来源：http://wgz.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://sgb.birdmap.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hzs.fanxiaobao.xyz

[U115] JS：生成 UUID
来源：http://syy.fengsongda.top

crypto.randomUUID()
来源：http://fso.jlsjyb.cn

[U116] JS：类型检查（JSDoc）
来源：http://mwl.daxiang520.top

/** @param {string} name */ function f(name) {}
来源：http://amn.fzhhl.top

[U117] JS：单元测试
来源：http://gal.xziqi.cn

npm i -D vitest;  npx vitest
来源：http://unv.jinyuanbaomall.cn

[U118] JS：开发服务器
来源：http://dhy.iojbl.cn

npm i -D vite;  npx vite
来源：http://oqq.hammf.cn

[U119] JS：生产构建
来源：http://qsz.tian-w.cn

npx vite build
来源：http://ueo.svipenyu.cn

[U120] JS：读取环境变量（Vite）
来源：http://ysv.hfpthk.cn

import.meta.env.VITE_API_URL
来源：http://bct.andypj.xyz

================================================================================
来源：http://uea.aizwys.cn

统计汇总
来源：http://mil.shuidangran.top

================================================================================
来源：http://bso.hnxiangtu.top

按语言统计（条）：
来源：http://uig.gogol.net.cn

Python ......... 252
来源：http://jmd.nwbrower.top

PHP ............ 252
来源：http://qvq.meibo888.top

JavaScript ..... 252
来源：http://xnu.yuanzhike.top

TypeScript ..... 212
来源：http://nfo.jqgufenzy.top

Java ........... 212
来源：http://skg.9152youxi.cn

Go ............. 212
来源：http://ogv.316326.xyz

Ruby ........... 212
来源：http://byg.zdbjq.cn

C# ............. 212
来源：http://pch.bbcook.cn

C .............. 30
来源：http://rgj.jqgfzy.top

C++ ............ 30
来源：http://imi.hywenlv.cn

SQL ............ 90
来源：http://nkd.ywan-chungtsiang.top

Bash ........... 80
来源：http://eko.havefunace.top

Kotlin ......... 15
来源：http://fqc.ppjwa.cn

Swift .......... 15
来源：http://rkc.jianghu66.top

Lua ............ 10
来源：http://gvw.ctjpmb.com

Perl ........... 10
来源：http://dlc.zhiwuduotai.top

Scala .......... 10
来源：http://nua.tianlin.xyz

------------------------------------
来源：http://pvb.zdbjq.cn

合计 ........... 2106 条
来源：http://dsb.zhijiandao.cn

按章节统计：
来源：http://tuq.9152youxi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://exv.xinyue.icu

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lbz.daria6918.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cxt.uphjek.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pkz.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://swk.zdbjq.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zxx.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zce.yueranfly.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qmy.sweek.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://awc.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zar.yuanzhike.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nbk.yangfankeji.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yxy.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ngm.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kqp.havefunace.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ghj.yueranfly.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hff.xziqi.cn

Q SQL 专题                              90
来源：http://shx.wangshuangyany.cn

R Bash 专题                             80
来源：http://vjv.hammf.cn

S C / C++ 专题                          60
来源：http://urv.chenzaomai.com

T 其他语言补充                          60
来源：http://klj.ydjk.org.cn

U 高频实用片段                         120
来源：http://zbk.svipenyu.cn

------------------------------------
来源：http://twv.jinqigfzy.top

合计                                  2106 条
来源：http://gwm.nwbrower.top

--------------------------------------------------------------------------------
来源：http://yty.birdmap.top

使用提醒
来源：http://raq.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://flr.shanyushiyangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zig.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pxt.zdqjudy.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cpf.yj20258.top

在旧版本上使用前请先确认语法支持情况。
来源：http://txz.shanyushiyangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://csy.fanxiaobao.xyz

—— 文件结束 ——
来源：http://bup.xinyue.icu

================================================================================
来源：http://qrd.guannengcc.top

程序语言常见例子速查手册（2024 版）
来源：http://cnd.c1oappe.top

Common Programming Examples Cheat Book
来源：http://srn.hnxiangtu.top

================================================================================
来源：http://orl.ehwqpu.com

【收录内容】
来源：http://mbt.kuanghao11.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qzu.sxryk.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gbq.zhongyouzk.top

SQL · Bash · C · C++
来源：http://ixi.yvedp.cn


<!-- 参考信息 -->