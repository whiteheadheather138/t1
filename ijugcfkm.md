代发 wailian999

[Q65] 回滚事务
来源：http://ykm.ybcxt.top

ROLLBACK;
来源：http://cer.pycfn.com

[Q66] 行锁查询
来源：http://aje.hammf.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zlb.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://yuh.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mpk.aizwys.cn

[Q68] 保存点
来源：http://ewr.meibo888.top

SAVEPOINT sp1;
来源：http://bgk.c1oappe.top

ROLLBACK TO sp1;
来源：http://cro.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://rxc.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zth.havefunace.top

[Q70] 更新统计信息
来源：http://wgz.dianchejie.cn

ANALYZE TABLE users;
来源：http://khz.yanxiufei.cn

[Q71] 查看建表语句
来源：http://nzc.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jim.ppjwa.cn

[Q72] 查看索引
来源：http://oyi.tian-w.cn

SHOW INDEX FROM users;
来源：http://yla.andypj.xyz

[Q73] 查看表状态
来源：http://eqo.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ldo.zhiwuduotai.top

[Q74] 强制使用索引
来源：http://loo.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lkw.jqgfzy.top

[Q75] 日期格式化
来源：http://aws.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qjf.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dfm.xylfe.cn

[Q76] 按天统计
来源：http://acq.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uwk.chenjidiqi.icu

[Q77] 时间加减
来源：http://rkf.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kcs.tarul.cn

[Q78] 当前时间
来源：http://qay.yueranfly.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://psx.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://oty.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lfx.jqgufenzy.top

[Q80] 字符串截取
来源：http://bns.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cat.sjlbkw.cn

[Q81] 字符串替换
来源：http://zbu.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rcz.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://uww.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nay.bjfxy.top

[Q83] 大小写转换
来源：http://bzc.hnxiangtu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hsl.mhx1999.top

[Q84] 去除首尾空格
来源：http://orl.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://tfo.xinyue.icu

[Q85] 数值取整
来源：http://mmm.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cwl.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://tvn.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qfz.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://elr.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://daa.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://qun.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oym.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hzi.cucudq.cn

[Q89] 判断表是否存在
来源：http://lnu.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ypr.svipenyu.cn

[Q90] 生成序号列
来源：http://ykj.aibaodan.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uzq.tanke756.top

================================================================================
来源：http://adc.yueranfly.top

R. Bash 专题
来源：http://wka.xuetiantiany.cn

================================================================================
来源：http://zce.tianlin.xyz

[R01] shebang 与严格模式
来源：http://kqa.vehdjk.com

#!/usr/bin/env bash
来源：http://ian.gzhubu.top

set -euo pipefail
来源：http://dkg.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://aco.ctjpmb.com

name="Tom"; echo "$name"
来源：http://whc.hnxiangtu.top

[R03] 只读变量
来源：http://cbw.xinyue.icu

readonly PI=3.14
来源：http://clz.hammf.cn

[R04] 位置参数
来源：http://bxo.snrcjt.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://atk.zdbjq.cn

[R05] 参数默认值
来源：http://wkp.xinyue.icu

name="${1:-default}"
来源：http://jzk.gzhubu.top

[R06] 判断命令是否存在
来源：http://ayx.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nne.wangshuangyany.cn

[R07] if 判断文件
来源：http://sfg.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://edd.gogol.net.cn

[R08] 数值比较
来源：http://fsf.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zsn.jinqigufen.top

[R09] 字符串比较
来源：http://wih.yj20258.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lpw.ehwqpu.com

[R10] 正则匹配
来源：http://abl.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hdr.hysaishi.cn

[R11] case 多分支
来源：http://row.jinqigfzy.top

case "$1" in
来源：http://keb.ivvv.top

start) echo "启动" ;;
来源：http://ljo.c1oappe.top

stop)  echo "停止" ;;
来源：http://ymd.havefunace.top

*)     echo "未知命令" ;;
来源：http://qny.vqdsnc.cn

esac
来源：http://fcc.guannengcc.top

[R12] for 遍历文件
来源：http://ifp.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://hzj.nanxinkj.top

[R13] for 计数循环
来源：http://itt.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://ckf.hywenlv.cn

[R14] C 风格 for
来源：http://ovt.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fqx.xylfe.cn

[R15] while 逐行读文件
来源：http://ogx.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://weh.hysaishi.cn

[R16] until 等待条件
来源：http://els.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zwl.hnxiangtu.top

[R17] 数组定义与取值
来源：http://elt.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://hvz.cdnleiting.top

[R18] 遍历数组
来源：http://xvl.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mgo.zhijiandao.cn

[R19] 数组长度
来源：http://fuf.gaohongyu789.top

echo "${#arr[@]}"
来源：http://xad.zhongyouzk.top

[R20] 关联数组（字典）
来源：http://uax.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yif.yfazqb.com

[R21] 字符串长度
来源：http://kev.haohaochexian.top

echo "${#s}"
来源：http://yfj.chenzaomai.com

[R22] 截取子串
来源：http://sry.tianlin.xyz

echo "${s:0:5}"
来源：http://uzu.yangfankeji.com

[R23] 字符串替换
来源：http://olk.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yzx.ybcxt.top

[R24] 大小写转换
来源：http://xdq.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ggy.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://pal.wangdashe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zfp.shuidangran.top

[R26] 命令替换
来源：http://qfa.cheryme.top

now=$(date +%F); echo "$now"
来源：http://jyo.yangfankeji.com

[R27] 算术展开
来源：http://xrl.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://evk.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://xix.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://tvz.iojbl.cn

[R29] 定义函数
来源：http://zms.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ysy.hnqzz.top

[R30] 函数返回状态码
来源：http://kmi.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://bwx.jinyuanbaomall.cn

[R31] 局部变量
来源：http://xog.dashuyun.cn

f() { local x=1; echo "$x"; }
来源：http://wef.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://ztv.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cfc.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://sfs.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qel.shuidangran.top

[R34] 退出时清理
来源：http://pry.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wee.bbcook.cn

[R35] 后台执行并等待
来源：http://gjk.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://bvy.nanxinkj.top

[R36] 并发执行多个任务
来源：http://fdl.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tcd.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://xkv.yonumen.top

files=$(ls -1)
来源：http://ffi.aibaodan.cn

[R38] 管道串联
来源：http://nad.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://wct.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://whr.havefunace.top

cmd > out.log 2>&1
来源：http://xlv.ivvv.top

[R40] 追加写日志
来源：http://evv.ydzc1.top

echo "log" >> out.log
来源：http://nqk.xuanzx.com

[R41] 丢弃输出
来源：http://mzf.wangdashe.top

cmd >/dev/null 2>&1
来源：http://myd.zhengqikj.top

[R42] 输入重定向
来源：http://bij.tarul.cn

wc -l < a.txt
来源：http://rzg.jianghu66.top

[R43] 按名字查找文件
来源：http://baw.zdbjq.cn

find . -name "*.log" -type f
来源：http://pdr.epnwcf.com

[R44] 按修改时间查找
来源：http://npx.ivvv.top

find . -mtime -7 -type f
来源：http://qur.nanxinkj.top

[R45] 批量删除
来源：http://ryu.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://bjb.snrcjt.cn

[R46] 递归替换文件内容
来源：http://dkj.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://izd.fengsongda.top

[R47] sed 单行替换
来源：http://bzv.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oir.cheryme.top

[R48] awk 取指定列
来源：http://cdh.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://fpc.svipenyu.cn

[R49] awk 带条件
来源：http://wrf.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fzl.hnxiangtu.top

[R50] awk 求和
来源：http://myf.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://hyf.jlsjyb.cn

[R51] 排序去重取前几
来源：http://nbk.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lpd.hongshengwenyu.top

[R52] 统计行数
来源：http://lqy.snrcjt.cn

wc -l a.txt
来源：http://qkz.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://ddb.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://opu.cdnleiting.top

[R54] 比较两个文件
来源：http://ofq.zdqjudy.top

diff a.txt b.txt
来源：http://qnc.aibaodan.cn

[R55] 压缩与解压
来源：http://oiz.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xkm.gotoacloud.top

[R56] 远程拷贝
来源：http://bqn.vqdsnc.cn

scp file user@host:/path/
来源：http://qsw.gotoacloud.top

[R57] 远程执行命令
来源：http://nmb.zhaomingkeji.xyz

ssh user@host 'uptime'
来源：http://hjo.ctjpmb.com

[R58] 下载文件
来源：http://plm.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mck.sweek.top

[R59] 发 POST JSON
来源：http://mhk.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bjw.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://sbv.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wqz.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://onf.yuxming.cn

df -h;  du -sh *
来源：http://mkh.daxiang520.top

[R62] 找最占空间的文件
来源：http://ttf.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://kpm.hfpthk.cn

[R63] 内存与进程
来源：http://azq.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://pbm.ybcxt.top

[R64] 结束进程
来源：http://ziy.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://vsr.hongshengwenyu.top

[R65] 查看端口占用
来源：http://qkm.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ezw.chenlongwang.top

[R66] 定时任务
来源：http://wtg.sjlbkw.cn

crontab -e;  crontab -l
来源：http://hub.wangdashe.top

[R67] 生成随机十六进制串
来源：http://wge.shanyushiyangtech.top

openssl rand -hex 16
来源：http://qrp.hnqzz.top

[R68] 计算文件校验值
来源：http://hhq.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://vmv.hnqzz.top

[R69] 生成随机密码
来源：http://lbb.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://yci.tian-w.cn

[R70] 时间戳与互转
来源：http://szk.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://ljs.zhixingplan.top

[R71] 日期格式化
来源：http://ujr.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://egq.sxryk.cn

[R72] 等待端口就绪
来源：http://nkl.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tns.meibo888.top

[R73] 分割大日志
来源：http://itu.yonumen.top

split -l 1000 big.log part_
来源：http://sxd.bjfxy.top

[R74] 批量重命名
来源：http://umd.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://syg.dianchejie.cn

[R75] 导出环境变量
来源：http://puv.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://eeo.wangdashe.top

[R76] 使用临时文件
来源：http://wml.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zqx.jqgufenzy.top

[R77] 读取用户输入
来源：http://ruy.sjlbkw.cn

read -rp "请输入: " ans
来源：http://rnu.sweek.top

[R78] 交互式菜单
来源：http://ywn.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mii.smart0.xyz

[R79] 解析命令行选项
来源：http://hty.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eog.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://uor.fengsongda.top

time ./run.sh
来源：http://vtg.wangdashe.top

================================================================================
来源：http://xib.xziqi.cn

S. C / C++ 专题
来源：http://mqx.sjlbkw.cn

================================================================================
来源：http://pnj.epnwcf.com

[S01] C：Hello World
来源：http://xfx.dashuyun.cn

#include <stdio.h>
来源：http://fin.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hze.fengsongda.top

[S02] C：变量与格式化输出
来源：http://bcz.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://wna.hammf.cn

[S03] C：读入整数
来源：http://ovj.chenlongwang.top

int x; scanf("%d", &x);
来源：http://qni.chenlongwang.top

[S04] C：字符串复制
来源：http://fot.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://vmp.hesvh.cn

[S05] C：字符串长度
来源：http://qhm.zhoulong.xyz

strlen(s)
来源：http://hof.daxiang520.top

[S06] C：字符串比较
来源：http://ifu.cucudq.cn

strcmp(a, b) == 0
来源：http://tmp.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://btg.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tyb.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://sbb.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wvw.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://wwm.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://val.tian-w.cn

[S10] C：指针与解引用
来源：http://gsw.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://bkz.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://sff.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://tpx.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hwp.hesvh.cn

fclose(f);
来源：http://gdf.cqqwz.cn

[S12] C：写文件
来源：http://kdt.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kca.birdmap.top

[S13] C：宏定义
来源：http://yyc.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://owu.yvedp.cn

[S14] C：枚举
来源：http://ahq.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://tsv.yanxiufei.cn

[S15] C：类型转换
来源：http://sco.hesvh.cn

(double) a / b
来源：http://ggh.zhixingplan.top

[S16] C：位操作置位
来源：http://gcm.tanke756.top

x |= (1 << 3);
来源：http://aiw.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://vfw.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hea.ppjwa.cn

[S18] C：命令行参数
来源：http://mhu.gaohongyu789.top

int main(int argc, char **argv)
来源：http://yar.zhoulong.xyz

[S19] C：快速排序
来源：http://mfi.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://uuh.zhijiandao.cn

[S20] C：二分查找
来源：http://dxo.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rfx.sufxvd.cn

[S21] C：字符类别判断
来源：http://yeg.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://but.sjlbkw.cn

[S22] C：字符串转数字
来源：http://ehl.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://hiq.cucudq.cn

[S23] C：随机数
来源：http://quf.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptf.zhoulong.xyz

[S24] C：获取本地时间
来源：http://zvi.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dfy.chenzaomai.com

[S25] C：内存拷贝
来源：http://lsq.cqqwz.cn

memcpy(dst, src, n);
来源：http://spw.smart0.xyz

[S26] C：内存清零
来源：http://got.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://jcd.shzxlz.cn

[S27] C：定义常量
来源：http://hny.tianlin.xyz

const double PI = 3.14159;
来源：http://sgh.iojbl.cn

[S28] C：静态变量
来源：http://vlt.yanxiufei.cn

static int counter = 0;
来源：http://fkr.9152youxi.cn

[S29] C：变参函数
来源：http://hip.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wuh.hammf.cn

[S30] C：头文件保护
来源：http://nks.snrcjt.cn

#ifndef X_H
来源：http://oku.jinghuilouyu.cn

#define X_H
来源：http://duu.hcnkem.com

#endif
来源：http://wom.svipenyu.cn

[S31] C++：Hello World
来源：http://rlk.yuanzhike.top

#include <iostream>
来源：http://hni.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://spd.vehdjk.com

[S32] C++：字符串
来源：http://ndz.meibo888.top

std::string s = "hi";  s += "!";
来源：http://kbe.guannengcc.top

[S33] C++：vector 增删
来源：http://kis.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oum.tanke756.top

[S34] C++：遍历 vector
来源：http://oca.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://sev.hywenlv.cn


<!-- 参考信息 -->