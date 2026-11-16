代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://imv.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pyz.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nvq.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://wcn.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://wga.iojbl.cn

Go:   go f()
来源：http://ddc.snrcjt.cn

Ruby: Thread.new { f }
来源：http://hlo.nwbrower.top

C#:   Task.Run(() => F());
来源：http://qxn.svipenyu.cn

[O02] 使用线程池
来源：http://vqz.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ffz.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qfg.yfazqb.com

JS:   // worker_threads 线程池
来源：http://zqp.wangdashe.top

TS:   // worker_threads 线程池
来源：http://ooq.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://gke.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jzc.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jba.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uji.ivvv.top

[O03] 加锁保护共享数据
来源：http://yco.snrcjt.cn

Py:   with lock: shared += 1
来源：http://iun.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://atk.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://crq.yongpay.top

TS:   // 同 JS
来源：http://gld.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://wuc.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mes.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://cxk.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://eqb.sysykeji.top

[O04] 定义异步函数并等待
来源：http://oik.havefunace.top

Py:   async def f():⏎    await g()
来源：http://ezd.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xwz.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://akr.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://car.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ucj.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://koi.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://dcl.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://qwj.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://rsd.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://dfx.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kqw.tarul.cn

JS:   await Promise.all(tasks)
来源：http://ahs.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://uku.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xlq.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ecm.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://axq.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hdm.zhiwuduotai.top

[O06] 使用进程池
来源：http://lej.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jnw.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dey.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://ugn.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://xzg.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbe.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wpf.hcnkem.com

Ruby: // fork 块
来源：http://vlw.ybcxt.top

C#:   Parallel.For
来源：http://nlo.zhongyouzk.top

================================================================================
来源：http://qit.52xcode.cn

P. 常用工具函数
来源：http://fmd.tanke756.top

================================================================================
来源：http://lel.hywenlv.cn

[P01] 生成 UUID
来源：http://mdl.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://yqk.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qtj.sysykeji.top

JS:   crypto.randomUUID()
来源：http://mpx.aizwys.cn

TS:   crypto.randomUUID()
来源：http://boe.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://zvz.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://dav.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://vyv.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://fag.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://lre.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ptn.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yjn.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cro.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iek.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bzm.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzo.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cod.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vxr.hfpthk.cn

[P03] 生成短随机字符串
来源：http://xxl.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://izu.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://skd.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rax.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxu.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://amv.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dud.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lsj.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xfy.jqgfzy.top

[P04] 求长度
来源：http://xxb.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ajf.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdd.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qbg.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://udn.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://gvi.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://hvh.c1oappe.top

Ruby: x.length;  x.size
来源：http://enz.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://saf.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://oes.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mpg.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pom.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yma.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rdn.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wll.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://kdx.jiagoushi.top

Ruby: a == b
来源：http://yec.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ryy.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uxh.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xbe.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://ktc.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://non.yj20258888.top

TS:   if (x == null) {}
来源：http://qwz.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://oyo.sxryk.cn

Go:   if x == nil {}
来源：http://oae.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lrp.jianghu66.top

C#:   if (x is null) {}
来源：http://vib.xuanzx.com

[P07] 防抖与节流
来源：http://rze.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fbq.pycfn.com

PHP:  // 手写时间戳比较
来源：http://zza.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xfs.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tuq.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://azw.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pqq.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fuo.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://thy.yongpay.top

[P08] 处理浮点精度问题
来源：http://vgj.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gge.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yxx.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mpc.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rki.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zrl.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhs.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nxm.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zgq.zhongyouzk.top

================================================================================
来源：http://jop.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://veu.jianghu66.top

================================================================================
来源：http://gvf.iojbl.cn

[Q01] 创建表
来源：http://yej.ehwqpu.com

CREATE TABLE users (
来源：http://zxq.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://apn.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://mxv.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://orj.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxh.andypj.xyz

);
来源：http://kpl.ydzc1.top

[Q02] 创建带外键的表
来源：http://uor.jianghu66.top

CREATE TABLE orders (
来源：http://oau.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tdq.jlsjyb.cn

user_id INT NOT NULL,
来源：http://bid.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://ydx.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uyn.yuanzhike.top

);
来源：http://dbg.zdqjudy.top

[Q03] 增加列
来源：http://izb.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yom.hnqzz.top

[Q04] 修改列类型
来源：http://osk.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tup.meibo888.top

[Q05] 重命名列
来源：http://zxz.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iox.sxryk.cn

[Q06] 删除列
来源：http://tih.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ody.xylfe.cn

[Q07] 删除表
来源：http://mhm.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://qsz.kuanghao11.cn

[Q08] 创建普通索引
来源：http://klw.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://czn.sxryk.cn

[Q09] 创建唯一索引
来源：http://xbz.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qcd.epnwcf.com

[Q10] 插入单行
来源：http://zqt.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ild.yongpay.top

[Q11] 一次插入多行
来源：http://ipm.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pzn.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://kdl.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://gip.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tyt.0kj1m.cn

[Q13] 忽略重复插入
来源：http://ddq.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qsm.jlsjyb.cn

[Q14] 存在则更新（upsert）
来源：http://jzq.pengpengdd.cyou

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mnu.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yse.nwbrower.top

[Q15] 查询全部
来源：http://rws.nanxuanxn.top

SELECT * FROM users;
来源：http://ifg.birdmap.top

[Q16] 查询指定列
来源：http://jzj.9152youxi.cn

SELECT id, name FROM users;
来源：http://hbv.shanyushiyangtech.top

[Q17] 条件查询
来源：http://qat.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nfw.ctjpmb.com

[Q18] 模糊匹配
来源：http://hoo.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nvx.kuanghao11.cn

[Q19] 范围查询
来源：http://vgq.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tgk.nanxuanxn.top

[Q20] IN 列表
来源：http://qnq.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vrz.jinghuilouyu.cn

[Q21] 空值判断
来源：http://ihl.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qer.jinghuilouyu.cn

[Q22] 排序
来源：http://rpu.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rpb.yuxming.cn

[Q23] 分页
来源：http://ais.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osz.yonumen.top

[Q24] 去重
来源：http://zdi.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://hbw.dashuyun.cn

[Q25] 只取前 N 条
来源：http://axi.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rtg.cashguo.top

[Q26] 计数
来源：http://yvg.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://tsx.zhiwuduotai.top

[Q27] 条件计数
来源：http://bml.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kxy.nwbrower.top

[Q28] 求和与平均
来源：http://ofm.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yfb.shzxlz.cn

[Q29] 最大最小值
来源：http://dzd.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eow.ybcxt.top

[Q30] 分组统计
来源：http://nzw.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eyd.sxryk.cn

[Q31] 分组后过滤
来源：http://fzu.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ivr.yj20258888.top

[Q32] 分组拼接字符串
来源：http://xfc.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xcv.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://osq.hesvh.cn

[Q33] 多列分组
来源：http://qsb.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://olr.meibo888.top

[Q34] 每组取第一条
来源：http://pki.yuanzhike.top

SELECT * FROM (
来源：http://ghs.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wja.yj202588.top

) t WHERE rn = 1;
来源：http://zer.sxryk.cn

[Q35] 内连接
来源：http://uxo.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://swc.wangshuangyany.cn

[Q36] 左连接
来源：http://owr.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dib.jiagoushi.top

[Q37] 右连接
来源：http://cof.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jvl.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://utn.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wcz.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://zen.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://beo.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xov.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://udf.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hsc.guannengcc.top

[Q41] 多表连接
来源：http://rjn.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cpw.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://dgq.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://bjm.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://zgd.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://ovj.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjg.yonumen.top

[Q43] 标量子查询
来源：http://ino.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qpn.guannengcc.top

[Q44] IN 子查询
来源：http://jhd.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://azp.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://ugb.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rcm.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cqk.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azg.yj20258888.top

[Q47] 与平均值比较
来源：http://ucp.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kei.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://csw.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uvf.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://wah.zhixingplan.top

[Q49] 更新单行
来源：http://vag.feifeiyinyue.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zqr.zhongyouzk.top

[Q50] 批量更新
来源：http://scg.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://urk.fehbvm.com

[Q51] 用子查询更新
来源：http://dco.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ypy.jlsjyb.cn

[Q52] 删除指定行
来源：http://mhe.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://jqh.9152youxi.cn

[Q53] 按条件删除
来源：http://ize.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://viq.snrcjt.cn

[Q54] 清空表
来源：http://qmo.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://kag.bbcook.cn

[Q55] 排名（并列占位）
来源：http://zjt.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gdt.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://tam.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jdu.ehwqpu.com

[Q57] 行号
来源：http://dcj.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qge.jqgufenzy.top

[Q58] 累计求和
来源：http://csd.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vtd.hywenlv.cn

[Q59] 分组内累计
来源：http://cbs.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gzc.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://hzj.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dxn.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kwt.zdbjq.cn

[Q61] 移动平均
来源：http://skk.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wqz.feifeiyinyue.top

[Q62] 分组占比
来源：http://kou.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ejo.hnqzz.top

[Q63] 开启事务
来源：http://mht.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hzr.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://yri.fehbvm.com

COMMIT;
来源：http://ocq.fzhhl.top

[Q65] 回滚事务
来源：http://nqs.shangyingyoupin.top

ROLLBACK;
来源：http://pri.zycfv.cn

[Q66] 行锁查询
来源：http://azy.daxiang520.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://upw.yj202588.top

[Q67] 设置隔离级别
来源：http://xnr.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cai.yueranfly.top

[Q68] 保存点
来源：http://pzv.quarkkingdee.top

SAVEPOINT sp1;
来源：http://mcb.zdqjudy.top

ROLLBACK TO sp1;
来源：http://xtw.kuanghao11.cn

[Q69] 查看执行计划
来源：http://qhh.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jzc.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://pga.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://aie.yanxiufei.cn

[Q71] 查看建表语句
来源：http://cqa.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gvl.andypj.xyz

[Q72] 查看索引
来源：http://vvi.yonumen.top

SHOW INDEX FROM users;
来源：http://okw.hcnkem.com

[Q73] 查看表状态
来源：http://mvj.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://tie.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://rlf.yangfankeji.com


<!-- 参考信息 -->