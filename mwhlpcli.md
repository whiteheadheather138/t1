代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://xvv.sysykeji.top

Go:   len(arr);  len(m)
来源：http://akr.cucudq.cn

Ruby: x.length;  x.size
来源：http://eeg.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jwb.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://bvv.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mii.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sob.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pry.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zbb.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lbw.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://wwi.yanxiufei.cn

Ruby: a == b
来源：http://anf.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hoi.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mph.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yac.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://wqc.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bcc.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://bta.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://clk.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://qur.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rkg.sjlbkw.cn

C#:   if (x is null) {}
来源：http://ksu.andypj.xyz

[P07] 防抖与节流
来源：http://wfi.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evn.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://kss.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hkq.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryh.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kvy.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fyz.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vox.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tuo.uphjek.com

[P08] 处理浮点精度问题
来源：http://rci.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wut.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mys.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xzh.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jht.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ifj.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gtq.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fkz.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zte.tianlin.xyz

================================================================================
来源：http://kax.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cob.shzxlz.cn

================================================================================
来源：http://gtg.jinyuanbaomall.cn

[Q01] 创建表
来源：http://rbf.aibaodan.cn

CREATE TABLE users (
来源：http://fmk.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xcj.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://ikv.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://rag.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mmy.gogol.net.cn

);
来源：http://ztw.zdbjq.cn

[Q02] 创建带外键的表
来源：http://hdj.meibo888.top

CREATE TABLE orders (
来源：http://ver.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqy.jinqigufen.top

user_id INT NOT NULL,
来源：http://mlx.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://gqr.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xct.pycfn.com

);
来源：http://mcg.shanyushiyangtech.top

[Q03] 增加列
来源：http://ext.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wih.ydzc1.top

[Q04] 修改列类型
来源：http://aez.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gbj.birdmap.top

[Q05] 重命名列
来源：http://nun.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tih.dashuyun.cn

[Q06] 删除列
来源：http://evv.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hby.nanxinkj.top

[Q07] 删除表
来源：http://egm.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://sdg.sxryk.cn

[Q08] 创建普通索引
来源：http://jrz.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sfc.wangdashe.top

[Q09] 创建唯一索引
来源：http://fsl.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://opf.havefunace.top

[Q10] 插入单行
来源：http://asg.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dou.zhixingplan.top

[Q11] 一次插入多行
来源：http://baz.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eka.nwbrower.top

[Q12] 插入后取自增 ID
来源：http://lfn.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://tep.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tqc.sweek.top

[Q13] 忽略重复插入
来源：http://ypw.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bhk.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://vuy.cucudq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://chz.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mrq.jiagoushi.top

[Q15] 查询全部
来源：http://cxt.hammf.cn

SELECT * FROM users;
来源：http://rwu.sjlbkw.cn

[Q16] 查询指定列
来源：http://cbp.cheryme.top

SELECT id, name FROM users;
来源：http://wdw.yongpay.top

[Q17] 条件查询
来源：http://fdi.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://off.aizwys.cn

[Q18] 模糊匹配
来源：http://ekl.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yhc.dianchejie.cn

[Q19] 范围查询
来源：http://xdn.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zsi.xylfe.cn

[Q20] IN 列表
来源：http://awd.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nwa.svipenyu.cn

[Q21] 空值判断
来源：http://wko.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bdu.yvedp.cn

[Q22] 排序
来源：http://spw.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xld.gotoacloud.top

[Q23] 分页
来源：http://leh.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iav.chenzaomai.com

[Q24] 去重
来源：http://xqe.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://zij.jianghu66.top

[Q25] 只取前 N 条
来源：http://riu.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lbn.zdbjq.cn

[Q26] 计数
来源：http://zfp.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://ecr.jyoumei.cn

[Q27] 条件计数
来源：http://prl.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yfd.hnqzz.top

[Q28] 求和与平均
来源：http://rgw.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zjh.sufxvd.cn

[Q29] 最大最小值
来源：http://zvo.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://phy.yfazqb.com

[Q30] 分组统计
来源：http://lmc.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nhf.jqgufenzy.top

[Q31] 分组后过滤
来源：http://xgp.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nmq.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://wwh.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aax.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://imn.andypj.xyz

[Q33] 多列分组
来源：http://mxz.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tii.cqqwz.cn

[Q34] 每组取第一条
来源：http://goq.cheryme.top

SELECT * FROM (
来源：http://uoo.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://omo.cashguo.top

) t WHERE rn = 1;
来源：http://ops.yueranfly.top

[Q35] 内连接
来源：http://ynn.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uka.wangshuangyany.cn

[Q36] 左连接
来源：http://msf.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dyv.cdnleiting.top

[Q37] 右连接
来源：http://rbq.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fkp.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mcv.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oyo.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://uvy.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jfh.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lwe.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://pvh.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lhh.52xcode.cn

[Q41] 多表连接
来源：http://meg.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dkm.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://rub.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://btv.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://bgk.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://pbv.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xkr.tanke756.top

[Q43] 标量子查询
来源：http://tof.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kxo.zhiwuduotai.top

[Q44] IN 子查询
来源：http://suc.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rnw.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://fsm.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://saq.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://qdk.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://osr.nanxuanxn.top

[Q47] 与平均值比较
来源：http://hjr.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dpi.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://rkq.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://edk.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://tht.birdmap.top

[Q49] 更新单行
来源：http://heo.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nsh.snrcjt.cn

[Q50] 批量更新
来源：http://dhw.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://atp.aizwys.cn

[Q51] 用子查询更新
来源：http://qbz.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rvq.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://jrq.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://ijd.pycfn.com

[Q53] 按条件删除
来源：http://bdz.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ztl.hnqzz.top

[Q54] 清空表
来源：http://mmb.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://mib.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://mbr.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fiq.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://cgb.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dgu.gotoacloud.top

[Q57] 行号
来源：http://wqr.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fnd.smart0.xyz

[Q58] 累计求和
来源：http://rzw.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bae.quarkkingdee.top

[Q59] 分组内累计
来源：http://ckp.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bdw.vehdjk.com

[Q60] 取上一行 / 下一行
来源：http://cba.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wqc.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gke.jinghuilouyu.cn

[Q61] 移动平均
来源：http://mza.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pdr.dashuyun.cn

[Q62] 分组占比
来源：http://prq.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://brl.jqgufenzy.top

[Q63] 开启事务
来源：http://foc.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cok.nwbrower.top

[Q64] 提交事务
来源：http://xah.cheryme.top

COMMIT;
来源：http://und.vqdsnc.cn

[Q65] 回滚事务
来源：http://yaz.jinghuilouyu.cn

ROLLBACK;
来源：http://jwc.ehwqpu.com

[Q66] 行锁查询
来源：http://jct.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qfg.daxiang520.top

[Q67] 设置隔离级别
来源：http://ubu.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yxn.shanyushiyangtech.top

[Q68] 保存点
来源：http://bxb.zdbjq.cn

SAVEPOINT sp1;
来源：http://hmj.c1oappe.top

ROLLBACK TO sp1;
来源：http://uef.nanxuanxn.top

[Q69] 查看执行计划
来源：http://qtt.fehbvm.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zny.zhixingplan.top

[Q70] 更新统计信息
来源：http://rqq.gzhubu.top

ANALYZE TABLE users;
来源：http://gna.xinyue.icu

[Q71] 查看建表语句
来源：http://hvo.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qng.snrcjt.cn

[Q72] 查看索引
来源：http://cii.pycfn.com

SHOW INDEX FROM users;
来源：http://zqk.shzxlz.cn

[Q73] 查看表状态
来源：http://swf.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ktm.tanke756.top

[Q74] 强制使用索引
来源：http://vxc.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xgw.jyoumei.cn

[Q75] 日期格式化
来源：http://ngj.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zpz.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pyl.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://hoi.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zqm.shangyingyoupin.top

[Q77] 时间加减
来源：http://axt.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://epe.hnxiangtu.top

[Q78] 当前时间
来源：http://ijp.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iul.vehdjk.com

[Q79] 字符串拼接
来源：http://qdv.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cjt.dashuyun.cn

[Q80] 字符串截取
来源：http://lrn.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dcu.hfpthk.cn

[Q81] 字符串替换
来源：http://ncg.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nsa.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://soq.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vth.wangshuangyany.cn

[Q83] 大小写转换
来源：http://zuq.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rzp.fehbvm.com

[Q84] 去除首尾空格
来源：http://rbz.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://wqn.zhijiandao.cn

[Q85] 数值取整
来源：http://nqc.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yui.yonumen.top

[Q86] 读取 JSON 字段
来源：http://nuz.fzhhl.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://htf.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://pft.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fjc.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://bps.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qqz.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://adh.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://pox.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xcj.daxiang520.top

[Q90] 生成序号列
来源：http://zsy.snrcjt.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xyg.gaohongyu789.top

================================================================================
来源：http://dfb.ppjwa.cn

R. Bash 专题
来源：http://gtz.ivvv.top

================================================================================
来源：http://lhw.yangfankeji.com

[R01] shebang 与严格模式
来源：http://yoa.hfpthk.cn

#!/usr/bin/env bash
来源：http://hpy.xingfuxueyuan.xyz

set -euo pipefail
来源：http://qea.daria6918.cn

[R02] 变量赋值与使用
来源：http://txn.redwolf501.top

name="Tom"; echo "$name"
来源：http://cjg.yj20258888.top

[R03] 只读变量
来源：http://rth.dianchejie.cn

readonly PI=3.14
来源：http://yef.cqqwz.cn

[R04] 位置参数
来源：http://iyw.jyoumei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ril.cucudq.cn

[R05] 参数默认值
来源：http://clc.yuanzhike.top

name="${1:-default}"
来源：http://bpa.hongshengwenyu.top

[R06] 判断命令是否存在
来源：http://fmu.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://twu.nanxinkj.top

[R07] if 判断文件
来源：http://rov.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tst.sweek.top

[R08] 数值比较
来源：http://hri.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bes.nwbrower.top

[R09] 字符串比较
来源：http://mcl.haohaochexian.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lbe.0kj1m.cn

[R10] 正则匹配
来源：http://ypk.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kjk.shuidangran.top

[R11] case 多分支
来源：http://gef.pengpengdd.cyou

case "$1" in
来源：http://jrl.xuetiantiany.cn

start) echo "启动" ;;
来源：http://xwk.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://kpr.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://dzj.svipenyu.cn

esac
来源：http://lwr.smart0.xyz

[R12] for 遍历文件
来源：http://pgd.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://mgq.tianlin.xyz

[R13] for 计数循环
来源：http://ilg.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://mrh.fanxiaobao.xyz

[R14] C 风格 for
来源：http://cxi.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sam.hysaishi.cn

[R15] while 逐行读文件
来源：http://ayy.52xcode.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zoc.epnwcf.com

[R16] until 等待条件
来源：http://ovf.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wos.guowangkeji.top

[R17] 数组定义与取值
来源：http://mjv.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://ucf.cucudq.cn

[R18] 遍历数组
来源：http://vih.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oae.gogol.net.cn

[R19] 数组长度
来源：http://wlr.tianlin.xyz

echo "${#arr[@]}"
来源：http://det.yuxming.cn

[R20] 关联数组（字典）
来源：http://yvb.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nsr.yvedp.cn

[R21] 字符串长度
来源：http://uan.hysaishi.cn

echo "${#s}"
来源：http://qzn.zhaomingkeji.xyz

[R22] 截取子串
来源：http://uxd.uphjek.com

echo "${s:0:5}"
来源：http://ufo.epnwcf.com

[R23] 字符串替换
来源：http://cua.ehwqpu.com


<!-- 参考信息 -->