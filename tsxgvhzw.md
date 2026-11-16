代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qyx.hongshengwenyu.top

[Q90] 生成序号列
来源：http://hmi.havefunace.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vnn.cucudq.cn

================================================================================
来源：http://bbz.chenjidiqi.icu

R. Bash 专题
来源：http://ctc.sweek.top

================================================================================
来源：http://eiy.gzhubu.top

[R01] shebang 与严格模式
来源：http://zzs.daxiang520.top

#!/usr/bin/env bash
来源：http://zwa.shangyingyoupin.top

set -euo pipefail
来源：http://dpf.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://ejv.nanxinkj.top

name="Tom"; echo "$name"
来源：http://gqc.xylfe.cn

[R03] 只读变量
来源：http://ujs.cashguo.top

readonly PI=3.14
来源：http://pas.smart0.xyz

[R04] 位置参数
来源：http://lzf.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qxl.yfazqb.com

[R05] 参数默认值
来源：http://owm.gogol.net.cn

name="${1:-default}"
来源：http://wxe.birdmap.top

[R06] 判断命令是否存在
来源：http://tki.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tcd.meibo888.top

[R07] if 判断文件
来源：http://saj.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ibu.zdqjudy.top

[R08] 数值比较
来源：http://ojr.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://epu.zhijiandao.cn

[R09] 字符串比较
来源：http://zgs.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://esk.tanke756.top

[R10] 正则匹配
来源：http://dzt.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dfz.jlsjyb.cn

[R11] case 多分支
来源：http://sqp.bjfxy.top

case "$1" in
来源：http://yiu.daria6918.cn

start) echo "启动" ;;
来源：http://yav.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://qxp.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://phd.zhaomingkeji.xyz

esac
来源：http://uuf.mhx1999.top

[R12] for 遍历文件
来源：http://ktr.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://fxh.52xcode.cn

[R13] for 计数循环
来源：http://yku.c1oappe.top

for i in {1..10}; do echo "$i"; done
来源：http://jpy.cucudq.cn

[R14] C 风格 for
来源：http://rnm.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sde.yj20258888.top

[R15] while 逐行读文件
来源：http://djq.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tnb.hywenlv.cn

[R16] until 等待条件
来源：http://seq.wangdashe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mhd.yuanzhike.top

[R17] 数组定义与取值
来源：http://rlz.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://rsv.guannengcc.top

[R18] 遍历数组
来源：http://qpk.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ltr.zdbjq.cn

[R19] 数组长度
来源：http://auk.chenlongwang.top

echo "${#arr[@]}"
来源：http://xin.daria6918.cn

[R20] 关联数组（字典）
来源：http://skm.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tmu.gotoacloud.top

[R21] 字符串长度
来源：http://uis.tian-w.cn

echo "${#s}"
来源：http://foa.andypj.xyz

[R22] 截取子串
来源：http://wsr.yueranfly.top

echo "${s:0:5}"
来源：http://ocz.zhengqikj.top

[R23] 字符串替换
来源：http://glf.uphjek.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://thh.guowangkeji.top

[R24] 大小写转换
来源：http://jcb.vqdsnc.cn

echo "${s^^}"; echo "${s,,}"
来源：http://btm.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://typ.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://eqk.kuanghao11.cn

[R26] 命令替换
来源：http://lvq.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://qxm.shangyingyoupin.top

[R27] 算术展开
来源：http://lpr.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://czz.nwbrower.top

[R28] 浮点运算
来源：http://svy.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://cyx.vqdsnc.cn

[R29] 定义函数
来源：http://xsi.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://efu.316326.xyz

[R30] 函数返回状态码
来源：http://qky.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://axd.mhx1999.top

[R31] 局部变量
来源：http://tbg.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://mln.quarkkingdee.top

[R32] 参数个数校验
来源：http://wto.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aif.316326.xyz

[R33] 捕获错误并提示行号
来源：http://htf.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ykp.zhiwuduotai.top

[R34] 退出时清理
来源：http://svd.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://tqj.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://pbd.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ogj.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://mij.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mdu.yangfankeji.com

[R37] 把输出赋给变量
来源：http://suw.daria6918.cn

files=$(ls -1)
来源：http://xgj.yangfankeji.com

[R38] 管道串联
来源：http://lov.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://rpq.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://hbl.tanke756.top

cmd > out.log 2>&1
来源：http://zvr.cashguo.top

[R40] 追加写日志
来源：http://luk.jianghu66.top

echo "log" >> out.log
来源：http://pyp.havefunace.top

[R41] 丢弃输出
来源：http://cjf.birdmap.top

cmd >/dev/null 2>&1
来源：http://uga.tian-w.cn

[R42] 输入重定向
来源：http://qqi.gogol.net.cn

wc -l < a.txt
来源：http://zoq.xylfe.cn

[R43] 按名字查找文件
来源：http://rwu.nanxuanxn.top

find . -name "*.log" -type f
来源：http://ges.yuxming.cn

[R44] 按修改时间查找
来源：http://guc.gaohongyu789.top

find . -mtime -7 -type f
来源：http://yym.zhoulong.xyz

[R45] 批量删除
来源：http://qya.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://ruy.xylfe.cn

[R46] 递归替换文件内容
来源：http://iti.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pqu.ppjwa.cn

[R47] sed 单行替换
来源：http://csx.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lyk.jlsjyb.cn

[R48] awk 取指定列
来源：http://gto.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://uor.svipenyu.cn

[R49] awk 带条件
来源：http://lvz.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jrm.jinyuanbaomall.cn

[R50] awk 求和
来源：http://vdd.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://xmc.hammf.cn

[R51] 排序去重取前几
来源：http://hwk.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qoc.iojbl.cn

[R52] 统计行数
来源：http://gkw.gzhubu.top

wc -l a.txt
来源：http://ysu.ivvv.top

[R53] 查看文件头与实时尾
来源：http://ovw.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://otj.jiagoushi.top

[R54] 比较两个文件
来源：http://zdz.ivvv.top

diff a.txt b.txt
来源：http://ixz.chenlongwang.top

[R55] 压缩与解压
来源：http://ygh.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://srm.jiagoushi.top

[R56] 远程拷贝
来源：http://vak.52xcode.cn

scp file user@host:/path/
来源：http://sze.chenlongwang.top

[R57] 远程执行命令
来源：http://cwu.zhijiandao.cn

ssh user@host 'uptime'
来源：http://adx.dianchejie.cn

[R58] 下载文件
来源：http://sjj.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://naa.shuidangran.top

[R59] 发 POST JSON
来源：http://jya.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kvs.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://tig.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wmc.fehbvm.com

[R61] 磁盘占用
来源：http://mji.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://ljc.xylfe.cn

[R62] 找最占空间的文件
来源：http://rdr.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://fjz.quarkkingdee.top

[R63] 内存与进程
来源：http://mxm.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://vtr.ybcxt.top

[R64] 结束进程
来源：http://qyi.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://ldv.wangshuangyany.cn

[R65] 查看端口占用
来源：http://yop.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nex.yj202588.top

[R66] 定时任务
来源：http://yme.ppjwa.cn

crontab -e;  crontab -l
来源：http://naq.sweek.top

[R67] 生成随机十六进制串
来源：http://hiw.hnqzz.top

openssl rand -hex 16
来源：http://uik.zdqjudy.top

[R68] 计算文件校验值
来源：http://itk.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://woe.zhiwuduotai.top

[R69] 生成随机密码
来源：http://jkz.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://qdy.ppjwa.cn

[R70] 时间戳与互转
来源：http://xpj.wangdashe.top

date +%s;  date -d @1700000000
来源：http://ihx.pengpengdd.cyou

[R71] 日期格式化
来源：http://bxj.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qgj.hnqzz.top

[R72] 等待端口就绪
来源：http://off.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fat.iojbl.cn

[R73] 分割大日志
来源：http://mot.yj202588.top

split -l 1000 big.log part_
来源：http://sam.cqqwz.cn

[R74] 批量重命名
来源：http://sop.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ays.hfpthk.cn

[R75] 导出环境变量
来源：http://gyq.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://mpi.yj20258888.top

[R76] 使用临时文件
来源：http://tgd.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cdw.ydzc1.top

[R77] 读取用户输入
来源：http://vvl.sjlbkw.cn

read -rp "请输入: " ans
来源：http://kae.c1oappe.top

[R78] 交互式菜单
来源：http://wxl.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wkj.cqqwz.cn

[R79] 解析命令行选项
来源：http://msp.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ocs.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://kpc.fehbvm.com

time ./run.sh
来源：http://lrc.yueranfly.top

================================================================================
来源：http://bqc.jiagoushi.top

S. C / C++ 专题
来源：http://ytj.birdmap.top

================================================================================
来源：http://lxi.hongshengwenyu.top

[S01] C：Hello World
来源：http://ecg.mhx1999.top

#include <stdio.h>
来源：http://lxr.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://luo.uphjek.com

[S02] C：变量与格式化输出
来源：http://ipd.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://zby.aizwys.cn

[S03] C：读入整数
来源：http://cwf.guowangkeji.top

int x; scanf("%d", &x);
来源：http://vlk.ydjk.org.cn

[S04] C：字符串复制
来源：http://njc.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://har.daria6918.cn

[S05] C：字符串长度
来源：http://may.yuanzhike.top

strlen(s)
来源：http://yul.tianlin.xyz

[S06] C：字符串比较
来源：http://ryu.cucudq.cn

strcmp(a, b) == 0
来源：http://tyx.zhengqikj.top

[S07] C：数组遍历求和
来源：http://qua.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tzo.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://kzb.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hoc.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://xma.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fqe.dashuyun.cn

[S10] C：指针与解引用
来源：http://syy.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://mvr.yongpay.top

[S11] C：逐行读文件
来源：http://dzk.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://cjd.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pux.fengsongda.top

fclose(f);
来源：http://jyh.zhaomingkeji.xyz

[S12] C：写文件
来源：http://lff.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kno.fanxiaobao.xyz

[S13] C：宏定义
来源：http://xzq.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lru.wangdashe.top

[S14] C：枚举
来源：http://nby.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://hkp.aizwys.cn

[S15] C：类型转换
来源：http://cet.xylfe.cn

(double) a / b
来源：http://szc.ydzc1.top

[S16] C：位操作置位
来源：http://zvi.c1oappe.top

x |= (1 << 3);
来源：http://xha.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://eql.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kms.tian-w.cn

[S18] C：命令行参数
来源：http://ywn.jianghu66.top

int main(int argc, char **argv)
来源：http://exz.xuetiantiany.cn

[S19] C：快速排序
来源：http://oyb.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://xyt.snrcjt.cn

[S20] C：二分查找
来源：http://miv.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dgg.dianchejie.cn

[S21] C：字符类别判断
来源：http://ibe.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ove.xinyue.icu

[S22] C：字符串转数字
来源：http://ldy.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wot.hesvh.cn

[S23] C：随机数
来源：http://hfe.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cme.mhx1999.top

[S24] C：获取本地时间
来源：http://dtr.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yyp.sufxvd.cn

[S25] C：内存拷贝
来源：http://tre.kuanghao11.cn

memcpy(dst, src, n);
来源：http://yjk.mhx1999.top

[S26] C：内存清零
来源：http://alf.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://phd.guannengcc.top

[S27] C：定义常量
来源：http://cev.mhx1999.top

const double PI = 3.14159;
来源：http://ymm.c1oappe.top

[S28] C：静态变量
来源：http://era.gzhubu.top

static int counter = 0;
来源：http://zyq.tarul.cn

[S29] C：变参函数
来源：http://hbu.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iwh.ybcxt.top

[S30] C：头文件保护
来源：http://aye.svipenyu.cn

#ifndef X_H
来源：http://ssu.snrcjt.cn

#define X_H
来源：http://lqp.vehdjk.com

#endif
来源：http://lnj.yj20258.top

[S31] C++：Hello World
来源：http://gdb.chenzaomai.com

#include <iostream>
来源：http://hkh.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://wkt.fengsongda.top

[S32] C++：字符串
来源：http://wqc.ivvv.top

std::string s = "hi";  s += "!";
来源：http://vvt.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://qcv.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://suo.0kj1m.cn

[S34] C++：遍历 vector
来源：http://kuq.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://ach.mhx1999.top

[S35] C++：map
来源：http://hgg.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sfn.bjfxy.top

[S36] C++：unordered_map
来源：http://lta.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cdk.zhengqikj.top

[S37] C++：set
来源：http://cqj.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tbb.316326.xyz

[S38] C++：排序
来源：http://vfv.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://poa.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://gng.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sgg.iojbl.cn

[S40] C++：查找元素
来源：http://adu.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rah.bjfxy.top

[S41] C++：类与构造函数
来源：http://qcc.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zbt.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://iis.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://igh.quarkkingdee.top

[S43] C++：智能指针
来源：http://qzz.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://sdy.ivvv.top

[S44] C++：引用传参
来源：http://tbw.bbcook.cn

void inc(int &x) { ++x; }
来源：http://ugf.ivvv.top

[S45] C++：lambda
来源：http://ire.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://wli.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://cqs.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blo.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://ryq.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xod.xinyue.icu

[S48] C++：逐行读文件
来源：http://fba.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qcq.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://ynb.ctjpmb.com

[S49] C++：写文件
来源：http://arr.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sqv.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://piy.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kdn.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://tgf.fehbvm.com

static_cast<double>(a) / b
来源：http://uad.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://kfx.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://uke.tarul.cn

[S53] C++：移动语义
来源：http://fhn.tarul.cn

std::vector<int> w = std::move(v);
来源：http://jov.daria6918.cn

[S54] C++：异常处理
来源：http://sme.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mtw.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://nxl.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pgp.feifeiyinyue.top

[S56] C++：optional
来源：http://zxc.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jpe.andypj.xyz

[S57] C++：编译期常量
来源：http://zht.epnwcf.com

constexpr int N = 10;
来源：http://pow.zycfv.cn

[S58] C++：命名空间
来源：http://tsb.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://oas.yfazqb.com

[S59] C++：静态断言
来源：http://udh.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://phu.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://hxf.yanxiufei.cn


<!-- 参考信息 -->