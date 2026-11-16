代发 wailian999

case "$1" in
来源：http://nns.yangfankeji.com

start) echo "启动" ;;
来源：http://dpy.aibaodan.cn

stop)  echo "停止" ;;
来源：http://boe.guannengcc.top

*)     echo "未知命令" ;;
来源：http://mpl.zhijiandao.cn

esac
来源：http://ykr.yvedp.cn

[R12] for 遍历文件
来源：http://xgx.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://uer.bjfxy.top

[R13] for 计数循环
来源：http://zhx.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://ksi.gogol.net.cn

[R14] C 风格 for
来源：http://jls.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sdb.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://ara.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://psw.fanxiaobao.xyz

[R16] until 等待条件
来源：http://cel.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fok.dianchejie.cn

[R17] 数组定义与取值
来源：http://naj.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://ber.chenzaomai.com

[R18] 遍历数组
来源：http://ire.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iil.jqgufenzy.top

[R19] 数组长度
来源：http://sfi.jqgufenzy.top

echo "${#arr[@]}"
来源：http://mjm.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://sra.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://knl.9152youxi.cn

[R21] 字符串长度
来源：http://jbp.xingfuxueyuan.xyz

echo "${#s}"
来源：http://zfy.ehwqpu.com

[R22] 截取子串
来源：http://tib.dashuyun.cn

echo "${s:0:5}"
来源：http://mqa.fzhhl.top

[R23] 字符串替换
来源：http://uta.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vas.hnxiangtu.top

[R24] 大小写转换
来源：http://ylf.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://dir.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://map.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rhp.zdbjq.cn

[R26] 命令替换
来源：http://jee.tanke756.top

now=$(date +%F); echo "$now"
来源：http://gtf.hesvh.cn

[R27] 算术展开
来源：http://try.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://rey.hcnkem.com

[R28] 浮点运算
来源：http://kmz.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://imq.jlsjyb.cn

[R29] 定义函数
来源：http://mzt.fehbvm.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hqt.cdnleiting.top

[R30] 函数返回状态码
来源：http://heq.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://njx.hammf.cn

[R31] 局部变量
来源：http://kmx.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://ubb.wangshuangyany.cn

[R32] 参数个数校验
来源：http://ibj.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://joz.aizwys.cn

[R33] 捕获错误并提示行号
来源：http://lne.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fyw.fanxiaobao.xyz

[R34] 退出时清理
来源：http://otb.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://ilk.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://zse.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://msn.jinqigufen.top

[R36] 并发执行多个任务
来源：http://esv.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rls.guannengcc.top

[R37] 把输出赋给变量
来源：http://jnf.gotoacloud.top

files=$(ls -1)
来源：http://qzv.bjfxy.top

[R38] 管道串联
来源：http://baw.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://rup.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://gus.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://oeq.yanxiufei.cn

[R40] 追加写日志
来源：http://dcx.zdbjq.cn

echo "log" >> out.log
来源：http://zhi.cashguo.top

[R41] 丢弃输出
来源：http://ikz.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://upc.guowangkeji.top

[R42] 输入重定向
来源：http://eqd.hfpthk.cn

wc -l < a.txt
来源：http://fzu.ivvv.top

[R43] 按名字查找文件
来源：http://grt.yueranfly.top

find . -name "*.log" -type f
来源：http://sbb.xziqi.cn

[R44] 按修改时间查找
来源：http://oxy.sysykeji.top

find . -mtime -7 -type f
来源：http://pxb.ydzc1.top

[R45] 批量删除
来源：http://pve.hcnkem.com

find . -name "*.tmp" -delete
来源：http://erm.bjfxy.top

[R46] 递归替换文件内容
来源：http://pzg.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qma.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://anb.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://lxm.zhongyouzk.top

[R48] awk 取指定列
来源：http://lsk.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://uvb.yuxming.cn

[R49] awk 带条件
来源：http://vqs.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mwg.bbcook.cn

[R50] awk 求和
来源：http://qgu.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://sbs.ctjpmb.com

[R51] 排序去重取前几
来源：http://fes.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nci.smart0.xyz

[R52] 统计行数
来源：http://qrd.haohaochexian.top

wc -l a.txt
来源：http://bsq.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://rqh.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bqz.uphjek.com

[R54] 比较两个文件
来源：http://lgu.316326.xyz

diff a.txt b.txt
来源：http://rau.gaohongyu789.top

[R55] 压缩与解压
来源：http://wzi.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://adb.dianchejie.cn

[R56] 远程拷贝
来源：http://svs.aibaodan.cn

scp file user@host:/path/
来源：http://rpl.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://fvw.tianlin.xyz

ssh user@host 'uptime'
来源：http://dqu.sweek.top

[R58] 下载文件
来源：http://fjr.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xuz.yueranfly.top

[R59] 发 POST JSON
来源：http://zbi.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zyq.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://jvm.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gej.chenzaomai.com

[R61] 磁盘占用
来源：http://baf.ivvv.top

df -h;  du -sh *
来源：http://bvq.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://huf.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://row.xuanzx.com

[R63] 内存与进程
来源：http://dxa.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://slg.pengpengdd.cyou

[R64] 结束进程
来源：http://vki.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://jqn.yj202588.top

[R65] 查看端口占用
来源：http://xen.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wti.chenzaomai.com

[R66] 定时任务
来源：http://zzk.hywenlv.cn

crontab -e;  crontab -l
来源：http://afh.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://zcl.tianlin.xyz

openssl rand -hex 16
来源：http://gcf.jqgfzy.top

[R68] 计算文件校验值
来源：http://ymj.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pkb.redwolf501.top

[R69] 生成随机密码
来源：http://jgh.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://yag.yj20258888.top

[R70] 时间戳与互转
来源：http://ncs.wangdashe.top

date +%s;  date -d @1700000000
来源：http://pwm.andypj.xyz

[R71] 日期格式化
来源：http://svy.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpe.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://jrk.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wjx.quarkkingdee.top

[R73] 分割大日志
来源：http://lbl.daxiang520.top

split -l 1000 big.log part_
来源：http://ytb.xuetiantiany.cn

[R74] 批量重命名
来源：http://ira.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yjn.yj202588.top

[R75] 导出环境变量
来源：http://lvg.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://lti.birdmap.top

[R76] 使用临时文件
来源：http://gqz.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fdq.sufxvd.cn

[R77] 读取用户输入
来源：http://oek.fzhhl.top

read -rp "请输入: " ans
来源：http://cut.sweek.top

[R78] 交互式菜单
来源：http://wmz.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dft.ybcxt.top

[R79] 解析命令行选项
来源：http://bcq.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fvf.cashguo.top

[R80] 查看脚本执行耗时
来源：http://yan.yfazqb.com

time ./run.sh
来源：http://hdc.yj20258.top

================================================================================
来源：http://mgh.sufxvd.cn

S. C / C++ 专题
来源：http://xoq.daria6918.cn

================================================================================
来源：http://cyw.jqgfzy.top

[S01] C：Hello World
来源：http://qhv.fanxiaobao.xyz

#include <stdio.h>
来源：http://hco.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iio.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://ybr.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://cmw.yongpay.top

[S03] C：读入整数
来源：http://awl.zdbjq.cn

int x; scanf("%d", &x);
来源：http://lrr.zhengqikj.top

[S04] C：字符串复制
来源：http://mrh.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zzg.mhx1999.top

[S05] C：字符串长度
来源：http://jqp.cqqwz.cn

strlen(s)
来源：http://bak.dashuyun.cn

[S06] C：字符串比较
来源：http://ukk.haohaochexian.top

strcmp(a, b) == 0
来源：http://ijw.xylfe.cn

[S07] C：数组遍历求和
来源：http://geg.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ntc.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://vos.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yww.yonumen.top

[S09] C：结构体定义与初始化
来源：http://vze.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tyx.daxiang520.top

[S10] C：指针与解引用
来源：http://wfn.tian-w.cn

int *p = &a;  *p = 5;
来源：http://jmd.ydzc1.top

[S11] C：逐行读文件
来源：http://dck.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://urj.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kil.mhx1999.top

fclose(f);
来源：http://ivj.cashguo.top

[S12] C：写文件
来源：http://grg.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://epe.bbcook.cn

[S13] C：宏定义
来源：http://qqa.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tnm.316326.xyz

[S14] C：枚举
来源：http://ylp.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://emn.vqdsnc.cn

[S15] C：类型转换
来源：http://tvt.chenzaomai.com

(double) a / b
来源：http://mrp.jinqigfzy.top

[S16] C：位操作置位
来源：http://pyb.wangdashe.top

x |= (1 << 3);
来源：http://jns.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://ymw.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ema.bjfxy.top

[S18] C：命令行参数
来源：http://jlt.tianlin.xyz

int main(int argc, char **argv)
来源：http://vmg.316326.xyz

[S19] C：快速排序
来源：http://fad.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ree.316326.xyz

[S20] C：二分查找
来源：http://hsh.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hob.yj202588.top

[S21] C：字符类别判断
来源：http://ldb.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dij.tarul.cn

[S22] C：字符串转数字
来源：http://zsm.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://grr.sjlbkw.cn

[S23] C：随机数
来源：http://oui.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zfk.iojbl.cn

[S24] C：获取本地时间
来源：http://waf.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://csw.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://kuk.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://yss.ehwqpu.com

[S26] C：内存清零
来源：http://mte.iojbl.cn

memset(a, 0, sizeof a);
来源：http://qwj.hnxiangtu.top

[S27] C：定义常量
来源：http://rgi.yongpay.top

const double PI = 3.14159;
来源：http://fxv.hnqzz.top

[S28] C：静态变量
来源：http://ulr.jianghu66.top

static int counter = 0;
来源：http://jsx.yanxiufei.cn

[S29] C：变参函数
来源：http://pqq.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://why.hnqzz.top

[S30] C：头文件保护
来源：http://duj.tian-w.cn

#ifndef X_H
来源：http://iqk.birdmap.top

#define X_H
来源：http://rzl.fanxiaobao.xyz

#endif
来源：http://xur.xuetiantiany.cn

[S31] C++：Hello World
来源：http://eew.yanxiufei.cn

#include <iostream>
来源：http://bza.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://zjc.quarkkingdee.top

[S32] C++：字符串
来源：http://qez.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://lft.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://qrh.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vxf.yueranfly.top

[S34] C++：遍历 vector
来源：http://wui.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://pfk.redwolf501.top

[S35] C++：map
来源：http://zco.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://euf.yj20258888.top

[S36] C++：unordered_map
来源：http://oxa.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gks.svipenyu.cn

[S37] C++：set
来源：http://ezp.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rrr.yj20258.top

[S38] C++：排序
来源：http://asb.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://syj.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://huk.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ahz.fktsv.cn

[S40] C++：查找元素
来源：http://ipd.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rjt.cheryme.top

[S41] C++：类与构造函数
来源：http://nas.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qht.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://fmc.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://stj.mhx1999.top

[S43] C++：智能指针
来源：http://ion.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://gce.yfazqb.com

[S44] C++：引用传参
来源：http://plc.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://uxs.fzhhl.top

[S45] C++：lambda
来源：http://eaj.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://xlt.gogol.net.cn

[S46] C++：函数模板
来源：http://hhz.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cup.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://okn.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxn.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://szi.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ney.birdmap.top

while (std::getline(in, line)) { }
来源：http://ewj.yongpay.top

[S49] C++：写文件
来源：http://vdo.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hcg.ehwqpu.com

[S50] C++：格式化数字
来源：http://woi.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ibs.aibaodan.cn

[S51] C++：显式类型转换
来源：http://alx.cashguo.top

static_cast<double>(a) / b
来源：http://ybq.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://yqh.hnqzz.top

int size() const noexcept { return n_; }
来源：http://bot.cdnleiting.top

[S53] C++：移动语义
来源：http://fgx.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://pvz.jqgfzy.top

[S54] C++：异常处理
来源：http://zxb.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://byn.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://uye.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iyc.zhijiandao.cn

[S56] C++：optional
来源：http://udd.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pfs.ybcxt.top

[S57] C++：编译期常量
来源：http://fjo.sufxvd.cn

constexpr int N = 10;
来源：http://vou.yonumen.top

[S58] C++：命名空间
来源：http://tpi.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://wup.9152youxi.cn

[S59] C++：静态断言
来源：http://phx.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vic.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://qna.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dzu.hesvh.cn

================================================================================
来源：http://fjl.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tll.hfpthk.cn

================================================================================
来源：http://eow.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://prd.feifeiyinyue.top

println("Hello")
来源：http://fgj.316326.xyz

[T02] Kotlin：变量
来源：http://cyj.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gcv.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://izg.gogol.net.cn

"值: $b"
来源：http://tql.yonumen.top

[T04] Kotlin：空安全
来源：http://xdx.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://rcf.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://wvt.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ung.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://zio.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xnx.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://qvu.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wdj.bjfxy.top

[T08] Kotlin：数据类
来源：http://cwa.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://arj.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://pno.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://ggb.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://ydc.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lnv.tian-w.cn

[T11] Kotlin：协程
来源：http://rpk.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hun.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://qlq.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://dqm.tanke756.top


<!-- 参考信息 -->