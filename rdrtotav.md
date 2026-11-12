代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ape.cashguo.top

[R30] 函数返回状态码
来源：http://iul.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://efd.zhixingplan.top

[R31] 局部变量
来源：http://tol.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://zni.shangyingyoupin.top

[R32] 参数个数校验
来源：http://rnl.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tjw.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://wsl.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ulj.shanyushiyangtech.top

[R34] 退出时清理
来源：http://tmx.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oqc.yuanzhike.top

[R35] 后台执行并等待
来源：http://fwy.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yek.cdnleiting.top

[R36] 并发执行多个任务
来源：http://box.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://var.aibaodan.cn

[R37] 把输出赋给变量
来源：http://dzp.hywenlv.cn

files=$(ls -1)
来源：http://bot.fanxiaobao.xyz

[R38] 管道串联
来源：http://bdf.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://ecu.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://nvp.mhx1999.top

cmd > out.log 2>&1
来源：http://byt.jqgfzy.top

[R40] 追加写日志
来源：http://sjr.hysaishi.cn

echo "log" >> out.log
来源：http://qys.hnqzz.top

[R41] 丢弃输出
来源：http://tio.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://pwx.zdbjq.cn

[R42] 输入重定向
来源：http://sxx.fehbvm.com

wc -l < a.txt
来源：http://fnv.fengsongda.top

[R43] 按名字查找文件
来源：http://glq.dianchejie.cn

find . -name "*.log" -type f
来源：http://dlr.pycfn.com

[R44] 按修改时间查找
来源：http://hmp.xuanzx.com

find . -mtime -7 -type f
来源：http://ykm.zdqjudy.top

[R45] 批量删除
来源：http://ipt.yfazqb.com

find . -name "*.tmp" -delete
来源：http://ngj.9152youxi.cn

[R46] 递归替换文件内容
来源：http://wzf.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvt.zhengqikj.top

[R47] sed 单行替换
来源：http://hqj.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jrj.hongshengwenyu.top

[R48] awk 取指定列
来源：http://tnc.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://vsm.nanxuanxn.top

[R49] awk 带条件
来源：http://oun.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tht.bjfxy.top

[R50] awk 求和
来源：http://egx.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://ryo.sweek.top

[R51] 排序去重取前几
来源：http://une.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://whx.iojbl.cn

[R52] 统计行数
来源：http://oox.hcnkem.com

wc -l a.txt
来源：http://qzh.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://rqk.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gob.zhijiandao.cn

[R54] 比较两个文件
来源：http://ndh.yonumen.top

diff a.txt b.txt
来源：http://kww.chenzaomai.com

[R55] 压缩与解压
来源：http://dtd.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zxg.gogol.net.cn

[R56] 远程拷贝
来源：http://znu.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://jwm.daxiang520.top

[R57] 远程执行命令
来源：http://wwx.yvedp.cn

ssh user@host 'uptime'
来源：http://ocf.hesvh.cn

[R58] 下载文件
来源：http://iph.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gpl.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://ibg.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipa.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://wzo.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xqw.jqgfzy.top

[R61] 磁盘占用
来源：http://cmg.ydzc1.top

df -h;  du -sh *
来源：http://gsd.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://wsb.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://pnb.316326.xyz

[R63] 内存与进程
来源：http://ius.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://rry.shangyingyoupin.top

[R64] 结束进程
来源：http://dhu.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://hvm.hywenlv.cn

[R65] 查看端口占用
来源：http://ole.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tvz.hysaishi.cn

[R66] 定时任务
来源：http://ljm.chenzaomai.com

crontab -e;  crontab -l
来源：http://dqg.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://jom.dianchejie.cn

openssl rand -hex 16
来源：http://lcl.316326.xyz

[R68] 计算文件校验值
来源：http://wwi.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://skg.jinqigufen.top

[R69] 生成随机密码
来源：http://lze.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://ppv.sjlbkw.cn

[R70] 时间戳与互转
来源：http://sqg.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://naf.jianghu66.top

[R71] 日期格式化
来源：http://rgf.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://uxf.dianchejie.cn

[R72] 等待端口就绪
来源：http://vte.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qfs.daxiang520.top

[R73] 分割大日志
来源：http://zyv.dashuyun.cn

split -l 1000 big.log part_
来源：http://ler.yanxiufei.cn

[R74] 批量重命名
来源：http://fgj.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wee.gogol.net.cn

[R75] 导出环境变量
来源：http://yfb.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://dvr.gotoacloud.top

[R76] 使用临时文件
来源：http://ugy.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uvj.quarkkingdee.top

[R77] 读取用户输入
来源：http://vqu.sysykeji.top

read -rp "请输入: " ans
来源：http://hop.tarul.cn

[R78] 交互式菜单
来源：http://zka.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jaj.xinyue.icu

[R79] 解析命令行选项
来源：http://zkb.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzy.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://gcl.yvedp.cn

time ./run.sh
来源：http://qkk.hcnkem.com

================================================================================
来源：http://sur.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://udu.shuidangran.top

================================================================================
来源：http://ywf.havefunace.top

[S01] C：Hello World
来源：http://vqx.yueranfly.top

#include <stdio.h>
来源：http://guu.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ypr.tarul.cn

[S02] C：变量与格式化输出
来源：http://gga.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://qze.jqgfzy.top

[S03] C：读入整数
来源：http://ytr.sysykeji.top

int x; scanf("%d", &x);
来源：http://tcg.redwolf501.top

[S04] C：字符串复制
来源：http://nsh.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kvr.xuanzx.com

[S05] C：字符串长度
来源：http://cep.c1oappe.top

strlen(s)
来源：http://sgq.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://ryu.mhx1999.top

strcmp(a, b) == 0
来源：http://mhi.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://xqq.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kpy.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://mze.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wjf.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://pgh.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://inx.pycfn.com

[S10] C：指针与解引用
来源：http://yll.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://mgo.aibaodan.cn

[S11] C：逐行读文件
来源：http://qcs.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://crt.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jrc.pengpengdd.cyou

fclose(f);
来源：http://zam.0kj1m.cn

[S12] C：写文件
来源：http://vjt.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fxe.birdmap.top

[S13] C：宏定义
来源：http://moc.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bxo.shangyingyoupin.top

[S14] C：枚举
来源：http://pnz.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://uhh.redwolf501.top

[S15] C：类型转换
来源：http://prw.xylfe.cn

(double) a / b
来源：http://aql.ydjk.org.cn

[S16] C：位操作置位
来源：http://aao.andypj.xyz

x |= (1 << 3);
来源：http://jta.jianghu66.top

[S17] C：安全拼接字符串
来源：http://mov.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://alw.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://aqe.bjfxy.top

int main(int argc, char **argv)
来源：http://oka.fanxiaobao.xyz

[S19] C：快速排序
来源：http://quu.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgr.fehbvm.com

[S20] C：二分查找
来源：http://xvp.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gbp.ctjpmb.com

[S21] C：字符类别判断
来源：http://idq.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jql.yanxiufei.cn

[S22] C：字符串转数字
来源：http://rvx.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ucu.cheryme.top

[S23] C：随机数
来源：http://ecv.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qrr.zhoulong.xyz

[S24] C：获取本地时间
来源：http://ntz.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xsp.ybcxt.top

[S25] C：内存拷贝
来源：http://hnx.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://ndw.yonumen.top

[S26] C：内存清零
来源：http://hvn.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://lmf.nanxinkj.top

[S27] C：定义常量
来源：http://bjd.yongpay.top

const double PI = 3.14159;
来源：http://wnp.yvedp.cn

[S28] C：静态变量
来源：http://nrj.birdmap.top

static int counter = 0;
来源：http://ttq.jqgufenzy.top

[S29] C：变参函数
来源：http://wuj.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xsw.cashguo.top

[S30] C：头文件保护
来源：http://tpu.cucudq.cn

#ifndef X_H
来源：http://tqs.daria6918.cn

#define X_H
来源：http://oev.svipenyu.cn

#endif
来源：http://jsh.jqgufenzy.top

[S31] C++：Hello World
来源：http://dpo.316326.xyz

#include <iostream>
来源：http://qux.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://fxr.dianchejie.cn

[S32] C++：字符串
来源：http://kgl.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://jyh.gotoacloud.top

[S33] C++：vector 增删
来源：http://wef.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bpv.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://cdh.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://wdo.wangdashe.top

[S35] C++：map
来源：http://urs.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://okl.hfpthk.cn

[S36] C++：unordered_map
来源：http://epg.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bue.jlsjyb.cn

[S37] C++：set
来源：http://hvt.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xtj.ydjk.org.cn

[S38] C++：排序
来源：http://jlc.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://iiw.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://bua.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gfh.dashuyun.cn

[S40] C++：查找元素
来源：http://hpd.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aba.ydzc1.top

[S41] C++：类与构造函数
来源：http://iew.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fqd.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://mij.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://wqb.sweek.top

[S43] C++：智能指针
来源：http://uqz.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://wlt.yuanzhike.top

[S44] C++：引用传参
来源：http://hwi.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://ncq.yanxiufei.cn

[S45] C++：lambda
来源：http://axz.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hbn.yj202588.top

[S46] C++：函数模板
来源：http://cdk.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://drc.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://sni.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oew.fengsongda.top

[S48] C++：逐行读文件
来源：http://dam.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://aep.daria6918.cn

while (std::getline(in, line)) { }
来源：http://sua.jlsjyb.cn

[S49] C++：写文件
来源：http://vdx.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wwk.nwbrower.top

[S50] C++：格式化数字
来源：http://rop.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wat.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://frc.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://kbn.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://hah.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://osp.yangfankeji.com

[S53] C++：移动语义
来源：http://ypq.316326.xyz

std::vector<int> w = std::move(v);
来源：http://hrv.hcnkem.com

[S54] C++：异常处理
来源：http://ufi.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rgn.jqgfzy.top

[S55] C++：结构化绑定
来源：http://dct.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rht.c1oappe.top

[S56] C++：optional
来源：http://yyd.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ckt.tianlin.xyz

[S57] C++：编译期常量
来源：http://gmz.hongshengwenyu.top

constexpr int N = 10;
来源：http://qra.dashuyun.cn

[S58] C++：命名空间
来源：http://ouk.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://lhk.yfazqb.com

[S59] C++：静态断言
来源：http://bzo.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xzs.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://gqm.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kwg.nanxuanxn.top

================================================================================
来源：http://utm.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kzm.kuanghao11.cn

================================================================================
来源：http://imo.daria6918.cn

[T01] Kotlin：Hello World
来源：http://dri.chenzaomai.com

println("Hello")
来源：http://lxp.tianlin.xyz

[T02] Kotlin：变量
来源：http://ioj.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gtn.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://oxv.feifeiyinyue.top

"值: $b"
来源：http://hpn.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://elg.ppjwa.cn

val n: String? = null;  n?.length
来源：http://oqa.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://mvs.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yxj.sweek.top

[T06] Kotlin：集合映射
来源：http://ola.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ueu.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://qwc.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://frz.redwolf501.top

[T08] Kotlin：数据类
来源：http://nos.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://ejb.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://vou.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://fiv.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://oln.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qwo.hcnkem.com

[T11] Kotlin：协程
来源：http://gsp.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mls.tarul.cn

[T12] Kotlin：解构声明
来源：http://jrp.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://vjw.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://ljd.52xcode.cn

val m = mapOf("a" to 1)
来源：http://zyw.fengsongda.top

[T14] Kotlin：循环
来源：http://gnp.zdqjudy.top

for (i in 1..10) println(i)
来源：http://wqi.dianchejie.cn

[T15] Kotlin：接口
来源：http://vlr.yfazqb.com

interface Shape { fun area(): Double }
来源：http://qml.hammf.cn

[T16] Swift：Hello World
来源：http://hff.hcnkem.com

print("Hello")
来源：http://wnz.jyoumei.cn

[T17] Swift：变量与常量
来源：http://fwc.ydjk.org.cn

var a = 1;  let b = 2
来源：http://ooc.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://wsj.yfazqb.com

"值: \(b)"
来源：http://blw.zhengqikj.top

[T19] Swift：可选绑定
来源：http://jfd.havefunace.top

if let n = opt { print(n) }
来源：http://tpg.yj20258888.top

[T20] Swift：数组操作
来源：http://krc.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://svp.gotoacloud.top

[T21] Swift：遍历
来源：http://dpg.nanxinkj.top

for x in a { print(x) }
来源：http://euq.0kj1m.cn

[T22] Swift：字典
来源：http://jhx.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tla.daxiang520.top

[T23] Swift：函数
来源：http://sbk.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sng.guowangkeji.top

[T24] Swift：闭包
来源：http://rjr.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nld.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://vwr.chenjidiqi.icu

struct P { var x: Int }
来源：http://pwm.yj20258888.top

[T26] Swift：类与重写
来源：http://iwa.bbcook.cn

class A: Base { override func f() {} }
来源：http://zzk.ydzc1.top

[T27] Swift：错误处理
来源：http://pto.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://qar.svipenyu.cn

[T28] Swift：枚举
来源：http://wyl.aibaodan.cn

enum Color { case red, green }
来源：http://xmc.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://ejv.ppjwa.cn

guard let x = opt else { return }
来源：http://zyw.jqgufenzy.top

[T30] Swift：协议
来源：http://dhi.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://lgt.sxryk.cn

[T31] Lua：Hello World
来源：http://mii.yj202588.top

print("Hello")
来源：http://cnd.iojbl.cn

[T32] Lua：局部变量
来源：http://kxa.dianchejie.cn

local a = 1
来源：http://ibq.jinqigufen.top


<!-- 参考信息 -->