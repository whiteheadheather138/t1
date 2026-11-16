代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bag.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xlk.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wfv.yj20258888.top

TS:   // 同 JS
来源：http://exm.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://gmj.fanxiaobao.xyz

Go:   go f()
来源：http://div.ybcxt.top

Ruby: Thread.new { f }
来源：http://fne.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://tvc.smart0.xyz

[O02] 使用线程池
来源：http://zur.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmk.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hte.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://ocg.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://htj.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bap.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://esn.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tfn.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nlc.yj20258.top

[O03] 加锁保护共享数据
来源：http://oim.hesvh.cn

Py:   with lock: shared += 1
来源：http://tnk.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://xhj.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sfb.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://hcf.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://vum.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbc.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jrv.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://vus.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://ddz.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://crx.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://utw.ydzc1.top

JS:   async function f() { await g(); }
来源：http://fkg.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ltr.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dml.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jyn.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qui.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://jjm.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://pem.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://jqu.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gzr.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://stu.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://qcn.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tks.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://erl.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://odr.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zlh.haohaochexian.top

[O06] 使用进程池
来源：http://rmf.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vnj.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fqg.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://vkw.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://oxh.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gzt.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fwy.fengsongda.top

Ruby: // fork 块
来源：http://uzd.0kj1m.cn

C#:   Parallel.For
来源：http://cxx.yanxiufei.cn

================================================================================
来源：http://iym.hfpthk.cn

P. 常用工具函数
来源：http://knv.ywan-chungtsiang.top

================================================================================
来源：http://lya.zycfv.cn

[P01] 生成 UUID
来源：http://qwb.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://mfw.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://shr.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://ofc.jianghu66.top

TS:   crypto.randomUUID()
来源：http://nxs.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://adb.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://rad.meibo888.top

Ruby: SecureRandom.uuid
来源：http://riu.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://fwy.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://lsb.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zie.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dru.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kmj.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlv.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tdr.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdo.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lhn.zhaomingkeji.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gsb.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://hdj.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xjd.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://apr.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tjk.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fhh.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rsn.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eut.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://klj.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qan.jinqigfzy.top

[P04] 求长度
来源：http://npw.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hac.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ywn.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzd.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvv.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://vdk.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://zfw.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://wbf.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jru.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://tun.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mfh.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kxj.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cdd.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eaz.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://crs.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ufu.aizwys.cn

Ruby: a == b
来源：http://tur.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ren.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hvp.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uvo.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://tvz.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hsl.mhx1999.top

TS:   if (x == null) {}
来源：http://lxt.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fyl.chenlongwang.top

Go:   if x == nil {}
来源：http://lex.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lsf.yuanzhike.top

C#:   if (x is null) {}
来源：http://dck.snrcjt.cn

[P07] 防抖与节流
来源：http://rlj.haohaochexian.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cpk.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://zdh.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oza.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qvj.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fhj.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eqt.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvp.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mwg.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://zgl.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gcc.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wqu.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xph.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qqu.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eqo.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bch.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vjb.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nbf.uphjek.com

================================================================================
来源：http://buz.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ifl.yj20258.top

================================================================================
来源：http://nyf.sjlbkw.cn

[Q01] 创建表
来源：http://xix.smart0.xyz

CREATE TABLE users (
来源：http://ucr.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cim.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://fqd.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://vyc.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vym.hywenlv.cn

);
来源：http://vwb.yangfankeji.com

[Q02] 创建带外键的表
来源：http://jur.chenlongwang.top

CREATE TABLE orders (
来源：http://wba.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pcz.yj202588.top

user_id INT NOT NULL,
来源：http://gwx.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://fke.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdu.cucudq.cn

);
来源：http://eof.shanyushiyangtech.top

[Q03] 增加列
来源：http://esa.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uye.dashuyun.cn

[Q04] 修改列类型
来源：http://fap.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xfh.hywenlv.cn

[Q05] 重命名列
来源：http://iei.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gde.chenzaomai.com

[Q06] 删除列
来源：http://ykk.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://tqw.redwolf501.top

[Q07] 删除表
来源：http://ohr.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://fcf.guowangkeji.top

[Q08] 创建普通索引
来源：http://fwg.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hui.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://zsz.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hbi.vehdjk.com

[Q10] 插入单行
来源：http://qhv.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mof.yvedp.cn

[Q11] 一次插入多行
来源：http://aqf.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aei.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://pvq.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://tcc.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pcg.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://kts.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jss.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://tjl.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fzy.yangfankeji.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qga.redwolf501.top

[Q15] 查询全部
来源：http://rzc.vehdjk.com

SELECT * FROM users;
来源：http://wyq.jinqigfzy.top

[Q16] 查询指定列
来源：http://qaq.shzxlz.cn

SELECT id, name FROM users;
来源：http://nls.nanxinkj.top

[Q17] 条件查询
来源：http://iuq.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mdf.svipenyu.cn

[Q18] 模糊匹配
来源：http://slj.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qbr.nanxinkj.top

[Q19] 范围查询
来源：http://exg.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ypd.aibaodan.cn

[Q20] IN 列表
来源：http://fpx.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bhz.sjlbkw.cn

[Q21] 空值判断
来源：http://ssu.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pcb.andypj.xyz

[Q22] 排序
来源：http://ftv.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tua.wangdashe.top

[Q23] 分页
来源：http://zev.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzo.pycfn.com

[Q24] 去重
来源：http://bmo.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://msr.hnxiangtu.top

[Q25] 只取前 N 条
来源：http://vju.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kwm.52xcode.cn

[Q26] 计数
来源：http://dlx.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://upw.hongshengwenyu.top

[Q27] 条件计数
来源：http://ysl.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dov.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://hbv.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qux.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://hwb.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://isr.ydzc1.top

[Q30] 分组统计
来源：http://tjg.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mae.cqqwz.cn

[Q31] 分组后过滤
来源：http://exv.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://llo.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://gai.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://knv.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://unk.zhongyouzk.top

[Q33] 多列分组
来源：http://gur.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qaw.hfpthk.cn

[Q34] 每组取第一条
来源：http://cle.nanxinkj.top

SELECT * FROM (
来源：http://daf.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cpt.cucudq.cn

) t WHERE rn = 1;
来源：http://xbj.sufxvd.cn

[Q35] 内连接
来源：http://eox.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vaa.jlsjyb.cn

[Q36] 左连接
来源：http://lrx.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ajb.zhaomingkeji.xyz

[Q37] 右连接
来源：http://vay.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rpy.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://xjd.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://haz.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://ffa.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zpk.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://azu.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wbm.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ihs.svipenyu.cn

[Q41] 多表连接
来源：http://avk.yongpay.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://svm.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://jcv.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://bza.bbcook.cn

[Q42] 连接条件附加过滤
来源：http://vkx.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://jnq.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vgy.ydzc1.top

[Q43] 标量子查询
来源：http://sve.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lvv.dianchejie.cn

[Q44] IN 子查询
来源：http://eyd.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dnf.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://ggj.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lnx.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ska.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czi.gotoacloud.top

[Q47] 与平均值比较
来源：http://ibv.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mow.fzhhl.top

[Q48] CTE 公用表表达式
来源：http://gmf.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tah.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://lte.jinghuilouyu.cn

[Q49] 更新单行
来源：http://wft.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kjq.shangyingyoupin.top

[Q50] 批量更新
来源：http://gyp.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lyp.bjfxy.top

[Q51] 用子查询更新
来源：http://hot.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wil.wangshuangyany.cn

[Q52] 删除指定行
来源：http://myr.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://qmb.hesvh.cn

[Q53] 按条件删除
来源：http://ree.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gzb.hesvh.cn

[Q54] 清空表
来源：http://aib.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://omc.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://dof.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vqs.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://eie.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kaf.xinyue.icu

[Q57] 行号
来源：http://ahr.jinyuanbaomall.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nyo.daria6918.cn

[Q58] 累计求和
来源：http://ovh.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://abe.yongpay.top

[Q59] 分组内累计
来源：http://paw.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jwh.hysaishi.cn

[Q60] 取上一行 / 下一行
来源：http://hvz.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fex.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zoq.hnqzz.top

[Q61] 移动平均
来源：http://afp.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hdr.nanxinkj.top

[Q62] 分组占比
来源：http://flm.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ytq.iojbl.cn

[Q63] 开启事务
来源：http://dgo.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://eqr.c1oappe.top

[Q64] 提交事务
来源：http://xlr.xuanzx.com

COMMIT;
来源：http://fyc.c1oappe.top

[Q65] 回滚事务
来源：http://zdh.iojbl.cn

ROLLBACK;
来源：http://now.jyoumei.cn

[Q66] 行锁查询
来源：http://nyk.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://paj.shanyushiyangkeji.top

[Q67] 设置隔离级别
来源：http://mml.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bmj.zhaomingkeji.xyz

[Q68] 保存点
来源：http://gnl.fengsongda.top

SAVEPOINT sp1;
来源：http://rux.fzhhl.top

ROLLBACK TO sp1;
来源：http://ymb.meibo888.top

[Q69] 查看执行计划
来源：http://ptp.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://faw.chenlongwang.top

[Q70] 更新统计信息
来源：http://ygk.chenzaomai.com

ANALYZE TABLE users;
来源：http://gii.ehwqpu.com

[Q71] 查看建表语句
来源：http://hqc.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://njb.sweek.top

[Q72] 查看索引
来源：http://vpa.tanke756.top

SHOW INDEX FROM users;
来源：http://uix.andypj.xyz

[Q73] 查看表状态
来源：http://vrj.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kze.nanxinkj.top

[Q74] 强制使用索引
来源：http://zvi.zhengqikj.top


<!-- 参考信息 -->