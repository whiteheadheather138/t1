代发 wailian999

set -euo pipefail
来源：http://jff.fehbvm.com

[R02] 变量赋值与使用
来源：http://tpr.yfazqb.com

name="Tom"; echo "$name"
来源：http://mbp.chenzaomai.com

[R03] 只读变量
来源：http://fiu.yangfankeji.com

readonly PI=3.14
来源：http://ejm.ivvv.top

[R04] 位置参数
来源：http://pmq.fanxiaobao.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kcv.nwbrower.top

[R05] 参数默认值
来源：http://stq.yanxiufei.cn

name="${1:-default}"
来源：http://bbq.shangyingyoupin.top

[R06] 判断命令是否存在
来源：http://yud.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifp.aibaodan.cn

[R07] if 判断文件
来源：http://cps.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mgh.sjlbkw.cn

[R08] 数值比较
来源：http://wlu.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://opc.uphjek.com

[R09] 字符串比较
来源：http://dga.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://muf.xuanzx.com

[R10] 正则匹配
来源：http://ixn.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://laa.daria6918.cn

[R11] case 多分支
来源：http://cwx.ctjpmb.com

case "$1" in
来源：http://zae.hfpthk.cn

start) echo "启动" ;;
来源：http://zxy.ybcxt.top

stop)  echo "停止" ;;
来源：http://gsu.aizwys.cn

*)     echo "未知命令" ;;
来源：http://mbe.shanyushiyangtech.top

esac
来源：http://hcj.hesvh.cn

[R12] for 遍历文件
来源：http://rny.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://kor.zdbjq.cn

[R13] for 计数循环
来源：http://rpz.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://fwo.jqgufenzy.top

[R14] C 风格 for
来源：http://wjl.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uue.zhijiandao.cn

[R15] while 逐行读文件
来源：http://kow.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jkk.bbcook.cn

[R16] until 等待条件
来源：http://jxk.daxiang520.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://buk.smart0.xyz

[R17] 数组定义与取值
来源：http://ebb.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://znq.jinyuanbaomall.cn

[R18] 遍历数组
来源：http://cbo.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jdf.haohaochexian.top

[R19] 数组长度
来源：http://gdn.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://ock.tarul.cn

[R20] 关联数组（字典）
来源：http://vxs.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vfw.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://nmz.xinyue.icu

echo "${#s}"
来源：http://afm.hammf.cn

[R22] 截取子串
来源：http://sol.quarkkingdee.top

echo "${s:0:5}"
来源：http://vgg.tarul.cn

[R23] 字符串替换
来源：http://tzh.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cpu.yvedp.cn

[R24] 大小写转换
来源：http://xmf.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://abo.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://hpr.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lfh.yj20258.top

[R26] 命令替换
来源：http://xfe.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://ryh.316326.xyz

[R27] 算术展开
来源：http://dpy.yonumen.top

echo $((1 + 2 * 3))
来源：http://zrc.jqgufenzy.top

[R28] 浮点运算
来源：http://ikg.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://tmx.birdmap.top

[R29] 定义函数
来源：http://usz.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vsf.yj20258888.top

[R30] 函数返回状态码
来源：http://pry.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://jux.zhiwuduotai.top

[R31] 局部变量
来源：http://ptj.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://opi.jinqigufen.top

[R32] 参数个数校验
来源：http://zaw.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mdn.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://hrw.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bbu.daxiang520.top

[R34] 退出时清理
来源：http://doo.yongpay.top

trap 'rm -f "$tmp"' EXIT
来源：http://uab.tarul.cn

[R35] 后台执行并等待
来源：http://wdh.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qax.svipenyu.cn

[R36] 并发执行多个任务
来源：http://gao.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://von.bjfxy.top

[R37] 把输出赋给变量
来源：http://ykl.wangshuangyany.cn

files=$(ls -1)
来源：http://fuq.c1oappe.top

[R38] 管道串联
来源：http://wtv.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://lgt.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://tcv.chenzaomai.com

cmd > out.log 2>&1
来源：http://irt.ivvv.top

[R40] 追加写日志
来源：http://api.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://pqa.xinyue.icu

[R41] 丢弃输出
来源：http://vvq.uphjek.com

cmd >/dev/null 2>&1
来源：http://grj.gogol.net.cn

[R42] 输入重定向
来源：http://xhg.quarkkingdee.top

wc -l < a.txt
来源：http://vhj.zhijiandao.cn

[R43] 按名字查找文件
来源：http://trc.smart0.xyz

find . -name "*.log" -type f
来源：http://awu.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://agv.ctjpmb.com

find . -mtime -7 -type f
来源：http://bmd.fzhhl.top

[R45] 批量删除
来源：http://jme.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://vgw.haohaochexian.top

[R46] 递归替换文件内容
来源：http://aek.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xos.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://rje.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://jqn.ehwqpu.com

[R48] awk 取指定列
来源：http://uuu.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://mto.jyoumei.cn

[R49] awk 带条件
来源：http://wjl.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rif.cqqwz.cn

[R50] awk 求和
来源：http://txg.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://qcy.yonumen.top

[R51] 排序去重取前几
来源：http://xkm.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pbi.zhongyouzk.top

[R52] 统计行数
来源：http://sfq.havefunace.top

wc -l a.txt
来源：http://rsz.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://fhi.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dtm.jyoumei.cn

[R54] 比较两个文件
来源：http://lyr.chenlongwang.top

diff a.txt b.txt
来源：http://xky.zycfv.cn

[R55] 压缩与解压
来源：http://ymg.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wnr.cheryme.top

[R56] 远程拷贝
来源：http://fzv.ivvv.top

scp file user@host:/path/
来源：http://cue.jianghu66.top

[R57] 远程执行命令
来源：http://bty.yongpay.top

ssh user@host 'uptime'
来源：http://fib.yfazqb.com

[R58] 下载文件
来源：http://ldi.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bmt.shzxlz.cn

[R59] 发 POST JSON
来源：http://hwu.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zkj.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://gir.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ash.shuidangran.top

[R61] 磁盘占用
来源：http://pdg.daxiang520.top

df -h;  du -sh *
来源：http://fay.fehbvm.com

[R62] 找最占空间的文件
来源：http://ppx.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://cbp.gotoacloud.top

[R63] 内存与进程
来源：http://zeq.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://gnk.yongpay.top

[R64] 结束进程
来源：http://gzr.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://tvf.hnqzz.top

[R65] 查看端口占用
来源：http://oqr.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pox.redwolf501.top

[R66] 定时任务
来源：http://yrx.316326.xyz

crontab -e;  crontab -l
来源：http://mgr.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://ava.zhiwuduotai.top

openssl rand -hex 16
来源：http://gkb.hammf.cn

[R68] 计算文件校验值
来源：http://mka.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://iiv.havefunace.top

[R69] 生成随机密码
来源：http://vux.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://nsl.yvedp.cn

[R70] 时间戳与互转
来源：http://yyw.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://vur.wangshuangyany.cn

[R71] 日期格式化
来源：http://zbf.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://cbt.zdbjq.cn

[R72] 等待端口就绪
来源：http://qaq.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ghw.tianlin.xyz

[R73] 分割大日志
来源：http://axl.ctjpmb.com

split -l 1000 big.log part_
来源：http://tog.fktsv.cn

[R74] 批量重命名
来源：http://fbs.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gld.tian-w.cn

[R75] 导出环境变量
来源：http://lhm.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://ixu.vehdjk.com

[R76] 使用临时文件
来源：http://usi.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uxq.fehbvm.com

[R77] 读取用户输入
来源：http://gcb.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://edk.yj20258.top

[R78] 交互式菜单
来源：http://chp.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ucv.ehwqpu.com

[R79] 解析命令行选项
来源：http://auc.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gzp.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://rif.sweek.top

time ./run.sh
来源：http://pek.zhijiandao.cn

================================================================================
来源：http://aps.c1oappe.top

S. C / C++ 专题
来源：http://ins.vqdsnc.cn

================================================================================
来源：http://qbz.sxryk.cn

[S01] C：Hello World
来源：http://owf.ydjk.org.cn

#include <stdio.h>
来源：http://uts.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://brr.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://gou.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://pos.iojbl.cn

[S03] C：读入整数
来源：http://nld.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://lxe.gzhubu.top

[S04] C：字符串复制
来源：http://uat.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://uxj.hammf.cn

[S05] C：字符串长度
来源：http://fjx.ybcxt.top

strlen(s)
来源：http://ilk.tian-w.cn

[S06] C：字符串比较
来源：http://swv.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://byu.yongpay.top

[S07] C：数组遍历求和
来源：http://vii.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fns.tarul.cn

[S08] C：动态内存分配与释放
来源：http://mbd.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ovv.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://zvr.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nse.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://iah.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://jqz.redwolf501.top

[S11] C：逐行读文件
来源：http://lgk.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://cep.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://upt.ppjwa.cn

fclose(f);
来源：http://yps.cqqwz.cn

[S12] C：写文件
来源：http://vis.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gje.epnwcf.com

[S13] C：宏定义
来源：http://nmi.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gmb.52xcode.cn

[S14] C：枚举
来源：http://ywc.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://uos.chenlongwang.top

[S15] C：类型转换
来源：http://zvx.cdnleiting.top

(double) a / b
来源：http://flq.xziqi.cn

[S16] C：位操作置位
来源：http://vec.nwbrower.top

x |= (1 << 3);
来源：http://fcl.iojbl.cn

[S17] C：安全拼接字符串
来源：http://jov.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gte.tianlin.xyz

[S18] C：命令行参数
来源：http://oju.jianghu66.top

int main(int argc, char **argv)
来源：http://gnx.mhx1999.top

[S19] C：快速排序
来源：http://sbu.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://nfs.shzxlz.cn

[S20] C：二分查找
来源：http://fyr.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ajj.ppjwa.cn

[S21] C：字符类别判断
来源：http://aji.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://slc.kuanghao11.cn

[S22] C：字符串转数字
来源：http://mox.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://qkz.tanke756.top

[S23] C：随机数
来源：http://hhz.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lbo.ppjwa.cn

[S24] C：获取本地时间
来源：http://vnm.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://amb.hnxiangtu.top

[S25] C：内存拷贝
来源：http://qwe.tanke756.top

memcpy(dst, src, n);
来源：http://qdx.jinghuilouyu.cn

[S26] C：内存清零
来源：http://mzt.redwolf501.top

memset(a, 0, sizeof a);
来源：http://crr.cucudq.cn

[S27] C：定义常量
来源：http://xvv.nwbrower.top

const double PI = 3.14159;
来源：http://lzq.meibo888.top

[S28] C：静态变量
来源：http://qcs.jinqigfzy.top

static int counter = 0;
来源：http://sar.xuanzx.com

[S29] C：变参函数
来源：http://mbc.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ewa.birdmap.top

[S30] C：头文件保护
来源：http://hox.hnqzz.top

#ifndef X_H
来源：http://qjs.andypj.xyz

#define X_H
来源：http://ikj.c1oappe.top

#endif
来源：http://tkh.yangfankeji.com

[S31] C++：Hello World
来源：http://vkx.sjlbkw.cn

#include <iostream>
来源：http://hdz.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://qsz.quarkkingdee.top

[S32] C++：字符串
来源：http://kux.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://wdf.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://loy.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fyi.shzxlz.cn

[S34] C++：遍历 vector
来源：http://vhh.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://fvx.mhx1999.top

[S35] C++：map
来源：http://rzz.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vhq.gzhubu.top

[S36] C++：unordered_map
来源：http://ima.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kze.smart0.xyz

[S37] C++：set
来源：http://pjl.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mqi.chenjidiqi.icu

[S38] C++：排序
来源：http://erz.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://bbu.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://yta.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vcu.snrcjt.cn

[S40] C++：查找元素
来源：http://ikd.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://axo.hammf.cn

[S41] C++：类与构造函数
来源：http://bzm.yuxming.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://obk.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://mig.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://zey.nanxinkj.top

[S43] C++：智能指针
来源：http://hpl.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://upu.daria6918.cn

[S44] C++：引用传参
来源：http://hye.cucudq.cn

void inc(int &x) { ++x; }
来源：http://bvg.jqgfzy.top

[S45] C++：lambda
来源：http://hum.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://ppy.cqqwz.cn

[S46] C++：函数模板
来源：http://zmp.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fvw.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://gov.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucn.yj20258.top

[S48] C++：逐行读文件
来源：http://rwd.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://rgu.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://pyb.ehwqpu.com

[S49] C++：写文件
来源：http://hxm.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ooi.birdmap.top

[S50] C++：格式化数字
来源：http://myn.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exz.ybcxt.top

[S51] C++：显式类型转换
来源：http://agc.guannengcc.top

static_cast<double>(a) / b
来源：http://dwr.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://tzq.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://dyk.andypj.xyz

[S53] C++：移动语义
来源：http://ogm.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://tnm.yj202588.top

[S54] C++：异常处理
来源：http://ies.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pru.zycfv.cn

[S55] C++：结构化绑定
来源：http://huw.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://vur.zhixingplan.top

[S56] C++：optional
来源：http://vnl.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xjg.zdbjq.cn

[S57] C++：编译期常量
来源：http://dne.sufxvd.cn

constexpr int N = 10;
来源：http://mxn.fktsv.cn

[S58] C++：命名空间
来源：http://ejo.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://iwo.jianghu66.top

[S59] C++：静态断言
来源：http://xky.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kft.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://twm.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uqo.hywenlv.cn

================================================================================
来源：http://thh.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cwl.ppjwa.cn

================================================================================
来源：http://zwy.daria6918.cn

[T01] Kotlin：Hello World
来源：http://wvq.yj202588.top

println("Hello")
来源：http://scm.hnxiangtu.top

[T02] Kotlin：变量
来源：http://ygi.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://owd.vqdsnc.cn


<!-- 参考信息 -->