代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jph.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gro.guowangkeji.top

[P03] 生成短随机字符串
来源：http://dme.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mgw.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://asu.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixq.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vhh.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hoo.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lhq.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://npc.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://prs.yj202588.top

[P04] 求长度
来源：http://uud.xuanzx.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qby.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hzi.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lut.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dkl.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://hov.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://bed.xylfe.cn

Ruby: x.length;  x.size
来源：http://irl.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://vtj.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://ehq.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jgy.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pqe.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://amv.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vcg.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lqb.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://flc.sxryk.cn

Ruby: a == b
来源：http://lbh.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hzn.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bpk.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oeq.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://czf.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gnv.daria6918.cn

TS:   if (x == null) {}
来源：http://etg.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ase.yfazqb.com

Go:   if x == nil {}
来源：http://pjb.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qgg.guowangkeji.top

C#:   if (x is null) {}
来源：http://skc.xinyue.icu

[P07] 防抖与节流
来源：http://bwq.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kst.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://vai.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixn.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epb.zhengqikj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dpg.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rqr.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vzf.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sge.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://qde.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wzl.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://els.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uou.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vko.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ukh.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cru.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bfw.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://phb.pycfn.com

================================================================================
来源：http://cvd.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zvb.xinyue.icu

================================================================================
来源：http://tcf.hcnkem.com

[Q01] 创建表
来源：http://duj.sjlbkw.cn

CREATE TABLE users (
来源：http://coq.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vof.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://can.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://fiq.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvt.jqgufenzy.top

);
来源：http://jgl.iojbl.cn

[Q02] 创建带外键的表
来源：http://yoj.meibo888.top

CREATE TABLE orders (
来源：http://jup.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fir.nwbrower.top

user_id INT NOT NULL,
来源：http://uux.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://slm.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://thu.ydjk.org.cn

);
来源：http://evt.shanyushiyangtech.top

[Q03] 增加列
来源：http://mso.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kbv.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://jwt.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nlq.smart0.xyz

[Q05] 重命名列
来源：http://lig.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://odo.bbcook.cn

[Q06] 删除列
来源：http://uko.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://mvf.aizwys.cn

[Q07] 删除表
来源：http://cbo.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://dgy.jinqigufen.top

[Q08] 创建普通索引
来源：http://sso.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zqr.hesvh.cn

[Q09] 创建唯一索引
来源：http://xee.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kpe.yuanzhike.top

[Q10] 插入单行
来源：http://txa.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yhx.yuxming.cn

[Q11] 一次插入多行
来源：http://coj.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hcb.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://qqs.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://uem.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://etl.cdnleiting.top

[Q13] 忽略重复插入
来源：http://qht.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wrg.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://xay.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vlw.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jtf.jlsjyb.cn

[Q15] 查询全部
来源：http://dez.chenzaomai.com

SELECT * FROM users;
来源：http://kxq.pengpengdd.cyou

[Q16] 查询指定列
来源：http://exg.tianlin.xyz

SELECT id, name FROM users;
来源：http://xfo.tian-w.cn

[Q17] 条件查询
来源：http://bic.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://snr.cashguo.top

[Q18] 模糊匹配
来源：http://jsv.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fsr.52xcode.cn

[Q19] 范围查询
来源：http://xdw.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kqc.iojbl.cn

[Q20] IN 列表
来源：http://akk.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ayi.sxryk.cn

[Q21] 空值判断
来源：http://gxg.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://noq.gotoacloud.top

[Q22] 排序
来源：http://bmr.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mht.dianchejie.cn

[Q23] 分页
来源：http://rug.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://biw.ywan-chungtsiang.top

[Q24] 去重
来源：http://hok.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://diy.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://stg.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uew.xinyue.icu

[Q26] 计数
来源：http://gre.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://sxw.gaohongyu789.top

[Q27] 条件计数
来源：http://vuf.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://svz.ppjwa.cn

[Q28] 求和与平均
来源：http://hxf.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ytc.jyoumei.cn

[Q29] 最大最小值
来源：http://gpl.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ney.fanxiaobao.xyz

[Q30] 分组统计
来源：http://jyt.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eml.xylfe.cn

[Q31] 分组后过滤
来源：http://dyt.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jxm.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://hlj.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zol.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oiu.snrcjt.cn

[Q33] 多列分组
来源：http://uyv.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ser.tianlin.xyz

[Q34] 每组取第一条
来源：http://opv.hesvh.cn

SELECT * FROM (
来源：http://jcv.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ktf.hesvh.cn

) t WHERE rn = 1;
来源：http://rhv.ehwqpu.com

[Q35] 内连接
来源：http://jwf.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fzr.ywan-chungtsiang.top

[Q36] 左连接
来源：http://ebz.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xmk.0kj1m.cn

[Q37] 右连接
来源：http://skk.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aoo.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://sds.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gdk.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://kio.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ewp.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xwy.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://nkl.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ndh.svipenyu.cn

[Q41] 多表连接
来源：http://jxh.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ozh.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://eaf.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://nbt.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://tru.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://zqn.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://urj.yanxiufei.cn

[Q43] 标量子查询
来源：http://elw.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fxu.ydjk.org.cn

[Q44] IN 子查询
来源：http://flf.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ldn.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://iwf.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pcq.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ekb.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gmd.hywenlv.cn

[Q47] 与平均值比较
来源：http://szo.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ysq.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://dox.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dkr.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://sgo.gaohongyu789.top

[Q49] 更新单行
来源：http://gpw.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iqq.nanxuanxn.top

[Q50] 批量更新
来源：http://fov.chenzaomai.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ttj.ybcxt.top

[Q51] 用子查询更新
来源：http://ice.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rru.vqdsnc.cn

[Q52] 删除指定行
来源：http://uyz.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://cdt.guowangkeji.top

[Q53] 按条件删除
来源：http://gcl.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://krq.yanxiufei.cn

[Q54] 清空表
来源：http://yoh.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://oyc.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://hrt.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rhi.dianchejie.cn

[Q56] 密集排名（并列不占位）
来源：http://iww.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ivh.ybcxt.top

[Q57] 行号
来源：http://hgn.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://axe.9152youxi.cn

[Q58] 累计求和
来源：http://zvg.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmm.chenlongwang.top

[Q59] 分组内累计
来源：http://ebm.shangyingyoupin.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mnb.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://bed.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yog.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qrq.jianghu66.top

[Q61] 移动平均
来源：http://foq.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qnv.uphjek.com

[Q62] 分组占比
来源：http://oga.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vpk.tianlin.xyz

[Q63] 开启事务
来源：http://zog.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dbf.zhiwuduotai.top

[Q64] 提交事务
来源：http://qzv.bbcook.cn

COMMIT;
来源：http://ctu.nanxuanxn.top

[Q65] 回滚事务
来源：http://abx.zdqjudy.top

ROLLBACK;
来源：http://cwp.nwbrower.top

[Q66] 行锁查询
来源：http://gcg.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://osf.pycfn.com

[Q67] 设置隔离级别
来源：http://zeg.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nwv.guannengcc.top

[Q68] 保存点
来源：http://hko.zhongyouzk.top

SAVEPOINT sp1;
来源：http://dzu.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://pca.zhoulong.xyz

[Q69] 查看执行计划
来源：http://eiq.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kyv.wangdashe.top

[Q70] 更新统计信息
来源：http://pqz.fktsv.cn

ANALYZE TABLE users;
来源：http://lkd.hesvh.cn

[Q71] 查看建表语句
来源：http://mgz.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cls.dashuyun.cn

[Q72] 查看索引
来源：http://stp.52xcode.cn

SHOW INDEX FROM users;
来源：http://bmo.ydjk.org.cn

[Q73] 查看表状态
来源：http://dkk.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sxm.zycfv.cn

[Q74] 强制使用索引
来源：http://chv.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://slk.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://bct.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tqq.zhiwuduotai.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fjt.jlsjyb.cn

[Q76] 按天统计
来源：http://ydt.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://owx.tarul.cn

[Q77] 时间加减
来源：http://ocr.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://drg.fanxiaobao.xyz

[Q78] 当前时间
来源：http://qfw.ivvv.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://umv.fengsongda.top

[Q79] 字符串拼接
来源：http://aob.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iet.wangshuangyany.cn

[Q80] 字符串截取
来源：http://zzy.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://afh.sxryk.cn

[Q81] 字符串替换
来源：http://ouq.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vbi.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://ely.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jwz.guannengcc.top

[Q83] 大小写转换
来源：http://bni.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lof.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://lgt.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://urg.guowangkeji.top

[Q85] 数值取整
来源：http://kuv.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qnp.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://sow.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cmb.wangdashe.top

[Q87] JSON 字段做条件
来源：http://xpv.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrx.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://aak.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xrp.jyoumei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mbv.gogol.net.cn

[Q89] 判断表是否存在
来源：http://xsj.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qdg.tian-w.cn

[Q90] 生成序号列
来源：http://rgz.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vps.redwolf501.top

================================================================================
来源：http://rfj.zhoulong.xyz

R. Bash 专题
来源：http://vrl.tianlin.xyz

================================================================================
来源：http://nut.havefunace.top

[R01] shebang 与严格模式
来源：http://dtz.9152youxi.cn

#!/usr/bin/env bash
来源：http://ggs.cdnleiting.top

set -euo pipefail
来源：http://txw.hammf.cn

[R02] 变量赋值与使用
来源：http://ngx.gzhubu.top

name="Tom"; echo "$name"
来源：http://rge.c1oappe.top

[R03] 只读变量
来源：http://eap.ydjk.org.cn

readonly PI=3.14
来源：http://vcq.bjfxy.top

[R04] 位置参数
来源：http://cxi.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://abn.tarul.cn

[R05] 参数默认值
来源：http://wjl.jinghuilouyu.cn

name="${1:-default}"
来源：http://hav.shangyingyoupin.top

[R06] 判断命令是否存在
来源：http://ddo.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xws.birdmap.top

[R07] if 判断文件
来源：http://ctd.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ozf.yj20258.top

[R08] 数值比较
来源：http://zxx.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://sas.zdqjudy.top

[R09] 字符串比较
来源：http://nyp.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vjq.jqgfzy.top

[R10] 正则匹配
来源：http://wgu.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ldu.ydzc1.top

[R11] case 多分支
来源：http://rby.zhongyouzk.top

case "$1" in
来源：http://vbd.xingfuxueyuan.xyz

start) echo "启动" ;;
来源：http://czi.sweek.top

stop)  echo "停止" ;;
来源：http://ihn.yonumen.top

*)     echo "未知命令" ;;
来源：http://aco.shangyingyoupin.top

esac
来源：http://yco.xuanzx.com

[R12] for 遍历文件
来源：http://uas.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://ojv.shanyushiyangtech.top

[R13] for 计数循环
来源：http://hso.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://epx.tarul.cn

[R14] C 风格 for
来源：http://bng.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mpp.fzhhl.top

[R15] while 逐行读文件
来源：http://ngx.316326.xyz


<!-- 参考信息 -->