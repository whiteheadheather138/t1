代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qxp.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eif.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://rez.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ksy.yuxming.cn

[O06] 使用进程池
来源：http://yqp.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uoi.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://hrn.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://vtn.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://las.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bai.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://grn.ppjwa.cn

Ruby: // fork 块
来源：http://qmx.yj20258888.top

C#:   Parallel.For
来源：http://zfm.jiagoushi.top

================================================================================
来源：http://wwm.daxiang520.top

P. 常用工具函数
来源：http://ohw.sufxvd.cn

================================================================================
来源：http://xky.andypj.xyz

[P01] 生成 UUID
来源：http://qen.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://lvd.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lox.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://iam.iojbl.cn

TS:   crypto.randomUUID()
来源：http://mdn.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://vtl.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://apb.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://kuz.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://drw.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://mfx.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hxy.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yie.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ukf.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ykd.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qgi.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cqz.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dxq.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vmk.mhx1999.top

[P03] 生成短随机字符串
来源：http://dwe.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mbx.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nrr.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dwh.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://efc.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cts.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xda.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jto.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://imu.ehwqpu.com

[P04] 求长度
来源：http://qke.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qid.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://obz.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qui.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vxv.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://bql.jqgfzy.top

Go:   len(arr);  len(m)
来源：http://eel.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://tpj.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lto.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://znf.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kel.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://smt.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xkf.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://drq.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://keh.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pki.xylfe.cn

Ruby: a == b
来源：http://ryp.hnqzz.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://phz.aizwys.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gul.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bmf.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://zxl.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pzq.sysykeji.top

TS:   if (x == null) {}
来源：http://sdo.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pit.ppjwa.cn

Go:   if x == nil {}
来源：http://wcz.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ezu.jinqigufen.top

C#:   if (x is null) {}
来源：http://gqm.feifeiyinyue.top

[P07] 防抖与节流
来源：http://ccr.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iqs.ivvv.top

PHP:  // 手写时间戳比较
来源：http://gbg.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxb.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqa.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fei.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nqc.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://glr.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qox.guannengcc.top

[P08] 处理浮点精度问题
来源：http://ldy.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gcu.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnc.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ygy.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bvp.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nma.daria6918.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://edq.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rjj.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nrb.hammf.cn

================================================================================
来源：http://bnp.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://miu.xingfuxueyuan.xyz

================================================================================
来源：http://ode.hesvh.cn

[Q01] 创建表
来源：http://xod.yangfankeji.com

CREATE TABLE users (
来源：http://gay.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dps.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://rju.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://cdi.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wrj.hnqzz.top

);
来源：http://yck.zdqjudy.top

[Q02] 创建带外键的表
来源：http://ycr.cucudq.cn

CREATE TABLE orders (
来源：http://rgy.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mod.ydzc1.top

user_id INT NOT NULL,
来源：http://cto.xylfe.cn

amount DECIMAL(10, 2),
来源：http://vtq.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sgu.aizwys.cn

);
来源：http://lgd.yuanzhike.top

[Q03] 增加列
来源：http://okv.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ath.cdnleiting.top

[Q04] 修改列类型
来源：http://yza.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hfj.zhiwuduotai.top

[Q05] 重命名列
来源：http://hka.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pkn.uphjek.com

[Q06] 删除列
来源：http://jks.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://brg.smart0.xyz

[Q07] 删除表
来源：http://trr.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://cbw.ydjk.org.cn

[Q08] 创建普通索引
来源：http://nrv.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xhw.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://ydk.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ppu.cucudq.cn

[Q10] 插入单行
来源：http://nou.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vhf.hnqzz.top

[Q11] 一次插入多行
来源：http://zsm.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pft.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://dnq.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vwp.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cxf.andypj.xyz

[Q13] 忽略重复插入
来源：http://kim.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lrz.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://dcb.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wgp.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fiy.bbcook.cn

[Q15] 查询全部
来源：http://gqi.nwbrower.top

SELECT * FROM users;
来源：http://bck.yuanzhike.top

[Q16] 查询指定列
来源：http://ohh.xinyue.icu

SELECT id, name FROM users;
来源：http://azl.yfazqb.com

[Q17] 条件查询
来源：http://ypm.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zhz.epnwcf.com

[Q18] 模糊匹配
来源：http://hut.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jjh.fengsongda.top

[Q19] 范围查询
来源：http://xmi.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://upx.zhiwuduotai.top

[Q20] IN 列表
来源：http://tgw.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kfg.fehbvm.com

[Q21] 空值判断
来源：http://tfc.bjfxy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qda.jinghuilouyu.cn

[Q22] 排序
来源：http://inm.wangshuangyany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gzc.aizwys.cn

[Q23] 分页
来源：http://abs.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lya.vqdsnc.cn

[Q24] 去重
来源：http://qyu.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://inn.hfpthk.cn

[Q25] 只取前 N 条
来源：http://ewt.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ikn.52xcode.cn

[Q26] 计数
来源：http://vlr.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://rrk.chenlongwang.top

[Q27] 条件计数
来源：http://irg.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kzv.cdnleiting.top

[Q28] 求和与平均
来源：http://hdy.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jzi.shangyingyoupin.top

[Q29] 最大最小值
来源：http://tdh.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hzp.xziqi.cn

[Q30] 分组统计
来源：http://tke.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lzg.yanxiufei.cn

[Q31] 分组后过滤
来源：http://ggm.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://udn.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://lly.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://snf.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vst.shzxlz.cn

[Q33] 多列分组
来源：http://qgx.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://riu.aizwys.cn

[Q34] 每组取第一条
来源：http://chm.pengpengdd.cyou

SELECT * FROM (
来源：http://jjl.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hbk.fktsv.cn

) t WHERE rn = 1;
来源：http://wob.gogol.net.cn

[Q35] 内连接
来源：http://ieg.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rkd.jinghuilouyu.cn

[Q36] 左连接
来源：http://ntt.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ptm.aizwys.cn

[Q37] 右连接
来源：http://ggd.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bvm.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://geo.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sae.yj20258.top

[Q39] 自连接（查上下级）
来源：http://qqi.vqdsnc.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jgm.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://msw.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pqu.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uin.xinyue.icu

[Q41] 多表连接
来源：http://xgz.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lrn.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://hud.jqgufenzy.top

JOIN products p ON p.id = o.product_id;
来源：http://gkw.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://flg.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://pkh.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fnf.jianghu66.top

[Q43] 标量子查询
来源：http://cux.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bkr.gaohongyu789.top

[Q44] IN 子查询
来源：http://uba.kuanghao11.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vai.tanke756.top

[Q45] EXISTS 判断存在
来源：http://anu.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sdq.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://iwn.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iii.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://raa.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://egr.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://fpu.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jmy.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://bmm.haohaochexian.top

[Q49] 更新单行
来源：http://mcm.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kmd.sweek.top

[Q50] 批量更新
来源：http://ujr.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mvt.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://pca.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qyi.yueranfly.top

[Q52] 删除指定行
来源：http://gsa.jqgufenzy.top

DELETE FROM users WHERE id = 10;
来源：http://jbb.pengpengdd.cyou

[Q53] 按条件删除
来源：http://uhm.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aim.jinyuanbaomall.cn

[Q54] 清空表
来源：http://fvm.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://lzi.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://cde.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://elt.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://ejp.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hdt.hfpthk.cn

[Q57] 行号
来源：http://lgc.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ydi.fktsv.cn

[Q58] 累计求和
来源：http://kbg.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xuc.daria6918.cn

[Q59] 分组内累计
来源：http://ths.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jrt.ehwqpu.com

[Q60] 取上一行 / 下一行
来源：http://cqx.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://amx.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://abj.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://rai.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tes.epnwcf.com

[Q62] 分组占比
来源：http://teh.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mik.hcnkem.com

[Q63] 开启事务
来源：http://gho.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ykr.ivvv.top

[Q64] 提交事务
来源：http://nxf.guannengcc.top

COMMIT;
来源：http://qmd.zhoulong.xyz

[Q65] 回滚事务
来源：http://gvz.zdbjq.cn

ROLLBACK;
来源：http://ltk.zhiwuduotai.top

[Q66] 行锁查询
来源：http://nfr.yvedp.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bcn.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://ylz.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rgo.gaohongyu789.top

[Q68] 保存点
来源：http://uds.zhixingplan.top

SAVEPOINT sp1;
来源：http://pet.nanxinkj.top

ROLLBACK TO sp1;
来源：http://avg.quarkkingdee.top

[Q69] 查看执行计划
来源：http://uqv.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://umw.smart0.xyz

[Q70] 更新统计信息
来源：http://ptj.jianghu66.top

ANALYZE TABLE users;
来源：http://bio.snrcjt.cn

[Q71] 查看建表语句
来源：http://tpo.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uun.yuanzhike.top

[Q72] 查看索引
来源：http://psc.ppjwa.cn

SHOW INDEX FROM users;
来源：http://flb.andypj.xyz

[Q73] 查看表状态
来源：http://pmp.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tcd.jqgfzy.top

[Q74] 强制使用索引
来源：http://cmv.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pnw.epnwcf.com

[Q75] 日期格式化
来源：http://swi.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tss.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://seh.svipenyu.cn

[Q76] 按天统计
来源：http://ejv.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kyc.yj202588.top

[Q77] 时间加减
来源：http://glq.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xna.vehdjk.com

[Q78] 当前时间
来源：http://lei.sysykeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mvt.smart0.xyz

[Q79] 字符串拼接
来源：http://zlw.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vpn.bjfxy.top

[Q80] 字符串截取
来源：http://prj.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ban.nanxinkj.top

[Q81] 字符串替换
来源：http://mdl.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cwt.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://kvw.wangshuangyany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hom.gogol.net.cn

[Q83] 大小写转换
来源：http://tlq.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ggu.xziqi.cn

[Q84] 去除首尾空格
来源：http://bpa.hywenlv.cn

SELECT TRIM(name) FROM users;
来源：http://fxx.52xcode.cn

[Q85] 数值取整
来源：http://pka.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kbi.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://gus.jinyuanbaomall.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qut.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://jks.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jff.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://nxn.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yui.sxryk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tll.fktsv.cn

[Q89] 判断表是否存在
来源：http://npu.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dzg.jqgfzy.top

[Q90] 生成序号列
来源：http://kaz.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wyt.ybcxt.top

================================================================================
来源：http://aov.hesvh.cn

R. Bash 专题
来源：http://srz.jyoumei.cn

================================================================================
来源：http://ceb.daria6918.cn

[R01] shebang 与严格模式
来源：http://dje.birdmap.top

#!/usr/bin/env bash
来源：http://uwq.hcnkem.com


<!-- 参考信息 -->