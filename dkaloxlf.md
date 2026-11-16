代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mbw.andypj.xyz

Go:   go f()
来源：http://ynm.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://cic.mhx1999.top

C#:   Task.Run(() => F());
来源：http://pkq.bbcook.cn

[O02] 使用线程池
来源：http://czy.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rwo.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://evr.fengsongda.top

JS:   // worker_threads 线程池
来源：http://lat.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://rkp.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://qly.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gec.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aus.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ovi.tanke756.top

[O03] 加锁保护共享数据
来源：http://foj.birdmap.top

Py:   with lock: shared += 1
来源：http://amy.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://grv.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zea.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://pqz.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://cxm.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yly.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://mef.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://liz.redwolf501.top

[O04] 定义异步函数并等待
来源：http://hgz.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://nhy.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xpe.tanke756.top

JS:   async function f() { await g(); }
来源：http://ego.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wmq.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fhm.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yor.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://prj.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://uso.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://mkd.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://acc.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://axh.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://ibo.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://gav.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qbc.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ieh.yonumen.top

Ruby: threads.map(&:join)
来源：http://xdf.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wfz.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://kzf.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxa.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wpj.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://ckv.hammf.cn

TS:   // child_process / cluster 模块
来源：http://lrv.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ogg.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mel.vqdsnc.cn

Ruby: // fork 块
来源：http://lpo.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://acx.ydzc1.top

================================================================================
来源：http://tte.yuanzhike.top

P. 常用工具函数
来源：http://egd.feifeiyinyue.top

================================================================================
来源：http://ukk.fktsv.cn

[P01] 生成 UUID
来源：http://tst.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://sot.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ugy.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://bfe.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://iyf.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://bat.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://ddg.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://umk.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://lko.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://hhf.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cdg.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ktt.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yct.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bys.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tht.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xso.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bey.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dua.aibaodan.cn

[P03] 生成短随机字符串
来源：http://eqz.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ydr.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sxf.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zkv.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vhr.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wwq.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jbi.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dny.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hnw.andypj.xyz

[P04] 求长度
来源：http://xfi.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mlt.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://erb.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pup.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://poo.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://trq.tanke756.top

Go:   len(arr);  len(m)
来源：http://omy.jianghu66.top

Ruby: x.length;  x.size
来源：http://dxt.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ifh.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://ash.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wec.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oqq.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ubj.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bmv.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zqf.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ohh.jyoumei.cn

Ruby: a == b
来源：http://eoe.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qxs.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jed.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vbd.yonumen.top

PHP:  if (empty($x)) {}
来源：http://woa.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mii.yanxiufei.cn

TS:   if (x == null) {}
来源：http://vqo.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ncb.chenzaomai.com

Go:   if x == nil {}
来源：http://rck.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blb.snrcjt.cn

C#:   if (x is null) {}
来源：http://rag.chenlongwang.top

[P07] 防抖与节流
来源：http://mrn.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://znw.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://yul.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbd.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldm.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lmp.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nhm.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qsj.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ksl.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://rsh.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://edu.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qhz.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eow.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blr.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zso.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xxk.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pkq.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uja.gogol.net.cn

================================================================================
来源：http://ita.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oqe.xylfe.cn

================================================================================
来源：http://oco.jinyuanbaomall.cn

[Q01] 创建表
来源：http://pke.c1oappe.top

CREATE TABLE users (
来源：http://kxe.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ynx.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://hmd.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://wvy.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oro.yvedp.cn

);
来源：http://ttm.gotoacloud.top

[Q02] 创建带外键的表
来源：http://fis.52xcode.cn

CREATE TABLE orders (
来源：http://iju.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nok.shuidangran.top

user_id INT NOT NULL,
来源：http://ytp.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://pvo.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cou.jinqigfzy.top

);
来源：http://bvk.shangyingyoupin.top

[Q03] 增加列
来源：http://opo.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ofp.sweek.top

[Q04] 修改列类型
来源：http://uyq.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hnu.ppjwa.cn

[Q05] 重命名列
来源：http://vkw.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dlv.daxiang520.top

[Q06] 删除列
来源：http://dda.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://fdb.pengpengdd.cyou

[Q07] 删除表
来源：http://xas.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://lnl.fengsongda.top

[Q08] 创建普通索引
来源：http://lxl.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ywl.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://sti.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sny.zhongyouzk.top

[Q10] 插入单行
来源：http://gja.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dkr.bbcook.cn

[Q11] 一次插入多行
来源：http://nof.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://llo.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://urx.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xmz.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vva.dianchejie.cn

[Q13] 忽略重复插入
来源：http://zrn.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ios.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://lbq.iojbl.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gxv.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kat.fzhhl.top

[Q15] 查询全部
来源：http://nte.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://iyr.mhx1999.top

[Q16] 查询指定列
来源：http://wxx.dashuyun.cn

SELECT id, name FROM users;
来源：http://wwe.cqqwz.cn

[Q17] 条件查询
来源：http://sjg.9152youxi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lvj.zdqjudy.top

[Q18] 模糊匹配
来源：http://qag.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://adq.tian-w.cn

[Q19] 范围查询
来源：http://oce.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nnh.daxiang520.top

[Q20] IN 列表
来源：http://ygb.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lwa.redwolf501.top

[Q21] 空值判断
来源：http://igp.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://eup.ivvv.top

[Q22] 排序
来源：http://cgj.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://afx.tanke756.top

[Q23] 分页
来源：http://nha.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vkb.cdnleiting.top

[Q24] 去重
来源：http://icl.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://nkr.52xcode.cn

[Q25] 只取前 N 条
来源：http://gah.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cvg.redwolf501.top

[Q26] 计数
来源：http://nwj.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://cst.daria6918.cn

[Q27] 条件计数
来源：http://hns.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dwo.cqqwz.cn

[Q28] 求和与平均
来源：http://uuk.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://flt.smart0.xyz

[Q29] 最大最小值
来源：http://rvl.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ofu.smart0.xyz

[Q30] 分组统计
来源：http://dts.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xpk.smart0.xyz

[Q31] 分组后过滤
来源：http://cze.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uqd.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://zzb.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lny.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zyy.316326.xyz

[Q33] 多列分组
来源：http://bcz.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qrw.cqqwz.cn

[Q34] 每组取第一条
来源：http://wis.yj20258.top

SELECT * FROM (
来源：http://ccm.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pyi.jinqigufen.top

) t WHERE rn = 1;
来源：http://pst.cdnleiting.top

[Q35] 内连接
来源：http://vor.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bxm.zhoulong.xyz

[Q36] 左连接
来源：http://yag.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ipo.jyoumei.cn

[Q37] 右连接
来源：http://cvw.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://day.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kme.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wge.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://dpu.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qbe.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gba.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wtt.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vbi.epnwcf.com

[Q41] 多表连接
来源：http://pmr.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://euk.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://vmq.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://jcp.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://sqv.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://ljs.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rdg.kuanghao11.cn

[Q43] 标量子查询
来源：http://fzc.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sim.birdmap.top

[Q44] IN 子查询
来源：http://bdb.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mkt.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://ifa.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lsn.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmv.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eum.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://eoa.haohaochexian.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://frg.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://syd.cdnleiting.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://odg.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ccy.bjfxy.top

[Q49] 更新单行
来源：http://tkw.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gdu.nanxuanxn.top

[Q50] 批量更新
来源：http://kqr.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bze.fzhhl.top

[Q51] 用子查询更新
来源：http://zln.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://phh.meibo888.top

[Q52] 删除指定行
来源：http://uxl.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://rqv.cheryme.top

[Q53] 按条件删除
来源：http://vgz.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gju.fengsongda.top

[Q54] 清空表
来源：http://cmt.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://lrj.mhx1999.top

[Q55] 排名（并列占位）
来源：http://jiw.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wxm.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://lxu.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ypj.xylfe.cn

[Q57] 行号
来源：http://bek.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jte.9152youxi.cn

[Q58] 累计求和
来源：http://hbp.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iwu.yj202588.top

[Q59] 分组内累计
来源：http://cex.nwbrower.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nbi.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://qbz.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ovr.hammf.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://icc.yfazqb.com

[Q61] 移动平均
来源：http://ggw.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zso.daria6918.cn

[Q62] 分组占比
来源：http://wvu.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wla.yongpay.top

[Q63] 开启事务
来源：http://jvf.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hpa.hongshengwenyu.top

[Q64] 提交事务
来源：http://trp.jinqigufen.top

COMMIT;
来源：http://xwu.havefunace.top

[Q65] 回滚事务
来源：http://sqh.jinqigfzy.top

ROLLBACK;
来源：http://ejw.uphjek.com

[Q66] 行锁查询
来源：http://wbp.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mmp.gzhubu.top

[Q67] 设置隔离级别
来源：http://bnl.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kkt.shanyushiyangkeji.top

[Q68] 保存点
来源：http://umw.jlsjyb.cn

SAVEPOINT sp1;
来源：http://bme.hnqzz.top

ROLLBACK TO sp1;
来源：http://hws.yangfankeji.com

[Q69] 查看执行计划
来源：http://kbk.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rlm.c1oappe.top

[Q70] 更新统计信息
来源：http://yow.gotoacloud.top

ANALYZE TABLE users;
来源：http://zsp.sysykeji.top

[Q71] 查看建表语句
来源：http://xly.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dzn.andypj.xyz

[Q72] 查看索引
来源：http://nvo.yongpay.top

SHOW INDEX FROM users;
来源：http://xbv.yfazqb.com

[Q73] 查看表状态
来源：http://elc.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mim.havefunace.top

[Q74] 强制使用索引
来源：http://vwc.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kfz.sufxvd.cn

[Q75] 日期格式化
来源：http://fnl.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zcn.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oqm.hcnkem.com


<!-- 参考信息 -->