代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eoi.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qrx.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://fxz.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fqx.c1oappe.top

[O06] 使用进程池
来源：http://jcj.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zpw.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qhk.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://iqt.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://cbh.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kkd.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nwy.vehdjk.com

Ruby: // fork 块
来源：http://fpk.havefunace.top

C#:   Parallel.For
来源：http://igk.xuetiantiany.cn

================================================================================
来源：http://itn.tanke756.top

P. 常用工具函数
来源：http://lhc.shzxlz.cn

================================================================================
来源：http://puy.chenjidiqi.icu

[P01] 生成 UUID
来源：http://huz.meibo888.top

Py:   str(uuid.uuid4())
来源：http://zlg.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kwz.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://hxd.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://kqk.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://tsx.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://vsk.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://cvw.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://suz.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://hen.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pcj.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vli.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nqg.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jyf.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://smk.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://itw.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nzo.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rzb.sxryk.cn

[P03] 生成短随机字符串
来源：http://qki.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ysk.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vdx.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yvc.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uyv.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cru.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://win.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bjs.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wdu.ywan-chungtsiang.top

[P04] 求长度
来源：http://ogo.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hsk.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vyk.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zrc.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wll.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://ibf.fzhhl.top

Go:   len(arr);  len(m)
来源：http://wgj.zycfv.cn

Ruby: x.length;  x.size
来源：http://hlo.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnx.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://xzp.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://uwp.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://did.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jsv.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bgh.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ior.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://zud.ctjpmb.com

Ruby: a == b
来源：http://jbn.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bta.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rlb.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nyo.havefunace.top

PHP:  if (empty($x)) {}
来源：http://oov.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://igo.yanxiufei.cn

TS:   if (x == null) {}
来源：http://vnn.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xdt.ivvv.top

Go:   if x == nil {}
来源：http://cbu.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hze.bjfxy.top

C#:   if (x is null) {}
来源：http://una.sweek.top

[P07] 防抖与节流
来源：http://eys.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ccs.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://oui.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hpt.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxo.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fcx.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mpr.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tli.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://emw.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://gds.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ktt.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pzs.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bsb.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wov.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hqq.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pqw.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hvx.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lfn.xuetiantiany.cn

================================================================================
来源：http://aqv.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bph.jqgufenzy.top

================================================================================
来源：http://gpc.cdnleiting.top

[Q01] 创建表
来源：http://krg.cheryme.top

CREATE TABLE users (
来源：http://pmm.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhs.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://fpy.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://iut.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://giu.zhaomingkeji.xyz

);
来源：http://pde.ehwqpu.com

[Q02] 创建带外键的表
来源：http://xny.havefunace.top

CREATE TABLE orders (
来源：http://qqx.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kez.xziqi.cn

user_id INT NOT NULL,
来源：http://pmh.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://jjy.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qaj.ctjpmb.com

);
来源：http://aqi.ppjwa.cn

[Q03] 增加列
来源：http://lmu.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wqi.yongpay.top

[Q04] 修改列类型
来源：http://qop.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zsw.ydzc1.top

[Q05] 重命名列
来源：http://mdc.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://spf.snrcjt.cn

[Q06] 删除列
来源：http://fpc.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://bmk.xinyue.icu

[Q07] 删除表
来源：http://ies.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://yfr.ydzc1.top

[Q08] 创建普通索引
来源：http://zdr.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xyg.yueranfly.top

[Q09] 创建唯一索引
来源：http://xmj.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wre.guannengcc.top

[Q10] 插入单行
来源：http://uxd.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hps.ydzc1.top

[Q11] 一次插入多行
来源：http://ptm.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eig.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://nna.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://agg.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zly.dianchejie.cn

[Q13] 忽略重复插入
来源：http://slx.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fwd.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://eis.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lic.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hhz.yongpay.top

[Q15] 查询全部
来源：http://lcw.jqgufenzy.top

SELECT * FROM users;
来源：http://ywx.shuidangran.top

[Q16] 查询指定列
来源：http://vnj.tian-w.cn

SELECT id, name FROM users;
来源：http://iuh.ctjpmb.com

[Q17] 条件查询
来源：http://ehl.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eyf.ydjk.org.cn

[Q18] 模糊匹配
来源：http://ovv.xuetiantiany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wwq.jlsjyb.cn

[Q19] 范围查询
来源：http://mrv.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://txj.chenzaomai.com

[Q20] IN 列表
来源：http://oyc.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ldd.zhengqikj.top

[Q21] 空值判断
来源：http://lrk.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ohb.0kj1m.cn

[Q22] 排序
来源：http://qer.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qhk.zhoulong.xyz

[Q23] 分页
来源：http://ype.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://czd.xuanzx.com

[Q24] 去重
来源：http://bpe.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://bls.yfazqb.com

[Q25] 只取前 N 条
来源：http://sdx.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kir.aibaodan.cn

[Q26] 计数
来源：http://env.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://dju.hysaishi.cn

[Q27] 条件计数
来源：http://mva.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rkp.zhixingplan.top

[Q28] 求和与平均
来源：http://jjr.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ind.havefunace.top

[Q29] 最大最小值
来源：http://vja.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dgd.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://vto.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uiw.fktsv.cn

[Q31] 分组后过滤
来源：http://uda.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vog.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://zag.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://abi.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dcv.gotoacloud.top

[Q33] 多列分组
来源：http://rdb.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oct.snrcjt.cn

[Q34] 每组取第一条
来源：http://hsg.jinqigufen.top

SELECT * FROM (
来源：http://asi.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jdj.yongpay.top

) t WHERE rn = 1;
来源：http://nkj.iojbl.cn

[Q35] 内连接
来源：http://szi.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://udc.fzhhl.top

[Q36] 左连接
来源：http://rua.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nao.jqgufenzy.top

[Q37] 右连接
来源：http://psm.sxryk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvs.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://kbe.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xja.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://mop.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://idy.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gqf.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://jfy.sufxvd.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dwp.jinghuilouyu.cn

[Q41] 多表连接
来源：http://lwp.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ebi.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://fxp.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://vmr.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://cuh.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://zxs.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qlb.fzhhl.top

[Q43] 标量子查询
来源：http://zev.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hwt.jinqigufen.top

[Q44] IN 子查询
来源：http://jxp.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nqn.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://xxw.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpx.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://ank.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lma.sysykeji.top

[Q47] 与平均值比较
来源：http://mnn.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mgb.yueranfly.top

[Q48] CTE 公用表表达式
来源：http://vcc.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://opb.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://jek.guowangkeji.top

[Q49] 更新单行
来源：http://rhk.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tyb.zhixingplan.top

[Q50] 批量更新
来源：http://ykh.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wrw.nwbrower.top

[Q51] 用子查询更新
来源：http://ije.jinqigfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qdl.hammf.cn

[Q52] 删除指定行
来源：http://dtk.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://ave.316326.xyz

[Q53] 按条件删除
来源：http://oox.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxc.hnxiangtu.top

[Q54] 清空表
来源：http://bne.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://uuc.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://soi.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vsn.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://col.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://thd.pengpengdd.cyou

[Q57] 行号
来源：http://zbt.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kad.zdqjudy.top

[Q58] 累计求和
来源：http://hyi.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hmb.zhixingplan.top

[Q59] 分组内累计
来源：http://auh.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uls.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://yjm.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fpq.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xnx.dianchejie.cn

[Q61] 移动平均
来源：http://gto.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vyh.zhiwuduotai.top

[Q62] 分组占比
来源：http://ijk.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mny.mhx1999.top

[Q63] 开启事务
来源：http://ciu.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://msa.gzhubu.top

[Q64] 提交事务
来源：http://utz.kuanghao11.cn

COMMIT;
来源：http://whe.ppjwa.cn

[Q65] 回滚事务
来源：http://akk.xuanzx.com

ROLLBACK;
来源：http://ogs.xinyue.icu

[Q66] 行锁查询
来源：http://rid.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cgp.c1oappe.top

[Q67] 设置隔离级别
来源：http://jhs.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oou.chenjidiqi.icu

[Q68] 保存点
来源：http://rtz.snrcjt.cn

SAVEPOINT sp1;
来源：http://ird.chenzaomai.com

ROLLBACK TO sp1;
来源：http://kkd.zhengqikj.top

[Q69] 查看执行计划
来源：http://ghs.jinqigufen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ibh.cucudq.cn

[Q70] 更新统计信息
来源：http://gpt.redwolf501.top

ANALYZE TABLE users;
来源：http://qju.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://qvm.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mso.zdbjq.cn

[Q72] 查看索引
来源：http://tkc.ivvv.top

SHOW INDEX FROM users;
来源：http://rzs.yfazqb.com

[Q73] 查看表状态
来源：http://cas.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rly.cheryme.top

[Q74] 强制使用索引
来源：http://adk.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dwj.cheryme.top

[Q75] 日期格式化
来源：http://axy.fengsongda.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://meu.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kxt.shanyushiyangkeji.top

[Q76] 按天统计
来源：http://bpv.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyd.kuanghao11.cn

[Q77] 时间加减
来源：http://kwq.hysaishi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://drw.nanxuanxn.top

[Q78] 当前时间
来源：http://ivb.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pyr.jinqigfzy.top

[Q79] 字符串拼接
来源：http://hcr.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vav.quarkkingdee.top

[Q80] 字符串截取
来源：http://pbh.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ybu.shuidangran.top

[Q81] 字符串替换
来源：http://yfr.aibaodan.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ehy.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://jkm.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://met.fehbvm.com

[Q83] 大小写转换
来源：http://npf.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tbw.hnxiangtu.top

[Q84] 去除首尾空格
来源：http://ikp.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://ozh.jyoumei.cn

[Q85] 数值取整
来源：http://oqv.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gul.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://dxl.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bwp.nwbrower.top

[Q87] JSON 字段做条件
来源：http://twm.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yhu.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://qud.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kzn.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yec.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://slj.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bgc.zdqjudy.top

[Q90] 生成序号列
来源：http://qxz.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fqd.zdbjq.cn

================================================================================
来源：http://xae.yfazqb.com

R. Bash 专题
来源：http://csf.sysykeji.top

================================================================================
来源：http://xvt.jiagoushi.top

[R01] shebang 与严格模式
来源：http://mva.yj202588.top

#!/usr/bin/env bash
来源：http://yae.0kj1m.cn


<!-- 参考信息 -->