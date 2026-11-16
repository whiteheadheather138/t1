代发 wailian999

================================================================================
来源：http://kun.daxiang520.top

O. 并发与异步
来源：http://ivq.0kj1m.cn

================================================================================
来源：http://ccs.zhijiandao.cn

[O01] 启动一个线程
来源：http://upn.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dov.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ozm.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wek.yangfankeji.com

TS:   // 同 JS
来源：http://mvv.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://nim.haohaochexian.top

Go:   go f()
来源：http://bka.zdqjudy.top

Ruby: Thread.new { f }
来源：http://tea.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://cxe.chenjidiqi.icu

[O02] 使用线程池
来源：http://nbl.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zeg.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gkt.tanke756.top

JS:   // worker_threads 线程池
来源：http://sik.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://cyf.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://bnx.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjh.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nvo.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cfl.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://yop.sweek.top

Py:   with lock: shared += 1
来源：http://hni.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://jvi.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://slh.bbcook.cn

TS:   // 同 JS
来源：http://whd.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://dob.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gpb.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uyc.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://gjc.yvedp.cn

[O04] 定义异步函数并等待
来源：http://dje.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://dsz.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wkf.pycfn.com

JS:   async function f() { await g(); }
来源：http://djm.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qzy.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qdp.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgs.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zkt.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://mbq.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://gai.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://qvf.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qxe.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://ubr.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://xgx.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pwb.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://skp.316326.xyz

Ruby: threads.map(&:join)
来源：http://iny.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nvd.cheryme.top

[O06] 使用进程池
来源：http://zbp.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://doz.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bsa.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://gpy.hammf.cn

TS:   // child_process / cluster 模块
来源：http://jdj.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bwg.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kgy.yongpay.top

Ruby: // fork 块
来源：http://xnu.zhixingplan.top

C#:   Parallel.For
来源：http://lrd.shanyushiyangtech.top

================================================================================
来源：http://ebu.gogol.net.cn

P. 常用工具函数
来源：http://kwq.ivvv.top

================================================================================
来源：http://xhu.sweek.top

[P01] 生成 UUID
来源：http://nyp.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://lvs.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hur.tian-w.cn

JS:   crypto.randomUUID()
来源：http://jlg.ydzc1.top

TS:   crypto.randomUUID()
来源：http://qif.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://yqp.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://mby.hammf.cn

Ruby: SecureRandom.uuid
来源：http://xvt.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://maz.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://odp.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://awy.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://aoy.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rsd.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fut.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://isu.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ivl.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hkj.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mrw.cheryme.top

[P03] 生成短随机字符串
来源：http://zpl.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jlq.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kwz.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cge.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qap.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nss.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvi.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://jzi.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ibb.52xcode.cn

[P04] 求长度
来源：http://oeh.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ecr.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jei.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyp.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lyz.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://mmr.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://bcm.fengsongda.top

Ruby: x.length;  x.size
来源：http://mxa.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://unt.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://klg.nanxinkj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yhb.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ykc.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rhr.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://snu.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ten.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://chg.chenlongwang.top

Ruby: a == b
来源：http://ajl.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hzu.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oqn.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gtx.cheryme.top

PHP:  if (empty($x)) {}
来源：http://tfp.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ppm.zycfv.cn

TS:   if (x == null) {}
来源：http://fca.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qqp.haohaochexian.top

Go:   if x == nil {}
来源：http://dcb.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yii.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://fpx.daria6918.cn

[P07] 防抖与节流
来源：http://ikh.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qit.yj20258.top

PHP:  // 手写时间戳比较
来源：http://ebm.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zij.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yle.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qht.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsw.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cca.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wwp.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://jid.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nkn.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lig.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://did.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wtq.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://npr.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fga.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ohp.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uqh.yanxiufei.cn

================================================================================
来源：http://seq.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lxd.gaohongyu789.top

================================================================================
来源：http://xuj.hcnkem.com

[Q01] 创建表
来源：http://sqb.iojbl.cn

CREATE TABLE users (
来源：http://hdc.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohg.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://klg.uphjek.com

email VARCHAR(100) UNIQUE,
来源：http://hlv.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ltj.hnxiangtu.top

);
来源：http://gdl.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://yli.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://npp.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mks.fehbvm.com

user_id INT NOT NULL,
来源：http://osa.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://csz.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dyh.chenjidiqi.icu

);
来源：http://ydj.0kj1m.cn

[Q03] 增加列
来源：http://enj.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vgk.shzxlz.cn

[Q04] 修改列类型
来源：http://rqp.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://juv.daxiang520.top

[Q05] 重命名列
来源：http://hdf.xylfe.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wsq.cucudq.cn

[Q06] 删除列
来源：http://bog.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://cii.guannengcc.top

[Q07] 删除表
来源：http://eqo.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://cgp.jqgfzy.top

[Q08] 创建普通索引
来源：http://xzn.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vhw.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://okw.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://prm.svipenyu.cn

[Q10] 插入单行
来源：http://tkx.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hmr.yongpay.top

[Q11] 一次插入多行
来源：http://wqa.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dkb.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://kzo.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dhj.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rah.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://qjd.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gvq.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://vrn.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcq.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bfb.xuanzx.com

[Q15] 查询全部
来源：http://qdx.0kj1m.cn

SELECT * FROM users;
来源：http://gag.tarul.cn

[Q16] 查询指定列
来源：http://xja.316326.xyz

SELECT id, name FROM users;
来源：http://zgi.quarkkingdee.top

[Q17] 条件查询
来源：http://pyw.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ahp.pycfn.com

[Q18] 模糊匹配
来源：http://mfp.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zql.nanxuanxn.top

[Q19] 范围查询
来源：http://ptg.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iuo.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://lhj.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wxt.fzhhl.top

[Q21] 空值判断
来源：http://kyd.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sla.bbcook.cn

[Q22] 排序
来源：http://vtq.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggi.52xcode.cn

[Q23] 分页
来源：http://ong.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://opm.hywenlv.cn

[Q24] 去重
来源：http://zbd.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://uau.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://tqp.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://djk.sxryk.cn

[Q26] 计数
来源：http://iqs.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://puw.smart0.xyz

[Q27] 条件计数
来源：http://zxm.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hni.ivvv.top

[Q28] 求和与平均
来源：http://squ.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mjr.bbcook.cn

[Q29] 最大最小值
来源：http://qfc.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dlj.yj20258.top

[Q30] 分组统计
来源：http://xmd.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dgt.smart0.xyz

[Q31] 分组后过滤
来源：http://kdn.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zdr.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://rdm.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mil.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dec.shzxlz.cn

[Q33] 多列分组
来源：http://gqe.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qxb.tanke756.top

[Q34] 每组取第一条
来源：http://tmi.ywan-chungtsiang.top

SELECT * FROM (
来源：http://hey.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tdq.yongpay.top

) t WHERE rn = 1;
来源：http://xkt.hnqzz.top

[Q35] 内连接
来源：http://irw.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mqb.xylfe.cn

[Q36] 左连接
来源：http://kxa.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eho.9152youxi.cn

[Q37] 右连接
来源：http://ibl.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vzu.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://wfk.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bud.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://bkc.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vcz.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kfk.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mwi.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://viz.shanyushiyangtech.top

[Q41] 多表连接
来源：http://pnw.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gyi.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://fpy.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://bgv.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://szd.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://fcu.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xnl.yj202588.top

[Q43] 标量子查询
来源：http://nfo.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cem.sweek.top

[Q44] IN 子查询
来源：http://gqc.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nbe.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://atf.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nxo.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://gra.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ses.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://vri.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://msr.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://yjb.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bpl.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://ogh.yj20258888.top

[Q49] 更新单行
来源：http://iqy.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oxl.yangfankeji.com

[Q50] 批量更新
来源：http://loc.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://awz.hnqzz.top

[Q51] 用子查询更新
来源：http://jyy.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ltx.cucudq.cn

[Q52] 删除指定行
来源：http://kup.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://nmr.ydjk.org.cn

[Q53] 按条件删除
来源：http://ycb.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gss.vqdsnc.cn

[Q54] 清空表
来源：http://uni.epnwcf.com

TRUNCATE TABLE logs;
来源：http://mwu.fktsv.cn

[Q55] 排名（并列占位）
来源：http://eac.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ete.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://wdv.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yjc.yongpay.top

[Q57] 行号
来源：http://lav.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bux.tanke756.top

[Q58] 累计求和
来源：http://rsv.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jgn.hongshengwenyu.top

[Q59] 分组内累计
来源：http://czc.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://opb.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://hai.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zdr.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dmv.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://lcb.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zjh.guowangkeji.top

[Q62] 分组占比
来源：http://ort.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gxd.snrcjt.cn

[Q63] 开启事务
来源：http://uue.havefunace.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eju.chenlongwang.top

[Q64] 提交事务
来源：http://uvz.wangdashe.top

COMMIT;
来源：http://pxw.yfazqb.com

[Q65] 回滚事务
来源：http://xck.pycfn.com

ROLLBACK;
来源：http://mav.jqgufenzy.top

[Q66] 行锁查询
来源：http://nyi.vqdsnc.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iia.xinyue.icu

[Q67] 设置隔离级别
来源：http://exy.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zxq.yueranfly.top

[Q68] 保存点
来源：http://zis.chenzaomai.com

SAVEPOINT sp1;
来源：http://jms.yvedp.cn

ROLLBACK TO sp1;
来源：http://jtt.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://awf.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rxw.yfazqb.com

[Q70] 更新统计信息
来源：http://rut.xylfe.cn

ANALYZE TABLE users;
来源：http://lgl.ivvv.top

[Q71] 查看建表语句
来源：http://jrf.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mhs.hesvh.cn

[Q72] 查看索引
来源：http://ivz.andypj.xyz


<!-- 参考信息 -->