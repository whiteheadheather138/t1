代发 wailian999

set -euo pipefail
来源：http://byt.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://xqb.pycfn.com

name="Tom"; echo "$name"
来源：http://cnf.chenlongwang.top

[R03] 只读变量
来源：http://vee.yfazqb.com

readonly PI=3.14
来源：http://swa.yvedp.cn

[R04] 位置参数
来源：http://knt.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fly.zdqjudy.top

[R05] 参数默认值
来源：http://gvp.ywan-chungtsiang.top

name="${1:-default}"
来源：http://ydr.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://bsg.ivvv.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://esu.epnwcf.com

[R07] if 判断文件
来源：http://xuo.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://azv.dianchejie.cn

[R08] 数值比较
来源：http://ydx.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://kcu.dashuyun.cn

[R09] 字符串比较
来源：http://zln.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mar.aibaodan.cn

[R10] 正则匹配
来源：http://xgb.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://znc.bbcook.cn

[R11] case 多分支
来源：http://gaa.yanxiufei.cn

case "$1" in
来源：http://unq.pycfn.com

start) echo "启动" ;;
来源：http://oxc.xziqi.cn

stop)  echo "停止" ;;
来源：http://ruo.sxryk.cn

*)     echo "未知命令" ;;
来源：http://jed.smart0.xyz

esac
来源：http://bcv.9152youxi.cn

[R12] for 遍历文件
来源：http://bhf.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://cdz.ydzc1.top

[R13] for 计数循环
来源：http://pae.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://vun.jyoumei.cn

[R14] C 风格 for
来源：http://oht.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hgb.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://xyl.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://poh.kuanghao11.cn

[R16] until 等待条件
来源：http://jxb.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ifk.quarkkingdee.top

[R17] 数组定义与取值
来源：http://wfi.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://vlc.xuanzx.com

[R18] 遍历数组
来源：http://qak.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tpn.sweek.top

[R19] 数组长度
来源：http://zth.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://rnz.jyoumei.cn

[R20] 关联数组（字典）
来源：http://cnn.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://koi.chenzaomai.com

[R21] 字符串长度
来源：http://nza.shanyushiyangtech.top

echo "${#s}"
来源：http://ftk.gotoacloud.top

[R22] 截取子串
来源：http://sul.ctjpmb.com

echo "${s:0:5}"
来源：http://fqz.jqgufenzy.top

[R23] 字符串替换
来源：http://vrq.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://alx.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://pcl.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://szi.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://tjn.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sjj.zhiwuduotai.top

[R26] 命令替换
来源：http://zdz.316326.xyz

now=$(date +%F); echo "$now"
来源：http://xdk.ybcxt.top

[R27] 算术展开
来源：http://czl.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://zmi.dashuyun.cn

[R28] 浮点运算
来源：http://une.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://fcb.ydzc1.top

[R29] 定义函数
来源：http://bkp.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ibk.mhx1999.top

[R30] 函数返回状态码
来源：http://gcv.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://ydi.jyoumei.cn

[R31] 局部变量
来源：http://vob.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://vyr.aibaodan.cn

[R32] 参数个数校验
来源：http://glb.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cpm.cashguo.top

[R33] 捕获错误并提示行号
来源：http://wlp.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yhg.pycfn.com

[R34] 退出时清理
来源：http://tai.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fmm.pengpengdd.cyou

[R35] 后台执行并等待
来源：http://vdb.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bqo.hcnkem.com

[R36] 并发执行多个任务
来源：http://gey.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cck.hysaishi.cn

[R37] 把输出赋给变量
来源：http://igf.yangfankeji.com

files=$(ls -1)
来源：http://ltt.yj20258888.top

[R38] 管道串联
来源：http://ztk.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://mzz.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://xod.andypj.xyz

cmd > out.log 2>&1
来源：http://woh.sysykeji.top

[R40] 追加写日志
来源：http://lke.iojbl.cn

echo "log" >> out.log
来源：http://hnz.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://yol.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://luw.zhijiandao.cn

[R42] 输入重定向
来源：http://pdt.fktsv.cn

wc -l < a.txt
来源：http://xvl.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://pze.sufxvd.cn

find . -name "*.log" -type f
来源：http://ksa.guannengcc.top

[R44] 按修改时间查找
来源：http://ipg.fehbvm.com

find . -mtime -7 -type f
来源：http://tya.daria6918.cn

[R45] 批量删除
来源：http://ulr.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://kgx.aizwys.cn

[R46] 递归替换文件内容
来源：http://tee.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eah.0kj1m.cn

[R47] sed 单行替换
来源：http://gcz.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://oxm.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://qkt.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://ywi.cashguo.top

[R49] awk 带条件
来源：http://nqh.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uze.guowangkeji.top

[R50] awk 求和
来源：http://lpy.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://znt.nwbrower.top

[R51] 排序去重取前几
来源：http://kri.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kjb.havefunace.top

[R52] 统计行数
来源：http://jgp.jyoumei.cn

wc -l a.txt
来源：http://jtj.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://yjj.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ust.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://byv.xinyue.icu

diff a.txt b.txt
来源：http://png.shangyingyoupin.top

[R55] 压缩与解压
来源：http://gdu.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcs.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://wth.snrcjt.cn

scp file user@host:/path/
来源：http://qse.zhiwuduotai.top

[R57] 远程执行命令
来源：http://duo.yongpay.top

ssh user@host 'uptime'
来源：http://csu.bjfxy.top

[R58] 下载文件
来源：http://keq.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tcj.zhijiandao.cn

[R59] 发 POST JSON
来源：http://pzw.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gwl.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://wom.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qya.gogol.net.cn

[R61] 磁盘占用
来源：http://cbp.jlsjyb.cn

df -h;  du -sh *
来源：http://llg.hesvh.cn

[R62] 找最占空间的文件
来源：http://dxg.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://yyb.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://aar.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://mje.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://tad.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://grn.cucudq.cn

[R65] 查看端口占用
来源：http://ppf.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xpi.c1oappe.top

[R66] 定时任务
来源：http://aog.shuidangran.top

crontab -e;  crontab -l
来源：http://vud.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://iai.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://ugb.fzhhl.top

[R68] 计算文件校验值
来源：http://kdd.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://snx.cashguo.top

[R69] 生成随机密码
来源：http://ykn.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://xjw.ydjk.org.cn

[R70] 时间戳与互转
来源：http://mte.cashguo.top

date +%s;  date -d @1700000000
来源：http://jnk.chenjidiqi.icu

[R71] 日期格式化
来源：http://rot.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ikw.dianchejie.cn

[R72] 等待端口就绪
来源：http://ivp.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://tok.birdmap.top

[R73] 分割大日志
来源：http://xjc.svipenyu.cn

split -l 1000 big.log part_
来源：http://sef.cucudq.cn

[R74] 批量重命名
来源：http://qom.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fod.9152youxi.cn

[R75] 导出环境变量
来源：http://wgi.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://czj.hongshengwenyu.top

[R76] 使用临时文件
来源：http://eta.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fza.zycfv.cn

[R77] 读取用户输入
来源：http://fik.hysaishi.cn

read -rp "请输入: " ans
来源：http://jsl.hywenlv.cn

[R78] 交互式菜单
来源：http://gtw.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wny.gogol.net.cn

[R79] 解析命令行选项
来源：http://amm.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zqz.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://ats.daxiang520.top

time ./run.sh
来源：http://lca.cucudq.cn

================================================================================
来源：http://gbw.haohaochexian.top

S. C / C++ 专题
来源：http://yzg.tarul.cn

================================================================================
来源：http://bnw.jqgfzy.top

[S01] C：Hello World
来源：http://orh.daria6918.cn

#include <stdio.h>
来源：http://cbg.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vvf.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://oba.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://gic.chenlongwang.top

[S03] C：读入整数
来源：http://qey.xylfe.cn

int x; scanf("%d", &x);
来源：http://glf.cdnleiting.top

[S04] C：字符串复制
来源：http://fid.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nrq.tian-w.cn

[S05] C：字符串长度
来源：http://lid.sweek.top

strlen(s)
来源：http://vpj.sxryk.cn

[S06] C：字符串比较
来源：http://xno.tianlin.xyz

strcmp(a, b) == 0
来源：http://jcg.hnqzz.top

[S07] C：数组遍历求和
来源：http://omf.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mur.yj20258.top

[S08] C：动态内存分配与释放
来源：http://kbm.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kkw.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://bwm.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ckq.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://jzd.jianghu66.top

int *p = &a;  *p = 5;
来源：http://xmm.gogol.net.cn

[S11] C：逐行读文件
来源：http://rxz.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://wry.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kib.haohaochexian.top

fclose(f);
来源：http://sno.hammf.cn

[S12] C：写文件
来源：http://jgj.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wqm.hywenlv.cn

[S13] C：宏定义
来源：http://qtp.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cvk.birdmap.top

[S14] C：枚举
来源：http://ykz.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://abf.fanxiaobao.xyz

[S15] C：类型转换
来源：http://ani.gotoacloud.top

(double) a / b
来源：http://vam.gzhubu.top

[S16] C：位操作置位
来源：http://uhf.nanxuanxn.top

x |= (1 << 3);
来源：http://let.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://mfo.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nfw.gaohongyu789.top

[S18] C：命令行参数
来源：http://rca.hammf.cn

int main(int argc, char **argv)
来源：http://fsr.fktsv.cn

[S19] C：快速排序
来源：http://cmi.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rcg.zdqjudy.top

[S20] C：二分查找
来源：http://ooc.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ygb.zhoulong.xyz

[S21] C：字符类别判断
来源：http://mam.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iiv.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://hnn.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nbg.zhaomingkeji.xyz

[S23] C：随机数
来源：http://pkq.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ysj.bbcook.cn

[S24] C：获取本地时间
来源：http://cup.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://phk.andypj.xyz

[S25] C：内存拷贝
来源：http://tqq.hnxiangtu.top

memcpy(dst, src, n);
来源：http://ssf.yangfankeji.com

[S26] C：内存清零
来源：http://nfj.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://pux.feifeiyinyue.top

[S27] C：定义常量
来源：http://wgb.guowangkeji.top

const double PI = 3.14159;
来源：http://akc.jqgufenzy.top

[S28] C：静态变量
来源：http://zjf.uphjek.com

static int counter = 0;
来源：http://mdl.chenzaomai.com

[S29] C：变参函数
来源：http://nqa.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://amt.zdbjq.cn

[S30] C：头文件保护
来源：http://ubu.nanxinkj.top

#ifndef X_H
来源：http://rqt.fzhhl.top

#define X_H
来源：http://cvo.fzhhl.top

#endif
来源：http://kah.tian-w.cn

[S31] C++：Hello World
来源：http://esf.cucudq.cn

#include <iostream>
来源：http://rhf.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://kiq.yuxming.cn

[S32] C++：字符串
来源：http://xch.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://foi.ybcxt.top

[S33] C++：vector 增删
来源：http://wio.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tys.ydzc1.top

[S34] C++：遍历 vector
来源：http://wkn.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://emi.sysykeji.top

[S35] C++：map
来源：http://muf.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vsu.yanxiufei.cn

[S36] C++：unordered_map
来源：http://tdn.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://beq.sjlbkw.cn

[S37] C++：set
来源：http://apv.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqg.fanxiaobao.xyz

[S38] C++：排序
来源：http://bel.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://ung.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://wch.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxh.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://goq.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ibb.zhixingplan.top

[S41] C++：类与构造函数
来源：http://eso.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aiw.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://oev.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://nlb.birdmap.top

[S43] C++：智能指针
来源：http://lle.gaohongyu789.top

auto p = std::make_unique<int>(5);
来源：http://tip.sweek.top

[S44] C++：引用传参
来源：http://kmb.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://kod.iojbl.cn

[S45] C++：lambda
来源：http://hav.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://gvh.xylfe.cn

[S46] C++：函数模板
来源：http://puf.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mij.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://bdk.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qyx.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://bqw.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://rpe.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://uyz.jinghuilouyu.cn

[S49] C++：写文件
来源：http://fjc.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cvd.hesvh.cn

[S50] C++：格式化数字
来源：http://hxn.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ndq.snrcjt.cn

[S51] C++：显式类型转换
来源：http://rsv.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://nxt.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://wrp.jianghu66.top

int size() const noexcept { return n_; }
来源：http://daq.jinqigfzy.top

[S53] C++：移动语义
来源：http://dbw.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://irq.kuanghao11.cn

[S54] C++：异常处理
来源：http://bhq.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cav.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://atv.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gnh.fengsongda.top

[S56] C++：optional
来源：http://ttn.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fui.fehbvm.com

[S57] C++：编译期常量
来源：http://lvm.havefunace.top

constexpr int N = 10;
来源：http://oll.yuanzhike.top

[S58] C++：命名空间
来源：http://wkz.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://qmw.fengsongda.top

[S59] C++：静态断言
来源：http://whs.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gqq.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ryg.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eev.bbcook.cn

================================================================================
来源：http://sti.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nkx.haohaochexian.top

================================================================================
来源：http://eyy.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://lmb.xuetiantiany.cn

println("Hello")
来源：http://mva.0kj1m.cn

[T02] Kotlin：变量
来源：http://wvd.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://suq.gotoacloud.top


<!-- 参考信息 -->