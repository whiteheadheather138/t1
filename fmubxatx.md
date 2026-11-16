代发 wailian999

[O02] 使用线程池
来源：http://qel.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ovj.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jpz.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://ehm.c1oappe.top

TS:   // worker_threads 线程池
来源：http://kqy.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hwh.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pzg.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bdz.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ubf.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://iod.tanke756.top

Py:   with lock: shared += 1
来源：http://euk.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://dwx.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vqy.zhongyouzk.top

TS:   // 同 JS
来源：http://dch.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://fhy.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myv.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ukn.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://vqi.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://ngi.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://tuz.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://glu.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://tfo.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jib.zhijiandao.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gbo.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yfl.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://reg.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://oja.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://ctj.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://sfy.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kyg.cashguo.top

JS:   await Promise.all(tasks)
来源：http://nay.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://cyh.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lap.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pkf.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://vfd.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ces.guowangkeji.top

[O06] 使用进程池
来源：http://odc.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rbn.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xrp.meibo888.top

JS:   // child_process / cluster 模块
来源：http://nfq.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://paq.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vfk.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xbq.xinyue.icu

Ruby: // fork 块
来源：http://csg.fzhhl.top

C#:   Parallel.For
来源：http://phg.vqdsnc.cn

================================================================================
来源：http://gjm.yvedp.cn

P. 常用工具函数
来源：http://blt.daria6918.cn

================================================================================
来源：http://zgb.zhiwuduotai.top

[P01] 生成 UUID
来源：http://pcg.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://nyx.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rar.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://qbv.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://ezw.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://dhl.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://hpv.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://tts.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://yql.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://mpg.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wlr.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eun.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agn.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xhi.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://orl.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jja.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nht.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ylz.yuanzhike.top

[P03] 生成短随机字符串
来源：http://ytk.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zyh.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kcx.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rgj.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wnx.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdi.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yje.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lyo.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ryw.yuxming.cn

[P04] 求长度
来源：http://mop.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lny.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://idm.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffs.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cic.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://cdo.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://fqz.hysaishi.cn

Ruby: x.length;  x.size
来源：http://cmm.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qsm.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://oat.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lhf.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ult.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rce.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ewk.yanxiufei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qxf.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://qrq.vehdjk.com

Ruby: a == b
来源：http://atm.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wgk.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cuu.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://osv.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://qxt.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jxj.hfpthk.cn

TS:   if (x == null) {}
来源：http://iyh.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bnh.zdbjq.cn

Go:   if x == nil {}
来源：http://bwb.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qhi.jianghu66.top

C#:   if (x is null) {}
来源：http://bde.zhoulong.xyz

[P07] 防抖与节流
来源：http://ywm.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpb.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://cya.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgf.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ccc.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cmb.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lih.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dnu.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ups.xylfe.cn

[P08] 处理浮点精度问题
来源：http://xvk.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ctb.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pge.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cnz.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://reg.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qhn.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zuc.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xne.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pvu.zhongyouzk.top

================================================================================
来源：http://jir.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bvm.nwbrower.top

================================================================================
来源：http://hgd.0kj1m.cn

[Q01] 创建表
来源：http://jso.sysykeji.top

CREATE TABLE users (
来源：http://uvy.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gwb.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://qwx.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://jgt.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dut.bbcook.cn

);
来源：http://uic.hywenlv.cn

[Q02] 创建带外键的表
来源：http://eto.ybcxt.top

CREATE TABLE orders (
来源：http://vlx.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://enh.xziqi.cn

user_id INT NOT NULL,
来源：http://ldb.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://fkm.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sfj.aizwys.cn

);
来源：http://sov.nanxuanxn.top

[Q03] 增加列
来源：http://wdn.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kab.aizwys.cn

[Q04] 修改列类型
来源：http://yrg.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tww.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://nan.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mkf.gogol.net.cn

[Q06] 删除列
来源：http://duj.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eti.ywan-chungtsiang.top

[Q07] 删除表
来源：http://jtj.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://mfy.jinqigufen.top

[Q08] 创建普通索引
来源：http://rhx.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mjm.xziqi.cn

[Q09] 创建唯一索引
来源：http://mgo.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bdu.ydjk.org.cn

[Q10] 插入单行
来源：http://ihu.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://usz.nwbrower.top

[Q11] 一次插入多行
来源：http://nhl.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yfb.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://ych.cdnleiting.top

INSERT INTO users (name) VALUES ('C');
来源：http://mnk.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rwq.pycfn.com

[Q13] 忽略重复插入
来源：http://fgj.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tih.wangshuangyany.cn

[Q14] 存在则更新（upsert）
来源：http://pjz.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgt.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lpc.zhiwuduotai.top

[Q15] 查询全部
来源：http://btv.ydzc1.top

SELECT * FROM users;
来源：http://acx.fktsv.cn

[Q16] 查询指定列
来源：http://hyl.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://qzk.tian-w.cn

[Q17] 条件查询
来源：http://fjg.guowangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vww.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://njy.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uxu.tarul.cn

[Q19] 范围查询
来源：http://mvv.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zxp.sysykeji.top

[Q20] IN 列表
来源：http://kza.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uqy.nwbrower.top

[Q21] 空值判断
来源：http://inv.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vyz.tianlin.xyz

[Q22] 排序
来源：http://pbx.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ukq.jlsjyb.cn

[Q23] 分页
来源：http://xyc.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oii.bjfxy.top

[Q24] 去重
来源：http://bxf.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://pki.hfpthk.cn

[Q25] 只取前 N 条
来源：http://mcw.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vai.bjfxy.top

[Q26] 计数
来源：http://tzi.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://qdc.zycfv.cn

[Q27] 条件计数
来源：http://mhm.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qhd.sweek.top

[Q28] 求和与平均
来源：http://vep.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mln.hfpthk.cn

[Q29] 最大最小值
来源：http://irm.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cha.gogol.net.cn

[Q30] 分组统计
来源：http://isw.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xhy.yfazqb.com

[Q31] 分组后过滤
来源：http://swz.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hie.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://zcm.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://otg.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ycz.tianlin.xyz

[Q33] 多列分组
来源：http://xyk.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zev.nanxinkj.top

[Q34] 每组取第一条
来源：http://ezi.xziqi.cn

SELECT * FROM (
来源：http://ewe.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ubi.fzhhl.top

) t WHERE rn = 1;
来源：http://zgw.feifeiyinyue.top

[Q35] 内连接
来源：http://tof.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sby.shanyushiyangtech.top

[Q36] 左连接
来源：http://pcv.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fat.hongshengwenyu.top

[Q37] 右连接
来源：http://ucu.ybcxt.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nqj.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sab.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yll.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://ibh.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://nem.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ohn.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xvo.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eds.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://fyd.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ziq.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://jyr.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://bix.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://bzc.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://rsk.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sjy.pycfn.com

[Q43] 标量子查询
来源：http://pqv.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iel.shangyingyoupin.top

[Q44] IN 子查询
来源：http://oyp.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dgh.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://uyi.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sio.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://ptl.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kbm.ydjk.org.cn

[Q47] 与平均值比较
来源：http://fgj.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://day.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://osg.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bkj.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://qcf.yueranfly.top

[Q49] 更新单行
来源：http://mev.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://njc.fehbvm.com

[Q50] 批量更新
来源：http://dlu.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ccr.snrcjt.cn

[Q51] 用子查询更新
来源：http://tlv.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgc.bbcook.cn

[Q52] 删除指定行
来源：http://rct.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://evt.yj20258888.top

[Q53] 按条件删除
来源：http://rzg.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://umk.ywan-chungtsiang.top

[Q54] 清空表
来源：http://uub.hesvh.cn

TRUNCATE TABLE logs;
来源：http://sgz.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://sjj.daxiang520.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iqs.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://ytd.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hoz.pycfn.com

[Q57] 行号
来源：http://otm.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gcd.cucudq.cn

[Q58] 累计求和
来源：http://zxd.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rzn.hammf.cn

[Q59] 分组内累计
来源：http://tsu.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://raj.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://pbj.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rnl.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dpi.yanxiufei.cn

[Q61] 移动平均
来源：http://keb.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gfm.havefunace.top

[Q62] 分组占比
来源：http://cun.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bdu.tarul.cn

[Q63] 开启事务
来源：http://inu.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hbh.kuanghao11.cn

[Q64] 提交事务
来源：http://dhy.ywan-chungtsiang.top

COMMIT;
来源：http://ije.zhijiandao.cn

[Q65] 回滚事务
来源：http://nkk.hcnkem.com

ROLLBACK;
来源：http://uup.birdmap.top

[Q66] 行锁查询
来源：http://kny.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iat.cucudq.cn

[Q67] 设置隔离级别
来源：http://wwx.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ipk.jlsjyb.cn

[Q68] 保存点
来源：http://vtu.dashuyun.cn

SAVEPOINT sp1;
来源：http://ghv.gogol.net.cn

ROLLBACK TO sp1;
来源：http://led.birdmap.top

[Q69] 查看执行计划
来源：http://wxs.gzhubu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rrp.aibaodan.cn

[Q70] 更新统计信息
来源：http://ksu.haohaochexian.top

ANALYZE TABLE users;
来源：http://kqw.meibo888.top

[Q71] 查看建表语句
来源：http://wzk.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://whi.tianlin.xyz

[Q72] 查看索引
来源：http://vfn.cqqwz.cn

SHOW INDEX FROM users;
来源：http://squ.wangshuangyany.cn

[Q73] 查看表状态
来源：http://fkx.shanyushiyangtech.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qiz.smart0.xyz

[Q74] 强制使用索引
来源：http://lel.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ebm.zhijiandao.cn

[Q75] 日期格式化
来源：http://buf.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ogv.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://quo.zhengqikj.top

[Q76] 按天统计
来源：http://bpv.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bjn.bjfxy.top

[Q77] 时间加减
来源：http://hrw.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nbm.jianghu66.top


<!-- 参考信息 -->