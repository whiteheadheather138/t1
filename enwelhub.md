代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vom.chenlongwang.top

[Q75] 日期格式化
来源：http://ulg.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cvq.hammf.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kwg.yj202588.top

[Q76] 按天统计
来源：http://aij.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://czj.cashguo.top

[Q77] 时间加减
来源：http://fqp.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://laz.yangfankeji.com

[Q78] 当前时间
来源：http://ckw.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ysv.vqdsnc.cn

[Q79] 字符串拼接
来源：http://rwe.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://njq.dashuyun.cn

[Q80] 字符串截取
来源：http://xyx.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nsw.yj202588.top

[Q81] 字符串替换
来源：http://taa.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jyh.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://fif.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ntt.redwolf501.top

[Q83] 大小写转换
来源：http://pis.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ekl.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://ibb.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://yfl.wangdashe.top

[Q85] 数值取整
来源：http://qkn.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bdy.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://rtr.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qra.ppjwa.cn

[Q87] JSON 字段做条件
来源：http://ivr.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ebs.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://lqo.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://drn.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibd.fengsongda.top

[Q89] 判断表是否存在
来源：http://xgr.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oxd.daria6918.cn

[Q90] 生成序号列
来源：http://pgx.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwx.fzhhl.top

================================================================================
来源：http://hug.jyoumei.cn

R. Bash 专题
来源：http://ndj.bjfxy.top

================================================================================
来源：http://qhs.bbcook.cn

[R01] shebang 与严格模式
来源：http://hei.dianchejie.cn

#!/usr/bin/env bash
来源：http://bcg.epnwcf.com

set -euo pipefail
来源：http://yze.hesvh.cn

[R02] 变量赋值与使用
来源：http://xgm.jiagoushi.top

name="Tom"; echo "$name"
来源：http://ooz.quarkkingdee.top

[R03] 只读变量
来源：http://eka.shanyushiyangtech.top

readonly PI=3.14
来源：http://kpn.tarul.cn

[R04] 位置参数
来源：http://wjp.xinyue.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sed.jlsjyb.cn

[R05] 参数默认值
来源：http://esk.jinqigfzy.top

name="${1:-default}"
来源：http://grq.hywenlv.cn

[R06] 判断命令是否存在
来源：http://ddd.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tut.sjlbkw.cn

[R07] if 判断文件
来源：http://lxd.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qfs.haohaochexian.top

[R08] 数值比较
来源：http://mac.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://aky.ehwqpu.com

[R09] 字符串比较
来源：http://upa.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bij.daria6918.cn

[R10] 正则匹配
来源：http://vaa.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://auv.aizwys.cn

[R11] case 多分支
来源：http://wnf.vehdjk.com

case "$1" in
来源：http://dif.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://fde.sysykeji.top

stop)  echo "停止" ;;
来源：http://fju.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://dxa.chenjidiqi.icu

esac
来源：http://idm.dashuyun.cn

[R12] for 遍历文件
来源：http://hgh.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://rgw.xuetiantiany.cn

[R13] for 计数循环
来源：http://cel.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://eun.feifeiyinyue.top

[R14] C 风格 for
来源：http://eua.yuanzhike.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://usn.cqqwz.cn

[R15] while 逐行读文件
来源：http://dvq.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ijq.yfazqb.com

[R16] until 等待条件
来源：http://app.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qtm.nanxinkj.top

[R17] 数组定义与取值
来源：http://voj.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://ify.zycfv.cn

[R18] 遍历数组
来源：http://ksr.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ztk.hesvh.cn

[R19] 数组长度
来源：http://pzh.meibo888.top

echo "${#arr[@]}"
来源：http://hjq.svipenyu.cn

[R20] 关联数组（字典）
来源：http://gfc.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vuv.svipenyu.cn

[R21] 字符串长度
来源：http://lnm.shanyushiyangkeji.top

echo "${#s}"
来源：http://cwb.quarkkingdee.top

[R22] 截取子串
来源：http://lwc.hammf.cn

echo "${s:0:5}"
来源：http://syp.havefunace.top

[R23] 字符串替换
来源：http://iiz.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pqk.xuetiantiany.cn

[R24] 大小写转换
来源：http://qmx.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://hiq.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://bwz.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wxe.jinghuilouyu.cn

[R26] 命令替换
来源：http://dnj.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://bez.fktsv.cn

[R27] 算术展开
来源：http://bpk.tian-w.cn

echo $((1 + 2 * 3))
来源：http://pow.daria6918.cn

[R28] 浮点运算
来源：http://avb.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://jnn.zdbjq.cn

[R29] 定义函数
来源：http://gxz.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://maq.chenzaomai.com

[R30] 函数返回状态码
来源：http://ouz.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://bxc.hywenlv.cn

[R31] 局部变量
来源：http://bfq.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://quy.zdbjq.cn

[R32] 参数个数校验
来源：http://whz.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://woc.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://qpu.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://frh.yongpay.top

[R34] 退出时清理
来源：http://rdq.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://kjc.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://ujw.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://duo.redwolf501.top

[R36] 并发执行多个任务
来源：http://uyo.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qpw.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://ueu.sxryk.cn

files=$(ls -1)
来源：http://poz.zhiwuduotai.top

[R38] 管道串联
来源：http://osz.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://xje.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://rsb.ctjpmb.com

cmd > out.log 2>&1
来源：http://nqh.zhongyouzk.top

[R40] 追加写日志
来源：http://aur.gzhubu.top

echo "log" >> out.log
来源：http://dnt.aizwys.cn

[R41] 丢弃输出
来源：http://iqv.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://tkq.c1oappe.top

[R42] 输入重定向
来源：http://muz.sysykeji.top

wc -l < a.txt
来源：http://kvi.ppjwa.cn

[R43] 按名字查找文件
来源：http://trn.tanke756.top

find . -name "*.log" -type f
来源：http://mew.316326.xyz

[R44] 按修改时间查找
来源：http://opm.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://uyf.ppjwa.cn

[R45] 批量删除
来源：http://pwl.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://ulk.0kj1m.cn

[R46] 递归替换文件内容
来源：http://auz.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gbp.hnxiangtu.top

[R47] sed 单行替换
来源：http://pno.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jzz.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://agf.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://psk.pycfn.com

[R49] awk 带条件
来源：http://dms.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ije.ydzc1.top

[R50] awk 求和
来源：http://bwo.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://dif.cqqwz.cn

[R51] 排序去重取前几
来源：http://awz.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ssi.tanke756.top

[R52] 统计行数
来源：http://amn.chenzaomai.com

wc -l a.txt
来源：http://gcl.guowangkeji.top

[R53] 查看文件头与实时尾
来源：http://lwc.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oqj.gzhubu.top

[R54] 比较两个文件
来源：http://pln.fanxiaobao.xyz

diff a.txt b.txt
来源：http://lyk.jinqigfzy.top

[R55] 压缩与解压
来源：http://bhy.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bly.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://yub.jinghuilouyu.cn

scp file user@host:/path/
来源：http://lbe.zhengqikj.top

[R57] 远程执行命令
来源：http://lev.cdnleiting.top

ssh user@host 'uptime'
来源：http://evj.shangyingyoupin.top

[R58] 下载文件
来源：http://vyd.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://acr.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://yua.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pxz.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://cbd.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cib.hfpthk.cn

[R61] 磁盘占用
来源：http://rcn.hesvh.cn

df -h;  du -sh *
来源：http://hhw.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://rbr.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://kdg.smart0.xyz

[R63] 内存与进程
来源：http://xlx.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://vvb.ywan-chungtsiang.top

[R64] 结束进程
来源：http://wjx.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://bzk.tianlin.xyz

[R65] 查看端口占用
来源：http://yap.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xli.yonumen.top

[R66] 定时任务
来源：http://fvv.yfazqb.com

crontab -e;  crontab -l
来源：http://ibc.smart0.xyz

[R67] 生成随机十六进制串
来源：http://zcf.smart0.xyz

openssl rand -hex 16
来源：http://txr.gotoacloud.top

[R68] 计算文件校验值
来源：http://tcu.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://ubu.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://gyd.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://zlc.daria6918.cn

[R70] 时间戳与互转
来源：http://iqj.xinyue.icu

date +%s;  date -d @1700000000
来源：http://voy.kuanghao11.cn

[R71] 日期格式化
来源：http://pak.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qls.fengsongda.top

[R72] 等待端口就绪
来源：http://djn.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://diu.jyoumei.cn

[R73] 分割大日志
来源：http://plq.hysaishi.cn

split -l 1000 big.log part_
来源：http://neb.zhixingplan.top

[R74] 批量重命名
来源：http://rxs.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqx.fktsv.cn

[R75] 导出环境变量
来源：http://scm.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://zzs.zhiwuduotai.top

[R76] 使用临时文件
来源：http://dvx.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nbi.gzhubu.top

[R77] 读取用户输入
来源：http://zai.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://xvl.tanke756.top

[R78] 交互式菜单
来源：http://ien.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oen.yj20258888.top

[R79] 解析命令行选项
来源：http://zqs.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uaa.tanke756.top

[R80] 查看脚本执行耗时
来源：http://qbz.c1oappe.top

time ./run.sh
来源：http://bvv.jinqigfzy.top

================================================================================
来源：http://dcb.zhoulong.xyz

S. C / C++ 专题
来源：http://ztc.jinqigufen.top

================================================================================
来源：http://cbj.chenzaomai.com

[S01] C：Hello World
来源：http://ylq.jqgfzy.top

#include <stdio.h>
来源：http://wnm.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iew.ivvv.top

[S02] C：变量与格式化输出
来源：http://ije.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://lrs.sysykeji.top

[S03] C：读入整数
来源：http://bcr.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://qil.cucudq.cn

[S04] C：字符串复制
来源：http://qlm.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://ufj.nwbrower.top

[S05] C：字符串长度
来源：http://avx.yj20258.top

strlen(s)
来源：http://fec.jianghu66.top

[S06] C：字符串比较
来源：http://scv.fktsv.cn

strcmp(a, b) == 0
来源：http://wre.fehbvm.com

[S07] C：数组遍历求和
来源：http://tmn.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://utu.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://bid.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aua.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://lek.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bhr.cqqwz.cn

[S10] C：指针与解引用
来源：http://zsl.fzhhl.top

int *p = &a;  *p = 5;
来源：http://uip.ybcxt.top

[S11] C：逐行读文件
来源：http://mne.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://ifh.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mrb.jqgfzy.top

fclose(f);
来源：http://ycd.cashguo.top

[S12] C：写文件
来源：http://lbd.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eas.bjfxy.top

[S13] C：宏定义
来源：http://alw.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ibh.ivvv.top

[S14] C：枚举
来源：http://jgj.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://iti.tanke756.top

[S15] C：类型转换
来源：http://mlb.guowangkeji.top

(double) a / b
来源：http://mzf.yuanzhike.top

[S16] C：位操作置位
来源：http://kll.hesvh.cn

x |= (1 << 3);
来源：http://uoy.yj202588.top

[S17] C：安全拼接字符串
来源：http://sld.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yit.havefunace.top

[S18] C：命令行参数
来源：http://ngz.hysaishi.cn

int main(int argc, char **argv)
来源：http://glu.dashuyun.cn

[S19] C：快速排序
来源：http://keb.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hsi.sjlbkw.cn

[S20] C：二分查找
来源：http://clw.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cce.yonumen.top

[S21] C：字符类别判断
来源：http://vgu.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cba.aibaodan.cn

[S22] C：字符串转数字
来源：http://xff.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://gkh.yj20258888.top

[S23] C：随机数
来源：http://ftv.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fhq.shzxlz.cn

[S24] C：获取本地时间
来源：http://nkf.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqn.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://nkf.pycfn.com

memcpy(dst, src, n);
来源：http://zdn.dianchejie.cn

[S26] C：内存清零
来源：http://zny.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://jga.xylfe.cn

[S27] C：定义常量
来源：http://azg.zhiwuduotai.top

const double PI = 3.14159;
来源：http://qqv.ydzc1.top

[S28] C：静态变量
来源：http://npo.fzhhl.top

static int counter = 0;
来源：http://rpt.jqgfzy.top

[S29] C：变参函数
来源：http://csx.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jqq.quarkkingdee.top

[S30] C：头文件保护
来源：http://zkn.zhengqikj.top

#ifndef X_H
来源：http://ydh.shzxlz.cn

#define X_H
来源：http://tko.c1oappe.top

#endif
来源：http://xzv.daria6918.cn

[S31] C++：Hello World
来源：http://ept.guannengcc.top

#include <iostream>
来源：http://usa.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://qxu.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://rle.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://oip.nwbrower.top

[S33] C++：vector 增删
来源：http://pdi.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gdk.zhengqikj.top

[S34] C++：遍历 vector
来源：http://kij.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://lbq.guowangkeji.top

[S35] C++：map
来源：http://dbk.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yep.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://uaf.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hzy.jyoumei.cn

[S37] C++：set
来源：http://svx.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vtt.jlsjyb.cn

[S38] C++：排序
来源：http://nvc.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://zxi.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://sjh.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://szu.meibo888.top

[S40] C++：查找元素
来源：http://kuq.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uiy.52xcode.cn

[S41] C++：类与构造函数
来源：http://ozk.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://znw.52xcode.cn

[S42] C++：继承与虚函数
来源：http://xfa.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://lyp.yfazqb.com

[S43] C++：智能指针
来源：http://naf.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://oom.nanxinkj.top

[S44] C++：引用传参
来源：http://saw.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://isf.cqqwz.cn


<!-- 参考信息 -->