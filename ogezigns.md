代发 wailian999

set -euo pipefail
来源：http://ifv.zdqjudy.top

[R02] 变量赋值与使用
来源：http://qtw.bbcook.cn

name="Tom"; echo "$name"
来源：http://fxt.shzxlz.cn

[R03] 只读变量
来源：http://nqf.hywenlv.cn

readonly PI=3.14
来源：http://xsg.jinqigfzy.top

[R04] 位置参数
来源：http://quk.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jnt.zhixingplan.top

[R05] 参数默认值
来源：http://fjs.jinqigufen.top

name="${1:-default}"
来源：http://iqt.gogol.net.cn

[R06] 判断命令是否存在
来源：http://qmh.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eua.nwbrower.top

[R07] if 判断文件
来源：http://scq.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xrh.yonumen.top

[R08] 数值比较
来源：http://qdh.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pds.xinyue.icu

[R09] 字符串比较
来源：http://wie.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rxo.xinyue.icu

[R10] 正则匹配
来源：http://iiw.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yza.ybcxt.top

[R11] case 多分支
来源：http://hhf.bjfxy.top

case "$1" in
来源：http://zrx.tianlin.xyz

start) echo "启动" ;;
来源：http://ckg.cheryme.top

stop)  echo "停止" ;;
来源：http://dzm.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://kmd.jqgfzy.top

esac
来源：http://gpe.redwolf501.top

[R12] for 遍历文件
来源：http://pzc.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://ser.wangdashe.top

[R13] for 计数循环
来源：http://iut.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://lfn.fzhhl.top

[R14] C 风格 for
来源：http://lkr.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zqx.xinyue.icu

[R15] while 逐行读文件
来源：http://uhg.zhengqikj.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vgs.0kj1m.cn

[R16] until 等待条件
来源：http://syw.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hoh.yj20258.top

[R17] 数组定义与取值
来源：http://obp.guannengcc.top

arr=(a b c); echo "${arr[0]}"
来源：http://job.wangdashe.top

[R18] 遍历数组
来源：http://sdd.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sju.gotoacloud.top

[R19] 数组长度
来源：http://ixk.daxiang520.top

echo "${#arr[@]}"
来源：http://gmu.jinqigfzy.top

[R20] 关联数组（字典）
来源：http://blh.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zin.aibaodan.cn

[R21] 字符串长度
来源：http://cus.sufxvd.cn

echo "${#s}"
来源：http://jzd.ywan-chungtsiang.top

[R22] 截取子串
来源：http://ypo.guannengcc.top

echo "${s:0:5}"
来源：http://bou.ybcxt.top

[R23] 字符串替换
来源：http://jut.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ami.nwbrower.top

[R24] 大小写转换
来源：http://grw.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://zqt.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://gmc.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tjt.sweek.top

[R26] 命令替换
来源：http://oug.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://thb.hammf.cn

[R27] 算术展开
来源：http://nhj.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://ito.mhx1999.top

[R28] 浮点运算
来源：http://xfb.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://pzp.hysaishi.cn

[R29] 定义函数
来源：http://dyd.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wnz.svipenyu.cn

[R30] 函数返回状态码
来源：http://sfk.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://srg.ywan-chungtsiang.top

[R31] 局部变量
来源：http://phf.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://svh.yuanzhike.top

[R32] 参数个数校验
来源：http://gpp.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fcq.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://ssd.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oth.meibo888.top

[R34] 退出时清理
来源：http://enf.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mri.zhijiandao.cn

[R35] 后台执行并等待
来源：http://job.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jmb.0kj1m.cn

[R36] 并发执行多个任务
来源：http://btz.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://chv.dianchejie.cn

[R37] 把输出赋给变量
来源：http://pbx.shanyushiyangkeji.top

files=$(ls -1)
来源：http://ayv.jinqigufen.top

[R38] 管道串联
来源：http://dhk.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://vlj.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://ems.chenzaomai.com

cmd > out.log 2>&1
来源：http://tpe.wangshuangyany.cn

[R40] 追加写日志
来源：http://xeu.haohaochexian.top

echo "log" >> out.log
来源：http://rqy.fktsv.cn

[R41] 丢弃输出
来源：http://dwb.wangdashe.top

cmd >/dev/null 2>&1
来源：http://egz.gaohongyu789.top

[R42] 输入重定向
来源：http://wmc.jinqigfzy.top

wc -l < a.txt
来源：http://ysv.fzhhl.top

[R43] 按名字查找文件
来源：http://tru.yuxming.cn

find . -name "*.log" -type f
来源：http://cac.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://rjm.xylfe.cn

find . -mtime -7 -type f
来源：http://wqj.c1oappe.top

[R45] 批量删除
来源：http://imw.bbcook.cn

find . -name "*.tmp" -delete
来源：http://cja.redwolf501.top

[R46] 递归替换文件内容
来源：http://ust.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://muj.yuanzhike.top

[R47] sed 单行替换
来源：http://fri.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qbh.hammf.cn

[R48] awk 取指定列
来源：http://sgp.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://vdo.nanxuanxn.top

[R49] awk 带条件
来源：http://uwu.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xlp.chenzaomai.com

[R50] awk 求和
来源：http://yfz.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://hcl.andypj.xyz

[R51] 排序去重取前几
来源：http://oym.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wis.hnxiangtu.top

[R52] 统计行数
来源：http://skv.shangyingyoupin.top

wc -l a.txt
来源：http://ppk.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://xyh.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://prf.0kj1m.cn

[R54] 比较两个文件
来源：http://yme.vqdsnc.cn

diff a.txt b.txt
来源：http://soj.epnwcf.com

[R55] 压缩与解压
来源：http://fvn.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ivr.bbcook.cn

[R56] 远程拷贝
来源：http://mjh.iojbl.cn

scp file user@host:/path/
来源：http://bpk.aibaodan.cn

[R57] 远程执行命令
来源：http://glm.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://xty.iojbl.cn

[R58] 下载文件
来源：http://dvh.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mer.yj20258888.top

[R59] 发 POST JSON
来源：http://few.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iqd.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://fxt.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lzl.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://gzl.xuanzx.com

df -h;  du -sh *
来源：http://myv.yj20258888.top

[R62] 找最占空间的文件
来源：http://tbq.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://yrn.ppjwa.cn

[R63] 内存与进程
来源：http://okh.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://ivz.sjlbkw.cn

[R64] 结束进程
来源：http://gvr.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://wuv.dashuyun.cn

[R65] 查看端口占用
来源：http://qwm.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zvz.haohaochexian.top

[R66] 定时任务
来源：http://dql.52xcode.cn

crontab -e;  crontab -l
来源：http://vib.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://wjy.sweek.top

openssl rand -hex 16
来源：http://ruj.yuanzhike.top

[R68] 计算文件校验值
来源：http://ztx.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://skk.cqqwz.cn

[R69] 生成随机密码
来源：http://frl.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://nkd.dianchejie.cn

[R70] 时间戳与互转
来源：http://xjc.xziqi.cn

date +%s;  date -d @1700000000
来源：http://gvd.snrcjt.cn

[R71] 日期格式化
来源：http://qte.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pep.xuanzx.com

[R72] 等待端口就绪
来源：http://sui.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ncu.ydjk.org.cn

[R73] 分割大日志
来源：http://ghx.havefunace.top

split -l 1000 big.log part_
来源：http://mvx.nanxuanxn.top

[R74] 批量重命名
来源：http://bmw.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sch.xuanzx.com

[R75] 导出环境变量
来源：http://hwy.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://bal.gogol.net.cn

[R76] 使用临时文件
来源：http://sig.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://akb.daria6918.cn

[R77] 读取用户输入
来源：http://jnq.chenlongwang.top

read -rp "请输入: " ans
来源：http://xim.zhijiandao.cn

[R78] 交互式菜单
来源：http://orb.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wkr.0kj1m.cn

[R79] 解析命令行选项
来源：http://exp.yangfankeji.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lba.tanke756.top

[R80] 查看脚本执行耗时
来源：http://phq.uphjek.com

time ./run.sh
来源：http://san.jinqigfzy.top

================================================================================
来源：http://vtn.vehdjk.com

S. C / C++ 专题
来源：http://gme.jqgfzy.top

================================================================================
来源：http://rwn.meibo888.top

[S01] C：Hello World
来源：http://azm.mhx1999.top

#include <stdio.h>
来源：http://nie.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhm.wangdashe.top

[S02] C：变量与格式化输出
来源：http://kbz.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://ysx.yanxiufei.cn

[S03] C：读入整数
来源：http://saf.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://iqb.zdqjudy.top

[S04] C：字符串复制
来源：http://dcc.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ycp.yueranfly.top

[S05] C：字符串长度
来源：http://pzn.ctjpmb.com

strlen(s)
来源：http://jen.gogol.net.cn

[S06] C：字符串比较
来源：http://kiz.mhx1999.top

strcmp(a, b) == 0
来源：http://ebu.jyoumei.cn

[S07] C：数组遍历求和
来源：http://pky.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zsh.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://zci.andypj.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fkm.yongpay.top

[S09] C：结构体定义与初始化
来源：http://buk.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nci.shuidangran.top

[S10] C：指针与解引用
来源：http://hie.hcnkem.com

int *p = &a;  *p = 5;
来源：http://ytn.jianghu66.top

[S11] C：逐行读文件
来源：http://lzc.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://moi.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vpj.sufxvd.cn

fclose(f);
来源：http://fgi.zdqjudy.top

[S12] C：写文件
来源：http://xkm.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yfi.cashguo.top

[S13] C：宏定义
来源：http://jfl.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://luy.tarul.cn

[S14] C：枚举
来源：http://oxl.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://yhp.fehbvm.com

[S15] C：类型转换
来源：http://kwv.hcnkem.com

(double) a / b
来源：http://yec.hcnkem.com

[S16] C：位操作置位
来源：http://aed.shzxlz.cn

x |= (1 << 3);
来源：http://jba.cashguo.top

[S17] C：安全拼接字符串
来源：http://olc.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vbl.iojbl.cn

[S18] C：命令行参数
来源：http://ctx.sxryk.cn

int main(int argc, char **argv)
来源：http://ymt.dianchejie.cn

[S19] C：快速排序
来源：http://reb.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://piy.zhongyouzk.top

[S20] C：二分查找
来源：http://jys.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hsf.meibo888.top

[S21] C：字符类别判断
来源：http://tob.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yun.fktsv.cn

[S22] C：字符串转数字
来源：http://ezl.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://pdc.jinqigfzy.top

[S23] C：随机数
来源：http://isf.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://byg.ydjk.org.cn

[S24] C：获取本地时间
来源：http://ihg.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ikl.uphjek.com

[S25] C：内存拷贝
来源：http://dzn.uphjek.com

memcpy(dst, src, n);
来源：http://jhl.zycfv.cn

[S26] C：内存清零
来源：http://kda.xziqi.cn

memset(a, 0, sizeof a);
来源：http://cjz.cqqwz.cn

[S27] C：定义常量
来源：http://xth.yonumen.top

const double PI = 3.14159;
来源：http://dpq.yj202588.top

[S28] C：静态变量
来源：http://aqf.ctjpmb.com

static int counter = 0;
来源：http://bwj.zhoulong.xyz

[S29] C：变参函数
来源：http://fyz.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rim.zhijiandao.cn

[S30] C：头文件保护
来源：http://ffv.jinqigfzy.top

#ifndef X_H
来源：http://kfg.ydjk.org.cn

#define X_H
来源：http://pfn.kuanghao11.cn

#endif
来源：http://bzg.vehdjk.com

[S31] C++：Hello World
来源：http://uwc.ctjpmb.com

#include <iostream>
来源：http://znj.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://azh.ydjk.org.cn

[S32] C++：字符串
来源：http://oqf.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://psu.iojbl.cn

[S33] C++：vector 增删
来源：http://qxk.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rcd.sufxvd.cn

[S34] C++：遍历 vector
来源：http://paa.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://bng.0kj1m.cn

[S35] C++：map
来源：http://orc.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ngh.yuxming.cn

[S36] C++：unordered_map
来源：http://gzy.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlu.cashguo.top

[S37] C++：set
来源：http://xty.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iqm.iojbl.cn

[S38] C++：排序
来源：http://qbd.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://duz.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://cvy.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kjv.chenzaomai.com

[S40] C++：查找元素
来源：http://vxv.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rdp.jiagoushi.top

[S41] C++：类与构造函数
来源：http://tue.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cxd.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://kco.sweek.top

class B : public Base { public: void f() override {} };
来源：http://puv.yj20258888.top

[S43] C++：智能指针
来源：http://nvx.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://wxr.yuanzhike.top

[S44] C++：引用传参
来源：http://dkf.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://ysw.cqqwz.cn

[S45] C++：lambda
来源：http://gwg.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://fxf.hywenlv.cn

[S46] C++：函数模板
来源：http://qhc.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zoy.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://kbx.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pqm.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://dhv.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://ahi.yvedp.cn

while (std::getline(in, line)) { }
来源：http://iwo.epnwcf.com

[S49] C++：写文件
来源：http://ldm.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jav.yueranfly.top

[S50] C++：格式化数字
来源：http://qnu.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://znr.daria6918.cn

[S51] C++：显式类型转换
来源：http://fwu.zhijiandao.cn

static_cast<double>(a) / b
来源：http://eeh.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://fvc.fzhhl.top

int size() const noexcept { return n_; }
来源：http://ary.kuanghao11.cn

[S53] C++：移动语义
来源：http://kvu.birdmap.top

std::vector<int> w = std::move(v);
来源：http://ujw.vqdsnc.cn

[S54] C++：异常处理
来源：http://vgn.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://owj.xuanzx.com

[S55] C++：结构化绑定
来源：http://pas.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vow.hnxiangtu.top

[S56] C++：optional
来源：http://szh.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cua.shzxlz.cn

[S57] C++：编译期常量
来源：http://hcg.nwbrower.top

constexpr int N = 10;
来源：http://dve.hesvh.cn

[S58] C++：命名空间
来源：http://fwt.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://swb.shangyingyoupin.top

[S59] C++：静态断言
来源：http://oam.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jpp.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://oad.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://khf.ywan-chungtsiang.top

================================================================================
来源：http://kaw.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wwp.xuanzx.com

================================================================================
来源：http://yzz.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://gud.fzhhl.top

println("Hello")
来源：http://mmt.havefunace.top

[T02] Kotlin：变量
来源：http://amd.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qkq.sjlbkw.cn


<!-- 参考信息 -->