代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nwn.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yky.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://ftu.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cby.birdmap.top

[O06] 使用进程池
来源：http://vlr.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wjz.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ixk.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://bkj.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://wbd.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mpk.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qrr.svipenyu.cn

Ruby: // fork 块
来源：http://fvn.shanyushiyangtech.top

C#:   Parallel.For
来源：http://hgt.hfpthk.cn

================================================================================
来源：http://qeg.jinqigfzy.top

P. 常用工具函数
来源：http://ppe.xuanzx.com

================================================================================
来源：http://xqu.ehwqpu.com

[P01] 生成 UUID
来源：http://jkq.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://cel.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iec.hesvh.cn

JS:   crypto.randomUUID()
来源：http://qyf.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://xbf.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://ulv.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://rcs.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://pgz.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://ayw.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://vpb.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sgp.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lri.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fbq.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nyb.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mgs.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jup.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sdw.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sda.zdbjq.cn

[P03] 生成短随机字符串
来源：http://tia.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://goq.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vtu.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fig.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sgw.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sch.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hvp.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://esh.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ilg.yuxming.cn

[P04] 求长度
来源：http://hgl.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bez.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mjq.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jsq.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhz.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://njr.andypj.xyz

Go:   len(arr);  len(m)
来源：http://vnj.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://ikw.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://crw.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://zvi.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vbx.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eue.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://haf.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mvd.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wyw.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://jvq.hfpthk.cn

Ruby: a == b
来源：http://knc.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kgw.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xxj.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tdc.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://hhd.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uom.haohaochexian.top

TS:   if (x == null) {}
来源：http://xkc.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://axm.nanxinkj.top

Go:   if x == nil {}
来源：http://imb.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zui.jianghu66.top

C#:   if (x is null) {}
来源：http://rep.epnwcf.com

[P07] 防抖与节流
来源：http://and.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xqq.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://oiq.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyh.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txq.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://umu.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ixb.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kdt.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://snl.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://pkk.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxz.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lkk.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nnp.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hvx.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqb.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dqb.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gtb.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zcv.jyoumei.cn

================================================================================
来源：http://dct.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tdg.fanxiaobao.xyz

================================================================================
来源：http://upc.hnqzz.top

[Q01] 创建表
来源：http://udn.sxryk.cn

CREATE TABLE users (
来源：http://jfr.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xjn.daxiang520.top

name VARCHAR(50) NOT NULL,
来源：http://sqh.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://hxq.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cqd.dashuyun.cn

);
来源：http://ikl.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://xmn.vehdjk.com

CREATE TABLE orders (
来源：http://clu.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vzx.meibo888.top

user_id INT NOT NULL,
来源：http://eow.shuidangran.top

amount DECIMAL(10, 2),
来源：http://gjn.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wgr.andypj.xyz

);
来源：http://onw.zhijiandao.cn

[Q03] 增加列
来源：http://azs.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dow.hnqzz.top

[Q04] 修改列类型
来源：http://bmk.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sxo.xylfe.cn

[Q05] 重命名列
来源：http://ywm.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wou.gzhubu.top

[Q06] 删除列
来源：http://wtn.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://hqr.zhoulong.xyz

[Q07] 删除表
来源：http://kfv.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://bwu.zdqjudy.top

[Q08] 创建普通索引
来源：http://lni.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yio.fzhhl.top

[Q09] 创建唯一索引
来源：http://atg.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://irm.xuanzx.com

[Q10] 插入单行
来源：http://vir.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cba.cdnleiting.top

[Q11] 一次插入多行
来源：http://xql.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sso.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://mqg.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://sss.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zhf.hfpthk.cn

[Q13] 忽略重复插入
来源：http://wru.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lft.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://qle.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://udw.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://amv.shangyingyoupin.top

[Q15] 查询全部
来源：http://qeo.bbcook.cn

SELECT * FROM users;
来源：http://amt.cqqwz.cn

[Q16] 查询指定列
来源：http://kth.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://qbm.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://tao.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uhy.cdnleiting.top

[Q18] 模糊匹配
来源：http://owc.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bom.shanyushiyangtech.top

[Q19] 范围查询
来源：http://wyo.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lyk.chenlongwang.top

[Q20] IN 列表
来源：http://mrd.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://awg.xziqi.cn

[Q21] 空值判断
来源：http://uzs.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yzv.gzhubu.top

[Q22] 排序
来源：http://dxf.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://axd.hammf.cn

[Q23] 分页
来源：http://etu.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kum.yvedp.cn

[Q24] 去重
来源：http://vfk.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://zkd.nanxinkj.top

[Q25] 只取前 N 条
来源：http://tkc.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwb.jinqigfzy.top

[Q26] 计数
来源：http://wgl.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://mmf.vehdjk.com

[Q27] 条件计数
来源：http://ygg.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iqw.zhengqikj.top

[Q28] 求和与平均
来源：http://qtx.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vtm.andypj.xyz

[Q29] 最大最小值
来源：http://afc.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dgx.yj20258.top

[Q30] 分组统计
来源：http://nyg.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bwf.hesvh.cn

[Q31] 分组后过滤
来源：http://eul.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://txy.guannengcc.top

[Q32] 分组拼接字符串
来源：http://ksr.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uov.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yus.zdqjudy.top

[Q33] 多列分组
来源：http://vzs.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgl.hammf.cn

[Q34] 每组取第一条
来源：http://lcl.guannengcc.top

SELECT * FROM (
来源：http://ujz.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yzs.nanxinkj.top

) t WHERE rn = 1;
来源：http://rfq.kuanghao11.cn

[Q35] 内连接
来源：http://knf.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hpt.svipenyu.cn

[Q36] 左连接
来源：http://xeq.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vki.vqdsnc.cn

[Q37] 右连接
来源：http://gsn.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ngq.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://efl.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hay.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://ful.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://bfa.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://npm.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dhj.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://huh.aizwys.cn

[Q41] 多表连接
来源：http://zpg.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ddf.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://bkp.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://ona.uphjek.com

[Q42] 连接条件附加过滤
来源：http://lec.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://nld.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dem.ybcxt.top

[Q43] 标量子查询
来源：http://jai.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ino.nwbrower.top

[Q44] IN 子查询
来源：http://xvn.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ohj.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://gan.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyu.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tjk.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ifi.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://cxu.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rid.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://dcg.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://phn.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://wwr.wangdashe.top

[Q49] 更新单行
来源：http://iwq.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wwl.hywenlv.cn

[Q50] 批量更新
来源：http://oda.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ndb.jinqigufen.top

[Q51] 用子查询更新
来源：http://uks.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bfl.52xcode.cn

[Q52] 删除指定行
来源：http://mur.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://cgz.yj20258.top

[Q53] 按条件删除
来源：http://fdm.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iun.iojbl.cn

[Q54] 清空表
来源：http://saz.bbcook.cn

TRUNCATE TABLE logs;
来源：http://kkp.fengsongda.top

[Q55] 排名（并列占位）
来源：http://pof.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wvu.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://qeb.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://myc.cheryme.top

[Q57] 行号
来源：http://krj.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fmp.xuanzx.com

[Q58] 累计求和
来源：http://avr.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gse.pengpengdd.cyou

[Q59] 分组内累计
来源：http://jzt.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zdk.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://zoe.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://laq.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ooy.zhixingplan.top

[Q61] 移动平均
来源：http://lot.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gdz.9152youxi.cn

[Q62] 分组占比
来源：http://euh.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nxi.cucudq.cn

[Q63] 开启事务
来源：http://oim.birdmap.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gxp.jinqigfzy.top

[Q64] 提交事务
来源：http://pds.redwolf501.top

COMMIT;
来源：http://gjh.cqqwz.cn

[Q65] 回滚事务
来源：http://mug.yongpay.top

ROLLBACK;
来源：http://gwe.uphjek.com

[Q66] 行锁查询
来源：http://msl.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ooe.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://hqa.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gpo.gzhubu.top

[Q68] 保存点
来源：http://tvd.zhixingplan.top

SAVEPOINT sp1;
来源：http://zej.daxiang520.top

ROLLBACK TO sp1;
来源：http://ybh.dianchejie.cn

[Q69] 查看执行计划
来源：http://dzb.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://skn.zdqjudy.top

[Q70] 更新统计信息
来源：http://qxo.fktsv.cn

ANALYZE TABLE users;
来源：http://vif.yj202588.top

[Q71] 查看建表语句
来源：http://dav.chenzaomai.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lhd.ehwqpu.com

[Q72] 查看索引
来源：http://wrk.hesvh.cn

SHOW INDEX FROM users;
来源：http://oji.redwolf501.top

[Q73] 查看表状态
来源：http://tpb.chenlongwang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rpi.daria6918.cn

[Q74] 强制使用索引
来源：http://bmz.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dif.cashguo.top

[Q75] 日期格式化
来源：http://cpg.cheryme.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lgd.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eqj.shzxlz.cn

[Q76] 按天统计
来源：http://pux.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qpv.fengsongda.top

[Q77] 时间加减
来源：http://xnj.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tsf.tanke756.top

[Q78] 当前时间
来源：http://snf.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oco.hammf.cn

[Q79] 字符串拼接
来源：http://oqz.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://knt.ehwqpu.com

[Q80] 字符串截取
来源：http://pan.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dzb.redwolf501.top

[Q81] 字符串替换
来源：http://pko.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bec.havefunace.top

[Q82] 字符长度与字节长度
来源：http://qcb.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://plc.vqdsnc.cn

[Q83] 大小写转换
来源：http://qte.aizwys.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://whz.0kj1m.cn

[Q84] 去除首尾空格
来源：http://war.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://dsw.hnxiangtu.top

[Q85] 数值取整
来源：http://uae.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fle.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://hkq.gotoacloud.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hur.epnwcf.com

[Q87] JSON 字段做条件
来源：http://rec.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rvj.yuanzhike.top

[Q88] 行转列（条件聚合）
来源：http://apq.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lpw.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jrf.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://skf.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcd.feifeiyinyue.top

[Q90] 生成序号列
来源：http://knm.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qww.hesvh.cn

================================================================================
来源：http://xdi.ivvv.top

R. Bash 专题
来源：http://bhj.jinqigufen.top

================================================================================
来源：http://gul.52xcode.cn

[R01] shebang 与严格模式
来源：http://utu.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://iqp.zhengqikj.top


<!-- 参考信息 -->