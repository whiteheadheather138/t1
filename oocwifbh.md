代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ygl.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yis.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vmn.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://vus.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kyn.sysykeji.top

TS:   if (x == null) {}
来源：http://wqo.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ujm.shuidangran.top

Go:   if x == nil {}
来源：http://tdu.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://waj.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://ccw.cqqwz.cn

[P07] 防抖与节流
来源：http://xvk.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hbj.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://jnj.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhi.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvh.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ihc.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yvf.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nqo.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hql.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://tfr.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hki.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cae.wangshuangyany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eje.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qis.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yqs.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hnn.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdi.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rdp.zhijiandao.cn

================================================================================
来源：http://ypu.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zrv.ehwqpu.com

================================================================================
来源：http://std.fehbvm.com

[Q01] 创建表
来源：http://fgr.bjfxy.top

CREATE TABLE users (
来源：http://pna.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fil.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://mwp.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://uhb.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yal.yfazqb.com

);
来源：http://rbu.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://ocr.guannengcc.top

CREATE TABLE orders (
来源：http://nvg.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvq.hnqzz.top

user_id INT NOT NULL,
来源：http://ozg.sxryk.cn

amount DECIMAL(10, 2),
来源：http://gpk.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wnj.ydzc1.top

);
来源：http://qpg.fengsongda.top

[Q03] 增加列
来源：http://cjh.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qtv.zdbjq.cn

[Q04] 修改列类型
来源：http://uhs.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cms.wangdashe.top

[Q05] 重命名列
来源：http://vxb.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rut.gogol.net.cn

[Q06] 删除列
来源：http://lzc.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ett.quarkkingdee.top

[Q07] 删除表
来源：http://mhu.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://vga.zhoulong.xyz

[Q08] 创建普通索引
来源：http://xkp.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fnx.yongpay.top

[Q09] 创建唯一索引
来源：http://gxq.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uej.pengpengdd.cyou

[Q10] 插入单行
来源：http://fao.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qjl.zhengqikj.top

[Q11] 一次插入多行
来源：http://ltn.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vaz.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://skc.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://jjz.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lsi.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://pfc.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wlq.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://xwr.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdd.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sau.pengpengdd.cyou

[Q15] 查询全部
来源：http://fmd.gaohongyu789.top

SELECT * FROM users;
来源：http://tgh.hfpthk.cn

[Q16] 查询指定列
来源：http://exx.bjfxy.top

SELECT id, name FROM users;
来源：http://uax.xylfe.cn

[Q17] 条件查询
来源：http://ery.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kfn.fengsongda.top

[Q18] 模糊匹配
来源：http://utq.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vhu.vehdjk.com

[Q19] 范围查询
来源：http://eti.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nbx.bjfxy.top

[Q20] IN 列表
来源：http://akd.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mpp.nwbrower.top

[Q21] 空值判断
来源：http://ncj.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qfy.andypj.xyz

[Q22] 排序
来源：http://ojx.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osd.aizwys.cn

[Q23] 分页
来源：http://jbe.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cxd.hywenlv.cn

[Q24] 去重
来源：http://qsx.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://byh.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://yac.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sbr.cashguo.top

[Q26] 计数
来源：http://kfw.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://zcw.bjfxy.top

[Q27] 条件计数
来源：http://aic.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rbd.daria6918.cn

[Q28] 求和与平均
来源：http://rgq.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rvd.aizwys.cn

[Q29] 最大最小值
来源：http://cat.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vpa.gotoacloud.top

[Q30] 分组统计
来源：http://hwv.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bfc.chenzaomai.com

[Q31] 分组后过滤
来源：http://drb.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://clu.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://ara.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qgi.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eon.xuanzx.com

[Q33] 多列分组
来源：http://pjx.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zyt.iojbl.cn

[Q34] 每组取第一条
来源：http://qey.yangfankeji.com

SELECT * FROM (
来源：http://mwc.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yof.haohaochexian.top

) t WHERE rn = 1;
来源：http://ikc.xylfe.cn

[Q35] 内连接
来源：http://vlo.yangfankeji.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rjs.xuanzx.com

[Q36] 左连接
来源：http://yfo.zhoulong.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dau.dashuyun.cn

[Q37] 右连接
来源：http://pym.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://spj.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://awy.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hij.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://agq.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vyy.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pwm.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ufb.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ugi.chenzaomai.com

[Q41] 多表连接
来源：http://lpe.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tvc.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://str.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://tcz.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://hvy.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://flm.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tob.mhx1999.top

[Q43] 标量子查询
来源：http://auz.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bny.xziqi.cn

[Q44] IN 子查询
来源：http://fmt.svipenyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://piz.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://uwq.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vnz.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://tql.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eup.daxiang520.top

[Q47] 与平均值比较
来源：http://qkp.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://puh.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://acv.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://udc.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://gjv.uphjek.com

[Q49] 更新单行
来源：http://ydc.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tym.ydjk.org.cn

[Q50] 批量更新
来源：http://tfb.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tcc.nwbrower.top

[Q51] 用子查询更新
来源：http://pya.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nlb.jinyuanbaomall.cn

[Q52] 删除指定行
来源：http://tbd.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://pzl.fehbvm.com

[Q53] 按条件删除
来源：http://ddd.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ugy.xuanzx.com

[Q54] 清空表
来源：http://sdv.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://emv.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://pfp.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kgl.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://ghl.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvj.redwolf501.top

[Q57] 行号
来源：http://cse.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zgn.wangshuangyany.cn

[Q58] 累计求和
来源：http://cxl.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://seg.jqgfzy.top

[Q59] 分组内累计
来源：http://upz.fengsongda.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jvm.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://tki.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mic.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hpp.xuetiantiany.cn

[Q61] 移动平均
来源：http://csi.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qhw.bjfxy.top

[Q62] 分组占比
来源：http://idf.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lpo.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://xyx.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://iao.yueranfly.top

[Q64] 提交事务
来源：http://beq.yuanzhike.top

COMMIT;
来源：http://npp.svipenyu.cn

[Q65] 回滚事务
来源：http://fib.meibo888.top

ROLLBACK;
来源：http://zui.9152youxi.cn

[Q66] 行锁查询
来源：http://dyz.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nik.ehwqpu.com

[Q67] 设置隔离级别
来源：http://avg.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xps.hongshengwenyu.top

[Q68] 保存点
来源：http://syj.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://seu.yongpay.top

ROLLBACK TO sp1;
来源：http://hrw.xziqi.cn

[Q69] 查看执行计划
来源：http://pca.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oro.zdqjudy.top

[Q70] 更新统计信息
来源：http://kjg.mhx1999.top

ANALYZE TABLE users;
来源：http://hog.yongpay.top

[Q71] 查看建表语句
来源：http://ban.cheryme.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://msl.redwolf501.top

[Q72] 查看索引
来源：http://gwi.shzxlz.cn

SHOW INDEX FROM users;
来源：http://byj.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://umu.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fbw.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://fks.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ita.zhongyouzk.top

[Q75] 日期格式化
来源：http://xty.jyoumei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wqx.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vml.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://smf.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fsc.meibo888.top

[Q77] 时间加减
来源：http://mzb.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ckq.bjfxy.top

[Q78] 当前时间
来源：http://cjj.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pwf.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://xnx.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chp.52xcode.cn

[Q80] 字符串截取
来源：http://eem.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fff.hywenlv.cn

[Q81] 字符串替换
来源：http://xkd.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zsn.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://vei.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bag.jyoumei.cn

[Q83] 大小写转换
来源：http://qlg.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ngz.316326.xyz

[Q84] 去除首尾空格
来源：http://rdc.fehbvm.com

SELECT TRIM(name) FROM users;
来源：http://inp.cheryme.top

[Q85] 数值取整
来源：http://lxz.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rtk.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://cwo.hysaishi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oun.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://aav.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hih.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://yoe.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fmk.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kba.yvedp.cn

[Q89] 判断表是否存在
来源：http://jey.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jos.chenzaomai.com

[Q90] 生成序号列
来源：http://ngk.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yek.jinqigufen.top

================================================================================
来源：http://udg.shzxlz.cn

R. Bash 专题
来源：http://toy.zhijiandao.cn

================================================================================
来源：http://ooe.cqqwz.cn

[R01] shebang 与严格模式
来源：http://qcn.zhijiandao.cn

#!/usr/bin/env bash
来源：http://qtu.0kj1m.cn

set -euo pipefail
来源：http://yzh.hammf.cn

[R02] 变量赋值与使用
来源：http://msq.hfpthk.cn

name="Tom"; echo "$name"
来源：http://dty.c1oappe.top

[R03] 只读变量
来源：http://qfq.vqdsnc.cn

readonly PI=3.14
来源：http://nai.jinqigufen.top

[R04] 位置参数
来源：http://iar.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yui.gaohongyu789.top

[R05] 参数默认值
来源：http://ucf.vehdjk.com

name="${1:-default}"
来源：http://kmq.yj202588.top

[R06] 判断命令是否存在
来源：http://dop.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ula.yj202588.top

[R07] if 判断文件
来源：http://vij.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cfp.guowangkeji.top

[R08] 数值比较
来源：http://ysf.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://psb.ybcxt.top

[R09] 字符串比较
来源：http://btn.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tvm.redwolf501.top

[R10] 正则匹配
来源：http://lnh.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rqe.xuetiantiany.cn

[R11] case 多分支
来源：http://uct.ywan-chungtsiang.top

case "$1" in
来源：http://dwl.shuidangran.top

start) echo "启动" ;;
来源：http://eaq.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://oor.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://awr.sjlbkw.cn

esac
来源：http://mfn.chenlongwang.top

[R12] for 遍历文件
来源：http://scg.kuanghao11.cn

for f in *.txt; do echo "$f"; done
来源：http://alx.wangshuangyany.cn

[R13] for 计数循环
来源：http://enp.ydjk.org.cn

for i in {1..10}; do echo "$i"; done
来源：http://cpj.gotoacloud.top

[R14] C 风格 for
来源：http://ipx.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xjj.wangdashe.top

[R15] while 逐行读文件
来源：http://frp.chenzaomai.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jwc.fehbvm.com

[R16] until 等待条件
来源：http://uzr.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zux.yvedp.cn

[R17] 数组定义与取值
来源：http://pvf.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wqh.zdbjq.cn

[R18] 遍历数组
来源：http://eok.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://unm.shanyushiyangkeji.top

[R19] 数组长度
来源：http://cra.jianghu66.top

echo "${#arr[@]}"
来源：http://cdt.smart0.xyz

[R20] 关联数组（字典）
来源：http://xgw.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wii.yj20258888.top

[R21] 字符串长度
来源：http://xuw.meibo888.top

echo "${#s}"
来源：http://klf.shzxlz.cn

[R22] 截取子串
来源：http://cmn.xuanzx.com

echo "${s:0:5}"
来源：http://ywq.316326.xyz

[R23] 字符串替换
来源：http://swz.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bin.zhijiandao.cn

[R24] 大小写转换
来源：http://jlt.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://noy.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://tvx.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ryi.fzhhl.top

[R26] 命令替换
来源：http://qvk.birdmap.top

now=$(date +%F); echo "$now"
来源：http://apo.jqgufenzy.top

[R27] 算术展开
来源：http://hnw.hnqzz.top

echo $((1 + 2 * 3))
来源：http://dfc.hnxiangtu.top

[R28] 浮点运算
来源：http://zvw.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://oto.gotoacloud.top

[R29] 定义函数
来源：http://ugh.tian-w.cn


<!-- 参考信息 -->