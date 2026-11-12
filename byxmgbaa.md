代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ron.ppjwa.cn

TS:   // 同 JS
来源：http://vcp.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://qik.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hde.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tee.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://vxy.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://ems.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://pdr.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yhc.fzhhl.top

JS:   async function f() { await g(); }
来源：http://mmx.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewd.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cjx.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://syb.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://rlj.yj202588.top

C#:   async Task F() { await G(); }
来源：http://six.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://zkm.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://znv.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yev.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://lsm.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://rvo.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hvp.52xcode.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kii.tian-w.cn

Ruby: threads.map(&:join)
来源：http://rgj.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://uvq.yuanzhike.top

[O06] 使用进程池
来源：http://fqm.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fxw.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://upg.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://wtc.birdmap.top

TS:   // child_process / cluster 模块
来源：http://lje.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hmn.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mpk.guowangkeji.top

Ruby: // fork 块
来源：http://tlu.gogol.net.cn

C#:   Parallel.For
来源：http://smf.zhongyouzk.top

================================================================================
来源：http://pcn.chenjidiqi.icu

P. 常用工具函数
来源：http://moq.jinyuanbaomall.cn

================================================================================
来源：http://brm.sxryk.cn

[P01] 生成 UUID
来源：http://wja.tarul.cn

Py:   str(uuid.uuid4())
来源：http://xrx.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vqx.fehbvm.com

JS:   crypto.randomUUID()
来源：http://yeg.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://icn.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://fnv.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://shs.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://kuw.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://ptk.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://qrj.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ssl.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ths.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qjv.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lly.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qut.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rta.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dyc.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://alj.tian-w.cn

[P03] 生成短随机字符串
来源：http://jjk.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://onc.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lnv.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cmj.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://enk.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fno.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mrf.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bkm.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aci.yuanzhike.top

[P04] 求长度
来源：http://odv.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hsl.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwk.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aty.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jup.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://ugs.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://epx.dashuyun.cn

Ruby: x.length;  x.size
来源：http://vwn.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sjr.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://suy.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://vdd.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hzv.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gue.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ktc.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xmm.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://zou.jinghuilouyu.cn

Ruby: a == b
来源：http://irr.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nlm.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fbn.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ncv.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://meq.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cxi.jiagoushi.top

TS:   if (x == null) {}
来源：http://efh.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://amw.cheryme.top

Go:   if x == nil {}
来源：http://vqu.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rzh.gotoacloud.top

C#:   if (x is null) {}
来源：http://bdj.xylfe.cn

[P07] 防抖与节流
来源：http://fix.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uru.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://gsf.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqw.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eck.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gdu.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://svq.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://huq.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gly.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://gqg.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hnc.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rwr.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kfo.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://idd.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nra.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xse.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yuj.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pbh.zhijiandao.cn

================================================================================
来源：http://zfu.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xla.wangshuangyany.cn

================================================================================
来源：http://tww.birdmap.top

[Q01] 创建表
来源：http://ami.sysykeji.top

CREATE TABLE users (
来源：http://ytn.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://puz.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://dfv.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://qmm.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hyr.meibo888.top

);
来源：http://gxd.ehwqpu.com

[Q02] 创建带外键的表
来源：http://spz.cqqwz.cn

CREATE TABLE orders (
来源：http://sqs.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sbe.tianlin.xyz

user_id INT NOT NULL,
来源：http://qcc.pycfn.com

amount DECIMAL(10, 2),
来源：http://lqd.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ndy.gzhubu.top

);
来源：http://doa.hnxiangtu.top

[Q03] 增加列
来源：http://mmr.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hzz.smart0.xyz

[Q04] 修改列类型
来源：http://ycw.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mvi.yongpay.top

[Q05] 重命名列
来源：http://unp.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hbr.mhx1999.top

[Q06] 删除列
来源：http://gzr.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://uzw.chenlongwang.top

[Q07] 删除表
来源：http://uiv.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://zfw.dianchejie.cn

[Q08] 创建普通索引
来源：http://xgs.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bny.yuanzhike.top

[Q09] 创建唯一索引
来源：http://llx.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dzj.c1oappe.top

[Q10] 插入单行
来源：http://aou.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://itc.hesvh.cn

[Q11] 一次插入多行
来源：http://uqf.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qiq.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://guv.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://xxu.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cgi.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://gzf.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fod.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://zhi.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cbm.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zsu.kuanghao11.cn

[Q15] 查询全部
来源：http://ung.uphjek.com

SELECT * FROM users;
来源：http://oyp.hesvh.cn

[Q16] 查询指定列
来源：http://bsa.shuidangran.top

SELECT id, name FROM users;
来源：http://zfy.havefunace.top

[Q17] 条件查询
来源：http://hln.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fcu.redwolf501.top

[Q18] 模糊匹配
来源：http://nvh.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rpd.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://eyr.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ucw.wangdashe.top

[Q20] IN 列表
来源：http://iwv.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://grn.zycfv.cn

[Q21] 空值判断
来源：http://vze.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://arf.yj202588.top

[Q22] 排序
来源：http://eae.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ohf.xuanzx.com

[Q23] 分页
来源：http://nnt.fengsongda.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vnd.xinyue.icu

[Q24] 去重
来源：http://yuc.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://vjd.daria6918.cn

[Q25] 只取前 N 条
来源：http://mej.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://otl.316326.xyz

[Q26] 计数
来源：http://bed.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://iaa.chenjidiqi.icu

[Q27] 条件计数
来源：http://qhl.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xrf.snrcjt.cn

[Q28] 求和与平均
来源：http://ryl.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://usx.jlsjyb.cn

[Q29] 最大最小值
来源：http://tce.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fbq.ivvv.top

[Q30] 分组统计
来源：http://qvj.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kqz.fengsongda.top

[Q31] 分组后过滤
来源：http://ojw.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wsu.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://opq.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uqy.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ptn.ybcxt.top

[Q33] 多列分组
来源：http://vmt.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hfy.zdqjudy.top

[Q34] 每组取第一条
来源：http://qeh.cashguo.top

SELECT * FROM (
来源：http://zqd.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gli.hammf.cn

) t WHERE rn = 1;
来源：http://jgl.zhiwuduotai.top

[Q35] 内连接
来源：http://dnr.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hoo.jinghuilouyu.cn

[Q36] 左连接
来源：http://izx.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pwt.yfazqb.com

[Q37] 右连接
来源：http://afc.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://njd.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cgs.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zto.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://mfe.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://woh.kuanghao11.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://olt.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://rva.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://min.yvedp.cn

[Q41] 多表连接
来源：http://bhk.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wva.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://rlj.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://tyh.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://qcm.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://xil.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dih.wangshuangyany.cn

[Q43] 标量子查询
来源：http://rgy.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imj.shangyingyoupin.top

[Q44] IN 子查询
来源：http://hfe.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uhu.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://juo.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://knk.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://jam.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vhh.guowangkeji.top

[Q47] 与平均值比较
来源：http://ufa.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dem.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://jvf.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ygi.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://pdh.sjlbkw.cn

[Q49] 更新单行
来源：http://dvj.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yfr.gotoacloud.top

[Q50] 批量更新
来源：http://faj.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yol.hesvh.cn

[Q51] 用子查询更新
来源：http://byn.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lja.jiagoushi.top

[Q52] 删除指定行
来源：http://mrv.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://oql.52xcode.cn

[Q53] 按条件删除
来源：http://met.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://alz.feifeiyinyue.top

[Q54] 清空表
来源：http://pwy.zycfv.cn

TRUNCATE TABLE logs;
来源：http://wgp.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://ymh.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://afj.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://otv.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jzj.havefunace.top

[Q57] 行号
来源：http://ydd.feifeiyinyue.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vef.zdbjq.cn

[Q58] 累计求和
来源：http://tyn.tianlin.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ljb.guannengcc.top

[Q59] 分组内累计
来源：http://aaq.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ivj.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://xam.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://epk.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vxe.nwbrower.top

[Q61] 移动平均
来源：http://hgb.zhijiandao.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zrz.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://oxx.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tsq.nanxinkj.top

[Q63] 开启事务
来源：http://rhf.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ief.pycfn.com

[Q64] 提交事务
来源：http://skv.wangshuangyany.cn

COMMIT;
来源：http://twm.jinqigufen.top

[Q65] 回滚事务
来源：http://svp.quarkkingdee.top

ROLLBACK;
来源：http://ynp.feifeiyinyue.top

[Q66] 行锁查询
来源：http://ilj.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fpp.cashguo.top

[Q67] 设置隔离级别
来源：http://xzc.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hkz.yangfankeji.com

[Q68] 保存点
来源：http://gjh.cqqwz.cn

SAVEPOINT sp1;
来源：http://idf.wangdashe.top

ROLLBACK TO sp1;
来源：http://yme.hysaishi.cn

[Q69] 查看执行计划
来源：http://exp.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wgf.gzhubu.top

[Q70] 更新统计信息
来源：http://ogc.tanke756.top

ANALYZE TABLE users;
来源：http://hdn.jinqigufen.top

[Q71] 查看建表语句
来源：http://rwp.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ncd.fengsongda.top

[Q72] 查看索引
来源：http://pgu.yueranfly.top

SHOW INDEX FROM users;
来源：http://ksd.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://fak.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dom.yonumen.top

[Q74] 强制使用索引
来源：http://zfp.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nfm.shanyushiyangkeji.top

[Q75] 日期格式化
来源：http://sfs.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lxr.pengpengdd.cyou

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rlt.nanxuanxn.top

[Q76] 按天统计
来源：http://ple.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://btk.iojbl.cn

[Q77] 时间加减
来源：http://max.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lyd.guannengcc.top

[Q78] 当前时间
来源：http://byw.quarkkingdee.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://puf.mhx1999.top

[Q79] 字符串拼接
来源：http://men.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dfi.uphjek.com

[Q80] 字符串截取
来源：http://ohv.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qng.cucudq.cn

[Q81] 字符串替换
来源：http://pyh.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tpo.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://wnn.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://slr.yangfankeji.com

[Q83] 大小写转换
来源：http://wmj.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nal.vehdjk.com


<!-- 参考信息 -->