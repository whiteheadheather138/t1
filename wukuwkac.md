代发 wailian999

R. Bash 专题
来源：http://nck.zycfv.cn

================================================================================
来源：http://kgf.tarul.cn

[R01] shebang 与严格模式
来源：http://cxe.xylfe.cn

#!/usr/bin/env bash
来源：http://rix.xuanzx.com

set -euo pipefail
来源：http://qqy.dianchejie.cn

[R02] 变量赋值与使用
来源：http://pvh.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://mqu.ehwqpu.com

[R03] 只读变量
来源：http://ihc.yuxming.cn

readonly PI=3.14
来源：http://jvo.hesvh.cn

[R04] 位置参数
来源：http://cyt.mhx1999.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mba.cqqwz.cn

[R05] 参数默认值
来源：http://zqj.jinyuanbaomall.cn

name="${1:-default}"
来源：http://tkr.tian-w.cn

[R06] 判断命令是否存在
来源：http://qyt.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pza.sxryk.cn

[R07] if 判断文件
来源：http://wxa.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jix.dianchejie.cn

[R08] 数值比较
来源：http://hca.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://quu.hcnkem.com

[R09] 字符串比较
来源：http://zhc.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ngg.shzxlz.cn

[R10] 正则匹配
来源：http://qss.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xjz.zhijiandao.cn

[R11] case 多分支
来源：http://sds.redwolf501.top

case "$1" in
来源：http://syn.zhijiandao.cn

start) echo "启动" ;;
来源：http://yfd.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://hor.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://jtt.svipenyu.cn

esac
来源：http://dyk.kuanghao11.cn

[R12] for 遍历文件
来源：http://yde.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://akw.jyoumei.cn

[R13] for 计数循环
来源：http://lnk.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://lnh.jinqigfzy.top

[R14] C 风格 for
来源：http://pkb.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lwv.cqqwz.cn

[R15] while 逐行读文件
来源：http://vlc.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fof.fanxiaobao.xyz

[R16] until 等待条件
来源：http://iix.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mdz.sweek.top

[R17] 数组定义与取值
来源：http://woe.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://not.hywenlv.cn

[R18] 遍历数组
来源：http://ocm.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wie.jyoumei.cn

[R19] 数组长度
来源：http://iqh.yvedp.cn

echo "${#arr[@]}"
来源：http://tne.daxiang520.top

[R20] 关联数组（字典）
来源：http://nvo.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qke.vehdjk.com

[R21] 字符串长度
来源：http://bkd.vehdjk.com

echo "${#s}"
来源：http://uag.bbcook.cn

[R22] 截取子串
来源：http://uqx.gzhubu.top

echo "${s:0:5}"
来源：http://vyz.daxiang520.top

[R23] 字符串替换
来源：http://gcl.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vtu.ybcxt.top

[R24] 大小写转换
来源：http://pgq.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://und.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://qmd.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ydb.zdqjudy.top

[R26] 命令替换
来源：http://rnb.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://trl.yonumen.top

[R27] 算术展开
来源：http://nqa.yueranfly.top

echo $((1 + 2 * 3))
来源：http://tre.yonumen.top

[R28] 浮点运算
来源：http://gnu.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://gvf.jinyuanbaomall.cn

[R29] 定义函数
来源：http://mqn.jlsjyb.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lhd.yfazqb.com

[R30] 函数返回状态码
来源：http://jmf.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://qhd.pengpengdd.cyou

[R31] 局部变量
来源：http://cqh.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://quu.yfazqb.com

[R32] 参数个数校验
来源：http://xun.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bmj.uphjek.com

[R33] 捕获错误并提示行号
来源：http://nmx.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dap.jianghu66.top

[R34] 退出时清理
来源：http://fbb.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cfx.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://vfe.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://vmi.yfazqb.com

[R36] 并发执行多个任务
来源：http://kwi.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cbo.hammf.cn

[R37] 把输出赋给变量
来源：http://rxb.jlsjyb.cn

files=$(ls -1)
来源：http://rkn.cashguo.top

[R38] 管道串联
来源：http://ehp.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://cju.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://srk.hnqzz.top

cmd > out.log 2>&1
来源：http://zen.ydzc1.top

[R40] 追加写日志
来源：http://ssq.cucudq.cn

echo "log" >> out.log
来源：http://eyb.cqqwz.cn

[R41] 丢弃输出
来源：http://lng.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://qml.mhx1999.top

[R42] 输入重定向
来源：http://kek.daria6918.cn

wc -l < a.txt
来源：http://dve.zycfv.cn

[R43] 按名字查找文件
来源：http://azh.wangdashe.top

find . -name "*.log" -type f
来源：http://zgq.bjfxy.top

[R44] 按修改时间查找
来源：http://vlh.svipenyu.cn

find . -mtime -7 -type f
来源：http://spv.pycfn.com

[R45] 批量删除
来源：http://hlv.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://ecv.nanxinkj.top

[R46] 递归替换文件内容
来源：http://fza.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wpz.yonumen.top

[R47] sed 单行替换
来源：http://vji.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tns.dashuyun.cn

[R48] awk 取指定列
来源：http://jju.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://owr.jyoumei.cn

[R49] awk 带条件
来源：http://gow.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aco.daxiang520.top

[R50] awk 求和
来源：http://yxe.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://ghv.zdqjudy.top

[R51] 排序去重取前几
来源：http://bej.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ckg.zhoulong.xyz

[R52] 统计行数
来源：http://gqr.mhx1999.top

wc -l a.txt
来源：http://jwm.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://pct.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vcv.guowangkeji.top

[R54] 比较两个文件
来源：http://vbb.chenlongwang.top

diff a.txt b.txt
来源：http://zof.yj20258888.top

[R55] 压缩与解压
来源：http://iuz.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://prt.dashuyun.cn

[R56] 远程拷贝
来源：http://egc.tarul.cn

scp file user@host:/path/
来源：http://yxl.sweek.top

[R57] 远程执行命令
来源：http://jbx.9152youxi.cn

ssh user@host 'uptime'
来源：http://rwx.wangdashe.top

[R58] 下载文件
来源：http://fln.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sxd.yfazqb.com

[R59] 发 POST JSON
来源：http://ztm.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wnc.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://abu.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://usz.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://fka.xuetiantiany.cn

df -h;  du -sh *
来源：http://bng.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://amk.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://pek.zhixingplan.top

[R63] 内存与进程
来源：http://frq.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://cbe.sysykeji.top

[R64] 结束进程
来源：http://iey.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://wrq.yangfankeji.com

[R65] 查看端口占用
来源：http://owq.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kfy.guannengcc.top

[R66] 定时任务
来源：http://zjd.smart0.xyz

crontab -e;  crontab -l
来源：http://azy.sweek.top

[R67] 生成随机十六进制串
来源：http://gwv.hfpthk.cn

openssl rand -hex 16
来源：http://exy.ppjwa.cn

[R68] 计算文件校验值
来源：http://rex.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://xoh.jinqigfzy.top

[R69] 生成随机密码
来源：http://pff.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://zfa.jlsjyb.cn

[R70] 时间戳与互转
来源：http://fab.vehdjk.com

date +%s;  date -d @1700000000
来源：http://lti.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://gwf.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pjm.andypj.xyz

[R72] 等待端口就绪
来源：http://www.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rjh.cdnleiting.top

[R73] 分割大日志
来源：http://xgl.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://ukv.epnwcf.com

[R74] 批量重命名
来源：http://hpi.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iuo.quarkkingdee.top

[R75] 导出环境变量
来源：http://dpc.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://uab.fktsv.cn

[R76] 使用临时文件
来源：http://fgs.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://toz.nanxinkj.top

[R77] 读取用户输入
来源：http://wve.sjlbkw.cn

read -rp "请输入: " ans
来源：http://qpw.zdbjq.cn

[R78] 交互式菜单
来源：http://tsg.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://czc.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://kuv.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzx.yonumen.top

[R80] 查看脚本执行耗时
来源：http://xdn.ppjwa.cn

time ./run.sh
来源：http://lbm.kuanghao11.cn

================================================================================
来源：http://pjd.hfpthk.cn

S. C / C++ 专题
来源：http://nze.fengsongda.top

================================================================================
来源：http://zcu.cashguo.top

[S01] C：Hello World
来源：http://ebg.tianlin.xyz

#include <stdio.h>
来源：http://hsa.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rri.bbcook.cn

[S02] C：变量与格式化输出
来源：http://atp.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://rmd.yj202588.top

[S03] C：读入整数
来源：http://pkn.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://opm.c1oappe.top

[S04] C：字符串复制
来源：http://gur.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://nvy.smart0.xyz

[S05] C：字符串长度
来源：http://dmn.xingfuxueyuan.xyz

strlen(s)
来源：http://dzc.zhijiandao.cn

[S06] C：字符串比较
来源：http://ogb.fktsv.cn

strcmp(a, b) == 0
来源：http://zvt.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://mww.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mcj.yongpay.top

[S08] C：动态内存分配与释放
来源：http://qmm.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hfs.meibo888.top

[S09] C：结构体定义与初始化
来源：http://ako.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rsj.iojbl.cn

[S10] C：指针与解引用
来源：http://gif.pycfn.com

int *p = &a;  *p = 5;
来源：http://kgy.daria6918.cn

[S11] C：逐行读文件
来源：http://mfe.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://uxq.nanxuanxn.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hhc.jinyuanbaomall.cn

fclose(f);
来源：http://klv.zhiwuduotai.top

[S12] C：写文件
来源：http://kfg.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://edo.yueranfly.top

[S13] C：宏定义
来源：http://ggh.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jfg.gotoacloud.top

[S14] C：枚举
来源：http://yyl.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://vsv.quarkkingdee.top

[S15] C：类型转换
来源：http://ptu.cucudq.cn

(double) a / b
来源：http://mri.epnwcf.com

[S16] C：位操作置位
来源：http://fwo.fengsongda.top

x |= (1 << 3);
来源：http://kaw.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://mlf.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lyx.nwbrower.top

[S18] C：命令行参数
来源：http://yvw.hnxiangtu.top

int main(int argc, char **argv)
来源：http://oyd.mhx1999.top

[S19] C：快速排序
来源：http://vgq.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://kbf.gzhubu.top

[S20] C：二分查找
来源：http://vhm.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baj.hnqzz.top

[S21] C：字符类别判断
来源：http://ucn.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lio.zhongyouzk.top

[S22] C：字符串转数字
来源：http://eoz.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://wvt.sufxvd.cn

[S23] C：随机数
来源：http://uhk.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://whn.uphjek.com

[S24] C：获取本地时间
来源：http://jyq.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wda.hesvh.cn

[S25] C：内存拷贝
来源：http://ret.yueranfly.top

memcpy(dst, src, n);
来源：http://jhh.yfazqb.com

[S26] C：内存清零
来源：http://tpg.cucudq.cn

memset(a, 0, sizeof a);
来源：http://whg.hcnkem.com

[S27] C：定义常量
来源：http://vku.sjlbkw.cn

const double PI = 3.14159;
来源：http://vzf.uphjek.com

[S28] C：静态变量
来源：http://dpt.dashuyun.cn

static int counter = 0;
来源：http://xth.zhixingplan.top

[S29] C：变参函数
来源：http://gij.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kyp.zhongyouzk.top

[S30] C：头文件保护
来源：http://bdz.zhijiandao.cn

#ifndef X_H
来源：http://rwf.ybcxt.top

#define X_H
来源：http://pbm.cheryme.top

#endif
来源：http://htq.bbcook.cn

[S31] C++：Hello World
来源：http://sgr.yj20258888.top

#include <iostream>
来源：http://iyw.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://wde.sjlbkw.cn

[S32] C++：字符串
来源：http://ekh.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://cyf.yj20258888.top

[S33] C++：vector 增删
来源：http://wod.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qdv.ctjpmb.com

[S34] C++：遍历 vector
来源：http://gjp.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://cvk.sysykeji.top

[S35] C++：map
来源：http://gqo.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iyl.gotoacloud.top

[S36] C++：unordered_map
来源：http://ism.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tzt.fehbvm.com

[S37] C++：set
来源：http://lur.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jkw.wangshuangyany.cn

[S38] C++：排序
来源：http://mqo.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://rly.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://gdo.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jee.52xcode.cn

[S40] C++：查找元素
来源：http://ula.nanxinkj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xbg.ybcxt.top

[S41] C++：类与构造函数
来源：http://cbu.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tub.yfazqb.com

[S42] C++：继承与虚函数
来源：http://tnl.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://shv.jqgufenzy.top

[S43] C++：智能指针
来源：http://ewh.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://jsr.wangshuangyany.cn

[S44] C++：引用传参
来源：http://kgj.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://niz.zhijiandao.cn

[S45] C++：lambda
来源：http://cnb.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://apx.shzxlz.cn

[S46] C++：函数模板
来源：http://flw.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rfs.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://rpg.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bve.yuanzhike.top

[S48] C++：逐行读文件
来源：http://phb.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://wmd.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://pql.hesvh.cn

[S49] C++：写文件
来源：http://wlr.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zaf.havefunace.top

[S50] C++：格式化数字
来源：http://eeu.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ldg.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://vjv.fktsv.cn

static_cast<double>(a) / b
来源：http://qeo.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://cqt.cashguo.top

int size() const noexcept { return n_; }
来源：http://anf.nwbrower.top

[S53] C++：移动语义
来源：http://isg.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://qnh.zdbjq.cn

[S54] C++：异常处理
来源：http://bho.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gww.sufxvd.cn

[S55] C++：结构化绑定
来源：http://sqs.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ced.shuidangran.top

[S56] C++：optional
来源：http://mvs.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kbr.pycfn.com

[S57] C++：编译期常量
来源：http://sjx.aizwys.cn

constexpr int N = 10;
来源：http://irg.yongpay.top

[S58] C++：命名空间
来源：http://wty.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://uvz.316326.xyz

[S59] C++：静态断言
来源：http://otj.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://som.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://dwn.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ehs.jinghuilouyu.cn

================================================================================
来源：http://vvv.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://awi.redwolf501.top

================================================================================
来源：http://zcd.pengpengdd.cyou


<!-- 参考信息 -->