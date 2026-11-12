代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jjf.tarul.cn

[O03] 加锁保护共享数据
来源：http://bef.yongpay.top

Py:   with lock: shared += 1
来源：http://psy.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://kdz.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qqk.hysaishi.cn

TS:   // 同 JS
来源：http://cqm.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://jgb.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://txh.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hwz.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://iju.uphjek.com

[O04] 定义异步函数并等待
来源：http://wcg.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://ahx.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://srv.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://vwz.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xpp.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://amd.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pev.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://gzd.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://sbe.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://yyr.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://eax.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cyt.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://hhq.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://hmu.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aqr.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://klh.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://oiz.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ogg.fanxiaobao.xyz

[O06] 使用进程池
来源：http://wxp.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dfh.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gfw.yj202588.top

JS:   // child_process / cluster 模块
来源：http://rxp.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://oxe.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vlu.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jco.316326.xyz

Ruby: // fork 块
来源：http://mcr.yanxiufei.cn

C#:   Parallel.For
来源：http://msg.tianlin.xyz

================================================================================
来源：http://fzl.316326.xyz

P. 常用工具函数
来源：http://gna.cqqwz.cn

================================================================================
来源：http://qcx.aibaodan.cn

[P01] 生成 UUID
来源：http://stm.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://iux.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mze.aizwys.cn

JS:   crypto.randomUUID()
来源：http://vnd.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://ufu.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://lzp.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://anh.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://oqo.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ljo.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://bfa.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nhq.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://uup.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yuh.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rml.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jmu.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://skf.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dqm.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iyw.xuanzx.com

[P03] 生成短随机字符串
来源：http://ggc.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pzr.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qkq.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nbt.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eff.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ocl.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fir.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://apb.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vjl.yuxming.cn

[P04] 求长度
来源：http://hts.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vni.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kga.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvv.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vkw.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://djf.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://nlf.iojbl.cn

Ruby: x.length;  x.size
来源：http://ork.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://hsg.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://sql.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rqu.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dsy.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pfr.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://stf.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sja.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sey.tanke756.top

Ruby: a == b
来源：http://yyc.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ngv.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nmn.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tfw.jyoumei.cn

PHP:  if (empty($x)) {}
来源：http://lxf.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sjl.hfpthk.cn

TS:   if (x == null) {}
来源：http://qts.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xnk.jqgufenzy.top

Go:   if x == nil {}
来源：http://yjd.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wyp.zdbjq.cn

C#:   if (x is null) {}
来源：http://bwg.cqqwz.cn

[P07] 防抖与节流
来源：http://qgh.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eok.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://gxc.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcv.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bks.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wfm.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://owo.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://npn.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://psf.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://yyn.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zyk.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://urg.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qex.ehwqpu.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pvp.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oon.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kxd.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mwv.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zfm.pengpengdd.cyou

================================================================================
来源：http://ued.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yyn.zycfv.cn

================================================================================
来源：http://tmh.yuxming.cn

[Q01] 创建表
来源：http://lyc.dashuyun.cn

CREATE TABLE users (
来源：http://rzz.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbc.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://dbw.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://rdz.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ytc.tian-w.cn

);
来源：http://vfu.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ulz.zhijiandao.cn

CREATE TABLE orders (
来源：http://ymh.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ebk.zhengqikj.top

user_id INT NOT NULL,
来源：http://mla.snrcjt.cn

amount DECIMAL(10, 2),
来源：http://vcy.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://chl.yj202588.top

);
来源：http://lvr.guannengcc.top

[Q03] 增加列
来源：http://ftt.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yqh.yj20258.top

[Q04] 修改列类型
来源：http://pgb.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jsx.xylfe.cn

[Q05] 重命名列
来源：http://lro.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wkn.andypj.xyz

[Q06] 删除列
来源：http://dwt.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gqj.ybcxt.top

[Q07] 删除表
来源：http://lat.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://rne.daxiang520.top

[Q08] 创建普通索引
来源：http://ymv.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fpi.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://yza.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tqj.sysykeji.top

[Q10] 插入单行
来源：http://eqb.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cnf.ydzc1.top

[Q11] 一次插入多行
来源：http://owr.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dck.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://nar.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://jiz.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sho.jqgfzy.top

[Q13] 忽略重复插入
来源：http://mzq.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxd.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://uwi.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wrc.yj202588.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://luo.jqgufenzy.top

[Q15] 查询全部
来源：http://inj.0kj1m.cn

SELECT * FROM users;
来源：http://crx.jlsjyb.cn

[Q16] 查询指定列
来源：http://gvi.tian-w.cn

SELECT id, name FROM users;
来源：http://zbm.svipenyu.cn

[Q17] 条件查询
来源：http://mgd.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zto.zhoulong.xyz

[Q18] 模糊匹配
来源：http://tnd.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://unp.mhx1999.top

[Q19] 范围查询
来源：http://snq.havefunace.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lsv.chenzaomai.com

[Q20] IN 列表
来源：http://ykx.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yof.yuxming.cn

[Q21] 空值判断
来源：http://kdf.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ife.aizwys.cn

[Q22] 排序
来源：http://dsf.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://exs.ydzc1.top

[Q23] 分页
来源：http://haz.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://diw.pengpengdd.cyou

[Q24] 去重
来源：http://fmq.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://hkm.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://ezb.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fsm.dashuyun.cn

[Q26] 计数
来源：http://oda.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://iuh.fktsv.cn

[Q27] 条件计数
来源：http://wqc.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cif.yvedp.cn

[Q28] 求和与平均
来源：http://lbq.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lyt.shuidangran.top

[Q29] 最大最小值
来源：http://vpx.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vhy.hysaishi.cn

[Q30] 分组统计
来源：http://rhk.sweek.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gtd.cdnleiting.top

[Q31] 分组后过滤
来源：http://rcp.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bph.c1oappe.top

[Q32] 分组拼接字符串
来源：http://lzg.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bef.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vhx.chenzaomai.com

[Q33] 多列分组
来源：http://gwu.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sln.jlsjyb.cn

[Q34] 每组取第一条
来源：http://nim.xuanzx.com

SELECT * FROM (
来源：http://etx.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ejv.hfpthk.cn

) t WHERE rn = 1;
来源：http://rxg.svipenyu.cn

[Q35] 内连接
来源：http://zeh.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hlw.yj202588.top

[Q36] 左连接
来源：http://rbk.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cyp.jinghuilouyu.cn

[Q37] 右连接
来源：http://wwq.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://krw.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://fgb.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://its.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://pbk.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qhc.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jga.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ggu.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xty.hysaishi.cn

[Q41] 多表连接
来源：http://mvb.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cwt.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://viv.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://tzu.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://nok.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://kwd.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://psa.bbcook.cn

[Q43] 标量子查询
来源：http://tza.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tiw.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://cpy.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wzw.cashguo.top

[Q45] EXISTS 判断存在
来源：http://hrc.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://omb.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://drf.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oeh.wangdashe.top

[Q47] 与平均值比较
来源：http://ffg.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://msz.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://nmm.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gby.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://vec.dashuyun.cn

[Q49] 更新单行
来源：http://gdw.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://juy.uphjek.com

[Q50] 批量更新
来源：http://awr.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://caa.fzhhl.top

[Q51] 用子查询更新
来源：http://ubp.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vbm.tanke756.top

[Q52] 删除指定行
来源：http://zcj.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://ima.pengpengdd.cyou

[Q53] 按条件删除
来源：http://nji.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://obp.bjfxy.top

[Q54] 清空表
来源：http://abx.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://ffp.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://kem.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ewd.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://pbo.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehb.ctjpmb.com

[Q57] 行号
来源：http://kvf.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvk.sweek.top

[Q58] 累计求和
来源：http://kii.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tyt.wangdashe.top

[Q59] 分组内累计
来源：http://vdk.hongshengwenyu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qmv.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://xkg.ydjk.org.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cgi.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kyf.nwbrower.top

[Q61] 移动平均
来源：http://dld.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jlm.daxiang520.top

[Q62] 分组占比
来源：http://whh.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nsp.ivvv.top

[Q63] 开启事务
来源：http://dha.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.jlsjyb.cn

[Q64] 提交事务
来源：http://hcr.fktsv.cn

COMMIT;
来源：http://gny.iojbl.cn

[Q65] 回滚事务
来源：http://dvy.zdbjq.cn

ROLLBACK;
来源：http://sif.sufxvd.cn

[Q66] 行锁查询
来源：http://sgk.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dwo.jqgfzy.top

[Q67] 设置隔离级别
来源：http://rcs.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://igy.zhoulong.xyz

[Q68] 保存点
来源：http://zqm.zhengqikj.top

SAVEPOINT sp1;
来源：http://goz.fengsongda.top

ROLLBACK TO sp1;
来源：http://kkz.zhongyouzk.top

[Q69] 查看执行计划
来源：http://wdg.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yoz.haohaochexian.top

[Q70] 更新统计信息
来源：http://cry.bbcook.cn

ANALYZE TABLE users;
来源：http://drp.nwbrower.top

[Q71] 查看建表语句
来源：http://stw.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rxw.redwolf501.top

[Q72] 查看索引
来源：http://qyi.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://kzk.aizwys.cn

[Q73] 查看表状态
来源：http://qrw.meibo888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ksd.ppjwa.cn

[Q74] 强制使用索引
来源：http://rjd.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://por.chenzaomai.com

[Q75] 日期格式化
来源：http://eca.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uow.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zok.xuanzx.com

[Q76] 按天统计
来源：http://gma.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jhg.ydjk.org.cn

[Q77] 时间加减
来源：http://fyo.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eno.mhx1999.top

[Q78] 当前时间
来源：http://gpw.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kgv.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://fxb.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iiv.jinqigufen.top

[Q80] 字符串截取
来源：http://ykd.yvedp.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://eyx.tian-w.cn

[Q81] 字符串替换
来源：http://ope.feifeiyinyue.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ohw.ehwqpu.com


<!-- 参考信息 -->