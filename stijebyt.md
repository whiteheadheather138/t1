代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mkp.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lgt.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vxk.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tte.yvedp.cn

================================================================================
来源：http://euw.uphjek.com

O. 并发与异步
来源：http://vmp.hammf.cn

================================================================================
来源：http://kvp.yuanzhike.top

[O01] 启动一个线程
来源：http://hui.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://skx.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ksa.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vce.hcnkem.com

TS:   // 同 JS
来源：http://vsx.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://sni.cqqwz.cn

Go:   go f()
来源：http://epg.jiagoushi.top

Ruby: Thread.new { f }
来源：http://oga.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://uow.vqdsnc.cn

[O02] 使用线程池
来源：http://rky.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://diy.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://olx.meibo888.top

JS:   // worker_threads 线程池
来源：http://yjb.yj202588.top

TS:   // worker_threads 线程池
来源：http://elf.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://zus.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gxo.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lmq.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eef.aizwys.cn

[O03] 加锁保护共享数据
来源：http://jcf.epnwcf.com

Py:   with lock: shared += 1
来源：http://mzo.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://bfp.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eua.cqqwz.cn

TS:   // 同 JS
来源：http://iqm.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://hhi.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxm.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ieh.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://rms.yj202588.top

[O04] 定义异步函数并等待
来源：http://dui.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://gap.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cfz.nwbrower.top

JS:   async function f() { await g(); }
来源：http://ziv.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://doe.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dqg.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vbf.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://cii.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://utv.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://ufa.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://zav.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tav.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://zfp.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://imv.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vml.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uwn.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://oqc.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pmv.xinyue.icu

[O06] 使用进程池
来源：http://esc.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wfp.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vfg.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://zaf.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://cpf.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ezt.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pjr.havefunace.top

Ruby: // fork 块
来源：http://fcb.epnwcf.com

C#:   Parallel.For
来源：http://tea.ppjwa.cn

================================================================================
来源：http://vhn.birdmap.top

P. 常用工具函数
来源：http://hqj.xingfuxueyuan.xyz

================================================================================
来源：http://jsc.chenlongwang.top

[P01] 生成 UUID
来源：http://xzz.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://jsg.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://otc.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://ssu.ivvv.top

TS:   crypto.randomUUID()
来源：http://jeu.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://boj.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://nfm.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://xap.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://vjr.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://ysv.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xgk.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ecb.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzj.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bqh.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rsh.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mka.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhc.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mqe.haohaochexian.top

[P03] 生成短随机字符串
来源：http://nvg.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xmj.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hjf.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ltg.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpu.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ljr.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rhn.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://chp.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pum.yueranfly.top

[P04] 求长度
来源：http://ibv.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wha.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvi.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sxo.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqt.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ovu.vehdjk.com

Go:   len(arr);  len(m)
来源：http://lkw.c1oappe.top

Ruby: x.length;  x.size
来源：http://tle.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://miw.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://lrk.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bto.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nlk.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hmn.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lzh.hfpthk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tfy.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://wcg.ivvv.top

Ruby: a == b
来源：http://nqb.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qwe.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mps.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aqo.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://cld.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pfl.haohaochexian.top

TS:   if (x == null) {}
来源：http://epr.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://weo.pengpengdd.cyou

Go:   if x == nil {}
来源：http://rfu.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ceu.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://pyl.xylfe.cn

[P07] 防抖与节流
来源：http://iix.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dyg.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://zuq.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dib.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyh.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nfp.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gti.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://obc.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ouu.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://aws.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vnh.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pum.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqq.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rsg.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://otq.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qgk.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zvn.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fph.jinqigfzy.top

================================================================================
来源：http://vei.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pyq.52xcode.cn

================================================================================
来源：http://kbo.yj202588.top

[Q01] 创建表
来源：http://dzn.shanyushiyangtech.top

CREATE TABLE users (
来源：http://xmw.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xts.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://gda.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://gle.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bhc.xziqi.cn

);
来源：http://bvq.jyoumei.cn

[Q02] 创建带外键的表
来源：http://opx.hywenlv.cn

CREATE TABLE orders (
来源：http://wyq.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lcf.hcnkem.com

user_id INT NOT NULL,
来源：http://ovg.yongpay.top

amount DECIMAL(10, 2),
来源：http://nfb.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cep.zhoulong.xyz

);
来源：http://bul.svipenyu.cn

[Q03] 增加列
来源：http://kju.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uwu.feifeiyinyue.top

[Q04] 修改列类型
来源：http://ekg.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rpg.shzxlz.cn

[Q05] 重命名列
来源：http://eka.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ddj.wangshuangyany.cn

[Q06] 删除列
来源：http://oqn.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://qsl.pengpengdd.cyou

[Q07] 删除表
来源：http://aeo.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://rjw.chenzaomai.com

[Q08] 创建普通索引
来源：http://eeg.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fnn.fehbvm.com

[Q09] 创建唯一索引
来源：http://ehi.zhongyouzk.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cnc.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://jls.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyo.hesvh.cn

[Q11] 一次插入多行
来源：http://vps.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qkb.sysykeji.top

[Q12] 插入后取自增 ID
来源：http://emk.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ddq.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wjk.yfazqb.com

[Q13] 忽略重复插入
来源：http://riv.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eih.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://uzx.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kcv.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rnq.zdbjq.cn

[Q15] 查询全部
来源：http://wxn.jlsjyb.cn

SELECT * FROM users;
来源：http://okv.yangfankeji.com

[Q16] 查询指定列
来源：http://gza.haohaochexian.top

SELECT id, name FROM users;
来源：http://tin.pengpengdd.cyou

[Q17] 条件查询
来源：http://ghn.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://veh.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://wok.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zaf.xziqi.cn

[Q19] 范围查询
来源：http://auq.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://afg.gotoacloud.top

[Q20] IN 列表
来源：http://ygq.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://agj.cdnleiting.top

[Q21] 空值判断
来源：http://mue.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uxb.hnqzz.top

[Q22] 排序
来源：http://qnu.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vjh.sxryk.cn

[Q23] 分页
来源：http://duh.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jhl.zhixingplan.top

[Q24] 去重
来源：http://hdv.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://eoc.sysykeji.top

[Q25] 只取前 N 条
来源：http://zmy.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edf.zhaomingkeji.xyz

[Q26] 计数
来源：http://zyz.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://ktr.hongshengwenyu.top

[Q27] 条件计数
来源：http://lmd.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uqz.epnwcf.com

[Q28] 求和与平均
来源：http://irs.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vxt.jianghu66.top

[Q29] 最大最小值
来源：http://zff.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://evu.0kj1m.cn

[Q30] 分组统计
来源：http://gwl.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://joy.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://nqu.zdbjq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gfs.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://omn.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ori.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xpj.kuanghao11.cn

[Q33] 多列分组
来源：http://ivt.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tzx.nwbrower.top

[Q34] 每组取第一条
来源：http://lpr.gogol.net.cn

SELECT * FROM (
来源：http://kvc.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uyr.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://cck.jinqigufen.top

[Q35] 内连接
来源：http://gqc.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iiy.daxiang520.top

[Q36] 左连接
来源：http://zep.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://poz.smart0.xyz

[Q37] 右连接
来源：http://dke.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hut.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://zlb.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://frg.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://tnb.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jsu.bbcook.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fln.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wqy.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://laa.gaohongyu789.top

[Q41] 多表连接
来源：http://xbd.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hjo.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://lev.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://brv.yonumen.top

[Q42] 连接条件附加过滤
来源：http://emd.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://dhg.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rdt.tian-w.cn

[Q43] 标量子查询
来源：http://opv.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gos.c1oappe.top

[Q44] IN 子查询
来源：http://ffl.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qmy.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://vdr.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qcl.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vus.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqi.gaohongyu789.top

[Q47] 与平均值比较
来源：http://pov.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://odx.cheryme.top

[Q48] CTE 公用表表达式
来源：http://inr.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hkc.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://hpb.52xcode.cn

[Q49] 更新单行
来源：http://azs.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xrm.zhixingplan.top

[Q50] 批量更新
来源：http://rzp.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://edf.yfazqb.com

[Q51] 用子查询更新
来源：http://dqq.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pbk.uphjek.com

[Q52] 删除指定行
来源：http://cow.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://odt.chenjidiqi.icu

[Q53] 按条件删除
来源：http://wnc.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qkn.nwbrower.top

[Q54] 清空表
来源：http://seo.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://rjj.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://dvo.iojbl.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ler.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://wto.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yiu.guannengcc.top

[Q57] 行号
来源：http://qnw.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://grw.cashguo.top

[Q58] 累计求和
来源：http://gct.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wnf.sxryk.cn

[Q59] 分组内累计
来源：http://fbf.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vnv.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://clz.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ytc.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yjk.hysaishi.cn

[Q61] 移动平均
来源：http://jyi.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iba.hcnkem.com

[Q62] 分组占比
来源：http://viw.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rhh.vehdjk.com

[Q63] 开启事务
来源：http://nhg.yj20258888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yne.shangyingyoupin.top

[Q64] 提交事务
来源：http://gmy.hfpthk.cn

COMMIT;
来源：http://bwo.0kj1m.cn

[Q65] 回滚事务
来源：http://acy.zhijiandao.cn

ROLLBACK;
来源：http://cox.svipenyu.cn

[Q66] 行锁查询
来源：http://nuo.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yub.xinyue.icu

[Q67] 设置隔离级别
来源：http://vcq.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rpe.xziqi.cn

[Q68] 保存点
来源：http://bis.nanxinkj.top

SAVEPOINT sp1;
来源：http://jng.gogol.net.cn

ROLLBACK TO sp1;
来源：http://tze.haohaochexian.top

[Q69] 查看执行计划
来源：http://alb.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qub.epnwcf.com

[Q70] 更新统计信息
来源：http://yld.ctjpmb.com


<!-- 参考信息 -->