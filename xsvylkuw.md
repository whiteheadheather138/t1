代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pnk.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gyq.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yct.ydzc1.top

TS:   // 同 JS
来源：http://dkn.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://uxz.yuanzhike.top

Go:   go f()
来源：http://ltt.aibaodan.cn

Ruby: Thread.new { f }
来源：http://rls.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://fsz.kuanghao11.cn

[O02] 使用线程池
来源：http://ehb.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zvv.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xjw.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://mlr.ydzc1.top

TS:   // worker_threads 线程池
来源：http://itz.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://qvo.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wgv.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kpw.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xpq.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://sax.sufxvd.cn

Py:   with lock: shared += 1
来源：http://pht.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://wez.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ugn.gotoacloud.top

TS:   // 同 JS
来源：http://ybr.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://trh.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ohx.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nhf.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://suj.316326.xyz

[O04] 定义异步函数并等待
来源：http://obc.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://xlc.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ddd.xinyue.icu

JS:   async function f() { await g(); }
来源：http://pap.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://efx.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ocj.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yuy.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ngi.meibo888.top

C#:   async Task F() { await G(); }
来源：http://htm.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://hyu.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://pkj.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fwe.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://cqx.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://frc.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dax.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pji.52xcode.cn

Ruby: threads.map(&:join)
来源：http://aze.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://nrq.yangfankeji.com

[O06] 使用进程池
来源：http://lhl.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ejc.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://kaa.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://tjy.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://uuw.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jtq.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tqw.yangfankeji.com

Ruby: // fork 块
来源：http://ceq.uphjek.com

C#:   Parallel.For
来源：http://ehy.nwbrower.top

================================================================================
来源：http://yss.gzhubu.top

P. 常用工具函数
来源：http://yqs.ydzc1.top

================================================================================
来源：http://tpo.fengsongda.top

[P01] 生成 UUID
来源：http://ybz.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://yqp.shzxlz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gff.meibo888.top

JS:   crypto.randomUUID()
来源：http://jtw.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://exi.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://lrb.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://heb.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://jqz.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://czw.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://ltc.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bzu.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://chg.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kkd.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wiu.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qsl.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xhq.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rgv.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wzo.hywenlv.cn

[P03] 生成短随机字符串
来源：http://lch.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jut.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ihi.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qzj.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bod.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tta.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fki.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kgz.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://alr.sysykeji.top

[P04] 求长度
来源：http://rlc.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cgy.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvj.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jxj.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kzy.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://bnz.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://xla.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://ksa.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://qwe.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://sup.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://brm.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://djz.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qkn.xziqi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tvb.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tlo.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://nhr.nwbrower.top

Ruby: a == b
来源：http://dqq.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gpp.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yoo.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nha.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://njm.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://skk.zdbjq.cn

TS:   if (x == null) {}
来源：http://xyb.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kea.gaohongyu789.top

Go:   if x == nil {}
来源：http://qzy.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pov.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://pwb.sysykeji.top

[P07] 防抖与节流
来源：http://qrv.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mnl.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://dic.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ilo.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://era.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://utf.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xpo.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uwf.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tio.cucudq.cn

[P08] 处理浮点精度问题
来源：http://taa.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xgv.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yxz.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rec.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ghq.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bez.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lpi.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://onc.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qbd.chenlongwang.top

================================================================================
来源：http://rxr.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvk.hnxiangtu.top

================================================================================
来源：http://kry.quarkkingdee.top

[Q01] 创建表
来源：http://fkt.shzxlz.cn

CREATE TABLE users (
来源：http://xau.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fno.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://sey.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://rvq.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jwv.vqdsnc.cn

);
来源：http://oso.hesvh.cn

[Q02] 创建带外键的表
来源：http://jna.guowangkeji.top

CREATE TABLE orders (
来源：http://xka.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zik.chenlongwang.top

user_id INT NOT NULL,
来源：http://prz.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://gdr.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fzj.xinyue.icu

);
来源：http://xzu.jinqigfzy.top

[Q03] 增加列
来源：http://hnb.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yre.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://txl.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xkl.aibaodan.cn

[Q05] 重命名列
来源：http://jwf.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nav.daxiang520.top

[Q06] 删除列
来源：http://itf.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://bmf.gzhubu.top

[Q07] 删除表
来源：http://hgt.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://dpl.zhixingplan.top

[Q08] 创建普通索引
来源：http://rpi.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dox.tianlin.xyz

[Q09] 创建唯一索引
来源：http://qrn.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msb.sysykeji.top

[Q10] 插入单行
来源：http://bdm.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://opn.haohaochexian.top

[Q11] 一次插入多行
来源：http://tlu.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://haj.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://lkh.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://avf.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://asg.tarul.cn

[Q13] 忽略重复插入
来源：http://szt.xylfe.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hjh.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://uye.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nvx.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://btx.daxiang520.top

[Q15] 查询全部
来源：http://avn.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://zrz.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://mxi.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://ifz.meibo888.top

[Q17] 条件查询
来源：http://jjn.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fid.guowangkeji.top

[Q18] 模糊匹配
来源：http://rvs.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zhl.yangfankeji.com

[Q19] 范围查询
来源：http://vjy.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gvg.xinyue.icu

[Q20] IN 列表
来源：http://vsj.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://imr.xylfe.cn

[Q21] 空值判断
来源：http://qso.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rfj.yj20258.top

[Q22] 排序
来源：http://bbh.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lgm.yuxming.cn

[Q23] 分页
来源：http://wvb.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzh.zhiwuduotai.top

[Q24] 去重
来源：http://rei.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://wjl.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://mgc.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ikl.fehbvm.com

[Q26] 计数
来源：http://bhn.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://bnq.0kj1m.cn

[Q27] 条件计数
来源：http://kjh.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://quj.zdqjudy.top

[Q28] 求和与平均
来源：http://wii.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ngu.mhx1999.top

[Q29] 最大最小值
来源：http://kic.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://edc.meibo888.top

[Q30] 分组统计
来源：http://xgq.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uab.ydzc1.top

[Q31] 分组后过滤
来源：http://pxx.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zip.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://jte.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wtd.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://efi.guowangkeji.top

[Q33] 多列分组
来源：http://bjz.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zwf.vehdjk.com

[Q34] 每组取第一条
来源：http://kvz.jianghu66.top

SELECT * FROM (
来源：http://uod.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tyj.hfpthk.cn

) t WHERE rn = 1;
来源：http://fxt.daria6918.cn

[Q35] 内连接
来源：http://vnb.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kyd.zhixingplan.top

[Q36] 左连接
来源：http://hrg.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ucb.yuanzhike.top

[Q37] 右连接
来源：http://bnj.shzxlz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tgg.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://glf.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://utl.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://dor.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://msd.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ubq.jqgufenzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rzz.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://smf.fengsongda.top

[Q41] 多表连接
来源：http://tow.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uca.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://rom.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://eos.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://gub.xinyue.icu

SELECT u.name, o.amount FROM users u
来源：http://ylu.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ebq.yonumen.top

[Q43] 标量子查询
来源：http://qdp.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nwf.jyoumei.cn

[Q44] IN 子查询
来源：http://htv.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dst.yj202588.top

[Q45] EXISTS 判断存在
来源：http://vrf.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqc.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://wfo.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rik.guowangkeji.top

[Q47] 与平均值比较
来源：http://khg.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nei.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://gow.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kpe.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://yul.svipenyu.cn

[Q49] 更新单行
来源：http://hoz.jianghu66.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ygs.xylfe.cn

[Q50] 批量更新
来源：http://rdb.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cbz.hnqzz.top

[Q51] 用子查询更新
来源：http://xez.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jxz.hnxiangtu.top

[Q52] 删除指定行
来源：http://tju.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://ebg.ivvv.top

[Q53] 按条件删除
来源：http://agt.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://guq.ivvv.top

[Q54] 清空表
来源：http://wsa.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://hql.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://jkq.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://alk.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://lpd.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rxe.zdbjq.cn

[Q57] 行号
来源：http://kvi.sxryk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://imq.mhx1999.top

[Q58] 累计求和
来源：http://itj.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kpa.daria6918.cn

[Q59] 分组内累计
来源：http://dto.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fkw.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://sme.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qjv.shzxlz.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gbx.nwbrower.top

[Q61] 移动平均
来源：http://qke.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gvk.pycfn.com

[Q62] 分组占比
来源：http://jjw.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://upk.yj20258.top

[Q63] 开启事务
来源：http://bza.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ycg.yj20258888.top

[Q64] 提交事务
来源：http://szv.yuxming.cn

COMMIT;
来源：http://bmp.yueranfly.top

[Q65] 回滚事务
来源：http://bfq.yfazqb.com

ROLLBACK;
来源：http://icm.xylfe.cn

[Q66] 行锁查询
来源：http://pnc.ydjk.org.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vjp.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://bwz.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rcg.zycfv.cn

[Q68] 保存点
来源：http://dbw.mhx1999.top

SAVEPOINT sp1;
来源：http://sav.fzhhl.top

ROLLBACK TO sp1;
来源：http://uqh.jyoumei.cn

[Q69] 查看执行计划
来源：http://bqj.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nud.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://ifp.svipenyu.cn

ANALYZE TABLE users;
来源：http://sqk.zhijiandao.cn

[Q71] 查看建表语句
来源：http://tvl.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ogq.epnwcf.com

[Q72] 查看索引
来源：http://rfm.bbcook.cn

SHOW INDEX FROM users;
来源：http://qut.wangdashe.top

[Q73] 查看表状态
来源：http://bng.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://evg.dashuyun.cn

[Q74] 强制使用索引
来源：http://tbm.fanxiaobao.xyz


<!-- 参考信息 -->