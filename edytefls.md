代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://bdz.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yuc.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://drd.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://ulo.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zuw.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mxc.ivvv.top

Ruby: threads.map(&:join)
来源：http://szm.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uiq.nanxuanxn.top

[O06] 使用进程池
来源：http://urz.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yzj.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xll.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://gdj.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://cxh.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ylt.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dhk.zhoulong.xyz

Ruby: // fork 块
来源：http://tzo.iojbl.cn

C#:   Parallel.For
来源：http://vxs.redwolf501.top

================================================================================
来源：http://fii.yueranfly.top

P. 常用工具函数
来源：http://muv.dianchejie.cn

================================================================================
来源：http://dyj.xylfe.cn

[P01] 生成 UUID
来源：http://tqg.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://ymp.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://owg.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://trg.sysykeji.top

TS:   crypto.randomUUID()
来源：http://wcy.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://wfs.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://rfb.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://irx.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://kbb.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://wlc.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://khj.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vzl.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nhh.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://goz.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ory.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hxf.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ybr.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yzj.tianlin.xyz

[P03] 生成短随机字符串
来源：http://fig.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nuu.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qgu.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fyz.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gto.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ueo.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyt.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xbi.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pgd.c1oappe.top

[P04] 求长度
来源：http://rfq.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mpg.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xww.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yrs.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rmk.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://gcg.fehbvm.com

Go:   len(arr);  len(m)
来源：http://cdz.aibaodan.cn

Ruby: x.length;  x.size
来源：http://zgq.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://smm.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://owj.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vqs.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tyv.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nwj.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dcp.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ykr.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lgv.yueranfly.top

Ruby: a == b
来源：http://mfz.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tei.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pyn.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lxi.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://kcb.fehbvm.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xjf.svipenyu.cn

TS:   if (x == null) {}
来源：http://jyq.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uru.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://bxc.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xwo.fktsv.cn

C#:   if (x is null) {}
来源：http://gac.ivvv.top

[P07] 防抖与节流
来源：http://rhb.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zet.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://lnf.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cns.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sql.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jxh.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ilv.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://swz.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pir.uphjek.com

[P08] 处理浮点精度问题
来源：http://kmz.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hyt.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xqe.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uye.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vge.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qgt.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bhi.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gzs.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nob.yj20258.top

================================================================================
来源：http://mfa.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jku.hammf.cn

================================================================================
来源：http://isj.zhaomingkeji.xyz

[Q01] 创建表
来源：http://hfs.sjlbkw.cn

CREATE TABLE users (
来源：http://vwu.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wwb.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://hba.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://jzj.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yrk.xingfuxueyuan.xyz

);
来源：http://lhj.cqqwz.cn

[Q02] 创建带外键的表
来源：http://exh.ppjwa.cn

CREATE TABLE orders (
来源：http://yxg.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqy.ctjpmb.com

user_id INT NOT NULL,
来源：http://yvi.hammf.cn

amount DECIMAL(10, 2),
来源：http://lvf.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://urp.zhijiandao.cn

);
来源：http://shp.gogol.net.cn

[Q03] 增加列
来源：http://clw.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lhn.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://xyn.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zch.nanxuanxn.top

[Q05] 重命名列
来源：http://zlk.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://olh.nanxinkj.top

[Q06] 删除列
来源：http://jhd.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://mqs.wangdashe.top

[Q07] 删除表
来源：http://syr.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://muq.yj20258.top

[Q08] 创建普通索引
来源：http://hwg.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ymo.316326.xyz

[Q09] 创建唯一索引
来源：http://gaq.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://piz.xylfe.cn

[Q10] 插入单行
来源：http://uyh.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gqn.yj20258888.top

[Q11] 一次插入多行
来源：http://npt.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eeq.yuanzhike.top

[Q12] 插入后取自增 ID
来源：http://csf.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uwk.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ioa.hcnkem.com

[Q13] 忽略重复插入
来源：http://tul.sweek.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rvp.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://pkl.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wts.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dww.redwolf501.top

[Q15] 查询全部
来源：http://yzs.zdqjudy.top

SELECT * FROM users;
来源：http://ecz.jinqigfzy.top

[Q16] 查询指定列
来源：http://hsj.epnwcf.com

SELECT id, name FROM users;
来源：http://rft.chenjidiqi.icu

[Q17] 条件查询
来源：http://klk.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aty.52xcode.cn

[Q18] 模糊匹配
来源：http://mkk.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cpn.jyoumei.cn

[Q19] 范围查询
来源：http://pba.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eky.nanxinkj.top

[Q20] IN 列表
来源：http://jgb.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gwz.shzxlz.cn

[Q21] 空值判断
来源：http://msx.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hop.0kj1m.cn

[Q22] 排序
来源：http://atr.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hkh.kuanghao11.cn

[Q23] 分页
来源：http://kpf.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yef.yangfankeji.com

[Q24] 去重
来源：http://yjr.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://frd.gogol.net.cn

[Q25] 只取前 N 条
来源：http://ckv.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ald.jianghu66.top

[Q26] 计数
来源：http://qxz.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://slw.zhoulong.xyz

[Q27] 条件计数
来源：http://mpk.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rpy.sysykeji.top

[Q28] 求和与平均
来源：http://uft.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bva.cucudq.cn

[Q29] 最大最小值
来源：http://wmj.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yjo.haohaochexian.top

[Q30] 分组统计
来源：http://pwp.nwbrower.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qnk.guannengcc.top

[Q31] 分组后过滤
来源：http://ckf.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bhf.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://kyi.iojbl.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bct.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gyh.yueranfly.top

[Q33] 多列分组
来源：http://uhw.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbh.ctjpmb.com

[Q34] 每组取第一条
来源：http://zbs.chenjidiqi.icu

SELECT * FROM (
来源：http://lju.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://irf.0kj1m.cn

) t WHERE rn = 1;
来源：http://qnd.yfazqb.com

[Q35] 内连接
来源：http://vim.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ywi.cucudq.cn

[Q36] 左连接
来源：http://yad.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aap.smart0.xyz

[Q37] 右连接
来源：http://raw.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://khp.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://mhe.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://foq.jinyuanbaomall.cn

[Q39] 自连接（查上下级）
来源：http://ftt.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wxb.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lnv.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lkr.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sut.ppjwa.cn

[Q41] 多表连接
来源：http://snv.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tjn.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://xil.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mhy.nanxuanxn.top

[Q42] 连接条件附加过滤
来源：http://gpb.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://oja.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sum.jqgfzy.top

[Q43] 标量子查询
来源：http://jhs.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mzv.smart0.xyz

[Q44] IN 子查询
来源：http://nwx.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jer.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://txt.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kyl.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://drq.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qwt.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://uxm.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gsp.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://nmf.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gkk.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://cxh.bjfxy.top

[Q49] 更新单行
来源：http://uns.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kir.zycfv.cn

[Q50] 批量更新
来源：http://jbb.ybcxt.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cov.hcnkem.com

[Q51] 用子查询更新
来源：http://bmz.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fdh.bbcook.cn

[Q52] 删除指定行
来源：http://hve.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://azi.zdqjudy.top

[Q53] 按条件删除
来源：http://agj.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nqr.fktsv.cn

[Q54] 清空表
来源：http://ayr.sysykeji.top

TRUNCATE TABLE logs;
来源：http://fll.shuidangran.top

[Q55] 排名（并列占位）
来源：http://byq.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qke.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://xev.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jlp.hesvh.cn

[Q57] 行号
来源：http://lum.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qfp.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://jbd.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://axc.vqdsnc.cn

[Q59] 分组内累计
来源：http://jlu.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://okc.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://xhz.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ylc.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jcs.guannengcc.top

[Q61] 移动平均
来源：http://wpd.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xpm.wangdashe.top

[Q62] 分组占比
来源：http://pzy.ydzc1.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tvu.jlsjyb.cn

[Q63] 开启事务
来源：http://nuh.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tso.hammf.cn

[Q64] 提交事务
来源：http://orm.hywenlv.cn

COMMIT;
来源：http://tef.quarkkingdee.top

[Q65] 回滚事务
来源：http://nbb.hysaishi.cn

ROLLBACK;
来源：http://tza.xziqi.cn

[Q66] 行锁查询
来源：http://trm.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cqd.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://jbo.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lmz.jlsjyb.cn

[Q68] 保存点
来源：http://xwm.hcnkem.com

SAVEPOINT sp1;
来源：http://msw.tian-w.cn

ROLLBACK TO sp1;
来源：http://cmt.epnwcf.com

[Q69] 查看执行计划
来源：http://wbw.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fxa.zhijiandao.cn

[Q70] 更新统计信息
来源：http://egl.hfpthk.cn

ANALYZE TABLE users;
来源：http://xxy.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://izk.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kwk.bbcook.cn

[Q72] 查看索引
来源：http://yxx.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://oea.tarul.cn

[Q73] 查看表状态
来源：http://kgo.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nso.snrcjt.cn

[Q74] 强制使用索引
来源：http://dhe.hammf.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ztx.jinqigfzy.top

[Q75] 日期格式化
来源：http://hws.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yct.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dmv.bjfxy.top

[Q76] 按天统计
来源：http://wjf.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uxj.gotoacloud.top

[Q77] 时间加减
来源：http://dyq.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://waz.haohaochexian.top

[Q78] 当前时间
来源：http://jnu.zhiwuduotai.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vth.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://ikq.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://brd.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://qta.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fgd.fktsv.cn

[Q81] 字符串替换
来源：http://zlq.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xsz.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://soe.smart0.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oaw.ehwqpu.com

[Q83] 大小写转换
来源：http://spq.daria6918.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xww.haohaochexian.top

[Q84] 去除首尾空格
来源：http://bwy.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://jwt.quarkkingdee.top

[Q85] 数值取整
来源：http://gzx.jinqigufen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfo.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://myq.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vmf.sjlbkw.cn

[Q87] JSON 字段做条件
来源：http://esz.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wlp.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://ofz.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hec.xylfe.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rdc.zhixingplan.top

[Q89] 判断表是否存在
来源：http://xab.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wly.cheryme.top

[Q90] 生成序号列
来源：http://awg.jinqigfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ola.hongshengwenyu.top

================================================================================
来源：http://vva.fanxiaobao.xyz


<!-- 参考信息 -->