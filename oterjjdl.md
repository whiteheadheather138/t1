代发 wailian999

[Q63] 开启事务
来源：http://imy.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://tqi.hysaishi.cn

[Q64] 提交事务
来源：http://qwi.mhx1999.top

COMMIT;
来源：http://txv.yuanzhike.top

[Q65] 回滚事务
来源：http://ufo.zhijiandao.cn

ROLLBACK;
来源：http://vjp.nanxinkj.top

[Q66] 行锁查询
来源：http://pxy.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wwq.vehdjk.com

[Q67] 设置隔离级别
来源：http://mzx.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://awa.hammf.cn

[Q68] 保存点
来源：http://xwx.gzhubu.top

SAVEPOINT sp1;
来源：http://mrf.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://knb.quarkkingdee.top

[Q69] 查看执行计划
来源：http://txs.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mpw.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://ctp.zhoulong.xyz

ANALYZE TABLE users;
来源：http://wrf.yangfankeji.com

[Q71] 查看建表语句
来源：http://eaz.bjfxy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qxz.yanxiufei.cn

[Q72] 查看索引
来源：http://cha.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://fyx.meibo888.top

[Q73] 查看表状态
来源：http://fvx.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dvr.chenlongwang.top

[Q74] 强制使用索引
来源：http://ret.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tzh.hesvh.cn

[Q75] 日期格式化
来源：http://qnc.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ykq.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fsj.hesvh.cn

[Q76] 按天统计
来源：http://mda.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://row.cqqwz.cn

[Q77] 时间加减
来源：http://odh.shangyingyoupin.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mqb.jianghu66.top

[Q78] 当前时间
来源：http://imu.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lwo.fehbvm.com

[Q79] 字符串拼接
来源：http://cgo.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ial.cashguo.top

[Q80] 字符串截取
来源：http://crm.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xff.aizwys.cn

[Q81] 字符串替换
来源：http://cuc.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zza.yonumen.top

[Q82] 字符长度与字节长度
来源：http://ouk.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kpe.xinyue.icu

[Q83] 大小写转换
来源：http://aqt.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bax.yfazqb.com

[Q84] 去除首尾空格
来源：http://mol.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://lkk.fanxiaobao.xyz

[Q85] 数值取整
来源：http://obd.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gwp.ivvv.top

[Q86] 读取 JSON 字段
来源：http://uwg.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wml.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://bzj.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mhz.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://tkr.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jty.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oku.zycfv.cn

[Q89] 判断表是否存在
来源：http://liy.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pom.smart0.xyz

[Q90] 生成序号列
来源：http://zpu.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://thc.yuanzhike.top

================================================================================
来源：http://kag.fktsv.cn

R. Bash 专题
来源：http://shn.cheryme.top

================================================================================
来源：http://jiw.jyoumei.cn

[R01] shebang 与严格模式
来源：http://qwp.yangfankeji.com

#!/usr/bin/env bash
来源：http://prk.zhengqikj.top

set -euo pipefail
来源：http://rja.yanxiufei.cn

[R02] 变量赋值与使用
来源：http://eaa.jqgfzy.top

name="Tom"; echo "$name"
来源：http://qrq.hfpthk.cn

[R03] 只读变量
来源：http://zmn.yangfankeji.com

readonly PI=3.14
来源：http://oup.xylfe.cn

[R04] 位置参数
来源：http://irv.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qvu.ywan-chungtsiang.top

[R05] 参数默认值
来源：http://xyp.cqqwz.cn

name="${1:-default}"
来源：http://fbg.ehwqpu.com

[R06] 判断命令是否存在
来源：http://gpw.nanxuanxn.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uub.havefunace.top

[R07] if 判断文件
来源：http://urf.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jbk.shangyingyoupin.top

[R08] 数值比较
来源：http://opa.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vbg.yangfankeji.com

[R09] 字符串比较
来源：http://kba.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://key.xuetiantiany.cn

[R10] 正则匹配
来源：http://ppy.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fxx.52xcode.cn

[R11] case 多分支
来源：http://jdh.havefunace.top

case "$1" in
来源：http://mkr.yanxiufei.cn

start) echo "启动" ;;
来源：http://wxy.fzhhl.top

stop)  echo "停止" ;;
来源：http://cxy.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://atc.tarul.cn

esac
来源：http://gor.uphjek.com

[R12] for 遍历文件
来源：http://bfi.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://wim.vehdjk.com

[R13] for 计数循环
来源：http://vjm.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://hgr.pycfn.com

[R14] C 风格 for
来源：http://dhs.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sda.meibo888.top

[R15] while 逐行读文件
来源：http://wtw.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nzk.uphjek.com

[R16] until 等待条件
来源：http://tnz.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vqp.gogol.net.cn

[R17] 数组定义与取值
来源：http://bay.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://ler.9152youxi.cn

[R18] 遍历数组
来源：http://uqe.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kig.daria6918.cn

[R19] 数组长度
来源：http://nqb.cdnleiting.top

echo "${#arr[@]}"
来源：http://xgt.guowangkeji.top

[R20] 关联数组（字典）
来源：http://xwt.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fro.jinqigfzy.top

[R21] 字符串长度
来源：http://vvf.yuanzhike.top

echo "${#s}"
来源：http://ono.nanxuanxn.top

[R22] 截取子串
来源：http://ukh.chenjidiqi.icu

echo "${s:0:5}"
来源：http://hkt.vqdsnc.cn

[R23] 字符串替换
来源：http://sgp.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wgw.guowangkeji.top

[R24] 大小写转换
来源：http://lsq.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ikz.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://zpu.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpg.ehwqpu.com

[R26] 命令替换
来源：http://jjs.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://tis.kuanghao11.cn

[R27] 算术展开
来源：http://qmq.fehbvm.com

echo $((1 + 2 * 3))
来源：http://rlq.ydzc1.top

[R28] 浮点运算
来源：http://tsi.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://aid.tanke756.top

[R29] 定义函数
来源：http://yku.mhx1999.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ghf.hywenlv.cn

[R30] 函数返回状态码
来源：http://cda.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hja.gzhubu.top

[R31] 局部变量
来源：http://vsc.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://aiq.0kj1m.cn

[R32] 参数个数校验
来源：http://ual.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lys.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://ieq.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fgz.birdmap.top

[R34] 退出时清理
来源：http://fkh.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://pzc.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://mrs.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oef.fanxiaobao.xyz

[R36] 并发执行多个任务
来源：http://mhs.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xlz.tianlin.xyz

[R37] 把输出赋给变量
来源：http://zvr.jlsjyb.cn

files=$(ls -1)
来源：http://rdh.fehbvm.com

[R38] 管道串联
来源：http://nkv.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://nui.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://xdi.9152youxi.cn

cmd > out.log 2>&1
来源：http://igk.jyoumei.cn

[R40] 追加写日志
来源：http://xnh.tian-w.cn

echo "log" >> out.log
来源：http://sox.zhiwuduotai.top

[R41] 丢弃输出
来源：http://aev.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://ccj.cashguo.top

[R42] 输入重定向
来源：http://bcv.ehwqpu.com

wc -l < a.txt
来源：http://ied.zhijiandao.cn

[R43] 按名字查找文件
来源：http://rgx.sysykeji.top

find . -name "*.log" -type f
来源：http://eme.gaohongyu789.top

[R44] 按修改时间查找
来源：http://mof.ppjwa.cn

find . -mtime -7 -type f
来源：http://kiw.gaohongyu789.top

[R45] 批量删除
来源：http://cdo.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://wwq.sweek.top

[R46] 递归替换文件内容
来源：http://cir.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://szq.zhoulong.xyz

[R47] sed 单行替换
来源：http://bxf.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vxv.mhx1999.top

[R48] awk 取指定列
来源：http://ign.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://irl.xuanzx.com

[R49] awk 带条件
来源：http://ohk.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bjr.mhx1999.top

[R50] awk 求和
来源：http://dmg.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://loc.aizwys.cn

[R51] 排序去重取前几
来源：http://hpc.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ykx.shuidangran.top

[R52] 统计行数
来源：http://jzp.dianchejie.cn

wc -l a.txt
来源：http://bbi.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://kjj.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zvn.dianchejie.cn

[R54] 比较两个文件
来源：http://fdv.ivvv.top

diff a.txt b.txt
来源：http://ufv.jianghu66.top

[R55] 压缩与解压
来源：http://oni.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://opw.hammf.cn

[R56] 远程拷贝
来源：http://tgx.xinyue.icu

scp file user@host:/path/
来源：http://tsx.jqgfzy.top

[R57] 远程执行命令
来源：http://kbb.ydjk.org.cn

ssh user@host 'uptime'
来源：http://rbi.cheryme.top

[R58] 下载文件
来源：http://qhw.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rge.vehdjk.com

[R59] 发 POST JSON
来源：http://klj.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fhw.yuanzhike.top

[R60] 只看 HTTP 状态码
来源：http://ire.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wmc.meibo888.top

[R61] 磁盘占用
来源：http://exs.jqgfzy.top

df -h;  du -sh *
来源：http://ctk.iojbl.cn

[R62] 找最占空间的文件
来源：http://ekl.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://nqn.daxiang520.top

[R63] 内存与进程
来源：http://hsk.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://ayo.tianlin.xyz

[R64] 结束进程
来源：http://bwl.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://flm.hysaishi.cn

[R65] 查看端口占用
来源：http://bbq.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kag.yanxiufei.cn

[R66] 定时任务
来源：http://wnx.jiagoushi.top

crontab -e;  crontab -l
来源：http://luh.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://mmn.shuidangran.top

openssl rand -hex 16
来源：http://uhr.yueranfly.top

[R68] 计算文件校验值
来源：http://lah.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://rln.yvedp.cn

[R69] 生成随机密码
来源：http://cov.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://nub.yanxiufei.cn

[R70] 时间戳与互转
来源：http://cgt.sweek.top

date +%s;  date -d @1700000000
来源：http://goa.hammf.cn

[R71] 日期格式化
来源：http://kky.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cby.cqqwz.cn

[R72] 等待端口就绪
来源：http://lmv.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vnt.yj20258888.top

[R73] 分割大日志
来源：http://gkd.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://qdu.fengsongda.top

[R74] 批量重命名
来源：http://obj.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mzh.bbcook.cn

[R75] 导出环境变量
来源：http://ysi.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://gbh.yuanzhike.top

[R76] 使用临时文件
来源：http://dfj.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pjh.cucudq.cn

[R77] 读取用户输入
来源：http://lof.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://lww.yanxiufei.cn

[R78] 交互式菜单
来源：http://cdi.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dfl.ppjwa.cn

[R79] 解析命令行选项
来源：http://jzj.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yye.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://jxm.fanxiaobao.xyz

time ./run.sh
来源：http://gqr.tian-w.cn

================================================================================
来源：http://sxt.yuxming.cn

S. C / C++ 专题
来源：http://pxh.xuetiantiany.cn

================================================================================
来源：http://wjy.wangdashe.top

[S01] C：Hello World
来源：http://jth.hnxiangtu.top

#include <stdio.h>
来源：http://rqv.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uez.cheryme.top

[S02] C：变量与格式化输出
来源：http://xwn.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://dlo.pycfn.com

[S03] C：读入整数
来源：http://lve.fzhhl.top

int x; scanf("%d", &x);
来源：http://mqe.fzhhl.top

[S04] C：字符串复制
来源：http://gpn.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://xny.yonumen.top

[S05] C：字符串长度
来源：http://gkc.havefunace.top

strlen(s)
来源：http://srx.svipenyu.cn

[S06] C：字符串比较
来源：http://pxf.meibo888.top

strcmp(a, b) == 0
来源：http://igq.cdnleiting.top

[S07] C：数组遍历求和
来源：http://cab.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nhz.tanke756.top

[S08] C：动态内存分配与释放
来源：http://clg.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jbp.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://kzp.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://woe.hywenlv.cn

[S10] C：指针与解引用
来源：http://cit.xuanzx.com

int *p = &a;  *p = 5;
来源：http://epj.haohaochexian.top

[S11] C：逐行读文件
来源：http://atp.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://enx.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aph.xinyue.icu

fclose(f);
来源：http://rsz.jinghuilouyu.cn

[S12] C：写文件
来源：http://jlx.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqt.jianghu66.top

[S13] C：宏定义
来源：http://efy.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uhg.vehdjk.com

[S14] C：枚举
来源：http://taf.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://jkh.zhengqikj.top

[S15] C：类型转换
来源：http://hyn.xuanzx.com

(double) a / b
来源：http://qrg.ehwqpu.com

[S16] C：位操作置位
来源：http://umt.bjfxy.top

x |= (1 << 3);
来源：http://xpn.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://ape.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wpp.chenzaomai.com

[S18] C：命令行参数
来源：http://zjj.fengsongda.top

int main(int argc, char **argv)
来源：http://msz.guannengcc.top

[S19] C：快速排序
来源：http://hdj.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://odl.52xcode.cn

[S20] C：二分查找
来源：http://ybz.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kzn.hcnkem.com

[S21] C：字符类别判断
来源：http://qsi.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rby.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://iah.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jph.yfazqb.com

[S23] C：随机数
来源：http://pql.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fdl.jqgufenzy.top

[S24] C：获取本地时间
来源：http://rkq.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oty.nanxinkj.top

[S25] C：内存拷贝
来源：http://cbv.snrcjt.cn

memcpy(dst, src, n);
来源：http://nnx.hywenlv.cn

[S26] C：内存清零
来源：http://qro.fehbvm.com

memset(a, 0, sizeof a);
来源：http://gyv.yj202588.top

[S27] C：定义常量
来源：http://lei.fktsv.cn

const double PI = 3.14159;
来源：http://zye.sysykeji.top

[S28] C：静态变量
来源：http://dvc.9152youxi.cn

static int counter = 0;
来源：http://ukb.ydjk.org.cn

[S29] C：变参函数
来源：http://nqv.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxc.jyoumei.cn

[S30] C：头文件保护
来源：http://fvg.zhoulong.xyz

#ifndef X_H
来源：http://cij.shuidangran.top

#define X_H
来源：http://iwh.xziqi.cn

#endif
来源：http://emp.ydjk.org.cn

[S31] C++：Hello World
来源：http://szh.zdqjudy.top

#include <iostream>
来源：http://law.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://sro.ivvv.top

[S32] C++：字符串
来源：http://xcc.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://xcg.ivvv.top


<!-- 参考信息 -->