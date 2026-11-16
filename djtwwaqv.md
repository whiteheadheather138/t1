代发 wailian999

================================================================================
来源：http://inf.c1oappe.top

O. 并发与异步
来源：http://ttd.zhengqikj.top

================================================================================
来源：http://fgf.vqdsnc.cn

[O01] 启动一个线程
来源：http://mdw.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://irb.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://opt.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vcs.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://vlf.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://uip.jinqigfzy.top

Go:   go f()
来源：http://emb.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://ntv.fktsv.cn

C#:   Task.Run(() => F());
来源：http://ipl.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://wgp.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgk.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://voo.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://oxp.ivvv.top

TS:   // worker_threads 线程池
来源：http://fih.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ftz.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://snk.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wgr.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cht.yj20258.top

[O03] 加锁保护共享数据
来源：http://uxl.yonumen.top

Py:   with lock: shared += 1
来源：http://gwy.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://eyp.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qdc.yj20258888.top

TS:   // 同 JS
来源：http://vqf.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://nmp.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qtf.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jyj.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://ayj.bjfxy.top

[O04] 定义异步函数并等待
来源：http://toy.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://gdx.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ttq.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://quj.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pfn.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ayb.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://llx.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mxj.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://cqz.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://zeh.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://zyw.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://atd.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://ogl.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://sbg.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qer.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kak.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://rvt.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tdc.wangshuangyany.cn

[O06] 使用进程池
来源：http://duw.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dhn.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fpv.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://eba.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://pqo.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iro.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://taq.c1oappe.top

Ruby: // fork 块
来源：http://ulo.zhijiandao.cn

C#:   Parallel.For
来源：http://auz.xuetiantiany.cn

================================================================================
来源：http://ccl.cheryme.top

P. 常用工具函数
来源：http://uhx.tarul.cn

================================================================================
来源：http://kfr.chenzaomai.com

[P01] 生成 UUID
来源：http://taj.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://rpj.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://coq.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://wct.dianchejie.cn

TS:   crypto.randomUUID()
来源：http://kml.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://xeq.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://kdr.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://bey.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://pww.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://vaf.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uxe.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vcw.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ogu.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wlz.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qrl.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://onl.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ziy.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kau.chenzaomai.com

[P03] 生成短随机字符串
来源：http://kmc.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zte.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wub.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uim.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ycr.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iqe.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gin.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://soa.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ffd.nwbrower.top

[P04] 求长度
来源：http://ggx.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hfe.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ulg.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://apo.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xnh.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://ecz.havefunace.top

Go:   len(arr);  len(m)
来源：http://xgb.yj202588.top

Ruby: x.length;  x.size
来源：http://uds.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xba.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://ait.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://clx.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cin.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lxp.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://obl.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ziy.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://uzj.jinyuanbaomall.cn

Ruby: a == b
来源：http://ona.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ofr.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pik.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jpw.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://qwa.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rwj.jqgufenzy.top

TS:   if (x == null) {}
来源：http://lpp.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xdt.zdbjq.cn

Go:   if x == nil {}
来源：http://jpj.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iic.kuanghao11.cn

C#:   if (x is null) {}
来源：http://wbv.chenlongwang.top

[P07] 防抖与节流
来源：http://saa.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xgk.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://tvp.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipn.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rph.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ozc.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vws.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nrx.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dsb.havefunace.top

[P08] 处理浮点精度问题
来源：http://smh.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fbt.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vix.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jgu.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jwz.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eow.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jox.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cle.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vca.tarul.cn

================================================================================
来源：http://hhu.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nso.sufxvd.cn

================================================================================
来源：http://wqm.chenzaomai.com

[Q01] 创建表
来源：http://zgu.shanyushiyangtech.top

CREATE TABLE users (
来源：http://hmr.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ytb.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://ele.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://yox.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ouf.zdqjudy.top

);
来源：http://jni.cashguo.top

[Q02] 创建带外键的表
来源：http://dzx.ppjwa.cn

CREATE TABLE orders (
来源：http://dfx.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://btj.bjfxy.top

user_id INT NOT NULL,
来源：http://ryy.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://kyz.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ugx.fktsv.cn

);
来源：http://vna.sufxvd.cn

[Q03] 增加列
来源：http://nku.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sox.sysykeji.top

[Q04] 修改列类型
来源：http://ljm.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gso.aizwys.cn

[Q05] 重命名列
来源：http://gvu.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cxq.nwbrower.top

[Q06] 删除列
来源：http://yap.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://qvj.fanxiaobao.xyz

[Q07] 删除表
来源：http://sec.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://qgr.fktsv.cn

[Q08] 创建普通索引
来源：http://uyc.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zbe.9152youxi.cn

[Q09] 创建唯一索引
来源：http://fel.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aph.daria6918.cn

[Q10] 插入单行
来源：http://zpg.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fbk.chenlongwang.top

[Q11] 一次插入多行
来源：http://sre.bjfxy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wad.cheryme.top

[Q12] 插入后取自增 ID
来源：http://kry.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://xca.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hep.yanxiufei.cn

[Q13] 忽略重复插入
来源：http://rmp.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dnh.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://ymy.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xcz.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zjd.zhengqikj.top

[Q15] 查询全部
来源：http://wkg.yuxming.cn

SELECT * FROM users;
来源：http://nht.jinqigfzy.top

[Q16] 查询指定列
来源：http://bzb.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://wkv.xuetiantiany.cn

[Q17] 条件查询
来源：http://pqq.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xmu.ivvv.top

[Q18] 模糊匹配
来源：http://cap.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lij.yongpay.top

[Q19] 范围查询
来源：http://uch.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dmd.hesvh.cn

[Q20] IN 列表
来源：http://qpz.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://esr.meibo888.top

[Q21] 空值判断
来源：http://wym.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ang.chenjidiqi.icu

[Q22] 排序
来源：http://dur.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vmi.tianlin.xyz

[Q23] 分页
来源：http://xwj.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qqf.aibaodan.cn

[Q24] 去重
来源：http://elc.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://puj.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://dpf.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ffj.shanyushiyangkeji.top

[Q26] 计数
来源：http://gaj.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://plc.sjlbkw.cn

[Q27] 条件计数
来源：http://zut.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xxg.epnwcf.com

[Q28] 求和与平均
来源：http://rcv.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jbh.jinqigfzy.top

[Q29] 最大最小值
来源：http://jlg.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgt.hcnkem.com

[Q30] 分组统计
来源：http://krz.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ick.jinqigfzy.top

[Q31] 分组后过滤
来源：http://sxu.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://exj.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://lik.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xnb.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yoc.zhengqikj.top

[Q33] 多列分组
来源：http://coz.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://olm.zhoulong.xyz

[Q34] 每组取第一条
来源：http://kkv.jianghu66.top

SELECT * FROM (
来源：http://eup.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fom.sxryk.cn

) t WHERE rn = 1;
来源：http://gjx.jlsjyb.cn

[Q35] 内连接
来源：http://xin.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://her.jiagoushi.top

[Q36] 左连接
来源：http://bnm.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ksr.redwolf501.top

[Q37] 右连接
来源：http://qlj.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jbe.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oqm.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zmt.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://nvd.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zhu.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bxm.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ybu.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dxm.sufxvd.cn

[Q41] 多表连接
来源：http://evv.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ugb.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://fcp.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://ruz.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://var.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://kwl.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zrn.cqqwz.cn

[Q43] 标量子查询
来源：http://yps.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aqv.shuidangran.top

[Q44] IN 子查询
来源：http://dgs.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ohf.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://hjt.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pno.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ysc.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ydz.tian-w.cn

[Q47] 与平均值比较
来源：http://gok.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wfo.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ssd.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gdk.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://scc.shanyushiyangtech.top

[Q49] 更新单行
来源：http://rrv.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhc.yangfankeji.com

[Q50] 批量更新
来源：http://shb.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lsv.smart0.xyz

[Q51] 用子查询更新
来源：http://nin.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwx.zhaomingkeji.xyz

[Q52] 删除指定行
来源：http://caq.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://ccv.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://odr.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fbc.wangdashe.top

[Q54] 清空表
来源：http://emh.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://ugp.andypj.xyz

[Q55] 排名（并列占位）
来源：http://aah.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://epm.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://iqc.gogol.net.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hki.havefunace.top

[Q57] 行号
来源：http://lwt.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://npm.dashuyun.cn

[Q58] 累计求和
来源：http://ybl.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mfj.epnwcf.com

[Q59] 分组内累计
来源：http://qfw.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://evd.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://zlr.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://olk.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mgw.daxiang520.top

[Q61] 移动平均
来源：http://tbb.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uhl.pengpengdd.cyou

[Q62] 分组占比
来源：http://frj.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bfl.jlsjyb.cn

[Q63] 开启事务
来源：http://dgu.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yer.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://rzf.cashguo.top

COMMIT;
来源：http://wun.aizwys.cn

[Q65] 回滚事务
来源：http://niq.redwolf501.top

ROLLBACK;
来源：http://kbj.sxryk.cn

[Q66] 行锁查询
来源：http://pnh.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://axu.zhaomingkeji.xyz

[Q67] 设置隔离级别
来源：http://ibv.daxiang520.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jhh.zdbjq.cn

[Q68] 保存点
来源：http://ghn.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://clc.cucudq.cn

ROLLBACK TO sp1;
来源：http://skj.nanxuanxn.top

[Q69] 查看执行计划
来源：http://ehb.feifeiyinyue.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ueo.hcnkem.com

[Q70] 更新统计信息
来源：http://nyh.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://tku.chenzaomai.com

[Q71] 查看建表语句
来源：http://maz.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yio.bbcook.cn

[Q72] 查看索引
来源：http://ahr.guowangkeji.top


<!-- 参考信息 -->