代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwa.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://liy.52xcode.cn

Ruby: threads.map(&:join)
来源：http://ojo.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://imb.hfpthk.cn

[O06] 使用进程池
来源：http://tgx.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hvs.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ufl.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://gdb.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://hwz.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tdk.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zak.ydzc1.top

Ruby: // fork 块
来源：http://vqy.shangyingyoupin.top

C#:   Parallel.For
来源：http://qvj.daria6918.cn

================================================================================
来源：http://wwq.kuanghao11.cn

P. 常用工具函数
来源：http://ocr.epnwcf.com

================================================================================
来源：http://nib.zhengqikj.top

[P01] 生成 UUID
来源：http://fnj.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://puk.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ixu.fengsongda.top

JS:   crypto.randomUUID()
来源：http://qje.xuanzx.com

TS:   crypto.randomUUID()
来源：http://tuk.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://qht.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://ebw.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://ryh.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://loz.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://bdd.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dbm.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://klu.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gyy.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cvf.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oxo.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzx.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sxg.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lwm.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://ebt.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xgu.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pwr.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvv.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vzd.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://psj.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://plj.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://wam.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vim.guowangkeji.top

[P04] 求长度
来源：http://thw.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnr.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfz.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nds.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggm.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://zuy.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://gfy.mhx1999.top

Ruby: x.length;  x.size
来源：http://zpl.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://nhy.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://bds.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://bwz.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bul.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vrz.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://koo.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ywl.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://dww.cheryme.top

Ruby: a == b
来源：http://drv.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zrq.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vwp.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ubf.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://iuy.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://icd.smart0.xyz

TS:   if (x == null) {}
来源：http://xxn.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ays.sweek.top

Go:   if x == nil {}
来源：http://lki.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://krq.zhengqikj.top

C#:   if (x is null) {}
来源：http://nmc.tian-w.cn

[P07] 防抖与节流
来源：http://rkb.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sqj.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://dds.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpr.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfv.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qch.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uuw.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lzx.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dik.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://wsn.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qrf.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lff.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://egh.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ptl.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aay.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xax.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nkc.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://swo.hnqzz.top

================================================================================
来源：http://uco.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ygz.jianghu66.top

================================================================================
来源：http://bej.yangfankeji.com

[Q01] 创建表
来源：http://gdi.jinqigufen.top

CREATE TABLE users (
来源：http://gmx.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zac.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://mxg.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://hfg.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tbr.nanxuanxn.top

);
来源：http://cgi.ctjpmb.com

[Q02] 创建带外键的表
来源：http://edn.jqgufenzy.top

CREATE TABLE orders (
来源：http://toa.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzg.cqqwz.cn

user_id INT NOT NULL,
来源：http://pma.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://otr.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zxj.ywan-chungtsiang.top

);
来源：http://kki.haohaochexian.top

[Q03] 增加列
来源：http://cfs.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://drv.chenlongwang.top

[Q04] 修改列类型
来源：http://jsv.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zwj.yanxiufei.cn

[Q05] 重命名列
来源：http://tzc.zhoulong.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://abv.nanxinkj.top

[Q06] 删除列
来源：http://fld.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eqn.jiagoushi.top

[Q07] 删除表
来源：http://hwi.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://kiv.jyoumei.cn

[Q08] 创建普通索引
来源：http://vaa.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://xuy.xylfe.cn

[Q09] 创建唯一索引
来源：http://vrv.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jpr.jinqigfzy.top

[Q10] 插入单行
来源：http://slu.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ysy.jianghu66.top

[Q11] 一次插入多行
来源：http://fkj.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mco.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://duk.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qzf.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mrn.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://xwz.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fis.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://brs.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://edj.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yft.chenjidiqi.icu

[Q15] 查询全部
来源：http://bbd.jianghu66.top

SELECT * FROM users;
来源：http://bwu.redwolf501.top

[Q16] 查询指定列
来源：http://xdx.guowangkeji.top

SELECT id, name FROM users;
来源：http://tka.hnxiangtu.top

[Q17] 条件查询
来源：http://act.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://npl.xziqi.cn

[Q18] 模糊匹配
来源：http://zph.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qpi.guannengcc.top

[Q19] 范围查询
来源：http://mvr.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rob.jinqigfzy.top

[Q20] IN 列表
来源：http://oqi.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ipz.316326.xyz

[Q21] 空值判断
来源：http://slq.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://dtk.xinyue.icu

[Q22] 排序
来源：http://yos.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kfw.mhx1999.top

[Q23] 分页
来源：http://oec.vqdsnc.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wot.yueranfly.top

[Q24] 去重
来源：http://sbf.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://clz.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://nzd.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zun.sysykeji.top

[Q26] 计数
来源：http://rqd.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://vxf.xuetiantiany.cn

[Q27] 条件计数
来源：http://vcc.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://beb.aibaodan.cn

[Q28] 求和与平均
来源：http://isg.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dlp.hysaishi.cn

[Q29] 最大最小值
来源：http://dcl.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uzd.cucudq.cn

[Q30] 分组统计
来源：http://jpe.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hpc.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://ufo.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tqz.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://set.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jfu.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lbo.yuanzhike.top

[Q33] 多列分组
来源：http://lvr.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://guo.ehwqpu.com

[Q34] 每组取第一条
来源：http://goq.quarkkingdee.top

SELECT * FROM (
来源：http://rjz.kuanghao11.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yna.gotoacloud.top

) t WHERE rn = 1;
来源：http://hzv.haohaochexian.top

[Q35] 内连接
来源：http://izz.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cvo.hywenlv.cn

[Q36] 左连接
来源：http://uxz.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sjd.chenjidiqi.icu

[Q37] 右连接
来源：http://xje.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gxy.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://apk.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yua.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://mlq.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kth.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dcz.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kbg.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vsn.mhx1999.top

[Q41] 多表连接
来源：http://grp.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://atc.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://clp.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://lzq.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://bma.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://czj.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://flo.haohaochexian.top

[Q43] 标量子查询
来源：http://dmr.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nhf.sweek.top

[Q44] IN 子查询
来源：http://kll.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ucz.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://ehl.svipenyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tdy.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lkr.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gge.wangdashe.top

[Q47] 与平均值比较
来源：http://qyy.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zfg.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://kps.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iwn.fanxiaobao.xyz

SELECT * FROM t WHERE c > 5;
来源：http://lib.yj20258888.top

[Q49] 更新单行
来源：http://qvr.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uca.aibaodan.cn

[Q50] 批量更新
来源：http://rmy.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftm.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://dsz.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kmr.svipenyu.cn

[Q52] 删除指定行
来源：http://lrr.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://uie.redwolf501.top

[Q53] 按条件删除
来源：http://ajw.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eep.bjfxy.top

[Q54] 清空表
来源：http://kxa.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://xzc.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://qjl.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sjs.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://lqp.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fps.xuanzx.com

[Q57] 行号
来源：http://ztq.tanke756.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zcs.zdbjq.cn

[Q58] 累计求和
来源：http://mpr.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kld.sjlbkw.cn

[Q59] 分组内累计
来源：http://zyi.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ser.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://ybo.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jax.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tdy.shanyushiyangtech.top

[Q61] 移动平均
来源：http://eul.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://var.gzhubu.top

[Q62] 分组占比
来源：http://enk.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://slc.0kj1m.cn

[Q63] 开启事务
来源：http://oxr.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tnx.sufxvd.cn

[Q64] 提交事务
来源：http://byp.jlsjyb.cn

COMMIT;
来源：http://kpb.jianghu66.top

[Q65] 回滚事务
来源：http://lus.sjlbkw.cn

ROLLBACK;
来源：http://wql.yangfankeji.com

[Q66] 行锁查询
来源：http://hji.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fpj.yonumen.top

[Q67] 设置隔离级别
来源：http://stb.pengpengdd.cyou

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yfx.ivvv.top

[Q68] 保存点
来源：http://nhl.xinyue.icu

SAVEPOINT sp1;
来源：http://bkl.birdmap.top

ROLLBACK TO sp1;
来源：http://dlq.svipenyu.cn

[Q69] 查看执行计划
来源：http://rkm.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://acx.smart0.xyz

[Q70] 更新统计信息
来源：http://ils.gogol.net.cn

ANALYZE TABLE users;
来源：http://dlt.smart0.xyz

[Q71] 查看建表语句
来源：http://fiq.epnwcf.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xmy.chenjidiqi.icu

[Q72] 查看索引
来源：http://gje.bjfxy.top

SHOW INDEX FROM users;
来源：http://oei.yj20258888.top

[Q73] 查看表状态
来源：http://kia.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://utj.ybcxt.top

[Q74] 强制使用索引
来源：http://wbz.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zfb.cdnleiting.top

[Q75] 日期格式化
来源：http://isv.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uib.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tga.ivvv.top

[Q76] 按天统计
来源：http://xva.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zzo.cucudq.cn

[Q77] 时间加减
来源：http://wpg.tianlin.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ovn.pengpengdd.cyou

[Q78] 当前时间
来源：http://wvi.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://prn.aizwys.cn

[Q79] 字符串拼接
来源：http://pyv.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tgy.chenlongwang.top

[Q80] 字符串截取
来源：http://ohs.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tka.yonumen.top

[Q81] 字符串替换
来源：http://lua.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://scs.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://hkp.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tgc.xylfe.cn

[Q83] 大小写转换
来源：http://bqy.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hsg.kuanghao11.cn

[Q84] 去除首尾空格
来源：http://ycz.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://dsg.hammf.cn

[Q85] 数值取整
来源：http://ozt.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dsy.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://ejw.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqa.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://jsj.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vaq.ybcxt.top

[Q88] 行转列（条件聚合）
来源：http://wzv.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://djq.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wni.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://wiu.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bjm.zhiwuduotai.top

[Q90] 生成序号列
来源：http://mwp.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ytm.yuxming.cn

================================================================================
来源：http://ilh.kuanghao11.cn

R. Bash 专题
来源：http://enr.hysaishi.cn

================================================================================
来源：http://rnf.meibo888.top

[R01] shebang 与严格模式
来源：http://aqs.yangfankeji.com

#!/usr/bin/env bash
来源：http://hfx.yj20258888.top


<!-- 参考信息 -->