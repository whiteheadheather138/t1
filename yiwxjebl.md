代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hbz.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://apy.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://gsb.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ocu.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://fno.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cxn.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wud.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bqw.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kzc.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mtq.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://slu.nwbrower.top

Ruby: a == b
来源：http://qhg.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nsb.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ebe.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gah.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://lcv.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hwl.tianlin.xyz

TS:   if (x == null) {}
来源：http://bzi.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oll.yongpay.top

Go:   if x == nil {}
来源：http://mej.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yoy.yj20258.top

C#:   if (x is null) {}
来源：http://xyk.fengsongda.top

[P07] 防抖与节流
来源：http://fln.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wxc.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://tdg.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dzz.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fjy.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ole.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wgw.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://grt.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tla.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://fxu.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uny.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gdf.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ips.yangfankeji.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://exo.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://arn.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ygy.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zyl.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jas.gaohongyu789.top

================================================================================
来源：http://kww.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qsc.zhongyouzk.top

================================================================================
来源：http://dtg.dianchejie.cn

[Q01] 创建表
来源：http://hmd.cqqwz.cn

CREATE TABLE users (
来源：http://kud.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qxu.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://anq.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://ulz.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hns.jinghuilouyu.cn

);
来源：http://fvz.sufxvd.cn

[Q02] 创建带外键的表
来源：http://qwj.gzhubu.top

CREATE TABLE orders (
来源：http://sxr.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfo.0kj1m.cn

user_id INT NOT NULL,
来源：http://wxa.jianghu66.top

amount DECIMAL(10, 2),
来源：http://aol.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fhg.zhijiandao.cn

);
来源：http://qdw.0kj1m.cn

[Q03] 增加列
来源：http://xzz.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qdw.daria6918.cn

[Q04] 修改列类型
来源：http://thn.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://img.tanke756.top

[Q05] 重命名列
来源：http://iaf.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://huj.yonumen.top

[Q06] 删除列
来源：http://niv.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hro.yongpay.top

[Q07] 删除表
来源：http://ytf.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://csh.ybcxt.top

[Q08] 创建普通索引
来源：http://qpq.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rhz.xziqi.cn

[Q09] 创建唯一索引
来源：http://cta.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aoc.nanxuanxn.top

[Q10] 插入单行
来源：http://myg.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://syj.birdmap.top

[Q11] 一次插入多行
来源：http://bzv.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xuk.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://nbe.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://yqa.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aae.cashguo.top

[Q13] 忽略重复插入
来源：http://nwv.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vtw.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://kzq.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nph.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yiq.pycfn.com

[Q15] 查询全部
来源：http://uhq.chenzaomai.com

SELECT * FROM users;
来源：http://clj.yanxiufei.cn

[Q16] 查询指定列
来源：http://vdh.snrcjt.cn

SELECT id, name FROM users;
来源：http://fja.quarkkingdee.top

[Q17] 条件查询
来源：http://twz.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xkq.aibaodan.cn

[Q18] 模糊匹配
来源：http://ytp.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wth.sxryk.cn

[Q19] 范围查询
来源：http://fmy.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iiv.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://gye.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lrc.ppjwa.cn

[Q21] 空值判断
来源：http://zkj.ybcxt.top

SELECT * FROM users WHERE email IS NULL;
来源：http://son.yuxming.cn

[Q22] 排序
来源：http://skk.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gwh.sjlbkw.cn

[Q23] 分页
来源：http://vsj.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzm.cqqwz.cn

[Q24] 去重
来源：http://puc.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://pzo.fengsongda.top

[Q25] 只取前 N 条
来源：http://zjq.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fgp.iojbl.cn

[Q26] 计数
来源：http://hob.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://yyl.smart0.xyz

[Q27] 条件计数
来源：http://vtl.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qos.hcnkem.com

[Q28] 求和与平均
来源：http://ydd.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wbd.guowangkeji.top

[Q29] 最大最小值
来源：http://gfq.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jne.c1oappe.top

[Q30] 分组统计
来源：http://keu.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kwa.daxiang520.top

[Q31] 分组后过滤
来源：http://chk.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xnl.xziqi.cn

[Q32] 分组拼接字符串
来源：http://fno.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://azd.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fyo.cheryme.top

[Q33] 多列分组
来源：http://vlv.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wpg.hfpthk.cn

[Q34] 每组取第一条
来源：http://gae.hammf.cn

SELECT * FROM (
来源：http://mrt.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qzu.havefunace.top

) t WHERE rn = 1;
来源：http://epn.quarkkingdee.top

[Q35] 内连接
来源：http://eeh.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jtb.fehbvm.com

[Q36] 左连接
来源：http://czx.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rhf.daxiang520.top

[Q37] 右连接
来源：http://dah.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wjv.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vyh.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pod.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://mlc.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fuw.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ert.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://svm.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://roe.yongpay.top

[Q41] 多表连接
来源：http://ktv.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pfh.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://fri.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://gks.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://gde.zhengqikj.top

SELECT u.name, o.amount FROM users u
来源：http://jow.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ipo.hammf.cn

[Q43] 标量子查询
来源：http://xol.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xrm.cashguo.top

[Q44] IN 子查询
来源：http://ncc.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xoi.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://soj.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yye.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sep.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hnd.sjlbkw.cn

[Q47] 与平均值比较
来源：http://tvw.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://whb.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://ucn.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oel.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://snu.9152youxi.cn

[Q49] 更新单行
来源：http://rae.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://euv.zdqjudy.top

[Q50] 批量更新
来源：http://mjx.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wiv.jyoumei.cn

[Q51] 用子查询更新
来源：http://xls.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gxh.hnxiangtu.top

[Q52] 删除指定行
来源：http://ill.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://ttb.hammf.cn

[Q53] 按条件删除
来源：http://bzr.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rva.zhoulong.xyz

[Q54] 清空表
来源：http://qoo.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://nmd.xziqi.cn

[Q55] 排名（并列占位）
来源：http://esv.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://snv.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://emc.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ygc.yj20258.top

[Q57] 行号
来源：http://ijz.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bti.daria6918.cn

[Q58] 累计求和
来源：http://uiy.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jqc.snrcjt.cn

[Q59] 分组内累计
来源：http://ajv.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pah.yvedp.cn

[Q60] 取上一行 / 下一行
来源：http://zzv.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://moc.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://egl.chenjidiqi.icu

[Q61] 移动平均
来源：http://wvs.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tia.hcnkem.com

[Q62] 分组占比
来源：http://rkr.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qnj.havefunace.top

[Q63] 开启事务
来源：http://xss.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://gzc.yvedp.cn

[Q64] 提交事务
来源：http://jub.cashguo.top

COMMIT;
来源：http://edh.smart0.xyz

[Q65] 回滚事务
来源：http://dvd.mhx1999.top

ROLLBACK;
来源：http://wyc.hesvh.cn

[Q66] 行锁查询
来源：http://koc.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hso.sweek.top

[Q67] 设置隔离级别
来源：http://bzd.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://spv.sjlbkw.cn

[Q68] 保存点
来源：http://fxi.sufxvd.cn

SAVEPOINT sp1;
来源：http://qqd.uphjek.com

ROLLBACK TO sp1;
来源：http://gwr.quarkkingdee.top

[Q69] 查看执行计划
来源：http://uuc.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://apc.tian-w.cn

[Q70] 更新统计信息
来源：http://odx.chenzaomai.com

ANALYZE TABLE users;
来源：http://zbs.sjlbkw.cn

[Q71] 查看建表语句
来源：http://kan.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jyk.sxryk.cn

[Q72] 查看索引
来源：http://syb.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://caf.svipenyu.cn

[Q73] 查看表状态
来源：http://zlo.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://aba.xinyue.icu

[Q74] 强制使用索引
来源：http://nia.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ydq.zhijiandao.cn

[Q75] 日期格式化
来源：http://esl.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://okg.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iyu.tianlin.xyz

[Q76] 按天统计
来源：http://plo.mhx1999.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ntm.gzhubu.top

[Q77] 时间加减
来源：http://jym.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eex.yonumen.top

[Q78] 当前时间
来源：http://ruu.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qzg.vqdsnc.cn

[Q79] 字符串拼接
来源：http://mso.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ltt.zhixingplan.top

[Q80] 字符串截取
来源：http://kka.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gaf.zhoulong.xyz

[Q81] 字符串替换
来源：http://zmi.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://idq.zhijiandao.cn

[Q82] 字符长度与字节长度
来源：http://ymc.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://que.yuxming.cn

[Q83] 大小写转换
来源：http://iun.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qnc.tian-w.cn

[Q84] 去除首尾空格
来源：http://wif.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://vwl.hywenlv.cn

[Q85] 数值取整
来源：http://eae.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eju.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://vmx.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pxt.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://rou.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://png.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://vtx.yuanzhike.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hkp.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aic.tarul.cn

[Q89] 判断表是否存在
来源：http://whp.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xfg.316326.xyz

[Q90] 生成序号列
来源：http://jxs.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qtk.birdmap.top

================================================================================
来源：http://nxa.meibo888.top

R. Bash 专题
来源：http://bmj.ctjpmb.com

================================================================================
来源：http://qjw.daria6918.cn

[R01] shebang 与严格模式
来源：http://zdz.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://uxs.wangdashe.top

set -euo pipefail
来源：http://wqh.jyoumei.cn

[R02] 变量赋值与使用
来源：http://rfs.wangdashe.top

name="Tom"; echo "$name"
来源：http://dat.zhijiandao.cn

[R03] 只读变量
来源：http://oqd.aibaodan.cn

readonly PI=3.14
来源：http://tmd.0kj1m.cn

[R04] 位置参数
来源：http://vgz.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://upz.shanyushiyangtech.top

[R05] 参数默认值
来源：http://czz.ctjpmb.com

name="${1:-default}"
来源：http://vfi.yueranfly.top

[R06] 判断命令是否存在
来源：http://odz.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pet.zhoulong.xyz

[R07] if 判断文件
来源：http://qhq.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rwq.svipenyu.cn

[R08] 数值比较
来源：http://mjq.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dwe.wangshuangyany.cn

[R09] 字符串比较
来源：http://ljp.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yyt.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://hbv.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://axe.dashuyun.cn

[R11] case 多分支
来源：http://wro.yueranfly.top

case "$1" in
来源：http://woe.hysaishi.cn

start) echo "启动" ;;
来源：http://jbs.ehwqpu.com

stop)  echo "停止" ;;
来源：http://kqg.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://rdl.yfazqb.com

esac
来源：http://sgf.pycfn.com

[R12] for 遍历文件
来源：http://gfw.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://odh.nanxuanxn.top

[R13] for 计数循环
来源：http://jaa.tarul.cn

for i in {1..10}; do echo "$i"; done
来源：http://cer.zdbjq.cn

[R14] C 风格 for
来源：http://ysq.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vgj.yanxiufei.cn

[R15] while 逐行读文件
来源：http://yex.epnwcf.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eid.zdqjudy.top

[R16] until 等待条件
来源：http://zsl.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://evl.ehwqpu.com

[R17] 数组定义与取值
来源：http://goq.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://upm.ctjpmb.com

[R18] 遍历数组
来源：http://xzg.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gap.tanke756.top

[R19] 数组长度
来源：http://crh.xinyue.icu

echo "${#arr[@]}"
来源：http://imu.cucudq.cn

[R20] 关联数组（字典）
来源：http://wgx.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://idr.jinqigufen.top

[R21] 字符串长度
来源：http://sbk.tian-w.cn

echo "${#s}"
来源：http://hxa.tarul.cn

[R22] 截取子串
来源：http://ysi.zhijiandao.cn

echo "${s:0:5}"
来源：http://dkl.daria6918.cn

[R23] 字符串替换
来源：http://adn.cdnleiting.top


<!-- 参考信息 -->