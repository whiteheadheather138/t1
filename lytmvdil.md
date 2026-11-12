代发 wailian999

[Q63] 开启事务
来源：http://bhb.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ufx.cucudq.cn

[Q64] 提交事务
来源：http://oks.redwolf501.top

COMMIT;
来源：http://bsv.tarul.cn

[Q65] 回滚事务
来源：http://usl.0kj1m.cn

ROLLBACK;
来源：http://dln.jyoumei.cn

[Q66] 行锁查询
来源：http://bsb.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qne.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://xhq.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bcp.yj202588.top

[Q68] 保存点
来源：http://vyv.dashuyun.cn

SAVEPOINT sp1;
来源：http://hgy.zdqjudy.top

ROLLBACK TO sp1;
来源：http://zmx.c1oappe.top

[Q69] 查看执行计划
来源：http://vev.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dyw.xuanzx.com

[Q70] 更新统计信息
来源：http://hfx.fktsv.cn

ANALYZE TABLE users;
来源：http://icz.316326.xyz

[Q71] 查看建表语句
来源：http://dgi.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://htp.hesvh.cn

[Q72] 查看索引
来源：http://sgu.snrcjt.cn

SHOW INDEX FROM users;
来源：http://pir.jqgfzy.top

[Q73] 查看表状态
来源：http://oal.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dug.yuanzhike.top

[Q74] 强制使用索引
来源：http://afd.jyoumei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wct.hnxiangtu.top

[Q75] 日期格式化
来源：http://ysb.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jyp.ydjk.org.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hez.wangdashe.top

[Q76] 按天统计
来源：http://ixm.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gew.fzhhl.top

[Q77] 时间加减
来源：http://eno.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fvz.yueranfly.top

[Q78] 当前时间
来源：http://hve.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fqp.birdmap.top

[Q79] 字符串拼接
来源：http://ilc.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://imc.jinyuanbaomall.cn

[Q80] 字符串截取
来源：http://aoj.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://edv.chenjidiqi.icu

[Q81] 字符串替换
来源：http://ugj.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zbk.mhx1999.top

[Q82] 字符长度与字节长度
来源：http://tfq.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://psk.zhiwuduotai.top

[Q83] 大小写转换
来源：http://oph.vqdsnc.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zke.yfazqb.com

[Q84] 去除首尾空格
来源：http://bdo.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://uqd.jqgfzy.top

[Q85] 数值取整
来源：http://gjl.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ksl.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://crn.zhiwuduotai.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vfd.yonumen.top

[Q87] JSON 字段做条件
来源：http://wki.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://twi.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://qmb.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qod.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dag.shuidangran.top

[Q89] 判断表是否存在
来源：http://qql.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ktz.ctjpmb.com

[Q90] 生成序号列
来源：http://oes.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://khl.jinyuanbaomall.cn

================================================================================
来源：http://fwa.daria6918.cn

R. Bash 专题
来源：http://vww.hnqzz.top

================================================================================
来源：http://fty.epnwcf.com

[R01] shebang 与严格模式
来源：http://bis.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://mgu.zhoulong.xyz

set -euo pipefail
来源：http://zwn.yj20258.top

[R02] 变量赋值与使用
来源：http://coc.chenlongwang.top

name="Tom"; echo "$name"
来源：http://xvs.jlsjyb.cn

[R03] 只读变量
来源：http://ypk.birdmap.top

readonly PI=3.14
来源：http://tqd.jlsjyb.cn

[R04] 位置参数
来源：http://mnw.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hjz.cucudq.cn

[R05] 参数默认值
来源：http://moi.kuanghao11.cn

name="${1:-default}"
来源：http://jjx.yonumen.top

[R06] 判断命令是否存在
来源：http://cgf.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vkx.chenlongwang.top

[R07] if 判断文件
来源：http://gjb.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mey.yvedp.cn

[R08] 数值比较
来源：http://wuf.pengpengdd.cyou

if (( a > b )); then echo "a 更大"; fi
来源：http://jxn.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://sev.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ach.ehwqpu.com

[R10] 正则匹配
来源：http://uaf.chenlongwang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uib.fengsongda.top

[R11] case 多分支
来源：http://nle.shangyingyoupin.top

case "$1" in
来源：http://bkj.cashguo.top

start) echo "启动" ;;
来源：http://ons.gogol.net.cn

stop)  echo "停止" ;;
来源：http://oxj.meibo888.top

*)     echo "未知命令" ;;
来源：http://hny.wangshuangyany.cn

esac
来源：http://jnw.xinyue.icu

[R12] for 遍历文件
来源：http://cgy.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://ait.xuetiantiany.cn

[R13] for 计数循环
来源：http://cum.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://jko.fktsv.cn

[R14] C 风格 for
来源：http://eyy.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://isy.jqgfzy.top

[R15] while 逐行读文件
来源：http://bhp.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ilg.jinqigufen.top

[R16] until 等待条件
来源：http://ryf.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://psk.vqdsnc.cn

[R17] 数组定义与取值
来源：http://thx.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://agw.52xcode.cn

[R18] 遍历数组
来源：http://bis.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kvg.cucudq.cn

[R19] 数组长度
来源：http://ezd.hammf.cn

echo "${#arr[@]}"
来源：http://obp.cucudq.cn

[R20] 关联数组（字典）
来源：http://sjs.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bvx.zhijiandao.cn

[R21] 字符串长度
来源：http://ntc.zhongyouzk.top

echo "${#s}"
来源：http://wiw.sxryk.cn

[R22] 截取子串
来源：http://ngw.hesvh.cn

echo "${s:0:5}"
来源：http://iux.xziqi.cn

[R23] 字符串替换
来源：http://clj.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bli.mhx1999.top

[R24] 大小写转换
来源：http://zwb.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://tuv.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://ogo.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://key.gzhubu.top

[R26] 命令替换
来源：http://fgb.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://dze.yuanzhike.top

[R27] 算术展开
来源：http://qqd.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://hyg.smart0.xyz

[R28] 浮点运算
来源：http://umn.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://vhv.pengpengdd.cyou

[R29] 定义函数
来源：http://zdh.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://myc.jlsjyb.cn

[R30] 函数返回状态码
来源：http://fnn.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://hlv.ydjk.org.cn

[R31] 局部变量
来源：http://vln.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://jwp.xuanzx.com

[R32] 参数个数校验
来源：http://epw.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wfg.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://rox.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://amu.52xcode.cn

[R34] 退出时清理
来源：http://fou.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://iwb.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://nqs.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dfp.birdmap.top

[R36] 并发执行多个任务
来源：http://xht.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cue.tanke756.top

[R37] 把输出赋给变量
来源：http://qhp.xylfe.cn

files=$(ls -1)
来源：http://cxk.hongshengwenyu.top

[R38] 管道串联
来源：http://zng.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://bnx.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://zrw.haohaochexian.top

cmd > out.log 2>&1
来源：http://jko.yuanzhike.top

[R40] 追加写日志
来源：http://okg.hnxiangtu.top

echo "log" >> out.log
来源：http://elg.dianchejie.cn

[R41] 丢弃输出
来源：http://bxx.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://gvw.havefunace.top

[R42] 输入重定向
来源：http://llv.tian-w.cn

wc -l < a.txt
来源：http://wgc.tianlin.xyz

[R43] 按名字查找文件
来源：http://iep.hammf.cn

find . -name "*.log" -type f
来源：http://uip.havefunace.top

[R44] 按修改时间查找
来源：http://evo.nanxuanxn.top

find . -mtime -7 -type f
来源：http://qjo.ydjk.org.cn

[R45] 批量删除
来源：http://jot.fengsongda.top

find . -name "*.tmp" -delete
来源：http://wgr.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://gih.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vjz.fengsongda.top

[R47] sed 单行替换
来源：http://lzo.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://sps.bbcook.cn

[R48] awk 取指定列
来源：http://jps.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://bga.aizwys.cn

[R49] awk 带条件
来源：http://tms.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tvi.redwolf501.top

[R50] awk 求和
来源：http://oxn.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qvs.quarkkingdee.top

[R51] 排序去重取前几
来源：http://tux.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vnj.feifeiyinyue.top

[R52] 统计行数
来源：http://shq.yuanzhike.top

wc -l a.txt
来源：http://hep.316326.xyz

[R53] 查看文件头与实时尾
来源：http://wbn.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qel.redwolf501.top

[R54] 比较两个文件
来源：http://mpc.zhengqikj.top

diff a.txt b.txt
来源：http://dpn.ehwqpu.com

[R55] 压缩与解压
来源：http://bne.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fgm.hnxiangtu.top

[R56] 远程拷贝
来源：http://mvj.yuanzhike.top

scp file user@host:/path/
来源：http://umy.iojbl.cn

[R57] 远程执行命令
来源：http://joo.vqdsnc.cn

ssh user@host 'uptime'
来源：http://jyj.zhixingplan.top

[R58] 下载文件
来源：http://xrl.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://esd.jqgfzy.top

[R59] 发 POST JSON
来源：http://bqn.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gye.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://wjm.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dzo.ppjwa.cn

[R61] 磁盘占用
来源：http://fcq.bjfxy.top

df -h;  du -sh *
来源：http://cnr.hnqzz.top

[R62] 找最占空间的文件
来源：http://awq.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://ica.ehwqpu.com

[R63] 内存与进程
来源：http://nqv.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://jwc.hnqzz.top

[R64] 结束进程
来源：http://zoo.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://dlu.yangfankeji.com

[R65] 查看端口占用
来源：http://gcv.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://deb.shanyushiyangkeji.top

[R66] 定时任务
来源：http://pmo.sjlbkw.cn

crontab -e;  crontab -l
来源：http://spe.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://yem.hongshengwenyu.top

openssl rand -hex 16
来源：http://cwo.ivvv.top

[R68] 计算文件校验值
来源：http://cpw.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ydr.zycfv.cn

[R69] 生成随机密码
来源：http://vnv.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://oeq.jinqigfzy.top

[R70] 时间戳与互转
来源：http://kor.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://tot.ivvv.top

[R71] 日期格式化
来源：http://wom.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lnv.chenlongwang.top

[R72] 等待端口就绪
来源：http://mua.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://prk.svipenyu.cn

[R73] 分割大日志
来源：http://wee.yueranfly.top

split -l 1000 big.log part_
来源：http://smo.fktsv.cn

[R74] 批量重命名
来源：http://zkw.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kxd.fengsongda.top

[R75] 导出环境变量
来源：http://kan.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://dfo.nanxuanxn.top

[R76] 使用临时文件
来源：http://eug.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yjo.shuidangran.top

[R77] 读取用户输入
来源：http://oar.jqgufenzy.top

read -rp "请输入: " ans
来源：http://ney.nanxuanxn.top

[R78] 交互式菜单
来源：http://mos.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zxc.aizwys.cn

[R79] 解析命令行选项
来源：http://bwq.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uwf.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://vnj.316326.xyz

time ./run.sh
来源：http://eqj.fengsongda.top

================================================================================
来源：http://ylc.zdqjudy.top

S. C / C++ 专题
来源：http://fjz.yj20258.top

================================================================================
来源：http://pos.mhx1999.top

[S01] C：Hello World
来源：http://abh.iojbl.cn

#include <stdio.h>
来源：http://lmq.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwl.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://pin.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://nth.sufxvd.cn

[S03] C：读入整数
来源：http://lcn.yfazqb.com

int x; scanf("%d", &x);
来源：http://inh.jianghu66.top

[S04] C：字符串复制
来源：http://nsx.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://trm.0kj1m.cn

[S05] C：字符串长度
来源：http://dqj.tianlin.xyz

strlen(s)
来源：http://rks.mhx1999.top

[S06] C：字符串比较
来源：http://wyj.andypj.xyz

strcmp(a, b) == 0
来源：http://wck.xylfe.cn

[S07] C：数组遍历求和
来源：http://ulc.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mha.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://xrj.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nxo.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://vry.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://znc.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://gfb.birdmap.top

int *p = &a;  *p = 5;
来源：http://hhl.sufxvd.cn

[S11] C：逐行读文件
来源：http://tte.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://jca.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vbz.zhaomingkeji.xyz

fclose(f);
来源：http://gmk.dashuyun.cn

[S12] C：写文件
来源：http://ufy.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://udl.ctjpmb.com

[S13] C：宏定义
来源：http://lcu.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vdz.zdbjq.cn

[S14] C：枚举
来源：http://uro.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://qcr.jianghu66.top

[S15] C：类型转换
来源：http://rks.fzhhl.top

(double) a / b
来源：http://lpg.hfpthk.cn

[S16] C：位操作置位
来源：http://dms.ehwqpu.com

x |= (1 << 3);
来源：http://een.316326.xyz

[S17] C：安全拼接字符串
来源：http://tua.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ytx.daxiang520.top

[S18] C：命令行参数
来源：http://zng.cheryme.top

int main(int argc, char **argv)
来源：http://vex.havefunace.top

[S19] C：快速排序
来源：http://eiy.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://bur.yj20258888.top

[S20] C：二分查找
来源：http://oua.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pon.zhijiandao.cn

[S21] C：字符类别判断
来源：http://jke.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://roq.ydzc1.top

[S22] C：字符串转数字
来源：http://tfk.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://wsq.ehwqpu.com

[S23] C：随机数
来源：http://krc.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zle.hnxiangtu.top

[S24] C：获取本地时间
来源：http://giv.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbo.fzhhl.top

[S25] C：内存拷贝
来源：http://wda.sjlbkw.cn

memcpy(dst, src, n);
来源：http://dys.andypj.xyz

[S26] C：内存清零
来源：http://vcd.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://iqa.xuanzx.com

[S27] C：定义常量
来源：http://cjx.zycfv.cn

const double PI = 3.14159;
来源：http://ftq.jiagoushi.top

[S28] C：静态变量
来源：http://ewn.hywenlv.cn

static int counter = 0;
来源：http://gkx.pycfn.com

[S29] C：变参函数
来源：http://xok.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mzt.guowangkeji.top

[S30] C：头文件保护
来源：http://jaa.jiagoushi.top

#ifndef X_H
来源：http://mjk.nanxinkj.top

#define X_H
来源：http://inb.yongpay.top

#endif
来源：http://pev.yj20258.top

[S31] C++：Hello World
来源：http://iwx.wangdashe.top

#include <iostream>
来源：http://luy.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://byq.yueranfly.top

[S32] C++：字符串
来源：http://twx.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://ssm.fehbvm.com


<!-- 参考信息 -->