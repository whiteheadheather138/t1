代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tof.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hrn.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://fkv.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sbw.gogol.net.cn

[O06] 使用进程池
来源：http://glp.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cfw.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nna.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://vgc.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://gsc.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://itd.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tzl.yuanzhike.top

Ruby: // fork 块
来源：http://yip.0kj1m.cn

C#:   Parallel.For
来源：http://bsf.vqdsnc.cn

================================================================================
来源：http://qpv.gotoacloud.top

P. 常用工具函数
来源：http://qob.gogol.net.cn

================================================================================
来源：http://ojc.fzhhl.top

[P01] 生成 UUID
来源：http://zpd.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://ims.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yrg.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://liu.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://djz.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://iru.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://gcq.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://duk.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://tuu.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://vob.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nxb.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rlk.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ylh.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tcq.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://njw.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lmd.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kee.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yoa.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://qtd.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nrv.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sdc.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rrw.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://axl.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xcv.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://epu.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nbx.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ksh.epnwcf.com

[P04] 求长度
来源：http://uem.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://woa.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgt.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lsu.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hep.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://nid.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://klz.haohaochexian.top

Ruby: x.length;  x.size
来源：http://cmf.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hxw.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://mwp.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cze.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hcd.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zhi.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ghd.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qme.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://ohm.jiagoushi.top

Ruby: a == b
来源：http://hks.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rth.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mgg.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ekr.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://pnu.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tth.sysykeji.top

TS:   if (x == null) {}
来源：http://vvv.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zyd.tarul.cn

Go:   if x == nil {}
来源：http://tfc.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aiq.ydzc1.top

C#:   if (x is null) {}
来源：http://ezy.0kj1m.cn

[P07] 防抖与节流
来源：http://rxy.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tnh.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://jbc.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aqd.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjp.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wvd.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycb.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mwd.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nql.yj20258.top

[P08] 处理浮点精度问题
来源：http://ggh.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://duv.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zmj.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hse.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hjr.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lyr.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ycb.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://phz.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cah.pengpengdd.cyou

================================================================================
来源：http://crl.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://btb.jinqigufen.top

================================================================================
来源：http://cbb.cqqwz.cn

[Q01] 创建表
来源：http://icc.fzhhl.top

CREATE TABLE users (
来源：http://mpw.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rww.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://xmc.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://xoy.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xyp.tanke756.top

);
来源：http://bqp.dianchejie.cn

[Q02] 创建带外键的表
来源：http://ciu.chenjidiqi.icu

CREATE TABLE orders (
来源：http://gon.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svk.hcnkem.com

user_id INT NOT NULL,
来源：http://rxn.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://rht.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmh.xingfuxueyuan.xyz

);
来源：http://qjm.hfpthk.cn

[Q03] 增加列
来源：http://ntu.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nng.chenlongwang.top

[Q04] 修改列类型
来源：http://hih.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cfv.ydjk.org.cn

[Q05] 重命名列
来源：http://hkp.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mdy.redwolf501.top

[Q06] 删除列
来源：http://fht.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fpn.shanyushiyangtech.top

[Q07] 删除表
来源：http://cqm.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://cij.chenlongwang.top

[Q08] 创建普通索引
来源：http://efk.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kby.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://pln.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gia.yvedp.cn

[Q10] 插入单行
来源：http://kfk.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qjr.gogol.net.cn

[Q11] 一次插入多行
来源：http://kpz.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rwx.yj20258.top

[Q12] 插入后取自增 ID
来源：http://uqp.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lzg.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dcd.316326.xyz

[Q13] 忽略重复插入
来源：http://kcx.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iko.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://hmg.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xho.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pip.yvedp.cn

[Q15] 查询全部
来源：http://hrd.xylfe.cn

SELECT * FROM users;
来源：http://gur.jinqigufen.top

[Q16] 查询指定列
来源：http://vka.xylfe.cn

SELECT id, name FROM users;
来源：http://dpa.tianlin.xyz

[Q17] 条件查询
来源：http://rcy.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cmv.hywenlv.cn

[Q18] 模糊匹配
来源：http://cqo.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mbl.tian-w.cn

[Q19] 范围查询
来源：http://szx.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://giu.cdnleiting.top

[Q20] IN 列表
来源：http://swa.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hwg.ybcxt.top

[Q21] 空值判断
来源：http://lib.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xzm.ywan-chungtsiang.top

[Q22] 排序
来源：http://hgp.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zao.sjlbkw.cn

[Q23] 分页
来源：http://tnu.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://msa.iojbl.cn

[Q24] 去重
来源：http://brr.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://xpb.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://fhm.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hvq.shzxlz.cn

[Q26] 计数
来源：http://xgf.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://fsb.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://wnh.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cok.sjlbkw.cn

[Q28] 求和与平均
来源：http://mek.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://itb.52xcode.cn

[Q29] 最大最小值
来源：http://ubl.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://daa.hysaishi.cn

[Q30] 分组统计
来源：http://cjk.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://non.fehbvm.com

[Q31] 分组后过滤
来源：http://gca.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xph.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://obj.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ayh.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jbr.gaohongyu789.top

[Q33] 多列分组
来源：http://kcx.iojbl.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://udn.tianlin.xyz

[Q34] 每组取第一条
来源：http://ffh.andypj.xyz

SELECT * FROM (
来源：http://thh.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kzp.andypj.xyz

) t WHERE rn = 1;
来源：http://ehn.chenlongwang.top

[Q35] 内连接
来源：http://fht.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ijh.hfpthk.cn

[Q36] 左连接
来源：http://dmb.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qyk.iojbl.cn

[Q37] 右连接
来源：http://jxh.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oee.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://zsa.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ixo.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://fbg.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dns.cqqwz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://shf.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aav.fktsv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dbr.chenjidiqi.icu

[Q41] 多表连接
来源：http://rww.dianchejie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://zup.fktsv.cn

JOIN users u ON u.id = o.user_id
来源：http://zvi.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://jqq.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://qkc.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://qvb.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://snh.svipenyu.cn

[Q43] 标量子查询
来源：http://rit.uphjek.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://szs.pycfn.com

[Q44] IN 子查询
来源：http://www.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iju.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://wum.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://luq.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://dnj.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvz.fktsv.cn

[Q47] 与平均值比较
来源：http://keg.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dai.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://mrj.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jmd.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://wim.chenlongwang.top

[Q49] 更新单行
来源：http://yjr.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xqo.shuidangran.top

[Q50] 批量更新
来源：http://knz.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bbk.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://gve.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://thp.snrcjt.cn

[Q52] 删除指定行
来源：http://tdn.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://zhs.hammf.cn

[Q53] 按条件删除
来源：http://tbr.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzx.9152youxi.cn

[Q54] 清空表
来源：http://kaj.cashguo.top

TRUNCATE TABLE logs;
来源：http://vlo.tian-w.cn

[Q55] 排名（并列占位）
来源：http://dfd.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tuo.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://gnw.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://god.wangdashe.top

[Q57] 行号
来源：http://arp.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://prj.jinqigfzy.top

[Q58] 累计求和
来源：http://ewg.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zmo.chenlongwang.top

[Q59] 分组内累计
来源：http://hyy.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uxw.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://cjy.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://acp.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kvj.chenzaomai.com

[Q61] 移动平均
来源：http://odq.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://quf.jianghu66.top

[Q62] 分组占比
来源：http://mbx.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gpw.hesvh.cn

[Q63] 开启事务
来源：http://ujy.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://adl.dianchejie.cn

[Q64] 提交事务
来源：http://ikq.yonumen.top

COMMIT;
来源：http://anh.shanyushiyangtech.top

[Q65] 回滚事务
来源：http://rkk.zhoulong.xyz

ROLLBACK;
来源：http://pti.xinyue.icu

[Q66] 行锁查询
来源：http://tsb.chenlongwang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nmq.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://fsi.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cqk.shzxlz.cn

[Q68] 保存点
来源：http://dhq.hnqzz.top

SAVEPOINT sp1;
来源：http://tpu.hnqzz.top

ROLLBACK TO sp1;
来源：http://fif.sweek.top

[Q69] 查看执行计划
来源：http://suy.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://voe.hnxiangtu.top

[Q70] 更新统计信息
来源：http://wav.daxiang520.top

ANALYZE TABLE users;
来源：http://gqi.yonumen.top

[Q71] 查看建表语句
来源：http://wxf.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fqw.jianghu66.top

[Q72] 查看索引
来源：http://sla.ppjwa.cn

SHOW INDEX FROM users;
来源：http://exn.vehdjk.com

[Q73] 查看表状态
来源：http://fub.ywan-chungtsiang.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jvv.gzhubu.top

[Q74] 强制使用索引
来源：http://vss.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ftb.cheryme.top

[Q75] 日期格式化
来源：http://iul.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fxu.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cfs.cashguo.top

[Q76] 按天统计
来源：http://acq.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tpk.fktsv.cn

[Q77] 时间加减
来源：http://zgg.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hwf.dashuyun.cn

[Q78] 当前时间
来源：http://fxk.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://olw.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://kms.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://epm.yfazqb.com

[Q80] 字符串截取
来源：http://mzt.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rsk.chenlongwang.top

[Q81] 字符串替换
来源：http://cxt.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ngs.epnwcf.com

[Q82] 字符长度与字节长度
来源：http://wdv.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ejt.gaohongyu789.top

[Q83] 大小写转换
来源：http://xip.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zhw.52xcode.cn

[Q84] 去除首尾空格
来源：http://mxh.vqdsnc.cn

SELECT TRIM(name) FROM users;
来源：http://awr.jiagoushi.top

[Q85] 数值取整
来源：http://dqi.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ygu.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://swp.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://svh.hysaishi.cn

[Q87] JSON 字段做条件
来源：http://khm.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kdo.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://wan.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tut.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sou.gotoacloud.top

[Q89] 判断表是否存在
来源：http://nhh.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gia.yueranfly.top

[Q90] 生成序号列
来源：http://ron.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bhe.hesvh.cn

================================================================================
来源：http://qhz.fengsongda.top

R. Bash 专题
来源：http://lyc.iojbl.cn

================================================================================
来源：http://nzd.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://nra.xuanzx.com

#!/usr/bin/env bash
来源：http://kph.ydzc1.top


<!-- 参考信息 -->