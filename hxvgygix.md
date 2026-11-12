代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://vki.9152youxi.cn

[R18] 遍历数组
来源：http://aay.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fgw.tarul.cn

[R19] 数组长度
来源：http://uup.ybcxt.top

echo "${#arr[@]}"
来源：http://aaa.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://czv.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pbg.jianghu66.top

[R21] 字符串长度
来源：http://vms.shangyingyoupin.top

echo "${#s}"
来源：http://gwn.quarkkingdee.top

[R22] 截取子串
来源：http://yob.bbcook.cn

echo "${s:0:5}"
来源：http://ekz.pengpengdd.cyou

[R23] 字符串替换
来源：http://mox.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vav.gaohongyu789.top

[R24] 大小写转换
来源：http://dpw.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://ybz.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://dkj.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gvz.jinyuanbaomall.cn

[R26] 命令替换
来源：http://gzn.cashguo.top

now=$(date +%F); echo "$now"
来源：http://ybq.316326.xyz

[R27] 算术展开
来源：http://xqq.316326.xyz

echo $((1 + 2 * 3))
来源：http://qmx.sweek.top

[R28] 浮点运算
来源：http://onc.fehbvm.com

echo "scale=2; 10/3" | bc
来源：http://xni.snrcjt.cn

[R29] 定义函数
来源：http://nlx.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dsu.yuxming.cn

[R30] 函数返回状态码
来源：http://ngu.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://mud.jqgufenzy.top

[R31] 局部变量
来源：http://pzi.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://yla.yvedp.cn

[R32] 参数个数校验
来源：http://xql.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://akx.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://zzf.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hip.daria6918.cn

[R34] 退出时清理
来源：http://mvi.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://cbk.ydjk.org.cn

[R35] 后台执行并等待
来源：http://jil.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yfd.jqgfzy.top

[R36] 并发执行多个任务
来源：http://gol.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://exi.dashuyun.cn

[R37] 把输出赋给变量
来源：http://nxc.vehdjk.com

files=$(ls -1)
来源：http://wqb.fanxiaobao.xyz

[R38] 管道串联
来源：http://xyg.ivvv.top

cat a.txt | grep -i error | wc -l
来源：http://cnc.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://zdm.xziqi.cn

cmd > out.log 2>&1
来源：http://vzb.quarkkingdee.top

[R40] 追加写日志
来源：http://wut.zhijiandao.cn

echo "log" >> out.log
来源：http://wzk.hnxiangtu.top

[R41] 丢弃输出
来源：http://icy.sweek.top

cmd >/dev/null 2>&1
来源：http://bkh.tarul.cn

[R42] 输入重定向
来源：http://cwy.sufxvd.cn

wc -l < a.txt
来源：http://xti.hfpthk.cn

[R43] 按名字查找文件
来源：http://qrh.mhx1999.top

find . -name "*.log" -type f
来源：http://gsk.xinyue.icu

[R44] 按修改时间查找
来源：http://ial.quarkkingdee.top

find . -mtime -7 -type f
来源：http://vat.daria6918.cn

[R45] 批量删除
来源：http://adm.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://jdy.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://rua.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://prq.sweek.top

[R47] sed 单行替换
来源：http://rlj.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xkv.svipenyu.cn

[R48] awk 取指定列
来源：http://wwg.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://ner.jlsjyb.cn

[R49] awk 带条件
来源：http://psw.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kql.vqdsnc.cn

[R50] awk 求和
来源：http://dbq.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://yko.c1oappe.top

[R51] 排序去重取前几
来源：http://jca.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zxn.c1oappe.top

[R52] 统计行数
来源：http://wga.sysykeji.top

wc -l a.txt
来源：http://rqm.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://hpt.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rnj.fengsongda.top

[R54] 比较两个文件
来源：http://con.aibaodan.cn

diff a.txt b.txt
来源：http://isv.ppjwa.cn

[R55] 压缩与解压
来源：http://fsg.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gkk.hnqzz.top

[R56] 远程拷贝
来源：http://ywk.ppjwa.cn

scp file user@host:/path/
来源：http://pyd.quarkkingdee.top

[R57] 远程执行命令
来源：http://hlf.ctjpmb.com

ssh user@host 'uptime'
来源：http://mcg.yonumen.top

[R58] 下载文件
来源：http://lhf.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uob.epnwcf.com

[R59] 发 POST JSON
来源：http://wun.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ixe.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://jdn.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vot.hongshengwenyu.top

[R61] 磁盘占用
来源：http://ron.nwbrower.top

df -h;  du -sh *
来源：http://qfx.tianlin.xyz

[R62] 找最占空间的文件
来源：http://znz.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://rrj.havefunace.top

[R63] 内存与进程
来源：http://ati.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://ptz.hfpthk.cn

[R64] 结束进程
来源：http://bdp.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://gwy.epnwcf.com

[R65] 查看端口占用
来源：http://urs.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ehm.yuxming.cn

[R66] 定时任务
来源：http://rjn.birdmap.top

crontab -e;  crontab -l
来源：http://sps.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://gib.yfazqb.com

openssl rand -hex 16
来源：http://wtv.snrcjt.cn

[R68] 计算文件校验值
来源：http://apr.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nxh.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://rjh.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://nou.nwbrower.top

[R70] 时间戳与互转
来源：http://our.yuxming.cn

date +%s;  date -d @1700000000
来源：http://cfa.gotoacloud.top

[R71] 日期格式化
来源：http://tli.zdqjudy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cqk.nanxuanxn.top

[R72] 等待端口就绪
来源：http://nog.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sah.zdbjq.cn

[R73] 分割大日志
来源：http://dnr.pycfn.com

split -l 1000 big.log part_
来源：http://kuv.yanxiufei.cn

[R74] 批量重命名
来源：http://btf.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vmk.ydzc1.top

[R75] 导出环境变量
来源：http://iob.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://nhw.dashuyun.cn

[R76] 使用临时文件
来源：http://kpr.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xao.yueranfly.top

[R77] 读取用户输入
来源：http://fal.ivvv.top

read -rp "请输入: " ans
来源：http://dqa.fktsv.cn

[R78] 交互式菜单
来源：http://env.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://prg.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://ufo.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ndu.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://tbr.meibo888.top

time ./run.sh
来源：http://rfy.xuanzx.com

================================================================================
来源：http://qjd.epnwcf.com

S. C / C++ 专题
来源：http://fcm.zdbjq.cn

================================================================================
来源：http://grz.zhixingplan.top

[S01] C：Hello World
来源：http://qya.hysaishi.cn

#include <stdio.h>
来源：http://fsf.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ope.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://bfu.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://pzb.shzxlz.cn

[S03] C：读入整数
来源：http://fqv.mhx1999.top

int x; scanf("%d", &x);
来源：http://bdm.zhijiandao.cn

[S04] C：字符串复制
来源：http://xtb.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ziy.fktsv.cn

[S05] C：字符串长度
来源：http://zgj.hysaishi.cn

strlen(s)
来源：http://ngl.xinyue.icu

[S06] C：字符串比较
来源：http://fxc.316326.xyz

strcmp(a, b) == 0
来源：http://wyc.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://nxz.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nbi.tanke756.top

[S08] C：动态内存分配与释放
来源：http://biz.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rrj.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://ney.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ceq.ybcxt.top

[S10] C：指针与解引用
来源：http://rvy.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://xnq.jlsjyb.cn

[S11] C：逐行读文件
来源：http://gsr.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://trq.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mlw.ppjwa.cn

fclose(f);
来源：http://qoh.hfpthk.cn

[S12] C：写文件
来源：http://qmw.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bmj.wangdashe.top

[S13] C：宏定义
来源：http://tgd.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ygu.haohaochexian.top

[S14] C：枚举
来源：http://ofx.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://kgs.ybcxt.top

[S15] C：类型转换
来源：http://voj.ybcxt.top

(double) a / b
来源：http://idv.zdqjudy.top

[S16] C：位操作置位
来源：http://kwj.xylfe.cn

x |= (1 << 3);
来源：http://roa.52xcode.cn

[S17] C：安全拼接字符串
来源：http://bsp.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://arl.tanke756.top

[S18] C：命令行参数
来源：http://avp.yj202588.top

int main(int argc, char **argv)
来源：http://xwh.xinyue.icu

[S19] C：快速排序
来源：http://fhn.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://kvj.jyoumei.cn

[S20] C：二分查找
来源：http://laz.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eeb.yanxiufei.cn

[S21] C：字符类别判断
来源：http://zku.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://skd.andypj.xyz

[S22] C：字符串转数字
来源：http://hgf.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://zew.dashuyun.cn

[S23] C：随机数
来源：http://uen.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uxt.haohaochexian.top

[S24] C：获取本地时间
来源：http://hhv.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aen.yj20258.top

[S25] C：内存拷贝
来源：http://jfj.jqgufenzy.top

memcpy(dst, src, n);
来源：http://dkk.ydzc1.top

[S26] C：内存清零
来源：http://grn.redwolf501.top

memset(a, 0, sizeof a);
来源：http://etn.haohaochexian.top

[S27] C：定义常量
来源：http://tmz.yfazqb.com

const double PI = 3.14159;
来源：http://gdb.tanke756.top

[S28] C：静态变量
来源：http://msw.nwbrower.top

static int counter = 0;
来源：http://rhi.sjlbkw.cn

[S29] C：变参函数
来源：http://liq.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mlo.nwbrower.top

[S30] C：头文件保护
来源：http://mpy.gzhubu.top

#ifndef X_H
来源：http://xtn.zhijiandao.cn

#define X_H
来源：http://eys.9152youxi.cn

#endif
来源：http://byf.jinqigufen.top

[S31] C++：Hello World
来源：http://fvc.zdqjudy.top

#include <iostream>
来源：http://yly.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://vgv.sysykeji.top

[S32] C++：字符串
来源：http://iqx.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://fhm.ctjpmb.com

[S33] C++：vector 增删
来源：http://xkh.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bck.yfazqb.com

[S34] C++：遍历 vector
来源：http://rbq.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://xpr.zdqjudy.top

[S35] C++：map
来源：http://sin.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bgp.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://uqp.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pai.hongshengwenyu.top

[S37] C++：set
来源：http://jod.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ore.ivvv.top

[S38] C++：排序
来源：http://tbg.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://gzv.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://jhi.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kpf.dianchejie.cn

[S40] C++：查找元素
来源：http://wzw.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://soo.dianchejie.cn

[S41] C++：类与构造函数
来源：http://eqj.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vok.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://vfi.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://shs.cashguo.top

[S43] C++：智能指针
来源：http://hrs.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://evh.sufxvd.cn

[S44] C++：引用传参
来源：http://hks.daxiang520.top

void inc(int &x) { ++x; }
来源：http://lze.xinyue.icu

[S45] C++：lambda
来源：http://fgj.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://wdl.sufxvd.cn

[S46] C++：函数模板
来源：http://ozq.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fmw.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://vrb.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://shb.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://btl.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vjn.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://fpj.bbcook.cn

[S49] C++：写文件
来源：http://qps.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mcb.tianlin.xyz

[S50] C++：格式化数字
来源：http://dye.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ixj.yfazqb.com

[S51] C++：显式类型转换
来源：http://vye.mhx1999.top

static_cast<double>(a) / b
来源：http://xua.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://uxk.hesvh.cn

int size() const noexcept { return n_; }
来源：http://jfk.ydjk.org.cn

[S53] C++：移动语义
来源：http://ukc.cashguo.top

std::vector<int> w = std::move(v);
来源：http://nwq.yj20258.top

[S54] C++：异常处理
来源：http://gcs.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvs.uphjek.com

[S55] C++：结构化绑定
来源：http://jek.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://spi.jiagoushi.top

[S56] C++：optional
来源：http://nhb.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bxk.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://aut.jyoumei.cn

constexpr int N = 10;
来源：http://fcl.tianlin.xyz

[S58] C++：命名空间
来源：http://xvq.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://rxj.chenlongwang.top

[S59] C++：静态断言
来源：http://qoa.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rmm.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://sxf.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yes.sufxvd.cn

================================================================================
来源：http://utg.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lkk.jqgfzy.top

================================================================================
来源：http://jbw.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://kyn.vqdsnc.cn

println("Hello")
来源：http://omr.uphjek.com

[T02] Kotlin：变量
来源：http://qjd.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mwf.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://ghb.daria6918.cn

"值: $b"
来源：http://hpi.zdqjudy.top

[T04] Kotlin：空安全
来源：http://afm.wangdashe.top

val n: String? = null;  n?.length
来源：http://qxs.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://vqn.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bdn.cheryme.top

[T06] Kotlin：集合映射
来源：http://bto.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mxb.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://kvn.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sys.cdnleiting.top

[T08] Kotlin：数据类
来源：http://eky.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://yor.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://owj.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://lsn.316326.xyz

[T10] Kotlin：默认参数
来源：http://pdb.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://sno.cashguo.top

[T11] Kotlin：协程
来源：http://xdy.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lar.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://nnj.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://hob.tanke756.top

[T13] Kotlin：只读 Map
来源：http://ome.jianghu66.top

val m = mapOf("a" to 1)
来源：http://txu.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://bwy.jianghu66.top

for (i in 1..10) println(i)
来源：http://duh.nwbrower.top

[T15] Kotlin：接口
来源：http://dcn.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://crh.haohaochexian.top

[T16] Swift：Hello World
来源：http://mcy.chenzaomai.com

print("Hello")
来源：http://ejo.bjfxy.top

[T17] Swift：变量与常量
来源：http://vtd.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://eoa.nanxinkj.top

[T18] Swift：字符串插值
来源：http://cfk.gaohongyu789.top

"值: \(b)"
来源：http://sor.chenjidiqi.icu

[T19] Swift：可选绑定
来源：http://gkb.zdbjq.cn

if let n = opt { print(n) }
来源：http://kpc.yueranfly.top

[T20] Swift：数组操作
来源：http://bba.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aom.chenjidiqi.icu


<!-- 参考信息 -->