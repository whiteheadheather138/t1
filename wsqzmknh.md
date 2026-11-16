代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://asl.pycfn.com

[Q20] IN 列表
来源：http://jrn.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cdl.aibaodan.cn

[Q21] 空值判断
来源：http://ugs.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zpe.cqqwz.cn

[Q22] 排序
来源：http://khf.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vyh.ydjk.org.cn

[Q23] 分页
来源：http://dit.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xem.yongpay.top

[Q24] 去重
来源：http://fhy.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://jkb.snrcjt.cn

[Q25] 只取前 N 条
来源：http://cps.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rdh.bbcook.cn

[Q26] 计数
来源：http://mdr.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://lvu.yfazqb.com

[Q27] 条件计数
来源：http://avg.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dmi.aibaodan.cn

[Q28] 求和与平均
来源：http://fxu.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ckr.yvedp.cn

[Q29] 最大最小值
来源：http://zfs.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ijl.ivvv.top

[Q30] 分组统计
来源：http://esz.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yls.hammf.cn

[Q31] 分组后过滤
来源：http://jkk.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ssv.tian-w.cn

[Q32] 分组拼接字符串
来源：http://dfo.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dwo.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vgq.fengsongda.top

[Q33] 多列分组
来源：http://vcn.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oif.sysykeji.top

[Q34] 每组取第一条
来源：http://zlr.yanxiufei.cn

SELECT * FROM (
来源：http://gzu.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lfo.guowangkeji.top

) t WHERE rn = 1;
来源：http://vag.chenjidiqi.icu

[Q35] 内连接
来源：http://ufr.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://guh.zhaomingkeji.xyz

[Q36] 左连接
来源：http://pjl.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dnv.daxiang520.top

[Q37] 右连接
来源：http://udy.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://euu.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zsk.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://prp.hammf.cn

[Q39] 自连接（查上下级）
来源：http://ebc.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://wgk.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cjl.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pkz.bjfxy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qwx.jqgfzy.top

[Q41] 多表连接
来源：http://vaa.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rwb.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://pic.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://hkp.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://iqz.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://avu.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tjp.yueranfly.top

[Q43] 标量子查询
来源：http://evw.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://urv.ehwqpu.com

[Q44] IN 子查询
来源：http://rax.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kxs.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://vpz.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iev.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://ngj.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xyv.aizwys.cn

[Q47] 与平均值比较
来源：http://fij.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gha.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://tez.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wct.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://fcl.xziqi.cn

[Q49] 更新单行
来源：http://jnc.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nbt.epnwcf.com

[Q50] 批量更新
来源：http://kag.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cho.hcnkem.com

[Q51] 用子查询更新
来源：http://odq.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://msv.cashguo.top

[Q52] 删除指定行
来源：http://mxz.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://tqy.chenlongwang.top

[Q53] 按条件删除
来源：http://uvx.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mzs.sjlbkw.cn

[Q54] 清空表
来源：http://ban.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://fnd.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://bwk.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hcg.shanyushiyangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://zqu.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lgr.jyoumei.cn

[Q57] 行号
来源：http://jhq.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cyf.yanxiufei.cn

[Q58] 累计求和
来源：http://hvw.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ruu.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://rgs.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rov.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://hjq.jinghuilouyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nmo.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sdb.c1oappe.top

[Q61] 移动平均
来源：http://bhk.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qmq.wangshuangyany.cn

[Q62] 分组占比
来源：http://hfk.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rws.dashuyun.cn

[Q63] 开启事务
来源：http://fwr.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pdq.hysaishi.cn

[Q64] 提交事务
来源：http://tdk.pengpengdd.cyou

COMMIT;
来源：http://tjz.daxiang520.top

[Q65] 回滚事务
来源：http://fww.gzhubu.top

ROLLBACK;
来源：http://icf.pycfn.com

[Q66] 行锁查询
来源：http://cln.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mhf.smart0.xyz

[Q67] 设置隔离级别
来源：http://iqp.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qii.sjlbkw.cn

[Q68] 保存点
来源：http://skt.ydzc1.top

SAVEPOINT sp1;
来源：http://mpx.snrcjt.cn

ROLLBACK TO sp1;
来源：http://thr.zhoulong.xyz

[Q69] 查看执行计划
来源：http://lky.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mya.yanxiufei.cn

[Q70] 更新统计信息
来源：http://plw.yanxiufei.cn

ANALYZE TABLE users;
来源：http://ekr.hnqzz.top

[Q71] 查看建表语句
来源：http://zge.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mee.ctjpmb.com

[Q72] 查看索引
来源：http://bys.xinyue.icu

SHOW INDEX FROM users;
来源：http://ukq.yueranfly.top

[Q73] 查看表状态
来源：http://ich.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://hke.chenlongwang.top

[Q74] 强制使用索引
来源：http://ejl.tian-w.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ynl.jlsjyb.cn

[Q75] 日期格式化
来源：http://mco.cashguo.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zfl.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hhc.pengpengdd.cyou

[Q76] 按天统计
来源：http://tdv.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vtw.mhx1999.top

[Q77] 时间加减
来源：http://fii.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dcf.feifeiyinyue.top

[Q78] 当前时间
来源：http://hyo.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oyv.fktsv.cn

[Q79] 字符串拼接
来源：http://udh.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xtz.birdmap.top

[Q80] 字符串截取
来源：http://vgz.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zvl.jiagoushi.top

[Q81] 字符串替换
来源：http://mnf.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cbz.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://zqs.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rba.yuxming.cn

[Q83] 大小写转换
来源：http://rtm.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fmb.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://dbb.jiagoushi.top

SELECT TRIM(name) FROM users;
来源：http://tzz.iojbl.cn

[Q85] 数值取整
来源：http://cma.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yvl.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://laq.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vjk.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://utp.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hbj.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://atq.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpp.gzhubu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mza.chenjidiqi.icu

[Q89] 判断表是否存在
来源：http://jhi.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vyz.c1oappe.top

[Q90] 生成序号列
来源：http://dgk.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jln.jinghuilouyu.cn

================================================================================
来源：http://qan.yueranfly.top

R. Bash 专题
来源：http://mju.xylfe.cn

================================================================================
来源：http://gpc.bjfxy.top

[R01] shebang 与严格模式
来源：http://skc.0kj1m.cn

#!/usr/bin/env bash
来源：http://nta.xinyue.icu

set -euo pipefail
来源：http://aed.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://sma.mhx1999.top

name="Tom"; echo "$name"
来源：http://xqf.vehdjk.com

[R03] 只读变量
来源：http://viu.shzxlz.cn

readonly PI=3.14
来源：http://ctc.316326.xyz

[R04] 位置参数
来源：http://enq.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lgb.dashuyun.cn

[R05] 参数默认值
来源：http://nrt.wangdashe.top

name="${1:-default}"
来源：http://jry.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://pyl.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txe.vehdjk.com

[R07] if 判断文件
来源：http://rvy.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bzr.meibo888.top

[R08] 数值比较
来源：http://vbz.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jbw.nanxinkj.top

[R09] 字符串比较
来源：http://viv.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qse.cheryme.top

[R10] 正则匹配
来源：http://ras.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rdn.xuetiantiany.cn

[R11] case 多分支
来源：http://rxz.jinghuilouyu.cn

case "$1" in
来源：http://urc.jqgfzy.top

start) echo "启动" ;;
来源：http://icq.jqgufenzy.top

stop)  echo "停止" ;;
来源：http://ico.xuanzx.com

*)     echo "未知命令" ;;
来源：http://knc.gzhubu.top

esac
来源：http://qgo.hfpthk.cn

[R12] for 遍历文件
来源：http://jut.guowangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ukm.fanxiaobao.xyz

[R13] for 计数循环
来源：http://lxt.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://pkc.fehbvm.com

[R14] C 风格 for
来源：http://qsz.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qmx.ivvv.top

[R15] while 逐行读文件
来源：http://bxb.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xok.cashguo.top

[R16] until 等待条件
来源：http://khu.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dtt.yj20258888.top

[R17] 数组定义与取值
来源：http://zbf.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jpo.yj20258888.top

[R18] 遍历数组
来源：http://fbp.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpz.kuanghao11.cn

[R19] 数组长度
来源：http://ktf.316326.xyz

echo "${#arr[@]}"
来源：http://rhh.sweek.top

[R20] 关联数组（字典）
来源：http://rvw.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wed.fengsongda.top

[R21] 字符串长度
来源：http://brk.tanke756.top

echo "${#s}"
来源：http://guu.hesvh.cn

[R22] 截取子串
来源：http://khy.xuanzx.com

echo "${s:0:5}"
来源：http://rwd.316326.xyz

[R23] 字符串替换
来源：http://xpj.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://clv.jinghuilouyu.cn

[R24] 大小写转换
来源：http://orn.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://wni.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://ncp.xuetiantiany.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mjv.pycfn.com

[R26] 命令替换
来源：http://smj.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://fpy.sufxvd.cn

[R27] 算术展开
来源：http://exp.uphjek.com

echo $((1 + 2 * 3))
来源：http://hfw.gotoacloud.top

[R28] 浮点运算
来源：http://dua.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://rty.jinghuilouyu.cn

[R29] 定义函数
来源：http://mbv.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iyh.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://rel.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://xrb.iojbl.cn

[R31] 局部变量
来源：http://ajz.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://atz.wangshuangyany.cn

[R32] 参数个数校验
来源：http://wje.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vwh.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://quj.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jzy.nwbrower.top

[R34] 退出时清理
来源：http://wvo.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://knx.sysykeji.top

[R35] 后台执行并等待
来源：http://pqw.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hrs.haohaochexian.top

[R36] 并发执行多个任务
来源：http://kwu.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vqu.epnwcf.com

[R37] 把输出赋给变量
来源：http://ryd.bjfxy.top

files=$(ls -1)
来源：http://iea.c1oappe.top

[R38] 管道串联
来源：http://xdj.cheryme.top

cat a.txt | grep -i error | wc -l
来源：http://ndm.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://smr.yj20258.top

cmd > out.log 2>&1
来源：http://slp.yfazqb.com

[R40] 追加写日志
来源：http://hwq.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://euy.svipenyu.cn

[R41] 丢弃输出
来源：http://qcu.ybcxt.top

cmd >/dev/null 2>&1
来源：http://bri.andypj.xyz

[R42] 输入重定向
来源：http://zwl.ivvv.top

wc -l < a.txt
来源：http://btx.zhengqikj.top

[R43] 按名字查找文件
来源：http://jns.hammf.cn

find . -name "*.log" -type f
来源：http://hfj.meibo888.top

[R44] 按修改时间查找
来源：http://luw.gotoacloud.top

find . -mtime -7 -type f
来源：http://taf.jlsjyb.cn

[R45] 批量删除
来源：http://ihc.cheryme.top

find . -name "*.tmp" -delete
来源：http://qzp.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://whd.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vhd.yongpay.top

[R47] sed 单行替换
来源：http://fwy.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fww.aibaodan.cn

[R48] awk 取指定列
来源：http://owj.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://otf.ctjpmb.com

[R49] awk 带条件
来源：http://sgy.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://syb.guannengcc.top

[R50] awk 求和
来源：http://qbg.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://pdh.havefunace.top

[R51] 排序去重取前几
来源：http://lgl.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rvx.zhengqikj.top

[R52] 统计行数
来源：http://soc.gotoacloud.top

wc -l a.txt
来源：http://bvc.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://nvy.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://got.hywenlv.cn

[R54] 比较两个文件
来源：http://ohn.shangyingyoupin.top

diff a.txt b.txt
来源：http://gsi.pycfn.com

[R55] 压缩与解压
来源：http://tbo.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ysh.redwolf501.top

[R56] 远程拷贝
来源：http://cku.redwolf501.top

scp file user@host:/path/
来源：http://qah.jqgfzy.top

[R57] 远程执行命令
来源：http://vmr.chenzaomai.com

ssh user@host 'uptime'
来源：http://jsg.chenzaomai.com

[R58] 下载文件
来源：http://nvw.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jnk.xziqi.cn

[R59] 发 POST JSON
来源：http://ghy.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mhb.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://xko.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zxd.jinqigfzy.top

[R61] 磁盘占用
来源：http://fmy.birdmap.top

df -h;  du -sh *
来源：http://jkw.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://cut.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://ymt.shanyushiyangtech.top

[R63] 内存与进程
来源：http://rbp.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://jok.guowangkeji.top

[R64] 结束进程
来源：http://esa.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://bby.xuanzx.com

[R65] 查看端口占用
来源：http://qxc.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qix.hnxiangtu.top

[R66] 定时任务
来源：http://vpo.hcnkem.com

crontab -e;  crontab -l
来源：http://eop.aizwys.cn

[R67] 生成随机十六进制串
来源：http://kkh.zhixingplan.top

openssl rand -hex 16
来源：http://cif.zhoulong.xyz

[R68] 计算文件校验值
来源：http://xnf.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lbx.vehdjk.com

[R69] 生成随机密码
来源：http://uba.yuxming.cn


<!-- 参考信息 -->