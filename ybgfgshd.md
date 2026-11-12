代发 wailian999

case "$1" in
来源：http://doz.andypj.xyz

start) echo "启动" ;;
来源：http://vgr.havefunace.top

stop)  echo "停止" ;;
来源：http://ura.xuanzx.com

*)     echo "未知命令" ;;
来源：http://pzq.cheryme.top

esac
来源：http://rlq.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://bqi.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://awk.zhoulong.xyz

[R13] for 计数循环
来源：http://hxr.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://uho.epnwcf.com

[R14] C 风格 for
来源：http://azk.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yav.yuanzhike.top

[R15] while 逐行读文件
来源：http://mmt.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wqd.epnwcf.com

[R16] until 等待条件
来源：http://ako.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nzm.shuidangran.top

[R17] 数组定义与取值
来源：http://szh.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://azz.aibaodan.cn

[R18] 遍历数组
来源：http://vsq.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bat.ydzc1.top

[R19] 数组长度
来源：http://jbe.shzxlz.cn

echo "${#arr[@]}"
来源：http://kks.epnwcf.com

[R20] 关联数组（字典）
来源：http://uey.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fld.gzhubu.top

[R21] 字符串长度
来源：http://hca.havefunace.top

echo "${#s}"
来源：http://ifa.gogol.net.cn

[R22] 截取子串
来源：http://scb.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://fdp.sjlbkw.cn

[R23] 字符串替换
来源：http://jvr.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ogj.nanxinkj.top

[R24] 大小写转换
来源：http://zem.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://qja.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://tvk.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pmb.zhixingplan.top

[R26] 命令替换
来源：http://qbw.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://rex.zdbjq.cn

[R27] 算术展开
来源：http://gdh.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://chw.nanxinkj.top

[R28] 浮点运算
来源：http://ytz.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://unz.meibo888.top

[R29] 定义函数
来源：http://mbw.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iuw.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://wzd.zhijiandao.cn

f() { return 0; }; f || echo "失败了"
来源：http://mzc.tarul.cn

[R31] 局部变量
来源：http://xhn.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://yao.yuxming.cn

[R32] 参数个数校验
来源：http://bcd.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qzp.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://kez.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://coz.zhijiandao.cn

[R34] 退出时清理
来源：http://qmx.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://oyq.fzhhl.top

[R35] 后台执行并等待
来源：http://joc.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bqd.cdnleiting.top

[R36] 并发执行多个任务
来源：http://qwm.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zhq.yj20258.top

[R37] 把输出赋给变量
来源：http://bvp.kuanghao11.cn

files=$(ls -1)
来源：http://pqn.tian-w.cn

[R38] 管道串联
来源：http://xmy.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://dqw.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://czv.sjlbkw.cn

cmd > out.log 2>&1
来源：http://ifq.sysykeji.top

[R40] 追加写日志
来源：http://mzo.jinqigufen.top

echo "log" >> out.log
来源：http://nig.yuxming.cn

[R41] 丢弃输出
来源：http://xsn.fengsongda.top

cmd >/dev/null 2>&1
来源：http://ubd.ivvv.top

[R42] 输入重定向
来源：http://paj.zhengqikj.top

wc -l < a.txt
来源：http://tvo.bbcook.cn

[R43] 按名字查找文件
来源：http://cof.uphjek.com

find . -name "*.log" -type f
来源：http://ifg.tanke756.top

[R44] 按修改时间查找
来源：http://cdr.xziqi.cn

find . -mtime -7 -type f
来源：http://rxa.xinyue.icu

[R45] 批量删除
来源：http://bim.redwolf501.top

find . -name "*.tmp" -delete
来源：http://gvz.dashuyun.cn

[R46] 递归替换文件内容
来源：http://uiq.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ffp.jinqigufen.top

[R47] sed 单行替换
来源：http://avk.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://bml.gaohongyu789.top

[R48] awk 取指定列
来源：http://ohh.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://whg.fzhhl.top

[R49] awk 带条件
来源：http://tjh.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://exn.yueranfly.top

[R50] awk 求和
来源：http://ihn.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dfv.jlsjyb.cn

[R51] 排序去重取前几
来源：http://jnt.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://whd.smart0.xyz

[R52] 统计行数
来源：http://mpl.ctjpmb.com

wc -l a.txt
来源：http://pvo.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://hou.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fmz.iojbl.cn

[R54] 比较两个文件
来源：http://gkf.hnqzz.top

diff a.txt b.txt
来源：http://msd.gotoacloud.top

[R55] 压缩与解压
来源：http://ewp.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gei.xylfe.cn

[R56] 远程拷贝
来源：http://rfw.yj20258.top

scp file user@host:/path/
来源：http://oic.redwolf501.top

[R57] 远程执行命令
来源：http://ded.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://qgx.tianlin.xyz

[R58] 下载文件
来源：http://ecx.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wzl.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://qwh.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xhu.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://ady.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zgd.9152youxi.cn

[R61] 磁盘占用
来源：http://jin.hfpthk.cn

df -h;  du -sh *
来源：http://ddp.tanke756.top

[R62] 找最占空间的文件
来源：http://fkd.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://awj.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://shj.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://oha.yueranfly.top

[R64] 结束进程
来源：http://ila.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://vme.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://ibl.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ywn.uphjek.com

[R66] 定时任务
来源：http://gpo.uphjek.com

crontab -e;  crontab -l
来源：http://ngo.uphjek.com

[R67] 生成随机十六进制串
来源：http://bmc.xuetiantiany.cn

openssl rand -hex 16
来源：http://emy.smart0.xyz

[R68] 计算文件校验值
来源：http://qfs.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bxk.redwolf501.top

[R69] 生成随机密码
来源：http://djn.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://yme.fengsongda.top

[R70] 时间戳与互转
来源：http://its.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://xhr.ydjk.org.cn

[R71] 日期格式化
来源：http://obp.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hgh.sjlbkw.cn

[R72] 等待端口就绪
来源：http://aaz.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://shp.nanxinkj.top

[R73] 分割大日志
来源：http://ypn.ydjk.org.cn

split -l 1000 big.log part_
来源：http://lvy.svipenyu.cn

[R74] 批量重命名
来源：http://koe.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ebj.zdqjudy.top

[R75] 导出环境变量
来源：http://bjg.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://jcz.ehwqpu.com

[R76] 使用临时文件
来源：http://nhb.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xpr.yongpay.top

[R77] 读取用户输入
来源：http://qnk.fehbvm.com

read -rp "请输入: " ans
来源：http://jnw.xylfe.cn

[R78] 交互式菜单
来源：http://sfl.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zqt.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://cpq.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://guq.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://pzy.fehbvm.com

time ./run.sh
来源：http://new.daxiang520.top

================================================================================
来源：http://lkv.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://yrz.jinghuilouyu.cn

================================================================================
来源：http://thc.svipenyu.cn

[S01] C：Hello World
来源：http://ohd.aibaodan.cn

#include <stdio.h>
来源：http://zma.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bqa.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://mum.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://req.hnxiangtu.top

[S03] C：读入整数
来源：http://usz.hnqzz.top

int x; scanf("%d", &x);
来源：http://tnx.yj20258888.top

[S04] C：字符串复制
来源：http://xsx.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hjq.jinqigfzy.top

[S05] C：字符串长度
来源：http://izl.daria6918.cn

strlen(s)
来源：http://mdd.yfazqb.com

[S06] C：字符串比较
来源：http://gaf.fzhhl.top

strcmp(a, b) == 0
来源：http://rfk.wangdashe.top

[S07] C：数组遍历求和
来源：http://zmu.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://quq.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://amc.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tud.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://ybu.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oqc.daria6918.cn

[S10] C：指针与解引用
来源：http://biv.fzhhl.top

int *p = &a;  *p = 5;
来源：http://ypx.ybcxt.top

[S11] C：逐行读文件
来源：http://ihq.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://fcw.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nma.dashuyun.cn

fclose(f);
来源：http://pcf.jinqigufen.top

[S12] C：写文件
来源：http://hhe.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rlx.aibaodan.cn

[S13] C：宏定义
来源：http://ugt.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rpy.yj20258.top

[S14] C：枚举
来源：http://rry.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://uod.yuanzhike.top

[S15] C：类型转换
来源：http://bha.jiagoushi.top

(double) a / b
来源：http://ail.tarul.cn

[S16] C：位操作置位
来源：http://voo.gotoacloud.top

x |= (1 << 3);
来源：http://lmd.cucudq.cn

[S17] C：安全拼接字符串
来源：http://hqp.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://clg.9152youxi.cn

[S18] C：命令行参数
来源：http://xyp.sjlbkw.cn

int main(int argc, char **argv)
来源：http://eqm.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://tek.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rtm.hywenlv.cn

[S20] C：二分查找
来源：http://azq.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xij.dianchejie.cn

[S21] C：字符类别判断
来源：http://ejq.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://apk.aizwys.cn

[S22] C：字符串转数字
来源：http://und.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://ptw.snrcjt.cn

[S23] C：随机数
来源：http://ufv.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://swx.ctjpmb.com

[S24] C：获取本地时间
来源：http://seu.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dzv.jqgfzy.top

[S25] C：内存拷贝
来源：http://uro.52xcode.cn

memcpy(dst, src, n);
来源：http://ipj.yangfankeji.com

[S26] C：内存清零
来源：http://kho.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://mkv.fengsongda.top

[S27] C：定义常量
来源：http://isy.jyoumei.cn

const double PI = 3.14159;
来源：http://jer.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://maq.chenzaomai.com

static int counter = 0;
来源：http://xdj.bbcook.cn

[S29] C：变参函数
来源：http://kbn.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ndu.ydjk.org.cn

[S30] C：头文件保护
来源：http://anb.xingfuxueyuan.xyz

#ifndef X_H
来源：http://ebh.gotoacloud.top

#define X_H
来源：http://rid.ivvv.top

#endif
来源：http://hzk.yangfankeji.com

[S31] C++：Hello World
来源：http://mdi.fengsongda.top

#include <iostream>
来源：http://yny.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://iol.0kj1m.cn

[S32] C++：字符串
来源：http://hof.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://rkw.nanxuanxn.top

[S33] C++：vector 增删
来源：http://meb.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ghx.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://xnu.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://imv.cqqwz.cn

[S35] C++：map
来源：http://mwi.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywo.cheryme.top

[S36] C++：unordered_map
来源：http://jtr.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kwd.zycfv.cn

[S37] C++：set
来源：http://rwx.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cbd.pengpengdd.cyou

[S38] C++：排序
来源：http://bej.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://zuw.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://pgt.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ype.zdbjq.cn

[S40] C++：查找元素
来源：http://srt.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wat.fzhhl.top

[S41] C++：类与构造函数
来源：http://rub.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ref.meibo888.top

[S42] C++：继承与虚函数
来源：http://frq.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://nxg.hammf.cn

[S43] C++：智能指针
来源：http://quk.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://irk.yuxming.cn

[S44] C++：引用传参
来源：http://rvr.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://hmy.fktsv.cn

[S45] C++：lambda
来源：http://eds.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://dhs.hysaishi.cn

[S46] C++：函数模板
来源：http://gpr.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wzn.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://uce.ivvv.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rqg.svipenyu.cn

[S48] C++：逐行读文件
来源：http://ejy.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://eey.shuidangran.top

while (std::getline(in, line)) { }
来源：http://qdm.hammf.cn

[S49] C++：写文件
来源：http://pbt.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gep.wangdashe.top

[S50] C++：格式化数字
来源：http://wcx.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jke.cashguo.top

[S51] C++：显式类型转换
来源：http://soh.hesvh.cn

static_cast<double>(a) / b
来源：http://kyk.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://dds.pycfn.com

int size() const noexcept { return n_; }
来源：http://ahx.shzxlz.cn

[S53] C++：移动语义
来源：http://rxb.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://lbp.daxiang520.top

[S54] C++：异常处理
来源：http://yfv.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kje.ctjpmb.com

[S55] C++：结构化绑定
来源：http://tfr.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://not.sjlbkw.cn

[S56] C++：optional
来源：http://jqx.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rah.jianghu66.top

[S57] C++：编译期常量
来源：http://pqw.dianchejie.cn

constexpr int N = 10;
来源：http://ktm.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://qpu.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://ndt.shangyingyoupin.top

[S59] C++：静态断言
来源：http://jpp.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jpx.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://rbw.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jpe.cashguo.top

================================================================================
来源：http://efz.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cel.yongpay.top

================================================================================
来源：http://kob.bbcook.cn

[T01] Kotlin：Hello World
来源：http://tbz.fehbvm.com

println("Hello")
来源：http://wsd.snrcjt.cn

[T02] Kotlin：变量
来源：http://jit.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fup.ivvv.top

[T03] Kotlin：字符串模板
来源：http://kpc.aizwys.cn

"值: $b"
来源：http://irf.dashuyun.cn

[T04] Kotlin：空安全
来源：http://udd.shzxlz.cn

val n: String? = null;  n?.length
来源：http://ugc.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://cew.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ylw.yfazqb.com

[T06] Kotlin：集合映射
来源：http://rsi.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mkb.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://fso.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nmc.xuanzx.com

[T08] Kotlin：数据类
来源：http://uyh.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://bxn.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://cqx.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://iau.cashguo.top

[T10] Kotlin：默认参数
来源：http://cgv.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ggs.wangdashe.top

[T11] Kotlin：协程
来源：http://qdz.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eiq.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://kjv.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://ylf.havefunace.top


<!-- 参考信息 -->