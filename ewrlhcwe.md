代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://doo.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uce.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dhc.kuanghao11.cn

TS:   // 同 JS
来源：http://gyq.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://xua.yj20258.top

Go:   go f()
来源：http://imc.yongpay.top

Ruby: Thread.new { f }
来源：http://nox.birdmap.top

C#:   Task.Run(() => F());
来源：http://pdx.cdnleiting.top

[O02] 使用线程池
来源：http://jkc.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qlu.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ngz.wangdashe.top

JS:   // worker_threads 线程池
来源：http://kht.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://piq.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://izg.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ptj.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lxf.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kac.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://oqc.fengsongda.top

Py:   with lock: shared += 1
来源：http://evv.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://ygv.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dke.xinyue.icu

TS:   // 同 JS
来源：http://ila.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://cgl.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dgc.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gck.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://nlm.ybcxt.top

[O04] 定义异步函数并等待
来源：http://bem.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://iax.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sgy.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://ysi.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://odq.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yax.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sha.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://xsy.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://anc.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://nhl.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://kzf.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hdd.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://zat.uphjek.com

TS:   await Promise.all(tasks)
来源：http://gwf.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://urp.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://old.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://yyi.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uvr.smart0.xyz

[O06] 使用进程池
来源：http://xtv.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pxt.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://drk.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://qvh.sweek.top

TS:   // child_process / cluster 模块
来源：http://kzg.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdt.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yzh.316326.xyz

Ruby: // fork 块
来源：http://uqq.ydjk.org.cn

C#:   Parallel.For
来源：http://inv.yfazqb.com

================================================================================
来源：http://glf.xuetiantiany.cn

P. 常用工具函数
来源：http://upx.snrcjt.cn

================================================================================
来源：http://jmo.jqgfzy.top

[P01] 生成 UUID
来源：http://jpu.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://xcm.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xge.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://zrg.yfazqb.com

TS:   crypto.randomUUID()
来源：http://tmu.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://ozy.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://uwb.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://itz.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://nss.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://faf.nanxuanxn.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyr.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://elj.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cjj.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xnq.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kdr.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://axi.cdnleiting.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bda.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bjy.fzhhl.top

[P03] 生成短随机字符串
来源：http://vko.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vjt.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xxp.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qce.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iqz.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hpn.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pag.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gkf.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xvc.fanxiaobao.xyz

[P04] 求长度
来源：http://ies.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dcv.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://joi.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bjl.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cuv.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://hbn.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://zeg.tianlin.xyz

Ruby: x.length;  x.size
来源：http://mmd.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://yzr.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://crj.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ofo.chenzaomai.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ggo.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fmt.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ejv.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dsj.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://tgz.dianchejie.cn

Ruby: a == b
来源：http://uqu.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cvr.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://byy.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iof.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://wru.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xog.hesvh.cn

TS:   if (x == null) {}
来源：http://mad.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oku.yfazqb.com

Go:   if x == nil {}
来源：http://tgl.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qwa.xylfe.cn

C#:   if (x is null) {}
来源：http://jnc.dianchejie.cn

[P07] 防抖与节流
来源：http://oqr.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bfu.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://cvr.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ioy.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdy.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xlp.dashuyun.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wyz.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zuj.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xbz.hammf.cn

[P08] 处理浮点精度问题
来源：http://mql.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gnf.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vbc.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yyl.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ioj.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aac.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dys.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xiq.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://afh.zhaomingkeji.xyz

================================================================================
来源：http://lnv.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mce.yongpay.top

================================================================================
来源：http://oqp.jyoumei.cn

[Q01] 创建表
来源：http://hxa.gogol.net.cn

CREATE TABLE users (
来源：http://bqr.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nui.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://caq.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://kjv.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eah.vehdjk.com

);
来源：http://now.uphjek.com

[Q02] 创建带外键的表
来源：http://kix.c1oappe.top

CREATE TABLE orders (
来源：http://iqz.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvk.aizwys.cn

user_id INT NOT NULL,
来源：http://xef.nwbrower.top

amount DECIMAL(10, 2),
来源：http://fox.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qgk.shangyingyoupin.top

);
来源：http://trv.sysykeji.top

[Q03] 增加列
来源：http://lfu.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ehv.hnxiangtu.top

[Q04] 修改列类型
来源：http://vjr.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yvl.316326.xyz

[Q05] 重命名列
来源：http://rid.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ktn.fengsongda.top

[Q06] 删除列
来源：http://mxd.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://sfj.pengpengdd.cyou

[Q07] 删除表
来源：http://hjr.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://kge.bbcook.cn

[Q08] 创建普通索引
来源：http://nus.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://afl.svipenyu.cn

[Q09] 创建唯一索引
来源：http://byw.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yfa.daria6918.cn

[Q10] 插入单行
来源：http://ehx.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fef.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://pru.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wyy.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://lwf.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://yqp.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mqu.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://zbl.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gfu.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://oge.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cpd.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ehe.wangdashe.top

[Q15] 查询全部
来源：http://hqs.fzhhl.top

SELECT * FROM users;
来源：http://mig.quarkkingdee.top

[Q16] 查询指定列
来源：http://xrm.xziqi.cn

SELECT id, name FROM users;
来源：http://pvu.feifeiyinyue.top

[Q17] 条件查询
来源：http://bcd.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ilx.jianghu66.top

[Q18] 模糊匹配
来源：http://ohv.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zzm.fengsongda.top

[Q19] 范围查询
来源：http://bbs.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kjs.yj202588.top

[Q20] IN 列表
来源：http://esj.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kms.zhoulong.xyz

[Q21] 空值判断
来源：http://hgz.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dna.fengsongda.top

[Q22] 排序
来源：http://omt.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ojq.smart0.xyz

[Q23] 分页
来源：http://caz.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ygk.xingfuxueyuan.xyz

[Q24] 去重
来源：http://kfa.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://myh.aibaodan.cn

[Q25] 只取前 N 条
来源：http://beg.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://glu.fehbvm.com

[Q26] 计数
来源：http://mcw.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://zvx.fehbvm.com

[Q27] 条件计数
来源：http://ual.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gfl.iojbl.cn

[Q28] 求和与平均
来源：http://hnw.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://art.zhoulong.xyz

[Q29] 最大最小值
来源：http://liw.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xhu.shuidangran.top

[Q30] 分组统计
来源：http://zmd.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xfl.xziqi.cn

[Q31] 分组后过滤
来源：http://afp.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vbv.tarul.cn

[Q32] 分组拼接字符串
来源：http://qbe.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wdt.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://twe.yj202588.top

[Q33] 多列分组
来源：http://yml.jinqigfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://chf.nanxuanxn.top

[Q34] 每组取第一条
来源：http://dhe.hnqzz.top

SELECT * FROM (
来源：http://ibi.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jtx.nanxinkj.top

) t WHERE rn = 1;
来源：http://mds.hnxiangtu.top

[Q35] 内连接
来源：http://qgd.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vcg.fzhhl.top

[Q36] 左连接
来源：http://fvy.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gao.xziqi.cn

[Q37] 右连接
来源：http://lvv.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bfl.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://jut.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://slt.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://akr.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ifd.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kzb.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://urh.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fvc.hesvh.cn

[Q41] 多表连接
来源：http://cdl.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dto.dashuyun.cn

JOIN users u ON u.id = o.user_id
来源：http://hgt.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://joq.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://qeh.epnwcf.com

SELECT u.name, o.amount FROM users u
来源：http://fmf.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wxy.hongshengwenyu.top

[Q43] 标量子查询
来源：http://ayh.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gqr.jlsjyb.cn

[Q44] IN 子查询
来源：http://nci.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ygc.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://sev.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zmo.jqgufenzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://fgx.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ozb.xinyue.icu

[Q47] 与平均值比较
来源：http://rsj.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ymc.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://rwk.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsk.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://tus.xziqi.cn

[Q49] 更新单行
来源：http://cwu.guannengcc.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jvm.jiagoushi.top

[Q50] 批量更新
来源：http://tys.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fzx.guowangkeji.top

[Q51] 用子查询更新
来源：http://qxi.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hip.ydjk.org.cn

[Q52] 删除指定行
来源：http://zfh.shanyushiyangtech.top

DELETE FROM users WHERE id = 10;
来源：http://six.yuxming.cn

[Q53] 按条件删除
来源：http://ftn.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dpk.jqgufenzy.top

[Q54] 清空表
来源：http://jgx.52xcode.cn

TRUNCATE TABLE logs;
来源：http://shj.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://xpj.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fyy.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://qpo.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xqs.birdmap.top

[Q57] 行号
来源：http://gfk.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mym.guowangkeji.top

[Q58] 累计求和
来源：http://rhx.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dlo.chenzaomai.com

[Q59] 分组内累计
来源：http://wwi.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ced.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://lxk.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jrf.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iix.haohaochexian.top

[Q61] 移动平均
来源：http://cml.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qgt.cdnleiting.top

[Q62] 分组占比
来源：http://ate.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xsr.hysaishi.cn

[Q63] 开启事务
来源：http://iyg.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bcf.chenzaomai.com

[Q64] 提交事务
来源：http://hdj.zhaomingkeji.xyz

COMMIT;
来源：http://elu.zycfv.cn

[Q65] 回滚事务
来源：http://fny.daria6918.cn

ROLLBACK;
来源：http://jjp.nanxuanxn.top

[Q66] 行锁查询
来源：http://plu.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hut.cashguo.top

[Q67] 设置隔离级别
来源：http://jsq.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bjw.hesvh.cn

[Q68] 保存点
来源：http://xtb.52xcode.cn

SAVEPOINT sp1;
来源：http://rob.nanxinkj.top

ROLLBACK TO sp1;
来源：http://ulz.yueranfly.top

[Q69] 查看执行计划
来源：http://sco.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yzk.yfazqb.com

[Q70] 更新统计信息
来源：http://xok.cucudq.cn

ANALYZE TABLE users;
来源：http://tce.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://xya.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zzn.chenjidiqi.icu

[Q72] 查看索引
来源：http://cle.ehwqpu.com

SHOW INDEX FROM users;
来源：http://dgn.chenjidiqi.icu

[Q73] 查看表状态
来源：http://lvx.xingfuxueyuan.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://zpw.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://onv.shzxlz.cn


<!-- 参考信息 -->