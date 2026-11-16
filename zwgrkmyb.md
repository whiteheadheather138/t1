代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://enc.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mrm.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zzl.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nzl.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ziq.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fff.fengsongda.top

[P03] 生成短随机字符串
来源：http://tkq.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eis.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cdv.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bcv.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qif.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kot.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tmr.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqa.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sie.zhijiandao.cn

[P04] 求长度
来源：http://exq.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ddl.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mye.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mmq.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aac.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://bro.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://rwb.birdmap.top

Ruby: x.length;  x.size
来源：http://uvc.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbf.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://bsx.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pfi.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yyc.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://btt.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://erk.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://isx.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://qkt.nanxinkj.top

Ruby: a == b
来源：http://bpw.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qff.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ivo.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xuz.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://kqk.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrg.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://duj.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bvf.chenzaomai.com

Go:   if x == nil {}
来源：http://mjq.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dak.shzxlz.cn

C#:   if (x is null) {}
来源：http://zyb.cheryme.top

[P07] 防抖与节流
来源：http://fgl.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tqd.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://ezr.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpq.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jok.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pfu.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oay.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hnp.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://txu.wangdashe.top

[P08] 处理浮点精度问题
来源：http://atg.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sho.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nqs.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lkj.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ojn.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iyg.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aqd.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sbr.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://stg.bjfxy.top

================================================================================
来源：http://hba.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gja.shanyushiyangtech.top

================================================================================
来源：http://vgi.sjlbkw.cn

[Q01] 创建表
来源：http://xap.fehbvm.com

CREATE TABLE users (
来源：http://bki.yj202588.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ezz.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://ptx.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://jlr.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zqn.xingfuxueyuan.xyz

);
来源：http://brv.bbcook.cn

[Q02] 创建带外键的表
来源：http://kdc.dashuyun.cn

CREATE TABLE orders (
来源：http://rxt.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://goi.sweek.top

user_id INT NOT NULL,
来源：http://prs.vehdjk.com

amount DECIMAL(10, 2),
来源：http://kwi.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://riq.jinqigfzy.top

);
来源：http://bsj.hnqzz.top

[Q03] 增加列
来源：http://mvh.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rpj.bjfxy.top

[Q04] 修改列类型
来源：http://ehc.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mkg.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://nxe.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vfp.yonumen.top

[Q06] 删除列
来源：http://evg.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://vtd.ydjk.org.cn

[Q07] 删除表
来源：http://cgc.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://rxo.0kj1m.cn

[Q08] 创建普通索引
来源：http://juw.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jyi.shuidangran.top

[Q09] 创建唯一索引
来源：http://ygx.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pak.jinqigfzy.top

[Q10] 插入单行
来源：http://plc.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://syw.nwbrower.top

[Q11] 一次插入多行
来源：http://csw.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cem.daria6918.cn

[Q12] 插入后取自增 ID
来源：http://gdk.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://acr.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pni.meibo888.top

[Q13] 忽略重复插入
来源：http://cvs.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xrc.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://rro.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fit.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://puj.zhiwuduotai.top

[Q15] 查询全部
来源：http://rhl.andypj.xyz

SELECT * FROM users;
来源：http://hlo.birdmap.top

[Q16] 查询指定列
来源：http://ofm.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://abh.hysaishi.cn

[Q17] 条件查询
来源：http://emo.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pms.zhoulong.xyz

[Q18] 模糊匹配
来源：http://tzv.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pko.sxryk.cn

[Q19] 范围查询
来源：http://chv.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jfo.ybcxt.top

[Q20] IN 列表
来源：http://olb.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vik.hnqzz.top

[Q21] 空值判断
来源：http://iux.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xok.daria6918.cn

[Q22] 排序
来源：http://uib.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rzp.shuidangran.top

[Q23] 分页
来源：http://vcf.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wfk.chenlongwang.top

[Q24] 去重
来源：http://hzu.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://rrk.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://itf.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ezd.9152youxi.cn

[Q26] 计数
来源：http://vsc.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://tyg.zhijiandao.cn

[Q27] 条件计数
来源：http://dgr.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fzq.dianchejie.cn

[Q28] 求和与平均
来源：http://zfq.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hhz.yanxiufei.cn

[Q29] 最大最小值
来源：http://pgn.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cpp.52xcode.cn

[Q30] 分组统计
来源：http://gqv.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ddu.iojbl.cn

[Q31] 分组后过滤
来源：http://rrl.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cvt.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://rdb.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jxj.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uah.epnwcf.com

[Q33] 多列分组
来源：http://jek.hnxiangtu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzy.dianchejie.cn

[Q34] 每组取第一条
来源：http://jwo.jinqigufen.top

SELECT * FROM (
来源：http://lzx.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://agv.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://vaw.shangyingyoupin.top

[Q35] 内连接
来源：http://jke.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://doc.ywan-chungtsiang.top

[Q36] 左连接
来源：http://zkd.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kiq.hesvh.cn

[Q37] 右连接
来源：http://exq.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvo.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://fww.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bxe.guowangkeji.top

[Q39] 自连接（查上下级）
来源：http://vtb.zhiwuduotai.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fto.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xhk.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://miw.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://leq.ydjk.org.cn

[Q41] 多表连接
来源：http://nbi.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vxp.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://aki.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://qqs.jinqigfzy.top

[Q42] 连接条件附加过滤
来源：http://fxs.cucudq.cn

SELECT u.name, o.amount FROM users u
来源：http://ilx.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pcd.cheryme.top

[Q43] 标量子查询
来源：http://zdw.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jxj.ivvv.top

[Q44] IN 子查询
来源：http://buk.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://htz.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://qls.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qah.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wrb.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lfl.yuanzhike.top

[Q47] 与平均值比较
来源：http://hgf.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://reh.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://bwv.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xqr.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://bfb.andypj.xyz

[Q49] 更新单行
来源：http://gra.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ddn.yueranfly.top

[Q50] 批量更新
来源：http://gzg.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://smk.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://gxm.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgs.nanxinkj.top

[Q52] 删除指定行
来源：http://zhi.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://ehy.daxiang520.top

[Q53] 按条件删除
来源：http://lky.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdg.ybcxt.top

[Q54] 清空表
来源：http://tbi.epnwcf.com

TRUNCATE TABLE logs;
来源：http://xbi.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://gxo.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xjz.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://tec.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yym.dashuyun.cn

[Q57] 行号
来源：http://jxi.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aqi.hysaishi.cn

[Q58] 累计求和
来源：http://pst.chenjidiqi.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aoc.daxiang520.top

[Q59] 分组内累计
来源：http://nal.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgw.9152youxi.cn

[Q60] 取上一行 / 下一行
来源：http://laf.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://byr.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vny.fzhhl.top

[Q61] 移动平均
来源：http://yof.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qtm.feifeiyinyue.top

[Q62] 分组占比
来源：http://jeq.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uff.sweek.top

[Q63] 开启事务
来源：http://xpu.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wpx.yfazqb.com

[Q64] 提交事务
来源：http://vwy.zhongyouzk.top

COMMIT;
来源：http://cak.xziqi.cn

[Q65] 回滚事务
来源：http://tfi.cashguo.top

ROLLBACK;
来源：http://zww.shangyingyoupin.top

[Q66] 行锁查询
来源：http://ztp.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oir.guannengcc.top

[Q67] 设置隔离级别
来源：http://qxk.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iyk.vqdsnc.cn

[Q68] 保存点
来源：http://zgg.ydzc1.top

SAVEPOINT sp1;
来源：http://mkr.smart0.xyz

ROLLBACK TO sp1;
来源：http://ifs.gzhubu.top

[Q69] 查看执行计划
来源：http://pqz.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hjr.sysykeji.top

[Q70] 更新统计信息
来源：http://rqd.bbcook.cn

ANALYZE TABLE users;
来源：http://ssk.yongpay.top

[Q71] 查看建表语句
来源：http://ata.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ryi.ybcxt.top

[Q72] 查看索引
来源：http://cdk.52xcode.cn

SHOW INDEX FROM users;
来源：http://mte.9152youxi.cn

[Q73] 查看表状态
来源：http://tog.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://eau.jianghu66.top

[Q74] 强制使用索引
来源：http://fue.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vis.aibaodan.cn

[Q75] 日期格式化
来源：http://drd.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kes.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ree.jianghu66.top

[Q76] 按天统计
来源：http://kwg.sufxvd.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://epk.yj20258888.top

[Q77] 时间加减
来源：http://bev.nwbrower.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://avf.xylfe.cn

[Q78] 当前时间
来源：http://pjc.fzhhl.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jqv.ctjpmb.com

[Q79] 字符串拼接
来源：http://npg.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hgy.yfazqb.com

[Q80] 字符串截取
来源：http://ldq.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mog.hysaishi.cn

[Q81] 字符串替换
来源：http://tvh.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ltq.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://iwd.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bym.havefunace.top

[Q83] 大小写转换
来源：http://fyn.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://een.hesvh.cn

[Q84] 去除首尾空格
来源：http://alp.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://guv.cucudq.cn

[Q85] 数值取整
来源：http://qgz.yfazqb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xen.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://dcz.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fld.fehbvm.com

[Q87] JSON 字段做条件
来源：http://ddb.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gui.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://ytw.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://scw.zdbjq.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mif.ehwqpu.com

[Q89] 判断表是否存在
来源：http://dih.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tol.shzxlz.cn

[Q90] 生成序号列
来源：http://zvh.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jjd.bjfxy.top

================================================================================
来源：http://fzt.meibo888.top

R. Bash 专题
来源：http://wkn.wangshuangyany.cn

================================================================================
来源：http://uok.dashuyun.cn

[R01] shebang 与严格模式
来源：http://ons.jyoumei.cn

#!/usr/bin/env bash
来源：http://pgi.jinyuanbaomall.cn

set -euo pipefail
来源：http://sop.hesvh.cn

[R02] 变量赋值与使用
来源：http://ugz.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://eie.pycfn.com

[R03] 只读变量
来源：http://rdo.tarul.cn

readonly PI=3.14
来源：http://yws.hywenlv.cn

[R04] 位置参数
来源：http://gal.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gvb.52xcode.cn

[R05] 参数默认值
来源：http://evn.hammf.cn

name="${1:-default}"
来源：http://gjw.sufxvd.cn

[R06] 判断命令是否存在
来源：http://puz.andypj.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qoz.jyoumei.cn

[R07] if 判断文件
来源：http://xzp.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bmq.jinqigufen.top

[R08] 数值比较
来源：http://ldk.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ast.shanyushiyangtech.top

[R09] 字符串比较
来源：http://qzz.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ieh.bjfxy.top

[R10] 正则匹配
来源：http://cbv.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xcs.zdbjq.cn

[R11] case 多分支
来源：http://jqz.guowangkeji.top

case "$1" in
来源：http://zws.daxiang520.top

start) echo "启动" ;;
来源：http://zbb.sweek.top

stop)  echo "停止" ;;
来源：http://lll.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://xpq.tian-w.cn

esac
来源：http://axb.andypj.xyz

[R12] for 遍历文件
来源：http://len.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://dqo.jiagoushi.top

[R13] for 计数循环
来源：http://svl.daxiang520.top


<!-- 参考信息 -->