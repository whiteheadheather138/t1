代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bnz.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bba.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zwg.sweek.top

TS:   // 同 JS
来源：http://kqj.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://huy.shzxlz.cn

Go:   go f()
来源：http://rkn.yj20258888.top

Ruby: Thread.new { f }
来源：http://sxj.uphjek.com

C#:   Task.Run(() => F());
来源：http://nni.fengsongda.top

[O02] 使用线程池
来源：http://wnm.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dby.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kzf.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://hys.gzhubu.top

TS:   // worker_threads 线程池
来源：http://rvv.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dfx.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hil.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dku.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jpn.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://ama.ybcxt.top

Py:   with lock: shared += 1
来源：http://xke.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://yfr.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ltr.yanxiufei.cn

TS:   // 同 JS
来源：http://qgc.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://vee.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yax.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cfh.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://cop.meibo888.top

[O04] 定义异步函数并等待
来源：http://hqq.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://ckg.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zjh.xinyue.icu

JS:   async function f() { await g(); }
来源：http://lie.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://jkd.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bhp.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qcm.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://pco.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://pag.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://rxo.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://ozn.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qqv.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ske.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://gqd.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ixq.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://izz.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://tak.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jot.sysykeji.top

[O06] 使用进程池
来源：http://xue.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tsh.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://qac.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://ybe.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://nbb.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ddp.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mgh.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://tlm.hnqzz.top

C#:   Parallel.For
来源：http://tbl.tanke756.top

================================================================================
来源：http://alc.hnqzz.top

P. 常用工具函数
来源：http://ikk.aibaodan.cn

================================================================================
来源：http://uzc.cdnleiting.top

[P01] 生成 UUID
来源：http://vif.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://uqa.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cuk.nwbrower.top

JS:   crypto.randomUUID()
来源：http://phm.nwbrower.top

TS:   crypto.randomUUID()
来源：http://ukx.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://qgh.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://aic.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://ymd.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://ypy.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://ebo.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://euy.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gaj.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zfl.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jyv.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xol.sysykeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npe.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ozo.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xyn.hywenlv.cn

[P03] 生成短随机字符串
来源：http://bbt.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vat.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mpy.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uce.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://biq.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jud.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gng.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rqb.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pmr.mhx1999.top

[P04] 求长度
来源：http://oxs.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vja.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxq.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rto.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nsl.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://fkl.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://mhk.yj20258888.top

Ruby: x.length;  x.size
来源：http://tqk.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pff.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://yfi.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://hix.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://znl.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mon.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jvk.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lts.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://mbl.jqgufenzy.top

Ruby: a == b
来源：http://frw.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zxu.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aeh.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vxe.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://bsj.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bws.9152youxi.cn

TS:   if (x == null) {}
来源：http://wpm.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sco.chenjidiqi.icu

Go:   if x == nil {}
来源：http://ezs.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pku.cqqwz.cn

C#:   if (x is null) {}
来源：http://hvg.cashguo.top

[P07] 防抖与节流
来源：http://oog.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ivp.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://wwk.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fav.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ast.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rdr.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ihz.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://plw.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yyg.wangdashe.top

[P08] 处理浮点精度问题
来源：http://jjb.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hys.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cjy.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ctz.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vsj.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cvl.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ljc.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lxu.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qru.yuxming.cn

================================================================================
来源：http://gee.jinyuanbaomall.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ama.hywenlv.cn

================================================================================
来源：http://vmy.zhaomingkeji.xyz

[Q01] 创建表
来源：http://pir.yonumen.top

CREATE TABLE users (
来源：http://liv.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://umw.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://fuo.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://wmb.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ula.yonumen.top

);
来源：http://snk.jinqigufen.top

[Q02] 创建带外键的表
来源：http://zby.nanxinkj.top

CREATE TABLE orders (
来源：http://dab.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jea.hesvh.cn

user_id INT NOT NULL,
来源：http://xsk.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://cod.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qit.gaohongyu789.top

);
来源：http://nrd.epnwcf.com

[Q03] 增加列
来源：http://nmz.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fih.yuanzhike.top

[Q04] 修改列类型
来源：http://mir.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gmw.jqgufenzy.top

[Q05] 重命名列
来源：http://evb.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gfa.hcnkem.com

[Q06] 删除列
来源：http://xuj.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jgf.epnwcf.com

[Q07] 删除表
来源：http://uxp.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://cab.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://wis.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vgx.ivvv.top

[Q09] 创建唯一索引
来源：http://moy.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fbo.yuxming.cn

[Q10] 插入单行
来源：http://kcc.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://opz.tanke756.top

[Q11] 一次插入多行
来源：http://ovj.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uit.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://bwm.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://pxb.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ula.tian-w.cn

[Q13] 忽略重复插入
来源：http://eic.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yox.sweek.top

[Q14] 存在则更新（upsert）
来源：http://xdn.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ejg.jlsjyb.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://art.jinqigfzy.top

[Q15] 查询全部
来源：http://gfm.jqgufenzy.top

SELECT * FROM users;
来源：http://kzi.zhixingplan.top

[Q16] 查询指定列
来源：http://kso.hesvh.cn

SELECT id, name FROM users;
来源：http://qzw.tarul.cn

[Q17] 条件查询
来源：http://vbd.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yqg.tarul.cn

[Q18] 模糊匹配
来源：http://ifz.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ikk.zhongyouzk.top

[Q19] 范围查询
来源：http://vhg.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dvf.ppjwa.cn

[Q20] IN 列表
来源：http://iqn.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dxg.zhijiandao.cn

[Q21] 空值判断
来源：http://cbm.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ule.aizwys.cn

[Q22] 排序
来源：http://xxi.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ftr.xuetiantiany.cn

[Q23] 分页
来源：http://erv.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dji.hcnkem.com

[Q24] 去重
来源：http://ojj.uphjek.com

SELECT DISTINCT city FROM users;
来源：http://bcm.yj202588.top

[Q25] 只取前 N 条
来源：http://nph.52xcode.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kso.316326.xyz

[Q26] 计数
来源：http://jgr.hongshengwenyu.top

SELECT COUNT(*) FROM users;
来源：http://fjj.svipenyu.cn

[Q27] 条件计数
来源：http://jyb.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qxx.zhoulong.xyz

[Q28] 求和与平均
来源：http://kdy.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cqu.yj202588.top

[Q29] 最大最小值
来源：http://vvs.52xcode.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://usd.sufxvd.cn

[Q30] 分组统计
来源：http://lsz.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tbo.ydzc1.top

[Q31] 分组后过滤
来源：http://enf.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://imc.birdmap.top

[Q32] 分组拼接字符串
来源：http://hzc.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xrh.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oid.xuanzx.com

[Q33] 多列分组
来源：http://nnc.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ghm.yj202588.top

[Q34] 每组取第一条
来源：http://wdk.nanxinkj.top

SELECT * FROM (
来源：http://nzy.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://val.9152youxi.cn

) t WHERE rn = 1;
来源：http://bwf.zhixingplan.top

[Q35] 内连接
来源：http://wuh.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qql.ydzc1.top

[Q36] 左连接
来源：http://gdj.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lpj.yueranfly.top

[Q37] 右连接
来源：http://irr.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dli.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hsy.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gex.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://ryi.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qde.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ude.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kyw.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ddc.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://mlq.cqqwz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ggc.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://xly.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://rxm.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://skm.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://nmt.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bot.gzhubu.top

[Q43] 标量子查询
来源：http://mvi.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nlk.c1oappe.top

[Q44] IN 子查询
来源：http://fiv.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pxr.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://zjx.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bdt.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ryu.bbcook.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tsx.fzhhl.top

[Q47] 与平均值比较
来源：http://iku.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cpp.yuxming.cn

[Q48] CTE 公用表表达式
来源：http://kzx.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lta.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://jha.xziqi.cn

[Q49] 更新单行
来源：http://eip.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iyq.0kj1m.cn

[Q50] 批量更新
来源：http://thf.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://orc.ehwqpu.com

[Q51] 用子查询更新
来源：http://nup.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rjn.ctjpmb.com

[Q52] 删除指定行
来源：http://fxk.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://qwt.dashuyun.cn

[Q53] 按条件删除
来源：http://dhv.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iwy.cheryme.top

[Q54] 清空表
来源：http://unk.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://czj.havefunace.top

[Q55] 排名（并列占位）
来源：http://yxp.jianghu66.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://elo.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://fja.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://efg.hywenlv.cn

[Q57] 行号
来源：http://lks.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bek.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://edi.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://msy.jiagoushi.top

[Q59] 分组内累计
来源：http://eht.xuanzx.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wji.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://dht.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tsj.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oda.yueranfly.top

[Q61] 移动平均
来源：http://klf.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://acb.redwolf501.top

[Q62] 分组占比
来源：http://cjh.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwh.zhixingplan.top

[Q63] 开启事务
来源：http://jdl.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lzx.redwolf501.top

[Q64] 提交事务
来源：http://dmk.xingfuxueyuan.xyz

COMMIT;
来源：http://zxh.tianlin.xyz

[Q65] 回滚事务
来源：http://sji.epnwcf.com

ROLLBACK;
来源：http://woc.jiagoushi.top

[Q66] 行锁查询
来源：http://yym.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uaf.ybcxt.top

[Q67] 设置隔离级别
来源：http://qkz.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://waj.chenzaomai.com

[Q68] 保存点
来源：http://tux.tianlin.xyz

SAVEPOINT sp1;
来源：http://hlu.xinyue.icu

ROLLBACK TO sp1;
来源：http://kta.yj20258.top

[Q69] 查看执行计划
来源：http://jmr.cashguo.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://clo.mhx1999.top

[Q70] 更新统计信息
来源：http://azz.jianghu66.top

ANALYZE TABLE users;
来源：http://cll.zhijiandao.cn

[Q71] 查看建表语句
来源：http://llj.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://noo.bjfxy.top

[Q72] 查看索引
来源：http://lqd.havefunace.top

SHOW INDEX FROM users;
来源：http://tjp.snrcjt.cn

[Q73] 查看表状态
来源：http://vuj.xinyue.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://gwv.fengsongda.top

[Q74] 强制使用索引
来源：http://tzy.tianlin.xyz


<!-- 参考信息 -->