代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tjr.zhixingplan.top

[Q54] 清空表
来源：http://unu.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://boc.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://wjl.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nyf.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://uzk.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dah.yfazqb.com

[Q57] 行号
来源：http://qui.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kep.nanxuanxn.top

[Q58] 累计求和
来源：http://jpl.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vay.snrcjt.cn

[Q59] 分组内累计
来源：http://xes.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://stc.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://qrp.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lsq.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tft.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://dcg.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gea.cqqwz.cn

[Q62] 分组占比
来源：http://fir.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hoj.ydzc1.top

[Q63] 开启事务
来源：http://pim.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://tjm.daxiang520.top

[Q64] 提交事务
来源：http://hsh.hfpthk.cn

COMMIT;
来源：http://vfp.bbcook.cn

[Q65] 回滚事务
来源：http://hsp.shangyingyoupin.top

ROLLBACK;
来源：http://myw.ctjpmb.com

[Q66] 行锁查询
来源：http://ijk.yongpay.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bwx.redwolf501.top

[Q67] 设置隔离级别
来源：http://yye.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mjt.fzhhl.top

[Q68] 保存点
来源：http://awn.bbcook.cn

SAVEPOINT sp1;
来源：http://fvu.nanxinkj.top

ROLLBACK TO sp1;
来源：http://zww.jlsjyb.cn

[Q69] 查看执行计划
来源：http://eoh.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pjv.zdqjudy.top

[Q70] 更新统计信息
来源：http://ghv.jqgufenzy.top

ANALYZE TABLE users;
来源：http://nhs.daria6918.cn

[Q71] 查看建表语句
来源：http://oxu.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://swr.zhijiandao.cn

[Q72] 查看索引
来源：http://man.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://rtt.ydzc1.top

[Q73] 查看表状态
来源：http://wha.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qno.ydzc1.top

[Q74] 强制使用索引
来源：http://ndf.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cpp.nanxinkj.top

[Q75] 日期格式化
来源：http://cqc.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://drb.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eav.gotoacloud.top

[Q76] 按天统计
来源：http://gqe.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ptc.jqgufenzy.top

[Q77] 时间加减
来源：http://zio.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://stl.gogol.net.cn

[Q78] 当前时间
来源：http://oez.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nqf.daxiang520.top

[Q79] 字符串拼接
来源：http://jpj.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xtr.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://dmd.hfpthk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rpe.yj20258.top

[Q81] 字符串替换
来源：http://ugi.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gtu.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://hqr.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urd.fehbvm.com

[Q83] 大小写转换
来源：http://cez.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cwf.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://ate.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://zcx.wangshuangyany.cn

[Q85] 数值取整
来源：http://kwz.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vni.pycfn.com

[Q86] 读取 JSON 字段
来源：http://ypn.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wqa.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://ftj.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyf.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://qho.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqe.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xbd.yj20258.top

[Q89] 判断表是否存在
来源：http://yso.xinyue.icu

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ezg.smart0.xyz

[Q90] 生成序号列
来源：http://fms.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rvv.pycfn.com

================================================================================
来源：http://beu.ywan-chungtsiang.top

R. Bash 专题
来源：http://bpi.sufxvd.cn

================================================================================
来源：http://hxs.andypj.xyz

[R01] shebang 与严格模式
来源：http://ero.zhixingplan.top

#!/usr/bin/env bash
来源：http://hwx.vqdsnc.cn

set -euo pipefail
来源：http://gtd.0kj1m.cn

[R02] 变量赋值与使用
来源：http://xls.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://cmc.hesvh.cn

[R03] 只读变量
来源：http://wps.zhiwuduotai.top

readonly PI=3.14
来源：http://vlt.52xcode.cn

[R04] 位置参数
来源：http://dey.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dbt.ybcxt.top

[R05] 参数默认值
来源：http://wta.yonumen.top

name="${1:-default}"
来源：http://qdu.yj20258888.top

[R06] 判断命令是否存在
来源：http://xqy.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ndt.hesvh.cn

[R07] if 判断文件
来源：http://qja.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nzj.guowangkeji.top

[R08] 数值比较
来源：http://ejv.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mrc.tarul.cn

[R09] 字符串比较
来源：http://bvx.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rmg.zhiwuduotai.top

[R10] 正则匹配
来源：http://jpx.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nwm.shangyingyoupin.top

[R11] case 多分支
来源：http://fjt.jinyuanbaomall.cn

case "$1" in
来源：http://toc.hnqzz.top

start) echo "启动" ;;
来源：http://jdy.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://amk.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://flf.birdmap.top

esac
来源：http://slh.gotoacloud.top

[R12] for 遍历文件
来源：http://mom.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://tvb.snrcjt.cn

[R13] for 计数循环
来源：http://sgc.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://gno.shangyingyoupin.top

[R14] C 风格 for
来源：http://uxy.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://akd.bbcook.cn

[R15] while 逐行读文件
来源：http://cii.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rnh.nwbrower.top

[R16] until 等待条件
来源：http://adj.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://psx.0kj1m.cn

[R17] 数组定义与取值
来源：http://wgl.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rmy.ppjwa.cn

[R18] 遍历数组
来源：http://ddh.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qhi.shangyingyoupin.top

[R19] 数组长度
来源：http://mdz.chenlongwang.top

echo "${#arr[@]}"
来源：http://kyb.ehwqpu.com

[R20] 关联数组（字典）
来源：http://gkf.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bux.gotoacloud.top

[R21] 字符串长度
来源：http://dkq.yj202588.top

echo "${#s}"
来源：http://lbt.gaohongyu789.top

[R22] 截取子串
来源：http://hoq.quarkkingdee.top

echo "${s:0:5}"
来源：http://thx.guowangkeji.top

[R23] 字符串替换
来源：http://whi.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://esw.cashguo.top

[R24] 大小写转换
来源：http://dqm.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cqm.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://cbf.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rfa.dashuyun.cn

[R26] 命令替换
来源：http://hsw.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://rqg.yj202588.top

[R27] 算术展开
来源：http://zuv.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://avb.gaohongyu789.top

[R28] 浮点运算
来源：http://kzq.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://gbj.sysykeji.top

[R29] 定义函数
来源：http://vgy.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kob.mhx1999.top

[R30] 函数返回状态码
来源：http://mux.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://hof.guowangkeji.top

[R31] 局部变量
来源：http://jns.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://ryk.smart0.xyz

[R32] 参数个数校验
来源：http://jlk.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jwl.ivvv.top

[R33] 捕获错误并提示行号
来源：http://trm.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hrm.kuanghao11.cn

[R34] 退出时清理
来源：http://gdq.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://iux.yangfankeji.com

[R35] 后台执行并等待
来源：http://vhl.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gus.hnxiangtu.top

[R36] 并发执行多个任务
来源：http://ksc.uphjek.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://htq.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://eqj.mhx1999.top

files=$(ls -1)
来源：http://xvy.52xcode.cn

[R38] 管道串联
来源：http://jas.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://gcv.birdmap.top

[R39] 重定向标准输出与错误
来源：http://yen.chenzaomai.com

cmd > out.log 2>&1
来源：http://oof.jianghu66.top

[R40] 追加写日志
来源：http://bht.dashuyun.cn

echo "log" >> out.log
来源：http://ukk.ydzc1.top

[R41] 丢弃输出
来源：http://klz.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://ycp.smart0.xyz

[R42] 输入重定向
来源：http://fit.chenzaomai.com

wc -l < a.txt
来源：http://mlc.ivvv.top

[R43] 按名字查找文件
来源：http://zjr.yonumen.top

find . -name "*.log" -type f
来源：http://liw.ctjpmb.com

[R44] 按修改时间查找
来源：http://qrr.aizwys.cn

find . -mtime -7 -type f
来源：http://wvf.pengpengdd.cyou

[R45] 批量删除
来源：http://zhs.pycfn.com

find . -name "*.tmp" -delete
来源：http://zyj.fktsv.cn

[R46] 递归替换文件内容
来源：http://olw.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tsc.kuanghao11.cn

[R47] sed 单行替换
来源：http://eah.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://njj.ybcxt.top

[R48] awk 取指定列
来源：http://vgj.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://tpj.tian-w.cn

[R49] awk 带条件
来源：http://ngq.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yqg.chenlongwang.top

[R50] awk 求和
来源：http://kmh.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://yqm.bjfxy.top

[R51] 排序去重取前几
来源：http://zev.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rdq.fengsongda.top

[R52] 统计行数
来源：http://rhi.hfpthk.cn

wc -l a.txt
来源：http://irm.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://yia.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hgi.fehbvm.com

[R54] 比较两个文件
来源：http://qvs.gaohongyu789.top

diff a.txt b.txt
来源：http://znu.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://kfb.52xcode.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qmc.aibaodan.cn

[R56] 远程拷贝
来源：http://ile.shuidangran.top

scp file user@host:/path/
来源：http://qvw.feifeiyinyue.top

[R57] 远程执行命令
来源：http://yre.yuanzhike.top

ssh user@host 'uptime'
来源：http://nlj.nanxinkj.top

[R58] 下载文件
来源：http://ntb.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xcr.uphjek.com

[R59] 发 POST JSON
来源：http://jtt.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cid.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://ecl.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eqz.ivvv.top

[R61] 磁盘占用
来源：http://lud.cucudq.cn

df -h;  du -sh *
来源：http://rrj.cdnleiting.top

[R62] 找最占空间的文件
来源：http://jtv.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://agl.bbcook.cn

[R63] 内存与进程
来源：http://vvu.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://hjc.nwbrower.top

[R64] 结束进程
来源：http://fqg.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://dwx.wangshuangyany.cn

[R65] 查看端口占用
来源：http://fdm.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hvy.xinyue.icu

[R66] 定时任务
来源：http://mei.tanke756.top

crontab -e;  crontab -l
来源：http://szs.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://nau.xuetiantiany.cn

openssl rand -hex 16
来源：http://wzl.xuanzx.com

[R68] 计算文件校验值
来源：http://ach.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://gnu.sxryk.cn

[R69] 生成随机密码
来源：http://bsj.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://tnb.yvedp.cn

[R70] 时间戳与互转
来源：http://obx.gzhubu.top

date +%s;  date -d @1700000000
来源：http://kyn.aizwys.cn

[R71] 日期格式化
来源：http://dbl.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://agg.shzxlz.cn

[R72] 等待端口就绪
来源：http://hgr.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sar.hesvh.cn

[R73] 分割大日志
来源：http://doz.epnwcf.com

split -l 1000 big.log part_
来源：http://hwx.tianlin.xyz

[R74] 批量重命名
来源：http://faj.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnt.wangdashe.top

[R75] 导出环境变量
来源：http://tou.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://omk.pengpengdd.cyou

[R76] 使用临时文件
来源：http://kjz.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kwm.yanxiufei.cn

[R77] 读取用户输入
来源：http://djh.fktsv.cn

read -rp "请输入: " ans
来源：http://dte.ydjk.org.cn

[R78] 交互式菜单
来源：http://ghi.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fke.ivvv.top

[R79] 解析命令行选项
来源：http://dke.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdm.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://lzj.mhx1999.top

time ./run.sh
来源：http://xrd.ydzc1.top

================================================================================
来源：http://gzk.jqgufenzy.top

S. C / C++ 专题
来源：http://ddw.316326.xyz

================================================================================
来源：http://tpc.bbcook.cn

[S01] C：Hello World
来源：http://zxs.guannengcc.top

#include <stdio.h>
来源：http://bpl.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qrk.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://icz.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://mam.shanyushiyangtech.top

[S03] C：读入整数
来源：http://cpk.havefunace.top

int x; scanf("%d", &x);
来源：http://dvf.havefunace.top

[S04] C：字符串复制
来源：http://dys.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ikq.haohaochexian.top

[S05] C：字符串长度
来源：http://otz.cdnleiting.top

strlen(s)
来源：http://wuz.fehbvm.com

[S06] C：字符串比较
来源：http://uhp.ppjwa.cn

strcmp(a, b) == 0
来源：http://pcn.smart0.xyz

[S07] C：数组遍历求和
来源：http://syz.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hms.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://wru.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exv.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://tdp.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ucp.jyoumei.cn

[S10] C：指针与解引用
来源：http://zwm.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://wkv.ydzc1.top

[S11] C：逐行读文件
来源：http://oyb.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://gpa.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zki.ywan-chungtsiang.top

fclose(f);
来源：http://qtz.tarul.cn

[S12] C：写文件
来源：http://kmy.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tfi.cashguo.top

[S13] C：宏定义
来源：http://obc.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xlt.xylfe.cn

[S14] C：枚举
来源：http://ufh.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://fsy.hesvh.cn

[S15] C：类型转换
来源：http://uur.chenzaomai.com

(double) a / b
来源：http://fzz.redwolf501.top

[S16] C：位操作置位
来源：http://fsw.hammf.cn

x |= (1 << 3);
来源：http://sgn.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://djl.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xvy.ctjpmb.com

[S18] C：命令行参数
来源：http://jxa.jinghuilouyu.cn

int main(int argc, char **argv)
来源：http://bfz.zhoulong.xyz

[S19] C：快速排序
来源：http://uuw.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://uch.zhongyouzk.top

[S20] C：二分查找
来源：http://dco.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vmo.andypj.xyz

[S21] C：字符类别判断
来源：http://mgh.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wwd.xziqi.cn

[S22] C：字符串转数字
来源：http://rdx.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wlj.yuanzhike.top

[S23] C：随机数
来源：http://ycu.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jue.tianlin.xyz

[S24] C：获取本地时间
来源：http://ilt.nanxuanxn.top


<!-- 参考信息 -->