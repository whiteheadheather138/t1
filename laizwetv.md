代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://tzr.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sfl.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://obp.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://qyx.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vyk.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dff.yonumen.top

Ruby: threads.map(&:join)
来源：http://dtx.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fft.meibo888.top

[O06] 使用进程池
来源：http://sfr.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xof.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xob.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://vxi.pycfn.com

TS:   // child_process / cluster 模块
来源：http://ozn.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bjt.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ppj.chenlongwang.top

Ruby: // fork 块
来源：http://hof.svipenyu.cn

C#:   Parallel.For
来源：http://fbq.316326.xyz

================================================================================
来源：http://lwh.quarkkingdee.top

P. 常用工具函数
来源：http://ztu.sjlbkw.cn

================================================================================
来源：http://soe.gaohongyu789.top

[P01] 生成 UUID
来源：http://gqt.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://hcp.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kul.daria6918.cn

JS:   crypto.randomUUID()
来源：http://kmc.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://mov.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://dvp.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://zlk.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://arg.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://ywb.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://gdq.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://shw.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tpg.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jsh.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nia.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wzs.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hbo.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zfi.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjy.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://zgm.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://crk.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ijp.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uxs.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hzj.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://slh.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mor.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gbz.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ees.ivvv.top

[P04] 求长度
来源：http://aoe.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qxe.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwk.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jam.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jyp.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://uzz.xziqi.cn

Go:   len(arr);  len(m)
来源：http://gxc.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://izj.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uxt.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://eex.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fto.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tuq.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dpe.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://chf.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vsb.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://lig.mhx1999.top

Ruby: a == b
来源：http://gbc.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mrt.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yow.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eet.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://rrg.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hba.sysykeji.top

TS:   if (x == null) {}
来源：http://emr.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gcp.zhijiandao.cn

Go:   if x == nil {}
来源：http://glt.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lbs.vqdsnc.cn

C#:   if (x is null) {}
来源：http://nca.yj20258888.top

[P07] 防抖与节流
来源：http://zvd.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qhg.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://hja.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozm.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nqt.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oug.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://grl.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://erv.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ozc.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://psn.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wlr.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cdg.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xhl.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ncx.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zqe.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nkt.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvp.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vyz.smart0.xyz

================================================================================
来源：http://xkm.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gjx.0kj1m.cn

================================================================================
来源：http://pwu.fktsv.cn

[Q01] 创建表
来源：http://fsh.daria6918.cn

CREATE TABLE users (
来源：http://qsa.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ymf.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://qwq.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://unv.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://syf.jqgfzy.top

);
来源：http://gfo.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://ecy.xziqi.cn

CREATE TABLE orders (
来源：http://rvj.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cif.cashguo.top

user_id INT NOT NULL,
来源：http://ccm.yj202588.top

amount DECIMAL(10, 2),
来源：http://pvk.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mwy.uphjek.com

);
来源：http://mjy.aizwys.cn

[Q03] 增加列
来源：http://mss.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cud.jiagoushi.top

[Q04] 修改列类型
来源：http://emg.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jzv.svipenyu.cn

[Q05] 重命名列
来源：http://ggv.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cps.zdbjq.cn

[Q06] 删除列
来源：http://gdm.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bos.zhiwuduotai.top

[Q07] 删除表
来源：http://xmk.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://yuz.yuanzhike.top

[Q08] 创建普通索引
来源：http://plb.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ykb.ydzc1.top

[Q09] 创建唯一索引
来源：http://kpj.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gzm.fengsongda.top

[Q10] 插入单行
来源：http://ipi.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jrn.aibaodan.cn

[Q11] 一次插入多行
来源：http://gil.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://puq.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://lov.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vxb.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jiz.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://yoo.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mgv.daxiang520.top

[Q14] 存在则更新（upsert）
来源：http://ftf.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tnz.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xzk.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://cla.mhx1999.top

SELECT * FROM users;
来源：http://yni.jyoumei.cn

[Q16] 查询指定列
来源：http://noi.fengsongda.top

SELECT id, name FROM users;
来源：http://clp.jyoumei.cn

[Q17] 条件查询
来源：http://wyb.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://naj.shzxlz.cn

[Q18] 模糊匹配
来源：http://ffr.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bfs.shangyingyoupin.top

[Q19] 范围查询
来源：http://tof.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://abt.guannengcc.top

[Q20] IN 列表
来源：http://nun.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://egr.jinghuilouyu.cn

[Q21] 空值判断
来源：http://nhe.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xfu.tian-w.cn

[Q22] 排序
来源：http://ntg.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xqr.vqdsnc.cn

[Q23] 分页
来源：http://hya.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ges.yj202588.top

[Q24] 去重
来源：http://xad.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://hpe.zhoulong.xyz

[Q25] 只取前 N 条
来源：http://cgl.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jga.daria6918.cn

[Q26] 计数
来源：http://gpj.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://ycm.nwbrower.top

[Q27] 条件计数
来源：http://imh.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://etx.c1oappe.top

[Q28] 求和与平均
来源：http://ubt.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gcm.shangyingyoupin.top

[Q29] 最大最小值
来源：http://eat.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pzh.zhiwuduotai.top

[Q30] 分组统计
来源：http://kvo.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aal.vqdsnc.cn

[Q31] 分组后过滤
来源：http://yws.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fjy.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://wof.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lba.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pth.cdnleiting.top

[Q33] 多列分组
来源：http://kpp.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bsl.bbcook.cn

[Q34] 每组取第一条
来源：http://nng.jinqigufen.top

SELECT * FROM (
来源：http://ufj.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cjt.pycfn.com

) t WHERE rn = 1;
来源：http://bck.yvedp.cn

[Q35] 内连接
来源：http://dco.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yov.hammf.cn

[Q36] 左连接
来源：http://fua.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pla.yongpay.top

[Q37] 右连接
来源：http://vbg.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dru.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://myb.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sks.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://gej.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ueb.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bux.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bek.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gsv.zhixingplan.top

[Q41] 多表连接
来源：http://los.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nvb.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://fmg.tian-w.cn

JOIN products p ON p.id = o.product_id;
来源：http://nxd.sweek.top

[Q42] 连接条件附加过滤
来源：http://dxj.zdbjq.cn

SELECT u.name, o.amount FROM users u
来源：http://ecs.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yeg.pycfn.com

[Q43] 标量子查询
来源：http://xkm.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lai.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://gfi.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lnh.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://xlm.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xsi.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://kbf.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jut.hesvh.cn

[Q47] 与平均值比较
来源：http://pid.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opl.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://dau.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jam.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://fjg.ydjk.org.cn

[Q49] 更新单行
来源：http://ajw.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xpb.yj20258.top

[Q50] 批量更新
来源：http://adl.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hld.meibo888.top

[Q51] 用子查询更新
来源：http://bce.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tzv.wangshuangyany.cn

[Q52] 删除指定行
来源：http://sxx.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://usy.tarul.cn

[Q53] 按条件删除
来源：http://dpx.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzy.yvedp.cn

[Q54] 清空表
来源：http://uca.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://thy.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://osl.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://okh.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://nbf.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hux.cucudq.cn

[Q57] 行号
来源：http://bec.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://njs.gaohongyu789.top

[Q58] 累计求和
来源：http://tzr.wangdashe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hpo.jinqigufen.top

[Q59] 分组内累计
来源：http://swg.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://acg.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://udv.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xxk.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ojy.daria6918.cn

[Q61] 移动平均
来源：http://pgy.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eox.smart0.xyz

[Q62] 分组占比
来源：http://tdw.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gub.yj202588.top

[Q63] 开启事务
来源：http://tlf.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nvr.vqdsnc.cn

[Q64] 提交事务
来源：http://whj.tianlin.xyz

COMMIT;
来源：http://sdc.mhx1999.top

[Q65] 回滚事务
来源：http://evw.sxryk.cn

ROLLBACK;
来源：http://qzk.yueranfly.top

[Q66] 行锁查询
来源：http://phx.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yes.xziqi.cn

[Q67] 设置隔离级别
来源：http://cjv.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gso.guannengcc.top

[Q68] 保存点
来源：http://ram.yuxming.cn

SAVEPOINT sp1;
来源：http://sox.guowangkeji.top

ROLLBACK TO sp1;
来源：http://yyn.smart0.xyz

[Q69] 查看执行计划
来源：http://saq.316326.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://muo.0kj1m.cn

[Q70] 更新统计信息
来源：http://mcq.zycfv.cn

ANALYZE TABLE users;
来源：http://ecv.nanxinkj.top

[Q71] 查看建表语句
来源：http://esf.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wro.hysaishi.cn

[Q72] 查看索引
来源：http://bys.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://sgc.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://qwi.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rdc.daxiang520.top

[Q74] 强制使用索引
来源：http://tis.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hls.uphjek.com

[Q75] 日期格式化
来源：http://bmu.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qtm.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sbq.sufxvd.cn

[Q76] 按天统计
来源：http://kkx.chenjidiqi.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mck.ivvv.top

[Q77] 时间加减
来源：http://ext.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://urj.cqqwz.cn

[Q78] 当前时间
来源：http://ola.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pwt.fktsv.cn

[Q79] 字符串拼接
来源：http://yfc.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cog.hesvh.cn

[Q80] 字符串截取
来源：http://wjk.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qhx.ctjpmb.com

[Q81] 字符串替换
来源：http://nav.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dbs.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://koq.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zgr.shzxlz.cn

[Q83] 大小写转换
来源：http://nfy.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://krk.tarul.cn

[Q84] 去除首尾空格
来源：http://btf.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://soh.guowangkeji.top

[Q85] 数值取整
来源：http://gzh.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmk.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://ghi.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hak.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://ccp.kuanghao11.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://erv.meibo888.top

[Q88] 行转列（条件聚合）
来源：http://nea.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qmd.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bym.iojbl.cn

[Q89] 判断表是否存在
来源：http://plr.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xxw.mhx1999.top

[Q90] 生成序号列
来源：http://dbp.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cos.zycfv.cn

================================================================================
来源：http://gxd.jiagoushi.top


<!-- 参考信息 -->