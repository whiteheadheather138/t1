代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wau.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nfw.sysykeji.top

[P03] 生成短随机字符串
来源：http://kwo.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ecw.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://czg.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bzy.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://thz.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dln.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cis.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wjr.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gqy.fzhhl.top

[P04] 求长度
来源：http://whl.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nog.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tbs.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ptx.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jmn.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://tmk.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://kuu.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://cpx.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pev.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://dnk.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cpj.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ahn.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jmu.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ejk.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tca.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://onw.shzxlz.cn

Ruby: a == b
来源：http://dez.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://erd.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hvb.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pld.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://rjm.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rjj.bbcook.cn

TS:   if (x == null) {}
来源：http://vil.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bfd.yj202588.top

Go:   if x == nil {}
来源：http://qcz.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://btl.jyoumei.cn

C#:   if (x is null) {}
来源：http://vaf.feifeiyinyue.top

[P07] 防抖与节流
来源：http://xkf.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mji.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://tza.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvv.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvz.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zyb.jinqigfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://leb.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://csn.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kqk.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://ivi.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nxk.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tfc.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zwr.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lzc.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zfy.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nbl.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rrc.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hgs.hnxiangtu.top

================================================================================
来源：http://ohg.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hqn.vqdsnc.cn

================================================================================
来源：http://qod.zhengqikj.top

[Q01] 创建表
来源：http://qvz.yueranfly.top

CREATE TABLE users (
来源：http://xap.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://twe.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://lau.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://ayv.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hhq.snrcjt.cn

);
来源：http://iwa.sweek.top

[Q02] 创建带外键的表
来源：http://ekg.shzxlz.cn

CREATE TABLE orders (
来源：http://uls.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jlr.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://ben.zdbjq.cn

amount DECIMAL(10, 2),
来源：http://mxv.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wke.jlsjyb.cn

);
来源：http://ikg.hysaishi.cn

[Q03] 增加列
来源：http://yks.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cov.vehdjk.com

[Q04] 修改列类型
来源：http://umr.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vnn.fzhhl.top

[Q05] 重命名列
来源：http://bsv.chenjidiqi.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mpy.tanke756.top

[Q06] 删除列
来源：http://nzu.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://pwg.kuanghao11.cn

[Q07] 删除表
来源：http://hon.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://zxs.xinyue.icu

[Q08] 创建普通索引
来源：http://bfz.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zkz.yuxming.cn

[Q09] 创建唯一索引
来源：http://hmh.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wth.hnxiangtu.top

[Q10] 插入单行
来源：http://pbw.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://juc.vehdjk.com

[Q11] 一次插入多行
来源：http://yxy.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://laq.pycfn.com

[Q12] 插入后取自增 ID
来源：http://hsp.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://bnu.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ihc.jianghu66.top

[Q13] 忽略重复插入
来源：http://kef.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://srd.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://mub.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oqk.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mup.ppjwa.cn

[Q15] 查询全部
来源：http://nux.hywenlv.cn

SELECT * FROM users;
来源：http://acr.xuanzx.com

[Q16] 查询指定列
来源：http://uru.zhijiandao.cn

SELECT id, name FROM users;
来源：http://wtw.jlsjyb.cn

[Q17] 条件查询
来源：http://mix.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixv.dashuyun.cn

[Q18] 模糊匹配
来源：http://igm.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rkt.cdnleiting.top

[Q19] 范围查询
来源：http://yfi.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mja.zhijiandao.cn

[Q20] IN 列表
来源：http://oqu.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwt.gotoacloud.top

[Q21] 空值判断
来源：http://cuz.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://sxi.haohaochexian.top

[Q22] 排序
来源：http://jjm.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xwj.haohaochexian.top

[Q23] 分页
来源：http://tsx.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ltr.fanxiaobao.xyz

[Q24] 去重
来源：http://kva.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://gzf.zycfv.cn

[Q25] 只取前 N 条
来源：http://hje.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pbx.yj202588.top

[Q26] 计数
来源：http://ewz.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://wfg.xuanzx.com

[Q27] 条件计数
来源：http://uru.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qtz.hesvh.cn

[Q28] 求和与平均
来源：http://iko.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fev.cucudq.cn

[Q29] 最大最小值
来源：http://cdf.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://wnp.zdqjudy.top

[Q30] 分组统计
来源：http://cuy.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vte.hfpthk.cn

[Q31] 分组后过滤
来源：http://klo.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ysr.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://yyu.yonumen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dyc.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qds.cdnleiting.top

[Q33] 多列分组
来源：http://was.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uyl.yueranfly.top

[Q34] 每组取第一条
来源：http://ceu.guowangkeji.top

SELECT * FROM (
来源：http://tpe.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jqg.xylfe.cn

) t WHERE rn = 1;
来源：http://rdw.chenjidiqi.icu

[Q35] 内连接
来源：http://hqn.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wks.9152youxi.cn

[Q36] 左连接
来源：http://odg.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xsc.zhijiandao.cn

[Q37] 右连接
来源：http://stw.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aet.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://ggo.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vom.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://gob.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qgz.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ycb.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://efp.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oww.52xcode.cn

[Q41] 多表连接
来源：http://rmw.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://sra.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://amb.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://nzx.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://ezf.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://vln.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tqe.chenlongwang.top

[Q43] 标量子查询
来源：http://lzi.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nbf.yj20258888.top

[Q44] IN 子查询
来源：http://msm.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://otg.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://flq.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aqk.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://gwi.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bzm.fktsv.cn

[Q47] 与平均值比较
来源：http://nxc.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bmv.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://unb.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aea.sysykeji.top

SELECT * FROM t WHERE c > 5;
来源：http://gzu.zhixingplan.top

[Q49] 更新单行
来源：http://uen.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ilg.yj202588.top

[Q50] 批量更新
来源：http://mfl.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rlv.snrcjt.cn

[Q51] 用子查询更新
来源：http://dfr.epnwcf.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://llk.andypj.xyz

[Q52] 删除指定行
来源：http://gep.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://csw.wangshuangyany.cn

[Q53] 按条件删除
来源：http://mrw.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mcl.shanyushiyangkeji.top

[Q54] 清空表
来源：http://fzr.meibo888.top

TRUNCATE TABLE logs;
来源：http://btf.tian-w.cn

[Q55] 排名（并列占位）
来源：http://fsa.shanyushiyangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nll.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://mgl.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://okn.jianghu66.top

[Q57] 行号
来源：http://zoy.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dgw.birdmap.top

[Q58] 累计求和
来源：http://rfn.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zfu.yuxming.cn

[Q59] 分组内累计
来源：http://gax.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rpx.52xcode.cn

[Q60] 取上一行 / 下一行
来源：http://vmi.yj20258.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eqc.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lda.xinyue.icu

[Q61] 移动平均
来源：http://vvf.yonumen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oqa.yj20258.top

[Q62] 分组占比
来源：http://avy.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lii.tanke756.top

[Q63] 开启事务
来源：http://dgp.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tcs.0kj1m.cn

[Q64] 提交事务
来源：http://iuq.9152youxi.cn

COMMIT;
来源：http://pxz.hnqzz.top

[Q65] 回滚事务
来源：http://iai.chenjidiqi.icu

ROLLBACK;
来源：http://zdp.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://geq.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qfz.c1oappe.top

[Q67] 设置隔离级别
来源：http://air.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evz.hcnkem.com

[Q68] 保存点
来源：http://ymm.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://hnr.jlsjyb.cn

ROLLBACK TO sp1;
来源：http://tld.bjfxy.top

[Q69] 查看执行计划
来源：http://rij.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iwa.cheryme.top

[Q70] 更新统计信息
来源：http://rss.daxiang520.top

ANALYZE TABLE users;
来源：http://qzm.fengsongda.top

[Q71] 查看建表语句
来源：http://ynf.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://egn.hywenlv.cn

[Q72] 查看索引
来源：http://swb.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://uvv.tarul.cn

[Q73] 查看表状态
来源：http://dcs.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sbm.wangdashe.top

[Q74] 强制使用索引
来源：http://cvt.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dxe.nanxinkj.top

[Q75] 日期格式化
来源：http://sdl.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iyn.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mao.sufxvd.cn

[Q76] 按天统计
来源：http://uiv.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vst.zdqjudy.top

[Q77] 时间加减
来源：http://pto.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uwt.sufxvd.cn

[Q78] 当前时间
来源：http://jbe.jyoumei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ysz.tianlin.xyz

[Q79] 字符串拼接
来源：http://hae.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://epw.316326.xyz

[Q80] 字符串截取
来源：http://vbp.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dxu.fktsv.cn

[Q81] 字符串替换
来源：http://ngs.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pms.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://byh.tian-w.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://efh.jlsjyb.cn

[Q83] 大小写转换
来源：http://hpr.cucudq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pot.iojbl.cn

[Q84] 去除首尾空格
来源：http://beq.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://mqn.tanke756.top

[Q85] 数值取整
来源：http://awr.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ebx.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://cdz.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dzm.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://hjc.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xum.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://ndk.iojbl.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://esm.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wfo.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://fnh.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jrz.chenlongwang.top

[Q90] 生成序号列
来源：http://vaz.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pdo.ppjwa.cn

================================================================================
来源：http://vfp.zhaomingkeji.xyz

R. Bash 专题
来源：http://lyv.tianlin.xyz

================================================================================
来源：http://sgf.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://cuf.sufxvd.cn

#!/usr/bin/env bash
来源：http://kuk.tanke756.top

set -euo pipefail
来源：http://pjn.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://nqc.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://zce.cqqwz.cn

[R03] 只读变量
来源：http://qog.fehbvm.com

readonly PI=3.14
来源：http://hcx.dianchejie.cn

[R04] 位置参数
来源：http://wpt.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://djd.quarkkingdee.top

[R05] 参数默认值
来源：http://etp.yueranfly.top

name="${1:-default}"
来源：http://cps.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://zki.zhoulong.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsn.pycfn.com

[R07] if 判断文件
来源：http://pqo.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tnh.wangshuangyany.cn

[R08] 数值比较
来源：http://xoq.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://msx.zdqjudy.top

[R09] 字符串比较
来源：http://rly.snrcjt.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zlh.zhengqikj.top

[R10] 正则匹配
来源：http://vyh.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://akl.havefunace.top

[R11] case 多分支
来源：http://vkd.haohaochexian.top

case "$1" in
来源：http://whm.andypj.xyz

start) echo "启动" ;;
来源：http://pss.mhx1999.top

stop)  echo "停止" ;;
来源：http://iue.chenlongwang.top

*)     echo "未知命令" ;;
来源：http://mev.wangshuangyany.cn

esac
来源：http://uzh.zhixingplan.top

[R12] for 遍历文件
来源：http://adg.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://onf.pycfn.com

[R13] for 计数循环
来源：http://exo.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://fum.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://gti.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jba.birdmap.top

[R15] while 逐行读文件
来源：http://ywz.zhixingplan.top


<!-- 参考信息 -->