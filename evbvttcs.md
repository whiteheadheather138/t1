代发 wailian999

[U03] Py：加载 .env 配置
来源：http://grb.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dsj.daria6918.cn

[U04] Py：变量调试打印
来源：http://nrq.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://daz.hcnkem.com

[U05] Py：列表去重且保序
来源：http://ghz.hammf.cn

list(dict.fromkeys(arr))
来源：http://cyv.ppjwa.cn

[U06] Py：合并两个字典
来源：http://ajz.havefunace.top

{**a, **b}
来源：http://kmo.svipenyu.cn

[U07] Py：反转字典键值
来源：http://xak.xinyue.icu

{v: k for k, v in d.items()}
来源：http://qut.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://egl.shzxlz.cn

[y for x in nested for y in x]
来源：http://xqv.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://gox.sufxvd.cn

max(d, key=d.get)
来源：http://eoq.fanxiaobao.xyz

[U10] Py：按值排序字典
来源：http://eqh.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pde.zycfv.cn

[U11] Py：生成器表达式
来源：http://lpt.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://box.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://snx.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://fpm.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://fkq.guannengcc.top

deque(maxlen=10)
来源：http://wtp.smart0.xyz

[U14] Py：分组收集到列表
来源：http://ylk.sysykeji.top

defaultdict(list)
来源：http://hxy.jinqigufen.top

[U15] Py：高精度计时
来源：http://lvw.zhongyouzk.top

t = time.perf_counter()
来源：http://eof.havefunace.top

[U16] Py：命令行参数解析
来源：http://bmm.daxiang520.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uuv.zhixingplan.top

[U17] Py：初始化日志
来源：http://gvo.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://ptw.vqdsnc.cn

[U18] Py：预编译正则
来源：http://bgb.yj202588.top

pat = re.compile(r"\d+")
来源：http://irz.gzhubu.top

[U19] Py：正则替换带回调
来源：http://emd.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://acu.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://lsy.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://uxw.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://ypq.haohaochexian.top

@contextlib.contextmanager
来源：http://nvu.guowangkeji.top

[U22] Py：矩阵转置
来源：http://eut.hnxiangtu.top

list(zip(*m))
来源：http://tnk.316326.xyz

[U23] Py：分块读取大文件
来源：http://pss.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wdw.shangyingyoupin.top

[U24] Py：路径操作
来源：http://kfh.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ngd.gzhubu.top

[U25] Py：CSV 按字典读
来源：http://riu.yonumen.top

csv.DictReader(f)
来源：http://lbj.shzxlz.cn

[U26] Py：并发下载
来源：http://ges.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://utd.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://mkt.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://rnj.daxiang520.top

[U28] Py：类型别名
来源：http://mqz.xylfe.cn

UserId = int
来源：http://jbh.sjlbkw.cn

[U29] Py：属性校验
来源：http://kgj.ehwqpu.com

@property 与 @x.setter 配合
来源：http://vwn.daria6918.cn

[U30] Py：数据类
来源：http://fzj.316326.xyz

@dataclass(slots=True)
来源：http://ong.tian-w.cn

[U31] Py：单测
来源：http://vwr.zdbjq.cn

python -m pytest -q
来源：http://inr.hfpthk.cn

[U32] Py：代码格式化
来源：http://uvz.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://gdb.zhongyouzk.top

[U33] Py：打包发布
来源：http://sfa.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://jmq.316326.xyz

[U34] Py：判断编码
来源：http://lkm.yvedp.cn

chardet.detect(raw)
来源：http://jjn.epnwcf.com

[U35] Py：发送邮件
来源：http://eyi.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://meg.jlsjyb.cn

[U36] Py：定时任务
来源：http://onn.chenjidiqi.icu

schedule.every(10).minutes.do(job)
来源：http://zvn.yvedp.cn

[U37] Py：读写 Excel
来源：http://ylv.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://qcp.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://icq.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://zsc.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://gfh.aibaodan.cn

sys.stdout.isatty()
来源：http://aib.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://fur.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://stj.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://tgs.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://zye.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://ktr.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://njk.sweek.top

[U43] PHP：声明命名空间
来源：http://fxa.gzhubu.top

namespace App\Http;
来源：http://hgs.pycfn.com

[U44] PHP：开启严格类型
来源：http://hem.sufxvd.cn

declare(strict_types=1);
来源：http://wvy.shzxlz.cn

[U45] PHP：类型声明与返回类型
来源：http://mob.cqqwz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jhb.svipenyu.cn

[U46] PHP：可空类型
来源：http://dmw.jiagoushi.top

?string $name = null
来源：http://zwf.xziqi.cn

[U47] PHP：联合类型
来源：http://ije.hesvh.cn

int|string $id
来源：http://qli.cucudq.cn

[U48] PHP：纯枚举
来源：http://xjg.daxiang520.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vxl.sweek.top

[U49] PHP：只读属性
来源：http://vqn.zhengqikj.top

public readonly string $name
来源：http://abp.sxryk.cn

[U50] PHP：构造器属性提升
来源：http://wkr.fzhhl.top

public function __construct(private int $id) {}
来源：http://orl.gzhubu.top

[U51] PHP：数组解构
来源：http://rfr.jyoumei.cn

[$a, $b] = $arr;
来源：http://afs.zhixingplan.top

[U52] PHP：箭头函数
来源：http://ufp.jianghu66.top

$double = fn($x) => $x * 2;
来源：http://sgt.xziqi.cn

[U53] PHP：空合并运算符
来源：http://ece.mhx1999.top

$v = $a ?? $b ?? "default";
来源：http://xsx.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://yif.shuidangran.top

$obj?->method()
来源：http://mit.daxiang520.top

[U55] PHP：match 表达式
来源：http://bqk.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://knf.havefunace.top

[U56] PHP：命名参数
来源：http://zny.aibaodan.cn

f(a: 1, b: 2)
来源：http://pef.tianlin.xyz

[U57] PHP：字符串插值
来源：http://vwg.ybcxt.top

"值: {$a}"
来源：http://elc.jiagoushi.top

[U58] PHP：数组三件套
来源：http://kbz.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pwj.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://wgh.wangdashe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hms.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://fxy.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hff.zhoulong.xyz

[U61] PHP：正则
来源：http://fvp.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://izu.cheryme.top

[U62] PHP：日期对象
来源：http://wka.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ajk.daria6918.cn

[U63] PHP：文件读写
来源：http://nbg.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mjj.hammf.cn

[U64] PHP：目录遍历
来源：http://zub.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://ant.havefunace.top

[U65] PHP：会话
来源：http://apf.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ejq.sweek.top

[U66] PHP：设置 Cookie
来源：http://yfx.cqqwz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://edr.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://vko.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pll.nwbrower.top

[U68] PHP：PDO 连接
来源：http://jve.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uho.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://lvd.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gtx.jinghuilouyu.cn

[U70] PHP：PDO 事务
来源：http://xyc.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bwa.jinyuanbaomall.cn

[U71] PHP：抛出异常
来源：http://frf.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://khn.fzhhl.top

[U72] PHP：写错误日志
来源：http://puk.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://rdn.zhixingplan.top

[U73] PHP：读取 ini 配置
来源：http://quw.ehwqpu.com

parse_ini_file("config.ini", true)
来源：http://sow.feifeiyinyue.top

[U74] PHP：读取环境变量
来源：http://phs.andypj.xyz

getenv("APP_ENV") ?: "production"
来源：http://dha.zdbjq.cn

[U75] PHP：依赖注入
来源：http://fjt.yvedp.cn

composer require psr/container
来源：http://wve.xziqi.cn

[U76] PHP：简单路由
来源：http://ivt.iojbl.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ktg.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://cnx.yuxming.cn

composer require twig/twig
来源：http://vqy.ppjwa.cn

[U78] PHP：单元测试
来源：http://tik.ydjk.org.cn

composer require --dev phpunit/phpunit
来源：http://fzr.hywenlv.cn

[U79] PHP：静态分析
来源：http://irx.daria6918.cn

composer require --dev phpstan/phpstan
来源：http://wlm.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://zfx.ywan-chungtsiang.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://nqq.daxiang520.top

[U81] JS：初始化项目
来源：http://wvw.haohaochexian.top

npm init -y;  npm i express
来源：http://zky.hnqzz.top

[U82] JS：package.json 脚本
来源：http://oyh.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ysj.bjfxy.top

[U83] JS：ES Module 导入导出
来源：http://wai.hongshengwenyu.top

export const a = 1;  import { a } from "./m.js";
来源：http://pao.fehbvm.com

[U84] JS：CommonJS 写法
来源：http://hjn.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://kzu.sysykeji.top

[U85] JS：可选链
来源：http://fig.hongshengwenyu.top

a?.b?.c
来源：http://cmj.hongshengwenyu.top

[U86] JS：空值合并
来源：http://ork.fanxiaobao.xyz

a ?? b
来源：http://cll.wangdashe.top

[U87] JS：解构默认值
来源：http://jhx.ydzc1.top

const { a = 1, b = 2 } = obj;
来源：http://kbl.shangyingyoupin.top

[U88] JS：对象展开合并
来源：http://umo.cdnleiting.top

{ ...a, ...b }
来源：http://rfg.shuidangran.top

[U89] JS：数组去重
来源：http://jpo.birdmap.top

[...new Set(arr)]
来源：http://dro.zdbjq.cn

[U90] JS：数字数组排序
来源：http://hmk.daria6918.cn

[...arr].sort((a, b) => a - b)
来源：http://lwx.316326.xyz

[U91] JS：对象键值遍历
来源：http://wcb.sufxvd.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dnw.52xcode.cn

[U92] JS：深拷贝
来源：http://jij.hfpthk.cn

structuredClone(obj)
来源：http://irv.yuxming.cn

[U93] JS：模板字符串
来源：http://rnp.xuanzx.com

`共 ${n} 条`
来源：http://jfv.mhx1999.top

[U94] JS：箭头函数
来源：http://hup.ywan-chungtsiang.top

const double = x => x * 2;
来源：http://qym.iojbl.cn

[U95] JS：Promise 包装
来源：http://ogy.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://rik.xingfuxueyuan.xyz

[U96] JS：async/await 与异常
来源：http://qbc.shanyushiyangkeji.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ifm.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://yhq.epnwcf.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ilk.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://che.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ono.smart0.xyz

[U99] JS：事件监听
来源：http://jkt.zhiwuduotai.top

el.addEventListener("click", e => {})
来源：http://rig.jianghu66.top

[U100] JS：DOM 查询
来源：http://bun.cucudq.cn

document.querySelector(".item")
来源：http://apu.ivvv.top

[U101] JS：classList 操作
来源：http://btv.chenjidiqi.icu

el.classList.toggle("active")
来源：http://gnh.jiagoushi.top

[U102] JS：本地存储
来源：http://afb.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bqs.aizwys.cn

[U103] JS：定时器
来源：http://yuz.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://doy.c1oappe.top

[U104] JS：防抖
来源：http://qmf.hammf.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfv.bjfxy.top

[U105] JS：节流
来源：http://vds.jinqigfzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fzy.hammf.cn

[U106] JS：日期格式化
来源：http://ncd.zycfv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oyl.meibo888.top

[U107] JS：数字千分位
来源：http://mmu.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kcz.shanyushiyangtech.top

[U108] JS：随机整数
来源：http://jlt.ivvv.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mfv.cashguo.top

[U109] JS：数组分组
来源：http://kwe.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://pga.zdqjudy.top

[U110] JS：数组分块
来源：http://laa.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jqm.fengsongda.top

[U111] JS：对象转 Map
来源：http://sus.tianlin.xyz

new Map(Object.entries(obj))
来源：http://rof.hongshengwenyu.top

[U112] JS：字符串补位
来源：http://yhn.wangshuangyany.cn

"7".padStart(3, "0")
来源：http://hps.cqqwz.cn

[U113] JS：正则替换全部
来源：http://dua.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://evn.xinyue.icu

[U114] JS：JSON 深比较
来源：http://fxv.chenjidiqi.icu

JSON.stringify(a) === JSON.stringify(b)
来源：http://ixc.hammf.cn

[U115] JS：生成 UUID
来源：http://ubg.yongpay.top

crypto.randomUUID()
来源：http://ise.hongshengwenyu.top

[U116] JS：类型检查（JSDoc）
来源：http://ffz.c1oappe.top

/** @param {string} name */ function f(name) {}
来源：http://mdw.xuetiantiany.cn

[U117] JS：单元测试
来源：http://dmc.9152youxi.cn

npm i -D vitest;  npx vitest
来源：http://fgs.nanxinkj.top

[U118] JS：开发服务器
来源：http://cht.zhixingplan.top

npm i -D vite;  npx vite
来源：http://omw.tianlin.xyz

[U119] JS：生产构建
来源：http://res.zdbjq.cn

npx vite build
来源：http://odq.epnwcf.com

[U120] JS：读取环境变量（Vite）
来源：http://ozp.hongshengwenyu.top

import.meta.env.VITE_API_URL
来源：http://tpu.quarkkingdee.top

================================================================================
来源：http://gar.ydzc1.top

统计汇总
来源：http://iab.sxryk.cn

================================================================================
来源：http://fkr.andypj.xyz

按语言统计（条）：
来源：http://oup.xziqi.cn

Python ......... 252
来源：http://aon.hcnkem.com

PHP ............ 252
来源：http://qbr.redwolf501.top

JavaScript ..... 252
来源：http://bqo.cqqwz.cn

TypeScript ..... 212
来源：http://uau.smart0.xyz

Java ........... 212
来源：http://zqy.wangdashe.top

Go ............. 212
来源：http://ati.ydjk.org.cn

Ruby ........... 212
来源：http://luu.svipenyu.cn

C# ............. 212
来源：http://zrz.smart0.xyz

C .............. 30
来源：http://tpa.tianlin.xyz

C++ ............ 30
来源：http://skk.jyoumei.cn

SQL ............ 90
来源：http://hcq.c1oappe.top

Bash ........... 80
来源：http://qxm.bbcook.cn

Kotlin ......... 15
来源：http://sjj.jinqigufen.top

Swift .......... 15
来源：http://tpc.bjfxy.top

Lua ............ 10
来源：http://tiv.kuanghao11.cn

Perl ........... 10
来源：http://eeq.yongpay.top

Scala .......... 10
来源：http://uhf.yj20258888.top

------------------------------------
来源：http://nqq.yonumen.top

合计 ........... 2106 条
来源：http://fkd.havefunace.top

按章节统计：
来源：http://jwv.cdnleiting.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://heq.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ydx.jianghu66.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ywp.redwolf501.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://huy.cdnleiting.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://qta.xziqi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ynn.redwolf501.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hji.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://uxe.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://llz.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zja.zdqjudy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://aae.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uxe.chenjidiqi.icu

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ame.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jtk.mhx1999.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ugg.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rpn.ppjwa.cn

Q SQL 专题                              90
来源：http://xrk.havefunace.top

R Bash 专题                             80
来源：http://bsp.gaohongyu789.top

S C / C++ 专题                          60
来源：http://wso.yuanzhike.top

T 其他语言补充                          60
来源：http://ylv.wangdashe.top

U 高频实用片段                         120
来源：http://lqs.ppjwa.cn

------------------------------------
来源：http://mvc.haohaochexian.top

合计                                  2106 条
来源：http://rnw.ydzc1.top

--------------------------------------------------------------------------------
来源：http://aca.shuidangran.top

使用提醒
来源：http://yfl.birdmap.top

--------------------------------------------------------------------------------
来源：http://fjz.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ryd.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mcf.hywenlv.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bhz.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://tbz.guowangkeji.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ktn.cdnleiting.top

—— 文件结束 ——
来源：http://jrb.zhongyouzk.top

================================================================================
来源：http://vey.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://cdg.birdmap.top

Common Programming Examples Cheat Book
来源：http://rqp.hnqzz.top

================================================================================
来源：http://inm.birdmap.top

【收录内容】
来源：http://ufu.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://zaf.jiagoushi.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yte.dianchejie.cn

SQL · Bash · C · C++
来源：http://hpw.ydjk.org.cn


<!-- 参考信息 -->