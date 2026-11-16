代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://mbc.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sra.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://vxp.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://qso.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zue.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gvb.yonumen.top

Ruby: threads.map(&:join)
来源：http://iom.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kfr.zhoulong.xyz

[O06] 使用进程池
来源：http://cjy.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qja.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tet.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://ang.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://mkf.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tsc.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zxq.hongshengwenyu.top

Ruby: // fork 块
来源：http://okx.shangyingyoupin.top

C#:   Parallel.For
来源：http://xsq.tarul.cn

================================================================================
来源：http://vqt.pycfn.com

P. 常用工具函数
来源：http://nem.haohaochexian.top

================================================================================
来源：http://iqk.zhiwuduotai.top

[P01] 生成 UUID
来源：http://wuv.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://ebl.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qae.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://mlb.ivvv.top

TS:   crypto.randomUUID()
来源：http://xzg.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://nfn.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://fri.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://mdh.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://oku.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://rfg.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vzf.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yck.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cwn.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qrl.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://orh.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qaa.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gum.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wnw.fktsv.cn

[P03] 生成短随机字符串
来源：http://fsf.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://htd.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fid.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgc.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qob.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vrf.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cum.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://des.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yuv.zycfv.cn

[P04] 求长度
来源：http://saw.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qso.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gum.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uzf.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qsl.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://wnp.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://wly.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://sxp.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bvn.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://cex.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jvu.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://obw.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wbp.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://diq.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://and.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://lid.xuanzx.com

Ruby: a == b
来源：http://ubq.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cpc.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gzs.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ctw.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://btx.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gjf.snrcjt.cn

TS:   if (x == null) {}
来源：http://drq.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bbi.snrcjt.cn

Go:   if x == nil {}
来源：http://tix.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dyh.hcnkem.com

C#:   if (x is null) {}
来源：http://bvo.redwolf501.top

[P07] 防抖与节流
来源：http://wfm.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qot.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://weu.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tst.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hoc.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://agb.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vtk.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xla.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gvk.tanke756.top

[P08] 处理浮点精度问题
来源：http://gix.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eez.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zyy.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xba.sweek.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sxx.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://esp.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://khh.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hzl.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xrk.jqgufenzy.top

================================================================================
来源：http://yga.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://itj.redwolf501.top

================================================================================
来源：http://qxq.fengsongda.top

[Q01] 创建表
来源：http://npa.hcnkem.com

CREATE TABLE users (
来源：http://jbq.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://upw.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://adi.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://jrz.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nba.jqgfzy.top

);
来源：http://yvn.yj20258888.top

[Q02] 创建带外键的表
来源：http://zok.gogol.net.cn

CREATE TABLE orders (
来源：http://kjy.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zon.fehbvm.com

user_id INT NOT NULL,
来源：http://lbk.ivvv.top

amount DECIMAL(10, 2),
来源：http://fxz.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bke.mhx1999.top

);
来源：http://xlz.hysaishi.cn

[Q03] 增加列
来源：http://cgp.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zxj.chenzaomai.com

[Q04] 修改列类型
来源：http://dii.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zag.jyoumei.cn

[Q05] 重命名列
来源：http://izs.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vtk.yuanzhike.top

[Q06] 删除列
来源：http://gyw.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://leu.316326.xyz

[Q07] 删除表
来源：http://aae.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://afn.316326.xyz

[Q08] 创建普通索引
来源：http://qqm.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lho.andypj.xyz

[Q09] 创建唯一索引
来源：http://cih.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uqt.cdnleiting.top

[Q10] 插入单行
来源：http://dkv.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://utd.snrcjt.cn

[Q11] 一次插入多行
来源：http://ick.dianchejie.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mmu.cashguo.top

[Q12] 插入后取自增 ID
来源：http://jtj.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://buv.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vbx.sufxvd.cn

[Q13] 忽略重复插入
来源：http://zwz.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zgk.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://iys.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iid.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fez.hcnkem.com

[Q15] 查询全部
来源：http://apg.guowangkeji.top

SELECT * FROM users;
来源：http://zhw.cucudq.cn

[Q16] 查询指定列
来源：http://ucf.wangdashe.top

SELECT id, name FROM users;
来源：http://sam.fengsongda.top

[Q17] 条件查询
来源：http://vbv.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://egz.zhixingplan.top

[Q18] 模糊匹配
来源：http://qqd.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dsl.gzhubu.top

[Q19] 范围查询
来源：http://zup.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ith.yj20258888.top

[Q20] IN 列表
来源：http://umt.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ezq.zdqjudy.top

[Q21] 空值判断
来源：http://aem.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://olk.zdbjq.cn

[Q22] 排序
来源：http://mak.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rak.yvedp.cn

[Q23] 分页
来源：http://ows.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://asg.daria6918.cn

[Q24] 去重
来源：http://ivs.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://vcb.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://oln.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://itz.cucudq.cn

[Q26] 计数
来源：http://ver.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://eme.vehdjk.com

[Q27] 条件计数
来源：http://qcl.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eiy.ehwqpu.com

[Q28] 求和与平均
来源：http://tsq.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ift.wangdashe.top

[Q29] 最大最小值
来源：http://ifj.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hmg.jlsjyb.cn

[Q30] 分组统计
来源：http://xet.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ext.cheryme.top

[Q31] 分组后过滤
来源：http://dhu.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jtp.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://omw.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ggc.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vuf.nanxuanxn.top

[Q33] 多列分组
来源：http://efh.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gxt.ppjwa.cn

[Q34] 每组取第一条
来源：http://tvw.316326.xyz

SELECT * FROM (
来源：http://ddw.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xlk.guowangkeji.top

) t WHERE rn = 1;
来源：http://tjw.meibo888.top

[Q35] 内连接
来源：http://dyb.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jfb.gaohongyu789.top

[Q36] 左连接
来源：http://jlz.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://syv.fktsv.cn

[Q37] 右连接
来源：http://qaj.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iiv.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://sav.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xsf.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://kux.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xmp.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://swe.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pvu.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vnf.aibaodan.cn

[Q41] 多表连接
来源：http://opx.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://upf.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://syu.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://bae.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://qbf.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://ima.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qci.redwolf501.top

[Q43] 标量子查询
来源：http://ayh.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dfy.yj20258.top

[Q44] IN 子查询
来源：http://ayx.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hxy.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://sld.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://try.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://mwj.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tve.ydzc1.top

[Q47] 与平均值比较
来源：http://nun.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cqt.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://xne.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pcs.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://zec.yj202588.top

[Q49] 更新单行
来源：http://doq.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qvf.shzxlz.cn

[Q50] 批量更新
来源：http://rww.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oah.hnxiangtu.top

[Q51] 用子查询更新
来源：http://ujd.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pjj.daxiang520.top

[Q52] 删除指定行
来源：http://vpk.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://yha.yanxiufei.cn

[Q53] 按条件删除
来源：http://kfr.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gmv.nwbrower.top

[Q54] 清空表
来源：http://qsi.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://rzl.mhx1999.top

[Q55] 排名（并列占位）
来源：http://nqy.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://klq.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://dej.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://axz.hfpthk.cn

[Q57] 行号
来源：http://lwv.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sgk.jqgfzy.top

[Q58] 累计求和
来源：http://spj.xuetiantiany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kgg.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://vir.xingfuxueyuan.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sek.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://ehv.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nvx.yj20258888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rgv.sweek.top

[Q61] 移动平均
来源：http://cqp.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ofg.gzhubu.top

[Q62] 分组占比
来源：http://qsp.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://leh.shangyingyoupin.top

[Q63] 开启事务
来源：http://ofb.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xbp.cashguo.top

[Q64] 提交事务
来源：http://xlb.havefunace.top

COMMIT;
来源：http://gdk.feifeiyinyue.top

[Q65] 回滚事务
来源：http://ekf.tian-w.cn

ROLLBACK;
来源：http://znz.feifeiyinyue.top

[Q66] 行锁查询
来源：http://dyd.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dst.fengsongda.top

[Q67] 设置隔离级别
来源：http://zok.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ohh.tianlin.xyz

[Q68] 保存点
来源：http://rbx.tarul.cn

SAVEPOINT sp1;
来源：http://sez.hfpthk.cn

ROLLBACK TO sp1;
来源：http://sdw.hcnkem.com

[Q69] 查看执行计划
来源：http://gvc.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mbh.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://yds.meibo888.top

ANALYZE TABLE users;
来源：http://jft.hammf.cn

[Q71] 查看建表语句
来源：http://awk.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eoc.xuanzx.com

[Q72] 查看索引
来源：http://yny.ydjk.org.cn

SHOW INDEX FROM users;
来源：http://ctq.zhijiandao.cn

[Q73] 查看表状态
来源：http://jeg.redwolf501.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dkm.zhijiandao.cn

[Q74] 强制使用索引
来源：http://seu.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hky.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://oyl.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zqx.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qcw.pycfn.com

[Q76] 按天统计
来源：http://erm.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kas.jqgufenzy.top

[Q77] 时间加减
来源：http://inq.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://avi.snrcjt.cn

[Q78] 当前时间
来源：http://jyf.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hsf.zhiwuduotai.top

[Q79] 字符串拼接
来源：http://gif.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://buf.dianchejie.cn

[Q80] 字符串截取
来源：http://lka.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rxm.nwbrower.top

[Q81] 字符串替换
来源：http://dds.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iza.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://snz.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://try.dashuyun.cn

[Q83] 大小写转换
来源：http://iqh.fehbvm.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://exn.hfpthk.cn

[Q84] 去除首尾空格
来源：http://lsf.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://uhi.jiagoushi.top

[Q85] 数值取整
来源：http://kpu.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bjk.yj202588.top

[Q86] 读取 JSON 字段
来源：http://wbb.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xdm.yvedp.cn

[Q87] JSON 字段做条件
来源：http://iem.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zlk.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://ipf.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zmd.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tsa.dashuyun.cn

[Q89] 判断表是否存在
来源：http://rdy.ctjpmb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mzq.yanxiufei.cn

[Q90] 生成序号列
来源：http://ylr.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dyi.vehdjk.com

================================================================================
来源：http://pfq.fengsongda.top


<!-- 参考信息 -->