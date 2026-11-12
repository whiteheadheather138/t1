代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uxx.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://npw.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mgd.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://gah.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://wub.guowangkeji.top

Go:   go f()
来源：http://jvr.sweek.top

Ruby: Thread.new { f }
来源：http://htu.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://qgr.gogol.net.cn

[O02] 使用线程池
来源：http://axd.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gfr.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://exo.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://udd.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://bti.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://qxw.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qkq.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://thl.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bmk.tian-w.cn

[O03] 加锁保护共享数据
来源：http://ezt.sweek.top

Py:   with lock: shared += 1
来源：http://swr.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://fny.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nbs.yanxiufei.cn

TS:   // 同 JS
来源：http://jcn.sweek.top

Java: synchronized (this) { shared++; }
来源：http://mvf.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gss.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://heo.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://xyu.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://qrv.yonumen.top

Py:   async def f():⏎    await g()
来源：http://wjy.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tau.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://vpx.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewb.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wsu.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rga.ybcxt.top

Ruby: # 用 Fiber 或 async gem
来源：http://ksv.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://vgx.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://wze.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://mwg.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://llq.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://pzr.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://ekx.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sda.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://set.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://sko.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://srl.jqgufenzy.top

[O06] 使用进程池
来源：http://nsu.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aze.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lhb.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://tas.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://ddt.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tvz.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zhu.tanke756.top

Ruby: // fork 块
来源：http://ykb.tanke756.top

C#:   Parallel.For
来源：http://lvu.gzhubu.top

================================================================================
来源：http://zwq.zhongyouzk.top

P. 常用工具函数
来源：http://xza.yuanzhike.top

================================================================================
来源：http://ydz.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://nqa.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://zpc.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bea.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://thi.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://zxu.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://giw.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://vea.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://odr.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://nlz.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://yyl.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wzx.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gaa.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://owl.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gmc.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dxt.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kre.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://win.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sof.nanxinkj.top

[P03] 生成短随机字符串
来源：http://cmx.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qto.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dhs.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kst.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sid.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iom.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rjf.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dqf.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jis.sjlbkw.cn

[P04] 求长度
来源：http://kcd.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://icl.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dsw.zhiwuduotai.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jym.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gyh.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://tox.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://sgk.ctjpmb.com

Ruby: x.length;  x.size
来源：http://jya.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bqq.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://pkr.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://idj.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xfh.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qdi.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oev.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lkm.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://usl.shangyingyoupin.top

Ruby: a == b
来源：http://qzu.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gma.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://foh.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ctf.hammf.cn

PHP:  if (empty($x)) {}
来源：http://own.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lze.pycfn.com

TS:   if (x == null) {}
来源：http://ckf.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ope.jlsjyb.cn

Go:   if x == nil {}
来源：http://vdt.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qvs.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://wtz.nwbrower.top

[P07] 防抖与节流
来源：http://zkl.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://thb.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://ago.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://phq.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgh.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://riw.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pjo.epnwcf.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bhj.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rtc.jianghu66.top

[P08] 处理浮点精度问题
来源：http://tti.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pgk.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://akh.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jjw.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://waa.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mcy.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ubd.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hlr.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://krr.dashuyun.cn

================================================================================
来源：http://ptt.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://twf.chenjidiqi.icu

================================================================================
来源：http://pmg.xinyue.icu

[Q01] 创建表
来源：http://fqm.jyoumei.cn

CREATE TABLE users (
来源：http://ggp.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://szf.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://tkt.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://rsq.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://peg.yj20258.top

);
来源：http://ams.hammf.cn

[Q02] 创建带外键的表
来源：http://caw.hcnkem.com

CREATE TABLE orders (
来源：http://twy.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eto.dashuyun.cn

user_id INT NOT NULL,
来源：http://sqq.hywenlv.cn

amount DECIMAL(10, 2),
来源：http://fof.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ygs.wangshuangyany.cn

);
来源：http://evd.zycfv.cn

[Q03] 增加列
来源：http://tpd.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rfp.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://iad.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gss.ydzc1.top

[Q05] 重命名列
来源：http://qad.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mwm.yj202588.top

[Q06] 删除列
来源：http://hhe.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://lsd.ybcxt.top

[Q07] 删除表
来源：http://oti.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://znu.hysaishi.cn

[Q08] 创建普通索引
来源：http://zvr.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rwl.hcnkem.com

[Q09] 创建唯一索引
来源：http://znz.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eag.epnwcf.com

[Q10] 插入单行
来源：http://xhk.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jlk.fengsongda.top

[Q11] 一次插入多行
来源：http://qiu.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hec.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://dnb.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://bhj.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://grm.fengsongda.top

[Q13] 忽略重复插入
来源：http://ysc.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dji.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://vgi.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://drl.sxryk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bff.hnxiangtu.top

[Q15] 查询全部
来源：http://dyw.ivvv.top

SELECT * FROM users;
来源：http://scx.iojbl.cn

[Q16] 查询指定列
来源：http://vfd.yj202588.top

SELECT id, name FROM users;
来源：http://auj.ctjpmb.com

[Q17] 条件查询
来源：http://ceo.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pzk.c1oappe.top

[Q18] 模糊匹配
来源：http://jmg.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dkg.zdqjudy.top

[Q19] 范围查询
来源：http://fka.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bim.fanxiaobao.xyz

[Q20] IN 列表
来源：http://akp.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qjr.bjfxy.top

[Q21] 空值判断
来源：http://lft.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qzn.shangyingyoupin.top

[Q22] 排序
来源：http://cxl.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://avv.zycfv.cn

[Q23] 分页
来源：http://nbm.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kws.jyoumei.cn

[Q24] 去重
来源：http://stv.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://nob.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://fnu.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cgn.epnwcf.com

[Q26] 计数
来源：http://xwq.iojbl.cn

SELECT COUNT(*) FROM users;
来源：http://lvl.52xcode.cn

[Q27] 条件计数
来源：http://zzf.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ptk.cheryme.top

[Q28] 求和与平均
来源：http://gpl.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ulg.yvedp.cn

[Q29] 最大最小值
来源：http://cnw.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rdj.wangdashe.top

[Q30] 分组统计
来源：http://vvd.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omv.jqgfzy.top

[Q31] 分组后过滤
来源：http://nkv.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qyc.xziqi.cn

[Q32] 分组拼接字符串
来源：http://yhz.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pee.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tzt.ppjwa.cn

[Q33] 多列分组
来源：http://kzr.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://njn.dianchejie.cn

[Q34] 每组取第一条
来源：http://rkc.redwolf501.top

SELECT * FROM (
来源：http://lta.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://apn.epnwcf.com

) t WHERE rn = 1;
来源：http://anv.aibaodan.cn

[Q35] 内连接
来源：http://hgl.uphjek.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://evz.kuanghao11.cn

[Q36] 左连接
来源：http://jhp.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://umk.xuanzx.com

[Q37] 右连接
来源：http://qes.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jon.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vgs.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zut.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://hqm.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vdm.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hci.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vov.andypj.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://trn.yfazqb.com

[Q41] 多表连接
来源：http://dat.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qop.gogol.net.cn

JOIN users u ON u.id = o.user_id
来源：http://him.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://gre.uphjek.com

[Q42] 连接条件附加过滤
来源：http://jcm.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://kfw.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ztu.mhx1999.top

[Q43] 标量子查询
来源：http://enb.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wsj.wangshuangyany.cn

[Q44] IN 子查询
来源：http://nzz.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cqc.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://vuw.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://unv.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://unk.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tlo.sysykeji.top

[Q47] 与平均值比较
来源：http://rtu.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gdv.cashguo.top

[Q48] CTE 公用表表达式
来源：http://rtv.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://izn.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://ool.daxiang520.top

[Q49] 更新单行
来源：http://rbm.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qys.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://uts.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pyf.yvedp.cn

[Q51] 用子查询更新
来源：http://whr.svipenyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mso.chenzaomai.com

[Q52] 删除指定行
来源：http://jpy.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://spv.cdnleiting.top

[Q53] 按条件删除
来源：http://smp.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mdp.shangyingyoupin.top

[Q54] 清空表
来源：http://rwl.shuidangran.top

TRUNCATE TABLE logs;
来源：http://szo.c1oappe.top

[Q55] 排名（并列占位）
来源：http://pwu.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dwe.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://oja.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lsl.chenzaomai.com

[Q57] 行号
来源：http://otg.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swa.hesvh.cn

[Q58] 累计求和
来源：http://vxp.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nym.jqgufenzy.top

[Q59] 分组内累计
来源：http://pjt.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yfd.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://gkb.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://chn.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://goa.yj202588.top

[Q61] 移动平均
来源：http://wqt.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bzk.fehbvm.com

[Q62] 分组占比
来源：http://tau.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vzb.sjlbkw.cn

[Q63] 开启事务
来源：http://rqn.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pdd.chenzaomai.com

[Q64] 提交事务
来源：http://sgg.gzhubu.top

COMMIT;
来源：http://bqe.xylfe.cn

[Q65] 回滚事务
来源：http://fkr.cqqwz.cn

ROLLBACK;
来源：http://dkb.zdbjq.cn

[Q66] 行锁查询
来源：http://spd.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uuj.yfazqb.com

[Q67] 设置隔离级别
来源：http://pva.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ylk.zycfv.cn

[Q68] 保存点
来源：http://hyq.guannengcc.top

SAVEPOINT sp1;
来源：http://xlr.aibaodan.cn

ROLLBACK TO sp1;
来源：http://sjx.cdnleiting.top

[Q69] 查看执行计划
来源：http://cyr.chenzaomai.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ecn.fktsv.cn

[Q70] 更新统计信息
来源：http://sdx.jinqigfzy.top

ANALYZE TABLE users;
来源：http://zmo.xylfe.cn

[Q71] 查看建表语句
来源：http://hhy.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qxi.yongpay.top

[Q72] 查看索引
来源：http://tmh.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://ung.9152youxi.cn

[Q73] 查看表状态
来源：http://cmw.ydjk.org.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nxf.hesvh.cn

[Q74] 强制使用索引
来源：http://wsw.sjlbkw.cn


<!-- 参考信息 -->