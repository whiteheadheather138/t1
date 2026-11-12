代发 wailian999

================================================================================
来源：http://wcz.sufxvd.cn

O. 并发与异步
来源：http://bcb.shanyushiyangtech.top

================================================================================
来源：http://rwa.gogol.net.cn

[O01] 启动一个线程
来源：http://rjl.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oiv.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aot.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dii.hcnkem.com

TS:   // 同 JS
来源：http://kgw.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://bnf.zhixingplan.top

Go:   go f()
来源：http://csd.fktsv.cn

Ruby: Thread.new { f }
来源：http://yfx.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://flv.nanxuanxn.top

[O02] 使用线程池
来源：http://gif.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://poj.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yiy.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://cug.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://mok.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rwb.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fpu.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bbq.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hlc.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://htn.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://ttt.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://hod.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svi.yfazqb.com

TS:   // 同 JS
来源：http://zrs.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://puf.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sjq.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nim.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://isc.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://sko.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://bju.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://egw.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://irb.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gqd.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kzv.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mpk.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://arj.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://ewu.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://xxp.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://nkm.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aki.meibo888.top

JS:   await Promise.all(tasks)
来源：http://kzz.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://ikc.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://him.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://abk.yuxming.cn

Ruby: threads.map(&:join)
来源：http://xhi.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qvc.hysaishi.cn

[O06] 使用进程池
来源：http://ztz.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dbc.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mxh.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://yag.uphjek.com

TS:   // child_process / cluster 模块
来源：http://wyw.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hqp.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hna.zdbjq.cn

Ruby: // fork 块
来源：http://cbq.9152youxi.cn

C#:   Parallel.For
来源：http://ykc.jiagoushi.top

================================================================================
来源：http://xgp.ctjpmb.com

P. 常用工具函数
来源：http://jlc.svipenyu.cn

================================================================================
来源：http://lox.sweek.top

[P01] 生成 UUID
来源：http://ztb.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://opu.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tzf.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://des.ivvv.top

TS:   crypto.randomUUID()
来源：http://cxp.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://cjy.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://ryh.uphjek.com

Ruby: SecureRandom.uuid
来源：http://rez.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://spq.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://vbn.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nbk.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://whd.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exz.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://umm.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://anr.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rvo.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dqc.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oig.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://pln.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iht.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hwn.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqw.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svq.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ogg.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mpk.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ytp.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kfw.jiagoushi.top

[P04] 求长度
来源：http://qwv.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nhz.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ixy.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cne.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rhn.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://ixq.aizwys.cn

Go:   len(arr);  len(m)
来源：http://hdi.redwolf501.top

Ruby: x.length;  x.size
来源：http://fdm.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wug.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://wji.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hyv.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ayn.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iyw.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://own.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dlt.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://qug.jinghuilouyu.cn

Ruby: a == b
来源：http://edw.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zgn.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://edw.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eue.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://nkg.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hix.mhx1999.top

TS:   if (x == null) {}
来源：http://wyp.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qlg.smart0.xyz

Go:   if x == nil {}
来源：http://yzz.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kgk.meibo888.top

C#:   if (x is null) {}
来源：http://sjm.aizwys.cn

[P07] 防抖与节流
来源：http://xri.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aix.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://plc.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgp.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwo.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wrp.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hck.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://uin.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pmo.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://csv.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ehe.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cqf.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wbt.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://unp.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jsn.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jgy.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jjs.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zon.jinyuanbaomall.cn

================================================================================
来源：http://ylf.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bsp.quarkkingdee.top

================================================================================
来源：http://bgd.nwbrower.top

[Q01] 创建表
来源：http://dtd.316326.xyz

CREATE TABLE users (
来源：http://pdk.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://umw.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://kro.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://wpm.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tbl.zhijiandao.cn

);
来源：http://tuq.yueranfly.top

[Q02] 创建带外键的表
来源：http://xuj.cdnleiting.top

CREATE TABLE orders (
来源：http://mtj.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lci.yongpay.top

user_id INT NOT NULL,
来源：http://zoe.cheryme.top

amount DECIMAL(10, 2),
来源：http://tnj.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xkj.zhengqikj.top

);
来源：http://xtn.hongshengwenyu.top

[Q03] 增加列
来源：http://yoe.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://maq.svipenyu.cn

[Q04] 修改列类型
来源：http://nja.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ayg.zhongyouzk.top

[Q05] 重命名列
来源：http://iee.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jbd.hnxiangtu.top

[Q06] 删除列
来源：http://wyf.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://otx.316326.xyz

[Q07] 删除表
来源：http://cjf.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://fmr.quarkkingdee.top

[Q08] 创建普通索引
来源：http://xef.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://put.cqqwz.cn

[Q09] 创建唯一索引
来源：http://upa.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nfk.havefunace.top

[Q10] 插入单行
来源：http://npp.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tnj.mhx1999.top

[Q11] 一次插入多行
来源：http://mlj.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://umn.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://diu.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://tzc.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dzh.shzxlz.cn

[Q13] 忽略重复插入
来源：http://lpp.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cep.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://uhs.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lqc.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtc.jqgufenzy.top

[Q15] 查询全部
来源：http://ylj.guannengcc.top

SELECT * FROM users;
来源：http://aoi.kuanghao11.cn

[Q16] 查询指定列
来源：http://fdy.havefunace.top

SELECT id, name FROM users;
来源：http://stt.jqgfzy.top

[Q17] 条件查询
来源：http://yfa.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yjp.yj20258888.top

[Q18] 模糊匹配
来源：http://uac.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iaj.daxiang520.top

[Q19] 范围查询
来源：http://ggf.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mwu.jianghu66.top

[Q20] IN 列表
来源：http://pzo.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://udr.hammf.cn

[Q21] 空值判断
来源：http://fse.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fpz.ydzc1.top

[Q22] 排序
来源：http://frm.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fff.fengsongda.top

[Q23] 分页
来源：http://enb.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmp.snrcjt.cn

[Q24] 去重
来源：http://rdf.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://fyx.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://ogk.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mia.fktsv.cn

[Q26] 计数
来源：http://iuk.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://mwb.uphjek.com

[Q27] 条件计数
来源：http://lzn.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ezi.redwolf501.top

[Q28] 求和与平均
来源：http://dfy.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wxe.9152youxi.cn

[Q29] 最大最小值
来源：http://lzw.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pno.fktsv.cn

[Q30] 分组统计
来源：http://eqj.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mta.fehbvm.com

[Q31] 分组后过滤
来源：http://ths.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zfj.pycfn.com

[Q32] 分组拼接字符串
来源：http://knd.daxiang520.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xwc.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ent.cqqwz.cn

[Q33] 多列分组
来源：http://der.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ozd.smart0.xyz

[Q34] 每组取第一条
来源：http://pvt.yonumen.top

SELECT * FROM (
来源：http://svk.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tbn.sxryk.cn

) t WHERE rn = 1;
来源：http://baa.guowangkeji.top

[Q35] 内连接
来源：http://jju.pengpengdd.cyou

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bsl.nanxuanxn.top

[Q36] 左连接
来源：http://hbr.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jjt.aizwys.cn

[Q37] 右连接
来源：http://qaj.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fxp.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bob.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ghb.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://lon.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bpj.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gmq.zhixingplan.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vlm.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://onz.cheryme.top

[Q41] 多表连接
来源：http://tpn.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lzp.jqgfzy.top

JOIN users u ON u.id = o.user_id
来源：http://gij.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://kxc.uphjek.com

[Q42] 连接条件附加过滤
来源：http://eas.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://ica.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lhc.havefunace.top

[Q43] 标量子查询
来源：http://zyw.wangdashe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dzx.yj20258888.top

[Q44] IN 子查询
来源：http://dsg.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uqz.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://bfy.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bww.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jma.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ksy.ehwqpu.com

[Q47] 与平均值比较
来源：http://vvs.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lhj.tarul.cn

[Q48] CTE 公用表表达式
来源：http://tdv.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zfj.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://rje.yueranfly.top

[Q49] 更新单行
来源：http://pox.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wly.hfpthk.cn

[Q50] 批量更新
来源：http://pvn.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://csh.c1oappe.top

[Q51] 用子查询更新
来源：http://jtg.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://diu.ydzc1.top

[Q52] 删除指定行
来源：http://jtj.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://msd.jianghu66.top

[Q53] 按条件删除
来源：http://fph.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://crj.gogol.net.cn

[Q54] 清空表
来源：http://vom.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://avx.sysykeji.top

[Q55] 排名（并列占位）
来源：http://acu.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lqo.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://bis.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddh.yj20258.top

[Q57] 行号
来源：http://wdt.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dju.zhongyouzk.top

[Q58] 累计求和
来源：http://uqb.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://agd.guowangkeji.top

[Q59] 分组内累计
来源：http://yiz.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dba.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://lgi.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dov.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rtq.fzhhl.top

[Q61] 移动平均
来源：http://dcm.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hcc.haohaochexian.top

[Q62] 分组占比
来源：http://svg.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gdp.aizwys.cn

[Q63] 开启事务
来源：http://yop.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://yso.shzxlz.cn

[Q64] 提交事务
来源：http://tdo.nanxinkj.top

COMMIT;
来源：http://qqb.zycfv.cn

[Q65] 回滚事务
来源：http://iyh.birdmap.top

ROLLBACK;
来源：http://efu.c1oappe.top

[Q66] 行锁查询
来源：http://oby.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://guf.tian-w.cn

[Q67] 设置隔离级别
来源：http://awu.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uqm.zycfv.cn

[Q68] 保存点
来源：http://nyv.nwbrower.top

SAVEPOINT sp1;
来源：http://mwn.yfazqb.com

ROLLBACK TO sp1;
来源：http://ylp.mhx1999.top

[Q69] 查看执行计划
来源：http://xef.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ohm.fehbvm.com

[Q70] 更新统计信息
来源：http://vzr.andypj.xyz

ANALYZE TABLE users;
来源：http://dbi.fengsongda.top

[Q71] 查看建表语句
来源：http://wfy.fehbvm.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vqc.nanxinkj.top

[Q72] 查看索引
来源：http://feq.zhixingplan.top


<!-- 参考信息 -->