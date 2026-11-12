代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tcu.hnqzz.top

[Q26] 计数
来源：http://nzg.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://scd.snrcjt.cn

[Q27] 条件计数
来源：http://tjk.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://loi.yuanzhike.top

[Q28] 求和与平均
来源：http://crq.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://frl.yanxiufei.cn

[Q29] 最大最小值
来源：http://wmt.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kqo.bbcook.cn

[Q30] 分组统计
来源：http://zrj.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qqu.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://eug.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tyn.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://jfa.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://voz.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ysn.cqqwz.cn

[Q33] 多列分组
来源：http://hsh.hnqzz.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nqn.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://irj.jinqigufen.top

SELECT * FROM (
来源：http://lqk.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gvn.gotoacloud.top

) t WHERE rn = 1;
来源：http://mod.shzxlz.cn

[Q35] 内连接
来源：http://qlq.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rob.meibo888.top

[Q36] 左连接
来源：http://ewu.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mcf.tianlin.xyz

[Q37] 右连接
来源：http://lwl.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tgz.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://svb.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://svt.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://coq.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hbg.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cri.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://lse.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oqw.yonumen.top

[Q41] 多表连接
来源：http://ett.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eqp.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://zsb.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://nbu.cashguo.top

[Q42] 连接条件附加过滤
来源：http://nen.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://vkp.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yww.yvedp.cn

[Q43] 标量子查询
来源：http://omj.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qqx.zhixingplan.top

[Q44] IN 子查询
来源：http://bzc.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sru.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://jjp.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://imu.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hwl.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpm.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://zar.tian-w.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ltl.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://kat.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fyf.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://fpr.tarul.cn

[Q49] 更新单行
来源：http://fda.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fbk.dianchejie.cn

[Q50] 批量更新
来源：http://uhj.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jcp.nanxinkj.top

[Q51] 用子查询更新
来源：http://noy.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ahf.uphjek.com

[Q52] 删除指定行
来源：http://tcm.hongshengwenyu.top

DELETE FROM users WHERE id = 10;
来源：http://ghw.tanke756.top

[Q53] 按条件删除
来源：http://bye.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://drp.vehdjk.com

[Q54] 清空表
来源：http://qkx.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://xqb.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://waj.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vvt.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://vwo.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://anf.yuanzhike.top

[Q57] 行号
来源：http://iqg.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sjl.yj202588.top

[Q58] 累计求和
来源：http://vbj.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tst.chenzaomai.com

[Q59] 分组内累计
来源：http://jsx.tanke756.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vls.shzxlz.cn

[Q60] 取上一行 / 下一行
来源：http://mpu.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pbh.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zts.9152youxi.cn

[Q61] 移动平均
来源：http://ppo.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gyw.shzxlz.cn

[Q62] 分组占比
来源：http://mcx.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wyy.svipenyu.cn

[Q63] 开启事务
来源：http://zka.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://apu.birdmap.top

[Q64] 提交事务
来源：http://ddo.zhijiandao.cn

COMMIT;
来源：http://ade.ppjwa.cn

[Q65] 回滚事务
来源：http://inn.svipenyu.cn

ROLLBACK;
来源：http://uyg.ywan-chungtsiang.top

[Q66] 行锁查询
来源：http://kha.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zdw.sweek.top

[Q67] 设置隔离级别
来源：http://jsb.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cbb.wangshuangyany.cn

[Q68] 保存点
来源：http://fcm.xinyue.icu

SAVEPOINT sp1;
来源：http://cwx.cdnleiting.top

ROLLBACK TO sp1;
来源：http://dmz.bbcook.cn

[Q69] 查看执行计划
来源：http://haa.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xih.zhongyouzk.top

[Q70] 更新统计信息
来源：http://dzh.hysaishi.cn

ANALYZE TABLE users;
来源：http://vbw.haohaochexian.top

[Q71] 查看建表语句
来源：http://twa.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zol.havefunace.top

[Q72] 查看索引
来源：http://frs.svipenyu.cn

SHOW INDEX FROM users;
来源：http://fuv.sufxvd.cn

[Q73] 查看表状态
来源：http://jop.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aux.epnwcf.com

[Q74] 强制使用索引
来源：http://cvj.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://avu.hesvh.cn

[Q75] 日期格式化
来源：http://tpu.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dtn.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wni.zhoulong.xyz

[Q76] 按天统计
来源：http://jlv.xingfuxueyuan.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gky.yj202588.top

[Q77] 时间加减
来源：http://sog.aibaodan.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yiv.yuanzhike.top

[Q78] 当前时间
来源：http://fby.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ufj.daria6918.cn

[Q79] 字符串拼接
来源：http://rim.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qnc.shzxlz.cn

[Q80] 字符串截取
来源：http://zlx.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dtr.yvedp.cn

[Q81] 字符串替换
来源：http://lxi.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yhv.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://wtz.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://alj.tanke756.top

[Q83] 大小写转换
来源：http://dah.fktsv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uou.uphjek.com

[Q84] 去除首尾空格
来源：http://ksq.shanyushiyangtech.top

SELECT TRIM(name) FROM users;
来源：http://llh.tian-w.cn

[Q85] 数值取整
来源：http://ccb.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wun.fktsv.cn

[Q86] 读取 JSON 字段
来源：http://fzi.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qtt.havefunace.top

[Q87] JSON 字段做条件
来源：http://irf.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zqz.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://nkn.bjfxy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://guu.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gpc.guowangkeji.top

[Q89] 判断表是否存在
来源：http://mjd.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mjp.meibo888.top

[Q90] 生成序号列
来源：http://yqw.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://elt.gaohongyu789.top

================================================================================
来源：http://jew.smart0.xyz

R. Bash 专题
来源：http://kmf.yuanzhike.top

================================================================================
来源：http://btq.birdmap.top

[R01] shebang 与严格模式
来源：http://zvj.vehdjk.com

#!/usr/bin/env bash
来源：http://zoo.316326.xyz

set -euo pipefail
来源：http://pfp.tanke756.top

[R02] 变量赋值与使用
来源：http://ibn.c1oappe.top

name="Tom"; echo "$name"
来源：http://xhv.xziqi.cn

[R03] 只读变量
来源：http://sct.hysaishi.cn

readonly PI=3.14
来源：http://yzb.sysykeji.top

[R04] 位置参数
来源：http://icm.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hnn.yfazqb.com

[R05] 参数默认值
来源：http://avq.zhoulong.xyz

name="${1:-default}"
来源：http://ycs.birdmap.top

[R06] 判断命令是否存在
来源：http://sxm.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bdg.epnwcf.com

[R07] if 判断文件
来源：http://wsi.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mqq.0kj1m.cn

[R08] 数值比较
来源：http://tag.xylfe.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://spb.vehdjk.com

[R09] 字符串比较
来源：http://ceu.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hfl.yueranfly.top

[R10] 正则匹配
来源：http://isx.ctjpmb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hzt.yfazqb.com

[R11] case 多分支
来源：http://kiv.cashguo.top

case "$1" in
来源：http://xmp.guannengcc.top

start) echo "启动" ;;
来源：http://zex.fengsongda.top

stop)  echo "停止" ;;
来源：http://arq.hnqzz.top

*)     echo "未知命令" ;;
来源：http://bxl.fehbvm.com

esac
来源：http://wey.haohaochexian.top

[R12] for 遍历文件
来源：http://amu.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://xhp.sufxvd.cn

[R13] for 计数循环
来源：http://jgc.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://uuf.pycfn.com

[R14] C 风格 for
来源：http://kpl.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wky.bbcook.cn

[R15] while 逐行读文件
来源：http://lxz.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dyi.guannengcc.top

[R16] until 等待条件
来源：http://nje.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wfa.haohaochexian.top

[R17] 数组定义与取值
来源：http://ynz.dashuyun.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tfe.0kj1m.cn

[R18] 遍历数组
来源：http://vsr.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vpf.chenlongwang.top

[R19] 数组长度
来源：http://gvf.guannengcc.top

echo "${#arr[@]}"
来源：http://pgn.jqgfzy.top

[R20] 关联数组（字典）
来源：http://snc.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sst.daxiang520.top

[R21] 字符串长度
来源：http://qpo.sweek.top

echo "${#s}"
来源：http://xdq.fktsv.cn

[R22] 截取子串
来源：http://bfy.zhongyouzk.top

echo "${s:0:5}"
来源：http://ohu.bjfxy.top

[R23] 字符串替换
来源：http://myw.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uot.yonumen.top

[R24] 大小写转换
来源：http://rwx.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yjd.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://wxk.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://xee.jqgfzy.top

[R26] 命令替换
来源：http://pph.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://qwc.dashuyun.cn

[R27] 算术展开
来源：http://qpx.xuanzx.com

echo $((1 + 2 * 3))
来源：http://nos.havefunace.top

[R28] 浮点运算
来源：http://wnz.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://olp.cqqwz.cn

[R29] 定义函数
来源：http://ojp.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zvu.sufxvd.cn

[R30] 函数返回状态码
来源：http://eim.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://hpu.vehdjk.com

[R31] 局部变量
来源：http://evz.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://qac.hesvh.cn

[R32] 参数个数校验
来源：http://ldg.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://swi.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://dls.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lvl.gaohongyu789.top

[R34] 退出时清理
来源：http://tip.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://bgj.hysaishi.cn

[R35] 后台执行并等待
来源：http://sqt.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hcs.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://nip.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://flb.ehwqpu.com

[R37] 把输出赋给变量
来源：http://dvf.feifeiyinyue.top

files=$(ls -1)
来源：http://xzw.fanxiaobao.xyz

[R38] 管道串联
来源：http://sqx.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://adx.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://ajx.yonumen.top

cmd > out.log 2>&1
来源：http://tei.yvedp.cn

[R40] 追加写日志
来源：http://lcs.9152youxi.cn

echo "log" >> out.log
来源：http://acs.wangshuangyany.cn

[R41] 丢弃输出
来源：http://orw.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://shz.bjfxy.top

[R42] 输入重定向
来源：http://wwc.tian-w.cn

wc -l < a.txt
来源：http://wvq.haohaochexian.top

[R43] 按名字查找文件
来源：http://syl.ybcxt.top

find . -name "*.log" -type f
来源：http://cme.jqgfzy.top

[R44] 按修改时间查找
来源：http://yqb.zdbjq.cn

find . -mtime -7 -type f
来源：http://zwh.guannengcc.top

[R45] 批量删除
来源：http://rkv.redwolf501.top

find . -name "*.tmp" -delete
来源：http://xes.dashuyun.cn

[R46] 递归替换文件内容
来源：http://pfi.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jft.snrcjt.cn

[R47] sed 单行替换
来源：http://lwm.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://arv.meibo888.top

[R48] awk 取指定列
来源：http://sfw.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://mop.guannengcc.top

[R49] awk 带条件
来源：http://sda.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ixq.cheryme.top

[R50] awk 求和
来源：http://xkb.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dfa.iojbl.cn

[R51] 排序去重取前几
来源：http://mfj.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rey.yonumen.top

[R52] 统计行数
来源：http://xcb.zycfv.cn

wc -l a.txt
来源：http://dsj.316326.xyz

[R53] 查看文件头与实时尾
来源：http://pdc.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ply.9152youxi.cn

[R54] 比较两个文件
来源：http://wph.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://jal.ppjwa.cn

[R55] 压缩与解压
来源：http://pqx.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://urn.tarul.cn

[R56] 远程拷贝
来源：http://ghs.ehwqpu.com

scp file user@host:/path/
来源：http://cbx.hnqzz.top

[R57] 远程执行命令
来源：http://dcj.quarkkingdee.top

ssh user@host 'uptime'
来源：http://gfq.dianchejie.cn

[R58] 下载文件
来源：http://oxe.52xcode.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sbz.jianghu66.top

[R59] 发 POST JSON
来源：http://ijd.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://din.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://qxq.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cme.xuetiantiany.cn

[R61] 磁盘占用
来源：http://hwb.smart0.xyz

df -h;  du -sh *
来源：http://scn.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://caz.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://mrj.dashuyun.cn

[R63] 内存与进程
来源：http://xls.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://ezw.hammf.cn

[R64] 结束进程
来源：http://oyz.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://yvs.yj202588.top

[R65] 查看端口占用
来源：http://oow.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://onx.hywenlv.cn

[R66] 定时任务
来源：http://uyx.zhoulong.xyz

crontab -e;  crontab -l
来源：http://jcu.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://xph.tarul.cn

openssl rand -hex 16
来源：http://ear.fengsongda.top

[R68] 计算文件校验值
来源：http://ieb.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://sdp.jqgfzy.top

[R69] 生成随机密码
来源：http://udf.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://nef.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://awn.c1oappe.top

date +%s;  date -d @1700000000
来源：http://lub.zhengqikj.top

[R71] 日期格式化
来源：http://gnl.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://bgi.tanke756.top

[R72] 等待端口就绪
来源：http://xcc.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://onu.ybcxt.top

[R73] 分割大日志
来源：http://etx.yj20258888.top

split -l 1000 big.log part_
来源：http://bbz.jinqigfzy.top

[R74] 批量重命名
来源：http://tla.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bex.zhongyouzk.top

[R75] 导出环境变量
来源：http://izd.shanyushiyangtech.top


<!-- 参考信息 -->