代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://deq.cashguo.top

[Q07] 删除表
来源：http://hts.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://eex.kuanghao11.cn

[Q08] 创建普通索引
来源：http://twb.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tdh.tianlin.xyz

[Q09] 创建唯一索引
来源：http://rgy.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yuw.vehdjk.com

[Q10] 插入单行
来源：http://kie.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kee.shzxlz.cn

[Q11] 一次插入多行
来源：http://zon.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://agy.nwbrower.top

[Q12] 插入后取自增 ID
来源：http://jqh.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://urg.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aai.jiagoushi.top

[Q13] 忽略重复插入
来源：http://tjl.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mtt.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://dyl.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gnk.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qin.zdqjudy.top

[Q15] 查询全部
来源：http://sxj.316326.xyz

SELECT * FROM users;
来源：http://nse.fengsongda.top

[Q16] 查询指定列
来源：http://mjk.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://ceh.fehbvm.com

[Q17] 条件查询
来源：http://bgm.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bdr.guannengcc.top

[Q18] 模糊匹配
来源：http://oov.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uha.gotoacloud.top

[Q19] 范围查询
来源：http://wyw.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mhi.fehbvm.com

[Q20] IN 列表
来源：http://tpt.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pqm.hongshengwenyu.top

[Q21] 空值判断
来源：http://tmp.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ctq.uphjek.com

[Q22] 排序
来源：http://bzy.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://txv.bjfxy.top

[Q23] 分页
来源：http://ild.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kdd.sufxvd.cn

[Q24] 去重
来源：http://rqv.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://asc.yangfankeji.com

[Q25] 只取前 N 条
来源：http://qqh.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pib.gzhubu.top

[Q26] 计数
来源：http://txj.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://xvy.wangdashe.top

[Q27] 条件计数
来源：http://zok.daxiang520.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uwr.zhiwuduotai.top

[Q28] 求和与平均
来源：http://cam.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://plv.xylfe.cn

[Q29] 最大最小值
来源：http://ijb.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kql.hnqzz.top

[Q30] 分组统计
来源：http://bov.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zrm.hammf.cn

[Q31] 分组后过滤
来源：http://www.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://caz.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://omk.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gdh.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cyy.yangfankeji.com

[Q33] 多列分组
来源：http://hnb.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vpj.ydjk.org.cn

[Q34] 每组取第一条
来源：http://ubd.haohaochexian.top

SELECT * FROM (
来源：http://ven.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xcc.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://ejn.jyoumei.cn

[Q35] 内连接
来源：http://yac.yj202588.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://awd.fehbvm.com

[Q36] 左连接
来源：http://dci.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ygr.tarul.cn

[Q37] 右连接
来源：http://mja.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fcb.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://alu.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oga.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://cil.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dzt.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xer.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vaf.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xfs.ppjwa.cn

[Q41] 多表连接
来源：http://jcl.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://gnd.sjlbkw.cn

JOIN users u ON u.id = o.user_id
来源：http://zvv.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://gtt.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://wjt.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://hbo.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wia.gogol.net.cn

[Q43] 标量子查询
来源：http://qjw.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ugc.vqdsnc.cn

[Q44] IN 子查询
来源：http://bhh.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://grg.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://gay.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fph.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vgo.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bgi.sysykeji.top

[Q47] 与平均值比较
来源：http://vkm.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cte.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://ted.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pve.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://ihq.vqdsnc.cn

[Q49] 更新单行
来源：http://xes.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tqq.jinqigfzy.top

[Q50] 批量更新
来源：http://phf.ivvv.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yhr.chenlongwang.top

[Q51] 用子查询更新
来源：http://gsz.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kqk.yj20258888.top

[Q52] 删除指定行
来源：http://pjo.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://tvp.zdbjq.cn

[Q53] 按条件删除
来源：http://ypo.nanxuanxn.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://omw.kuanghao11.cn

[Q54] 清空表
来源：http://oce.yuxming.cn

TRUNCATE TABLE logs;
来源：http://ios.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://yki.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qmj.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://xnz.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ruc.xziqi.cn

[Q57] 行号
来源：http://ipc.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dop.smart0.xyz

[Q58] 累计求和
来源：http://sbq.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://foc.316326.xyz

[Q59] 分组内累计
来源：http://okx.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hkj.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://vbp.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uui.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kmu.ydzc1.top

[Q61] 移动平均
来源：http://ufc.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jtd.yuxming.cn

[Q62] 分组占比
来源：http://joi.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbv.ivvv.top

[Q63] 开启事务
来源：http://rkm.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://rhq.yongpay.top

[Q64] 提交事务
来源：http://tst.zhixingplan.top

COMMIT;
来源：http://wbx.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://xau.ybcxt.top

ROLLBACK;
来源：http://bwo.nanxuanxn.top

[Q66] 行锁查询
来源：http://xdl.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nux.ehwqpu.com

[Q67] 设置隔离级别
来源：http://wrq.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zfd.zhixingplan.top

[Q68] 保存点
来源：http://qew.yongpay.top

SAVEPOINT sp1;
来源：http://nki.xuanzx.com

ROLLBACK TO sp1;
来源：http://jqe.kuanghao11.cn

[Q69] 查看执行计划
来源：http://fej.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hpv.dianchejie.cn

[Q70] 更新统计信息
来源：http://xou.ydzc1.top

ANALYZE TABLE users;
来源：http://vcx.zhixingplan.top

[Q71] 查看建表语句
来源：http://kzg.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yjn.jinyuanbaomall.cn

[Q72] 查看索引
来源：http://zde.tarul.cn

SHOW INDEX FROM users;
来源：http://jbu.chenjidiqi.icu

[Q73] 查看表状态
来源：http://iiv.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nua.uphjek.com

[Q74] 强制使用索引
来源：http://fbn.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jwy.c1oappe.top

[Q75] 日期格式化
来源：http://gjc.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aed.jqgfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://naw.xziqi.cn

[Q76] 按天统计
来源：http://ppa.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tcl.cqqwz.cn

[Q77] 时间加减
来源：http://ppt.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fjo.yj20258.top

[Q78] 当前时间
来源：http://rps.zhixingplan.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zzf.hcnkem.com

[Q79] 字符串拼接
来源：http://smh.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pld.fktsv.cn

[Q80] 字符串截取
来源：http://bna.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bhu.sysykeji.top

[Q81] 字符串替换
来源：http://rta.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qdg.fktsv.cn

[Q82] 字符长度与字节长度
来源：http://dev.jianghu66.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fze.tanke756.top

[Q83] 大小写转换
来源：http://yms.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bix.yangfankeji.com

[Q84] 去除首尾空格
来源：http://yww.cqqwz.cn

SELECT TRIM(name) FROM users;
来源：http://dlk.ppjwa.cn

[Q85] 数值取整
来源：http://zsl.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wwy.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://epf.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wux.daria6918.cn

[Q87] JSON 字段做条件
来源：http://div.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wib.uphjek.com

[Q88] 行转列（条件聚合）
来源：http://qbc.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xic.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ayu.daxiang520.top

[Q89] 判断表是否存在
来源：http://fde.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://roq.nanxinkj.top

[Q90] 生成序号列
来源：http://hoq.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uqm.ivvv.top

================================================================================
来源：http://gvj.daria6918.cn

R. Bash 专题
来源：http://qrz.hammf.cn

================================================================================
来源：http://cpd.xinyue.icu

[R01] shebang 与严格模式
来源：http://gmt.sweek.top

#!/usr/bin/env bash
来源：http://mji.sweek.top

set -euo pipefail
来源：http://kvk.daxiang520.top

[R02] 变量赋值与使用
来源：http://knd.svipenyu.cn

name="Tom"; echo "$name"
来源：http://kdg.jinyuanbaomall.cn

[R03] 只读变量
来源：http://bfw.birdmap.top

readonly PI=3.14
来源：http://xkz.xylfe.cn

[R04] 位置参数
来源：http://fxj.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://odq.fzhhl.top

[R05] 参数默认值
来源：http://xht.gzhubu.top

name="${1:-default}"
来源：http://ghq.zhixingplan.top

[R06] 判断命令是否存在
来源：http://cbu.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://for.pycfn.com

[R07] if 判断文件
来源：http://nos.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dbi.sjlbkw.cn

[R08] 数值比较
来源：http://phi.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cpi.cheryme.top

[R09] 字符串比较
来源：http://wit.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qnn.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://rry.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rqs.bbcook.cn

[R11] case 多分支
来源：http://xkv.jinghuilouyu.cn

case "$1" in
来源：http://inm.fehbvm.com

start) echo "启动" ;;
来源：http://fsu.jianghu66.top

stop)  echo "停止" ;;
来源：http://jin.sweek.top

*)     echo "未知命令" ;;
来源：http://wqy.pengpengdd.cyou

esac
来源：http://wzz.daxiang520.top

[R12] for 遍历文件
来源：http://qtc.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://fna.sufxvd.cn

[R13] for 计数循环
来源：http://ova.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://jdd.fanxiaobao.xyz

[R14] C 风格 for
来源：http://lgr.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wxz.epnwcf.com

[R15] while 逐行读文件
来源：http://fsx.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wqy.xziqi.cn

[R16] until 等待条件
来源：http://itt.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ihv.guowangkeji.top

[R17] 数组定义与取值
来源：http://ypt.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xct.mhx1999.top

[R18] 遍历数组
来源：http://wci.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bbt.jinqigfzy.top

[R19] 数组长度
来源：http://ppy.zhiwuduotai.top

echo "${#arr[@]}"
来源：http://uhn.hcnkem.com

[R20] 关联数组（字典）
来源：http://ijv.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kfb.vqdsnc.cn

[R21] 字符串长度
来源：http://jot.kuanghao11.cn

echo "${#s}"
来源：http://bjw.shuidangran.top

[R22] 截取子串
来源：http://qnk.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://att.quarkkingdee.top

[R23] 字符串替换
来源：http://gln.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://seq.sysykeji.top

[R24] 大小写转换
来源：http://avv.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://oiq.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://ytb.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bzc.sjlbkw.cn

[R26] 命令替换
来源：http://tix.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://pej.yj20258888.top

[R27] 算术展开
来源：http://crt.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://mhl.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://qbq.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://ght.wangshuangyany.cn

[R29] 定义函数
来源：http://avj.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nof.jqgfzy.top

[R30] 函数返回状态码
来源：http://ikh.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://yaj.tanke756.top

[R31] 局部变量
来源：http://buf.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://ame.yanxiufei.cn

[R32] 参数个数校验
来源：http://whu.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iay.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://ziv.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eld.zdqjudy.top

[R34] 退出时清理
来源：http://jun.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://sej.gzhubu.top

[R35] 后台执行并等待
来源：http://opr.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://paj.dianchejie.cn

[R36] 并发执行多个任务
来源：http://urd.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nvb.bjfxy.top

[R37] 把输出赋给变量
来源：http://rew.zhijiandao.cn

files=$(ls -1)
来源：http://deb.hfpthk.cn

[R38] 管道串联
来源：http://tcv.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://fyu.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://khu.birdmap.top

cmd > out.log 2>&1
来源：http://ecp.yuanzhike.top

[R40] 追加写日志
来源：http://uil.yonumen.top

echo "log" >> out.log
来源：http://fdh.hcnkem.com

[R41] 丢弃输出
来源：http://tzx.tian-w.cn

cmd >/dev/null 2>&1
来源：http://qej.jyoumei.cn

[R42] 输入重定向
来源：http://uye.52xcode.cn

wc -l < a.txt
来源：http://xiw.hywenlv.cn

[R43] 按名字查找文件
来源：http://cda.yvedp.cn

find . -name "*.log" -type f
来源：http://jmg.svipenyu.cn

[R44] 按修改时间查找
来源：http://pyr.hnqzz.top

find . -mtime -7 -type f
来源：http://xow.redwolf501.top

[R45] 批量删除
来源：http://wyw.epnwcf.com

find . -name "*.tmp" -delete
来源：http://tyx.hywenlv.cn

[R46] 递归替换文件内容
来源：http://pqx.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mzc.ppjwa.cn

[R47] sed 单行替换
来源：http://yzp.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://ljp.sysykeji.top

[R48] awk 取指定列
来源：http://zap.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://zss.fzhhl.top

[R49] awk 带条件
来源：http://gbn.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avy.smart0.xyz

[R50] awk 求和
来源：http://kgr.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://fom.jlsjyb.cn

[R51] 排序去重取前几
来源：http://oha.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cxm.yonumen.top

[R52] 统计行数
来源：http://fcd.mhx1999.top

wc -l a.txt
来源：http://hsm.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://sgx.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zry.ydzc1.top

[R54] 比较两个文件
来源：http://qoa.quarkkingdee.top

diff a.txt b.txt
来源：http://otd.epnwcf.com

[R55] 压缩与解压
来源：http://xjm.gogol.net.cn


<!-- 参考信息 -->