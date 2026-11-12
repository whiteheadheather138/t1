代发 wailian999

ANALYZE TABLE users;
来源：http://gsy.zhengqikj.top

[Q71] 查看建表语句
来源：http://hxz.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xyg.316326.xyz

[Q72] 查看索引
来源：http://jom.fzhhl.top

SHOW INDEX FROM users;
来源：http://xwk.chenzaomai.com

[Q73] 查看表状态
来源：http://lrd.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xcv.316326.xyz

[Q74] 强制使用索引
来源：http://kro.jqgfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bcu.tanke756.top

[Q75] 日期格式化
来源：http://dlv.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mfp.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rpv.yj20258888.top

[Q76] 按天统计
来源：http://bgr.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ffo.yueranfly.top

[Q77] 时间加减
来源：http://oon.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rcq.gzhubu.top

[Q78] 当前时间
来源：http://mux.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mkh.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://nhl.zhongyouzk.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://puo.pycfn.com

[Q80] 字符串截取
来源：http://bnj.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ump.yongpay.top

[Q81] 字符串替换
来源：http://keb.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oxb.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://kus.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://knl.bjfxy.top

[Q83] 大小写转换
来源：http://quk.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pgg.ybcxt.top

[Q84] 去除首尾空格
来源：http://zhv.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://qbg.fehbvm.com

[Q85] 数值取整
来源：http://bis.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kle.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://ekh.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rkz.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://etp.ctjpmb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xxy.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://fwq.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://djr.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tfq.yuxming.cn

[Q89] 判断表是否存在
来源：http://oae.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zps.yongpay.top

[Q90] 生成序号列
来源：http://oix.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nsm.ydjk.org.cn

================================================================================
来源：http://rcf.ybcxt.top

R. Bash 专题
来源：http://ztd.zdbjq.cn

================================================================================
来源：http://emd.sjlbkw.cn

[R01] shebang 与严格模式
来源：http://wuh.pengpengdd.cyou

#!/usr/bin/env bash
来源：http://sgm.iojbl.cn

set -euo pipefail
来源：http://nng.fktsv.cn

[R02] 变量赋值与使用
来源：http://wvn.cdnleiting.top

name="Tom"; echo "$name"
来源：http://zzd.ppjwa.cn

[R03] 只读变量
来源：http://sms.jlsjyb.cn

readonly PI=3.14
来源：http://zwa.fehbvm.com

[R04] 位置参数
来源：http://vcn.cheryme.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tpz.xuanzx.com

[R05] 参数默认值
来源：http://fbj.yangfankeji.com

name="${1:-default}"
来源：http://tjo.cucudq.cn

[R06] 判断命令是否存在
来源：http://eby.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sne.daria6918.cn

[R07] if 判断文件
来源：http://uxz.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gmt.yonumen.top

[R08] 数值比较
来源：http://coq.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lbh.jqgfzy.top

[R09] 字符串比较
来源：http://wir.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://klt.iojbl.cn

[R10] 正则匹配
来源：http://fhw.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lcw.zdqjudy.top

[R11] case 多分支
来源：http://hff.sysykeji.top

case "$1" in
来源：http://tiz.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://tnx.dashuyun.cn

stop)  echo "停止" ;;
来源：http://jfg.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://rhf.zdbjq.cn

esac
来源：http://tmq.chenlongwang.top

[R12] for 遍历文件
来源：http://dbq.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://adl.shuidangran.top

[R13] for 计数循环
来源：http://dqu.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://eps.smart0.xyz

[R14] C 风格 for
来源：http://rph.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pua.sysykeji.top

[R15] while 逐行读文件
来源：http://jsv.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jdw.daria6918.cn

[R16] until 等待条件
来源：http://yqw.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fri.sweek.top

[R17] 数组定义与取值
来源：http://vyh.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://kfg.xylfe.cn

[R18] 遍历数组
来源：http://qtg.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bkd.hcnkem.com

[R19] 数组长度
来源：http://qxf.jqgfzy.top

echo "${#arr[@]}"
来源：http://jmw.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://brp.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsp.feifeiyinyue.top

[R21] 字符串长度
来源：http://omg.yj20258.top

echo "${#s}"
来源：http://fcg.cashguo.top

[R22] 截取子串
来源：http://bqo.tianlin.xyz

echo "${s:0:5}"
来源：http://mvu.aizwys.cn

[R23] 字符串替换
来源：http://rlh.tanke756.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lfh.tianlin.xyz

[R24] 大小写转换
来源：http://ius.shangyingyoupin.top

echo "${s^^}"; echo "${s,,}"
来源：http://dum.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://yfr.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://imt.jinqigfzy.top

[R26] 命令替换
来源：http://ueg.316326.xyz

now=$(date +%F); echo "$now"
来源：http://qhw.fzhhl.top

[R27] 算术展开
来源：http://lbq.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://kwu.haohaochexian.top

[R28] 浮点运算
来源：http://cvc.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://asg.ctjpmb.com

[R29] 定义函数
来源：http://xdn.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dvu.xziqi.cn

[R30] 函数返回状态码
来源：http://swc.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://xjr.daria6918.cn

[R31] 局部变量
来源：http://jkh.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://mnu.fehbvm.com

[R32] 参数个数校验
来源：http://xoj.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jig.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://tib.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pst.wangshuangyany.cn

[R34] 退出时清理
来源：http://dfc.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wgn.gaohongyu789.top

[R35] 后台执行并等待
来源：http://ohr.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://cra.tanke756.top

[R36] 并发执行多个任务
来源：http://gzc.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yuj.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://mpq.zycfv.cn

files=$(ls -1)
来源：http://knz.shanyushiyangkeji.top

[R38] 管道串联
来源：http://kjg.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://fqx.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://kso.svipenyu.cn

cmd > out.log 2>&1
来源：http://fgp.daria6918.cn

[R40] 追加写日志
来源：http://epr.jianghu66.top

echo "log" >> out.log
来源：http://tpo.epnwcf.com

[R41] 丢弃输出
来源：http://luv.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://utn.ydzc1.top

[R42] 输入重定向
来源：http://tjd.fzhhl.top

wc -l < a.txt
来源：http://lez.0kj1m.cn

[R43] 按名字查找文件
来源：http://tpc.xinyue.icu

find . -name "*.log" -type f
来源：http://gws.yuanzhike.top

[R44] 按修改时间查找
来源：http://tzr.sysykeji.top

find . -mtime -7 -type f
来源：http://lpa.snrcjt.cn

[R45] 批量删除
来源：http://dju.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://bum.nanxinkj.top

[R46] 递归替换文件内容
来源：http://nud.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ziv.jlsjyb.cn

[R47] sed 单行替换
来源：http://djf.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dqo.daria6918.cn

[R48] awk 取指定列
来源：http://vwb.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://wic.ydzc1.top

[R49] awk 带条件
来源：http://veg.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xzc.jyoumei.cn

[R50] awk 求和
来源：http://idq.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://srk.hesvh.cn

[R51] 排序去重取前几
来源：http://fmq.yj202588.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ogn.zhiwuduotai.top

[R52] 统计行数
来源：http://jfs.jinqigfzy.top

wc -l a.txt
来源：http://dvv.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://msd.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://abt.kuanghao11.cn

[R54] 比较两个文件
来源：http://dzp.cucudq.cn

diff a.txt b.txt
来源：http://shg.xuanzx.com

[R55] 压缩与解压
来源：http://vlc.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://inw.yongpay.top

[R56] 远程拷贝
来源：http://zgc.zhiwuduotai.top

scp file user@host:/path/
来源：http://abc.dianchejie.cn

[R57] 远程执行命令
来源：http://ddm.pycfn.com

ssh user@host 'uptime'
来源：http://axw.xylfe.cn

[R58] 下载文件
来源：http://thi.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ehe.tarul.cn

[R59] 发 POST JSON
来源：http://lrg.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ofd.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://mbz.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yao.jinqigufen.top

[R61] 磁盘占用
来源：http://jvi.feifeiyinyue.top

df -h;  du -sh *
来源：http://seb.tanke756.top

[R62] 找最占空间的文件
来源：http://dti.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://kay.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://iie.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://ftm.vehdjk.com

[R64] 结束进程
来源：http://gde.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://rqd.gzhubu.top

[R65] 查看端口占用
来源：http://ijk.zycfv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cpc.ydzc1.top

[R66] 定时任务
来源：http://csj.jqgufenzy.top

crontab -e;  crontab -l
来源：http://zra.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://rar.shuidangran.top

openssl rand -hex 16
来源：http://zbc.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://fkn.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zjz.cdnleiting.top

[R69] 生成随机密码
来源：http://npu.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://ptv.haohaochexian.top

[R70] 时间戳与互转
来源：http://zbp.yj20258888.top

date +%s;  date -d @1700000000
来源：http://uva.xziqi.cn

[R71] 日期格式化
来源：http://dnh.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pmc.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://nbt.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://qid.snrcjt.cn

[R73] 分割大日志
来源：http://mus.chenzaomai.com

split -l 1000 big.log part_
来源：http://lkl.ehwqpu.com

[R74] 批量重命名
来源：http://owe.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://awh.pengpengdd.cyou

[R75] 导出环境变量
来源：http://nta.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://yaf.fehbvm.com

[R76] 使用临时文件
来源：http://mbf.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://loy.ydzc1.top

[R77] 读取用户输入
来源：http://hjf.xinyue.icu

read -rp "请输入: " ans
来源：http://baj.zhengqikj.top

[R78] 交互式菜单
来源：http://fpi.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gyn.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://qba.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://imn.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://eou.sjlbkw.cn

time ./run.sh
来源：http://rsn.smart0.xyz

================================================================================
来源：http://ewp.yuanzhike.top

S. C / C++ 专题
来源：http://qbl.tarul.cn

================================================================================
来源：http://utg.cucudq.cn

[S01] C：Hello World
来源：http://uga.hywenlv.cn

#include <stdio.h>
来源：http://qfs.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xxw.ydzc1.top

[S02] C：变量与格式化输出
来源：http://kcm.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://rht.hesvh.cn

[S03] C：读入整数
来源：http://koi.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://rpf.guannengcc.top

[S04] C：字符串复制
来源：http://dly.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://rik.9152youxi.cn

[S05] C：字符串长度
来源：http://tci.hcnkem.com

strlen(s)
来源：http://wlg.kuanghao11.cn

[S06] C：字符串比较
来源：http://utz.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://fut.xylfe.cn

[S07] C：数组遍历求和
来源：http://gan.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kyc.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://cbg.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hxk.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://rtc.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://erh.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://htj.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://ful.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://zwi.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://kvg.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nyk.xinyue.icu

fclose(f);
来源：http://mye.vehdjk.com

[S12] C：写文件
来源：http://chm.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qta.yvedp.cn

[S13] C：宏定义
来源：http://tcp.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://udx.andypj.xyz

[S14] C：枚举
来源：http://dko.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://und.zhongyouzk.top

[S15] C：类型转换
来源：http://jcw.jinghuilouyu.cn

(double) a / b
来源：http://gij.yangfankeji.com

[S16] C：位操作置位
来源：http://wee.kuanghao11.cn

x |= (1 << 3);
来源：http://jdp.xylfe.cn

[S17] C：安全拼接字符串
来源：http://orr.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dhr.mhx1999.top

[S18] C：命令行参数
来源：http://acy.hesvh.cn

int main(int argc, char **argv)
来源：http://dcm.zycfv.cn

[S19] C：快速排序
来源：http://zjp.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fpa.hongshengwenyu.top

[S20] C：二分查找
来源：http://xts.hfpthk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nft.gogol.net.cn

[S21] C：字符类别判断
来源：http://tey.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lbc.vqdsnc.cn

[S22] C：字符串转数字
来源：http://cwy.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vkk.yj202588.top

[S23] C：随机数
来源：http://ony.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://frb.jqgfzy.top

[S24] C：获取本地时间
来源：http://kyw.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://snt.gogol.net.cn

[S25] C：内存拷贝
来源：http://pfl.ydjk.org.cn

memcpy(dst, src, n);
来源：http://hho.ivvv.top

[S26] C：内存清零
来源：http://bjn.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://zcn.tian-w.cn

[S27] C：定义常量
来源：http://ziq.cdnleiting.top

const double PI = 3.14159;
来源：http://fob.yvedp.cn

[S28] C：静态变量
来源：http://mxc.cqqwz.cn

static int counter = 0;
来源：http://rtp.shuidangran.top

[S29] C：变参函数
来源：http://cvf.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://quu.dashuyun.cn

[S30] C：头文件保护
来源：http://wvm.hnxiangtu.top

#ifndef X_H
来源：http://nrt.yanxiufei.cn

#define X_H
来源：http://sau.hywenlv.cn

#endif
来源：http://qhd.sweek.top

[S31] C++：Hello World
来源：http://ync.yonumen.top

#include <iostream>
来源：http://ucs.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://poq.ivvv.top

[S32] C++：字符串
来源：http://jro.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://soo.ydjk.org.cn

[S33] C++：vector 增删
来源：http://sca.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vqr.zhixingplan.top

[S34] C++：遍历 vector
来源：http://ynu.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://uwl.hongshengwenyu.top

[S35] C++：map
来源：http://ajo.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ikl.cheryme.top

[S36] C++：unordered_map
来源：http://nip.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hdb.shanyushiyangtech.top

[S37] C++：set
来源：http://cjc.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rcz.yvedp.cn

[S38] C++：排序
来源：http://kqa.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://ujy.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://iue.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uic.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://yus.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyd.hysaishi.cn


<!-- 参考信息 -->