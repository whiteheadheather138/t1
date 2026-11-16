代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://hrl.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwh.ydjk.org.cn

[Q43] 标量子查询
来源：http://uop.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qku.cheryme.top

[Q44] IN 子查询
来源：http://jib.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gix.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://psu.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dcy.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jpx.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://out.hywenlv.cn

[Q47] 与平均值比较
来源：http://dll.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nhz.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://tpn.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wxc.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://gwa.ehwqpu.com

[Q49] 更新单行
来源：http://fog.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ysa.yanxiufei.cn

[Q50] 批量更新
来源：http://ese.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://riq.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://izz.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iee.xziqi.cn

[Q52] 删除指定行
来源：http://kki.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://kbm.tianlin.xyz

[Q53] 按条件删除
来源：http://rwo.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vpc.sxryk.cn

[Q54] 清空表
来源：http://hln.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://kpr.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://nhl.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pwh.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://swb.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rro.iojbl.cn

[Q57] 行号
来源：http://epi.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ypr.zdbjq.cn

[Q58] 累计求和
来源：http://olb.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ltu.ydzc1.top

[Q59] 分组内累计
来源：http://ofr.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rng.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://fql.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wah.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tgk.yongpay.top

[Q61] 移动平均
来源：http://zwb.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rra.yonumen.top

[Q62] 分组占比
来源：http://zmq.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mdy.quarkkingdee.top

[Q63] 开启事务
来源：http://gja.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://bdg.jianghu66.top

[Q64] 提交事务
来源：http://wwn.gaohongyu789.top

COMMIT;
来源：http://jdn.dianchejie.cn

[Q65] 回滚事务
来源：http://gkb.jinqigufen.top

ROLLBACK;
来源：http://uom.zdqjudy.top

[Q66] 行锁查询
来源：http://kqw.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qzx.daxiang520.top

[Q67] 设置隔离级别
来源：http://cqq.ppjwa.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bnj.sweek.top

[Q68] 保存点
来源：http://cjm.tarul.cn

SAVEPOINT sp1;
来源：http://lpl.0kj1m.cn

ROLLBACK TO sp1;
来源：http://qtf.ppjwa.cn

[Q69] 查看执行计划
来源：http://qwj.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uxq.fktsv.cn

[Q70] 更新统计信息
来源：http://hbw.kuanghao11.cn

ANALYZE TABLE users;
来源：http://rmo.wangdashe.top

[Q71] 查看建表语句
来源：http://mea.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://slw.zhoulong.xyz

[Q72] 查看索引
来源：http://prc.daria6918.cn

SHOW INDEX FROM users;
来源：http://tww.yueranfly.top

[Q73] 查看表状态
来源：http://gzn.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qyc.redwolf501.top

[Q74] 强制使用索引
来源：http://cbv.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mjy.jqgfzy.top

[Q75] 日期格式化
来源：http://iax.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ppk.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ymt.ivvv.top

[Q76] 按天统计
来源：http://mhv.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://srm.vehdjk.com

[Q77] 时间加减
来源：http://shp.jinqigufen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mxz.aibaodan.cn

[Q78] 当前时间
来源：http://dmb.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://scy.yanxiufei.cn

[Q79] 字符串拼接
来源：http://mek.sjlbkw.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ydc.zdqjudy.top

[Q80] 字符串截取
来源：http://dyy.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qdf.52xcode.cn

[Q81] 字符串替换
来源：http://ctg.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://syy.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://lix.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gpq.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://bvr.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rhn.tianlin.xyz

[Q84] 去除首尾空格
来源：http://mvg.hysaishi.cn

SELECT TRIM(name) FROM users;
来源：http://cjl.yonumen.top

[Q85] 数值取整
来源：http://fuu.yj20258.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://okx.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://hqh.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jzj.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://gpf.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wip.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://egd.yfazqb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tvs.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://leb.fengsongda.top

[Q89] 判断表是否存在
来源：http://ebu.vehdjk.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jnj.yvedp.cn

[Q90] 生成序号列
来源：http://ipl.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gbq.chenlongwang.top

================================================================================
来源：http://mgu.tian-w.cn

R. Bash 专题
来源：http://dot.ydjk.org.cn

================================================================================
来源：http://nwg.xuanzx.com

[R01] shebang 与严格模式
来源：http://czt.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://bzy.wangdashe.top

set -euo pipefail
来源：http://ost.fzhhl.top

[R02] 变量赋值与使用
来源：http://fwe.jqgfzy.top

name="Tom"; echo "$name"
来源：http://bna.zycfv.cn

[R03] 只读变量
来源：http://jxw.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://qil.meibo888.top

[R04] 位置参数
来源：http://vxl.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pkb.fktsv.cn

[R05] 参数默认值
来源：http://ffz.dianchejie.cn

name="${1:-default}"
来源：http://wgu.yangfankeji.com

[R06] 判断命令是否存在
来源：http://kpr.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ian.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://uoz.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cyl.meibo888.top

[R08] 数值比较
来源：http://whe.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xpc.guowangkeji.top

[R09] 字符串比较
来源：http://nqi.fzhhl.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xtu.yvedp.cn

[R10] 正则匹配
来源：http://sxg.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kkq.yj202588.top

[R11] case 多分支
来源：http://nou.ydjk.org.cn

case "$1" in
来源：http://lvl.zhijiandao.cn

start) echo "启动" ;;
来源：http://fvu.hywenlv.cn

stop)  echo "停止" ;;
来源：http://ten.ctjpmb.com

*)     echo "未知命令" ;;
来源：http://kuz.sweek.top

esac
来源：http://ffs.vqdsnc.cn

[R12] for 遍历文件
来源：http://lbt.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://krn.cheryme.top

[R13] for 计数循环
来源：http://ruk.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://zsb.jiagoushi.top

[R14] C 风格 for
来源：http://rdl.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nde.ppjwa.cn

[R15] while 逐行读文件
来源：http://puu.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mdq.quarkkingdee.top

[R16] until 等待条件
来源：http://hhn.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://odp.nwbrower.top

[R17] 数组定义与取值
来源：http://onz.jinqigfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://yif.xinyue.icu

[R18] 遍历数组
来源：http://gqq.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qqx.nanxuanxn.top

[R19] 数组长度
来源：http://ivb.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://xeo.fehbvm.com

[R20] 关联数组（字典）
来源：http://uta.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eji.hnqzz.top

[R21] 字符串长度
来源：http://pkg.gotoacloud.top

echo "${#s}"
来源：http://jky.yueranfly.top

[R22] 截取子串
来源：http://nsn.hcnkem.com

echo "${s:0:5}"
来源：http://trp.nwbrower.top

[R23] 字符串替换
来源：http://ppc.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jtx.smart0.xyz

[R24] 大小写转换
来源：http://phk.cheryme.top

echo "${s^^}"; echo "${s,,}"
来源：http://wdt.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://lgb.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://spe.jinghuilouyu.cn

[R26] 命令替换
来源：http://zjx.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://cwe.zhiwuduotai.top

[R27] 算术展开
来源：http://hlf.fehbvm.com

echo $((1 + 2 * 3))
来源：http://xal.yvedp.cn

[R28] 浮点运算
来源：http://udv.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://ign.yanxiufei.cn

[R29] 定义函数
来源：http://pax.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wpm.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://qxv.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://oib.zhaomingkeji.xyz

[R31] 局部变量
来源：http://bko.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://oew.dashuyun.cn

[R32] 参数个数校验
来源：http://wna.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wlv.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://dai.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sii.zhoulong.xyz

[R34] 退出时清理
来源：http://xmu.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://mpj.smart0.xyz

[R35] 后台执行并等待
来源：http://gby.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xpc.uphjek.com

[R36] 并发执行多个任务
来源：http://kbb.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zjh.nanxinkj.top

[R37] 把输出赋给变量
来源：http://rfs.zhiwuduotai.top

files=$(ls -1)
来源：http://bmm.jinqigfzy.top

[R38] 管道串联
来源：http://qmy.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://zxl.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://ovv.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://osf.pengpengdd.cyou

[R40] 追加写日志
来源：http://jca.hesvh.cn

echo "log" >> out.log
来源：http://ajn.jianghu66.top

[R41] 丢弃输出
来源：http://nxj.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://lhu.chenjidiqi.icu

[R42] 输入重定向
来源：http://erl.jinyuanbaomall.cn

wc -l < a.txt
来源：http://xas.jianghu66.top

[R43] 按名字查找文件
来源：http://xst.sjlbkw.cn

find . -name "*.log" -type f
来源：http://ufz.jqgfzy.top

[R44] 按修改时间查找
来源：http://ywp.yj20258888.top

find . -mtime -7 -type f
来源：http://azo.ppjwa.cn

[R45] 批量删除
来源：http://ohb.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://sno.tianlin.xyz

[R46] 递归替换文件内容
来源：http://irp.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vcq.sysykeji.top

[R47] sed 单行替换
来源：http://rug.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://yro.bbcook.cn

[R48] awk 取指定列
来源：http://dmh.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://uin.shanyushiyangtech.top

[R49] awk 带条件
来源：http://ixw.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bby.pycfn.com

[R50] awk 求和
来源：http://zer.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pzb.zycfv.cn

[R51] 排序去重取前几
来源：http://fjc.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://sfv.316326.xyz

[R52] 统计行数
来源：http://czh.hnxiangtu.top

wc -l a.txt
来源：http://idz.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://wgf.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jrf.quarkkingdee.top

[R54] 比较两个文件
来源：http://nwy.sysykeji.top

diff a.txt b.txt
来源：http://tzi.wangshuangyany.cn

[R55] 压缩与解压
来源：http://pxo.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zch.jyoumei.cn

[R56] 远程拷贝
来源：http://rlz.havefunace.top

scp file user@host:/path/
来源：http://pnh.smart0.xyz

[R57] 远程执行命令
来源：http://irs.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://ggr.hongshengwenyu.top

[R58] 下载文件
来源：http://uyg.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dvr.svipenyu.cn

[R59] 发 POST JSON
来源：http://jxa.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vxl.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://glb.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://krt.jqgfzy.top

[R61] 磁盘占用
来源：http://tqg.jlsjyb.cn

df -h;  du -sh *
来源：http://ndy.jinqigufen.top

[R62] 找最占空间的文件
来源：http://cog.nwbrower.top

du -ah . | sort -rh | head -10
来源：http://aip.shzxlz.cn

[R63] 内存与进程
来源：http://txg.tian-w.cn

free -h;  ps aux | grep nginx
来源：http://asq.feifeiyinyue.top

[R64] 结束进程
来源：http://zgq.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://beq.ctjpmb.com

[R65] 查看端口占用
来源：http://apl.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ksb.xinyue.icu

[R66] 定时任务
来源：http://vbo.hfpthk.cn

crontab -e;  crontab -l
来源：http://but.yonumen.top

[R67] 生成随机十六进制串
来源：http://wrq.andypj.xyz

openssl rand -hex 16
来源：http://xht.yuxming.cn

[R68] 计算文件校验值
来源：http://ggr.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zzc.jlsjyb.cn

[R69] 生成随机密码
来源：http://nkp.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://xys.zhixingplan.top

[R70] 时间戳与互转
来源：http://mln.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://vaa.svipenyu.cn

[R71] 日期格式化
来源：http://umk.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mdt.yj20258.top

[R72] 等待端口就绪
来源：http://pam.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bbb.xylfe.cn

[R73] 分割大日志
来源：http://lao.yj20258.top

split -l 1000 big.log part_
来源：http://dyb.mhx1999.top

[R74] 批量重命名
来源：http://nku.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://orc.ehwqpu.com

[R75] 导出环境变量
来源：http://ngi.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://fjn.chenzaomai.com

[R76] 使用临时文件
来源：http://dyz.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://psy.zdqjudy.top

[R77] 读取用户输入
来源：http://tst.tarul.cn

read -rp "请输入: " ans
来源：http://ydb.gogol.net.cn

[R78] 交互式菜单
来源：http://jth.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ytf.zhixingplan.top

[R79] 解析命令行选项
来源：http://gox.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ote.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://rqn.zdqjudy.top

time ./run.sh
来源：http://fss.zdbjq.cn

================================================================================
来源：http://wuu.ivvv.top

S. C / C++ 专题
来源：http://aak.hfpthk.cn

================================================================================
来源：http://nmc.zhoulong.xyz

[S01] C：Hello World
来源：http://kpp.zhijiandao.cn

#include <stdio.h>
来源：http://yvg.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://liz.316326.xyz

[S02] C：变量与格式化输出
来源：http://nwm.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://zsw.haohaochexian.top

[S03] C：读入整数
来源：http://pzb.gzhubu.top

int x; scanf("%d", &x);
来源：http://uiy.epnwcf.com

[S04] C：字符串复制
来源：http://adb.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ljf.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://hjm.sxryk.cn

strlen(s)
来源：http://ddw.mhx1999.top

[S06] C：字符串比较
来源：http://vlt.nanxuanxn.top

strcmp(a, b) == 0
来源：http://uir.yueranfly.top

[S07] C：数组遍历求和
来源：http://jlw.yj202588.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yjd.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://acx.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sgi.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://sgg.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uji.yj202588.top

[S10] C：指针与解引用
来源：http://tud.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://brz.yj20258888.top

[S11] C：逐行读文件
来源：http://qvs.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://wyq.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://urx.sxryk.cn

fclose(f);
来源：http://whk.bbcook.cn

[S12] C：写文件
来源：http://dpm.fengsongda.top


<!-- 参考信息 -->