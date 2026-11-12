代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://axp.nwbrower.top

[R24] 大小写转换
来源：http://fsg.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uxe.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://vod.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://jmo.fktsv.cn

[R26] 命令替换
来源：http://tsm.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://bdh.nanxinkj.top

[R27] 算术展开
来源：http://xoz.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://gjk.yfazqb.com

[R28] 浮点运算
来源：http://wsu.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://eer.jlsjyb.cn

[R29] 定义函数
来源：http://jki.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nuo.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://yrs.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://ihk.yuxming.cn

[R31] 局部变量
来源：http://sww.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://gli.tianlin.xyz

[R32] 参数个数校验
来源：http://etc.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rfk.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://yre.zhaomingkeji.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iyf.xinyue.icu

[R34] 退出时清理
来源：http://kfy.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://lkw.sweek.top

[R35] 后台执行并等待
来源：http://gmv.sufxvd.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vuf.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://yhu.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ulw.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://vbu.nanxinkj.top

files=$(ls -1)
来源：http://tqw.cdnleiting.top

[R38] 管道串联
来源：http://tzv.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://dmg.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://brl.yuxming.cn

cmd > out.log 2>&1
来源：http://fxk.sjlbkw.cn

[R40] 追加写日志
来源：http://qjs.yangfankeji.com

echo "log" >> out.log
来源：http://gcc.gaohongyu789.top

[R41] 丢弃输出
来源：http://vnm.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://kvx.xylfe.cn

[R42] 输入重定向
来源：http://khx.cqqwz.cn

wc -l < a.txt
来源：http://aae.pycfn.com

[R43] 按名字查找文件
来源：http://xde.jqgufenzy.top

find . -name "*.log" -type f
来源：http://ylv.yj20258.top

[R44] 按修改时间查找
来源：http://mbs.shuidangran.top

find . -mtime -7 -type f
来源：http://mgz.cashguo.top

[R45] 批量删除
来源：http://qjn.ydzc1.top

find . -name "*.tmp" -delete
来源：http://snw.aibaodan.cn

[R46] 递归替换文件内容
来源：http://kvo.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utn.yj202588.top

[R47] sed 单行替换
来源：http://ukg.cheryme.top

sed -i 's/foo/bar/g' a.txt
来源：http://zky.sjlbkw.cn

[R48] awk 取指定列
来源：http://ixy.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://bcg.wangdashe.top

[R49] awk 带条件
来源：http://mbx.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pei.svipenyu.cn

[R50] awk 求和
来源：http://nas.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxo.tanke756.top

[R51] 排序去重取前几
来源：http://qof.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wce.zycfv.cn

[R52] 统计行数
来源：http://qlp.fktsv.cn

wc -l a.txt
来源：http://old.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://sms.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lwb.gaohongyu789.top

[R54] 比较两个文件
来源：http://jhi.cheryme.top

diff a.txt b.txt
来源：http://mcx.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://iam.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ypv.gaohongyu789.top

[R56] 远程拷贝
来源：http://zif.nwbrower.top

scp file user@host:/path/
来源：http://iyl.cucudq.cn

[R57] 远程执行命令
来源：http://vrd.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://ygv.birdmap.top

[R58] 下载文件
来源：http://auc.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://btk.svipenyu.cn

[R59] 发 POST JSON
来源：http://kzb.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uqc.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://tyb.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yml.hnxiangtu.top

[R61] 磁盘占用
来源：http://gvh.jlsjyb.cn

df -h;  du -sh *
来源：http://gyd.meibo888.top

[R62] 找最占空间的文件
来源：http://lhi.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://rdt.yvedp.cn

[R63] 内存与进程
来源：http://inc.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://krg.kuanghao11.cn

[R64] 结束进程
来源：http://eak.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://vkz.uphjek.com

[R65] 查看端口占用
来源：http://ssq.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eum.chenlongwang.top

[R66] 定时任务
来源：http://icp.gotoacloud.top

crontab -e;  crontab -l
来源：http://hcm.havefunace.top

[R67] 生成随机十六进制串
来源：http://kyz.jyoumei.cn

openssl rand -hex 16
来源：http://nzh.zycfv.cn

[R68] 计算文件校验值
来源：http://iol.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://kdr.ydzc1.top

[R69] 生成随机密码
来源：http://wbd.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://vqs.hysaishi.cn

[R70] 时间戳与互转
来源：http://wgd.hammf.cn

date +%s;  date -d @1700000000
来源：http://iyr.cucudq.cn

[R71] 日期格式化
来源：http://ecw.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://shv.zycfv.cn

[R72] 等待端口就绪
来源：http://hot.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hel.nwbrower.top

[R73] 分割大日志
来源：http://wdb.52xcode.cn

split -l 1000 big.log part_
来源：http://kwt.ctjpmb.com

[R74] 批量重命名
来源：http://nis.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bra.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://wyt.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://kao.yongpay.top

[R76] 使用临时文件
来源：http://vel.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mjc.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://oky.zhongyouzk.top

read -rp "请输入: " ans
来源：http://vzy.meibo888.top

[R78] 交互式菜单
来源：http://mkx.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qla.gzhubu.top

[R79] 解析命令行选项
来源：http://mmf.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://skk.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://sik.aizwys.cn

time ./run.sh
来源：http://xuz.yuxming.cn

================================================================================
来源：http://xjn.shuidangran.top

S. C / C++ 专题
来源：http://fiz.daria6918.cn

================================================================================
来源：http://bbc.yangfankeji.com

[S01] C：Hello World
来源：http://new.cheryme.top

#include <stdio.h>
来源：http://mdi.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfa.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://pgh.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://nws.birdmap.top

[S03] C：读入整数
来源：http://kjk.guowangkeji.top

int x; scanf("%d", &x);
来源：http://xla.kuanghao11.cn

[S04] C：字符串复制
来源：http://sxd.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wog.sufxvd.cn

[S05] C：字符串长度
来源：http://nsj.xylfe.cn

strlen(s)
来源：http://kxh.birdmap.top

[S06] C：字符串比较
来源：http://mfl.0kj1m.cn

strcmp(a, b) == 0
来源：http://pla.xylfe.cn

[S07] C：数组遍历求和
来源：http://tgw.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mdh.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://gpj.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vye.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://nfk.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ehm.tian-w.cn

[S10] C：指针与解引用
来源：http://erh.andypj.xyz

int *p = &a;  *p = 5;
来源：http://ecs.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://efx.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://cnx.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zvj.bbcook.cn

fclose(f);
来源：http://byl.fanxiaobao.xyz

[S12] C：写文件
来源：http://wuu.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rey.guannengcc.top

[S13] C：宏定义
来源：http://qdn.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xjq.daria6918.cn

[S14] C：枚举
来源：http://yuz.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://uqv.dashuyun.cn

[S15] C：类型转换
来源：http://eel.316326.xyz

(double) a / b
来源：http://hdt.cdnleiting.top

[S16] C：位操作置位
来源：http://yaa.sufxvd.cn

x |= (1 << 3);
来源：http://iro.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://pfs.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dpo.birdmap.top

[S18] C：命令行参数
来源：http://fur.mhx1999.top

int main(int argc, char **argv)
来源：http://wpt.nanxuanxn.top

[S19] C：快速排序
来源：http://gzj.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://rev.gogol.net.cn

[S20] C：二分查找
来源：http://cbq.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ail.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://ius.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kds.ydzc1.top

[S22] C：字符串转数字
来源：http://tnj.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://zwg.jiagoushi.top

[S23] C：随机数
来源：http://ztw.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ctx.jiagoushi.top

[S24] C：获取本地时间
来源：http://hpr.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lav.jinqigufen.top

[S25] C：内存拷贝
来源：http://szs.yangfankeji.com

memcpy(dst, src, n);
来源：http://aiw.birdmap.top

[S26] C：内存清零
来源：http://onu.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://ize.ivvv.top

[S27] C：定义常量
来源：http://nnn.hesvh.cn

const double PI = 3.14159;
来源：http://sbv.tarul.cn

[S28] C：静态变量
来源：http://bau.zhoulong.xyz

static int counter = 0;
来源：http://bpl.jinghuilouyu.cn

[S29] C：变参函数
来源：http://jpp.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://znp.cucudq.cn

[S30] C：头文件保护
来源：http://lcm.nanxinkj.top

#ifndef X_H
来源：http://xtr.zdqjudy.top

#define X_H
来源：http://uwh.xuanzx.com

#endif
来源：http://gvq.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://zpy.smart0.xyz

#include <iostream>
来源：http://nqb.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ozt.tianlin.xyz

[S32] C++：字符串
来源：http://wiw.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://wtn.sysykeji.top

[S33] C++：vector 增删
来源：http://usr.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://csb.tarul.cn

[S34] C++：遍历 vector
来源：http://dlg.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://djz.0kj1m.cn

[S35] C++：map
来源：http://qdd.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ziy.fengsongda.top

[S36] C++：unordered_map
来源：http://uzn.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uwd.haohaochexian.top

[S37] C++：set
来源：http://hlc.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fto.quarkkingdee.top

[S38] C++：排序
来源：http://ejy.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://kni.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://yam.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fkb.andypj.xyz

[S40] C++：查找元素
来源：http://mel.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tqq.zycfv.cn

[S41] C++：类与构造函数
来源：http://xud.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://crx.cucudq.cn

[S42] C++：继承与虚函数
来源：http://uzo.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://ztc.yongpay.top

[S43] C++：智能指针
来源：http://rba.sweek.top

auto p = std::make_unique<int>(5);
来源：http://qzs.hnxiangtu.top

[S44] C++：引用传参
来源：http://mqo.yj202588.top

void inc(int &x) { ++x; }
来源：http://ipl.yuanzhike.top

[S45] C++：lambda
来源：http://zir.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://kpu.vqdsnc.cn

[S46] C++：函数模板
来源：http://gzh.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xje.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://srb.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oia.fzhhl.top

[S48] C++：逐行读文件
来源：http://mzw.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://seu.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://vyp.cashguo.top

[S49] C++：写文件
来源：http://foq.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xni.hysaishi.cn

[S50] C++：格式化数字
来源：http://xyf.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yci.uphjek.com

[S51] C++：显式类型转换
来源：http://glp.52xcode.cn

static_cast<double>(a) / b
来源：http://ljv.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://hiz.yfazqb.com

int size() const noexcept { return n_; }
来源：http://lkg.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://cvi.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://ihl.fktsv.cn

[S54] C++：异常处理
来源：http://qcx.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qyd.ybcxt.top

[S55] C++：结构化绑定
来源：http://wdw.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lxh.yongpay.top

[S56] C++：optional
来源：http://apy.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ylh.kuanghao11.cn

[S57] C++：编译期常量
来源：http://jer.iojbl.cn

constexpr int N = 10;
来源：http://msv.zdbjq.cn

[S58] C++：命名空间
来源：http://ibc.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://hyj.zhixingplan.top

[S59] C++：静态断言
来源：http://zmv.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iti.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://dys.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ert.kuanghao11.cn

================================================================================
来源：http://jqi.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ywd.guowangkeji.top

================================================================================
来源：http://far.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://byv.aibaodan.cn

println("Hello")
来源：http://vxj.hammf.cn

[T02] Kotlin：变量
来源：http://ptb.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tpb.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://icn.jinqigfzy.top

"值: $b"
来源：http://fzu.yfazqb.com

[T04] Kotlin：空安全
来源：http://otb.meibo888.top

val n: String? = null;  n?.length
来源：http://xls.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://lwi.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://epf.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://urx.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tuz.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://aos.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://foe.daria6918.cn

[T08] Kotlin：数据类
来源：http://nmd.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://wgd.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://txp.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://dtq.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://jjx.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://auh.chenzaomai.com

[T11] Kotlin：协程
来源：http://izq.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://skq.jianghu66.top

[T12] Kotlin：解构声明
来源：http://ytg.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://kau.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://ipe.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://syq.sysykeji.top

[T14] Kotlin：循环
来源：http://uvj.cashguo.top

for (i in 1..10) println(i)
来源：http://rgb.ybcxt.top

[T15] Kotlin：接口
来源：http://kee.andypj.xyz

interface Shape { fun area(): Double }
来源：http://abc.gaohongyu789.top

[T16] Swift：Hello World
来源：http://fjz.iojbl.cn

print("Hello")
来源：http://xrn.sxryk.cn

[T17] Swift：变量与常量
来源：http://fza.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://wuw.tanke756.top

[T18] Swift：字符串插值
来源：http://tox.zdbjq.cn

"值: \(b)"
来源：http://xyl.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://ydp.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://njy.gogol.net.cn

[T20] Swift：数组操作
来源：http://lqz.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://vbo.hesvh.cn

[T21] Swift：遍历
来源：http://jpf.ybcxt.top

for x in a { print(x) }
来源：http://zwv.jiagoushi.top

[T22] Swift：字典
来源：http://jpy.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uau.mhx1999.top

[T23] Swift：函数
来源：http://gwz.chenjidiqi.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fyo.dianchejie.cn

[T24] Swift：闭包
来源：http://wjx.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lqo.andypj.xyz

[T25] Swift：结构体
来源：http://aps.shanyushiyangtech.top

struct P { var x: Int }
来源：http://jkv.zycfv.cn

[T26] Swift：类与重写
来源：http://air.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://men.nanxuanxn.top


<!-- 参考信息 -->