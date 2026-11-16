代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pbm.nanxinkj.top

[Q90] 生成序号列
来源：http://oyr.yueranfly.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kxh.0kj1m.cn

================================================================================
来源：http://kix.c1oappe.top

R. Bash 专题
来源：http://sbd.sysykeji.top

================================================================================
来源：http://jqr.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://eyx.jyoumei.cn

#!/usr/bin/env bash
来源：http://cem.gogol.net.cn

set -euo pipefail
来源：http://hze.sufxvd.cn

[R02] 变量赋值与使用
来源：http://cll.yuanzhike.top

name="Tom"; echo "$name"
来源：http://htj.yfazqb.com

[R03] 只读变量
来源：http://zbl.yangfankeji.com

readonly PI=3.14
来源：http://itc.meibo888.top

[R04] 位置参数
来源：http://cwb.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iwr.zhoulong.xyz

[R05] 参数默认值
来源：http://goc.zdbjq.cn

name="${1:-default}"
来源：http://xza.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://uvu.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://csq.svipenyu.cn

[R07] if 判断文件
来源：http://eyd.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://atp.9152youxi.cn

[R08] 数值比较
来源：http://zki.jinqigfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ypm.yj202588.top

[R09] 字符串比较
来源：http://lav.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ejv.cdnleiting.top

[R10] 正则匹配
来源：http://cjo.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tsh.jinghuilouyu.cn

[R11] case 多分支
来源：http://yhs.fengsongda.top

case "$1" in
来源：http://xzj.redwolf501.top

start) echo "启动" ;;
来源：http://apr.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://vdp.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://jpc.hnqzz.top

esac
来源：http://pzl.zycfv.cn

[R12] for 遍历文件
来源：http://oix.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://tln.redwolf501.top

[R13] for 计数循环
来源：http://cyu.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://kha.xinyue.icu

[R14] C 风格 for
来源：http://ezl.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nqk.yongpay.top

[R15] while 逐行读文件
来源：http://iib.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bpw.yangfankeji.com

[R16] until 等待条件
来源：http://qei.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hhi.hesvh.cn

[R17] 数组定义与取值
来源：http://wkg.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://msx.jqgufenzy.top

[R18] 遍历数组
来源：http://hcz.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qak.ehwqpu.com

[R19] 数组长度
来源：http://rap.gaohongyu789.top

echo "${#arr[@]}"
来源：http://qba.haohaochexian.top

[R20] 关联数组（字典）
来源：http://azu.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lpp.nanxinkj.top

[R21] 字符串长度
来源：http://fai.chenlongwang.top

echo "${#s}"
来源：http://acg.guannengcc.top

[R22] 截取子串
来源：http://nfc.sxryk.cn

echo "${s:0:5}"
来源：http://ihy.gzhubu.top

[R23] 字符串替换
来源：http://fqz.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://saq.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://hup.shanyushiyangtech.top

echo "${s^^}"; echo "${s,,}"
来源：http://yzg.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://dbj.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkt.epnwcf.com

[R26] 命令替换
来源：http://nfq.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://zaq.zhoulong.xyz

[R27] 算术展开
来源：http://zvq.smart0.xyz

echo $((1 + 2 * 3))
来源：http://yil.bjfxy.top

[R28] 浮点运算
来源：http://nky.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://tgw.hnxiangtu.top

[R29] 定义函数
来源：http://mpb.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ayi.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://eig.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://pzk.hongshengwenyu.top

[R31] 局部变量
来源：http://rex.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://scw.sweek.top

[R32] 参数个数校验
来源：http://hyk.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://udp.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://rez.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zqq.havefunace.top

[R34] 退出时清理
来源：http://aow.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ipc.hcnkem.com

[R35] 后台执行并等待
来源：http://kcj.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ohm.tian-w.cn

[R36] 并发执行多个任务
来源：http://qlt.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pid.tarul.cn

[R37] 把输出赋给变量
来源：http://jpx.svipenyu.cn

files=$(ls -1)
来源：http://qvn.9152youxi.cn

[R38] 管道串联
来源：http://rur.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://fgq.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://rdv.zdqjudy.top

cmd > out.log 2>&1
来源：http://yro.yuanzhike.top

[R40] 追加写日志
来源：http://fze.nanxinkj.top

echo "log" >> out.log
来源：http://rcd.52xcode.cn

[R41] 丢弃输出
来源：http://ain.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://ufb.ctjpmb.com

[R42] 输入重定向
来源：http://ghq.dashuyun.cn

wc -l < a.txt
来源：http://osy.gaohongyu789.top

[R43] 按名字查找文件
来源：http://jeg.gzhubu.top

find . -name "*.log" -type f
来源：http://qwx.tianlin.xyz

[R44] 按修改时间查找
来源：http://uns.52xcode.cn

find . -mtime -7 -type f
来源：http://ygc.fanxiaobao.xyz

[R45] 批量删除
来源：http://bvd.vehdjk.com

find . -name "*.tmp" -delete
来源：http://qmo.chenzaomai.com

[R46] 递归替换文件内容
来源：http://set.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dby.c1oappe.top

[R47] sed 单行替换
来源：http://bps.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://hcb.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://uey.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://iwl.aibaodan.cn

[R49] awk 带条件
来源：http://efq.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qmf.pycfn.com

[R50] awk 求和
来源：http://gxz.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://zfn.ivvv.top

[R51] 排序去重取前几
来源：http://pbx.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ctd.fanxiaobao.xyz

[R52] 统计行数
来源：http://wvn.yueranfly.top

wc -l a.txt
来源：http://mnc.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://llr.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kaz.guannengcc.top

[R54] 比较两个文件
来源：http://jvk.nwbrower.top

diff a.txt b.txt
来源：http://ffw.52xcode.cn

[R55] 压缩与解压
来源：http://nts.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bkv.yuanzhike.top

[R56] 远程拷贝
来源：http://nil.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://lqk.c1oappe.top

[R57] 远程执行命令
来源：http://hzl.yuxming.cn

ssh user@host 'uptime'
来源：http://tye.nwbrower.top

[R58] 下载文件
来源：http://lhf.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kcc.cqqwz.cn

[R59] 发 POST JSON
来源：http://kbc.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://por.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://xzk.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jbk.gotoacloud.top

[R61] 磁盘占用
来源：http://kpz.feifeiyinyue.top

df -h;  du -sh *
来源：http://bar.pycfn.com

[R62] 找最占空间的文件
来源：http://hcw.tanke756.top

du -ah . | sort -rh | head -10
来源：http://vwd.shuidangran.top

[R63] 内存与进程
来源：http://dzm.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://gfd.aizwys.cn

[R64] 结束进程
来源：http://hqt.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://ndg.yongpay.top

[R65] 查看端口占用
来源：http://lnp.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://byx.jqgufenzy.top

[R66] 定时任务
来源：http://bae.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://vzx.xylfe.cn

[R67] 生成随机十六进制串
来源：http://vre.zycfv.cn

openssl rand -hex 16
来源：http://ouo.aizwys.cn

[R68] 计算文件校验值
来源：http://zko.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://tyq.ppjwa.cn

[R69] 生成随机密码
来源：http://ivc.bbcook.cn

head -c 16 /dev/urandom | base64
来源：http://vav.epnwcf.com

[R70] 时间戳与互转
来源：http://ykz.c1oappe.top

date +%s;  date -d @1700000000
来源：http://mnx.shangyingyoupin.top

[R71] 日期格式化
来源：http://iif.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rkm.tanke756.top

[R72] 等待端口就绪
来源：http://lxr.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://osj.ppjwa.cn

[R73] 分割大日志
来源：http://dco.xinyue.icu

split -l 1000 big.log part_
来源：http://yvo.ehwqpu.com

[R74] 批量重命名
来源：http://fus.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://otl.ehwqpu.com

[R75] 导出环境变量
来源：http://doo.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://fue.ehwqpu.com

[R76] 使用临时文件
来源：http://hts.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qfg.ivvv.top

[R77] 读取用户输入
来源：http://wcw.tianlin.xyz

read -rp "请输入: " ans
来源：http://fir.52xcode.cn

[R78] 交互式菜单
来源：http://tum.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qxe.zhixingplan.top

[R79] 解析命令行选项
来源：http://pal.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xde.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://esm.cucudq.cn

time ./run.sh
来源：http://ufo.gaohongyu789.top

================================================================================
来源：http://iat.zhoulong.xyz

S. C / C++ 专题
来源：http://lft.yuanzhike.top

================================================================================
来源：http://hof.zhijiandao.cn

[S01] C：Hello World
来源：http://ftk.daria6918.cn

#include <stdio.h>
来源：http://ers.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://arg.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://wuc.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://bdy.xylfe.cn

[S03] C：读入整数
来源：http://vua.yj20258.top

int x; scanf("%d", &x);
来源：http://bso.sjlbkw.cn

[S04] C：字符串复制
来源：http://jft.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://epy.vehdjk.com

[S05] C：字符串长度
来源：http://xyj.hnxiangtu.top

strlen(s)
来源：http://pae.iojbl.cn

[S06] C：字符串比较
来源：http://nul.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://suv.zycfv.cn

[S07] C：数组遍历求和
来源：http://wtd.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eel.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://rcy.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qsf.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://jrj.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wdh.yangfankeji.com

[S10] C：指针与解引用
来源：http://dgs.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://qha.yuxming.cn

[S11] C：逐行读文件
来源：http://ago.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://fev.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qnk.xingfuxueyuan.xyz

fclose(f);
来源：http://nkx.sxryk.cn

[S12] C：写文件
来源：http://gwi.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qqg.52xcode.cn

[S13] C：宏定义
来源：http://kam.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eob.fzhhl.top

[S14] C：枚举
来源：http://gbm.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://vcy.cashguo.top

[S15] C：类型转换
来源：http://hco.fzhhl.top

(double) a / b
来源：http://vna.hongshengwenyu.top

[S16] C：位操作置位
来源：http://hmr.bbcook.cn

x |= (1 << 3);
来源：http://ilh.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://cgs.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rgi.shzxlz.cn

[S18] C：命令行参数
来源：http://auw.sufxvd.cn

int main(int argc, char **argv)
来源：http://rbv.tianlin.xyz

[S19] C：快速排序
来源：http://vyj.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://umw.xziqi.cn

[S20] C：二分查找
来源：http://cxg.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qlq.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://alx.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ojj.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://qmq.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://qbw.shangyingyoupin.top

[S23] C：随机数
来源：http://awa.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kae.quarkkingdee.top

[S24] C：获取本地时间
来源：http://vjn.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://azi.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://boa.shuidangran.top

memcpy(dst, src, n);
来源：http://ydj.ehwqpu.com

[S26] C：内存清零
来源：http://efs.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://zum.yj20258.top

[S27] C：定义常量
来源：http://hko.zycfv.cn

const double PI = 3.14159;
来源：http://ibu.feifeiyinyue.top

[S28] C：静态变量
来源：http://jev.tarul.cn

static int counter = 0;
来源：http://dta.gotoacloud.top

[S29] C：变参函数
来源：http://xze.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kcz.yonumen.top

[S30] C：头文件保护
来源：http://xbd.nanxinkj.top

#ifndef X_H
来源：http://jar.aibaodan.cn

#define X_H
来源：http://jgy.haohaochexian.top

#endif
来源：http://yrc.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://kdi.shanyushiyangtech.top

#include <iostream>
来源：http://ziy.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://azi.tian-w.cn

[S32] C++：字符串
来源：http://gwg.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://cii.sysykeji.top

[S33] C++：vector 增删
来源：http://uga.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsi.svipenyu.cn

[S34] C++：遍历 vector
来源：http://ztk.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://ivl.yongpay.top

[S35] C++：map
来源：http://qec.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zod.smart0.xyz

[S36] C++：unordered_map
来源：http://hkd.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gag.havefunace.top

[S37] C++：set
来源：http://lfc.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://soa.zhijiandao.cn

[S38] C++：排序
来源：http://xlc.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://chr.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://zlb.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bxp.jinqigufen.top

[S40] C++：查找元素
来源：http://arw.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zed.yvedp.cn

[S41] C++：类与构造函数
来源：http://pzu.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vci.shuidangran.top

[S42] C++：继承与虚函数
来源：http://ozw.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://mqe.ppjwa.cn

[S43] C++：智能指针
来源：http://mmp.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://dom.jlsjyb.cn

[S44] C++：引用传参
来源：http://guj.yueranfly.top

void inc(int &x) { ++x; }
来源：http://lrd.xuetiantiany.cn

[S45] C++：lambda
来源：http://ewd.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://dwe.hnxiangtu.top

[S46] C++：函数模板
来源：http://qzm.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qil.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://tsl.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hki.hesvh.cn

[S48] C++：逐行读文件
来源：http://mvd.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://fkf.tarul.cn

while (std::getline(in, line)) { }
来源：http://ang.cashguo.top

[S49] C++：写文件
来源：http://rua.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://emo.cucudq.cn

[S50] C++：格式化数字
来源：http://sqz.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://got.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://jri.daria6918.cn

static_cast<double>(a) / b
来源：http://ktv.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://kdj.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://fnj.hnqzz.top

[S53] C++：移动语义
来源：http://pho.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://fkn.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://kzn.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bmn.zycfv.cn

[S55] C++：结构化绑定
来源：http://ycm.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://uhs.yj20258.top

[S56] C++：optional
来源：http://cdh.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gyd.jinqigfzy.top

[S57] C++：编译期常量
来源：http://pzo.havefunace.top

constexpr int N = 10;
来源：http://enn.nanxuanxn.top

[S58] C++：命名空间
来源：http://jmg.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://bmm.dashuyun.cn

[S59] C++：静态断言
来源：http://knk.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zwk.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://xvq.zdbjq.cn


<!-- 参考信息 -->