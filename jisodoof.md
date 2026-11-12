代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://lbi.vehdjk.com

[Q07] 删除表
来源：http://dhv.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://eqa.jlsjyb.cn

[Q08] 创建普通索引
来源：http://tdo.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vas.daxiang520.top

[Q09] 创建唯一索引
来源：http://jvp.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zdo.hongshengwenyu.top

[Q10] 插入单行
来源：http://nww.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://meb.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://jua.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pjr.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://yhw.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://raa.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rif.ivvv.top

[Q13] 忽略重复插入
来源：http://ngh.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://crz.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://nlv.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mxa.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eqi.xuetiantiany.cn

[Q15] 查询全部
来源：http://hte.jqgufenzy.top

SELECT * FROM users;
来源：http://ful.yfazqb.com

[Q16] 查询指定列
来源：http://qug.jlsjyb.cn

SELECT id, name FROM users;
来源：http://ajg.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://kqc.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://unh.haohaochexian.top

[Q18] 模糊匹配
来源：http://wjp.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wlg.52xcode.cn

[Q19] 范围查询
来源：http://fwn.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gxi.hongshengwenyu.top

[Q20] IN 列表
来源：http://npc.sxryk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjv.hywenlv.cn

[Q21] 空值判断
来源：http://wrb.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kom.52xcode.cn

[Q22] 排序
来源：http://kqx.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://emi.andypj.xyz

[Q23] 分页
来源：http://cxe.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://diq.smart0.xyz

[Q24] 去重
来源：http://edo.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://kvd.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://jix.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vog.cucudq.cn

[Q26] 计数
来源：http://gik.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://xli.meibo888.top

[Q27] 条件计数
来源：http://anh.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pwe.tian-w.cn

[Q28] 求和与平均
来源：http://erg.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wky.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://avf.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lkb.jiagoushi.top

[Q30] 分组统计
来源：http://dki.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yph.316326.xyz

[Q31] 分组后过滤
来源：http://opl.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ftb.yongpay.top

[Q32] 分组拼接字符串
来源：http://lpw.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qgr.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://khk.zhoulong.xyz

[Q33] 多列分组
来源：http://ccg.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ayw.jinqigfzy.top

[Q34] 每组取第一条
来源：http://njf.gotoacloud.top

SELECT * FROM (
来源：http://owk.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qkx.sufxvd.cn

) t WHERE rn = 1;
来源：http://rbq.jianghu66.top

[Q35] 内连接
来源：http://ibh.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ldb.feifeiyinyue.top

[Q36] 左连接
来源：http://sqd.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://suh.316326.xyz

[Q37] 右连接
来源：http://dev.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvn.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://cxs.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nmn.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://qdy.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xrz.mhx1999.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qot.hnqzz.top

[Q40] 交叉连接（笛卡尔积）
来源：http://chd.zycfv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bvi.hnqzz.top

[Q41] 多表连接
来源：http://rcr.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://euw.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://gxz.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://tbn.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://wdr.chenjidiqi.icu

SELECT u.name, o.amount FROM users u
来源：http://esu.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ech.zhongyouzk.top

[Q43] 标量子查询
来源：http://yuf.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ogr.yonumen.top

[Q44] IN 子查询
来源：http://vuo.xuanzx.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://euj.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://fgw.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aux.vehdjk.com

[Q46] NOT EXISTS 判断不存在
来源：http://snn.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eyt.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://irt.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://usv.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://rqv.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ahf.ydzc1.top

SELECT * FROM t WHERE c > 5;
来源：http://tpm.gaohongyu789.top

[Q49] 更新单行
来源：http://wcu.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iun.nanxinkj.top

[Q50] 批量更新
来源：http://jvd.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jvn.pycfn.com

[Q51] 用子查询更新
来源：http://fjv.meibo888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://etc.vehdjk.com

[Q52] 删除指定行
来源：http://ozt.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://kbg.sweek.top

[Q53] 按条件删除
来源：http://qtd.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qsj.shanyushiyangtech.top

[Q54] 清空表
来源：http://qfl.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://god.guannengcc.top

[Q55] 排名（并列占位）
来源：http://esz.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uah.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://erp.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fwr.gzhubu.top

[Q57] 行号
来源：http://ioj.yj20258888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xzb.yj202588.top

[Q58] 累计求和
来源：http://mzb.mhx1999.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lun.dianchejie.cn

[Q59] 分组内累计
来源：http://vtz.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gok.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://qbj.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://den.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qqf.tianlin.xyz

[Q61] 移动平均
来源：http://uwe.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pqn.xziqi.cn

[Q62] 分组占比
来源：http://zjp.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://boo.fzhhl.top

[Q63] 开启事务
来源：http://eqv.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://qdq.mhx1999.top

[Q64] 提交事务
来源：http://lqi.sjlbkw.cn

COMMIT;
来源：http://tys.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://qtv.hywenlv.cn

ROLLBACK;
来源：http://nsn.tarul.cn

[Q66] 行锁查询
来源：http://tkw.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jwv.tianlin.xyz

[Q67] 设置隔离级别
来源：http://vde.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ybq.andypj.xyz

[Q68] 保存点
来源：http://dxk.tanke756.top

SAVEPOINT sp1;
来源：http://wmg.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://ktx.vehdjk.com

[Q69] 查看执行计划
来源：http://izh.nanxinkj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxc.sufxvd.cn

[Q70] 更新统计信息
来源：http://hpx.cashguo.top

ANALYZE TABLE users;
来源：http://waf.fehbvm.com

[Q71] 查看建表语句
来源：http://syh.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cfg.vqdsnc.cn

[Q72] 查看索引
来源：http://efw.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://rqm.hnxiangtu.top

[Q73] 查看表状态
来源：http://nbh.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qzb.sufxvd.cn

[Q74] 强制使用索引
来源：http://dhq.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://irv.ydzc1.top

[Q75] 日期格式化
来源：http://dov.gzhubu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tdm.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://egm.hammf.cn

[Q76] 按天统计
来源：http://fyu.iojbl.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pzn.jlsjyb.cn

[Q77] 时间加减
来源：http://eip.xuetiantiany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://els.wangdashe.top

[Q78] 当前时间
来源：http://axh.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hiu.hnxiangtu.top

[Q79] 字符串拼接
来源：http://dnn.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rtr.ydzc1.top

[Q80] 字符串截取
来源：http://ehr.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pqj.yonumen.top

[Q81] 字符串替换
来源：http://nup.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yog.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://cto.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rge.nanxinkj.top

[Q83] 大小写转换
来源：http://qwp.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eeg.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://ean.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://bou.ppjwa.cn

[Q85] 数值取整
来源：http://uhn.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vgt.cashguo.top

[Q86] 读取 JSON 字段
来源：http://yyh.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://liy.xziqi.cn

[Q87] JSON 字段做条件
来源：http://lwr.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sjc.yj202588.top

[Q88] 行转列（条件聚合）
来源：http://bgz.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://azm.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vmn.meibo888.top

[Q89] 判断表是否存在
来源：http://rva.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://prx.yongpay.top

[Q90] 生成序号列
来源：http://slz.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://twz.pengpengdd.cyou

================================================================================
来源：http://mha.fengsongda.top

R. Bash 专题
来源：http://yah.xingfuxueyuan.xyz

================================================================================
来源：http://jpt.hfpthk.cn

[R01] shebang 与严格模式
来源：http://pdi.daxiang520.top

#!/usr/bin/env bash
来源：http://tdf.yfazqb.com

set -euo pipefail
来源：http://tpw.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://dej.yj202588.top

name="Tom"; echo "$name"
来源：http://buo.hesvh.cn

[R03] 只读变量
来源：http://xdu.hammf.cn

readonly PI=3.14
来源：http://rpa.tian-w.cn

[R04] 位置参数
来源：http://szv.cqqwz.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://svu.zycfv.cn

[R05] 参数默认值
来源：http://paz.sjlbkw.cn

name="${1:-default}"
来源：http://pib.shuidangran.top

[R06] 判断命令是否存在
来源：http://oqs.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ajg.pengpengdd.cyou

[R07] if 判断文件
来源：http://emz.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ncb.sweek.top

[R08] 数值比较
来源：http://pyd.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fve.xinyue.icu

[R09] 字符串比较
来源：http://rwe.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rxh.yangfankeji.com

[R10] 正则匹配
来源：http://ytu.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gcg.xziqi.cn

[R11] case 多分支
来源：http://npu.shanyushiyangtech.top

case "$1" in
来源：http://nek.fehbvm.com

start) echo "启动" ;;
来源：http://xxa.hywenlv.cn

stop)  echo "停止" ;;
来源：http://mie.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://bgk.yj20258888.top

esac
来源：http://ftm.xziqi.cn

[R12] for 遍历文件
来源：http://kff.52xcode.cn

for f in *.txt; do echo "$f"; done
来源：http://imk.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://mse.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://oqj.haohaochexian.top

[R14] C 风格 for
来源：http://kgo.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wgy.tianlin.xyz

[R15] while 逐行读文件
来源：http://ucv.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tue.zhixingplan.top

[R16] until 等待条件
来源：http://pez.zhaomingkeji.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cif.zhongyouzk.top

[R17] 数组定义与取值
来源：http://vmg.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://nqm.smart0.xyz

[R18] 遍历数组
来源：http://azn.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qcj.zhixingplan.top

[R19] 数组长度
来源：http://qpu.ydjk.org.cn

echo "${#arr[@]}"
来源：http://lrz.xinyue.icu

[R20] 关联数组（字典）
来源：http://jfz.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kvk.tian-w.cn

[R21] 字符串长度
来源：http://vli.aizwys.cn

echo "${#s}"
来源：http://jah.fehbvm.com

[R22] 截取子串
来源：http://isb.fzhhl.top

echo "${s:0:5}"
来源：http://mwx.dashuyun.cn

[R23] 字符串替换
来源：http://ohx.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tdj.daria6918.cn

[R24] 大小写转换
来源：http://kjn.yj20258888.top

echo "${s^^}"; echo "${s,,}"
来源：http://log.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://fsh.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ydc.wangshuangyany.cn

[R26] 命令替换
来源：http://osz.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://smu.hongshengwenyu.top

[R27] 算术展开
来源：http://icd.yfazqb.com

echo $((1 + 2 * 3))
来源：http://kpt.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://vsu.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://zwi.jlsjyb.cn

[R29] 定义函数
来源：http://axf.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://evg.fehbvm.com

[R30] 函数返回状态码
来源：http://gmi.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://ayo.shanyushiyangtech.top

[R31] 局部变量
来源：http://yqe.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://aix.hesvh.cn

[R32] 参数个数校验
来源：http://ulr.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ewe.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://pzs.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ehy.jlsjyb.cn

[R34] 退出时清理
来源：http://nvy.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tkn.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://cbr.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://evq.yfazqb.com

[R36] 并发执行多个任务
来源：http://qmy.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vmo.zdbjq.cn

[R37] 把输出赋给变量
来源：http://hbc.jinghuilouyu.cn

files=$(ls -1)
来源：http://eao.shanyushiyangkeji.top

[R38] 管道串联
来源：http://rlv.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://cmm.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://cko.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://wyu.yangfankeji.com

[R40] 追加写日志
来源：http://fdx.dianchejie.cn

echo "log" >> out.log
来源：http://exs.fehbvm.com

[R41] 丢弃输出
来源：http://ctl.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://pjq.yonumen.top

[R42] 输入重定向
来源：http://akv.fktsv.cn

wc -l < a.txt
来源：http://ajx.0kj1m.cn

[R43] 按名字查找文件
来源：http://bis.gotoacloud.top

find . -name "*.log" -type f
来源：http://atq.zdqjudy.top

[R44] 按修改时间查找
来源：http://yks.sweek.top

find . -mtime -7 -type f
来源：http://pqv.yuxming.cn

[R45] 批量删除
来源：http://vpr.ivvv.top

find . -name "*.tmp" -delete
来源：http://npr.shuidangran.top

[R46] 递归替换文件内容
来源：http://mfi.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ixd.pengpengdd.cyou

[R47] sed 单行替换
来源：http://efj.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mlf.dashuyun.cn

[R48] awk 取指定列
来源：http://cvb.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://kky.jyoumei.cn

[R49] awk 带条件
来源：http://cgs.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://srd.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://bdy.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://yhe.svipenyu.cn

[R51] 排序去重取前几
来源：http://ocj.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iuf.zhiwuduotai.top

[R52] 统计行数
来源：http://qws.fzhhl.top

wc -l a.txt
来源：http://qmq.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://ulc.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vfu.fzhhl.top

[R54] 比较两个文件
来源：http://wrz.pycfn.com

diff a.txt b.txt
来源：http://jvl.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://kyh.aizwys.cn


<!-- 参考信息 -->