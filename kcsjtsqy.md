代发 wailian999

case "$1" in
来源：http://tnx.shuidangran.top

start) echo "启动" ;;
来源：http://wcp.hnqzz.top

stop)  echo "停止" ;;
来源：http://fgs.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://ryi.havefunace.top

esac
来源：http://rxf.zycfv.cn

[R12] for 遍历文件
来源：http://bet.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://jur.zhijiandao.cn

[R13] for 计数循环
来源：http://ike.pycfn.com

for i in {1..10}; do echo "$i"; done
来源：http://vgs.jiagoushi.top

[R14] C 风格 for
来源：http://qqq.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://okw.jinqigufen.top

[R15] while 逐行读文件
来源：http://tcw.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nds.svipenyu.cn

[R16] until 等待条件
来源：http://yyi.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vqw.ydzc1.top

[R17] 数组定义与取值
来源：http://tsx.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iyj.xziqi.cn

[R18] 遍历数组
来源：http://idf.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ebn.tianlin.xyz

[R19] 数组长度
来源：http://kke.redwolf501.top

echo "${#arr[@]}"
来源：http://ryp.birdmap.top

[R20] 关联数组（字典）
来源：http://fms.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ppt.xuetiantiany.cn

[R21] 字符串长度
来源：http://wow.iojbl.cn

echo "${#s}"
来源：http://vps.ydjk.org.cn

[R22] 截取子串
来源：http://zmv.cqqwz.cn

echo "${s:0:5}"
来源：http://zug.jiagoushi.top

[R23] 字符串替换
来源：http://wnw.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uww.wangshuangyany.cn

[R24] 大小写转换
来源：http://vph.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://rip.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://iic.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kyb.zhaomingkeji.xyz

[R26] 命令替换
来源：http://gni.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://fbs.iojbl.cn

[R27] 算术展开
来源：http://tiy.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://gqx.jiagoushi.top

[R28] 浮点运算
来源：http://tse.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://aku.tian-w.cn

[R29] 定义函数
来源：http://ntn.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://stx.zhijiandao.cn

[R30] 函数返回状态码
来源：http://lqd.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://hgz.9152youxi.cn

[R31] 局部变量
来源：http://apk.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://ken.uphjek.com

[R32] 参数个数校验
来源：http://acj.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qai.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://lio.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hks.smart0.xyz

[R34] 退出时清理
来源：http://hnc.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://xnf.vqdsnc.cn

[R35] 后台执行并等待
来源：http://zgo.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lzk.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://jtx.zdqjudy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ndz.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://ytf.shangyingyoupin.top

files=$(ls -1)
来源：http://sqs.jianghu66.top

[R38] 管道串联
来源：http://uav.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://dod.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://sgd.smart0.xyz

cmd > out.log 2>&1
来源：http://lcq.zhiwuduotai.top

[R40] 追加写日志
来源：http://ucb.shangyingyoupin.top

echo "log" >> out.log
来源：http://xat.wangdashe.top

[R41] 丢弃输出
来源：http://xse.hcnkem.com

cmd >/dev/null 2>&1
来源：http://jfs.shangyingyoupin.top

[R42] 输入重定向
来源：http://dfe.chenlongwang.top

wc -l < a.txt
来源：http://vpf.cucudq.cn

[R43] 按名字查找文件
来源：http://qaw.snrcjt.cn

find . -name "*.log" -type f
来源：http://fef.svipenyu.cn

[R44] 按修改时间查找
来源：http://jij.hnxiangtu.top

find . -mtime -7 -type f
来源：http://bfv.ydzc1.top

[R45] 批量删除
来源：http://far.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://fbf.316326.xyz

[R46] 递归替换文件内容
来源：http://zgq.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fcn.ybcxt.top

[R47] sed 单行替换
来源：http://uij.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pch.gotoacloud.top

[R48] awk 取指定列
来源：http://fxu.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://jsg.yonumen.top

[R49] awk 带条件
来源：http://idi.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kzr.xylfe.cn

[R50] awk 求和
来源：http://zzd.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://brx.meibo888.top

[R51] 排序去重取前几
来源：http://qqe.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://npp.jqgfzy.top

[R52] 统计行数
来源：http://etf.jlsjyb.cn

wc -l a.txt
来源：http://xrm.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://zro.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mmb.andypj.xyz

[R54] 比较两个文件
来源：http://non.nwbrower.top

diff a.txt b.txt
来源：http://whf.yuxming.cn

[R55] 压缩与解压
来源：http://ytx.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pco.cdnleiting.top

[R56] 远程拷贝
来源：http://skw.tianlin.xyz

scp file user@host:/path/
来源：http://zco.jiagoushi.top

[R57] 远程执行命令
来源：http://gxg.jianghu66.top

ssh user@host 'uptime'
来源：http://tsu.hnxiangtu.top

[R58] 下载文件
来源：http://yhr.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eyn.yj20258.top

[R59] 发 POST JSON
来源：http://ilk.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://axl.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://bah.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbe.yanxiufei.cn

[R61] 磁盘占用
来源：http://lmx.mhx1999.top

df -h;  du -sh *
来源：http://gox.daria6918.cn

[R62] 找最占空间的文件
来源：http://zvw.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://qpo.epnwcf.com

[R63] 内存与进程
来源：http://gww.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://qvo.zdbjq.cn

[R64] 结束进程
来源：http://btn.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://cmh.yuxming.cn

[R65] 查看端口占用
来源：http://vsx.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kil.cashguo.top

[R66] 定时任务
来源：http://dak.ydzc1.top

crontab -e;  crontab -l
来源：http://muw.cheryme.top

[R67] 生成随机十六进制串
来源：http://hav.yj20258888.top

openssl rand -hex 16
来源：http://vvt.hcnkem.com

[R68] 计算文件校验值
来源：http://lix.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://egq.daxiang520.top

[R69] 生成随机密码
来源：http://whu.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://fxe.zhengqikj.top

[R70] 时间戳与互转
来源：http://twf.hcnkem.com

date +%s;  date -d @1700000000
来源：http://wwn.yuxming.cn

[R71] 日期格式化
来源：http://npq.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ahz.zdqjudy.top

[R72] 等待端口就绪
来源：http://lno.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bci.gogol.net.cn

[R73] 分割大日志
来源：http://umv.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://vug.fktsv.cn

[R74] 批量重命名
来源：http://bmj.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qdx.cqqwz.cn

[R75] 导出环境变量
来源：http://bgp.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://ffs.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://tnk.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zud.haohaochexian.top

[R77] 读取用户输入
来源：http://rvi.gaohongyu789.top

read -rp "请输入: " ans
来源：http://dwe.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://xyc.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xzn.tanke756.top

[R79] 解析命令行选项
来源：http://avh.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xjb.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://ksn.snrcjt.cn

time ./run.sh
来源：http://gkj.yueranfly.top

================================================================================
来源：http://zvp.dianchejie.cn

S. C / C++ 专题
来源：http://nex.zhiwuduotai.top

================================================================================
来源：http://jde.jianghu66.top

[S01] C：Hello World
来源：http://otk.gzhubu.top

#include <stdio.h>
来源：http://ite.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fgg.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://zfw.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://nzz.sweek.top

[S03] C：读入整数
来源：http://ppf.hysaishi.cn

int x; scanf("%d", &x);
来源：http://fwy.jqgfzy.top

[S04] C：字符串复制
来源：http://lix.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://xtc.hnxiangtu.top

[S05] C：字符串长度
来源：http://ejo.zhengqikj.top

strlen(s)
来源：http://ucv.uphjek.com

[S06] C：字符串比较
来源：http://yur.snrcjt.cn

strcmp(a, b) == 0
来源：http://whb.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://odt.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbu.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://axd.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayo.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://rdn.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vfh.cheryme.top

[S10] C：指针与解引用
来源：http://hwp.redwolf501.top

int *p = &a;  *p = 5;
来源：http://vuo.guowangkeji.top

[S11] C：逐行读文件
来源：http://fdy.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://zkf.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://flf.yj20258.top

fclose(f);
来源：http://mae.hfpthk.cn

[S12] C：写文件
来源：http://tdo.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://psh.epnwcf.com

[S13] C：宏定义
来源：http://mem.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qiq.zhaomingkeji.xyz

[S14] C：枚举
来源：http://vhl.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://jto.hysaishi.cn

[S15] C：类型转换
来源：http://pjw.zhongyouzk.top

(double) a / b
来源：http://ako.guowangkeji.top

[S16] C：位操作置位
来源：http://ocx.ctjpmb.com

x |= (1 << 3);
来源：http://hgm.birdmap.top

[S17] C：安全拼接字符串
来源：http://rkj.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://scr.yuxming.cn

[S18] C：命令行参数
来源：http://apr.mhx1999.top

int main(int argc, char **argv)
来源：http://osg.guowangkeji.top

[S19] C：快速排序
来源：http://acw.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://uzt.sysykeji.top

[S20] C：二分查找
来源：http://snb.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rrf.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://dqy.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://isb.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://vwa.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gat.jianghu66.top

[S23] C：随机数
来源：http://ptn.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://gvr.yongpay.top

[S24] C：获取本地时间
来源：http://rjp.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fgz.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://woy.zhijiandao.cn

memcpy(dst, src, n);
来源：http://jvz.gogol.net.cn

[S26] C：内存清零
来源：http://trt.iojbl.cn

memset(a, 0, sizeof a);
来源：http://qvi.daria6918.cn

[S27] C：定义常量
来源：http://pgv.gogol.net.cn

const double PI = 3.14159;
来源：http://aen.xylfe.cn

[S28] C：静态变量
来源：http://ojl.9152youxi.cn

static int counter = 0;
来源：http://zkp.chenjidiqi.icu

[S29] C：变参函数
来源：http://adu.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvg.jlsjyb.cn

[S30] C：头文件保护
来源：http://ojl.zhoulong.xyz

#ifndef X_H
来源：http://jko.fanxiaobao.xyz

#define X_H
来源：http://thw.daxiang520.top

#endif
来源：http://xjq.fengsongda.top

[S31] C++：Hello World
来源：http://xnl.kuanghao11.cn

#include <iostream>
来源：http://szf.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://voz.ppjwa.cn

[S32] C++：字符串
来源：http://bpb.uphjek.com

std::string s = "hi";  s += "!";
来源：http://puo.ybcxt.top

[S33] C++：vector 增删
来源：http://zxf.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hnw.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://xjr.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ebj.shanyushiyangkeji.top

[S35] C++：map
来源：http://qve.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://odl.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://ybx.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ycb.havefunace.top

[S37] C++：set
来源：http://kwr.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://svk.yuxming.cn

[S38] C++：排序
来源：http://yfq.havefunace.top

std::sort(v.begin(), v.end());
来源：http://jyb.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://dud.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hnd.yueranfly.top

[S40] C++：查找元素
来源：http://nrz.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wdz.nanxinkj.top

[S41] C++：类与构造函数
来源：http://lrw.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vgs.zdbjq.cn

[S42] C++：继承与虚函数
来源：http://mkn.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://hbb.chenzaomai.com

[S43] C++：智能指针
来源：http://psh.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://sve.9152youxi.cn

[S44] C++：引用传参
来源：http://uhk.epnwcf.com

void inc(int &x) { ++x; }
来源：http://kbe.yvedp.cn

[S45] C++：lambda
来源：http://bfy.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://iax.hongshengwenyu.top

[S46] C++：函数模板
来源：http://iia.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fuy.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://jhd.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qkw.nwbrower.top

[S48] C++：逐行读文件
来源：http://vuw.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://owt.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://tvo.aizwys.cn

[S49] C++：写文件
来源：http://rej.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://src.meibo888.top

[S50] C++：格式化数字
来源：http://wif.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sly.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://pdj.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://wzj.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://zgy.yonumen.top

int size() const noexcept { return n_; }
来源：http://xev.nwbrower.top

[S53] C++：移动语义
来源：http://nlw.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://hdr.ydjk.org.cn

[S54] C++：异常处理
来源：http://czj.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzz.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://lgy.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dxq.yj202588.top

[S56] C++：optional
来源：http://drz.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://joo.svipenyu.cn

[S57] C++：编译期常量
来源：http://lhk.daria6918.cn

constexpr int N = 10;
来源：http://yid.zhoulong.xyz

[S58] C++：命名空间
来源：http://par.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://qja.tianlin.xyz

[S59] C++：静态断言
来源：http://isj.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://opm.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://kmz.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lnf.c1oappe.top

================================================================================
来源：http://vaf.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kpj.jiagoushi.top

================================================================================
来源：http://ecb.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://chs.guowangkeji.top

println("Hello")
来源：http://zej.redwolf501.top

[T02] Kotlin：变量
来源：http://qhl.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mgh.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://osb.hysaishi.cn

"值: $b"
来源：http://rlb.hysaishi.cn

[T04] Kotlin：空安全
来源：http://ezk.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://zch.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://xmk.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsf.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://trb.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xst.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://gnb.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzd.ehwqpu.com

[T08] Kotlin：数据类
来源：http://idk.pycfn.com

data class User(val name: String, val age: Int)
来源：http://drw.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://cpw.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://mur.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://hot.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iyk.daria6918.cn

[T11] Kotlin：协程
来源：http://dwa.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cue.yueranfly.top

[T12] Kotlin：解构声明
来源：http://axh.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://bel.gzhubu.top


<!-- 参考信息 -->