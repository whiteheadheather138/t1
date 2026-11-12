代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://anx.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cly.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cab.ydjk.org.cn

[Q15] 查询全部
来源：http://tko.cucudq.cn

SELECT * FROM users;
来源：http://goz.havefunace.top

[Q16] 查询指定列
来源：http://ijg.xziqi.cn

SELECT id, name FROM users;
来源：http://kpn.pycfn.com

[Q17] 条件查询
来源：http://iyg.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ohu.smart0.xyz

[Q18] 模糊匹配
来源：http://ssh.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vtk.jianghu66.top

[Q19] 范围查询
来源：http://tbc.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pvr.havefunace.top

[Q20] IN 列表
来源：http://fkx.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sbu.sjlbkw.cn

[Q21] 空值判断
来源：http://pta.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ezs.fzhhl.top

[Q22] 排序
来源：http://yqd.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tve.zhiwuduotai.top

[Q23] 分页
来源：http://epe.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sbg.ehwqpu.com

[Q24] 去重
来源：http://sac.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://xqp.52xcode.cn

[Q25] 只取前 N 条
来源：http://yke.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lik.pycfn.com

[Q26] 计数
来源：http://qop.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://wjr.hcnkem.com

[Q27] 条件计数
来源：http://xbr.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oxc.sysykeji.top

[Q28] 求和与平均
来源：http://wgt.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://let.jlsjyb.cn

[Q29] 最大最小值
来源：http://khs.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qiw.vehdjk.com

[Q30] 分组统计
来源：http://jxx.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qkl.yueranfly.top

[Q31] 分组后过滤
来源：http://zbh.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wiz.yvedp.cn

[Q32] 分组拼接字符串
来源：http://ixe.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ihe.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hum.tianlin.xyz

[Q33] 多列分组
来源：http://jci.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ogh.xziqi.cn

[Q34] 每组取第一条
来源：http://bgu.aizwys.cn

SELECT * FROM (
来源：http://eml.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cjg.nanxinkj.top

) t WHERE rn = 1;
来源：http://qml.gaohongyu789.top

[Q35] 内连接
来源：http://fzc.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://txb.wangdashe.top

[Q36] 左连接
来源：http://wsa.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ock.gzhubu.top

[Q37] 右连接
来源：http://gyk.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eao.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://hpz.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://knf.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://zco.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hho.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vxo.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ofs.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wpf.daria6918.cn

[Q41] 多表连接
来源：http://frr.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ihp.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://xbo.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://yee.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://vgv.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://qbk.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://axu.yanxiufei.cn

[Q43] 标量子查询
来源：http://iph.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rev.jqgfzy.top

[Q44] IN 子查询
来源：http://qhz.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mjl.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://nbw.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bbi.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://flx.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mns.gzhubu.top

[Q47] 与平均值比较
来源：http://trm.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xpt.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://gbq.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kzg.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://noz.smart0.xyz

[Q49] 更新单行
来源：http://cyx.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ozy.uphjek.com

[Q50] 批量更新
来源：http://uzz.quarkkingdee.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aey.zhoulong.xyz

[Q51] 用子查询更新
来源：http://bdc.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vpw.hcnkem.com

[Q52] 删除指定行
来源：http://stq.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://kcx.chenjidiqi.icu

[Q53] 按条件删除
来源：http://jwo.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tyo.ppjwa.cn

[Q54] 清空表
来源：http://mnl.redwolf501.top

TRUNCATE TABLE logs;
来源：http://skl.xuanzx.com

[Q55] 排名（并列占位）
来源：http://ixi.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hbi.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://cvx.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kws.vehdjk.com

[Q57] 行号
来源：http://bfr.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://owb.nanxuanxn.top

[Q58] 累计求和
来源：http://azv.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://glc.sjlbkw.cn

[Q59] 分组内累计
来源：http://krn.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yfm.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://fub.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vrm.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bbp.yvedp.cn

[Q61] 移动平均
来源：http://lpg.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ulr.bbcook.cn

[Q62] 分组占比
来源：http://zhq.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qtc.gzhubu.top

[Q63] 开启事务
来源：http://grj.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://srp.fanxiaobao.xyz

[Q64] 提交事务
来源：http://zuz.aibaodan.cn

COMMIT;
来源：http://amv.dashuyun.cn

[Q65] 回滚事务
来源：http://vpj.vqdsnc.cn

ROLLBACK;
来源：http://cno.sxryk.cn

[Q66] 行锁查询
来源：http://qvo.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rgr.sysykeji.top

[Q67] 设置隔离级别
来源：http://niu.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jsl.quarkkingdee.top

[Q68] 保存点
来源：http://mku.hywenlv.cn

SAVEPOINT sp1;
来源：http://hsn.cqqwz.cn

ROLLBACK TO sp1;
来源：http://cqu.ydzc1.top

[Q69] 查看执行计划
来源：http://vda.fktsv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oxe.daxiang520.top

[Q70] 更新统计信息
来源：http://ytc.chenlongwang.top

ANALYZE TABLE users;
来源：http://puj.fehbvm.com

[Q71] 查看建表语句
来源：http://peh.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ppp.vehdjk.com

[Q72] 查看索引
来源：http://hyp.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://zkg.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://nlp.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nsx.fehbvm.com

[Q74] 强制使用索引
来源：http://wdr.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ujy.shzxlz.cn

[Q75] 日期格式化
来源：http://dur.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vyp.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uss.xziqi.cn

[Q76] 按天统计
来源：http://zoq.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iqv.hcnkem.com

[Q77] 时间加减
来源：http://ywc.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://unu.c1oappe.top

[Q78] 当前时间
来源：http://qcu.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lye.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://puo.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rnk.kuanghao11.cn

[Q80] 字符串截取
来源：http://tbm.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ggt.pycfn.com

[Q81] 字符串替换
来源：http://ysh.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vlx.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://bht.guowangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yat.ehwqpu.com

[Q83] 大小写转换
来源：http://aoz.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lav.daxiang520.top

[Q84] 去除首尾空格
来源：http://mfn.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://yyq.xuetiantiany.cn

[Q85] 数值取整
来源：http://bwo.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jpq.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://vmu.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zyi.xuanzx.com

[Q87] JSON 字段做条件
来源：http://shm.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://noa.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://arp.dianchejie.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nim.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oom.aibaodan.cn

[Q89] 判断表是否存在
来源：http://thm.hywenlv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bfh.hnxiangtu.top

[Q90] 生成序号列
来源：http://egb.zhengqikj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mbt.jianghu66.top

================================================================================
来源：http://shu.hammf.cn

R. Bash 专题
来源：http://ude.yanxiufei.cn

================================================================================
来源：http://ics.chenjidiqi.icu

[R01] shebang 与严格模式
来源：http://ruk.vehdjk.com

#!/usr/bin/env bash
来源：http://umx.zhiwuduotai.top

set -euo pipefail
来源：http://mbx.shuidangran.top

[R02] 变量赋值与使用
来源：http://wca.sxryk.cn

name="Tom"; echo "$name"
来源：http://fon.xuanzx.com

[R03] 只读变量
来源：http://uvt.pycfn.com

readonly PI=3.14
来源：http://ihp.sxryk.cn

[R04] 位置参数
来源：http://wtq.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ysz.meibo888.top

[R05] 参数默认值
来源：http://tjk.yonumen.top

name="${1:-default}"
来源：http://yqo.yongpay.top

[R06] 判断命令是否存在
来源：http://sck.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uog.yanxiufei.cn

[R07] if 判断文件
来源：http://clw.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yfq.yj20258888.top

[R08] 数值比较
来源：http://uhb.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jtz.zdbjq.cn

[R09] 字符串比较
来源：http://tug.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lam.vqdsnc.cn

[R10] 正则匹配
来源：http://dio.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ukj.52xcode.cn

[R11] case 多分支
来源：http://wfm.sxryk.cn

case "$1" in
来源：http://rqc.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://xah.ehwqpu.com

stop)  echo "停止" ;;
来源：http://ksq.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://vji.52xcode.cn

esac
来源：http://ebx.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://msv.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://vts.zdbjq.cn

[R13] for 计数循环
来源：http://tbv.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://tsl.zdbjq.cn

[R14] C 风格 for
来源：http://wjt.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xai.yuxming.cn

[R15] while 逐行读文件
来源：http://lmm.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xvm.zhengqikj.top

[R16] until 等待条件
来源：http://dkr.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xkm.jiagoushi.top

[R17] 数组定义与取值
来源：http://kpa.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://vlx.c1oappe.top

[R18] 遍历数组
来源：http://zmd.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qbc.meibo888.top

[R19] 数组长度
来源：http://evi.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://uyk.tianlin.xyz

[R20] 关联数组（字典）
来源：http://euw.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ogy.quarkkingdee.top

[R21] 字符串长度
来源：http://agz.svipenyu.cn

echo "${#s}"
来源：http://qfk.shzxlz.cn

[R22] 截取子串
来源：http://gpe.tian-w.cn

echo "${s:0:5}"
来源：http://ven.mhx1999.top

[R23] 字符串替换
来源：http://kto.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://chk.nwbrower.top

[R24] 大小写转换
来源：http://abw.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://cqm.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://uvx.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ypm.ppjwa.cn

[R26] 命令替换
来源：http://cko.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://klz.ydjk.org.cn

[R27] 算术展开
来源：http://tgh.hesvh.cn

echo $((1 + 2 * 3))
来源：http://wrh.xuetiantiany.cn

[R28] 浮点运算
来源：http://glw.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://qav.chenlongwang.top

[R29] 定义函数
来源：http://cug.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dxs.pycfn.com

[R30] 函数返回状态码
来源：http://tcj.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://weh.sjlbkw.cn

[R31] 局部变量
来源：http://xqv.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://hhl.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://ibd.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yab.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://ikb.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bca.hongshengwenyu.top

[R34] 退出时清理
来源：http://wjt.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://xil.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://fma.dianchejie.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://khl.52xcode.cn

[R36] 并发执行多个任务
来源：http://cgy.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hzp.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://ohv.epnwcf.com

files=$(ls -1)
来源：http://pxu.smart0.xyz

[R38] 管道串联
来源：http://vxc.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://udf.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://bnp.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://qmn.wangdashe.top

[R40] 追加写日志
来源：http://fio.ctjpmb.com

echo "log" >> out.log
来源：http://aet.yanxiufei.cn

[R41] 丢弃输出
来源：http://qwq.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://doc.shzxlz.cn

[R42] 输入重定向
来源：http://jtt.yueranfly.top

wc -l < a.txt
来源：http://lvt.tarul.cn

[R43] 按名字查找文件
来源：http://oxn.jinqigfzy.top

find . -name "*.log" -type f
来源：http://rhb.shzxlz.cn

[R44] 按修改时间查找
来源：http://icw.ivvv.top

find . -mtime -7 -type f
来源：http://lfn.tarul.cn

[R45] 批量删除
来源：http://zvh.nwbrower.top

find . -name "*.tmp" -delete
来源：http://zcu.ctjpmb.com

[R46] 递归替换文件内容
来源：http://kxf.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rrx.tian-w.cn

[R47] sed 单行替换
来源：http://lax.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://ldi.zhengqikj.top

[R48] awk 取指定列
来源：http://wqw.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://poq.chenlongwang.top

[R49] awk 带条件
来源：http://crb.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yzn.pycfn.com

[R50] awk 求和
来源：http://qsl.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://oqt.tianlin.xyz

[R51] 排序去重取前几
来源：http://voc.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xqe.zhixingplan.top

[R52] 统计行数
来源：http://hpi.chenjidiqi.icu

wc -l a.txt
来源：http://pbj.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://ajy.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jib.zhengqikj.top

[R54] 比较两个文件
来源：http://ttb.guannengcc.top

diff a.txt b.txt
来源：http://gtm.316326.xyz

[R55] 压缩与解压
来源：http://sis.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qmf.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://wll.fktsv.cn

scp file user@host:/path/
来源：http://syd.guowangkeji.top

[R57] 远程执行命令
来源：http://rsw.smart0.xyz

ssh user@host 'uptime'
来源：http://qbf.fktsv.cn

[R58] 下载文件
来源：http://opr.meibo888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eer.epnwcf.com

[R59] 发 POST JSON
来源：http://dzi.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipb.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://wut.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://juc.jlsjyb.cn

[R61] 磁盘占用
来源：http://dbg.sweek.top

df -h;  du -sh *
来源：http://kqm.chenzaomai.com

[R62] 找最占空间的文件
来源：http://uep.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://jjq.cashguo.top

[R63] 内存与进程
来源：http://bof.jiagoushi.top


<!-- 参考信息 -->