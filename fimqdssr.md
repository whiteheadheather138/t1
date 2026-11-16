代发 wailian999

[U05] Py：列表去重且保序
来源：http://vqn.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://aro.yongpay.top

[U06] Py：合并两个字典
来源：http://icd.birdmap.top

{**a, **b}
来源：http://pxe.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://add.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://xdh.nwbrower.top

[U08] Py：展平二维列表
来源：http://vof.sufxvd.cn

[y for x in nested for y in x]
来源：http://ssy.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://xry.guowangkeji.top

max(d, key=d.get)
来源：http://nek.dashuyun.cn

[U10] Py：按值排序字典
来源：http://tuf.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ujs.0kj1m.cn

[U11] Py：生成器表达式
来源：http://qsc.sweek.top

(x * 2 for x in arr)
来源：http://avf.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tan.c1oappe.top

Counter(arr).most_common(3)
来源：http://ccb.zhixingplan.top

[U13] Py：固定长度队列
来源：http://qnd.meibo888.top

deque(maxlen=10)
来源：http://ldr.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://tce.hammf.cn

defaultdict(list)
来源：http://khl.jianghu66.top

[U15] Py：高精度计时
来源：http://wij.jqgufenzy.top

t = time.perf_counter()
来源：http://kbf.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://gbe.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwn.jiagoushi.top

[U17] Py：初始化日志
来源：http://ngi.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://vnx.yangfankeji.com

[U18] Py：预编译正则
来源：http://gbe.ydzc1.top

pat = re.compile(r"\d+")
来源：http://zyc.ctjpmb.com

[U19] Py：正则替换带回调
来源：http://fpn.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://knr.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://pfo.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://oor.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://afg.vqdsnc.cn

@contextlib.contextmanager
来源：http://tha.yj20258.top

[U22] Py：矩阵转置
来源：http://cjk.iojbl.cn

list(zip(*m))
来源：http://pxb.guannengcc.top

[U23] Py：分块读取大文件
来源：http://bty.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hli.hnxiangtu.top

[U24] Py：路径操作
来源：http://tfw.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nrx.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://uyb.svipenyu.cn

csv.DictReader(f)
来源：http://byl.jlsjyb.cn

[U26] Py：并发下载
来源：http://jaa.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xib.tanke756.top

[U27] Py：异步 HTTP
来源：http://ajr.xylfe.cn

aiohttp.ClientSession() 配合 async with
来源：http://cuo.cdnleiting.top

[U28] Py：类型别名
来源：http://tre.shangyingyoupin.top

UserId = int
来源：http://rat.bjfxy.top

[U29] Py：属性校验
来源：http://tcb.andypj.xyz

@property 与 @x.setter 配合
来源：http://baw.hammf.cn

[U30] Py：数据类
来源：http://mid.tian-w.cn

@dataclass(slots=True)
来源：http://xxp.ppjwa.cn

[U31] Py：单测
来源：http://gme.nanxinkj.top

python -m pytest -q
来源：http://icg.cheryme.top

[U32] Py：代码格式化
来源：http://jht.tarul.cn

ruff format . && ruff check --fix .
来源：http://zmv.pengpengdd.cyou

[U33] Py：打包发布
来源：http://zyw.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://hex.ydjk.org.cn

[U34] Py：判断编码
来源：http://yzj.cucudq.cn

chardet.detect(raw)
来源：http://adv.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://wac.zdqjudy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mht.hywenlv.cn

[U36] Py：定时任务
来源：http://hre.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://wdq.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://vpp.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fbr.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://gqy.fehbvm.com

Path(__file__).resolve().parent
来源：http://wlq.hysaishi.cn

[U39] Py：判断是否在交互环境
来源：http://hfq.haohaochexian.top

sys.stdout.isatty()
来源：http://hgb.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://ttj.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://gqu.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://blx.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xgg.yuanzhike.top

[U42] PHP：PSR-4 自动加载
来源：http://shk.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ygj.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://spu.gotoacloud.top

namespace App\Http;
来源：http://wsn.nwbrower.top

[U44] PHP：开启严格类型
来源：http://hqu.havefunace.top

declare(strict_types=1);
来源：http://caf.daxiang520.top

[U45] PHP：类型声明与返回类型
来源：http://kkt.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gpu.hammf.cn

[U46] PHP：可空类型
来源：http://vft.daxiang520.top

?string $name = null
来源：http://quh.ybcxt.top

[U47] PHP：联合类型
来源：http://pkd.ppjwa.cn

int|string $id
来源：http://qnq.jqgfzy.top

[U48] PHP：纯枚举
来源：http://boz.yuxming.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kob.chenlongwang.top

[U49] PHP：只读属性
来源：http://jls.xziqi.cn

public readonly string $name
来源：http://qlu.birdmap.top

[U50] PHP：构造器属性提升
来源：http://uzr.aizwys.cn

public function __construct(private int $id) {}
来源：http://xef.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://qim.smart0.xyz

[$a, $b] = $arr;
来源：http://srp.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://ecn.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://rpa.sufxvd.cn

[U53] PHP：空合并运算符
来源：http://oem.xingfuxueyuan.xyz

$v = $a ?? $b ?? "default";
来源：http://xnl.tian-w.cn

[U54] PHP：空安全调用
来源：http://gjr.hnqzz.top

$obj?->method()
来源：http://khi.hywenlv.cn

[U55] PHP：match 表达式
来源：http://fox.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrk.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://aue.hammf.cn

f(a: 1, b: 2)
来源：http://jwa.zycfv.cn

[U57] PHP：字符串插值
来源：http://tym.ybcxt.top

"值: {$a}"
来源：http://kbz.sweek.top

[U58] PHP：数组三件套
来源：http://rtr.yueranfly.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eol.ctjpmb.com

[U59] PHP：自定义排序
来源：http://hba.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jrp.tanke756.top

[U60] PHP：JSON 编解码
来源：http://spi.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gmd.cucudq.cn

[U61] PHP：正则
来源：http://sne.aizwys.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pde.0kj1m.cn

[U62] PHP：日期对象
来源：http://vrc.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pdm.fzhhl.top

[U63] PHP：文件读写
来源：http://jmy.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uyv.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://cxj.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://eyv.yfazqb.com

[U65] PHP：会话
来源：http://ebs.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pdt.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://xob.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xpt.ivvv.top

[U67] PHP：处理文件上传
来源：http://bkk.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vne.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://axs.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ynl.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://bsf.havefunace.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mve.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://jue.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://djl.yj20258888.top

[U71] PHP：抛出异常
来源：http://hkp.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://abp.yj202588.top

[U72] PHP：写错误日志
来源：http://bfg.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://uie.sweek.top

[U73] PHP：读取 ini 配置
来源：http://gih.zhiwuduotai.top

parse_ini_file("config.ini", true)
来源：http://jbc.iojbl.cn

[U74] PHP：读取环境变量
来源：http://fxr.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://kgb.jinqigufen.top

[U75] PHP：依赖注入
来源：http://axr.uphjek.com

composer require psr/container
来源：http://wjt.c1oappe.top

[U76] PHP：简单路由
来源：http://bqy.dianchejie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ntj.yvedp.cn

[U77] PHP：模板渲染
来源：http://ldy.uphjek.com

composer require twig/twig
来源：http://jxb.jinqigfzy.top

[U78] PHP：单元测试
来源：http://tfp.gzhubu.top

composer require --dev phpunit/phpunit
来源：http://vxs.9152youxi.cn

[U79] PHP：静态分析
来源：http://tsc.nwbrower.top

composer require --dev phpstan/phpstan
来源：http://oua.chenlongwang.top

[U80] PHP：代码规范修复
来源：http://fgu.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gqf.daxiang520.top

[U81] JS：初始化项目
来源：http://yhg.daria6918.cn

npm init -y;  npm i express
来源：http://fxj.sysykeji.top

[U82] JS：package.json 脚本
来源：http://hie.aibaodan.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nrh.fengsongda.top

[U83] JS：ES Module 导入导出
来源：http://ghe.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hmw.sxryk.cn

[U84] JS：CommonJS 写法
来源：http://vks.cdnleiting.top

module.exports = { a };  const { a } = require("./m");
来源：http://mti.xuanzx.com

[U85] JS：可选链
来源：http://kbc.fehbvm.com

a?.b?.c
来源：http://qaw.shangyingyoupin.top

[U86] JS：空值合并
来源：http://fdr.wangshuangyany.cn

a ?? b
来源：http://tbp.vqdsnc.cn

[U87] JS：解构默认值
来源：http://ywx.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://new.ywan-chungtsiang.top

[U88] JS：对象展开合并
来源：http://nwu.xuetiantiany.cn

{ ...a, ...b }
来源：http://ooy.zhongyouzk.top

[U89] JS：数组去重
来源：http://pjr.xziqi.cn

[...new Set(arr)]
来源：http://uvu.aibaodan.cn

[U90] JS：数字数组排序
来源：http://cqh.shangyingyoupin.top

[...arr].sort((a, b) => a - b)
来源：http://itd.sxryk.cn

[U91] JS：对象键值遍历
来源：http://lvo.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kbq.sjlbkw.cn

[U92] JS：深拷贝
来源：http://dqg.vqdsnc.cn

structuredClone(obj)
来源：http://rlg.jianghu66.top

[U93] JS：模板字符串
来源：http://yfx.yongpay.top

`共 ${n} 条`
来源：http://gya.316326.xyz

[U94] JS：箭头函数
来源：http://zha.jqgfzy.top

const double = x => x * 2;
来源：http://rzd.shanyushiyangtech.top

[U95] JS：Promise 包装
来源：http://gdd.hammf.cn

new Promise((resolve, reject) => {})
来源：http://usg.wangshuangyany.cn

[U96] JS：async/await 与异常
来源：http://hkt.kuanghao11.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://htl.c1oappe.top

[U97] JS：并发请求
来源：http://vcu.havefunace.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ocg.zhaomingkeji.xyz

[U98] JS：fetch 带 JSON
来源：http://fkh.zycfv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://deh.xingfuxueyuan.xyz

[U99] JS：事件监听
来源：http://rnf.dashuyun.cn

el.addEventListener("click", e => {})
来源：http://wfm.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://czq.zhixingplan.top

document.querySelector(".item")
来源：http://yjj.havefunace.top

[U101] JS：classList 操作
来源：http://nce.hammf.cn

el.classList.toggle("active")
来源：http://mxt.fehbvm.com

[U102] JS：本地存储
来源：http://quh.nanxinkj.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://osx.haohaochexian.top

[U103] JS：定时器
来源：http://mdn.nanxinkj.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://exu.uphjek.com

[U104] JS：防抖
来源：http://utd.shanyushiyangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://leh.xinyue.icu

[U105] JS：节流
来源：http://qxg.hnqzz.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pja.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://yxn.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ngj.fengsongda.top

[U107] JS：数字千分位
来源：http://pqa.mhx1999.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tqj.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://hkl.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ssy.nanxuanxn.top

[U109] JS：数组分组
来源：http://krf.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://hov.zhongyouzk.top

[U110] JS：数组分块
来源：http://wup.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ego.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://mss.vehdjk.com

new Map(Object.entries(obj))
来源：http://ysx.sweek.top

[U112] JS：字符串补位
来源：http://mmw.ydzc1.top

"7".padStart(3, "0")
来源：http://rnh.xylfe.cn

[U113] JS：正则替换全部
来源：http://oeh.fzhhl.top

s.replaceAll("a", "b")
来源：http://ext.chenzaomai.com

[U114] JS：JSON 深比较
来源：http://qek.gzhubu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tup.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://ydu.yongpay.top

crypto.randomUUID()
来源：http://xfc.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://bmu.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://dgx.ydjk.org.cn

[U117] JS：单元测试
来源：http://vpt.smart0.xyz

npm i -D vitest;  npx vitest
来源：http://fcn.xziqi.cn

[U118] JS：开发服务器
来源：http://ohn.gaohongyu789.top

npm i -D vite;  npx vite
来源：http://krl.xingfuxueyuan.xyz

[U119] JS：生产构建
来源：http://ziq.haohaochexian.top

npx vite build
来源：http://shq.cashguo.top

[U120] JS：读取环境变量（Vite）
来源：http://atp.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://ttn.yueranfly.top

================================================================================
来源：http://vzb.xingfuxueyuan.xyz

统计汇总
来源：http://hue.zhixingplan.top

================================================================================
来源：http://ycj.tian-w.cn

按语言统计（条）：
来源：http://btt.yonumen.top

Python ......... 252
来源：http://gwm.xylfe.cn

PHP ............ 252
来源：http://yrn.zhixingplan.top

JavaScript ..... 252
来源：http://doh.yuxming.cn

TypeScript ..... 212
来源：http://ohx.bbcook.cn

Java ........... 212
来源：http://elo.cdnleiting.top

Go ............. 212
来源：http://mys.yanxiufei.cn

Ruby ........... 212
来源：http://lnt.ppjwa.cn

C# ............. 212
来源：http://teq.chenzaomai.com

C .............. 30
来源：http://dbb.jlsjyb.cn

C++ ............ 30
来源：http://dii.cqqwz.cn

SQL ............ 90
来源：http://jem.ppjwa.cn

Bash ........... 80
来源：http://wwc.birdmap.top

Kotlin ......... 15
来源：http://btk.0kj1m.cn

Swift .......... 15
来源：http://ofa.xuanzx.com

Lua ............ 10
来源：http://bww.xziqi.cn

Perl ........... 10
来源：http://stf.jqgfzy.top

Scala .......... 10
来源：http://awl.yvedp.cn

------------------------------------
来源：http://ftu.nanxinkj.top

合计 ........... 2106 条
来源：http://wii.jqgfzy.top

按章节统计：
来源：http://ffz.fktsv.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://irh.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qma.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xtf.yueranfly.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://amk.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://drz.bjfxy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dvu.chenzaomai.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wqk.quarkkingdee.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jrd.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://syd.hesvh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wtk.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fte.xingfuxueyuan.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tdp.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ekk.cdnleiting.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pgj.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://byl.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mdt.tianlin.xyz

Q SQL 专题                              90
来源：http://roz.jinghuilouyu.cn

R Bash 专题                             80
来源：http://lxy.cashguo.top

S C / C++ 专题                          60
来源：http://rsq.zhengqikj.top

T 其他语言补充                          60
来源：http://ozz.52xcode.cn

U 高频实用片段                         120
来源：http://sdf.zhiwuduotai.top

------------------------------------
来源：http://ktn.hnqzz.top

合计                                  2106 条
来源：http://nbi.xinyue.icu

--------------------------------------------------------------------------------
来源：http://zme.zhaomingkeji.xyz

使用提醒
来源：http://cee.yj20258888.top

--------------------------------------------------------------------------------
来源：http://jsg.havefunace.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://usk.yj202588.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vpz.jinyuanbaomall.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://feo.tanke756.top

在旧版本上使用前请先确认语法支持情况。
来源：http://eai.tian-w.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kiv.sxryk.cn

—— 文件结束 ——
来源：http://xcz.pengpengdd.cyou

================================================================================
来源：http://eyf.haohaochexian.top

程序语言常见例子速查手册（2024 版）
来源：http://kei.xingfuxueyuan.xyz

Common Programming Examples Cheat Book
来源：http://jyu.zhijiandao.cn

================================================================================
来源：http://nja.fktsv.cn

【收录内容】
来源：http://pso.tanke756.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://gjy.yj20258888.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ugh.zhongyouzk.top

SQL · Bash · C · C++
来源：http://dto.quarkkingdee.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ptg.xuetiantiany.cn

【使用说明】
来源：http://lci.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xez.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fnh.ydzc1.top


<!-- 参考信息 -->