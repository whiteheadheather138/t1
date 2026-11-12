代发 wailian999

[Q76] 按天统计
来源：http://uvm.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ilv.cashguo.top

[Q77] 时间加减
来源：http://vvx.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qox.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://jrr.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://klp.hnqzz.top

[Q79] 字符串拼接
来源：http://biz.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rpy.gaohongyu789.top

[Q80] 字符串截取
来源：http://acq.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vrv.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://bdw.daxiang520.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iup.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://eiu.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ign.ivvv.top

[Q83] 大小写转换
来源：http://iyb.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xzd.ywan-chungtsiang.top

[Q84] 去除首尾空格
来源：http://lqo.zhixingplan.top

SELECT TRIM(name) FROM users;
来源：http://tcf.tian-w.cn

[Q85] 数值取整
来源：http://iab.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pvf.chenjidiqi.icu

[Q86] 读取 JSON 字段
来源：http://ccc.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sfg.yonumen.top

[Q87] JSON 字段做条件
来源：http://pta.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pux.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://ygl.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tcv.mhx1999.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tpq.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://eng.tianlin.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bqd.cqqwz.cn

[Q90] 生成序号列
来源：http://nag.fzhhl.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vap.zhongyouzk.top

================================================================================
来源：http://ikt.ydjk.org.cn

R. Bash 专题
来源：http://pub.yuxming.cn

================================================================================
来源：http://byx.aibaodan.cn

[R01] shebang 与严格模式
来源：http://tiz.dashuyun.cn

#!/usr/bin/env bash
来源：http://gyj.jinqigufen.top

set -euo pipefail
来源：http://xux.pengpengdd.cyou

[R02] 变量赋值与使用
来源：http://roc.vehdjk.com

name="Tom"; echo "$name"
来源：http://sfp.jiagoushi.top

[R03] 只读变量
来源：http://run.zhoulong.xyz

readonly PI=3.14
来源：http://cwo.xylfe.cn

[R04] 位置参数
来源：http://fui.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hvj.zhiwuduotai.top

[R05] 参数默认值
来源：http://umb.ybcxt.top

name="${1:-default}"
来源：http://sce.yj202588.top

[R06] 判断命令是否存在
来源：http://wjv.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hha.yj20258888.top

[R07] if 判断文件
来源：http://epz.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eai.svipenyu.cn

[R08] 数值比较
来源：http://fpu.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yrb.pengpengdd.cyou

[R09] 字符串比较
来源：http://tok.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zea.ybcxt.top

[R10] 正则匹配
来源：http://def.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ura.snrcjt.cn

[R11] case 多分支
来源：http://jof.gaohongyu789.top

case "$1" in
来源：http://auv.guowangkeji.top

start) echo "启动" ;;
来源：http://rrt.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://jrv.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://obc.redwolf501.top

esac
来源：http://fne.jiagoushi.top

[R12] for 遍历文件
来源：http://hme.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://gwc.dashuyun.cn

[R13] for 计数循环
来源：http://tnp.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://hdz.sxryk.cn

[R14] C 风格 for
来源：http://drn.fktsv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dhr.cdnleiting.top

[R15] while 逐行读文件
来源：http://bpm.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lak.shanyushiyangtech.top

[R16] until 等待条件
来源：http://ahe.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tdr.xziqi.cn

[R17] 数组定义与取值
来源：http://mlh.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://inh.fengsongda.top

[R18] 遍历数组
来源：http://esg.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hif.jinghuilouyu.cn

[R19] 数组长度
来源：http://eoe.ybcxt.top

echo "${#arr[@]}"
来源：http://mcv.guowangkeji.top

[R20] 关联数组（字典）
来源：http://gsi.dashuyun.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aph.yj20258.top

[R21] 字符串长度
来源：http://ift.jinqigufen.top

echo "${#s}"
来源：http://ctw.sxryk.cn

[R22] 截取子串
来源：http://ftq.vqdsnc.cn

echo "${s:0:5}"
来源：http://phx.jinyuanbaomall.cn

[R23] 字符串替换
来源：http://let.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ncn.dashuyun.cn

[R24] 大小写转换
来源：http://tbl.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://ufr.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://ogp.hongshengwenyu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gyi.hywenlv.cn

[R26] 命令替换
来源：http://fln.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://cqc.jinghuilouyu.cn

[R27] 算术展开
来源：http://muw.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://bvl.52xcode.cn

[R28] 浮点运算
来源：http://wqu.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://axa.yonumen.top

[R29] 定义函数
来源：http://npn.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nnm.daxiang520.top

[R30] 函数返回状态码
来源：http://eel.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://tnz.ctjpmb.com

[R31] 局部变量
来源：http://ayo.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://uqf.hnxiangtu.top

[R32] 参数个数校验
来源：http://ler.smart0.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wqp.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://dgp.sjlbkw.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fva.cdnleiting.top

[R34] 退出时清理
来源：http://ger.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://hkl.epnwcf.com

[R35] 后台执行并等待
来源：http://phh.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bjv.gzhubu.top

[R36] 并发执行多个任务
来源：http://sfu.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dzf.sweek.top

[R37] 把输出赋给变量
来源：http://wum.yueranfly.top

files=$(ls -1)
来源：http://cim.zhoulong.xyz

[R38] 管道串联
来源：http://gup.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://bgu.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://vfm.smart0.xyz

cmd > out.log 2>&1
来源：http://ieb.hesvh.cn

[R40] 追加写日志
来源：http://mxy.yfazqb.com

echo "log" >> out.log
来源：http://bkz.aibaodan.cn

[R41] 丢弃输出
来源：http://ihw.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://kct.ctjpmb.com

[R42] 输入重定向
来源：http://dem.ctjpmb.com

wc -l < a.txt
来源：http://vsa.dashuyun.cn

[R43] 按名字查找文件
来源：http://hiy.hesvh.cn

find . -name "*.log" -type f
来源：http://atn.yuanzhike.top

[R44] 按修改时间查找
来源：http://raz.mhx1999.top

find . -mtime -7 -type f
来源：http://cni.xylfe.cn

[R45] 批量删除
来源：http://rlz.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://vtj.zhixingplan.top

[R46] 递归替换文件内容
来源：http://hzj.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rqw.ydzc1.top

[R47] sed 单行替换
来源：http://jvo.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://ufq.c1oappe.top

[R48] awk 取指定列
来源：http://hzg.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://bsh.chenlongwang.top

[R49] awk 带条件
来源：http://yhz.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wbh.xziqi.cn

[R50] awk 求和
来源：http://dnh.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://cqv.quarkkingdee.top

[R51] 排序去重取前几
来源：http://orj.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mpr.ivvv.top

[R52] 统计行数
来源：http://tty.shzxlz.cn

wc -l a.txt
来源：http://fkr.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://yui.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zli.hnxiangtu.top

[R54] 比较两个文件
来源：http://wvn.birdmap.top

diff a.txt b.txt
来源：http://rfg.tian-w.cn

[R55] 压缩与解压
来源：http://rsx.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngz.yfazqb.com

[R56] 远程拷贝
来源：http://fsq.zdqjudy.top

scp file user@host:/path/
来源：http://mtk.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://qgn.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://hcd.shangyingyoupin.top

[R58] 下载文件
来源：http://tba.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cdf.zhixingplan.top

[R59] 发 POST JSON
来源：http://umb.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cgs.tianlin.xyz

[R60] 只看 HTTP 状态码
来源：http://qhr.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kkl.sjlbkw.cn

[R61] 磁盘占用
来源：http://bqy.tianlin.xyz

df -h;  du -sh *
来源：http://gus.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://tse.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://qmu.yongpay.top

[R63] 内存与进程
来源：http://juc.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://tqs.xuetiantiany.cn

[R64] 结束进程
来源：http://rnp.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://hai.kuanghao11.cn

[R65] 查看端口占用
来源：http://nbg.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://axe.yvedp.cn

[R66] 定时任务
来源：http://obs.cucudq.cn

crontab -e;  crontab -l
来源：http://ktp.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://anb.yj20258888.top

openssl rand -hex 16
来源：http://cyg.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://ruf.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wss.vqdsnc.cn

[R69] 生成随机密码
来源：http://giv.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://onl.guannengcc.top

[R70] 时间戳与互转
来源：http://sel.daria6918.cn

date +%s;  date -d @1700000000
来源：http://uwi.shzxlz.cn

[R71] 日期格式化
来源：http://svo.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://cxj.uphjek.com

[R72] 等待端口就绪
来源：http://dxv.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://chm.pycfn.com

[R73] 分割大日志
来源：http://qfp.bjfxy.top

split -l 1000 big.log part_
来源：http://ncf.sweek.top

[R74] 批量重命名
来源：http://bdf.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rbu.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://auh.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://lsl.smart0.xyz

[R76] 使用临时文件
来源：http://bfo.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://umm.jlsjyb.cn

[R77] 读取用户输入
来源：http://zrc.svipenyu.cn

read -rp "请输入: " ans
来源：http://scz.sjlbkw.cn

[R78] 交互式菜单
来源：http://xtu.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://chd.guowangkeji.top

[R79] 解析命令行选项
来源：http://zpu.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uzf.yj202588.top

[R80] 查看脚本执行耗时
来源：http://aqb.jianghu66.top

time ./run.sh
来源：http://mdu.yonumen.top

================================================================================
来源：http://khj.daria6918.cn

S. C / C++ 专题
来源：http://ybo.birdmap.top

================================================================================
来源：http://tob.havefunace.top

[S01] C：Hello World
来源：http://iiz.ivvv.top

#include <stdio.h>
来源：http://aut.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxi.fehbvm.com

[S02] C：变量与格式化输出
来源：http://elb.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://zmp.haohaochexian.top

[S03] C：读入整数
来源：http://ork.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://uqq.zhengqikj.top

[S04] C：字符串复制
来源：http://nqv.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://lhg.cucudq.cn

[S05] C：字符串长度
来源：http://qzj.zhongyouzk.top

strlen(s)
来源：http://cyj.hfpthk.cn

[S06] C：字符串比较
来源：http://ufv.yj20258888.top

strcmp(a, b) == 0
来源：http://fyx.cashguo.top

[S07] C：数组遍历求和
来源：http://ilr.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zfz.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://vhn.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ghf.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://cwd.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wss.fengsongda.top

[S10] C：指针与解引用
来源：http://ewm.ivvv.top

int *p = &a;  *p = 5;
来源：http://fub.jianghu66.top

[S11] C：逐行读文件
来源：http://vkw.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://lsu.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dmw.meibo888.top

fclose(f);
来源：http://obt.haohaochexian.top

[S12] C：写文件
来源：http://qag.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cvg.yuxming.cn

[S13] C：宏定义
来源：http://lec.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://onb.sweek.top

[S14] C：枚举
来源：http://prb.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://csu.yuxming.cn

[S15] C：类型转换
来源：http://pjs.tian-w.cn

(double) a / b
来源：http://aai.zycfv.cn

[S16] C：位操作置位
来源：http://bqp.yuanzhike.top

x |= (1 << 3);
来源：http://jai.gzhubu.top

[S17] C：安全拼接字符串
来源：http://vfa.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fsc.shzxlz.cn

[S18] C：命令行参数
来源：http://jfg.yonumen.top

int main(int argc, char **argv)
来源：http://ezv.zhijiandao.cn

[S19] C：快速排序
来源：http://qva.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bmr.gaohongyu789.top

[S20] C：二分查找
来源：http://mzy.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nit.jyoumei.cn

[S21] C：字符类别判断
来源：http://fyi.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hcd.ehwqpu.com

[S22] C：字符串转数字
来源：http://sai.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://dev.chenjidiqi.icu

[S23] C：随机数
来源：http://oiw.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qok.xuanzx.com

[S24] C：获取本地时间
来源：http://els.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bhh.yuanzhike.top

[S25] C：内存拷贝
来源：http://dlq.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://smy.yj20258.top

[S26] C：内存清零
来源：http://ojo.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://bpw.tanke756.top

[S27] C：定义常量
来源：http://dbq.fzhhl.top

const double PI = 3.14159;
来源：http://zsc.hcnkem.com

[S28] C：静态变量
来源：http://lqq.xinyue.icu

static int counter = 0;
来源：http://fid.fengsongda.top

[S29] C：变参函数
来源：http://nuv.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://atz.wangdashe.top

[S30] C：头文件保护
来源：http://tmt.iojbl.cn

#ifndef X_H
来源：http://xxb.zhengqikj.top

#define X_H
来源：http://cnz.ydjk.org.cn

#endif
来源：http://ghk.tian-w.cn

[S31] C++：Hello World
来源：http://abc.cashguo.top

#include <iostream>
来源：http://fux.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://ang.ivvv.top

[S32] C++：字符串
来源：http://egq.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://vqc.sysykeji.top

[S33] C++：vector 增删
来源：http://fre.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://foz.316326.xyz

[S34] C++：遍历 vector
来源：http://hwu.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://ajc.ctjpmb.com

[S35] C++：map
来源：http://vhr.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://clc.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://rxi.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://alb.yj202588.top

[S37] C++：set
来源：http://bvy.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vhr.dashuyun.cn

[S38] C++：排序
来源：http://nzj.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://zpu.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://mlh.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qkl.dashuyun.cn

[S40] C++：查找元素
来源：http://jbp.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xup.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://grs.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rok.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://lwr.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://rhn.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://atl.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://jkz.tarul.cn

[S44] C++：引用传参
来源：http://lvp.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://das.kuanghao11.cn

[S45] C++：lambda
来源：http://rjl.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rlh.sysykeji.top

[S46] C++：函数模板
来源：http://dbz.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://klg.tanke756.top


<!-- 参考信息 -->