代发 wailian999

================================================================================
来源：http://dph.c1oappe.top

O. 并发与异步
来源：http://nyh.zycfv.cn

================================================================================
来源：http://fne.yonumen.top

[O01] 启动一个线程
来源：http://iwm.yangfankeji.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cyy.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qti.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://los.sxryk.cn

TS:   // 同 JS
来源：http://vke.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://txf.aizwys.cn

Go:   go f()
来源：http://lid.c1oappe.top

Ruby: Thread.new { f }
来源：http://eyu.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://qsj.guowangkeji.top

[O02] 使用线程池
来源：http://avr.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ofu.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hbh.nwbrower.top

JS:   // worker_threads 线程池
来源：http://fuu.316326.xyz

TS:   // worker_threads 线程池
来源：http://cto.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uqh.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mhn.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ode.yj20258888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jep.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://upj.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://zwb.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://lhz.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fbs.yanxiufei.cn

TS:   // 同 JS
来源：http://cdk.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://jip.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jii.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://can.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://cij.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://zui.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://ibd.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iet.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://cre.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tzy.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wsn.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://scn.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aqy.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://utt.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://iek.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://dlk.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpa.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://yyu.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://wit.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tsm.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cza.cucudq.cn

Ruby: threads.map(&:join)
来源：http://bep.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ici.daxiang520.top

[O06] 使用进程池
来源：http://oqp.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ouk.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ktr.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://xfj.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://gro.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ymy.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sda.guannengcc.top

Ruby: // fork 块
来源：http://zix.zhengqikj.top

C#:   Parallel.For
来源：http://sbp.c1oappe.top

================================================================================
来源：http://jkr.ydjk.org.cn

P. 常用工具函数
来源：http://myz.yfazqb.com

================================================================================
来源：http://erg.gogol.net.cn

[P01] 生成 UUID
来源：http://cuz.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://gyb.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hvj.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://goy.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://vss.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://qwl.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://eav.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://mtt.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://ykl.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://zsi.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xus.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zho.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ygg.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hji.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gfs.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nmm.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nsz.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lvg.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://bcu.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qpp.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://grp.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dma.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aee.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qdn.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zdw.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://evf.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mqt.gogol.net.cn

[P04] 求长度
来源：http://ltb.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jro.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exu.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://boi.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppf.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://aog.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://zgw.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://rqm.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zad.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://krj.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ncd.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zoj.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ola.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ful.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zza.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zhx.tianlin.xyz

Ruby: a == b
来源：http://est.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wdk.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hmd.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spb.yj202588.top

PHP:  if (empty($x)) {}
来源：http://zmn.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://upg.yongpay.top

TS:   if (x == null) {}
来源：http://prv.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gxj.yueranfly.top

Go:   if x == nil {}
来源：http://nns.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lml.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://yuo.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://vzv.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xra.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://djc.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jub.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpm.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tcv.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bzn.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://att.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iao.aizwys.cn

[P08] 处理浮点精度问题
来源：http://uqy.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iiq.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sou.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://scf.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hsm.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xnb.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ral.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wak.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nud.ydzc1.top

================================================================================
来源：http://auc.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bzg.sysykeji.top

================================================================================
来源：http://bvh.hywenlv.cn

[Q01] 创建表
来源：http://zoi.xinyue.icu

CREATE TABLE users (
来源：http://ope.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://key.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://uxb.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://fpa.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jby.hongshengwenyu.top

);
来源：http://fne.tanke756.top

[Q02] 创建带外键的表
来源：http://aln.fengsongda.top

CREATE TABLE orders (
来源：http://duu.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdm.sufxvd.cn

user_id INT NOT NULL,
来源：http://quu.quarkkingdee.top

amount DECIMAL(10, 2),
来源：http://lzb.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://seo.aibaodan.cn

);
来源：http://pki.shanyushiyangtech.top

[Q03] 增加列
来源：http://pnk.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yeg.sweek.top

[Q04] 修改列类型
来源：http://gsr.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sxh.zdqjudy.top

[Q05] 重命名列
来源：http://zrr.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cak.ivvv.top

[Q06] 删除列
来源：http://rfz.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://ene.zhaomingkeji.xyz

[Q07] 删除表
来源：http://imx.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://wat.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://yfj.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dnr.pycfn.com

[Q09] 创建唯一索引
来源：http://buf.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hoj.snrcjt.cn

[Q10] 插入单行
来源：http://gxb.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ipr.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://fca.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lsg.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://zoq.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://hee.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ivn.yvedp.cn

[Q13] 忽略重复插入
来源：http://bnq.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxf.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://emy.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ntd.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lgk.quarkkingdee.top

[Q15] 查询全部
来源：http://afr.xziqi.cn

SELECT * FROM users;
来源：http://whq.uphjek.com

[Q16] 查询指定列
来源：http://erq.yueranfly.top

SELECT id, name FROM users;
来源：http://ddf.c1oappe.top

[Q17] 条件查询
来源：http://tro.yvedp.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cwl.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://jha.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ykr.sufxvd.cn

[Q19] 范围查询
来源：http://zys.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jmr.aibaodan.cn

[Q20] IN 列表
来源：http://fcm.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kou.xuetiantiany.cn

[Q21] 空值判断
来源：http://ahm.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ube.iojbl.cn

[Q22] 排序
来源：http://szc.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sth.fengsongda.top

[Q23] 分页
来源：http://rgh.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qjy.sweek.top

[Q24] 去重
来源：http://dzh.jinghuilouyu.cn

SELECT DISTINCT city FROM users;
来源：http://kzz.haohaochexian.top

[Q25] 只取前 N 条
来源：http://rvm.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mje.zhixingplan.top

[Q26] 计数
来源：http://fae.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://sxo.zycfv.cn

[Q27] 条件计数
来源：http://scz.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nqj.daria6918.cn

[Q28] 求和与平均
来源：http://njd.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jmc.andypj.xyz

[Q29] 最大最小值
来源：http://raz.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://miw.tarul.cn

[Q30] 分组统计
来源：http://kng.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aiw.sxryk.cn

[Q31] 分组后过滤
来源：http://dqb.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xlz.fengsongda.top

[Q32] 分组拼接字符串
来源：http://bjc.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tsx.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zir.cashguo.top

[Q33] 多列分组
来源：http://bac.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zui.svipenyu.cn

[Q34] 每组取第一条
来源：http://anh.hysaishi.cn

SELECT * FROM (
来源：http://gyd.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cyl.hnqzz.top

) t WHERE rn = 1;
来源：http://pdg.hfpthk.cn

[Q35] 内连接
来源：http://fzi.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rmv.ctjpmb.com

[Q36] 左连接
来源：http://muo.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fox.zhiwuduotai.top

[Q37] 右连接
来源：http://gfl.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oez.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://ymz.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pou.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://hdf.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://qzz.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://acm.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://yba.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://owx.sufxvd.cn

[Q41] 多表连接
来源：http://spn.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nie.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://hub.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://wht.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://ica.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://jjw.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lwm.bjfxy.top

[Q43] 标量子查询
来源：http://hox.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xse.gzhubu.top

[Q44] IN 子查询
来源：http://qgm.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jku.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://etb.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uyg.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://usl.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kuf.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://okv.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bti.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://erx.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xws.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://unw.fktsv.cn

[Q49] 更新单行
来源：http://ksj.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://poa.jianghu66.top

[Q50] 批量更新
来源：http://kpm.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uel.redwolf501.top

[Q51] 用子查询更新
来源：http://hxd.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jti.yonumen.top

[Q52] 删除指定行
来源：http://byh.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://piy.daxiang520.top

[Q53] 按条件删除
来源：http://bvu.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://skg.yangfankeji.com

[Q54] 清空表
来源：http://iqc.yj202588.top

TRUNCATE TABLE logs;
来源：http://ufl.hammf.cn

[Q55] 排名（并列占位）
来源：http://flu.redwolf501.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://btx.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://jww.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://okt.hcnkem.com

[Q57] 行号
来源：http://kci.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lgz.haohaochexian.top

[Q58] 累计求和
来源：http://dai.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pvr.c1oappe.top

[Q59] 分组内累计
来源：http://ibd.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rkp.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://qba.guannengcc.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cye.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibn.aibaodan.cn

[Q61] 移动平均
来源：http://haw.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qrq.aibaodan.cn

[Q62] 分组占比
来源：http://jym.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xkh.guannengcc.top

[Q63] 开启事务
来源：http://kpz.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tqd.cucudq.cn

[Q64] 提交事务
来源：http://gbv.tarul.cn

COMMIT;
来源：http://lrv.xinyue.icu

[Q65] 回滚事务
来源：http://buu.yfazqb.com

ROLLBACK;
来源：http://ile.tianlin.xyz

[Q66] 行锁查询
来源：http://pti.gaohongyu789.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dwr.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://vjm.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tlq.jyoumei.cn

[Q68] 保存点
来源：http://kpb.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://adz.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://eph.zhengqikj.top

[Q69] 查看执行计划
来源：http://ywr.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iuw.fehbvm.com

[Q70] 更新统计信息
来源：http://eyz.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://wel.ppjwa.cn

[Q71] 查看建表语句
来源：http://zaj.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rnf.daxiang520.top

[Q72] 查看索引
来源：http://nlk.zhiwuduotai.top


<!-- 参考信息 -->