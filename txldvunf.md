代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bmr.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tda.cashguo.top

Ruby: threads.map(&:join)
来源：http://woy.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://syw.gotoacloud.top

[O06] 使用进程池
来源：http://hwn.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vsl.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ssu.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://lrk.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://fih.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xxn.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rew.feifeiyinyue.top

Ruby: // fork 块
来源：http://xfy.c1oappe.top

C#:   Parallel.For
来源：http://mhb.zhiwuduotai.top

================================================================================
来源：http://wtr.vqdsnc.cn

P. 常用工具函数
来源：http://fce.haohaochexian.top

================================================================================
来源：http://brj.guannengcc.top

[P01] 生成 UUID
来源：http://ldp.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://qee.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://evb.yvedp.cn

JS:   crypto.randomUUID()
来源：http://yxb.316326.xyz

TS:   crypto.randomUUID()
来源：http://ljd.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://rqa.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://jxr.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://wdq.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://rgu.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://gwb.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bgz.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iig.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hbp.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://enb.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tao.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzj.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jil.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ubh.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://rbd.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhf.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mlp.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://taw.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://air.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cql.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uid.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sub.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jye.ctjpmb.com

[P04] 求长度
来源：http://ukt.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxa.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fxm.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://afw.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nli.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://ipj.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://cen.yj202588.top

Ruby: x.length;  x.size
来源：http://pmf.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xqc.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://lon.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ugv.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rws.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ihw.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hmx.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmb.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pas.yvedp.cn

Ruby: a == b
来源：http://nxq.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytj.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gnl.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cfl.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://azc.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hmg.nanxuanxn.top

TS:   if (x == null) {}
来源：http://vfl.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://glm.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://dtj.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zbw.yueranfly.top

C#:   if (x is null) {}
来源：http://vdd.ydjk.org.cn

[P07] 防抖与节流
来源：http://nac.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ory.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://hrb.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ebb.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wuu.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jzm.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eti.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pic.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lpf.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://xjh.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://urn.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lzw.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tms.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uok.shanyushiyangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pxm.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sua.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tnw.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bkp.yvedp.cn

================================================================================
来源：http://ojg.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mmn.guannengcc.top

================================================================================
来源：http://fey.xuetiantiany.cn

[Q01] 创建表
来源：http://agz.xziqi.cn

CREATE TABLE users (
来源：http://puj.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwj.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://qnm.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://cry.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lbh.fehbvm.com

);
来源：http://iqf.uphjek.com

[Q02] 创建带外键的表
来源：http://gng.c1oappe.top

CREATE TABLE orders (
来源：http://xyz.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dph.nanxuanxn.top

user_id INT NOT NULL,
来源：http://xhs.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://dnu.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zdp.fzhhl.top

);
来源：http://dwc.yangfankeji.com

[Q03] 增加列
来源：http://tkv.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cmq.tianlin.xyz

[Q04] 修改列类型
来源：http://izn.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://omw.yuxming.cn

[Q05] 重命名列
来源：http://eoe.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ium.xziqi.cn

[Q06] 删除列
来源：http://dhv.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vry.shuidangran.top

[Q07] 删除表
来源：http://mfq.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://mhe.yj20258.top

[Q08] 创建普通索引
来源：http://ksf.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://nov.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://itb.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jip.yvedp.cn

[Q10] 插入单行
来源：http://kwo.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mec.nanxuanxn.top

[Q11] 一次插入多行
来源：http://wmg.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rny.xinyue.icu

[Q12] 插入后取自增 ID
来源：http://jih.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://fhj.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hxb.ctjpmb.com

[Q13] 忽略重复插入
来源：http://ncv.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qpx.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://ioq.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://prs.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zel.tarul.cn

[Q15] 查询全部
来源：http://zlo.zhengqikj.top

SELECT * FROM users;
来源：http://xmk.hysaishi.cn

[Q16] 查询指定列
来源：http://aei.jinqigfzy.top

SELECT id, name FROM users;
来源：http://vfe.shuidangran.top

[Q17] 条件查询
来源：http://fat.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ber.sweek.top

[Q18] 模糊匹配
来源：http://wmz.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ojm.yj20258888.top

[Q19] 范围查询
来源：http://glu.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hvp.cucudq.cn

[Q20] IN 列表
来源：http://fyy.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oaz.zhongyouzk.top

[Q21] 空值判断
来源：http://qrj.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jqg.yvedp.cn

[Q22] 排序
来源：http://ele.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pxi.shanyushiyangkeji.top

[Q23] 分页
来源：http://ogf.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qwg.shanyushiyangkeji.top

[Q24] 去重
来源：http://rdj.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://fqx.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://uvd.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zfz.ydjk.org.cn

[Q26] 计数
来源：http://irb.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://wyt.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://sol.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rbc.yj20258.top

[Q28] 求和与平均
来源：http://sio.kuanghao11.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vii.nanxuanxn.top

[Q29] 最大最小值
来源：http://leu.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xlr.jiagoushi.top

[Q30] 分组统计
来源：http://gat.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qdd.hesvh.cn

[Q31] 分组后过滤
来源：http://ljc.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kor.fktsv.cn

[Q32] 分组拼接字符串
来源：http://pyg.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ain.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://orr.fengsongda.top

[Q33] 多列分组
来源：http://bab.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zsm.vqdsnc.cn

[Q34] 每组取第一条
来源：http://rnf.andypj.xyz

SELECT * FROM (
来源：http://lzs.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uml.hesvh.cn

) t WHERE rn = 1;
来源：http://gqf.cheryme.top

[Q35] 内连接
来源：http://zhk.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxg.ctjpmb.com

[Q36] 左连接
来源：http://ajo.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dwi.fehbvm.com

[Q37] 右连接
来源：http://uic.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fsy.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://mll.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lxa.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://mjt.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zry.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ixw.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xfd.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://anq.yvedp.cn

[Q41] 多表连接
来源：http://hql.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://qla.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://vrz.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://dzl.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://yzu.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://dst.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tpn.yanxiufei.cn

[Q43] 标量子查询
来源：http://wxx.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vij.pengpengdd.cyou

[Q44] IN 子查询
来源：http://tzv.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ncr.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://cua.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iay.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://nph.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qpa.sysykeji.top

[Q47] 与平均值比较
来源：http://dyc.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dvu.cqqwz.cn

[Q48] CTE 公用表表达式
来源：http://dyk.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hql.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://bvy.birdmap.top

[Q49] 更新单行
来源：http://wuq.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://szo.316326.xyz

[Q50] 批量更新
来源：http://nzb.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bvj.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://hgn.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ttz.haohaochexian.top

[Q52] 删除指定行
来源：http://dyn.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://mfq.tarul.cn

[Q53] 按条件删除
来源：http://yjl.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sgx.smart0.xyz

[Q54] 清空表
来源：http://xtq.daxiang520.top

TRUNCATE TABLE logs;
来源：http://uih.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://fpc.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ock.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://ojj.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://job.smart0.xyz

[Q57] 行号
来源：http://mxx.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vrr.tarul.cn

[Q58] 累计求和
来源：http://qtz.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pta.zhixingplan.top

[Q59] 分组内累计
来源：http://dng.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zvu.cdnleiting.top

[Q60] 取上一行 / 下一行
来源：http://vte.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wwm.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vqf.zdqjudy.top

[Q61] 移动平均
来源：http://lfq.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aaq.tian-w.cn

[Q62] 分组占比
来源：http://uml.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xyp.hammf.cn

[Q63] 开启事务
来源：http://lpv.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wwk.sjlbkw.cn

[Q64] 提交事务
来源：http://fcj.xinyue.icu

COMMIT;
来源：http://hnp.aizwys.cn

[Q65] 回滚事务
来源：http://hjt.yongpay.top

ROLLBACK;
来源：http://ydj.gogol.net.cn

[Q66] 行锁查询
来源：http://kuq.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://noj.epnwcf.com

[Q67] 设置隔离级别
来源：http://pfx.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ota.tanke756.top

[Q68] 保存点
来源：http://nqv.jyoumei.cn

SAVEPOINT sp1;
来源：http://ozl.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://pnm.jinqigufen.top

[Q69] 查看执行计划
来源：http://sjw.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zdc.jiagoushi.top

[Q70] 更新统计信息
来源：http://ehg.gaohongyu789.top

ANALYZE TABLE users;
来源：http://rcx.yanxiufei.cn

[Q71] 查看建表语句
来源：http://yha.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wdy.xziqi.cn

[Q72] 查看索引
来源：http://blg.yueranfly.top

SHOW INDEX FROM users;
来源：http://jwx.nwbrower.top

[Q73] 查看表状态
来源：http://tum.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tkk.xziqi.cn

[Q74] 强制使用索引
来源：http://dld.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vpc.bjfxy.top

[Q75] 日期格式化
来源：http://mjw.mhx1999.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://liu.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qbf.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://bkt.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aqc.zhengqikj.top

[Q77] 时间加减
来源：http://lwc.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rxx.uphjek.com

[Q78] 当前时间
来源：http://auk.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gza.hysaishi.cn

[Q79] 字符串拼接
来源：http://vle.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bah.yangfankeji.com

[Q80] 字符串截取
来源：http://ive.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fws.cucudq.cn

[Q81] 字符串替换
来源：http://mgt.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zna.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://hao.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://udh.ehwqpu.com

[Q83] 大小写转换
来源：http://pdh.nanxuanxn.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bld.yj202588.top

[Q84] 去除首尾空格
来源：http://vmh.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://smk.tian-w.cn

[Q85] 数值取整
来源：http://mvq.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xwa.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://tch.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iro.pycfn.com

[Q87] JSON 字段做条件
来源：http://rlk.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eap.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://dus.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mww.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lnm.tian-w.cn

[Q89] 判断表是否存在
来源：http://sjd.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bgd.pycfn.com

[Q90] 生成序号列
来源：http://dvs.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zwb.zycfv.cn

================================================================================
来源：http://jrb.yj20258.top

R. Bash 专题
来源：http://zmk.sxryk.cn

================================================================================
来源：http://snh.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://zoa.52xcode.cn

#!/usr/bin/env bash
来源：http://xob.yj20258.top


<!-- 参考信息 -->