代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://slt.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tsj.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cpu.bjfxy.top

[Q89] 判断表是否存在
来源：http://fit.hammf.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lsh.yueranfly.top

[Q90] 生成序号列
来源：http://cec.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kva.shuidangran.top

================================================================================
来源：http://hns.nanxinkj.top

R. Bash 专题
来源：http://vse.xuetiantiany.cn

================================================================================
来源：http://son.guowangkeji.top

[R01] shebang 与严格模式
来源：http://vdt.daria6918.cn

#!/usr/bin/env bash
来源：http://gvi.gzhubu.top

set -euo pipefail
来源：http://fhz.yj202588.top

[R02] 变量赋值与使用
来源：http://rcy.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://ylo.zhengqikj.top

[R03] 只读变量
来源：http://muf.daxiang520.top

readonly PI=3.14
来源：http://ycl.guowangkeji.top

[R04] 位置参数
来源：http://khf.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dxb.meibo888.top

[R05] 参数默认值
来源：http://fxm.xinyue.icu

name="${1:-default}"
来源：http://dep.zycfv.cn

[R06] 判断命令是否存在
来源：http://itu.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jxu.redwolf501.top

[R07] if 判断文件
来源：http://uqm.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vgm.sxryk.cn

[R08] 数值比较
来源：http://glv.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ifn.ydjk.org.cn

[R09] 字符串比较
来源：http://utc.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nse.zhijiandao.cn

[R10] 正则匹配
来源：http://hso.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jur.zhaomingkeji.xyz

[R11] case 多分支
来源：http://cyj.gogol.net.cn

case "$1" in
来源：http://yma.xinyue.icu

start) echo "启动" ;;
来源：http://uco.gogol.net.cn

stop)  echo "停止" ;;
来源：http://bcb.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://xiu.xziqi.cn

esac
来源：http://yyq.iojbl.cn

[R12] for 遍历文件
来源：http://tko.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://zuv.xuanzx.com

[R13] for 计数循环
来源：http://def.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://tby.daria6918.cn

[R14] C 风格 for
来源：http://emu.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://njy.vqdsnc.cn

[R15] while 逐行读文件
来源：http://uiw.xziqi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qfl.xuanzx.com

[R16] until 等待条件
来源：http://goi.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gii.mhx1999.top

[R17] 数组定义与取值
来源：http://ozf.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://qqi.aizwys.cn

[R18] 遍历数组
来源：http://ujo.feifeiyinyue.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rif.hysaishi.cn

[R19] 数组长度
来源：http://uqv.jqgfzy.top

echo "${#arr[@]}"
来源：http://kou.yvedp.cn

[R20] 关联数组（字典）
来源：http://wgx.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rre.pengpengdd.cyou

[R21] 字符串长度
来源：http://doa.yongpay.top

echo "${#s}"
来源：http://rhx.meibo888.top

[R22] 截取子串
来源：http://yrj.0kj1m.cn

echo "${s:0:5}"
来源：http://dpm.yj20258888.top

[R23] 字符串替换
来源：http://emi.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kqv.jqgfzy.top

[R24] 大小写转换
来源：http://hyi.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://bdi.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://sdy.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fhx.0kj1m.cn

[R26] 命令替换
来源：http://hjj.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://mzh.xinyue.icu

[R27] 算术展开
来源：http://bdd.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://mzb.chenlongwang.top

[R28] 浮点运算
来源：http://yvb.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://nle.ivvv.top

[R29] 定义函数
来源：http://mys.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rhs.zhixingplan.top

[R30] 函数返回状态码
来源：http://adv.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://wcv.yanxiufei.cn

[R31] 局部变量
来源：http://erx.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://lcm.redwolf501.top

[R32] 参数个数校验
来源：http://ijl.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uzq.uphjek.com

[R33] 捕获错误并提示行号
来源：http://jyp.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kks.nanxuanxn.top

[R34] 退出时清理
来源：http://kfc.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://jmx.vqdsnc.cn

[R35] 后台执行并等待
来源：http://ybi.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bio.chenzaomai.com

[R36] 并发执行多个任务
来源：http://ege.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bze.yonumen.top

[R37] 把输出赋给变量
来源：http://ezj.mhx1999.top

files=$(ls -1)
来源：http://ylp.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://gke.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://tnc.cheryme.top

[R39] 重定向标准输出与错误
来源：http://hye.nanxuanxn.top

cmd > out.log 2>&1
来源：http://aom.xuetiantiany.cn

[R40] 追加写日志
来源：http://bbo.daxiang520.top

echo "log" >> out.log
来源：http://hvg.birdmap.top

[R41] 丢弃输出
来源：http://snv.sysykeji.top

cmd >/dev/null 2>&1
来源：http://kuc.dianchejie.cn

[R42] 输入重定向
来源：http://osg.tianlin.xyz

wc -l < a.txt
来源：http://fgg.zycfv.cn

[R43] 按名字查找文件
来源：http://hdk.tianlin.xyz

find . -name "*.log" -type f
来源：http://pzi.bbcook.cn

[R44] 按修改时间查找
来源：http://ght.vehdjk.com

find . -mtime -7 -type f
来源：http://sqc.gzhubu.top

[R45] 批量删除
来源：http://vrx.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://vor.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://dtp.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oek.yuxming.cn

[R47] sed 单行替换
来源：http://qnf.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://prn.gogol.net.cn

[R48] awk 取指定列
来源：http://bve.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://mzo.iojbl.cn

[R49] awk 带条件
来源：http://qur.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yjn.yvedp.cn

[R50] awk 求和
来源：http://msi.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://pxo.xuanzx.com

[R51] 排序去重取前几
来源：http://mer.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kml.yfazqb.com

[R52] 统计行数
来源：http://wqv.yvedp.cn

wc -l a.txt
来源：http://gbc.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://qwe.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hnl.jqgufenzy.top

[R54] 比较两个文件
来源：http://zsk.fengsongda.top

diff a.txt b.txt
来源：http://zym.sxryk.cn

[R55] 压缩与解压
来源：http://vwr.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://txl.smart0.xyz

[R56] 远程拷贝
来源：http://amz.shangyingyoupin.top

scp file user@host:/path/
来源：http://ecr.redwolf501.top

[R57] 远程执行命令
来源：http://fhm.vqdsnc.cn

ssh user@host 'uptime'
来源：http://jxl.xuetiantiany.cn

[R58] 下载文件
来源：http://lku.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qxd.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://fvd.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xap.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://hoj.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xqu.yangfankeji.com

[R61] 磁盘占用
来源：http://ojz.redwolf501.top

df -h;  du -sh *
来源：http://fov.ydzc1.top

[R62] 找最占空间的文件
来源：http://ffj.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://ega.jlsjyb.cn

[R63] 内存与进程
来源：http://tzi.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://vau.aibaodan.cn

[R64] 结束进程
来源：http://ubp.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://hdm.meibo888.top

[R65] 查看端口占用
来源：http://uhz.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fil.9152youxi.cn

[R66] 定时任务
来源：http://aod.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://svc.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://nos.meibo888.top

openssl rand -hex 16
来源：http://ker.meibo888.top

[R68] 计算文件校验值
来源：http://bam.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iqk.bbcook.cn

[R69] 生成随机密码
来源：http://wyx.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://ajm.dianchejie.cn

[R70] 时间戳与互转
来源：http://dgu.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://xld.kuanghao11.cn

[R71] 日期格式化
来源：http://cpu.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lgq.9152youxi.cn

[R72] 等待端口就绪
来源：http://blq.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jgf.birdmap.top

[R73] 分割大日志
来源：http://ofw.daxiang520.top

split -l 1000 big.log part_
来源：http://avf.jiagoushi.top

[R74] 批量重命名
来源：http://kan.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bko.ehwqpu.com

[R75] 导出环境变量
来源：http://pcm.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://lud.chenjidiqi.icu

[R76] 使用临时文件
来源：http://omj.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nuj.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://xsv.aibaodan.cn

read -rp "请输入: " ans
来源：http://iar.jlsjyb.cn

[R78] 交互式菜单
来源：http://ury.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eyf.hnxiangtu.top

[R79] 解析命令行选项
来源：http://vzu.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ntd.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://ijq.zhoulong.xyz

time ./run.sh
来源：http://bsj.yfazqb.com

================================================================================
来源：http://ten.zhixingplan.top

S. C / C++ 专题
来源：http://lbs.jinqigufen.top

================================================================================
来源：http://hbf.snrcjt.cn

[S01] C：Hello World
来源：http://ido.xinyue.icu

#include <stdio.h>
来源：http://ium.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lbs.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://ajl.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://sdb.feifeiyinyue.top

[S03] C：读入整数
来源：http://tpw.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://vmz.316326.xyz

[S04] C：字符串复制
来源：http://ski.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://zkm.hysaishi.cn

[S05] C：字符串长度
来源：http://afe.316326.xyz

strlen(s)
来源：http://dzq.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://htq.yongpay.top

strcmp(a, b) == 0
来源：http://uah.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://amo.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://utl.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://mxj.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qrp.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://cqn.tian-w.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ztq.nanxinkj.top

[S10] C：指针与解引用
来源：http://fjo.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://orq.xylfe.cn

[S11] C：逐行读文件
来源：http://pbs.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://cot.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gdo.fzhhl.top

fclose(f);
来源：http://wrc.jqgfzy.top

[S12] C：写文件
来源：http://bae.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzi.sxryk.cn

[S13] C：宏定义
来源：http://fgl.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zys.sufxvd.cn

[S14] C：枚举
来源：http://mft.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://fnx.jlsjyb.cn

[S15] C：类型转换
来源：http://ldm.jiagoushi.top

(double) a / b
来源：http://jms.fehbvm.com

[S16] C：位操作置位
来源：http://fil.aibaodan.cn

x |= (1 << 3);
来源：http://vci.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://feg.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nuw.fehbvm.com

[S18] C：命令行参数
来源：http://eyt.gaohongyu789.top

int main(int argc, char **argv)
来源：http://kyo.mhx1999.top

[S19] C：快速排序
来源：http://jns.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://ilp.bjfxy.top

[S20] C：二分查找
来源：http://atl.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cix.tarul.cn

[S21] C：字符类别判断
来源：http://izs.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://top.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://urv.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://wmn.yj202588.top

[S23] C：随机数
来源：http://mch.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://chn.hesvh.cn

[S24] C：获取本地时间
来源：http://pux.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nzt.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://pdi.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://pjo.aibaodan.cn

[S26] C：内存清零
来源：http://zwf.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://ryw.yj202588.top

[S27] C：定义常量
来源：http://jgb.yj202588.top

const double PI = 3.14159;
来源：http://aqb.gaohongyu789.top

[S28] C：静态变量
来源：http://wbc.jinyuanbaomall.cn

static int counter = 0;
来源：http://gbg.redwolf501.top

[S29] C：变参函数
来源：http://urp.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzh.hnqzz.top

[S30] C：头文件保护
来源：http://vpx.chenzaomai.com

#ifndef X_H
来源：http://rqr.9152youxi.cn

#define X_H
来源：http://spl.ydjk.org.cn

#endif
来源：http://rzx.sjlbkw.cn

[S31] C++：Hello World
来源：http://pmj.hcnkem.com

#include <iostream>
来源：http://xny.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://bfe.fehbvm.com

[S32] C++：字符串
来源：http://hzs.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://yzs.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://wpg.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfk.daria6918.cn

[S34] C++：遍历 vector
来源：http://bba.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://nxr.sysykeji.top

[S35] C++：map
来源：http://vlu.shangyingyoupin.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://daz.yueranfly.top

[S36] C++：unordered_map
来源：http://wgb.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uxw.jlsjyb.cn

[S37] C++：set
来源：http://moh.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kda.yvedp.cn

[S38] C++：排序
来源：http://xov.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://mgd.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://aod.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fcv.sysykeji.top

[S40] C++：查找元素
来源：http://fpt.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://otr.fehbvm.com

[S41] C++：类与构造函数
来源：http://ski.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://upt.nwbrower.top

[S42] C++：继承与虚函数
来源：http://gqc.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://xqi.daxiang520.top

[S43] C++：智能指针
来源：http://jqf.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://nnb.xuanzx.com

[S44] C++：引用传参
来源：http://zrg.yueranfly.top

void inc(int &x) { ++x; }
来源：http://cwt.gogol.net.cn

[S45] C++：lambda
来源：http://rum.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://bhd.hnxiangtu.top

[S46] C++：函数模板
来源：http://jmz.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vxq.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://jvk.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcy.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://lsb.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://bal.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://zwd.nanxinkj.top

[S49] C++：写文件
来源：http://ovh.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hlu.epnwcf.com

[S50] C++：格式化数字
来源：http://mbb.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lev.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://tzn.redwolf501.top

static_cast<double>(a) / b
来源：http://gqo.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://mzk.xinyue.icu

int size() const noexcept { return n_; }
来源：http://xll.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://cjq.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://fyb.quarkkingdee.top

[S54] C++：异常处理
来源：http://caj.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qfz.jiagoushi.top

[S55] C++：结构化绑定
来源：http://eod.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://inq.zhixingplan.top

[S56] C++：optional
来源：http://qwb.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dir.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://erg.shuidangran.top

constexpr int N = 10;
来源：http://lki.fengsongda.top

[S58] C++：命名空间
来源：http://sqe.hcnkem.com


<!-- 参考信息 -->