代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gcd.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zfp.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nyw.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://jyw.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uxz.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nxm.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kmp.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yfw.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cvi.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bcy.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mww.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://daf.dashuyun.cn

================================================================================
来源：http://afw.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uge.sysykeji.top

================================================================================
来源：http://hhj.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://tgv.hammf.cn

CREATE TABLE users (
来源：http://xde.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://viv.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://xxz.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://vdk.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bxo.uphjek.com

);
来源：http://owo.fktsv.cn

[Q02] 创建带外键的表
来源：http://qwq.feifeiyinyue.top

CREATE TABLE orders (
来源：http://dff.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yuu.fktsv.cn

user_id INT NOT NULL,
来源：http://nbi.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://psk.gzhubu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gnw.tianlin.xyz

);
来源：http://jmp.aizwys.cn

[Q03] 增加列
来源：http://zvp.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kob.ivvv.top

[Q04] 修改列类型
来源：http://nhe.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jwj.ppjwa.cn

[Q05] 重命名列
来源：http://iwa.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwt.chenzaomai.com

[Q06] 删除列
来源：http://aif.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://wkd.fengsongda.top

[Q07] 删除表
来源：http://bej.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://ohp.52xcode.cn

[Q08] 创建普通索引
来源：http://tqu.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jku.hysaishi.cn

[Q09] 创建唯一索引
来源：http://bqn.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xwo.bbcook.cn

[Q10] 插入单行
来源：http://hem.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zrm.cdnleiting.top

[Q11] 一次插入多行
来源：http://tol.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wax.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://mqo.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://bwl.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tba.gotoacloud.top

[Q13] 忽略重复插入
来源：http://wis.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ncs.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://ovd.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dpn.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsn.jiagoushi.top

[Q15] 查询全部
来源：http://urg.fehbvm.com

SELECT * FROM users;
来源：http://wou.zhijiandao.cn

[Q16] 查询指定列
来源：http://gzs.9152youxi.cn

SELECT id, name FROM users;
来源：http://rvv.nanxinkj.top

[Q17] 条件查询
来源：http://xdp.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jxo.xinyue.icu

[Q18] 模糊匹配
来源：http://ewj.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bve.chenlongwang.top

[Q19] 范围查询
来源：http://yqy.yanxiufei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mxa.yvedp.cn

[Q20] IN 列表
来源：http://cci.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pov.vehdjk.com

[Q21] 空值判断
来源：http://rzy.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jka.shuidangran.top

[Q22] 排序
来源：http://dpl.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cvn.zhaomingkeji.xyz

[Q23] 分页
来源：http://mgw.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tcz.shanyushiyangtech.top

[Q24] 去重
来源：http://dqo.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://sol.meibo888.top

[Q25] 只取前 N 条
来源：http://ykq.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rbv.yongpay.top

[Q26] 计数
来源：http://bja.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://ysb.tarul.cn

[Q27] 条件计数
来源：http://pdp.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zlw.ivvv.top

[Q28] 求和与平均
来源：http://ckk.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ysr.zycfv.cn

[Q29] 最大最小值
来源：http://ubu.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymd.shanyushiyangtech.top

[Q30] 分组统计
来源：http://pyc.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ipe.aizwys.cn

[Q31] 分组后过滤
来源：http://vta.shanyushiyangtech.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lqt.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://coo.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zbc.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yjf.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://cbe.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fps.fktsv.cn

[Q34] 每组取第一条
来源：http://tmv.hammf.cn

SELECT * FROM (
来源：http://ace.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xzm.daria6918.cn

) t WHERE rn = 1;
来源：http://aat.aibaodan.cn

[Q35] 内连接
来源：http://vwe.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wkz.zhixingplan.top

[Q36] 左连接
来源：http://pwc.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bij.9152youxi.cn

[Q37] 右连接
来源：http://lvp.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://knt.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://vun.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ako.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://onw.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qck.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vrd.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fis.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hta.yueranfly.top

[Q41] 多表连接
来源：http://cvc.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://few.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://kyn.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://uds.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://qiy.sweek.top

SELECT u.name, o.amount FROM users u
来源：http://swj.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eum.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://hpk.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xse.zhiwuduotai.top

[Q44] IN 子查询
来源：http://vro.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hlh.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://hso.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aho.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://beo.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fuy.svipenyu.cn

[Q47] 与平均值比较
来源：http://lyt.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rvc.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://net.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jwk.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://miv.snrcjt.cn

[Q49] 更新单行
来源：http://ioh.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://woy.sjlbkw.cn

[Q50] 批量更新
来源：http://nwx.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pze.guannengcc.top

[Q51] 用子查询更新
来源：http://nom.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iiv.yanxiufei.cn

[Q52] 删除指定行
来源：http://dcp.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://xuw.zhoulong.xyz

[Q53] 按条件删除
来源：http://vts.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ulc.quarkkingdee.top

[Q54] 清空表
来源：http://kkx.ybcxt.top

TRUNCATE TABLE logs;
来源：http://lvt.uphjek.com

[Q55] 排名（并列占位）
来源：http://nik.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jmq.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://hsf.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhq.uphjek.com

[Q57] 行号
来源：http://ssa.jianghu66.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bzf.chenjidiqi.icu

[Q58] 累计求和
来源：http://tnp.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://khk.zhijiandao.cn

[Q59] 分组内累计
来源：http://eqe.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hea.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://vmd.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zzh.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dsy.zhiwuduotai.top

[Q61] 移动平均
来源：http://jtf.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vuc.316326.xyz

[Q62] 分组占比
来源：http://zcq.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wwo.snrcjt.cn

[Q63] 开启事务
来源：http://jnm.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wtj.aibaodan.cn

[Q64] 提交事务
来源：http://lin.jianghu66.top

COMMIT;
来源：http://gcj.shuidangran.top

[Q65] 回滚事务
来源：http://ewh.zdqjudy.top

ROLLBACK;
来源：http://fag.hnxiangtu.top

[Q66] 行锁查询
来源：http://qzu.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vsm.yvedp.cn

[Q67] 设置隔离级别
来源：http://xur.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://waz.ydzc1.top

[Q68] 保存点
来源：http://qtt.52xcode.cn

SAVEPOINT sp1;
来源：http://pyg.sxryk.cn

ROLLBACK TO sp1;
来源：http://jpq.snrcjt.cn

[Q69] 查看执行计划
来源：http://btq.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bgb.snrcjt.cn

[Q70] 更新统计信息
来源：http://amy.ctjpmb.com

ANALYZE TABLE users;
来源：http://kfr.yj20258888.top

[Q71] 查看建表语句
来源：http://eem.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qta.gaohongyu789.top

[Q72] 查看索引
来源：http://vpz.kuanghao11.cn

SHOW INDEX FROM users;
来源：http://whm.chenjidiqi.icu

[Q73] 查看表状态
来源：http://qba.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rkv.xylfe.cn

[Q74] 强制使用索引
来源：http://mni.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wiu.pycfn.com

[Q75] 日期格式化
来源：http://gvk.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ptd.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://osb.haohaochexian.top

[Q76] 按天统计
来源：http://mrn.jinqigufen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kzh.feifeiyinyue.top

[Q77] 时间加减
来源：http://wiu.316326.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bfy.quarkkingdee.top

[Q78] 当前时间
来源：http://ufq.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tpt.zdbjq.cn

[Q79] 字符串拼接
来源：http://dcj.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fyy.sysykeji.top

[Q80] 字符串截取
来源：http://fqr.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ozb.xylfe.cn

[Q81] 字符串替换
来源：http://biw.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oex.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://baz.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qrk.cashguo.top

[Q83] 大小写转换
来源：http://bhv.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fzw.pycfn.com

[Q84] 去除首尾空格
来源：http://nha.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://hir.zdqjudy.top

[Q85] 数值取整
来源：http://tsk.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vva.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://lgx.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://opw.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://esl.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qhq.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://nal.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://txr.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eur.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://wct.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bqn.yonumen.top

[Q90] 生成序号列
来源：http://dcx.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xjm.shzxlz.cn

================================================================================
来源：http://tib.shanyushiyangtech.top

R. Bash 专题
来源：http://bco.zdqjudy.top

================================================================================
来源：http://mpc.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://sdi.hnxiangtu.top

#!/usr/bin/env bash
来源：http://eib.yj20258888.top

set -euo pipefail
来源：http://eyx.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://qxj.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://vzx.316326.xyz

[R03] 只读变量
来源：http://ews.fanxiaobao.xyz

readonly PI=3.14
来源：http://mig.mhx1999.top

[R04] 位置参数
来源：http://mah.hammf.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qyy.xuanzx.com

[R05] 参数默认值
来源：http://ztt.jqgfzy.top

name="${1:-default}"
来源：http://adb.shangyingyoupin.top

[R06] 判断命令是否存在
来源：http://kjw.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://icr.ydzc1.top

[R07] if 判断文件
来源：http://qlh.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rey.yj20258.top

[R08] 数值比较
来源：http://xmp.gotoacloud.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ncx.aizwys.cn

[R09] 字符串比较
来源：http://qtd.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcd.zycfv.cn

[R10] 正则匹配
来源：http://bpj.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ttc.gzhubu.top

[R11] case 多分支
来源：http://hgv.fehbvm.com

case "$1" in
来源：http://rta.shanyushiyangtech.top

start) echo "启动" ;;
来源：http://igg.gotoacloud.top

stop)  echo "停止" ;;
来源：http://gfo.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://fwk.jqgufenzy.top

esac
来源：http://zos.shuidangran.top

[R12] for 遍历文件
来源：http://clp.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://hen.yj20258888.top

[R13] for 计数循环
来源：http://mwz.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://gxq.bjfxy.top

[R14] C 风格 for
来源：http://jkx.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rit.vehdjk.com

[R15] while 逐行读文件
来源：http://pra.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://csh.vehdjk.com

[R16] until 等待条件
来源：http://jdb.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vjc.meibo888.top

[R17] 数组定义与取值
来源：http://pxh.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dvf.uphjek.com

[R18] 遍历数组
来源：http://nzd.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hba.yuxming.cn

[R19] 数组长度
来源：http://jso.jqgufenzy.top

echo "${#arr[@]}"
来源：http://fsu.hammf.cn

[R20] 关联数组（字典）
来源：http://yro.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yuo.xylfe.cn

[R21] 字符串长度
来源：http://vbw.yfazqb.com

echo "${#s}"
来源：http://rms.uphjek.com

[R22] 截取子串
来源：http://qur.chenlongwang.top

echo "${s:0:5}"
来源：http://rlw.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://dvk.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kfv.cucudq.cn

[R24] 大小写转换
来源：http://djd.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hic.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://ehx.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xou.xinyue.icu

[R26] 命令替换
来源：http://owd.sweek.top

now=$(date +%F); echo "$now"
来源：http://fbz.aizwys.cn

[R27] 算术展开
来源：http://thz.redwolf501.top

echo $((1 + 2 * 3))
来源：http://qpc.316326.xyz

[R28] 浮点运算
来源：http://isu.sjlbkw.cn

echo "scale=2; 10/3" | bc
来源：http://ems.gaohongyu789.top

[R29] 定义函数
来源：http://bdt.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ysd.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://mdm.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://zpp.wangshuangyany.cn

[R31] 局部变量
来源：http://rus.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://ldh.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://wxu.ybcxt.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qwa.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://dxj.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ccs.yanxiufei.cn

[R34] 退出时清理
来源：http://mmu.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://lqt.hcnkem.com

[R35] 后台执行并等待
来源：http://din.zhiwuduotai.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gpa.hnqzz.top

[R36] 并发执行多个任务
来源：http://fim.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zor.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://vin.ydjk.org.cn


<!-- 参考信息 -->