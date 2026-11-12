代发 wailian999

[Q67] 设置隔离级别
来源：http://wxc.zdbjq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://juz.zhijiandao.cn

[Q68] 保存点
来源：http://nip.jinqigufen.top

SAVEPOINT sp1;
来源：http://dwl.haohaochexian.top

ROLLBACK TO sp1;
来源：http://klq.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://ryo.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fzr.cheryme.top

[Q70] 更新统计信息
来源：http://hbd.mhx1999.top

ANALYZE TABLE users;
来源：http://kfa.yongpay.top

[Q71] 查看建表语句
来源：http://vlf.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://umh.guowangkeji.top

[Q72] 查看索引
来源：http://usj.iojbl.cn

SHOW INDEX FROM users;
来源：http://qju.yj20258888.top

[Q73] 查看表状态
来源：http://vhe.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://akb.yuanzhike.top

[Q74] 强制使用索引
来源：http://kwp.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://klf.fzhhl.top

[Q75] 日期格式化
来源：http://svf.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://emf.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://grz.9152youxi.cn

[Q76] 按天统计
来源：http://lzr.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tkp.sufxvd.cn

[Q77] 时间加减
来源：http://cpm.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cxk.guowangkeji.top

[Q78] 当前时间
来源：http://xpb.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jec.yuxming.cn

[Q79] 字符串拼接
来源：http://ozp.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eog.epnwcf.com

[Q80] 字符串截取
来源：http://kfx.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wgv.ybcxt.top

[Q81] 字符串替换
来源：http://yhn.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tvs.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://rzu.ehwqpu.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uzv.guannengcc.top

[Q83] 大小写转换
来源：http://djm.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vlj.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://cqo.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://koc.snrcjt.cn

[Q85] 数值取整
来源：http://urd.sysykeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zdw.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://mji.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jmv.hcnkem.com

[Q87] JSON 字段做条件
来源：http://apz.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yeg.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://wjy.ppjwa.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qee.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gls.epnwcf.com

[Q89] 判断表是否存在
来源：http://fkm.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ptm.kuanghao11.cn

[Q90] 生成序号列
来源：http://yfn.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mmz.hnxiangtu.top

================================================================================
来源：http://okm.hcnkem.com

R. Bash 专题
来源：http://otn.ehwqpu.com

================================================================================
来源：http://iog.yonumen.top

[R01] shebang 与严格模式
来源：http://aoa.chenzaomai.com

#!/usr/bin/env bash
来源：http://mbe.andypj.xyz

set -euo pipefail
来源：http://qzb.guowangkeji.top

[R02] 变量赋值与使用
来源：http://mns.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://xbw.jlsjyb.cn

[R03] 只读变量
来源：http://vhp.hnqzz.top

readonly PI=3.14
来源：http://tiz.shuidangran.top

[R04] 位置参数
来源：http://rdj.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mnt.hywenlv.cn

[R05] 参数默认值
来源：http://iwq.jianghu66.top

name="${1:-default}"
来源：http://gis.xinyue.icu

[R06] 判断命令是否存在
来源：http://pgu.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hqr.hongshengwenyu.top

[R07] if 判断文件
来源：http://ksg.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kqn.jinghuilouyu.cn

[R08] 数值比较
来源：http://yuh.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qaz.yuxming.cn

[R09] 字符串比较
来源：http://vfh.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pwl.zhiwuduotai.top

[R10] 正则匹配
来源：http://upn.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bcy.sysykeji.top

[R11] case 多分支
来源：http://ksh.jinyuanbaomall.cn

case "$1" in
来源：http://vzo.ydjk.org.cn

start) echo "启动" ;;
来源：http://bxu.zhixingplan.top

stop)  echo "停止" ;;
来源：http://xdt.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://sck.sxryk.cn

esac
来源：http://czc.nanxinkj.top

[R12] for 遍历文件
来源：http://cqo.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://sbj.epnwcf.com

[R13] for 计数循环
来源：http://hgh.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://xce.ppjwa.cn

[R14] C 风格 for
来源：http://fap.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://squ.nanxuanxn.top

[R15] while 逐行读文件
来源：http://ydl.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tut.epnwcf.com

[R16] until 等待条件
来源：http://uid.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://znf.cdnleiting.top

[R17] 数组定义与取值
来源：http://ytt.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ghg.ehwqpu.com

[R18] 遍历数组
来源：http://vwd.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pvi.birdmap.top

[R19] 数组长度
来源：http://wvr.tianlin.xyz

echo "${#arr[@]}"
来源：http://mxm.zhixingplan.top

[R20] 关联数组（字典）
来源：http://shm.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dwb.quarkkingdee.top

[R21] 字符串长度
来源：http://rje.yuanzhike.top

echo "${#s}"
来源：http://nkr.yuxming.cn

[R22] 截取子串
来源：http://vzc.316326.xyz

echo "${s:0:5}"
来源：http://kyp.wangdashe.top

[R23] 字符串替换
来源：http://bew.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nkg.yuanzhike.top

[R24] 大小写转换
来源：http://ihe.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://qig.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://taq.haohaochexian.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rtj.pengpengdd.cyou

[R26] 命令替换
来源：http://lme.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://urw.yfazqb.com

[R27] 算术展开
来源：http://zgc.gzhubu.top

echo $((1 + 2 * 3))
来源：http://sbj.hongshengwenyu.top

[R28] 浮点运算
来源：http://wid.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://aon.jqgufenzy.top

[R29] 定义函数
来源：http://akr.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://adh.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://btt.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://ucv.gaohongyu789.top

[R31] 局部变量
来源：http://trn.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://igb.yanxiufei.cn

[R32] 参数个数校验
来源：http://rkd.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yky.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://anu.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uqx.pengpengdd.cyou

[R34] 退出时清理
来源：http://mdt.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zin.zhengqikj.top

[R35] 后台执行并等待
来源：http://mgp.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nxq.yfazqb.com

[R36] 并发执行多个任务
来源：http://yrw.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fug.daria6918.cn

[R37] 把输出赋给变量
来源：http://gmc.wangdashe.top

files=$(ls -1)
来源：http://rdg.ywan-chungtsiang.top

[R38] 管道串联
来源：http://csi.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://mke.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://xac.fehbvm.com

cmd > out.log 2>&1
来源：http://dma.0kj1m.cn

[R40] 追加写日志
来源：http://uxs.vehdjk.com

echo "log" >> out.log
来源：http://pca.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://nli.yuxming.cn

cmd >/dev/null 2>&1
来源：http://eno.aizwys.cn

[R42] 输入重定向
来源：http://cmo.yj20258.top

wc -l < a.txt
来源：http://jxu.iojbl.cn

[R43] 按名字查找文件
来源：http://jrt.smart0.xyz

find . -name "*.log" -type f
来源：http://grp.guowangkeji.top

[R44] 按修改时间查找
来源：http://iyu.snrcjt.cn

find . -mtime -7 -type f
来源：http://ujg.jinghuilouyu.cn

[R45] 批量删除
来源：http://knp.birdmap.top

find . -name "*.tmp" -delete
来源：http://xaq.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://pvt.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hkz.gotoacloud.top

[R47] sed 单行替换
来源：http://wnr.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://ifi.cdnleiting.top

[R48] awk 取指定列
来源：http://tok.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://zgm.zhixingplan.top

[R49] awk 带条件
来源：http://udm.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lso.zdbjq.cn

[R50] awk 求和
来源：http://nie.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://bbt.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://cfg.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://rfe.xziqi.cn

[R52] 统计行数
来源：http://dwz.yfazqb.com

wc -l a.txt
来源：http://jwi.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://ibh.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dkr.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://aag.shanyushiyangtech.top

diff a.txt b.txt
来源：http://vnq.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://fhb.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://amv.yonumen.top

[R56] 远程拷贝
来源：http://epg.gotoacloud.top

scp file user@host:/path/
来源：http://zmw.9152youxi.cn

[R57] 远程执行命令
来源：http://yzh.andypj.xyz

ssh user@host 'uptime'
来源：http://fgf.havefunace.top

[R58] 下载文件
来源：http://szu.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://biq.zhoulong.xyz

[R59] 发 POST JSON
来源：http://wiu.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jor.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://lgd.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aqm.wangdashe.top

[R61] 磁盘占用
来源：http://wwv.chenlongwang.top

df -h;  du -sh *
来源：http://myr.havefunace.top

[R62] 找最占空间的文件
来源：http://gff.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://ele.zhixingplan.top

[R63] 内存与进程
来源：http://lcu.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://guz.ehwqpu.com

[R64] 结束进程
来源：http://jjz.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://pkp.ehwqpu.com

[R65] 查看端口占用
来源：http://hro.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpc.dianchejie.cn

[R66] 定时任务
来源：http://twp.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://rva.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://ofg.sjlbkw.cn

openssl rand -hex 16
来源：http://iqe.zhongyouzk.top

[R68] 计算文件校验值
来源：http://urf.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://uoc.ivvv.top

[R69] 生成随机密码
来源：http://jhf.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://uvb.yangfankeji.com

[R70] 时间戳与互转
来源：http://tmy.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://fmb.gotoacloud.top

[R71] 日期格式化
来源：http://mpt.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dyb.ivvv.top

[R72] 等待端口就绪
来源：http://pjc.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://khq.zhixingplan.top

[R73] 分割大日志
来源：http://dpg.daria6918.cn

split -l 1000 big.log part_
来源：http://lob.fanxiaobao.xyz

[R74] 批量重命名
来源：http://leb.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uga.ctjpmb.com

[R75] 导出环境变量
来源：http://cdq.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://twk.zdqjudy.top

[R76] 使用临时文件
来源：http://nvd.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://luv.jinqigufen.top

[R77] 读取用户输入
来源：http://xfu.mhx1999.top

read -rp "请输入: " ans
来源：http://tcn.zhijiandao.cn

[R78] 交互式菜单
来源：http://erl.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ulu.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://tde.zhaomingkeji.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pfy.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://dud.redwolf501.top

time ./run.sh
来源：http://sda.jyoumei.cn

================================================================================
来源：http://cgc.gaohongyu789.top

S. C / C++ 专题
来源：http://vjf.hongshengwenyu.top

================================================================================
来源：http://khz.guowangkeji.top

[S01] C：Hello World
来源：http://mbm.zhoulong.xyz

#include <stdio.h>
来源：http://zog.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://htx.fengsongda.top

[S02] C：变量与格式化输出
来源：http://goy.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://arc.zhoulong.xyz

[S03] C：读入整数
来源：http://ekr.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://qtf.cdnleiting.top

[S04] C：字符串复制
来源：http://cne.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://usa.xuanzx.com

[S05] C：字符串长度
来源：http://rje.epnwcf.com

strlen(s)
来源：http://ygi.zycfv.cn

[S06] C：字符串比较
来源：http://vds.zdqjudy.top

strcmp(a, b) == 0
来源：http://lij.ydzc1.top

[S07] C：数组遍历求和
来源：http://uul.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yaw.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://kjt.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xos.pycfn.com

[S09] C：结构体定义与初始化
来源：http://svc.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ygh.yueranfly.top

[S10] C：指针与解引用
来源：http://pnv.cashguo.top

int *p = &a;  *p = 5;
来源：http://ven.ppjwa.cn

[S11] C：逐行读文件
来源：http://lgk.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://nly.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rac.c1oappe.top

fclose(f);
来源：http://rsg.havefunace.top

[S12] C：写文件
来源：http://tqw.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ubf.hammf.cn

[S13] C：宏定义
来源：http://fur.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mnl.zdbjq.cn

[S14] C：枚举
来源：http://rvm.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://hjk.nwbrower.top

[S15] C：类型转换
来源：http://aqr.cucudq.cn

(double) a / b
来源：http://pbi.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://pqy.guowangkeji.top

x |= (1 << 3);
来源：http://rlb.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://utg.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ckd.fktsv.cn

[S18] C：命令行参数
来源：http://nor.pycfn.com

int main(int argc, char **argv)
来源：http://gdi.gotoacloud.top

[S19] C：快速排序
来源：http://rpf.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://quf.svipenyu.cn

[S20] C：二分查找
来源：http://ldm.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zsr.hcnkem.com

[S21] C：字符类别判断
来源：http://ugz.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zoy.ehwqpu.com

[S22] C：字符串转数字
来源：http://ozz.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://zbq.xylfe.cn

[S23] C：随机数
来源：http://hxu.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vct.chenzaomai.com

[S24] C：获取本地时间
来源：http://rub.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zhp.yj20258.top

[S25] C：内存拷贝
来源：http://zvz.0kj1m.cn

memcpy(dst, src, n);
来源：http://fgu.c1oappe.top

[S26] C：内存清零
来源：http://hid.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://ocu.pengpengdd.cyou

[S27] C：定义常量
来源：http://oqh.yueranfly.top

const double PI = 3.14159;
来源：http://mha.hfpthk.cn

[S28] C：静态变量
来源：http://lte.sweek.top

static int counter = 0;
来源：http://qkb.daria6918.cn

[S29] C：变参函数
来源：http://yng.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://obz.tanke756.top

[S30] C：头文件保护
来源：http://ade.jinqigufen.top

#ifndef X_H
来源：http://pgb.yonumen.top

#define X_H
来源：http://mly.quarkkingdee.top

#endif
来源：http://oav.yvedp.cn

[S31] C++：Hello World
来源：http://thj.wangshuangyany.cn

#include <iostream>
来源：http://ufd.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://xni.jinqigufen.top

[S32] C++：字符串
来源：http://shg.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://hbk.9152youxi.cn

[S33] C++：vector 增删
来源：http://xce.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jhv.fzhhl.top

[S34] C++：遍历 vector
来源：http://fpg.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://wot.hongshengwenyu.top

[S35] C++：map
来源：http://eyq.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://txc.nanxinkj.top

[S36] C++：unordered_map
来源：http://iba.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ach.yuanzhike.top


<!-- 参考信息 -->