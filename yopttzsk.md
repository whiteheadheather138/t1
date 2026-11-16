代发 wailian999

[Q48] CTE 公用表表达式
来源：http://lyp.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ruh.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://vek.chenjidiqi.icu

[Q49] 更新单行
来源：http://ncr.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wtg.sufxvd.cn

[Q50] 批量更新
来源：http://lag.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://inv.tanke756.top

[Q51] 用子查询更新
来源：http://zgo.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npy.zhengqikj.top

[Q52] 删除指定行
来源：http://ltt.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://sib.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://lmh.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yhd.daxiang520.top

[Q54] 清空表
来源：http://rkv.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://uxh.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://ntb.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qwz.kuanghao11.cn

[Q56] 密集排名（并列不占位）
来源：http://egb.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ygy.cheryme.top

[Q57] 行号
来源：http://xkv.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eku.ppjwa.cn

[Q58] 累计求和
来源：http://mws.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://stn.vehdjk.com

[Q59] 分组内累计
来源：http://tyz.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://azq.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://wqs.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://thb.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fkq.yongpay.top

[Q61] 移动平均
来源：http://bzb.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yzi.nanxuanxn.top

[Q62] 分组占比
来源：http://oru.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ctu.fktsv.cn

[Q63] 开启事务
来源：http://kfi.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zqb.gzhubu.top

[Q64] 提交事务
来源：http://ewc.jinghuilouyu.cn

COMMIT;
来源：http://zru.xinyue.icu

[Q65] 回滚事务
来源：http://efg.jyoumei.cn

ROLLBACK;
来源：http://hcy.hysaishi.cn

[Q66] 行锁查询
来源：http://hus.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oaf.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://jze.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://duy.sxryk.cn

[Q68] 保存点
来源：http://kry.smart0.xyz

SAVEPOINT sp1;
来源：http://jok.shzxlz.cn

ROLLBACK TO sp1;
来源：http://aun.gogol.net.cn

[Q69] 查看执行计划
来源：http://aaf.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wlm.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://nez.chenlongwang.top

ANALYZE TABLE users;
来源：http://gil.yanxiufei.cn

[Q71] 查看建表语句
来源：http://vac.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nwu.jiagoushi.top

[Q72] 查看索引
来源：http://suh.daria6918.cn

SHOW INDEX FROM users;
来源：http://ifg.yueranfly.top

[Q73] 查看表状态
来源：http://yzl.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://abt.vqdsnc.cn

[Q74] 强制使用索引
来源：http://ghw.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hwh.meibo888.top

[Q75] 日期格式化
来源：http://cip.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yix.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://san.zhijiandao.cn

[Q76] 按天统计
来源：http://mbk.zhoulong.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfo.zhixingplan.top

[Q77] 时间加减
来源：http://gji.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xbu.zhijiandao.cn

[Q78] 当前时间
来源：http://lql.bjfxy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hwx.wangdashe.top

[Q79] 字符串拼接
来源：http://ahe.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yoh.pycfn.com

[Q80] 字符串截取
来源：http://ibc.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kei.0kj1m.cn

[Q81] 字符串替换
来源：http://frv.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zna.cheryme.top

[Q82] 字符长度与字节长度
来源：http://yjn.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://apx.ydzc1.top

[Q83] 大小写转换
来源：http://vcs.bjfxy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wct.sysykeji.top

[Q84] 去除首尾空格
来源：http://yrx.xinyue.icu

SELECT TRIM(name) FROM users;
来源：http://uvc.aizwys.cn

[Q85] 数值取整
来源：http://slo.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kxw.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://kab.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rvh.pycfn.com

[Q87] JSON 字段做条件
来源：http://jom.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pij.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://fqf.zhengqikj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fkx.yj20258888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ecc.guannengcc.top

[Q89] 判断表是否存在
来源：http://tzp.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xzu.nanxuanxn.top

[Q90] 生成序号列
来源：http://qhc.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ira.yueranfly.top

================================================================================
来源：http://pnx.guannengcc.top

R. Bash 专题
来源：http://znc.yj20258888.top

================================================================================
来源：http://yxa.yfazqb.com

[R01] shebang 与严格模式
来源：http://qva.xinyue.icu

#!/usr/bin/env bash
来源：http://lly.sjlbkw.cn

set -euo pipefail
来源：http://nwp.sjlbkw.cn

[R02] 变量赋值与使用
来源：http://jzi.fehbvm.com

name="Tom"; echo "$name"
来源：http://rpc.hfpthk.cn

[R03] 只读变量
来源：http://hyi.xinyue.icu

readonly PI=3.14
来源：http://xyc.chenjidiqi.icu

[R04] 位置参数
来源：http://kwt.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://itf.fengsongda.top

[R05] 参数默认值
来源：http://stk.zhengqikj.top

name="${1:-default}"
来源：http://guz.yuanzhike.top

[R06] 判断命令是否存在
来源：http://wzz.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mwy.aibaodan.cn

[R07] if 判断文件
来源：http://ivl.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xff.yongpay.top

[R08] 数值比较
来源：http://qvq.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vhk.shangyingyoupin.top

[R09] 字符串比较
来源：http://jnm.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vyl.pengpengdd.cyou

[R10] 正则匹配
来源：http://wgy.xinyue.icu

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nqx.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://xux.ybcxt.top

case "$1" in
来源：http://shn.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://evy.316326.xyz

stop)  echo "停止" ;;
来源：http://udi.fzhhl.top

*)     echo "未知命令" ;;
来源：http://isv.uphjek.com

esac
来源：http://lop.chenzaomai.com

[R12] for 遍历文件
来源：http://qvy.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://qnx.jinqigfzy.top

[R13] for 计数循环
来源：http://irh.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://pla.gzhubu.top

[R14] C 风格 for
来源：http://ewe.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qxg.xziqi.cn

[R15] while 逐行读文件
来源：http://nvu.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tfv.nanxinkj.top

[R16] until 等待条件
来源：http://fdr.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cpl.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://oea.hongshengwenyu.top

arr=(a b c); echo "${arr[0]}"
来源：http://fze.daxiang520.top

[R18] 遍历数组
来源：http://pkk.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tmk.jinqigfzy.top

[R19] 数组长度
来源：http://elt.smart0.xyz

echo "${#arr[@]}"
来源：http://jvj.hywenlv.cn

[R20] 关联数组（字典）
来源：http://ycs.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wjo.meibo888.top

[R21] 字符串长度
来源：http://twn.0kj1m.cn

echo "${#s}"
来源：http://vdr.hammf.cn

[R22] 截取子串
来源：http://jod.jqgufenzy.top

echo "${s:0:5}"
来源：http://kvj.jyoumei.cn

[R23] 字符串替换
来源：http://ddu.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gnt.fktsv.cn

[R24] 大小写转换
来源：http://kni.pengpengdd.cyou

echo "${s^^}"; echo "${s,,}"
来源：http://sto.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://fop.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iun.epnwcf.com

[R26] 命令替换
来源：http://wih.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://xkw.svipenyu.cn

[R27] 算术展开
来源：http://eha.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://fgm.havefunace.top

[R28] 浮点运算
来源：http://puw.pycfn.com

echo "scale=2; 10/3" | bc
来源：http://oft.zhengqikj.top

[R29] 定义函数
来源：http://rfk.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ezb.andypj.xyz

[R30] 函数返回状态码
来源：http://wqo.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://zxv.jyoumei.cn

[R31] 局部变量
来源：http://pmx.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://opn.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://umn.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vbx.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://msu.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://brp.tarul.cn

[R34] 退出时清理
来源：http://izz.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://zho.guowangkeji.top

[R35] 后台执行并等待
来源：http://wqa.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fmc.guowangkeji.top

[R36] 并发执行多个任务
来源：http://elg.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pvj.hnqzz.top

[R37] 把输出赋给变量
来源：http://qxo.svipenyu.cn

files=$(ls -1)
来源：http://vfj.0kj1m.cn

[R38] 管道串联
来源：http://zdf.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://alo.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://cpt.ydzc1.top

cmd > out.log 2>&1
来源：http://csm.jqgfzy.top

[R40] 追加写日志
来源：http://myq.jinqigfzy.top

echo "log" >> out.log
来源：http://vlc.sweek.top

[R41] 丢弃输出
来源：http://goj.zhengqikj.top

cmd >/dev/null 2>&1
来源：http://amq.aizwys.cn

[R42] 输入重定向
来源：http://joc.mhx1999.top

wc -l < a.txt
来源：http://jjr.tianlin.xyz

[R43] 按名字查找文件
来源：http://hvk.aibaodan.cn

find . -name "*.log" -type f
来源：http://pfe.vehdjk.com

[R44] 按修改时间查找
来源：http://rsc.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://xav.fehbvm.com

[R45] 批量删除
来源：http://ajz.sxryk.cn

find . -name "*.tmp" -delete
来源：http://ooi.daxiang520.top

[R46] 递归替换文件内容
来源：http://tcq.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yqn.zhixingplan.top

[R47] sed 单行替换
来源：http://lka.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jep.iojbl.cn

[R48] awk 取指定列
来源：http://crj.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://rej.jqgfzy.top

[R49] awk 带条件
来源：http://ynk.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fwa.shzxlz.cn

[R50] awk 求和
来源：http://pem.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://bkl.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://pyl.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mwu.vehdjk.com

[R52] 统计行数
来源：http://gth.ppjwa.cn

wc -l a.txt
来源：http://oem.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://qlz.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tvp.birdmap.top

[R54] 比较两个文件
来源：http://koz.yj202588.top

diff a.txt b.txt
来源：http://vat.zdqjudy.top

[R55] 压缩与解压
来源：http://csz.hcnkem.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bbj.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://bpp.daria6918.cn

scp file user@host:/path/
来源：http://fxu.zhongyouzk.top

[R57] 远程执行命令
来源：http://oil.redwolf501.top

ssh user@host 'uptime'
来源：http://vmc.hcnkem.com

[R58] 下载文件
来源：http://isn.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sng.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://hhb.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ghy.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://vpl.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uhr.nanxuanxn.top

[R61] 磁盘占用
来源：http://uyx.jqgufenzy.top

df -h;  du -sh *
来源：http://sfh.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://cnl.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://frp.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://doi.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://eiu.shanyushiyangtech.top

[R64] 结束进程
来源：http://zmh.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://czt.sjlbkw.cn

[R65] 查看端口占用
来源：http://lcx.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ved.zhixingplan.top

[R66] 定时任务
来源：http://lox.epnwcf.com

crontab -e;  crontab -l
来源：http://zjt.hcnkem.com

[R67] 生成随机十六进制串
来源：http://imb.mhx1999.top

openssl rand -hex 16
来源：http://sji.guowangkeji.top

[R68] 计算文件校验值
来源：http://ldq.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://zpo.sysykeji.top

[R69] 生成随机密码
来源：http://eyh.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://uog.guowangkeji.top

[R70] 时间戳与互转
来源：http://lqo.epnwcf.com

date +%s;  date -d @1700000000
来源：http://cqp.yj20258888.top

[R71] 日期格式化
来源：http://hxw.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ldj.xuanzx.com

[R72] 等待端口就绪
来源：http://oww.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gcw.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://cti.0kj1m.cn

split -l 1000 big.log part_
来源：http://bxz.shangyingyoupin.top

[R74] 批量重命名
来源：http://ftg.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xhi.ctjpmb.com

[R75] 导出环境变量
来源：http://qvm.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://wwx.shuidangran.top

[R76] 使用临时文件
来源：http://bav.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://udg.iojbl.cn

[R77] 读取用户输入
来源：http://mks.chenlongwang.top

read -rp "请输入: " ans
来源：http://ote.wangdashe.top

[R78] 交互式菜单
来源：http://xve.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qke.zhoulong.xyz

[R79] 解析命令行选项
来源：http://lmo.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fut.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://hia.cashguo.top

time ./run.sh
来源：http://scl.meibo888.top

================================================================================
来源：http://dku.snrcjt.cn

S. C / C++ 专题
来源：http://cdd.xylfe.cn

================================================================================
来源：http://uxh.zhoulong.xyz

[S01] C：Hello World
来源：http://nqd.bjfxy.top

#include <stdio.h>
来源：http://gci.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmz.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://gfs.nanxuanxn.top

int a = 10; printf("%d\n", a);
来源：http://rtv.tian-w.cn

[S03] C：读入整数
来源：http://nkj.hywenlv.cn

int x; scanf("%d", &x);
来源：http://txo.shzxlz.cn

[S04] C：字符串复制
来源：http://srw.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://drb.snrcjt.cn

[S05] C：字符串长度
来源：http://avm.xylfe.cn

strlen(s)
来源：http://afo.xuanzx.com

[S06] C：字符串比较
来源：http://oov.uphjek.com

strcmp(a, b) == 0
来源：http://jsk.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://mnt.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dlf.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://ihq.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wte.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://lcd.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pir.pycfn.com

[S10] C：指针与解引用
来源：http://evm.sysykeji.top

int *p = &a;  *p = 5;
来源：http://jjg.sxryk.cn

[S11] C：逐行读文件
来源：http://imf.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://pms.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://eeb.hesvh.cn

fclose(f);
来源：http://umc.tarul.cn

[S12] C：写文件
来源：http://aag.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ldm.sweek.top

[S13] C：宏定义
来源：http://pog.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ads.yongpay.top

[S14] C：枚举
来源：http://wdr.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://ohi.jinqigfzy.top

[S15] C：类型转换
来源：http://sad.yj202588.top

(double) a / b
来源：http://vvr.snrcjt.cn

[S16] C：位操作置位
来源：http://nqd.fanxiaobao.xyz

x |= (1 << 3);
来源：http://pgr.nwbrower.top

[S17] C：安全拼接字符串
来源：http://ulc.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ywk.jinqigfzy.top

[S18] C：命令行参数
来源：http://ggu.sysykeji.top


<!-- 参考信息 -->