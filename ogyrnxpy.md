代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wbx.hammf.cn

[Q90] 生成序号列
来源：http://bxr.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kce.tian-w.cn

================================================================================
来源：http://cok.sufxvd.cn

R. Bash 专题
来源：http://agm.hcnkem.com

================================================================================
来源：http://rmu.yangfankeji.com

[R01] shebang 与严格模式
来源：http://jxl.pycfn.com

#!/usr/bin/env bash
来源：http://zxx.gaohongyu789.top

set -euo pipefail
来源：http://isd.cheryme.top

[R02] 变量赋值与使用
来源：http://gtr.fzhhl.top

name="Tom"; echo "$name"
来源：http://maz.ywan-chungtsiang.top

[R03] 只读变量
来源：http://dgr.yanxiufei.cn

readonly PI=3.14
来源：http://gdo.hnqzz.top

[R04] 位置参数
来源：http://tnr.hnqzz.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mmb.yuanzhike.top

[R05] 参数默认值
来源：http://ghs.shangyingyoupin.top

name="${1:-default}"
来源：http://qxg.hcnkem.com

[R06] 判断命令是否存在
来源：http://uoo.xuetiantiany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lco.daxiang520.top

[R07] if 判断文件
来源：http://hug.yfazqb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xaz.fktsv.cn

[R08] 数值比较
来源：http://aru.sufxvd.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://auw.yangfankeji.com

[R09] 字符串比较
来源：http://zhh.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hpb.ybcxt.top

[R10] 正则匹配
来源：http://zej.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zkt.sweek.top

[R11] case 多分支
来源：http://lcg.hnxiangtu.top

case "$1" in
来源：http://ugd.shzxlz.cn

start) echo "启动" ;;
来源：http://imq.nwbrower.top

stop)  echo "停止" ;;
来源：http://zht.yonumen.top

*)     echo "未知命令" ;;
来源：http://hfh.yanxiufei.cn

esac
来源：http://bvx.ivvv.top

[R12] for 遍历文件
来源：http://ltt.ctjpmb.com

for f in *.txt; do echo "$f"; done
来源：http://cnt.jiagoushi.top

[R13] for 计数循环
来源：http://gqh.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://mjb.havefunace.top

[R14] C 风格 for
来源：http://gjv.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kan.hesvh.cn

[R15] while 逐行读文件
来源：http://tpk.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dbj.birdmap.top

[R16] until 等待条件
来源：http://xqh.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://msu.feifeiyinyue.top

[R17] 数组定义与取值
来源：http://sgc.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://lqc.jlsjyb.cn

[R18] 遍历数组
来源：http://psu.zdqjudy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xqc.bjfxy.top

[R19] 数组长度
来源：http://tsm.dianchejie.cn

echo "${#arr[@]}"
来源：http://uda.yonumen.top

[R20] 关联数组（字典）
来源：http://uwh.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ubp.mhx1999.top

[R21] 字符串长度
来源：http://uai.9152youxi.cn

echo "${#s}"
来源：http://mqe.guowangkeji.top

[R22] 截取子串
来源：http://gpl.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://wom.fanxiaobao.xyz

[R23] 字符串替换
来源：http://dfy.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pnc.wangshuangyany.cn

[R24] 大小写转换
来源：http://aop.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://glm.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://muf.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrg.sjlbkw.cn

[R26] 命令替换
来源：http://ykb.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://faq.haohaochexian.top

[R27] 算术展开
来源：http://bjb.wangdashe.top

echo $((1 + 2 * 3))
来源：http://ejg.bbcook.cn

[R28] 浮点运算
来源：http://adc.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://bdr.chenjidiqi.icu

[R29] 定义函数
来源：http://nts.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pwa.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://rob.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://iew.zhongyouzk.top

[R31] 局部变量
来源：http://bza.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://omx.yfazqb.com

[R32] 参数个数校验
来源：http://pud.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mcz.uphjek.com

[R33] 捕获错误并提示行号
来源：http://frq.316326.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fre.jiagoushi.top

[R34] 退出时清理
来源：http://ywm.epnwcf.com

trap 'rm -f "$tmp"' EXIT
来源：http://adw.zhixingplan.top

[R35] 后台执行并等待
来源：http://qou.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xmd.jiagoushi.top

[R36] 并发执行多个任务
来源：http://mfa.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zwt.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://fzv.zycfv.cn

files=$(ls -1)
来源：http://xgq.shanyushiyangtech.top

[R38] 管道串联
来源：http://lrk.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://vfq.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://hfo.redwolf501.top

cmd > out.log 2>&1
来源：http://sdi.ybcxt.top

[R40] 追加写日志
来源：http://bqy.bbcook.cn

echo "log" >> out.log
来源：http://zrb.aibaodan.cn

[R41] 丢弃输出
来源：http://gew.bjfxy.top

cmd >/dev/null 2>&1
来源：http://kqw.gotoacloud.top

[R42] 输入重定向
来源：http://own.wangdashe.top

wc -l < a.txt
来源：http://shk.jinqigufen.top

[R43] 按名字查找文件
来源：http://igg.vehdjk.com

find . -name "*.log" -type f
来源：http://pwe.zycfv.cn

[R44] 按修改时间查找
来源：http://rxo.ctjpmb.com

find . -mtime -7 -type f
来源：http://nos.nwbrower.top

[R45] 批量删除
来源：http://ini.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://tzk.daria6918.cn

[R46] 递归替换文件内容
来源：http://fym.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eqe.zhiwuduotai.top

[R47] sed 单行替换
来源：http://ccq.meibo888.top

sed -i 's/foo/bar/g' a.txt
来源：http://jsg.gotoacloud.top

[R48] awk 取指定列
来源：http://ygf.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://cwn.havefunace.top

[R49] awk 带条件
来源：http://qmd.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mcd.yuanzhike.top

[R50] awk 求和
来源：http://dyi.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://trn.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://toh.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cqs.guowangkeji.top

[R52] 统计行数
来源：http://uur.hnqzz.top

wc -l a.txt
来源：http://aof.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://hwr.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qyi.nwbrower.top

[R54] 比较两个文件
来源：http://sfd.feifeiyinyue.top

diff a.txt b.txt
来源：http://iip.hammf.cn

[R55] 压缩与解压
来源：http://uuw.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kbb.gzhubu.top

[R56] 远程拷贝
来源：http://xri.yj202588.top

scp file user@host:/path/
来源：http://vtd.jinqigfzy.top

[R57] 远程执行命令
来源：http://rlv.c1oappe.top

ssh user@host 'uptime'
来源：http://rel.hesvh.cn

[R58] 下载文件
来源：http://zvg.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lil.ydzc1.top

[R59] 发 POST JSON
来源：http://ooq.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xjt.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://vxu.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://udw.yongpay.top

[R61] 磁盘占用
来源：http://fie.fzhhl.top

df -h;  du -sh *
来源：http://loz.ivvv.top

[R62] 找最占空间的文件
来源：http://phq.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://fth.zdbjq.cn

[R63] 内存与进程
来源：http://vos.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://wif.meibo888.top

[R64] 结束进程
来源：http://dbb.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://qrr.hnqzz.top

[R65] 查看端口占用
来源：http://dvn.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gjl.mhx1999.top

[R66] 定时任务
来源：http://jxe.hcnkem.com

crontab -e;  crontab -l
来源：http://ozp.yj20258888.top

[R67] 生成随机十六进制串
来源：http://hbg.dianchejie.cn

openssl rand -hex 16
来源：http://ney.snrcjt.cn

[R68] 计算文件校验值
来源：http://rho.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://eek.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://hus.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://ujr.yj20258.top

[R70] 时间戳与互转
来源：http://knn.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://pcb.yuxming.cn

[R71] 日期格式化
来源：http://xkn.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://veg.chenlongwang.top

[R72] 等待端口就绪
来源：http://jfu.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xrf.tianlin.xyz

[R73] 分割大日志
来源：http://fjm.meibo888.top

split -l 1000 big.log part_
来源：http://ezj.fengsongda.top

[R74] 批量重命名
来源：http://ews.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fzm.xziqi.cn

[R75] 导出环境变量
来源：http://aqt.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://xhj.yj20258888.top

[R76] 使用临时文件
来源：http://ibp.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://swu.guowangkeji.top

[R77] 读取用户输入
来源：http://fni.yj20258888.top

read -rp "请输入: " ans
来源：http://hgm.jyoumei.cn

[R78] 交互式菜单
来源：http://bnh.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://iwk.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://mku.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ivl.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ozf.hysaishi.cn

time ./run.sh
来源：http://lia.ydzc1.top

================================================================================
来源：http://wjm.epnwcf.com

S. C / C++ 专题
来源：http://ggf.hnqzz.top

================================================================================
来源：http://pkz.yj20258888.top

[S01] C：Hello World
来源：http://ohc.dianchejie.cn

#include <stdio.h>
来源：http://ffz.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://khs.zycfv.cn

[S02] C：变量与格式化输出
来源：http://exm.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://vup.yfazqb.com

[S03] C：读入整数
来源：http://rtw.pycfn.com

int x; scanf("%d", &x);
来源：http://lum.zdbjq.cn

[S04] C：字符串复制
来源：http://pkt.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://wbw.fzhhl.top

[S05] C：字符串长度
来源：http://klp.cucudq.cn

strlen(s)
来源：http://eny.nanxuanxn.top

[S06] C：字符串比较
来源：http://avu.redwolf501.top

strcmp(a, b) == 0
来源：http://qlw.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://dyt.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dfy.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://ifa.yongpay.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iap.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://pax.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mmx.nanxuanxn.top

[S10] C：指针与解引用
来源：http://foz.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://fgm.quarkkingdee.top

[S11] C：逐行读文件
来源：http://ucv.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://eoo.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://cgs.yueranfly.top

fclose(f);
来源：http://quf.daxiang520.top

[S12] C：写文件
来源：http://awr.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dtw.xylfe.cn

[S13] C：宏定义
来源：http://pea.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zhq.aizwys.cn

[S14] C：枚举
来源：http://tff.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://tlb.fktsv.cn

[S15] C：类型转换
来源：http://pqe.gogol.net.cn

(double) a / b
来源：http://jnq.daxiang520.top

[S16] C：位操作置位
来源：http://xux.yfazqb.com

x |= (1 << 3);
来源：http://alc.uphjek.com

[S17] C：安全拼接字符串
来源：http://rlh.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tyk.hcnkem.com

[S18] C：命令行参数
来源：http://baa.zhixingplan.top

int main(int argc, char **argv)
来源：http://egc.sysykeji.top

[S19] C：快速排序
来源：http://jpa.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://zwr.gogol.net.cn

[S20] C：二分查找
来源：http://mqs.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://reh.guowangkeji.top

[S21] C：字符类别判断
来源：http://loo.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gic.jiagoushi.top

[S22] C：字符串转数字
来源：http://hqn.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://rgc.jinqigfzy.top

[S23] C：随机数
来源：http://qcd.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xzo.dianchejie.cn

[S24] C：获取本地时间
来源：http://exw.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://paq.yvedp.cn

[S25] C：内存拷贝
来源：http://amd.epnwcf.com

memcpy(dst, src, n);
来源：http://ucr.guowangkeji.top

[S26] C：内存清零
来源：http://yya.sweek.top

memset(a, 0, sizeof a);
来源：http://jem.ybcxt.top

[S27] C：定义常量
来源：http://qbr.xuanzx.com

const double PI = 3.14159;
来源：http://wtv.pycfn.com

[S28] C：静态变量
来源：http://ykg.cashguo.top

static int counter = 0;
来源：http://grc.yueranfly.top

[S29] C：变参函数
来源：http://haw.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tod.yanxiufei.cn

[S30] C：头文件保护
来源：http://epr.jqgfzy.top

#ifndef X_H
来源：http://mfj.hnxiangtu.top

#define X_H
来源：http://kve.andypj.xyz

#endif
来源：http://uhz.fengsongda.top

[S31] C++：Hello World
来源：http://taa.jinqigfzy.top

#include <iostream>
来源：http://ian.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://zfm.meibo888.top

[S32] C++：字符串
来源：http://kka.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://csd.hnqzz.top

[S33] C++：vector 增删
来源：http://mca.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://shd.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://uun.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://bxd.shuidangran.top

[S35] C++：map
来源：http://zpy.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dyx.guowangkeji.top

[S36] C++：unordered_map
来源：http://ydt.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://azw.ehwqpu.com

[S37] C++：set
来源：http://fat.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xmz.jinghuilouyu.cn

[S38] C++：排序
来源：http://qqe.tanke756.top

std::sort(v.begin(), v.end());
来源：http://jkk.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://cyu.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rsw.ydzc1.top

[S40] C++：查找元素
来源：http://ypn.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ess.chenzaomai.com

[S41] C++：类与构造函数
来源：http://yzz.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cym.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://qwo.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://ajy.quarkkingdee.top

[S43] C++：智能指针
来源：http://wqd.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://kfb.shangyingyoupin.top

[S44] C++：引用传参
来源：http://erz.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://tjq.zdqjudy.top

[S45] C++：lambda
来源：http://spw.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://jhl.hcnkem.com

[S46] C++：函数模板
来源：http://pvm.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gmh.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://wjx.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wjl.dashuyun.cn

[S48] C++：逐行读文件
来源：http://hoa.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qha.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://fao.aizwys.cn

[S49] C++：写文件
来源：http://nkp.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xzm.aibaodan.cn

[S50] C++：格式化数字
来源：http://zum.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://okc.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://gfa.0kj1m.cn

static_cast<double>(a) / b
来源：http://ggw.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://qhb.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://njv.jlsjyb.cn

[S53] C++：移动语义
来源：http://xmy.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://ycs.pycfn.com

[S54] C++：异常处理
来源：http://zmb.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sws.chenlongwang.top

[S55] C++：结构化绑定
来源：http://ehd.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://znh.mhx1999.top

[S56] C++：optional
来源：http://dbf.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xnt.wangdashe.top

[S57] C++：编译期常量
来源：http://jmb.cqqwz.cn

constexpr int N = 10;
来源：http://dox.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://hhm.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://hbw.ybcxt.top

[S59] C++：静态断言
来源：http://kwn.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fem.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://zts.vqdsnc.cn


<!-- 参考信息 -->