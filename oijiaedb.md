代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xpo.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dfk.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://yru.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aho.chenlongwang.top

[O06] 使用进程池
来源：http://pfi.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lqv.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uld.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://dhk.cashguo.top

TS:   // child_process / cluster 模块
来源：http://iqg.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ybm.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tgo.yuxming.cn

Ruby: // fork 块
来源：http://hzv.sjlbkw.cn

C#:   Parallel.For
来源：http://cyk.iojbl.cn

================================================================================
来源：http://uav.guowangkeji.top

P. 常用工具函数
来源：http://cqr.yanxiufei.cn

================================================================================
来源：http://ajc.bbcook.cn

[P01] 生成 UUID
来源：http://ipy.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://eeo.ywan-chungtsiang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kiy.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://hke.tarul.cn

TS:   crypto.randomUUID()
来源：http://fba.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://qkw.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://gwm.tarul.cn

Ruby: SecureRandom.uuid
来源：http://zdo.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://pqw.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://gax.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://htv.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xlw.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lrx.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emb.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xvh.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gzv.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xxr.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://szm.cucudq.cn

[P03] 生成短随机字符串
来源：http://eic.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qup.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nbt.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kmp.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzz.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sfs.andypj.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mup.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mua.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jds.chenzaomai.com

[P04] 求长度
来源：http://bed.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pqy.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://biy.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcn.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vfm.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://uje.wangdashe.top

Go:   len(arr);  len(m)
来源：http://qpk.zhixingplan.top

Ruby: x.length;  x.size
来源：http://gam.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nzv.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://lwi.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kda.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szo.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gxb.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wte.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wfw.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://njl.aizwys.cn

Ruby: a == b
来源：http://plr.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hcj.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ycz.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xhm.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://avp.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jfq.birdmap.top

TS:   if (x == null) {}
来源：http://olx.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yuh.sufxvd.cn

Go:   if x == nil {}
来源：http://yqz.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eqv.9152youxi.cn

C#:   if (x is null) {}
来源：http://brj.nanxinkj.top

[P07] 防抖与节流
来源：http://frs.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dnm.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://phf.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mak.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kod.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kts.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dio.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://mzl.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jld.pycfn.com

[P08] 处理浮点精度问题
来源：http://gkt.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://etk.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://owl.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://njv.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rnj.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://phq.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tjj.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xke.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rpz.chenlongwang.top

================================================================================
来源：http://slc.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ngg.daria6918.cn

================================================================================
来源：http://ppy.tian-w.cn

[Q01] 创建表
来源：http://cey.jianghu66.top

CREATE TABLE users (
来源：http://ktj.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xzi.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://bxx.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://akj.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rwq.zdbjq.cn

);
来源：http://iur.yueranfly.top

[Q02] 创建带外键的表
来源：http://jwc.tanke756.top

CREATE TABLE orders (
来源：http://enc.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tuo.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://jzm.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://isa.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vik.iojbl.cn

);
来源：http://hew.yueranfly.top

[Q03] 增加列
来源：http://kzt.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uxw.tian-w.cn

[Q04] 修改列类型
来源：http://ati.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ipp.aibaodan.cn

[Q05] 重命名列
来源：http://vpc.fehbvm.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yzr.pycfn.com

[Q06] 删除列
来源：http://thf.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://mzp.redwolf501.top

[Q07] 删除表
来源：http://ogk.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://ctk.daria6918.cn

[Q08] 创建普通索引
来源：http://aam.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oey.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://vrb.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lir.guowangkeji.top

[Q10] 插入单行
来源：http://vmi.ppjwa.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cpb.fktsv.cn

[Q11] 一次插入多行
来源：http://drr.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzd.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://tlf.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nir.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://roi.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://scj.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ngl.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://hjd.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://naz.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://odk.jqgfzy.top

[Q15] 查询全部
来源：http://gla.yongpay.top

SELECT * FROM users;
来源：http://zxu.9152youxi.cn

[Q16] 查询指定列
来源：http://kol.cheryme.top

SELECT id, name FROM users;
来源：http://ozu.chenjidiqi.icu

[Q17] 条件查询
来源：http://cip.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ctv.9152youxi.cn

[Q18] 模糊匹配
来源：http://ggh.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wca.yuanzhike.top

[Q19] 范围查询
来源：http://fki.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kzn.316326.xyz

[Q20] IN 列表
来源：http://dms.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kgu.bbcook.cn

[Q21] 空值判断
来源：http://fye.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ecp.yueranfly.top

[Q22] 排序
来源：http://hrd.jianghu66.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rvk.ctjpmb.com

[Q23] 分页
来源：http://sgn.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tpw.pycfn.com

[Q24] 去重
来源：http://ctc.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://pfa.snrcjt.cn

[Q25] 只取前 N 条
来源：http://blm.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qnf.aibaodan.cn

[Q26] 计数
来源：http://mpv.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://gzo.meibo888.top

[Q27] 条件计数
来源：http://pdw.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nkv.xylfe.cn

[Q28] 求和与平均
来源：http://gjv.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://txh.quarkkingdee.top

[Q29] 最大最小值
来源：http://xdm.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://lwc.sufxvd.cn

[Q30] 分组统计
来源：http://nxz.hnqzz.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nrz.daria6918.cn

[Q31] 分组后过滤
来源：http://gtx.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://knc.xinyue.icu

[Q32] 分组拼接字符串
来源：http://jik.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hyp.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://whh.kuanghao11.cn

[Q33] 多列分组
来源：http://rzq.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ual.yj20258.top

[Q34] 每组取第一条
来源：http://dwf.hcnkem.com

SELECT * FROM (
来源：http://wjf.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sml.ydjk.org.cn

) t WHERE rn = 1;
来源：http://prb.yonumen.top

[Q35] 内连接
来源：http://ulf.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uwr.redwolf501.top

[Q36] 左连接
来源：http://jcb.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zgv.chenzaomai.com

[Q37] 右连接
来源：http://lyi.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://piu.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://ovu.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oyl.316326.xyz

[Q39] 自连接（查上下级）
来源：http://tya.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zuh.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fwo.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jmt.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ngc.sufxvd.cn

[Q41] 多表连接
来源：http://zyn.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yre.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://rbh.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://zex.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://ruc.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://fyp.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://del.jiagoushi.top

[Q43] 标量子查询
来源：http://bro.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yuh.wangshuangyany.cn

[Q44] IN 子查询
来源：http://wzj.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zos.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://yem.xingfuxueyuan.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyo.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://bti.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iup.redwolf501.top

[Q47] 与平均值比较
来源：http://ivb.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://shp.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://pjq.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://awb.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://nxi.yfazqb.com

[Q49] 更新单行
来源：http://brf.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qwn.shangyingyoupin.top

[Q50] 批量更新
来源：http://vxp.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ots.tianlin.xyz

[Q51] 用子查询更新
来源：http://uee.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lso.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://qyp.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://fdt.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://fus.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vxr.fanxiaobao.xyz

[Q54] 清空表
来源：http://ric.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://inq.cheryme.top

[Q55] 排名（并列占位）
来源：http://lbj.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ukm.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://dit.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lzr.jinqigfzy.top

[Q57] 行号
来源：http://dsq.smart0.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mbf.nanxuanxn.top

[Q58] 累计求和
来源：http://igf.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://djo.ydjk.org.cn

[Q59] 分组内累计
来源：http://teu.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yln.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://ssz.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ioo.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sta.gotoacloud.top

[Q61] 移动平均
来源：http://wiz.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nbx.hfpthk.cn

[Q62] 分组占比
来源：http://aoj.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zpm.jinqigufen.top

[Q63] 开启事务
来源：http://esc.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mxy.zhongyouzk.top

[Q64] 提交事务
来源：http://pyo.zhoulong.xyz

COMMIT;
来源：http://ilj.ctjpmb.com

[Q65] 回滚事务
来源：http://the.pengpengdd.cyou

ROLLBACK;
来源：http://vry.zhongyouzk.top

[Q66] 行锁查询
来源：http://riy.ivvv.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fkg.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://mpd.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bsq.xinyue.icu

[Q68] 保存点
来源：http://nap.yuxming.cn

SAVEPOINT sp1;
来源：http://zbe.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://rsq.bjfxy.top

[Q69] 查看执行计划
来源：http://vcs.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tsz.ydzc1.top

[Q70] 更新统计信息
来源：http://css.snrcjt.cn

ANALYZE TABLE users;
来源：http://cvb.jiagoushi.top

[Q71] 查看建表语句
来源：http://nho.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ata.zycfv.cn

[Q72] 查看索引
来源：http://opt.hnqzz.top

SHOW INDEX FROM users;
来源：http://mzs.redwolf501.top

[Q73] 查看表状态
来源：http://jya.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://egj.aibaodan.cn

[Q74] 强制使用索引
来源：http://vlg.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gqq.0kj1m.cn

[Q75] 日期格式化
来源：http://uya.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aam.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fdm.jiagoushi.top

[Q76] 按天统计
来源：http://zxk.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kbb.yj20258.top

[Q77] 时间加减
来源：http://ejh.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yjy.yangfankeji.com

[Q78] 当前时间
来源：http://ypl.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://puk.snrcjt.cn

[Q79] 字符串拼接
来源：http://nuj.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mlp.zhoulong.xyz

[Q80] 字符串截取
来源：http://mys.zdbjq.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hpk.yonumen.top

[Q81] 字符串替换
来源：http://uxv.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qhe.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://gkb.hysaishi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bjs.hongshengwenyu.top

[Q83] 大小写转换
来源：http://mvt.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://heg.tianlin.xyz

[Q84] 去除首尾空格
来源：http://bup.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://puc.dashuyun.cn

[Q85] 数值取整
来源：http://ntf.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qgi.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://ris.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikj.0kj1m.cn

[Q87] JSON 字段做条件
来源：http://zfp.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://maf.cashguo.top

[Q88] 行转列（条件聚合）
来源：http://zez.jqgufenzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ggd.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xxn.yuanzhike.top

[Q89] 判断表是否存在
来源：http://dzj.zhoulong.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gub.jinqigfzy.top

[Q90] 生成序号列
来源：http://uqd.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zku.vehdjk.com

================================================================================
来源：http://xtj.cdnleiting.top

R. Bash 专题
来源：http://hag.quarkkingdee.top

================================================================================
来源：http://rda.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://yyn.ppjwa.cn

#!/usr/bin/env bash
来源：http://tjr.zdbjq.cn


<!-- 参考信息 -->