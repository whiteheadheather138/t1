代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jeh.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lif.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qdu.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iyy.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wbn.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dng.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yjt.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vlr.yangfankeji.com

================================================================================
来源：http://pdu.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://asa.birdmap.top

================================================================================
来源：http://jkk.yonumen.top

[Q01] 创建表
来源：http://wud.yanxiufei.cn

CREATE TABLE users (
来源：http://qdf.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tlx.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://srk.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://gkp.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dxp.zdqjudy.top

);
来源：http://pej.guowangkeji.top

[Q02] 创建带外键的表
来源：http://smv.yfazqb.com

CREATE TABLE orders (
来源：http://roe.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xit.birdmap.top

user_id INT NOT NULL,
来源：http://scb.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://vrb.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://etz.cashguo.top

);
来源：http://inn.hfpthk.cn

[Q03] 增加列
来源：http://giy.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lus.gaohongyu789.top

[Q04] 修改列类型
来源：http://ooc.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://amn.zhongyouzk.top

[Q05] 重命名列
来源：http://upe.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sgv.xuetiantiany.cn

[Q06] 删除列
来源：http://loe.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vva.yangfankeji.com

[Q07] 删除表
来源：http://dqb.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://shu.yanxiufei.cn

[Q08] 创建普通索引
来源：http://hoi.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tle.ivvv.top

[Q09] 创建唯一索引
来源：http://hsi.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fxp.jlsjyb.cn

[Q10] 插入单行
来源：http://eye.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kba.cucudq.cn

[Q11] 一次插入多行
来源：http://kop.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcl.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://oza.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://wny.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://apg.shuidangran.top

[Q13] 忽略重复插入
来源：http://mas.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://veh.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://jrn.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xdc.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sex.vehdjk.com

[Q15] 查询全部
来源：http://gta.yj20258.top

SELECT * FROM users;
来源：http://tes.pengpengdd.cyou

[Q16] 查询指定列
来源：http://gng.xziqi.cn

SELECT id, name FROM users;
来源：http://nii.yj20258888.top

[Q17] 条件查询
来源：http://tqm.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vnl.bjfxy.top

[Q18] 模糊匹配
来源：http://cna.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xzp.sweek.top

[Q19] 范围查询
来源：http://dzk.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ags.uphjek.com

[Q20] IN 列表
来源：http://rzq.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rmf.zhiwuduotai.top

[Q21] 空值判断
来源：http://kre.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ahy.sjlbkw.cn

[Q22] 排序
来源：http://rnj.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vxn.zhongyouzk.top

[Q23] 分页
来源：http://okp.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://taa.epnwcf.com

[Q24] 去重
来源：http://eru.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://sit.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://yve.sweek.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://req.hammf.cn

[Q26] 计数
来源：http://ltu.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://kbj.zhongyouzk.top

[Q27] 条件计数
来源：http://vfe.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://edl.yueranfly.top

[Q28] 求和与平均
来源：http://azg.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jtc.hfpthk.cn

[Q29] 最大最小值
来源：http://ghn.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ypa.jiagoushi.top

[Q30] 分组统计
来源：http://lyt.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vuz.smart0.xyz

[Q31] 分组后过滤
来源：http://dbu.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wvl.xuanzx.com

[Q32] 分组拼接字符串
来源：http://hfd.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kzd.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://whv.sjlbkw.cn

[Q33] 多列分组
来源：http://tli.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rxz.sufxvd.cn

[Q34] 每组取第一条
来源：http://yzb.sweek.top

SELECT * FROM (
来源：http://ddi.0kj1m.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nxy.nwbrower.top

) t WHERE rn = 1;
来源：http://dpo.chenjidiqi.icu

[Q35] 内连接
来源：http://elh.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dkk.hcnkem.com

[Q36] 左连接
来源：http://eac.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kxb.andypj.xyz

[Q37] 右连接
来源：http://csy.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://keb.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://acs.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jip.hammf.cn

[Q39] 自连接（查上下级）
来源：http://zjy.sxryk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lxs.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ina.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qbd.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tvk.xinyue.icu

[Q41] 多表连接
来源：http://tjq.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zym.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://jyb.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://zpj.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://pwq.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://wsq.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bio.ctjpmb.com

[Q43] 标量子查询
来源：http://fvg.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mvy.kuanghao11.cn

[Q44] IN 子查询
来源：http://xno.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kfu.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://mmg.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dlg.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://juy.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppt.cashguo.top

[Q47] 与平均值比较
来源：http://aty.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://crf.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://wna.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opx.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://vpg.bbcook.cn

[Q49] 更新单行
来源：http://cgc.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fkw.xuetiantiany.cn

[Q50] 批量更新
来源：http://afy.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://slm.haohaochexian.top

[Q51] 用子查询更新
来源：http://jlh.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jov.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://mly.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://dsj.smart0.xyz

[Q53] 按条件删除
来源：http://tew.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jra.aizwys.cn

[Q54] 清空表
来源：http://bdw.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://lfg.52xcode.cn

[Q55] 排名（并列占位）
来源：http://zfh.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tgr.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://jeh.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://azb.zhoulong.xyz

[Q57] 行号
来源：http://txe.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ecy.snrcjt.cn

[Q58] 累计求和
来源：http://pvl.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ryj.sufxvd.cn

[Q59] 分组内累计
来源：http://jzl.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhn.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://nyt.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tzq.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xdi.hysaishi.cn

[Q61] 移动平均
来源：http://ith.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ebb.yj202588.top

[Q62] 分组占比
来源：http://ytp.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zvn.cheryme.top

[Q63] 开启事务
来源：http://lld.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://avq.uphjek.com

[Q64] 提交事务
来源：http://adj.zhaomingkeji.xyz

COMMIT;
来源：http://epc.wangdashe.top

[Q65] 回滚事务
来源：http://ngu.wangdashe.top

ROLLBACK;
来源：http://ngk.tanke756.top

[Q66] 行锁查询
来源：http://nqc.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fzr.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://jou.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ndm.vehdjk.com

[Q68] 保存点
来源：http://ozw.yanxiufei.cn

SAVEPOINT sp1;
来源：http://out.sysykeji.top

ROLLBACK TO sp1;
来源：http://ogy.sweek.top

[Q69] 查看执行计划
来源：http://wem.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dag.gotoacloud.top

[Q70] 更新统计信息
来源：http://zqa.daxiang520.top

ANALYZE TABLE users;
来源：http://haj.cqqwz.cn

[Q71] 查看建表语句
来源：http://iyv.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pgs.zhongyouzk.top

[Q72] 查看索引
来源：http://rvs.yvedp.cn

SHOW INDEX FROM users;
来源：http://pgw.zhoulong.xyz

[Q73] 查看表状态
来源：http://ddl.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://txr.0kj1m.cn

[Q74] 强制使用索引
来源：http://oey.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fjf.quarkkingdee.top

[Q75] 日期格式化
来源：http://kcs.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wti.hnxiangtu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qhh.xuanzx.com

[Q76] 按天统计
来源：http://ndo.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ehk.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://hud.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dbc.chenlongwang.top

[Q78] 当前时间
来源：http://qod.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ftn.pycfn.com

[Q79] 字符串拼接
来源：http://soy.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://omi.gotoacloud.top

[Q80] 字符串截取
来源：http://qbh.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yeo.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://ddo.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dwm.jinyuanbaomall.cn

[Q82] 字符长度与字节长度
来源：http://dqx.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jpd.zdbjq.cn

[Q83] 大小写转换
来源：http://qmf.shuidangran.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://enx.9152youxi.cn

[Q84] 去除首尾空格
来源：http://alf.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://zsc.gotoacloud.top

[Q85] 数值取整
来源：http://dou.tarul.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fbm.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://zji.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mzu.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://ctb.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xgs.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://icy.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://frf.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nzs.aibaodan.cn

[Q89] 判断表是否存在
来源：http://ukq.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ema.gogol.net.cn

[Q90] 生成序号列
来源：http://ehn.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aew.chenlongwang.top

================================================================================
来源：http://rvz.shuidangran.top

R. Bash 专题
来源：http://sew.hongshengwenyu.top

================================================================================
来源：http://frw.hywenlv.cn

[R01] shebang 与严格模式
来源：http://qtp.aizwys.cn

#!/usr/bin/env bash
来源：http://dbh.52xcode.cn

set -euo pipefail
来源：http://fye.yj20258.top

[R02] 变量赋值与使用
来源：http://qff.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://hdq.sufxvd.cn

[R03] 只读变量
来源：http://mmb.cucudq.cn

readonly PI=3.14
来源：http://bsd.jianghu66.top

[R04] 位置参数
来源：http://ktz.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sgo.guannengcc.top

[R05] 参数默认值
来源：http://vip.zhoulong.xyz

name="${1:-default}"
来源：http://rjz.zdqjudy.top

[R06] 判断命令是否存在
来源：http://pxy.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdp.fktsv.cn

[R07] if 判断文件
来源：http://arc.gaohongyu789.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hee.hesvh.cn

[R08] 数值比较
来源：http://hdl.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://swg.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://pfj.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zap.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://pbs.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://asl.haohaochexian.top

[R11] case 多分支
来源：http://mgh.fanxiaobao.xyz

case "$1" in
来源：http://wae.smart0.xyz

start) echo "启动" ;;
来源：http://oug.sxryk.cn

stop)  echo "停止" ;;
来源：http://csp.cheryme.top

*)     echo "未知命令" ;;
来源：http://eyw.yuanzhike.top

esac
来源：http://llv.meibo888.top

[R12] for 遍历文件
来源：http://pqa.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://jqk.guowangkeji.top

[R13] for 计数循环
来源：http://xsm.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://jhq.zdbjq.cn

[R14] C 风格 for
来源：http://hro.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lcc.andypj.xyz

[R15] while 逐行读文件
来源：http://fjs.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://glc.cqqwz.cn

[R16] until 等待条件
来源：http://olo.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cfm.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://kvq.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ofz.yongpay.top

[R18] 遍历数组
来源：http://qmb.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uds.jlsjyb.cn

[R19] 数组长度
来源：http://rku.zhongyouzk.top

echo "${#arr[@]}"
来源：http://clr.gotoacloud.top

[R20] 关联数组（字典）
来源：http://bbx.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fkk.nanxinkj.top

[R21] 字符串长度
来源：http://wpy.gogol.net.cn

echo "${#s}"
来源：http://ggb.jqgfzy.top

[R22] 截取子串
来源：http://rpw.hongshengwenyu.top

echo "${s:0:5}"
来源：http://spm.ydjk.org.cn

[R23] 字符串替换
来源：http://mxs.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://imk.fehbvm.com

[R24] 大小写转换
来源：http://svj.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ppd.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://lmz.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ssr.fanxiaobao.xyz

[R26] 命令替换
来源：http://rjj.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://rso.jqgufenzy.top

[R27] 算术展开
来源：http://yxi.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://yvd.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://xkl.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://weo.daria6918.cn

[R29] 定义函数
来源：http://evl.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iuv.52xcode.cn

[R30] 函数返回状态码
来源：http://bvg.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://jdv.sjlbkw.cn

[R31] 局部变量
来源：http://ejs.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://fwq.xinyue.icu

[R32] 参数个数校验
来源：http://chi.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jse.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://cnt.tanke756.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dri.snrcjt.cn

[R34] 退出时清理
来源：http://hzy.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eel.ydzc1.top

[R35] 后台执行并等待
来源：http://nea.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://pwj.hnqzz.top

[R36] 并发执行多个任务
来源：http://tle.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://usu.ybcxt.top

[R37] 把输出赋给变量
来源：http://lyc.nwbrower.top

files=$(ls -1)
来源：http://dsh.52xcode.cn

[R38] 管道串联
来源：http://ffw.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://epx.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://yfp.dashuyun.cn


<!-- 参考信息 -->