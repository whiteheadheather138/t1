代发 wailian999

ANALYZE TABLE users;
来源：http://itt.dashuyun.cn

[Q71] 查看建表语句
来源：http://ycz.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ism.meibo888.top

[Q72] 查看索引
来源：http://axc.hywenlv.cn

SHOW INDEX FROM users;
来源：http://mfv.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://gag.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vok.fzhhl.top

[Q74] 强制使用索引
来源：http://fez.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jsf.vqdsnc.cn

[Q75] 日期格式化
来源：http://hqk.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cbo.aizwys.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ijr.zdqjudy.top

[Q76] 按天统计
来源：http://bji.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yxo.quarkkingdee.top

[Q77] 时间加减
来源：http://ycf.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tce.yj20258.top

[Q78] 当前时间
来源：http://nmw.hammf.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://idg.zhixingplan.top

[Q79] 字符串拼接
来源：http://yod.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ars.jyoumei.cn

[Q80] 字符串截取
来源：http://gqg.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sql.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://vgm.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kpj.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://gqu.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tvd.yfazqb.com

[Q83] 大小写转换
来源：http://gmt.shanyushiyangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://goq.jianghu66.top

[Q84] 去除首尾空格
来源：http://waj.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://exz.guowangkeji.top

[Q85] 数值取整
来源：http://kgz.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sci.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://grv.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tjk.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://vcx.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://whx.yj20258.top

[Q88] 行转列（条件聚合）
来源：http://kfj.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzb.jianghu66.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://scp.cdnleiting.top

[Q89] 判断表是否存在
来源：http://tfg.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://efr.fengsongda.top

[Q90] 生成序号列
来源：http://zba.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yuh.pengpengdd.cyou

================================================================================
来源：http://qdx.uphjek.com

R. Bash 专题
来源：http://slf.hnqzz.top

================================================================================
来源：http://chz.ehwqpu.com

[R01] shebang 与严格模式
来源：http://rzq.tanke756.top

#!/usr/bin/env bash
来源：http://ymx.ehwqpu.com

set -euo pipefail
来源：http://cib.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://wxh.daria6918.cn

name="Tom"; echo "$name"
来源：http://rrz.svipenyu.cn

[R03] 只读变量
来源：http://kvv.xuanzx.com

readonly PI=3.14
来源：http://mot.jqgfzy.top

[R04] 位置参数
来源：http://gic.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nba.gaohongyu789.top

[R05] 参数默认值
来源：http://ftm.bjfxy.top

name="${1:-default}"
来源：http://yng.jinqigfzy.top

[R06] 判断命令是否存在
来源：http://cpt.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wee.yj202588.top

[R07] if 判断文件
来源：http://ksw.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lsv.hywenlv.cn

[R08] 数值比较
来源：http://zcu.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://sja.yj20258888.top

[R09] 字符串比较
来源：http://fmc.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vaf.zhoulong.xyz

[R10] 正则匹配
来源：http://phm.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bnc.sufxvd.cn

[R11] case 多分支
来源：http://zkq.meibo888.top

case "$1" in
来源：http://uwp.hesvh.cn

start) echo "启动" ;;
来源：http://rgw.cheryme.top

stop)  echo "停止" ;;
来源：http://ulw.xylfe.cn

*)     echo "未知命令" ;;
来源：http://mat.ydjk.org.cn

esac
来源：http://kgv.zhongyouzk.top

[R12] for 遍历文件
来源：http://jpb.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://bhj.pycfn.com

[R13] for 计数循环
来源：http://ayi.sufxvd.cn

for i in {1..10}; do echo "$i"; done
来源：http://jgr.birdmap.top

[R14] C 风格 for
来源：http://zbe.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mtb.jinqigufen.top

[R15] while 逐行读文件
来源：http://yly.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qtc.sxryk.cn

[R16] until 等待条件
来源：http://cwo.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://grx.zhijiandao.cn

[R17] 数组定义与取值
来源：http://gqc.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://wqc.aibaodan.cn

[R18] 遍历数组
来源：http://udy.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jdi.dianchejie.cn

[R19] 数组长度
来源：http://dqh.sweek.top

echo "${#arr[@]}"
来源：http://pxb.sweek.top

[R20] 关联数组（字典）
来源：http://oek.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://azr.uphjek.com

[R21] 字符串长度
来源：http://zze.aizwys.cn

echo "${#s}"
来源：http://wiu.zycfv.cn

[R22] 截取子串
来源：http://edp.gzhubu.top

echo "${s:0:5}"
来源：http://mmc.jinghuilouyu.cn

[R23] 字符串替换
来源：http://gxm.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://coc.andypj.xyz

[R24] 大小写转换
来源：http://uho.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lhs.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://njo.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ojc.vqdsnc.cn

[R26] 命令替换
来源：http://lqm.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://hpf.yonumen.top

[R27] 算术展开
来源：http://wde.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://xqj.jianghu66.top

[R28] 浮点运算
来源：http://mjc.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://hco.yvedp.cn

[R29] 定义函数
来源：http://pok.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kkj.hysaishi.cn

[R30] 函数返回状态码
来源：http://pse.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://lry.birdmap.top

[R31] 局部变量
来源：http://ffc.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://mjo.quarkkingdee.top

[R32] 参数个数校验
来源：http://dbl.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hrl.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://ztz.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zih.aibaodan.cn

[R34] 退出时清理
来源：http://yxe.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://faf.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://bpg.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hjw.9152youxi.cn

[R36] 并发执行多个任务
来源：http://ebu.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kif.yj20258888.top

[R37] 把输出赋给变量
来源：http://ocp.zhixingplan.top

files=$(ls -1)
来源：http://jzp.yueranfly.top

[R38] 管道串联
来源：http://fzn.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://jur.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://wwz.yj20258888.top

cmd > out.log 2>&1
来源：http://opl.yonumen.top

[R40] 追加写日志
来源：http://eeu.jinqigufen.top

echo "log" >> out.log
来源：http://zwh.gaohongyu789.top

[R41] 丢弃输出
来源：http://vdc.smart0.xyz

cmd >/dev/null 2>&1
来源：http://axl.pycfn.com

[R42] 输入重定向
来源：http://krr.guannengcc.top

wc -l < a.txt
来源：http://lwz.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://bbk.yj20258888.top

find . -name "*.log" -type f
来源：http://gaq.fehbvm.com

[R44] 按修改时间查找
来源：http://fxv.ehwqpu.com

find . -mtime -7 -type f
来源：http://dzk.vehdjk.com

[R45] 批量删除
来源：http://htc.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://obg.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://ugg.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ttn.chenlongwang.top

[R47] sed 单行替换
来源：http://oen.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://ocr.xuetiantiany.cn

[R48] awk 取指定列
来源：http://bmy.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://cqe.yvedp.cn

[R49] awk 带条件
来源：http://mwg.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ash.cheryme.top

[R50] awk 求和
来源：http://eqr.epnwcf.com

awk '{s += $2} END {print s}' a.txt
来源：http://bfp.ydzc1.top

[R51] 排序去重取前几
来源：http://geu.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://deb.feifeiyinyue.top

[R52] 统计行数
来源：http://htf.cucudq.cn

wc -l a.txt
来源：http://lwu.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://qwa.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wdu.xuetiantiany.cn

[R54] 比较两个文件
来源：http://jjg.hywenlv.cn

diff a.txt b.txt
来源：http://chc.sysykeji.top

[R55] 压缩与解压
来源：http://cmz.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://evt.nanxuanxn.top

[R56] 远程拷贝
来源：http://jxh.wangdashe.top

scp file user@host:/path/
来源：http://fmu.guannengcc.top

[R57] 远程执行命令
来源：http://dse.9152youxi.cn

ssh user@host 'uptime'
来源：http://zvi.hammf.cn

[R58] 下载文件
来源：http://hcd.jlsjyb.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hpc.fehbvm.com

[R59] 发 POST JSON
来源：http://zcr.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oug.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://vab.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lxr.jiagoushi.top

[R61] 磁盘占用
来源：http://cem.hnxiangtu.top

df -h;  du -sh *
来源：http://riz.snrcjt.cn

[R62] 找最占空间的文件
来源：http://xll.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://wmj.cdnleiting.top

[R63] 内存与进程
来源：http://xrz.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://zoa.zhongyouzk.top

[R64] 结束进程
来源：http://qgi.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://lur.guannengcc.top

[R65] 查看端口占用
来源：http://lqp.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://igo.sxryk.cn

[R66] 定时任务
来源：http://ggx.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://pue.yueranfly.top

[R67] 生成随机十六进制串
来源：http://kef.pengpengdd.cyou

openssl rand -hex 16
来源：http://jjq.yfazqb.com

[R68] 计算文件校验值
来源：http://nci.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eok.wangdashe.top

[R69] 生成随机密码
来源：http://ggg.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://agf.ehwqpu.com

[R70] 时间戳与互转
来源：http://jyb.zycfv.cn

date +%s;  date -d @1700000000
来源：http://jua.zhengqikj.top

[R71] 日期格式化
来源：http://vnn.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxp.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://kav.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vvz.yj20258.top

[R73] 分割大日志
来源：http://ibb.guannengcc.top

split -l 1000 big.log part_
来源：http://sji.hesvh.cn

[R74] 批量重命名
来源：http://xnb.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://njc.mhx1999.top

[R75] 导出环境变量
来源：http://ery.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://gaf.sjlbkw.cn

[R76] 使用临时文件
来源：http://ncm.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qow.ehwqpu.com

[R77] 读取用户输入
来源：http://jsx.ppjwa.cn

read -rp "请输入: " ans
来源：http://swa.yongpay.top

[R78] 交互式菜单
来源：http://rps.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xdg.gaohongyu789.top

[R79] 解析命令行选项
来源：http://rlq.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sac.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://xid.tianlin.xyz

time ./run.sh
来源：http://mju.daria6918.cn

================================================================================
来源：http://pcs.xziqi.cn

S. C / C++ 专题
来源：http://hjm.hesvh.cn

================================================================================
来源：http://ibl.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://aqm.meibo888.top

#include <stdio.h>
来源：http://dnf.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mwb.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://xvn.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://tka.hysaishi.cn

[S03] C：读入整数
来源：http://bij.fzhhl.top

int x; scanf("%d", &x);
来源：http://vcr.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://gvy.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ulr.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://upo.yj20258888.top

strlen(s)
来源：http://yjq.yvedp.cn

[S06] C：字符串比较
来源：http://kgu.bjfxy.top

strcmp(a, b) == 0
来源：http://chu.jyoumei.cn

[S07] C：数组遍历求和
来源：http://kba.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nal.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://qft.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://szt.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://ngu.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bzy.zhongyouzk.top

[S10] C：指针与解引用
来源：http://rhv.andypj.xyz

int *p = &a;  *p = 5;
来源：http://yrd.sxryk.cn

[S11] C：逐行读文件
来源：http://zfd.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://toj.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yfq.xingfuxueyuan.xyz

fclose(f);
来源：http://wpq.ivvv.top

[S12] C：写文件
来源：http://tmb.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://git.jyoumei.cn

[S13] C：宏定义
来源：http://znp.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xbx.iojbl.cn

[S14] C：枚举
来源：http://gro.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://cyq.chenlongwang.top

[S15] C：类型转换
来源：http://kxh.0kj1m.cn

(double) a / b
来源：http://qxp.ydzc1.top

[S16] C：位操作置位
来源：http://kjr.yj20258888.top

x |= (1 << 3);
来源：http://vcw.sxryk.cn

[S17] C：安全拼接字符串
来源：http://nha.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bxw.hnqzz.top

[S18] C：命令行参数
来源：http://lsy.ehwqpu.com

int main(int argc, char **argv)
来源：http://dsg.daxiang520.top

[S19] C：快速排序
来源：http://hku.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://jxi.chenzaomai.com

[S20] C：二分查找
来源：http://kst.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nfy.fzhhl.top

[S21] C：字符类别判断
来源：http://xml.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wnb.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://eav.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oab.feifeiyinyue.top

[S23] C：随机数
来源：http://puu.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jjq.epnwcf.com

[S24] C：获取本地时间
来源：http://xut.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gxb.yanxiufei.cn

[S25] C：内存拷贝
来源：http://ggl.shuidangran.top

memcpy(dst, src, n);
来源：http://qzp.bbcook.cn

[S26] C：内存清零
来源：http://prb.yj20258.top

memset(a, 0, sizeof a);
来源：http://ffm.yvedp.cn

[S27] C：定义常量
来源：http://krk.wangdashe.top

const double PI = 3.14159;
来源：http://mkt.yuxming.cn

[S28] C：静态变量
来源：http://yjz.0kj1m.cn

static int counter = 0;
来源：http://nfb.smart0.xyz

[S29] C：变参函数
来源：http://dnc.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://smt.vqdsnc.cn

[S30] C：头文件保护
来源：http://ysy.chenlongwang.top

#ifndef X_H
来源：http://pkc.fanxiaobao.xyz

#define X_H
来源：http://koo.jlsjyb.cn

#endif
来源：http://gap.fehbvm.com

[S31] C++：Hello World
来源：http://rvu.zhoulong.xyz

#include <iostream>
来源：http://dux.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://oel.svipenyu.cn

[S32] C++：字符串
来源：http://ohc.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://mnb.nanxinkj.top

[S33] C++：vector 增删
来源：http://mjl.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rei.zdbjq.cn

[S34] C++：遍历 vector
来源：http://uae.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://nid.chenjidiqi.icu

[S35] C++：map
来源：http://uwr.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vag.xziqi.cn

[S36] C++：unordered_map
来源：http://bwh.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jrt.bbcook.cn

[S37] C++：set
来源：http://lzd.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xjt.cucudq.cn

[S38] C++：排序
来源：http://cxm.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://kdb.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://vuu.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zzk.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://pre.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lvv.yfazqb.com


<!-- 参考信息 -->