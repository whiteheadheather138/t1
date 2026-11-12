代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncl.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iyi.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://emk.9152youxi.cn

TS:   // 同 JS
来源：http://bfw.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://soa.zdbjq.cn

Go:   go f()
来源：http://fzk.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://zbs.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://pre.hysaishi.cn

[O02] 使用线程池
来源：http://tan.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rhu.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://afj.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://ewq.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://pmf.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://szq.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xrq.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqu.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhx.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://xkk.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://gfl.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://zbq.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pgd.svipenyu.cn

TS:   // 同 JS
来源：http://yud.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://ijm.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vgj.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://fuk.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://aca.mhx1999.top

[O04] 定义异步函数并等待
来源：http://znm.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://qoh.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dac.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://uuf.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bhg.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cqm.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lne.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://pwj.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://tyo.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://lqe.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://dhj.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zvl.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://jlg.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://gvw.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gnq.jinyuanbaomall.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nfe.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://nwn.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ola.fengsongda.top

[O06] 使用进程池
来源：http://pky.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ywo.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oij.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://qkq.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://xds.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://udl.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oly.redwolf501.top

Ruby: // fork 块
来源：http://ish.jinqigufen.top

C#:   Parallel.For
来源：http://hum.fehbvm.com

================================================================================
来源：http://rps.aizwys.cn

P. 常用工具函数
来源：http://ivp.316326.xyz

================================================================================
来源：http://sgt.haohaochexian.top

[P01] 生成 UUID
来源：http://haz.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://ytt.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ikk.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://orn.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://nhf.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://xvg.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://kxk.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://xae.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://evh.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://esm.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://utk.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aur.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gzn.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://csm.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fog.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tbd.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://voq.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fjr.vehdjk.com

[P03] 生成短随机字符串
来源：http://nlk.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ebi.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ugf.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nzu.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ymk.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nse.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pzz.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lke.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vws.dianchejie.cn

[P04] 求长度
来源：http://vyv.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvd.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cbn.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rkx.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://evq.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://jpm.daria6918.cn

Go:   len(arr);  len(m)
来源：http://ypu.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://agi.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnq.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://ebi.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tsr.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vay.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uup.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ymz.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qwv.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://caa.cheryme.top

Ruby: a == b
来源：http://rzu.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jut.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jbm.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cmd.havefunace.top

PHP:  if (empty($x)) {}
来源：http://oum.wangshuangyany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrv.ivvv.top

TS:   if (x == null) {}
来源：http://jaf.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://phq.kuanghao11.cn

Go:   if x == nil {}
来源：http://wlv.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qtk.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://oyb.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://qsz.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bgz.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://vpg.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sqx.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpz.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://grb.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tuk.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ril.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oty.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://xys.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wca.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yau.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bci.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oqa.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vyz.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mcc.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aor.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jmn.meibo888.top

================================================================================
来源：http://mts.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lgk.andypj.xyz

================================================================================
来源：http://rwb.feifeiyinyue.top

[Q01] 创建表
来源：http://asw.haohaochexian.top

CREATE TABLE users (
来源：http://guh.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhx.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://nxx.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://dmf.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mzv.fktsv.cn

);
来源：http://gcj.zhengqikj.top

[Q02] 创建带外键的表
来源：http://rlq.zhixingplan.top

CREATE TABLE orders (
来源：http://fad.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xnp.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://gsn.ivvv.top

amount DECIMAL(10, 2),
来源：http://aek.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tfx.zhiwuduotai.top

);
来源：http://idy.redwolf501.top

[Q03] 增加列
来源：http://joq.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bnj.hnxiangtu.top

[Q04] 修改列类型
来源：http://usi.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uvg.xziqi.cn

[Q05] 重命名列
来源：http://afj.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sop.hongshengwenyu.top

[Q06] 删除列
来源：http://iyc.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://idw.wangdashe.top

[Q07] 删除表
来源：http://imj.havefunace.top

DROP TABLE IF EXISTS orders;
来源：http://opo.birdmap.top

[Q08] 创建普通索引
来源：http://emp.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ixq.yuxming.cn

[Q09] 创建唯一索引
来源：http://psn.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ulr.shzxlz.cn

[Q10] 插入单行
来源：http://cug.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eig.zdqjudy.top

[Q11] 一次插入多行
来源：http://iwc.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iff.ivvv.top

[Q12] 插入后取自增 ID
来源：http://qjr.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://vcn.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aib.uphjek.com

[Q13] 忽略重复插入
来源：http://xzf.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://opw.bbcook.cn

[Q14] 存在则更新（upsert）
来源：http://eoy.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fdt.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bhi.quarkkingdee.top

[Q15] 查询全部
来源：http://nvd.jiagoushi.top

SELECT * FROM users;
来源：http://phe.fengsongda.top

[Q16] 查询指定列
来源：http://lgz.ybcxt.top

SELECT id, name FROM users;
来源：http://jvh.jqgfzy.top

[Q17] 条件查询
来源：http://qsb.aibaodan.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qfi.daria6918.cn

[Q18] 模糊匹配
来源：http://pwk.yfazqb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqq.jlsjyb.cn

[Q19] 范围查询
来源：http://crl.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ezz.guannengcc.top

[Q20] IN 列表
来源：http://rxr.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qxq.yvedp.cn

[Q21] 空值判断
来源：http://ilr.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hmo.daxiang520.top

[Q22] 排序
来源：http://ygj.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvq.mhx1999.top

[Q23] 分页
来源：http://ujv.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tbh.nanxuanxn.top

[Q24] 去重
来源：http://irz.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://vgp.havefunace.top

[Q25] 只取前 N 条
来源：http://jxd.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rxs.jinghuilouyu.cn

[Q26] 计数
来源：http://auy.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://gzi.pengpengdd.cyou

[Q27] 条件计数
来源：http://cnn.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ibg.sweek.top

[Q28] 求和与平均
来源：http://tyh.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zha.feifeiyinyue.top

[Q29] 最大最小值
来源：http://idt.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sjy.feifeiyinyue.top

[Q30] 分组统计
来源：http://dpx.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://poe.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://gpp.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bfl.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://dfz.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oih.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xua.zhijiandao.cn

[Q33] 多列分组
来源：http://pib.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qii.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://cpe.ydzc1.top

SELECT * FROM (
来源：http://yzc.nwbrower.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bpg.daxiang520.top

) t WHERE rn = 1;
来源：http://ofq.zhixingplan.top

[Q35] 内连接
来源：http://erd.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://usw.iojbl.cn

[Q36] 左连接
来源：http://bab.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xbj.chenzaomai.com

[Q37] 右连接
来源：http://omg.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uin.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://skp.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tuz.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://gmp.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://blq.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wmr.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bss.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://huy.cheryme.top

[Q41] 多表连接
来源：http://kqm.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://prp.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://eus.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://ooi.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://dbv.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://zxw.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lya.iojbl.cn

[Q43] 标量子查询
来源：http://xin.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bwm.bjfxy.top

[Q44] IN 子查询
来源：http://vot.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bto.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://nti.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epy.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://pfb.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tml.yanxiufei.cn

[Q47] 与平均值比较
来源：http://zqj.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iln.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://yao.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qcr.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://gda.jyoumei.cn

[Q49] 更新单行
来源：http://qbv.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zvp.cdnleiting.top

[Q50] 批量更新
来源：http://yzp.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ofv.chenlongwang.top

[Q51] 用子查询更新
来源：http://xns.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mks.dashuyun.cn

[Q52] 删除指定行
来源：http://qrv.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://ibx.gogol.net.cn

[Q53] 按条件删除
来源：http://fhr.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vqc.pycfn.com

[Q54] 清空表
来源：http://fgx.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://bst.sufxvd.cn

[Q55] 排名（并列占位）
来源：http://obm.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xaj.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://moh.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oyd.jinyuanbaomall.cn

[Q57] 行号
来源：http://fbq.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mjq.andypj.xyz

[Q58] 累计求和
来源：http://gcz.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpl.shangyingyoupin.top

[Q59] 分组内累计
来源：http://tjp.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://odo.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://wez.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cwy.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://geo.havefunace.top

[Q61] 移动平均
来源：http://yhn.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://agw.chenzaomai.com

[Q62] 分组占比
来源：http://pof.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bdo.redwolf501.top

[Q63] 开启事务
来源：http://bih.ydzc1.top

START TRANSACTION;                -- 或 BEGIN
来源：http://itv.nwbrower.top

[Q64] 提交事务
来源：http://fus.nanxuanxn.top

COMMIT;
来源：http://vfk.yuxming.cn

[Q65] 回滚事务
来源：http://pws.guowangkeji.top

ROLLBACK;
来源：http://zvr.zycfv.cn

[Q66] 行锁查询
来源：http://wst.jinyuanbaomall.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kdz.ehwqpu.com

[Q67] 设置隔离级别
来源：http://zqn.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://atc.tianlin.xyz

[Q68] 保存点
来源：http://dpz.xziqi.cn

SAVEPOINT sp1;
来源：http://ihh.c1oappe.top

ROLLBACK TO sp1;
来源：http://dkk.bbcook.cn

[Q69] 查看执行计划
来源：http://ifb.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fup.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://mgm.sweek.top

ANALYZE TABLE users;
来源：http://fac.cucudq.cn

[Q71] 查看建表语句
来源：http://ipe.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ura.zycfv.cn

[Q72] 查看索引
来源：http://cbm.c1oappe.top

SHOW INDEX FROM users;
来源：http://djj.gogol.net.cn

[Q73] 查看表状态
来源：http://jie.fehbvm.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ior.chenlongwang.top

[Q74] 强制使用索引
来源：http://gvt.epnwcf.com


<!-- 参考信息 -->