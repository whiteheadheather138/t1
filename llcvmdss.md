代发 wailian999

[Q84] 去除首尾空格
来源：http://oub.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://mpu.ehwqpu.com

[Q85] 数值取整
来源：http://xlx.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fhe.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://flg.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oea.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://kzc.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sij.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://igy.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qon.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fhm.yj20258888.top

[Q89] 判断表是否存在
来源：http://ese.316326.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vyn.nwbrower.top

[Q90] 生成序号列
来源：http://gsw.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvn.cheryme.top

================================================================================
来源：http://yhg.52xcode.cn

R. Bash 专题
来源：http://tip.xingfuxueyuan.xyz

================================================================================
来源：http://ciq.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://yai.zhaomingkeji.xyz

#!/usr/bin/env bash
来源：http://htp.meibo888.top

set -euo pipefail
来源：http://oxw.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://lfx.ybcxt.top

name="Tom"; echo "$name"
来源：http://wep.cashguo.top

[R03] 只读变量
来源：http://hqt.hywenlv.cn

readonly PI=3.14
来源：http://svh.hfpthk.cn

[R04] 位置参数
来源：http://mjm.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ujt.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://msy.hnxiangtu.top

name="${1:-default}"
来源：http://tdf.jinqigufen.top

[R06] 判断命令是否存在
来源：http://qns.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jjn.daria6918.cn

[R07] if 判断文件
来源：http://irj.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hhw.chenjidiqi.icu

[R08] 数值比较
来源：http://fjr.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cpr.andypj.xyz

[R09] 字符串比较
来源：http://uyb.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fjo.zhoulong.xyz

[R10] 正则匹配
来源：http://qly.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hvs.gotoacloud.top

[R11] case 多分支
来源：http://atx.hfpthk.cn

case "$1" in
来源：http://ljn.bbcook.cn

start) echo "启动" ;;
来源：http://gms.ybcxt.top

stop)  echo "停止" ;;
来源：http://ehd.shuidangran.top

*)     echo "未知命令" ;;
来源：http://eyz.chenlongwang.top

esac
来源：http://opl.hnxiangtu.top

[R12] for 遍历文件
来源：http://ttb.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://uah.cashguo.top

[R13] for 计数循环
来源：http://neo.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://sbo.tarul.cn

[R14] C 风格 for
来源：http://nqx.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aiv.zdqjudy.top

[R15] while 逐行读文件
来源：http://qrp.cdnleiting.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://suj.daria6918.cn

[R16] until 等待条件
来源：http://alu.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nmq.yangfankeji.com

[R17] 数组定义与取值
来源：http://zqb.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://gnw.hfpthk.cn

[R18] 遍历数组
来源：http://yyy.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fnw.jinyuanbaomall.cn

[R19] 数组长度
来源：http://ozy.52xcode.cn

echo "${#arr[@]}"
来源：http://tdz.yongpay.top

[R20] 关联数组（字典）
来源：http://ptt.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://via.fanxiaobao.xyz

[R21] 字符串长度
来源：http://fqk.redwolf501.top

echo "${#s}"
来源：http://xcm.andypj.xyz

[R22] 截取子串
来源：http://pbs.meibo888.top

echo "${s:0:5}"
来源：http://byz.andypj.xyz

[R23] 字符串替换
来源：http://soo.gzhubu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ede.hywenlv.cn

[R24] 大小写转换
来源：http://mig.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://vrc.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://sxj.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pgv.ehwqpu.com

[R26] 命令替换
来源：http://aju.tanke756.top

now=$(date +%F); echo "$now"
来源：http://lej.uphjek.com

[R27] 算术展开
来源：http://kqs.quarkkingdee.top

echo $((1 + 2 * 3))
来源：http://mzh.jqgfzy.top

[R28] 浮点运算
来源：http://vbk.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://eqq.cheryme.top

[R29] 定义函数
来源：http://rwo.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qnh.zhixingplan.top

[R30] 函数返回状态码
来源：http://zwk.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://jll.wangshuangyany.cn

[R31] 局部变量
来源：http://cdv.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://xxd.jqgufenzy.top

[R32] 参数个数校验
来源：http://tmd.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oca.ybcxt.top

[R33] 捕获错误并提示行号
来源：http://qtx.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://etp.9152youxi.cn

[R34] 退出时清理
来源：http://wco.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://vsc.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://fkl.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dfk.smart0.xyz

[R36] 并发执行多个任务
来源：http://vaq.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lbu.havefunace.top

[R37] 把输出赋给变量
来源：http://yam.xziqi.cn

files=$(ls -1)
来源：http://oyz.cashguo.top

[R38] 管道串联
来源：http://pqw.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://ztw.birdmap.top

[R39] 重定向标准输出与错误
来源：http://uhl.yongpay.top

cmd > out.log 2>&1
来源：http://vpl.hongshengwenyu.top

[R40] 追加写日志
来源：http://etw.shzxlz.cn

echo "log" >> out.log
来源：http://its.jianghu66.top

[R41] 丢弃输出
来源：http://snv.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://uwz.kuanghao11.cn

[R42] 输入重定向
来源：http://gbd.hongshengwenyu.top

wc -l < a.txt
来源：http://fmn.ehwqpu.com

[R43] 按名字查找文件
来源：http://eis.tian-w.cn

find . -name "*.log" -type f
来源：http://rto.c1oappe.top

[R44] 按修改时间查找
来源：http://jlh.ctjpmb.com

find . -mtime -7 -type f
来源：http://ksm.9152youxi.cn

[R45] 批量删除
来源：http://umj.sxryk.cn

find . -name "*.tmp" -delete
来源：http://cgs.sweek.top

[R46] 递归替换文件内容
来源：http://xgy.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pkd.dianchejie.cn

[R47] sed 单行替换
来源：http://pqn.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xrj.yj202588.top

[R48] awk 取指定列
来源：http://hht.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://qlw.uphjek.com

[R49] awk 带条件
来源：http://mpf.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pih.aibaodan.cn

[R50] awk 求和
来源：http://inm.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://yiv.tanke756.top

[R51] 排序去重取前几
来源：http://rhm.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dgs.kuanghao11.cn

[R52] 统计行数
来源：http://aed.xingfuxueyuan.xyz

wc -l a.txt
来源：http://pio.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://jll.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jjo.jqgufenzy.top

[R54] 比较两个文件
来源：http://pbc.ivvv.top

diff a.txt b.txt
来源：http://rrl.feifeiyinyue.top

[R55] 压缩与解压
来源：http://ans.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jzm.yj20258.top

[R56] 远程拷贝
来源：http://gnx.redwolf501.top

scp file user@host:/path/
来源：http://ple.vqdsnc.cn

[R57] 远程执行命令
来源：http://bim.yueranfly.top

ssh user@host 'uptime'
来源：http://ioh.zhengqikj.top

[R58] 下载文件
来源：http://vyn.mhx1999.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dmo.svipenyu.cn

[R59] 发 POST JSON
来源：http://nyt.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lqb.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://wmx.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xaa.52xcode.cn

[R61] 磁盘占用
来源：http://vex.hnxiangtu.top

df -h;  du -sh *
来源：http://hxl.cheryme.top

[R62] 找最占空间的文件
来源：http://tqx.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://vom.redwolf501.top

[R63] 内存与进程
来源：http://qiv.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://vrn.cashguo.top

[R64] 结束进程
来源：http://yum.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://jms.wangshuangyany.cn

[R65] 查看端口占用
来源：http://bmh.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rfk.316326.xyz

[R66] 定时任务
来源：http://qnk.nwbrower.top

crontab -e;  crontab -l
来源：http://abo.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://eln.tarul.cn

openssl rand -hex 16
来源：http://fss.zhoulong.xyz

[R68] 计算文件校验值
来源：http://djf.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wzp.epnwcf.com

[R69] 生成随机密码
来源：http://biv.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://itb.zycfv.cn

[R70] 时间戳与互转
来源：http://sit.vehdjk.com

date +%s;  date -d @1700000000
来源：http://xta.yangfankeji.com

[R71] 日期格式化
来源：http://nmx.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kat.hnqzz.top

[R72] 等待端口就绪
来源：http://sbt.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://agz.daria6918.cn

[R73] 分割大日志
来源：http://adl.tian-w.cn

split -l 1000 big.log part_
来源：http://dpx.sxryk.cn

[R74] 批量重命名
来源：http://cvi.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hum.jinqigfzy.top

[R75] 导出环境变量
来源：http://byh.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://ajf.yanxiufei.cn

[R76] 使用临时文件
来源：http://khr.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ion.hesvh.cn

[R77] 读取用户输入
来源：http://how.dashuyun.cn

read -rp "请输入: " ans
来源：http://srq.zhongyouzk.top

[R78] 交互式菜单
来源：http://vqe.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jtc.bbcook.cn

[R79] 解析命令行选项
来源：http://fqt.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://apn.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://rkf.cheryme.top

time ./run.sh
来源：http://amx.hesvh.cn

================================================================================
来源：http://xgr.chenjidiqi.icu

S. C / C++ 专题
来源：http://dhb.xinyue.icu

================================================================================
来源：http://enj.daria6918.cn

[S01] C：Hello World
来源：http://ucn.ehwqpu.com

#include <stdio.h>
来源：http://cem.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://giz.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://fds.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://bek.ehwqpu.com

[S03] C：读入整数
来源：http://eci.daxiang520.top

int x; scanf("%d", &x);
来源：http://tsr.hysaishi.cn

[S04] C：字符串复制
来源：http://ijc.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://vgv.sufxvd.cn

[S05] C：字符串长度
来源：http://hbx.yvedp.cn

strlen(s)
来源：http://onj.hnxiangtu.top

[S06] C：字符串比较
来源：http://zbh.xziqi.cn

strcmp(a, b) == 0
来源：http://ryf.yueranfly.top

[S07] C：数组遍历求和
来源：http://ant.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://srz.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://omu.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vye.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://baf.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pyk.hesvh.cn

[S10] C：指针与解引用
来源：http://qcp.cashguo.top

int *p = &a;  *p = 5;
来源：http://iud.nanxuanxn.top

[S11] C：逐行读文件
来源：http://evv.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://sgs.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yqd.tanke756.top

fclose(f);
来源：http://rlj.zhiwuduotai.top

[S12] C：写文件
来源：http://tom.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixc.xuanzx.com

[S13] C：宏定义
来源：http://nio.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ifq.uphjek.com

[S14] C：枚举
来源：http://nxp.gaohongyu789.top

enum Color { RED, GREEN, BLUE };
来源：http://zkt.hcnkem.com

[S15] C：类型转换
来源：http://wlz.ydzc1.top

(double) a / b
来源：http://hie.nanxuanxn.top

[S16] C：位操作置位
来源：http://fiy.gaohongyu789.top

x |= (1 << 3);
来源：http://vup.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://pad.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zno.yueranfly.top

[S18] C：命令行参数
来源：http://lks.yangfankeji.com

int main(int argc, char **argv)
来源：http://usx.zdqjudy.top

[S19] C：快速排序
来源：http://tym.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://miz.ehwqpu.com

[S20] C：二分查找
来源：http://amx.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lhz.epnwcf.com

[S21] C：字符类别判断
来源：http://ncs.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uyw.fehbvm.com

[S22] C：字符串转数字
来源：http://zrp.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://sia.yonumen.top

[S23] C：随机数
来源：http://dei.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vzc.chenlongwang.top

[S24] C：获取本地时间
来源：http://ela.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jlj.aizwys.cn

[S25] C：内存拷贝
来源：http://xtz.zhoulong.xyz

memcpy(dst, src, n);
来源：http://qhn.fktsv.cn

[S26] C：内存清零
来源：http://ojt.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://sil.sxryk.cn

[S27] C：定义常量
来源：http://cwf.jiagoushi.top

const double PI = 3.14159;
来源：http://zhc.ppjwa.cn

[S28] C：静态变量
来源：http://hjq.havefunace.top

static int counter = 0;
来源：http://lfj.0kj1m.cn

[S29] C：变参函数
来源：http://swv.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pyn.wangshuangyany.cn

[S30] C：头文件保护
来源：http://ovn.epnwcf.com

#ifndef X_H
来源：http://fem.zhiwuduotai.top

#define X_H
来源：http://bhk.0kj1m.cn

#endif
来源：http://qfj.sxryk.cn

[S31] C++：Hello World
来源：http://pdq.daxiang520.top

#include <iostream>
来源：http://dzt.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://ryg.jinqigufen.top

[S32] C++：字符串
来源：http://xkk.tanke756.top

std::string s = "hi";  s += "!";
来源：http://zjq.ydzc1.top

[S33] C++：vector 增删
来源：http://lcb.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lpt.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://wuc.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://ecb.sweek.top

[S35] C++：map
来源：http://oov.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qzp.zycfv.cn

[S36] C++：unordered_map
来源：http://qpd.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ofs.dianchejie.cn

[S37] C++：set
来源：http://srd.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxs.nanxinkj.top

[S38] C++：排序
来源：http://gdm.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://sgo.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://nem.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jmf.tanke756.top

[S40] C++：查找元素
来源：http://bbi.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tue.hywenlv.cn

[S41] C++：类与构造函数
来源：http://vmw.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wtq.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://ttl.zhoulong.xyz

class B : public Base { public: void f() override {} };
来源：http://dsv.bjfxy.top

[S43] C++：智能指针
来源：http://bak.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://amx.kuanghao11.cn

[S44] C++：引用传参
来源：http://gjd.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://fgo.zdbjq.cn

[S45] C++：lambda
来源：http://xig.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://yqs.vqdsnc.cn

[S46] C++：函数模板
来源：http://hym.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iwp.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://vpf.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iyb.snrcjt.cn

[S48] C++：逐行读文件
来源：http://dyo.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yha.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://mlw.jinqigfzy.top

[S49] C++：写文件
来源：http://kye.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://llv.xinyue.icu

[S50] C++：格式化数字
来源：http://utp.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oqs.nwbrower.top

[S51] C++：显式类型转换
来源：http://bvn.svipenyu.cn

static_cast<double>(a) / b
来源：http://gqq.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://nzo.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://hsg.jianghu66.top

[S53] C++：移动语义
来源：http://hsm.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://mcu.ivvv.top

[S54] C++：异常处理
来源：http://wwx.jyoumei.cn


<!-- 参考信息 -->