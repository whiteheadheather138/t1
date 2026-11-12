代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgn.shanyushiyangtech.top

[R08] 数值比较
来源：http://acn.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://xrv.zhaomingkeji.xyz

[R09] 字符串比较
来源：http://rvq.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://urw.ppjwa.cn

[R10] 正则匹配
来源：http://thn.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bxv.haohaochexian.top

[R11] case 多分支
来源：http://jys.daria6918.cn

case "$1" in
来源：http://qcd.chenzaomai.com

start) echo "启动" ;;
来源：http://sip.yj20258888.top

stop)  echo "停止" ;;
来源：http://snt.pycfn.com

*)     echo "未知命令" ;;
来源：http://toy.zhongyouzk.top

esac
来源：http://yxl.nanxuanxn.top

[R12] for 遍历文件
来源：http://dkn.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://zgw.yangfankeji.com

[R13] for 计数循环
来源：http://rff.feifeiyinyue.top

for i in {1..10}; do echo "$i"; done
来源：http://tvo.fehbvm.com

[R14] C 风格 for
来源：http://coo.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vse.pycfn.com

[R15] while 逐行读文件
来源：http://gng.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tbn.ydjk.org.cn

[R16] until 等待条件
来源：http://few.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://syy.smart0.xyz

[R17] 数组定义与取值
来源：http://jfu.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wvi.bbcook.cn

[R18] 遍历数组
来源：http://xus.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iik.tian-w.cn

[R19] 数组长度
来源：http://hms.hammf.cn

echo "${#arr[@]}"
来源：http://aau.svipenyu.cn

[R20] 关联数组（字典）
来源：http://tdw.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wjb.xylfe.cn

[R21] 字符串长度
来源：http://hhs.ywan-chungtsiang.top

echo "${#s}"
来源：http://bbq.316326.xyz

[R22] 截取子串
来源：http://xla.aibaodan.cn

echo "${s:0:5}"
来源：http://rmf.gzhubu.top

[R23] 字符串替换
来源：http://cak.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lrj.yonumen.top

[R24] 大小写转换
来源：http://ghb.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://gsh.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://uxd.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://tki.sysykeji.top

[R26] 命令替换
来源：http://mgp.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://tnb.epnwcf.com

[R27] 算术展开
来源：http://fky.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://rjx.havefunace.top

[R28] 浮点运算
来源：http://ktt.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://dmr.pengpengdd.cyou

[R29] 定义函数
来源：http://mox.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uph.yuanzhike.top

[R30] 函数返回状态码
来源：http://ppn.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://ltb.wangdashe.top

[R31] 局部变量
来源：http://ueb.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://oww.sweek.top

[R32] 参数个数校验
来源：http://uth.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gfr.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://unf.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://riq.fanxiaobao.xyz

[R34] 退出时清理
来源：http://twu.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://ujk.yuxming.cn

[R35] 后台执行并等待
来源：http://onr.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fny.bbcook.cn

[R36] 并发执行多个任务
来源：http://xjf.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://omt.zdbjq.cn

[R37] 把输出赋给变量
来源：http://uif.feifeiyinyue.top

files=$(ls -1)
来源：http://meo.yangfankeji.com

[R38] 管道串联
来源：http://xpf.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://lfr.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://diq.meibo888.top

cmd > out.log 2>&1
来源：http://vgu.fanxiaobao.xyz

[R40] 追加写日志
来源：http://dmf.cucudq.cn

echo "log" >> out.log
来源：http://jys.yanxiufei.cn

[R41] 丢弃输出
来源：http://pnu.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://umn.zycfv.cn

[R42] 输入重定向
来源：http://mii.chenlongwang.top

wc -l < a.txt
来源：http://nkc.zhijiandao.cn

[R43] 按名字查找文件
来源：http://xlt.fehbvm.com

find . -name "*.log" -type f
来源：http://cta.ydzc1.top

[R44] 按修改时间查找
来源：http://wmx.zdbjq.cn

find . -mtime -7 -type f
来源：http://mzh.epnwcf.com

[R45] 批量删除
来源：http://xak.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://hfi.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://bji.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gbc.zycfv.cn

[R47] sed 单行替换
来源：http://ntw.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sph.ybcxt.top

[R48] awk 取指定列
来源：http://rzj.ydjk.org.cn

awk '{print $1, $3}' a.txt
来源：http://gkd.yvedp.cn

[R49] awk 带条件
来源：http://kzx.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zod.dianchejie.cn

[R50] awk 求和
来源：http://gpw.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iot.birdmap.top

[R51] 排序去重取前几
来源：http://tyb.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cox.jinqigufen.top

[R52] 统计行数
来源：http://ljj.9152youxi.cn

wc -l a.txt
来源：http://yrp.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://qmh.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rgi.mhx1999.top

[R54] 比较两个文件
来源：http://ecn.chenjidiqi.icu

diff a.txt b.txt
来源：http://btm.jiagoushi.top

[R55] 压缩与解压
来源：http://mlh.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://afx.zdqjudy.top

[R56] 远程拷贝
来源：http://fvj.haohaochexian.top

scp file user@host:/path/
来源：http://diy.bjfxy.top

[R57] 远程执行命令
来源：http://ukj.fehbvm.com

ssh user@host 'uptime'
来源：http://reu.jiagoushi.top

[R58] 下载文件
来源：http://dui.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qwe.aizwys.cn

[R59] 发 POST JSON
来源：http://low.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfp.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://nnu.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://djx.hongshengwenyu.top

[R61] 磁盘占用
来源：http://nqz.52xcode.cn

df -h;  du -sh *
来源：http://uaj.smart0.xyz

[R62] 找最占空间的文件
来源：http://hgt.yongpay.top

du -ah . | sort -rh | head -10
来源：http://xka.zhiwuduotai.top

[R63] 内存与进程
来源：http://jug.ivvv.top

free -h;  ps aux | grep nginx
来源：http://eck.xylfe.cn

[R64] 结束进程
来源：http://hix.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://vst.gogol.net.cn

[R65] 查看端口占用
来源：http://bbd.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vig.ydzc1.top

[R66] 定时任务
来源：http://ehd.52xcode.cn

crontab -e;  crontab -l
来源：http://sbt.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://hhr.hfpthk.cn

openssl rand -hex 16
来源：http://xld.fktsv.cn

[R68] 计算文件校验值
来源：http://cfz.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vmm.uphjek.com

[R69] 生成随机密码
来源：http://xky.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://dbg.ehwqpu.com

[R70] 时间戳与互转
来源：http://pqe.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://muo.jqgufenzy.top

[R71] 日期格式化
来源：http://ucw.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://dug.ehwqpu.com

[R72] 等待端口就绪
来源：http://azz.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hbx.meibo888.top

[R73] 分割大日志
来源：http://not.daria6918.cn

split -l 1000 big.log part_
来源：http://ayt.wangshuangyany.cn

[R74] 批量重命名
来源：http://mcm.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oxf.xylfe.cn

[R75] 导出环境变量
来源：http://bcq.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://mmb.shangyingyoupin.top

[R76] 使用临时文件
来源：http://xbk.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hmx.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://mmb.uphjek.com

read -rp "请输入: " ans
来源：http://xhb.ydzc1.top

[R78] 交互式菜单
来源：http://rzt.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rdo.zhoulong.xyz

[R79] 解析命令行选项
来源：http://lxo.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://udd.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://uac.gaohongyu789.top

time ./run.sh
来源：http://vri.yfazqb.com

================================================================================
来源：http://upf.pengpengdd.cyou

S. C / C++ 专题
来源：http://vsh.yfazqb.com

================================================================================
来源：http://jvq.ehwqpu.com

[S01] C：Hello World
来源：http://qng.gogol.net.cn

#include <stdio.h>
来源：http://ysf.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vch.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://ogz.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://fdv.hnxiangtu.top

[S03] C：读入整数
来源：http://ajj.fktsv.cn

int x; scanf("%d", &x);
来源：http://wnp.zhijiandao.cn

[S04] C：字符串复制
来源：http://ygp.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yiu.xuanzx.com

[S05] C：字符串长度
来源：http://kgl.daxiang520.top

strlen(s)
来源：http://hpo.cheryme.top

[S06] C：字符串比较
来源：http://ecs.bbcook.cn

strcmp(a, b) == 0
来源：http://rco.bjfxy.top

[S07] C：数组遍历求和
来源：http://blb.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jrx.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://mfd.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wht.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://tcd.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jjg.fengsongda.top

[S10] C：指针与解引用
来源：http://nxw.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://dmw.vehdjk.com

[S11] C：逐行读文件
来源：http://umo.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://kst.xziqi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bqe.cheryme.top

fclose(f);
来源：http://loz.nanxinkj.top

[S12] C：写文件
来源：http://vnl.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rso.hcnkem.com

[S13] C：宏定义
来源：http://dby.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nid.yangfankeji.com

[S14] C：枚举
来源：http://wqu.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ewb.c1oappe.top

[S15] C：类型转换
来源：http://cwh.guannengcc.top

(double) a / b
来源：http://zop.yfazqb.com

[S16] C：位操作置位
来源：http://gbz.cucudq.cn

x |= (1 << 3);
来源：http://kiv.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://klv.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pud.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://hsk.yongpay.top

int main(int argc, char **argv)
来源：http://ohr.yuxming.cn

[S19] C：快速排序
来源：http://agi.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lsd.jlsjyb.cn

[S20] C：二分查找
来源：http://vjx.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dpq.zdbjq.cn

[S21] C：字符类别判断
来源：http://tcq.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fxa.fktsv.cn

[S22] C：字符串转数字
来源：http://fpv.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://vaw.shzxlz.cn

[S23] C：随机数
来源：http://cig.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nld.jianghu66.top

[S24] C：获取本地时间
来源：http://dwg.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mqs.zhoulong.xyz

[S25] C：内存拷贝
来源：http://iwc.nanxuanxn.top

memcpy(dst, src, n);
来源：http://ybw.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://pzy.52xcode.cn

memset(a, 0, sizeof a);
来源：http://sgo.tarul.cn

[S27] C：定义常量
来源：http://itr.zhongyouzk.top

const double PI = 3.14159;
来源：http://otr.nwbrower.top

[S28] C：静态变量
来源：http://epz.quarkkingdee.top

static int counter = 0;
来源：http://lvt.xziqi.cn

[S29] C：变参函数
来源：http://lxd.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fwj.yanxiufei.cn

[S30] C：头文件保护
来源：http://dhv.redwolf501.top

#ifndef X_H
来源：http://bgr.zhaomingkeji.xyz

#define X_H
来源：http://ccu.vehdjk.com

#endif
来源：http://bjh.bbcook.cn

[S31] C++：Hello World
来源：http://mzu.hywenlv.cn

#include <iostream>
来源：http://eml.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://kfo.jqgufenzy.top

[S32] C++：字符串
来源：http://vma.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://zdi.aizwys.cn

[S33] C++：vector 增删
来源：http://mqu.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jbd.yongpay.top

[S34] C++：遍历 vector
来源：http://yjn.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://qee.andypj.xyz

[S35] C++：map
来源：http://lfr.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://psj.jiagoushi.top

[S36] C++：unordered_map
来源：http://ixx.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xzr.sysykeji.top

[S37] C++：set
来源：http://tmf.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ifd.gotoacloud.top

[S38] C++：排序
来源：http://fpr.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://jpt.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://pxm.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zyo.xuanzx.com

[S40] C++：查找元素
来源：http://vda.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://etw.zycfv.cn

[S41] C++：类与构造函数
来源：http://utn.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gmv.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://wzo.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://vif.yueranfly.top

[S43] C++：智能指针
来源：http://fol.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://yav.zycfv.cn

[S44] C++：引用传参
来源：http://ava.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://jsm.fehbvm.com

[S45] C++：lambda
来源：http://tki.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xek.cheryme.top

[S46] C++：函数模板
来源：http://vgt.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wkk.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://htd.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://awa.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://kml.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://bux.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://wmu.zdqjudy.top

[S49] C++：写文件
来源：http://gwp.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofm.birdmap.top

[S50] C++：格式化数字
来源：http://txp.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksj.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://vqi.cqqwz.cn

static_cast<double>(a) / b
来源：http://jyw.uphjek.com

[S52] C++：const 与 noexcept
来源：http://nfr.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://pge.mhx1999.top

[S53] C++：移动语义
来源：http://asp.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://ive.yangfankeji.com

[S54] C++：异常处理
来源：http://gcj.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ihc.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://jlb.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jrj.cheryme.top

[S56] C++：optional
来源：http://tgq.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fim.nwbrower.top

[S57] C++：编译期常量
来源：http://cos.andypj.xyz

constexpr int N = 10;
来源：http://xuw.tarul.cn

[S58] C++：命名空间
来源：http://oud.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://buk.shuidangran.top

[S59] C++：静态断言
来源：http://bbz.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jyv.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://ycx.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hxa.quarkkingdee.top

================================================================================
来源：http://qfa.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uaz.zdbjq.cn

================================================================================
来源：http://htl.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://tle.52xcode.cn

println("Hello")
来源：http://kyt.yongpay.top

[T02] Kotlin：变量
来源：http://lzb.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nqp.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://itz.dianchejie.cn

"值: $b"
来源：http://nvm.dianchejie.cn

[T04] Kotlin：空安全
来源：http://sre.mhx1999.top

val n: String? = null;  n?.length
来源：http://lbw.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://iwl.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qbd.hesvh.cn

[T06] Kotlin：集合映射
来源：http://knm.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jhr.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://lyw.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhz.yuanzhike.top

[T08] Kotlin：数据类
来源：http://qbw.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://rfy.nanxinkj.top


<!-- 参考信息 -->