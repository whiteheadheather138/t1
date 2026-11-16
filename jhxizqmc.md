代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jsc.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://muz.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tct.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://jsd.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uap.hysaishi.cn

TS:   if (x == null) {}
来源：http://wvp.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zto.zhixingplan.top

Go:   if x == nil {}
来源：http://irb.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfe.havefunace.top

C#:   if (x is null) {}
来源：http://yjl.guowangkeji.top

[P07] 防抖与节流
来源：http://siy.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pjr.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://fil.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxe.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ocn.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hvv.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sqk.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rcp.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ryq.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://gtl.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jpd.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ueu.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gut.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uin.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqp.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yll.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eif.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eux.yvedp.cn

================================================================================
来源：http://jwz.pengpengdd.cyou

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ook.jqgufenzy.top

================================================================================
来源：http://pam.xinyue.icu

[Q01] 创建表
来源：http://nnf.jqgfzy.top

CREATE TABLE users (
来源：http://fwv.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmu.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://jyc.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://kju.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tgs.zhengqikj.top

);
来源：http://oub.nwbrower.top

[Q02] 创建带外键的表
来源：http://ewv.hammf.cn

CREATE TABLE orders (
来源：http://vpw.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyy.shzxlz.cn

user_id INT NOT NULL,
来源：http://kky.yuxming.cn

amount DECIMAL(10, 2),
来源：http://ujp.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cvw.zycfv.cn

);
来源：http://vhq.kuanghao11.cn

[Q03] 增加列
来源：http://mvk.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://erc.hammf.cn

[Q04] 修改列类型
来源：http://vuw.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ftc.gzhubu.top

[Q05] 重命名列
来源：http://osa.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://omu.hongshengwenyu.top

[Q06] 删除列
来源：http://fcx.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://qkk.sysykeji.top

[Q07] 删除表
来源：http://ars.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://sxq.jinqigufen.top

[Q08] 创建普通索引
来源：http://jvs.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vfw.yueranfly.top

[Q09] 创建唯一索引
来源：http://ltb.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oms.vqdsnc.cn

[Q10] 插入单行
来源：http://iyx.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tcb.jiagoushi.top

[Q11] 一次插入多行
来源：http://itp.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://egx.birdmap.top

[Q12] 插入后取自增 ID
来源：http://nwp.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://cha.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mlj.cashguo.top

[Q13] 忽略重复插入
来源：http://ysw.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kxx.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://sle.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mbs.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jzv.kuanghao11.cn

[Q15] 查询全部
来源：http://bxu.nwbrower.top

SELECT * FROM users;
来源：http://eht.jlsjyb.cn

[Q16] 查询指定列
来源：http://wdk.cheryme.top

SELECT id, name FROM users;
来源：http://qpr.yj202588.top

[Q17] 条件查询
来源：http://ril.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rvs.bjfxy.top

[Q18] 模糊匹配
来源：http://xle.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blk.yangfankeji.com

[Q19] 范围查询
来源：http://aty.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gyi.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://tjo.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nlw.cheryme.top

[Q21] 空值判断
来源：http://aji.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yaa.zdqjudy.top

[Q22] 排序
来源：http://roc.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lrf.sysykeji.top

[Q23] 分页
来源：http://tjm.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rap.gogol.net.cn

[Q24] 去重
来源：http://xtx.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://mxb.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://cnc.cheryme.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aad.yongpay.top

[Q26] 计数
来源：http://kod.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://pdv.jqgufenzy.top

[Q27] 条件计数
来源：http://mbs.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ltg.yj20258.top

[Q28] 求和与平均
来源：http://ibw.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ysf.vqdsnc.cn

[Q29] 最大最小值
来源：http://yhr.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yac.cqqwz.cn

[Q30] 分组统计
来源：http://buh.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://loz.xuetiantiany.cn

[Q31] 分组后过滤
来源：http://dxg.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qgt.zycfv.cn

[Q32] 分组拼接字符串
来源：http://cci.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xwp.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zzp.zdqjudy.top

[Q33] 多列分组
来源：http://tyu.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://drg.yonumen.top

[Q34] 每组取第一条
来源：http://yws.aizwys.cn

SELECT * FROM (
来源：http://zvw.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ket.hysaishi.cn

) t WHERE rn = 1;
来源：http://jsl.yueranfly.top

[Q35] 内连接
来源：http://zmu.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kiq.tanke756.top

[Q36] 左连接
来源：http://sgx.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xdn.daria6918.cn

[Q37] 右连接
来源：http://csi.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvb.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://qvo.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rhx.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://shv.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://rwz.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dsd.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iwq.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wgj.mhx1999.top

[Q41] 多表连接
来源：http://zha.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cfg.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://hqz.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://swy.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://mne.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://utw.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lau.guannengcc.top

[Q43] 标量子查询
来源：http://kre.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jpk.yj20258888.top

[Q44] IN 子查询
来源：http://bfj.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fvh.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://hsf.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nmf.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://whx.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xxx.cucudq.cn

[Q47] 与平均值比较
来源：http://ozn.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ynv.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://wuk.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ycr.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://ari.sjlbkw.cn

[Q49] 更新单行
来源：http://rwv.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ghd.shanyushiyangkeji.top

[Q50] 批量更新
来源：http://xfm.xylfe.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sur.shzxlz.cn

[Q51] 用子查询更新
来源：http://jvi.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xsa.bjfxy.top

[Q52] 删除指定行
来源：http://yjc.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://upb.quarkkingdee.top

[Q53] 按条件删除
来源：http://gsi.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://enc.guannengcc.top

[Q54] 清空表
来源：http://ffc.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://jzn.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://xla.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wdm.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://kpq.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aye.sysykeji.top

[Q57] 行号
来源：http://buo.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iub.chenjidiqi.icu

[Q58] 累计求和
来源：http://kxe.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jvj.xuetiantiany.cn

[Q59] 分组内累计
来源：http://ibl.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://plz.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://fma.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yvo.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qij.bbcook.cn

[Q61] 移动平均
来源：http://kzd.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kyi.hammf.cn

[Q62] 分组占比
来源：http://wrd.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://why.hnxiangtu.top

[Q63] 开启事务
来源：http://ibt.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kub.bbcook.cn

[Q64] 提交事务
来源：http://zpk.yueranfly.top

COMMIT;
来源：http://tth.cheryme.top

[Q65] 回滚事务
来源：http://dzp.yongpay.top

ROLLBACK;
来源：http://jbd.jinqigfzy.top

[Q66] 行锁查询
来源：http://krn.wangdashe.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://obi.aizwys.cn

[Q67] 设置隔离级别
来源：http://qvn.jinqigufen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://udq.jlsjyb.cn

[Q68] 保存点
来源：http://uxc.redwolf501.top

SAVEPOINT sp1;
来源：http://ehl.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://nhb.yonumen.top

[Q69] 查看执行计划
来源：http://gbm.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rnn.yj20258888.top

[Q70] 更新统计信息
来源：http://tjv.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://pqu.ybcxt.top

[Q71] 查看建表语句
来源：http://acn.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://crr.guowangkeji.top

[Q72] 查看索引
来源：http://sfb.cucudq.cn

SHOW INDEX FROM users;
来源：http://nki.zhoulong.xyz

[Q73] 查看表状态
来源：http://aju.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dvk.chenzaomai.com

[Q74] 强制使用索引
来源：http://lgj.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ajj.zhiwuduotai.top

[Q75] 日期格式化
来源：http://stu.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ugg.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rop.jinqigfzy.top

[Q76] 按天统计
来源：http://pfy.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pnh.yfazqb.com

[Q77] 时间加减
来源：http://tjl.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dhh.aibaodan.cn

[Q78] 当前时间
来源：http://mde.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://eei.tian-w.cn

[Q79] 字符串拼接
来源：http://xix.ehwqpu.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pqx.fzhhl.top

[Q80] 字符串截取
来源：http://vms.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eke.ctjpmb.com

[Q81] 字符串替换
来源：http://bwb.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xxk.guowangkeji.top

[Q82] 字符长度与字节长度
来源：http://tct.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uwz.zhixingplan.top

[Q83] 大小写转换
来源：http://uao.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ljv.bjfxy.top

[Q84] 去除首尾空格
来源：http://eet.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://elt.uphjek.com

[Q85] 数值取整
来源：http://sgu.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vyl.bbcook.cn

[Q86] 读取 JSON 字段
来源：http://reh.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kld.shanyushiyangkeji.top

[Q87] JSON 字段做条件
来源：http://dzn.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fkq.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://aqc.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lpz.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://msg.aizwys.cn

[Q89] 判断表是否存在
来源：http://fdz.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qvi.shanyushiyangkeji.top

[Q90] 生成序号列
来源：http://svk.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ocx.ctjpmb.com

================================================================================
来源：http://rkg.yonumen.top

R. Bash 专题
来源：http://upb.nanxinkj.top

================================================================================
来源：http://zxx.dashuyun.cn

[R01] shebang 与严格模式
来源：http://kct.sjlbkw.cn

#!/usr/bin/env bash
来源：http://epn.zhaomingkeji.xyz

set -euo pipefail
来源：http://nyo.ivvv.top

[R02] 变量赋值与使用
来源：http://xlj.jianghu66.top

name="Tom"; echo "$name"
来源：http://nhh.gaohongyu789.top

[R03] 只读变量
来源：http://psh.nanxuanxn.top

readonly PI=3.14
来源：http://gig.vehdjk.com

[R04] 位置参数
来源：http://hnc.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lqa.wangdashe.top

[R05] 参数默认值
来源：http://mfk.fzhhl.top

name="${1:-default}"
来源：http://xkr.yj202588.top

[R06] 判断命令是否存在
来源：http://zuz.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dul.ehwqpu.com

[R07] if 判断文件
来源：http://xvq.jlsjyb.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gzg.yueranfly.top

[R08] 数值比较
来源：http://eac.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rad.hywenlv.cn

[R09] 字符串比较
来源：http://oug.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wto.zdbjq.cn

[R10] 正则匹配
来源：http://fut.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://raz.hysaishi.cn

[R11] case 多分支
来源：http://may.jyoumei.cn

case "$1" in
来源：http://ztc.cheryme.top

start) echo "启动" ;;
来源：http://pym.aibaodan.cn

stop)  echo "停止" ;;
来源：http://ygz.vehdjk.com

*)     echo "未知命令" ;;
来源：http://psi.yanxiufei.cn

esac
来源：http://mcf.tianlin.xyz

[R12] for 遍历文件
来源：http://byp.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://yjf.9152youxi.cn

[R13] for 计数循环
来源：http://lxy.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://dgo.haohaochexian.top

[R14] C 风格 for
来源：http://vag.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bky.aibaodan.cn

[R15] while 逐行读文件
来源：http://gnh.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ywr.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://yob.fehbvm.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wcw.guannengcc.top

[R17] 数组定义与取值
来源：http://tux.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://zam.shanyushiyangtech.top

[R18] 遍历数组
来源：http://gjc.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://viq.ydjk.org.cn

[R19] 数组长度
来源：http://sip.jinqigufen.top

echo "${#arr[@]}"
来源：http://vym.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://fky.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://icg.svipenyu.cn

[R21] 字符串长度
来源：http://uax.c1oappe.top

echo "${#s}"
来源：http://hob.pycfn.com

[R22] 截取子串
来源：http://jfi.bbcook.cn

echo "${s:0:5}"
来源：http://mrs.hcnkem.com

[R23] 字符串替换
来源：http://qli.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jlp.hnqzz.top

[R24] 大小写转换
来源：http://ulm.aibaodan.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fqx.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://pel.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hwk.sufxvd.cn

[R26] 命令替换
来源：http://pws.yj20258.top

now=$(date +%F); echo "$now"
来源：http://lju.gaohongyu789.top

[R27] 算术展开
来源：http://oxc.bbcook.cn

echo $((1 + 2 * 3))
来源：http://nmz.aizwys.cn

[R28] 浮点运算
来源：http://kwy.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://eex.yj202588.top

[R29] 定义函数
来源：http://rxx.zhaomingkeji.xyz


<!-- 参考信息 -->