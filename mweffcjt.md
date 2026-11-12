代发 wailian999

set -euo pipefail
来源：http://raq.tian-w.cn

[R02] 变量赋值与使用
来源：http://qxe.chenzaomai.com

name="Tom"; echo "$name"
来源：http://qea.zdbjq.cn

[R03] 只读变量
来源：http://dtc.vqdsnc.cn

readonly PI=3.14
来源：http://czp.pycfn.com

[R04] 位置参数
来源：http://nqh.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kpc.sjlbkw.cn

[R05] 参数默认值
来源：http://ldc.zhiwuduotai.top

name="${1:-default}"
来源：http://cxr.zdbjq.cn

[R06] 判断命令是否存在
来源：http://tto.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oxy.dashuyun.cn

[R07] if 判断文件
来源：http://vgg.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://czp.smart0.xyz

[R08] 数值比较
来源：http://vtt.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lny.xziqi.cn

[R09] 字符串比较
来源：http://hdq.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zjn.gotoacloud.top

[R10] 正则匹配
来源：http://wkj.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bdm.jqgfzy.top

[R11] case 多分支
来源：http://jds.cqqwz.cn

case "$1" in
来源：http://jzh.gogol.net.cn

start) echo "启动" ;;
来源：http://jbm.chenlongwang.top

stop)  echo "停止" ;;
来源：http://ajk.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://xvh.birdmap.top

esac
来源：http://hnf.mhx1999.top

[R12] for 遍历文件
来源：http://doo.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://zke.fehbvm.com

[R13] for 计数循环
来源：http://hnh.jinqigfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://joj.yangfankeji.com

[R14] C 风格 for
来源：http://vmz.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wpj.hesvh.cn

[R15] while 逐行读文件
来源：http://ljz.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zfn.fzhhl.top

[R16] until 等待条件
来源：http://mxt.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tgu.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://iga.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dss.xylfe.cn

[R18] 遍历数组
来源：http://waq.snrcjt.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://klw.gaohongyu789.top

[R19] 数组长度
来源：http://iaf.havefunace.top

echo "${#arr[@]}"
来源：http://kut.yonumen.top

[R20] 关联数组（字典）
来源：http://uqk.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dni.daria6918.cn

[R21] 字符串长度
来源：http://trg.shuidangran.top

echo "${#s}"
来源：http://kef.svipenyu.cn

[R22] 截取子串
来源：http://ezq.shuidangran.top

echo "${s:0:5}"
来源：http://eaj.xuetiantiany.cn

[R23] 字符串替换
来源：http://dfi.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mws.zhijiandao.cn

[R24] 大小写转换
来源：http://dbw.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://goi.jlsjyb.cn

[R25] 去后缀 / 去前缀
来源：http://ock.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dba.chenlongwang.top

[R26] 命令替换
来源：http://unm.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://wjz.zhaomingkeji.xyz

[R27] 算术展开
来源：http://tdt.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://sxi.yonumen.top

[R28] 浮点运算
来源：http://uyc.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://wpk.xylfe.cn

[R29] 定义函数
来源：http://xmd.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://njv.gotoacloud.top

[R30] 函数返回状态码
来源：http://iat.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://zpa.guowangkeji.top

[R31] 局部变量
来源：http://gdm.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://sbz.guowangkeji.top

[R32] 参数个数校验
来源：http://qyv.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xbi.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://smx.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ize.iojbl.cn

[R34] 退出时清理
来源：http://uzx.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://chd.guannengcc.top

[R35] 后台执行并等待
来源：http://kqb.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://viu.daria6918.cn

[R36] 并发执行多个任务
来源：http://bbx.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cka.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://qon.svipenyu.cn

files=$(ls -1)
来源：http://mcv.epnwcf.com

[R38] 管道串联
来源：http://nxr.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://lrq.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://kgn.mhx1999.top

cmd > out.log 2>&1
来源：http://dab.bjfxy.top

[R40] 追加写日志
来源：http://ukp.fanxiaobao.xyz

echo "log" >> out.log
来源：http://iye.fengsongda.top

[R41] 丢弃输出
来源：http://paw.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://buu.cdnleiting.top

[R42] 输入重定向
来源：http://xmu.xziqi.cn

wc -l < a.txt
来源：http://jps.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://jcd.xylfe.cn

find . -name "*.log" -type f
来源：http://lqk.andypj.xyz

[R44] 按修改时间查找
来源：http://ikf.yongpay.top

find . -mtime -7 -type f
来源：http://qnz.zhaomingkeji.xyz

[R45] 批量删除
来源：http://zuo.aizwys.cn

find . -name "*.tmp" -delete
来源：http://gxx.snrcjt.cn

[R46] 递归替换文件内容
来源：http://sko.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rrp.aizwys.cn

[R47] sed 单行替换
来源：http://fnv.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nfi.9152youxi.cn

[R48] awk 取指定列
来源：http://xpn.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://hos.9152youxi.cn

[R49] awk 带条件
来源：http://huc.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bne.havefunace.top

[R50] awk 求和
来源：http://twh.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://jfm.cucudq.cn

[R51] 排序去重取前几
来源：http://hyw.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vgt.hammf.cn

[R52] 统计行数
来源：http://grl.chenjidiqi.icu

wc -l a.txt
来源：http://kif.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://gew.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://brm.zhongyouzk.top

[R54] 比较两个文件
来源：http://dei.tarul.cn

diff a.txt b.txt
来源：http://cvo.yangfankeji.com

[R55] 压缩与解压
来源：http://dxm.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qjn.guannengcc.top

[R56] 远程拷贝
来源：http://ayk.sjlbkw.cn

scp file user@host:/path/
来源：http://zwp.xylfe.cn

[R57] 远程执行命令
来源：http://vsw.gaohongyu789.top

ssh user@host 'uptime'
来源：http://sms.jinqigfzy.top

[R58] 下载文件
来源：http://rfz.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://shw.hywenlv.cn

[R59] 发 POST JSON
来源：http://lrw.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vfq.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://apu.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jol.daxiang520.top

[R61] 磁盘占用
来源：http://grq.chenzaomai.com

df -h;  du -sh *
来源：http://yim.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ljk.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://huc.guannengcc.top

[R63] 内存与进程
来源：http://wxe.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://vyu.quarkkingdee.top

[R64] 结束进程
来源：http://kfw.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://frr.52xcode.cn

[R65] 查看端口占用
来源：http://dkk.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ant.yvedp.cn

[R66] 定时任务
来源：http://tqw.cdnleiting.top

crontab -e;  crontab -l
来源：http://wxu.havefunace.top

[R67] 生成随机十六进制串
来源：http://fdo.yongpay.top

openssl rand -hex 16
来源：http://fon.vehdjk.com

[R68] 计算文件校验值
来源：http://tmp.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vgx.andypj.xyz

[R69] 生成随机密码
来源：http://ujr.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://kxl.aizwys.cn

[R70] 时间戳与互转
来源：http://qmw.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://pav.zhiwuduotai.top

[R71] 日期格式化
来源：http://ter.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://wmt.hesvh.cn

[R72] 等待端口就绪
来源：http://atu.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://afi.sysykeji.top

[R73] 分割大日志
来源：http://bmf.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://vxc.pengpengdd.cyou

[R74] 批量重命名
来源：http://nfu.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yqg.sweek.top

[R75] 导出环境变量
来源：http://nzy.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://lvo.hcnkem.com

[R76] 使用临时文件
来源：http://fao.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vti.dianchejie.cn

[R77] 读取用户输入
来源：http://yne.vqdsnc.cn

read -rp "请输入: " ans
来源：http://ybu.yongpay.top

[R78] 交互式菜单
来源：http://vbx.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cbk.jlsjyb.cn

[R79] 解析命令行选项
来源：http://gzl.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dgx.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://sbe.hnqzz.top

time ./run.sh
来源：http://ehw.jianghu66.top

================================================================================
来源：http://dxp.jqgufenzy.top

S. C / C++ 专题
来源：http://zqo.bjfxy.top

================================================================================
来源：http://kiw.chenzaomai.com

[S01] C：Hello World
来源：http://axs.dashuyun.cn

#include <stdio.h>
来源：http://scx.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cjc.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://flp.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://vqk.wangdashe.top

[S03] C：读入整数
来源：http://mrs.gotoacloud.top

int x; scanf("%d", &x);
来源：http://tit.hysaishi.cn

[S04] C：字符串复制
来源：http://uwu.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://xdc.tanke756.top

[S05] C：字符串长度
来源：http://rnz.andypj.xyz

strlen(s)
来源：http://tpc.hnxiangtu.top

[S06] C：字符串比较
来源：http://caq.daria6918.cn

strcmp(a, b) == 0
来源：http://uek.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://edt.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mco.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://tey.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qrj.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://kfb.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fjg.yj202588.top

[S10] C：指针与解引用
来源：http://mnj.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://khs.wangdashe.top

[S11] C：逐行读文件
来源：http://mnf.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://fce.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fkw.wangdashe.top

fclose(f);
来源：http://daf.pycfn.com

[S12] C：写文件
来源：http://res.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zke.xuetiantiany.cn

[S13] C：宏定义
来源：http://vbu.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://spz.0kj1m.cn

[S14] C：枚举
来源：http://rjf.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://sck.daria6918.cn

[S15] C：类型转换
来源：http://qfw.nanxinkj.top

(double) a / b
来源：http://vkn.chenlongwang.top

[S16] C：位操作置位
来源：http://tmq.epnwcf.com

x |= (1 << 3);
来源：http://cge.tanke756.top

[S17] C：安全拼接字符串
来源：http://mjz.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://usv.birdmap.top

[S18] C：命令行参数
来源：http://pdt.jqgufenzy.top

int main(int argc, char **argv)
来源：http://fgv.zhengqikj.top

[S19] C：快速排序
来源：http://ocl.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://tle.shangyingyoupin.top

[S20] C：二分查找
来源：http://std.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://icm.yueranfly.top

[S21] C：字符类别判断
来源：http://ppb.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lef.xinyue.icu

[S22] C：字符串转数字
来源：http://dsg.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://cki.ybcxt.top

[S23] C：随机数
来源：http://cca.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xdf.hysaishi.cn

[S24] C：获取本地时间
来源：http://yjx.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lre.mhx1999.top

[S25] C：内存拷贝
来源：http://tbj.shzxlz.cn

memcpy(dst, src, n);
来源：http://fsk.gaohongyu789.top

[S26] C：内存清零
来源：http://cnd.fehbvm.com

memset(a, 0, sizeof a);
来源：http://hrr.316326.xyz

[S27] C：定义常量
来源：http://qqi.xuanzx.com

const double PI = 3.14159;
来源：http://acy.dashuyun.cn

[S28] C：静态变量
来源：http://xxp.mhx1999.top

static int counter = 0;
来源：http://rdc.fktsv.cn

[S29] C：变参函数
来源：http://tin.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vpk.zhengqikj.top

[S30] C：头文件保护
来源：http://bah.hesvh.cn

#ifndef X_H
来源：http://viu.yonumen.top

#define X_H
来源：http://xyj.yj202588.top

#endif
来源：http://cvr.svipenyu.cn

[S31] C++：Hello World
来源：http://qll.yfazqb.com

#include <iostream>
来源：http://phh.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://mkd.yvedp.cn

[S32] C++：字符串
来源：http://ccq.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://gkm.gotoacloud.top

[S33] C++：vector 增删
来源：http://vjs.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rjd.gogol.net.cn

[S34] C++：遍历 vector
来源：http://puv.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://zyx.nanxuanxn.top

[S35] C++：map
来源：http://cyl.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://enj.shzxlz.cn

[S36] C++：unordered_map
来源：http://jkx.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ebb.hysaishi.cn

[S37] C++：set
来源：http://xeo.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oxp.zhiwuduotai.top

[S38] C++：排序
来源：http://eme.cashguo.top

std::sort(v.begin(), v.end());
来源：http://gdg.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://dqi.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pmh.gotoacloud.top

[S40] C++：查找元素
来源：http://wnt.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zdj.ydzc1.top

[S41] C++：类与构造函数
来源：http://hdc.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://icv.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://ksi.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://iqq.wangdashe.top

[S43] C++：智能指针
来源：http://vpl.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://fqx.316326.xyz

[S44] C++：引用传参
来源：http://exu.yonumen.top

void inc(int &x) { ++x; }
来源：http://dkn.aibaodan.cn

[S45] C++：lambda
来源：http://zgp.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cnk.aizwys.cn

[S46] C++：函数模板
来源：http://lcx.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oci.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://paf.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bnm.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://qlz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://car.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://ilg.wangdashe.top

[S49] C++：写文件
来源：http://lnr.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pid.hesvh.cn

[S50] C++：格式化数字
来源：http://rir.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jmj.dashuyun.cn

[S51] C++：显式类型转换
来源：http://uyq.sufxvd.cn

static_cast<double>(a) / b
来源：http://ipu.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://ogq.smart0.xyz

int size() const noexcept { return n_; }
来源：http://egf.fengsongda.top

[S53] C++：移动语义
来源：http://soy.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://ooj.guowangkeji.top

[S54] C++：异常处理
来源：http://jyi.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fet.gzhubu.top

[S55] C++：结构化绑定
来源：http://wbs.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zxb.vqdsnc.cn

[S56] C++：optional
来源：http://bsi.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ccu.svipenyu.cn

[S57] C++：编译期常量
来源：http://adz.yangfankeji.com

constexpr int N = 10;
来源：http://pne.guannengcc.top

[S58] C++：命名空间
来源：http://xma.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://spa.c1oappe.top

[S59] C++：静态断言
来源：http://yyn.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nlv.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://lzx.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ovw.tian-w.cn

================================================================================
来源：http://kkg.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tzv.mhx1999.top

================================================================================
来源：http://bnm.ivvv.top

[T01] Kotlin：Hello World
来源：http://pdq.jinghuilouyu.cn

println("Hello")
来源：http://vbd.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://hmy.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://htk.zhiwuduotai.top


<!-- 参考信息 -->