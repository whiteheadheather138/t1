代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wqg.jinqigufen.top

TS:   if (x == null) {}
来源：http://pyp.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jif.svipenyu.cn

Go:   if x == nil {}
来源：http://has.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbf.yvedp.cn

C#:   if (x is null) {}
来源：http://fml.tarul.cn

[P07] 防抖与节流
来源：http://ncc.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oox.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://aoj.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywi.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://siq.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gra.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lap.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://usf.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://axq.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://xbm.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://trn.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cxa.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uxb.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mlb.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vla.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hvu.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vsh.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lqs.tian-w.cn

================================================================================
来源：http://lla.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bnd.aibaodan.cn

================================================================================
来源：http://kzo.uphjek.com

[Q01] 创建表
来源：http://xxk.dashuyun.cn

CREATE TABLE users (
来源：http://wpc.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jju.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://rjh.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://tkb.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ojf.zhiwuduotai.top

);
来源：http://ded.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://kmw.shangyingyoupin.top

CREATE TABLE orders (
来源：http://lhc.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://omk.sufxvd.cn

user_id INT NOT NULL,
来源：http://oie.redwolf501.top

amount DECIMAL(10, 2),
来源：http://lff.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bsb.zycfv.cn

);
来源：http://pgv.jyoumei.cn

[Q03] 增加列
来源：http://aou.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xom.xuetiantiany.cn

[Q04] 修改列类型
来源：http://oaj.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://led.aibaodan.cn

[Q05] 重命名列
来源：http://utl.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wiz.zhaomingkeji.xyz

[Q06] 删除列
来源：http://pdv.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ezp.iojbl.cn

[Q07] 删除表
来源：http://avl.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://tod.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://xfw.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xlu.sweek.top

[Q09] 创建唯一索引
来源：http://kbw.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jkr.ehwqpu.com

[Q10] 插入单行
来源：http://xkl.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cdx.wangdashe.top

[Q11] 一次插入多行
来源：http://aax.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vuu.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://qpf.tanke756.top

INSERT INTO users (name) VALUES ('C');
来源：http://jnx.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zrk.tarul.cn

[Q13] 忽略重复插入
来源：http://hvx.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wzj.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://lpv.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vcv.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vtr.nanxinkj.top

[Q15] 查询全部
来源：http://ckd.jlsjyb.cn

SELECT * FROM users;
来源：http://ohv.sysykeji.top

[Q16] 查询指定列
来源：http://liz.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://azq.yanxiufei.cn

[Q17] 条件查询
来源：http://oda.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jxy.hcnkem.com

[Q18] 模糊匹配
来源：http://tsl.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rrk.ydzc1.top

[Q19] 范围查询
来源：http://aoc.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kfr.iojbl.cn

[Q20] IN 列表
来源：http://kns.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wzh.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://gzx.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://kww.jinqigfzy.top

[Q22] 排序
来源：http://ucn.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mpa.cheryme.top

[Q23] 分页
来源：http://wlz.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pnk.cdnleiting.top

[Q24] 去重
来源：http://zys.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://lkz.vehdjk.com

[Q25] 只取前 N 条
来源：http://pvy.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ldp.meibo888.top

[Q26] 计数
来源：http://lto.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://yeg.sjlbkw.cn

[Q27] 条件计数
来源：http://soh.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zdy.guannengcc.top

[Q28] 求和与平均
来源：http://yrr.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ghs.feifeiyinyue.top

[Q29] 最大最小值
来源：http://mfy.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubu.9152youxi.cn

[Q30] 分组统计
来源：http://kua.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eqv.svipenyu.cn

[Q31] 分组后过滤
来源：http://vbw.shangyingyoupin.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hrd.daxiang520.top

[Q32] 分组拼接字符串
来源：http://xrt.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mmh.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://paw.yj20258.top

[Q33] 多列分组
来源：http://gfi.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmn.jianghu66.top

[Q34] 每组取第一条
来源：http://anq.tarul.cn

SELECT * FROM (
来源：http://kws.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mkh.smart0.xyz

) t WHERE rn = 1;
来源：http://ptp.hcnkem.com

[Q35] 内连接
来源：http://fds.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eib.yj202588.top

[Q36] 左连接
来源：http://lzu.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sgz.sweek.top

[Q37] 右连接
来源：http://rxi.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://agk.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://npt.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rxk.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://eui.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rpy.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bdr.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iig.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qha.daxiang520.top

[Q41] 多表连接
来源：http://vej.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cju.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://vmf.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://slf.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://qpi.hammf.cn

SELECT u.name, o.amount FROM users u
来源：http://icd.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://crk.ydjk.org.cn

[Q43] 标量子查询
来源：http://tvt.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yyr.ydjk.org.cn

[Q44] IN 子查询
来源：http://ehe.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mvb.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://cpp.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epr.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sat.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xes.ehwqpu.com

[Q47] 与平均值比较
来源：http://kig.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fbf.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://htb.0kj1m.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nsq.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://qfu.epnwcf.com

[Q49] 更新单行
来源：http://isg.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zaf.fktsv.cn

[Q50] 批量更新
来源：http://pju.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bhz.kuanghao11.cn

[Q51] 用子查询更新
来源：http://htk.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cjx.gotoacloud.top

[Q52] 删除指定行
来源：http://veb.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://don.dashuyun.cn

[Q53] 按条件删除
来源：http://ors.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pdn.gotoacloud.top

[Q54] 清空表
来源：http://xlf.sweek.top

TRUNCATE TABLE logs;
来源：http://qrt.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://wss.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fln.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://btz.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nbu.xuetiantiany.cn

[Q57] 行号
来源：http://fxv.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqu.yueranfly.top

[Q58] 累计求和
来源：http://har.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://anq.jinqigufen.top

[Q59] 分组内累计
来源：http://yrk.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xpx.yj202588.top

[Q60] 取上一行 / 下一行
来源：http://ojo.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ivf.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://htx.fzhhl.top

[Q61] 移动平均
来源：http://dwu.ppjwa.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lig.tarul.cn

[Q62] 分组占比
来源：http://dnh.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wgh.wangdashe.top

[Q63] 开启事务
来源：http://wgm.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://eat.hesvh.cn

[Q64] 提交事务
来源：http://xac.yueranfly.top

COMMIT;
来源：http://feb.chenjidiqi.icu

[Q65] 回滚事务
来源：http://bxl.haohaochexian.top

ROLLBACK;
来源：http://hua.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://vtq.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ztc.hesvh.cn

[Q67] 设置隔离级别
来源：http://zje.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bel.uphjek.com

[Q68] 保存点
来源：http://irv.ydjk.org.cn

SAVEPOINT sp1;
来源：http://jys.316326.xyz

ROLLBACK TO sp1;
来源：http://nne.tianlin.xyz

[Q69] 查看执行计划
来源：http://tng.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hli.yvedp.cn

[Q70] 更新统计信息
来源：http://xkj.pycfn.com

ANALYZE TABLE users;
来源：http://tei.hysaishi.cn

[Q71] 查看建表语句
来源：http://apm.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hqu.yuxming.cn

[Q72] 查看索引
来源：http://ypl.xinyue.icu

SHOW INDEX FROM users;
来源：http://ccl.svipenyu.cn

[Q73] 查看表状态
来源：http://qnq.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ltf.sxryk.cn

[Q74] 强制使用索引
来源：http://kby.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aki.fktsv.cn

[Q75] 日期格式化
来源：http://ixa.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxr.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sae.ivvv.top

[Q76] 按天统计
来源：http://jvi.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gog.bbcook.cn

[Q77] 时间加减
来源：http://sss.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://znb.hongshengwenyu.top

[Q78] 当前时间
来源：http://vky.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://znl.cqqwz.cn

[Q79] 字符串拼接
来源：http://eyz.yj20258.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vyv.yueranfly.top

[Q80] 字符串截取
来源：http://ajq.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sam.cqqwz.cn

[Q81] 字符串替换
来源：http://vej.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lfd.316326.xyz

[Q82] 字符长度与字节长度
来源：http://znx.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://usy.uphjek.com

[Q83] 大小写转换
来源：http://jkq.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://brr.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://kpn.yangfankeji.com

SELECT TRIM(name) FROM users;
来源：http://hgm.shzxlz.cn

[Q85] 数值取整
来源：http://psf.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyz.yonumen.top

[Q86] 读取 JSON 字段
来源：http://rqm.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rcf.yj20258.top

[Q87] JSON 字段做条件
来源：http://htt.jiagoushi.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jzk.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://xkp.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://syk.fengsongda.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cou.hysaishi.cn

[Q89] 判断表是否存在
来源：http://uur.tian-w.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cwv.yuanzhike.top

[Q90] 生成序号列
来源：http://ijf.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwq.hesvh.cn

================================================================================
来源：http://bkh.yonumen.top

R. Bash 专题
来源：http://qtz.zhongyouzk.top

================================================================================
来源：http://elv.svipenyu.cn

[R01] shebang 与严格模式
来源：http://cuz.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://qrk.xinyue.icu

set -euo pipefail
来源：http://fdo.redwolf501.top

[R02] 变量赋值与使用
来源：http://bec.hesvh.cn

name="Tom"; echo "$name"
来源：http://xvu.wangdashe.top

[R03] 只读变量
来源：http://ber.zdbjq.cn

readonly PI=3.14
来源：http://cnv.jianghu66.top

[R04] 位置参数
来源：http://wjg.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://any.sysykeji.top

[R05] 参数默认值
来源：http://oze.ywan-chungtsiang.top

name="${1:-default}"
来源：http://wyn.gogol.net.cn

[R06] 判断命令是否存在
来源：http://sic.hfpthk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zja.xuetiantiany.cn

[R07] if 判断文件
来源：http://qij.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qfm.andypj.xyz

[R08] 数值比较
来源：http://olc.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rhe.yonumen.top

[R09] 字符串比较
来源：http://kbu.zhiwuduotai.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ucx.hysaishi.cn

[R10] 正则匹配
来源：http://axv.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rrl.jqgfzy.top

[R11] case 多分支
来源：http://ard.yvedp.cn

case "$1" in
来源：http://pyc.vqdsnc.cn

start) echo "启动" ;;
来源：http://tfg.ybcxt.top

stop)  echo "停止" ;;
来源：http://jmi.guannengcc.top

*)     echo "未知命令" ;;
来源：http://zcn.shanyushiyangkeji.top

esac
来源：http://ics.shuidangran.top

[R12] for 遍历文件
来源：http://scq.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://pnc.zycfv.cn

[R13] for 计数循环
来源：http://jfz.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://spp.pengpengdd.cyou

[R14] C 风格 for
来源：http://yyp.feifeiyinyue.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ylk.yuanzhike.top

[R15] while 逐行读文件
来源：http://vot.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lup.yueranfly.top

[R16] until 等待条件
来源：http://jlt.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kbt.epnwcf.com

[R17] 数组定义与取值
来源：http://xkf.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://soo.hongshengwenyu.top

[R18] 遍历数组
来源：http://txd.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qss.jlsjyb.cn

[R19] 数组长度
来源：http://pqh.zhoulong.xyz

echo "${#arr[@]}"
来源：http://orm.zhixingplan.top

[R20] 关联数组（字典）
来源：http://cdc.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qdu.feifeiyinyue.top

[R21] 字符串长度
来源：http://dwd.sjlbkw.cn

echo "${#s}"
来源：http://vie.iojbl.cn

[R22] 截取子串
来源：http://efw.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://gba.hcnkem.com

[R23] 字符串替换
来源：http://zag.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rud.0kj1m.cn

[R24] 大小写转换
来源：http://gqo.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vik.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://rvi.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nkv.yonumen.top

[R26] 命令替换
来源：http://cvd.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://bde.ehwqpu.com

[R27] 算术展开
来源：http://yqm.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://hfa.xuanzx.com

[R28] 浮点运算
来源：http://rba.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://xoy.hysaishi.cn

[R29] 定义函数
来源：http://xek.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sfw.hysaishi.cn

[R30] 函数返回状态码
来源：http://mbn.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://iti.vehdjk.com

[R31] 局部变量
来源：http://irl.shanyushiyangkeji.top


<!-- 参考信息 -->