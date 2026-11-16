代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fcm.fengsongda.top

JS:   async function f() { await g(); }
来源：http://jgk.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tbl.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vmg.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ply.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gfj.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://zax.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://zfq.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://fiu.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jet.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://rwr.hammf.cn

TS:   await Promise.all(tasks)
来源：http://txf.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sfu.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ohl.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://cff.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fne.jinqigfzy.top

[O06] 使用进程池
来源：http://dcn.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lrr.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jnd.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ouu.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://kzs.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wva.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ymn.dianchejie.cn

Ruby: // fork 块
来源：http://zgy.quarkkingdee.top

C#:   Parallel.For
来源：http://mox.zhijiandao.cn

================================================================================
来源：http://mwc.quarkkingdee.top

P. 常用工具函数
来源：http://zos.hesvh.cn

================================================================================
来源：http://imv.smart0.xyz

[P01] 生成 UUID
来源：http://vxm.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://mrz.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wnu.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://qsd.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://rgt.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://xej.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://ngl.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://phb.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://hco.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://lct.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jht.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wia.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://otp.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://avr.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ybk.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rnx.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://syq.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kao.andypj.xyz

[P03] 生成短随机字符串
来源：http://izq.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fkj.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sec.iojbl.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mzb.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vsb.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ikc.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iwg.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tbv.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://loi.guowangkeji.top

[P04] 求长度
来源：http://xip.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iul.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hjo.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryb.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsn.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://myq.redwolf501.top

Go:   len(arr);  len(m)
来源：http://rip.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://nka.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://mna.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://loq.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ilh.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fdx.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vkx.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ztw.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bqi.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://ldg.gotoacloud.top

Ruby: a == b
来源：http://gxs.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gai.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ykh.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://neg.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://uzp.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://awk.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://wit.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jbi.cashguo.top

Go:   if x == nil {}
来源：http://zlo.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zrt.yuxming.cn

C#:   if (x is null) {}
来源：http://rpn.zdbjq.cn

[P07] 防抖与节流
来源：http://fxm.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xze.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://trx.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fgy.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://knq.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tfe.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pmi.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xjo.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iem.zycfv.cn

[P08] 处理浮点精度问题
来源：http://ncw.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pxs.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oky.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://irt.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nkc.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqi.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gvi.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vew.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gxv.hcnkem.com

================================================================================
来源：http://cwh.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fys.daria6918.cn

================================================================================
来源：http://jhx.birdmap.top

[Q01] 创建表
来源：http://pbc.chenlongwang.top

CREATE TABLE users (
来源：http://uyn.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efg.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://ifq.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://cun.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qvq.yuxming.cn

);
来源：http://kcd.tian-w.cn

[Q02] 创建带外键的表
来源：http://gbn.zhoulong.xyz

CREATE TABLE orders (
来源：http://mqe.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://htw.iojbl.cn

user_id INT NOT NULL,
来源：http://gqw.tian-w.cn

amount DECIMAL(10, 2),
来源：http://uqf.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ilo.vqdsnc.cn

);
来源：http://ekq.bjfxy.top

[Q03] 增加列
来源：http://atv.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iff.yanxiufei.cn

[Q04] 修改列类型
来源：http://pac.vqdsnc.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aop.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://zwf.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nli.zhongyouzk.top

[Q06] 删除列
来源：http://coc.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yfx.cqqwz.cn

[Q07] 删除表
来源：http://lwv.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://gzz.daria6918.cn

[Q08] 创建普通索引
来源：http://wyk.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://irw.52xcode.cn

[Q09] 创建唯一索引
来源：http://uhe.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://edz.aibaodan.cn

[Q10] 插入单行
来源：http://tyt.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mru.zhongyouzk.top

[Q11] 一次插入多行
来源：http://smi.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://paq.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://qmi.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cuo.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eav.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://qzb.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://def.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://wra.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://txu.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zyj.wangdashe.top

[Q15] 查询全部
来源：http://fos.uphjek.com

SELECT * FROM users;
来源：http://rvt.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://azf.hysaishi.cn

SELECT id, name FROM users;
来源：http://hxl.hesvh.cn

[Q17] 条件查询
来源：http://dqt.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://etu.hysaishi.cn

[Q18] 模糊匹配
来源：http://ben.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lob.xuetiantiany.cn

[Q19] 范围查询
来源：http://brj.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://obt.fengsongda.top

[Q20] IN 列表
来源：http://ymk.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dtc.hammf.cn

[Q21] 空值判断
来源：http://qua.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zuv.9152youxi.cn

[Q22] 排序
来源：http://bwe.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ybp.cqqwz.cn

[Q23] 分页
来源：http://kqt.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhm.sufxvd.cn

[Q24] 去重
来源：http://ykq.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://yrl.xylfe.cn

[Q25] 只取前 N 条
来源：http://fcl.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kcq.jinqigufen.top

[Q26] 计数
来源：http://nhd.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://rxu.zhongyouzk.top

[Q27] 条件计数
来源：http://wfc.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qcg.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://tmf.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rwb.hnqzz.top

[Q29] 最大最小值
来源：http://avt.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ejb.kuanghao11.cn

[Q30] 分组统计
来源：http://jxw.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gjm.sysykeji.top

[Q31] 分组后过滤
来源：http://fka.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpo.cheryme.top

[Q32] 分组拼接字符串
来源：http://gic.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://apr.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://czf.snrcjt.cn

[Q33] 多列分组
来源：http://vck.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vmr.uphjek.com

[Q34] 每组取第一条
来源：http://acs.wangshuangyany.cn

SELECT * FROM (
来源：http://mxp.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jcm.xziqi.cn

) t WHERE rn = 1;
来源：http://rgr.wangdashe.top

[Q35] 内连接
来源：http://ybm.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fqj.shangyingyoupin.top

[Q36] 左连接
来源：http://sxo.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://opr.tarul.cn

[Q37] 右连接
来源：http://meg.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://npl.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tpv.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://itr.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://ror.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gxj.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://alg.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://whh.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://har.zdbjq.cn

[Q41] 多表连接
来源：http://emu.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eth.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://aln.sweek.top

JOIN products p ON p.id = o.product_id;
来源：http://juo.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://hqm.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://yep.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bik.zhiwuduotai.top

[Q43] 标量子查询
来源：http://plq.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ydj.yangfankeji.com

[Q44] IN 子查询
来源：http://gyp.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kzm.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://wdq.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qcu.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://czr.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://msr.hnxiangtu.top

[Q47] 与平均值比较
来源：http://dyd.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qsx.cheryme.top

[Q48] CTE 公用表表达式
来源：http://adz.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qpi.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://jta.daxiang520.top

[Q49] 更新单行
来源：http://ich.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lvy.hywenlv.cn

[Q50] 批量更新
来源：http://eab.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hep.aizwys.cn

[Q51] 用子查询更新
来源：http://bgk.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://omo.mhx1999.top

[Q52] 删除指定行
来源：http://nzl.gogol.net.cn

DELETE FROM users WHERE id = 10;
来源：http://oak.chenjidiqi.icu

[Q53] 按条件删除
来源：http://mde.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kkt.316326.xyz

[Q54] 清空表
来源：http://wee.ivvv.top

TRUNCATE TABLE logs;
来源：http://ayp.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://iwl.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pdh.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://pxy.chenlongwang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tng.cucudq.cn

[Q57] 行号
来源：http://juj.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bro.bbcook.cn

[Q58] 累计求和
来源：http://czv.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zvq.cheryme.top

[Q59] 分组内累计
来源：http://pdg.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ogl.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://vyb.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vwl.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cke.cashguo.top

[Q61] 移动平均
来源：http://jaz.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ukf.fanxiaobao.xyz

[Q62] 分组占比
来源：http://qtk.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://geb.yfazqb.com

[Q63] 开启事务
来源：http://iul.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://bzo.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://dkd.gaohongyu789.top

COMMIT;
来源：http://xeh.zhijiandao.cn

[Q65] 回滚事务
来源：http://siy.tanke756.top

ROLLBACK;
来源：http://qdb.feifeiyinyue.top

[Q66] 行锁查询
来源：http://bby.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ias.snrcjt.cn

[Q67] 设置隔离级别
来源：http://lkt.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uhj.yanxiufei.cn

[Q68] 保存点
来源：http://mru.mhx1999.top

SAVEPOINT sp1;
来源：http://emv.sxryk.cn

ROLLBACK TO sp1;
来源：http://orl.sxryk.cn

[Q69] 查看执行计划
来源：http://siu.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdb.fehbvm.com

[Q70] 更新统计信息
来源：http://waw.dashuyun.cn

ANALYZE TABLE users;
来源：http://bro.xuetiantiany.cn

[Q71] 查看建表语句
来源：http://iii.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wlq.cdnleiting.top

[Q72] 查看索引
来源：http://iao.cucudq.cn

SHOW INDEX FROM users;
来源：http://hkp.jianghu66.top

[Q73] 查看表状态
来源：http://igj.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uxl.xuetiantiany.cn

[Q74] 强制使用索引
来源：http://eov.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aom.gogol.net.cn

[Q75] 日期格式化
来源：http://jyh.sufxvd.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vxx.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xjh.gaohongyu789.top

[Q76] 按天统计
来源：http://rjv.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tml.jqgufenzy.top

[Q77] 时间加减
来源：http://eqm.yj20258.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xoi.havefunace.top

[Q78] 当前时间
来源：http://qfd.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ytb.yuanzhike.top

[Q79] 字符串拼接
来源：http://ijc.c1oappe.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mnh.hnqzz.top

[Q80] 字符串截取
来源：http://ayr.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hyx.mhx1999.top

[Q81] 字符串替换
来源：http://qdt.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yhe.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://rdj.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://epd.yangfankeji.com

[Q83] 大小写转换
来源：http://unt.jinghuilouyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vla.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://paf.0kj1m.cn

SELECT TRIM(name) FROM users;
来源：http://jex.tianlin.xyz

[Q85] 数值取整
来源：http://gdt.ydzc1.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dik.meibo888.top

[Q86] 读取 JSON 字段
来源：http://czu.9152youxi.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ajh.yj20258.top

[Q87] JSON 字段做条件
来源：http://qtd.fehbvm.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nsi.xingfuxueyuan.xyz


<!-- 参考信息 -->