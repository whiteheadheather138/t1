代发 wailian999

TS:   // worker_threads 线程池
来源：http://zav.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://wgg.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wxn.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eod.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dre.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://eyy.yj20258.top

Py:   with lock: shared += 1
来源：http://qwl.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://xqz.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vdu.zdbjq.cn

TS:   // 同 JS
来源：http://kcv.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://ugp.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ero.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nsx.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://jkw.ybcxt.top

[O04] 定义异步函数并等待
来源：http://njp.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://dyi.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xiq.daria6918.cn

JS:   async function f() { await g(); }
来源：http://ofn.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pea.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gcs.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rqu.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wbg.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://pmj.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://cjo.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://cae.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ceu.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://ybs.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://cuc.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://taj.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xfw.smart0.xyz

Ruby: threads.map(&:join)
来源：http://zci.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gqt.chenzaomai.com

[O06] 使用进程池
来源：http://sav.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hec.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://noa.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://gom.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://gfz.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ajm.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xzk.cucudq.cn

Ruby: // fork 块
来源：http://jlc.shangyingyoupin.top

C#:   Parallel.For
来源：http://htc.epnwcf.com

================================================================================
来源：http://tmq.fktsv.cn

P. 常用工具函数
来源：http://itl.wangshuangyany.cn

================================================================================
来源：http://xxj.xuetiantiany.cn

[P01] 生成 UUID
来源：http://szf.havefunace.top

Py:   str(uuid.uuid4())
来源：http://obc.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://heg.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://xtd.yuxming.cn

TS:   crypto.randomUUID()
来源：http://aah.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://gii.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://nxi.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://fwh.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://icx.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://wul.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xog.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lhx.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://poq.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yed.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qlm.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eze.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tbb.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://muc.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://ogk.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ckn.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ahm.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pbb.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zka.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rcl.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qrz.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://adj.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tha.jinyuanbaomall.cn

[P04] 求长度
来源：http://cjv.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nms.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rik.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xzc.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ckn.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://zfn.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://gwj.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://fhr.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fmm.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://uzj.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://znx.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ulz.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://opl.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://scl.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fuh.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://pfd.chenlongwang.top

Ruby: a == b
来源：http://skb.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kbb.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://stf.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://txm.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://uev.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pep.cdnleiting.top

TS:   if (x == null) {}
来源：http://vxu.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://yrk.aibaodan.cn

Go:   if x == nil {}
来源：http://snv.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uyo.hcnkem.com

C#:   if (x is null) {}
来源：http://lej.yonumen.top

[P07] 防抖与节流
来源：http://ser.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://osb.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://rfa.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwa.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptx.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ife.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swa.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wug.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vvr.daria6918.cn

[P08] 处理浮点精度问题
来源：http://jqo.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wtb.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://doi.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mcq.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ccz.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vyf.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ghj.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wka.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cij.gotoacloud.top

================================================================================
来源：http://xlw.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iib.sxryk.cn

================================================================================
来源：http://xis.xylfe.cn

[Q01] 创建表
来源：http://vrd.ydjk.org.cn

CREATE TABLE users (
来源：http://owg.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ada.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://iyr.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://khq.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hio.bbcook.cn

);
来源：http://sun.jianghu66.top

[Q02] 创建带外键的表
来源：http://ogz.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://uoo.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ezu.jyoumei.cn

user_id INT NOT NULL,
来源：http://ruf.shuidangran.top

amount DECIMAL(10, 2),
来源：http://sha.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zsb.pycfn.com

);
来源：http://iyo.xinyue.icu

[Q03] 增加列
来源：http://luq.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jer.daxiang520.top

[Q04] 修改列类型
来源：http://qvi.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fro.sjlbkw.cn

[Q05] 重命名列
来源：http://hml.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eqy.sufxvd.cn

[Q06] 删除列
来源：http://kdb.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://buc.xylfe.cn

[Q07] 删除表
来源：http://ykb.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://fwq.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://she.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tnv.jinqigufen.top

[Q09] 创建唯一索引
来源：http://swv.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gjk.yuxming.cn

[Q10] 插入单行
来源：http://bfp.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ydm.wangdashe.top

[Q11] 一次插入多行
来源：http://izn.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sjo.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://dxc.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://jdo.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vzk.0kj1m.cn

[Q13] 忽略重复插入
来源：http://afc.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://epj.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://gqy.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgj.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aux.chenlongwang.top

[Q15] 查询全部
来源：http://klm.yuanzhike.top

SELECT * FROM users;
来源：http://hdf.yj202588.top

[Q16] 查询指定列
来源：http://rir.sysykeji.top

SELECT id, name FROM users;
来源：http://ylq.feifeiyinyue.top

[Q17] 条件查询
来源：http://jkw.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aiw.sufxvd.cn

[Q18] 模糊匹配
来源：http://jlr.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iai.fanxiaobao.xyz

[Q19] 范围查询
来源：http://mon.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ctb.hnqzz.top

[Q20] IN 列表
来源：http://pzm.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fnw.cdnleiting.top

[Q21] 空值判断
来源：http://dbd.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mij.zhoulong.xyz

[Q22] 排序
来源：http://pau.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tki.uphjek.com

[Q23] 分页
来源：http://sax.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rbf.epnwcf.com

[Q24] 去重
来源：http://tkc.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://kxb.chenzaomai.com

[Q25] 只取前 N 条
来源：http://txk.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kkq.yanxiufei.cn

[Q26] 计数
来源：http://cuk.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://scp.guannengcc.top

[Q27] 条件计数
来源：http://yiv.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cxg.ehwqpu.com

[Q28] 求和与平均
来源：http://htb.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uya.ctjpmb.com

[Q29] 最大最小值
来源：http://pzd.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fii.zhijiandao.cn

[Q30] 分组统计
来源：http://cdb.nanxuanxn.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jpk.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://kyq.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rib.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://paf.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oiv.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kew.fzhhl.top

[Q33] 多列分组
来源：http://sco.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zik.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://phf.nanxinkj.top

SELECT * FROM (
来源：http://yyh.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pag.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://zcc.jinghuilouyu.cn

[Q35] 内连接
来源：http://vtz.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zvp.zhengqikj.top

[Q36] 左连接
来源：http://lps.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ghq.chenzaomai.com

[Q37] 右连接
来源：http://lgy.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qdo.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://ryg.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://phw.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://lvu.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kcz.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pys.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zal.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ecd.hongshengwenyu.top

[Q41] 多表连接
来源：http://qsb.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hxs.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://vuh.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://qro.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://snl.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://jet.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://otd.yj20258888.top

[Q43] 标量子查询
来源：http://dty.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xme.zdbjq.cn

[Q44] IN 子查询
来源：http://kxq.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hrv.wangdashe.top

[Q45] EXISTS 判断存在
来源：http://sgy.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fln.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://bvi.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ujx.yuxming.cn

[Q47] 与平均值比较
来源：http://fmv.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wyr.ivvv.top

[Q48] CTE 公用表表达式
来源：http://bqh.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mvs.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://qld.ydjk.org.cn

[Q49] 更新单行
来源：http://wsb.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rbk.yueranfly.top

[Q50] 批量更新
来源：http://pui.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://muh.pycfn.com

[Q51] 用子查询更新
来源：http://gyh.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gjm.hfpthk.cn

[Q52] 删除指定行
来源：http://pcc.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://ldh.tarul.cn

[Q53] 按条件删除
来源：http://daz.jqgufenzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ind.vehdjk.com

[Q54] 清空表
来源：http://qdw.hnqzz.top

TRUNCATE TABLE logs;
来源：http://eaj.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://agc.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wyh.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://hbn.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dtq.yj202588.top

[Q57] 行号
来源：http://gww.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xtv.zhongyouzk.top

[Q58] 累计求和
来源：http://jxe.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://avr.andypj.xyz

[Q59] 分组内累计
来源：http://lap.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qdz.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://mxt.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ewc.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vgv.xylfe.cn

[Q61] 移动平均
来源：http://you.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oxr.shanyushiyangtech.top

[Q62] 分组占比
来源：http://vdv.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bno.pengpengdd.cyou

[Q63] 开启事务
来源：http://zdt.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qer.zhixingplan.top

[Q64] 提交事务
来源：http://swr.cqqwz.cn

COMMIT;
来源：http://uxu.yanxiufei.cn

[Q65] 回滚事务
来源：http://lml.birdmap.top

ROLLBACK;
来源：http://kii.yfazqb.com

[Q66] 行锁查询
来源：http://sdx.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eyv.tarul.cn

[Q67] 设置隔离级别
来源：http://mul.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uny.xinyue.icu

[Q68] 保存点
来源：http://dek.gzhubu.top

SAVEPOINT sp1;
来源：http://ozf.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://vyh.haohaochexian.top

[Q69] 查看执行计划
来源：http://cld.yj20258888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ahs.zdqjudy.top

[Q70] 更新统计信息
来源：http://uch.yuanzhike.top

ANALYZE TABLE users;
来源：http://bje.hysaishi.cn

[Q71] 查看建表语句
来源：http://lea.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://loj.jinqigfzy.top

[Q72] 查看索引
来源：http://fgu.shzxlz.cn

SHOW INDEX FROM users;
来源：http://moz.cqqwz.cn

[Q73] 查看表状态
来源：http://xse.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lpd.sxryk.cn

[Q74] 强制使用索引
来源：http://cwi.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hhi.fehbvm.com

[Q75] 日期格式化
来源：http://anc.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yfi.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xfd.zhongyouzk.top

[Q76] 按天统计
来源：http://san.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vco.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://mon.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cjm.guowangkeji.top

[Q78] 当前时间
来源：http://lih.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://edc.jyoumei.cn

[Q79] 字符串拼接
来源：http://vne.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rcp.meibo888.top


<!-- 参考信息 -->