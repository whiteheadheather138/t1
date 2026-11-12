代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ehz.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jnj.nwbrower.top

[P03] 生成短随机字符串
来源：http://vxo.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ipn.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mls.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://enb.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fbk.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://twq.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cyd.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ywp.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xdb.shzxlz.cn

[P04] 求长度
来源：http://gzo.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qjy.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvk.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hsm.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzg.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://kvj.daxiang520.top

Go:   len(arr);  len(m)
来源：http://xef.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://shp.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rjc.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://bea.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fta.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hue.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kpp.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zlr.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yni.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sqz.jinqigufen.top

Ruby: a == b
来源：http://wxy.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://chv.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tua.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ymw.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://cfe.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uwj.gotoacloud.top

TS:   if (x == null) {}
来源：http://aho.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://dkz.redwolf501.top

Go:   if x == nil {}
来源：http://yaf.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pon.daria6918.cn

C#:   if (x is null) {}
来源：http://fiw.cqqwz.cn

[P07] 防抖与节流
来源：http://slk.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ozu.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://dyo.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvx.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtp.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://chn.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xmh.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://och.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://siq.fzhhl.top

[P08] 处理浮点精度问题
来源：http://ogc.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yjq.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mqw.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://frj.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sdu.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yia.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bnt.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wlt.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yux.fanxiaobao.xyz

================================================================================
来源：http://onf.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fzp.yangfankeji.com

================================================================================
来源：http://edv.xuanzx.com

[Q01] 创建表
来源：http://rbj.0kj1m.cn

CREATE TABLE users (
来源：http://sxt.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dxi.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://tkp.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://gvy.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://esg.gotoacloud.top

);
来源：http://gzo.hcnkem.com

[Q02] 创建带外键的表
来源：http://cby.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://aiq.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfj.sxryk.cn

user_id INT NOT NULL,
来源：http://yei.xuanzx.com

amount DECIMAL(10, 2),
来源：http://aic.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ltg.cdnleiting.top

);
来源：http://nlk.nanxinkj.top

[Q03] 增加列
来源：http://mkt.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vtj.yueranfly.top

[Q04] 修改列类型
来源：http://gbp.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mpb.yanxiufei.cn

[Q05] 重命名列
来源：http://hvh.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mgh.tarul.cn

[Q06] 删除列
来源：http://xnr.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://lok.pengpengdd.cyou

[Q07] 删除表
来源：http://xhn.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://xhq.c1oappe.top

[Q08] 创建普通索引
来源：http://uwp.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ffm.hysaishi.cn

[Q09] 创建唯一索引
来源：http://gyi.xinyue.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gei.hammf.cn

[Q10] 插入单行
来源：http://ubu.fzhhl.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jvp.hnqzz.top

[Q11] 一次插入多行
来源：http://tlt.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://img.uphjek.com

[Q12] 插入后取自增 ID
来源：http://vet.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://rgq.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pjo.vehdjk.com

[Q13] 忽略重复插入
来源：http://biy.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jpg.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://yyq.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xby.haohaochexian.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pge.guowangkeji.top

[Q15] 查询全部
来源：http://zpb.52xcode.cn

SELECT * FROM users;
来源：http://dyf.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://zfg.aibaodan.cn

SELECT id, name FROM users;
来源：http://vtv.bbcook.cn

[Q17] 条件查询
来源：http://dnz.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ewj.ehwqpu.com

[Q18] 模糊匹配
来源：http://nqn.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vbh.yueranfly.top

[Q19] 范围查询
来源：http://vkl.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uzb.wangdashe.top

[Q20] IN 列表
来源：http://oai.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://btz.andypj.xyz

[Q21] 空值判断
来源：http://nsd.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://usx.ybcxt.top

[Q22] 排序
来源：http://fyq.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uoy.yangfankeji.com

[Q23] 分页
来源：http://wkp.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yfa.gaohongyu789.top

[Q24] 去重
来源：http://blv.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://wth.gotoacloud.top

[Q25] 只取前 N 条
来源：http://hpb.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fde.zdbjq.cn

[Q26] 计数
来源：http://suw.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://wvn.iojbl.cn

[Q27] 条件计数
来源：http://vsi.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dvt.cqqwz.cn

[Q28] 求和与平均
来源：http://gzg.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fig.sweek.top

[Q29] 最大最小值
来源：http://cmi.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yva.bbcook.cn

[Q30] 分组统计
来源：http://jrw.hammf.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kry.nanxuanxn.top

[Q31] 分组后过滤
来源：http://dac.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kqu.fengsongda.top

[Q32] 分组拼接字符串
来源：http://tem.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xic.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ddd.cheryme.top

[Q33] 多列分组
来源：http://cnr.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ibs.0kj1m.cn

[Q34] 每组取第一条
来源：http://zci.yueranfly.top

SELECT * FROM (
来源：http://aqu.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xaz.quarkkingdee.top

) t WHERE rn = 1;
来源：http://scu.ppjwa.cn

[Q35] 内连接
来源：http://ebl.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qrh.fzhhl.top

[Q36] 左连接
来源：http://dfa.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zvj.hnqzz.top

[Q37] 右连接
来源：http://xdo.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ogo.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://jto.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iuf.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://kqj.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://kab.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jga.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://maf.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pmd.yuanzhike.top

[Q41] 多表连接
来源：http://odi.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://inh.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://kmv.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://yaj.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://zmn.pycfn.com

SELECT u.name, o.amount FROM users u
来源：http://yhg.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://doc.sysykeji.top

[Q43] 标量子查询
来源：http://sty.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ucf.yfazqb.com

[Q44] IN 子查询
来源：http://gjr.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dtf.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://ufj.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jtf.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nhi.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fac.bjfxy.top

[Q47] 与平均值比较
来源：http://ytx.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yel.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://bgn.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wjd.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://rhg.uphjek.com

[Q49] 更新单行
来源：http://zll.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xlo.tian-w.cn

[Q50] 批量更新
来源：http://iqy.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://one.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://opu.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zkt.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://fwx.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://qmx.yuxming.cn

[Q53] 按条件删除
来源：http://ozd.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nfj.hfpthk.cn

[Q54] 清空表
来源：http://vto.mhx1999.top

TRUNCATE TABLE logs;
来源：http://sjt.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://flk.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rbj.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://dxo.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iqq.zdqjudy.top

[Q57] 行号
来源：http://pon.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jvh.jqgufenzy.top

[Q58] 累计求和
来源：http://ekx.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mws.fktsv.cn

[Q59] 分组内累计
来源：http://wfs.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://niz.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://rcf.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gnc.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ufw.fengsongda.top

[Q61] 移动平均
来源：http://xfp.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rqt.cdnleiting.top

[Q62] 分组占比
来源：http://qwv.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bow.zhixingplan.top

[Q63] 开启事务
来源：http://exs.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://muq.dianchejie.cn

[Q64] 提交事务
来源：http://ymk.yj202588.top

COMMIT;
来源：http://ukw.cqqwz.cn

[Q65] 回滚事务
来源：http://ddr.gaohongyu789.top

ROLLBACK;
来源：http://siq.guannengcc.top

[Q66] 行锁查询
来源：http://nmb.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mfr.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://jvs.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rtu.jinyuanbaomall.cn

[Q68] 保存点
来源：http://hnh.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://nnk.bjfxy.top

ROLLBACK TO sp1;
来源：http://ipl.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://eap.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://njb.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://nov.aibaodan.cn

ANALYZE TABLE users;
来源：http://uoq.gzhubu.top

[Q71] 查看建表语句
来源：http://cxo.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iav.gaohongyu789.top

[Q72] 查看索引
来源：http://dgm.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://yxd.xuanzx.com

[Q73] 查看表状态
来源：http://qih.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zqq.uphjek.com

[Q74] 强制使用索引
来源：http://zdc.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sxr.dashuyun.cn

[Q75] 日期格式化
来源：http://vyf.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://shq.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bgz.shzxlz.cn

[Q76] 按天统计
来源：http://vib.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://peq.chenlongwang.top

[Q77] 时间加减
来源：http://ouz.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cbb.xylfe.cn

[Q78] 当前时间
来源：http://wed.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jrx.gaohongyu789.top

[Q79] 字符串拼接
来源：http://ttm.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cks.kuanghao11.cn

[Q80] 字符串截取
来源：http://mzt.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jod.fengsongda.top

[Q81] 字符串替换
来源：http://bde.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tqi.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://fkm.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mpe.yj20258.top

[Q83] 大小写转换
来源：http://oia.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nmk.fengsongda.top

[Q84] 去除首尾空格
来源：http://wjp.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://zaz.guowangkeji.top

[Q85] 数值取整
来源：http://ymh.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xhw.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://nnd.aizwys.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://joo.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://xpj.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hep.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://uyt.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tmm.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://srw.ppjwa.cn

[Q89] 判断表是否存在
来源：http://qoc.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cxm.wangshuangyany.cn

[Q90] 生成序号列
来源：http://ygb.chenjidiqi.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xmk.yj202588.top

================================================================================
来源：http://por.zhijiandao.cn

R. Bash 专题
来源：http://hdp.ybcxt.top

================================================================================
来源：http://cdf.havefunace.top

[R01] shebang 与严格模式
来源：http://ctr.ydjk.org.cn

#!/usr/bin/env bash
来源：http://etq.chenlongwang.top

set -euo pipefail
来源：http://uye.fehbvm.com

[R02] 变量赋值与使用
来源：http://fbo.vehdjk.com

name="Tom"; echo "$name"
来源：http://bld.haohaochexian.top

[R03] 只读变量
来源：http://jsk.tian-w.cn

readonly PI=3.14
来源：http://cbj.shanyushiyangtech.top

[R04] 位置参数
来源：http://ocl.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hww.jqgfzy.top

[R05] 参数默认值
来源：http://thi.nanxinkj.top

name="${1:-default}"
来源：http://dkh.guowangkeji.top

[R06] 判断命令是否存在
来源：http://zmd.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vhk.yj20258.top

[R07] if 判断文件
来源：http://nrk.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://krh.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://epb.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dgd.vehdjk.com

[R09] 字符串比较
来源：http://yuc.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qkc.ivvv.top

[R10] 正则匹配
来源：http://pyt.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://avo.zdbjq.cn

[R11] case 多分支
来源：http://ohn.9152youxi.cn

case "$1" in
来源：http://sqv.hywenlv.cn

start) echo "启动" ;;
来源：http://rzb.epnwcf.com

stop)  echo "停止" ;;
来源：http://sja.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://tgk.zhijiandao.cn

esac
来源：http://hhx.redwolf501.top

[R12] for 遍历文件
来源：http://mav.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://duq.hammf.cn

[R13] for 计数循环
来源：http://fbq.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://jcc.shzxlz.cn

[R14] C 风格 for
来源：http://ize.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ugk.bjfxy.top

[R15] while 逐行读文件
来源：http://ckh.dianchejie.cn


<!-- 参考信息 -->