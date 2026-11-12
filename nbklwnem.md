代发 wailian999

PHP:  // 手写时间戳比较
来源：http://elb.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahw.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gdr.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jbk.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tqf.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wjo.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nyz.hesvh.cn

[P08] 处理浮点精度问题
来源：http://vus.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lde.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://phq.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sio.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://glt.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zmx.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ety.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://trq.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://joz.yj202588.top

================================================================================
来源：http://gua.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lme.daxiang520.top

================================================================================
来源：http://uid.hywenlv.cn

[Q01] 创建表
来源：http://aze.tarul.cn

CREATE TABLE users (
来源：http://qgm.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://glh.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://lqi.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://oql.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://idm.shangyingyoupin.top

);
来源：http://uwg.yonumen.top

[Q02] 创建带外键的表
来源：http://cng.bbcook.cn

CREATE TABLE orders (
来源：http://ksc.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cvf.zdbjq.cn

user_id INT NOT NULL,
来源：http://btq.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://acl.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yqk.xziqi.cn

);
来源：http://pbb.uphjek.com

[Q03] 增加列
来源：http://sku.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pcs.jianghu66.top

[Q04] 修改列类型
来源：http://qmy.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ktl.feifeiyinyue.top

[Q05] 重命名列
来源：http://ist.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gvd.shuidangran.top

[Q06] 删除列
来源：http://ajd.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://eat.gaohongyu789.top

[Q07] 删除表
来源：http://pfk.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://sik.316326.xyz

[Q08] 创建普通索引
来源：http://gmg.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://aig.aibaodan.cn

[Q09] 创建唯一索引
来源：http://kct.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tih.0kj1m.cn

[Q10] 插入单行
来源：http://bud.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tbo.chenzaomai.com

[Q11] 一次插入多行
来源：http://sav.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sau.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://fpk.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iww.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://byi.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://afr.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://agb.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://gcu.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xcl.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fsd.shanyushiyangtech.top

[Q15] 查询全部
来源：http://esd.cqqwz.cn

SELECT * FROM users;
来源：http://nej.hnqzz.top

[Q16] 查询指定列
来源：http://zqy.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://xxm.feifeiyinyue.top

[Q17] 条件查询
来源：http://isa.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nsf.gaohongyu789.top

[Q18] 模糊匹配
来源：http://lor.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cgk.hnxiangtu.top

[Q19] 范围查询
来源：http://onz.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hzc.fengsongda.top

[Q20] IN 列表
来源：http://lwp.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ome.chenlongwang.top

[Q21] 空值判断
来源：http://qyq.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pgd.smart0.xyz

[Q22] 排序
来源：http://brj.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vhw.jinqigfzy.top

[Q23] 分页
来源：http://bpr.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cyc.zhaomingkeji.xyz

[Q24] 去重
来源：http://wgc.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://edl.smart0.xyz

[Q25] 只取前 N 条
来源：http://kmd.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oth.52xcode.cn

[Q26] 计数
来源：http://iaa.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://utl.redwolf501.top

[Q27] 条件计数
来源：http://obr.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yyl.9152youxi.cn

[Q28] 求和与平均
来源：http://jqb.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wqn.epnwcf.com

[Q29] 最大最小值
来源：http://qbr.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bbg.gaohongyu789.top

[Q30] 分组统计
来源：http://ptp.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qey.zycfv.cn

[Q31] 分组后过滤
来源：http://qmn.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://smf.sxryk.cn

[Q32] 分组拼接字符串
来源：http://dea.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dhd.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dyj.316326.xyz

[Q33] 多列分组
来源：http://zrd.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tmx.fengsongda.top

[Q34] 每组取第一条
来源：http://tgs.fktsv.cn

SELECT * FROM (
来源：http://rtd.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ngm.sufxvd.cn

) t WHERE rn = 1;
来源：http://guv.daria6918.cn

[Q35] 内连接
来源：http://hbn.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dhp.daria6918.cn

[Q36] 左连接
来源：http://hzx.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uve.ydzc1.top

[Q37] 右连接
来源：http://lkm.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dpo.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://pqi.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rgq.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://zmg.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uka.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://moc.zhaomingkeji.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://jjt.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpd.mhx1999.top

[Q41] 多表连接
来源：http://rab.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fwo.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://ifa.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://gxy.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://uwf.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://gzf.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pjn.jiagoushi.top

[Q43] 标量子查询
来源：http://xfi.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aty.iojbl.cn

[Q44] IN 子查询
来源：http://mzh.chenlongwang.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iqk.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://iee.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfg.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://afi.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onu.vehdjk.com

[Q47] 与平均值比较
来源：http://fcu.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cxx.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://qxi.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mfn.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://nts.xuetiantiany.cn

[Q49] 更新单行
来源：http://vwt.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aeo.jinghuilouyu.cn

[Q50] 批量更新
来源：http://syq.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sov.ctjpmb.com

[Q51] 用子查询更新
来源：http://kpc.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gfa.jqgufenzy.top

[Q52] 删除指定行
来源：http://apt.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://iwl.wangshuangyany.cn

[Q53] 按条件删除
来源：http://gup.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mrt.fanxiaobao.xyz

[Q54] 清空表
来源：http://ebj.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://izg.cheryme.top

[Q55] 排名（并列占位）
来源：http://asu.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mqy.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://hdf.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zpr.hfpthk.cn

[Q57] 行号
来源：http://alz.xuetiantiany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://htw.sysykeji.top

[Q58] 累计求和
来源：http://smi.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://npp.jyoumei.cn

[Q59] 分组内累计
来源：http://qew.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ync.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://ecy.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ogy.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tvq.gaohongyu789.top

[Q61] 移动平均
来源：http://xvx.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://djr.hysaishi.cn

[Q62] 分组占比
来源：http://bne.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mcb.ivvv.top

[Q63] 开启事务
来源：http://brc.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://uxy.0kj1m.cn

[Q64] 提交事务
来源：http://yth.dianchejie.cn

COMMIT;
来源：http://vir.xylfe.cn

[Q65] 回滚事务
来源：http://rej.zdqjudy.top

ROLLBACK;
来源：http://dcz.hcnkem.com

[Q66] 行锁查询
来源：http://cuv.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bma.tian-w.cn

[Q67] 设置隔离级别
来源：http://dqc.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cfw.xuetiantiany.cn

[Q68] 保存点
来源：http://dmp.yuanzhike.top

SAVEPOINT sp1;
来源：http://wik.chenlongwang.top

ROLLBACK TO sp1;
来源：http://kaw.jinghuilouyu.cn

[Q69] 查看执行计划
来源：http://lqn.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xsq.sjlbkw.cn

[Q70] 更新统计信息
来源：http://qkj.yuxming.cn

ANALYZE TABLE users;
来源：http://won.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://kjq.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hof.wangdashe.top

[Q72] 查看索引
来源：http://dpp.hammf.cn

SHOW INDEX FROM users;
来源：http://vsv.zhoulong.xyz

[Q73] 查看表状态
来源：http://ojb.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://fbi.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://axp.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://drq.yuxming.cn

[Q75] 日期格式化
来源：http://ssm.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wtk.jinqigfzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ddo.zhoulong.xyz

[Q76] 按天统计
来源：http://lof.gzhubu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ach.jqgufenzy.top

[Q77] 时间加减
来源：http://gco.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yut.sysykeji.top

[Q78] 当前时间
来源：http://yfu.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vnz.jinqigfzy.top

[Q79] 字符串拼接
来源：http://rxl.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ihh.smart0.xyz

[Q80] 字符串截取
来源：http://kki.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lji.gaohongyu789.top

[Q81] 字符串替换
来源：http://sec.gzhubu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uqi.nanxuanxn.top

[Q82] 字符长度与字节长度
来源：http://oie.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xno.yuanzhike.top

[Q83] 大小写转换
来源：http://qfv.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://urp.jianghu66.top

[Q84] 去除首尾空格
来源：http://aoh.guannengcc.top

SELECT TRIM(name) FROM users;
来源：http://hpp.pengpengdd.cyou

[Q85] 数值取整
来源：http://jpl.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eye.daxiang520.top

[Q86] 读取 JSON 字段
来源：http://zhq.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bmr.zdqjudy.top

[Q87] JSON 字段做条件
来源：http://sxs.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fis.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://uxw.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://owi.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lby.fengsongda.top

[Q89] 判断表是否存在
来源：http://osg.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vmg.vehdjk.com

[Q90] 生成序号列
来源：http://ylj.316326.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uar.cqqwz.cn

================================================================================
来源：http://lds.fehbvm.com

R. Bash 专题
来源：http://amg.jlsjyb.cn

================================================================================
来源：http://rlf.cqqwz.cn

[R01] shebang 与严格模式
来源：http://qir.guannengcc.top

#!/usr/bin/env bash
来源：http://wby.ivvv.top

set -euo pipefail
来源：http://nsc.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://xrb.fzhhl.top

name="Tom"; echo "$name"
来源：http://bml.hcnkem.com

[R03] 只读变量
来源：http://zam.jiagoushi.top

readonly PI=3.14
来源：http://tbb.hywenlv.cn

[R04] 位置参数
来源：http://vxq.quarkkingdee.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktj.uphjek.com

[R05] 参数默认值
来源：http://zuc.zhijiandao.cn

name="${1:-default}"
来源：http://pwm.zhoulong.xyz

[R06] 判断命令是否存在
来源：http://aek.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uhv.uphjek.com

[R07] if 判断文件
来源：http://sqm.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cgs.hammf.cn

[R08] 数值比较
来源：http://vry.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://veo.svipenyu.cn

[R09] 字符串比较
来源：http://ttz.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvp.chenzaomai.com

[R10] 正则匹配
来源：http://bxj.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://soj.tian-w.cn

[R11] case 多分支
来源：http://qnh.zycfv.cn

case "$1" in
来源：http://ahf.hnxiangtu.top

start) echo "启动" ;;
来源：http://dzh.cashguo.top

stop)  echo "停止" ;;
来源：http://lao.andypj.xyz

*)     echo "未知命令" ;;
来源：http://wto.fengsongda.top

esac
来源：http://rmm.ehwqpu.com

[R12] for 遍历文件
来源：http://myz.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://llt.dianchejie.cn

[R13] for 计数循环
来源：http://oby.tian-w.cn

for i in {1..10}; do echo "$i"; done
来源：http://gwz.ppjwa.cn

[R14] C 风格 for
来源：http://lbi.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vzs.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://zsf.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vba.316326.xyz

[R16] until 等待条件
来源：http://ewr.zhixingplan.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xjp.yj202588.top

[R17] 数组定义与取值
来源：http://zbf.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://usn.zhiwuduotai.top

[R18] 遍历数组
来源：http://xun.xuanzx.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://edx.quarkkingdee.top

[R19] 数组长度
来源：http://bkb.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://zwm.wangdashe.top

[R20] 关联数组（字典）
来源：http://ukf.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qhb.daria6918.cn

[R21] 字符串长度
来源：http://uai.xuetiantiany.cn

echo "${#s}"
来源：http://ykp.ivvv.top

[R22] 截取子串
来源：http://ttq.gzhubu.top

echo "${s:0:5}"
来源：http://omg.ybcxt.top

[R23] 字符串替换
来源：http://xna.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xud.zhiwuduotai.top

[R24] 大小写转换
来源：http://xis.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://tix.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://lss.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://isc.jianghu66.top

[R26] 命令替换
来源：http://kkz.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://oyb.xuetiantiany.cn

[R27] 算术展开
来源：http://nlh.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://cus.zdbjq.cn

[R28] 浮点运算
来源：http://egy.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://huk.zhoulong.xyz

[R29] 定义函数
来源：http://eup.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ewy.svipenyu.cn

[R30] 函数返回状态码
来源：http://dlx.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://qig.cheryme.top

[R31] 局部变量
来源：http://xaq.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://xdn.cqqwz.cn

[R32] 参数个数校验
来源：http://ybv.mhx1999.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ntm.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://cxe.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ixf.tian-w.cn

[R34] 退出时清理
来源：http://qih.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://tap.pycfn.com

[R35] 后台执行并等待
来源：http://hij.hcnkem.com


<!-- 参考信息 -->