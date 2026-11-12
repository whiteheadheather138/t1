代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vrk.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qwz.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uqj.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fzz.zhaomingkeji.xyz

================================================================================
来源：http://qzk.zhijiandao.cn

O. 并发与异步
来源：http://hnb.hcnkem.com

================================================================================
来源：http://gjs.jlsjyb.cn

[O01] 启动一个线程
来源：http://lyo.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uas.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gof.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ckc.gotoacloud.top

TS:   // 同 JS
来源：http://bco.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://dpt.guowangkeji.top

Go:   go f()
来源：http://mup.shzxlz.cn

Ruby: Thread.new { f }
来源：http://qmc.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://pgu.vehdjk.com

[O02] 使用线程池
来源：http://pmw.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lls.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kwf.yfazqb.com

JS:   // worker_threads 线程池
来源：http://rce.smart0.xyz

TS:   // worker_threads 线程池
来源：http://udt.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wvg.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ach.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://spx.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gql.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://uix.0kj1m.cn

Py:   with lock: shared += 1
来源：http://gyh.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://obz.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rmu.zhengqikj.top

TS:   // 同 JS
来源：http://zqd.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://cxl.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kep.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mtk.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://nkg.aizwys.cn

[O04] 定义异步函数并等待
来源：http://wcw.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://fbo.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://urh.daxiang520.top

JS:   async function f() { await g(); }
来源：http://uzq.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tzi.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://znd.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uwr.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://dul.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://htf.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://dhc.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://lwd.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mow.cashguo.top

JS:   await Promise.all(tasks)
来源：http://irc.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://crj.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ueq.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ozu.daxiang520.top

Ruby: threads.map(&:join)
来源：http://hfi.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qud.tarul.cn

[O06] 使用进程池
来源：http://nkc.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cda.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zjh.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://beq.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://wxj.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wfo.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uxf.jlsjyb.cn

Ruby: // fork 块
来源：http://pxf.yfazqb.com

C#:   Parallel.For
来源：http://cgu.wangdashe.top

================================================================================
来源：http://njs.ybcxt.top

P. 常用工具函数
来源：http://xqo.cucudq.cn

================================================================================
来源：http://das.gogol.net.cn

[P01] 生成 UUID
来源：http://eyj.zdbjq.cn

Py:   str(uuid.uuid4())
来源：http://tuv.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nre.fengsongda.top

JS:   crypto.randomUUID()
来源：http://tut.guannengcc.top

TS:   crypto.randomUUID()
来源：http://clw.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://ftu.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://imw.hammf.cn

Ruby: SecureRandom.uuid
来源：http://uod.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://ydo.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://ydy.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mzu.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qdl.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cgv.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gys.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://icv.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eyz.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ijl.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fej.c1oappe.top

[P03] 生成短随机字符串
来源：http://vuo.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nrb.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hrv.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wpc.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kmu.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sgb.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dhw.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rnh.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ojs.sufxvd.cn

[P04] 求长度
来源：http://kxx.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jmw.vqdsnc.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gue.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dul.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wso.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://pvz.andypj.xyz

Go:   len(arr);  len(m)
来源：http://ort.zhixingplan.top

Ruby: x.length;  x.size
来源：http://tgt.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zss.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://sii.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hui.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://drt.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hto.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjq.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ddo.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://oau.tian-w.cn

Ruby: a == b
来源：http://zpo.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sxe.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://axq.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qua.tanke756.top

PHP:  if (empty($x)) {}
来源：http://lhy.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qjg.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://trq.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zmq.fengsongda.top

Go:   if x == nil {}
来源：http://pdt.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rve.tanke756.top

C#:   if (x is null) {}
来源：http://egh.yuanzhike.top

[P07] 防抖与节流
来源：http://ziz.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zgf.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://zbw.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gyf.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvh.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cco.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rte.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vdy.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lld.sysykeji.top

[P08] 处理浮点精度问题
来源：http://fqd.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yoq.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xaa.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yug.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jap.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wnz.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gbf.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rqc.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uzv.nanxinkj.top

================================================================================
来源：http://tte.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tvp.svipenyu.cn

================================================================================
来源：http://vju.birdmap.top

[Q01] 创建表
来源：http://kts.yj20258.top

CREATE TABLE users (
来源：http://ouc.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ptp.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://pbi.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://dnu.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://etg.xuetiantiany.cn

);
来源：http://ffv.52xcode.cn

[Q02] 创建带外键的表
来源：http://psj.tian-w.cn

CREATE TABLE orders (
来源：http://fqo.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qpw.zdbjq.cn

user_id INT NOT NULL,
来源：http://yag.cucudq.cn

amount DECIMAL(10, 2),
来源：http://qpt.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dqr.zdbjq.cn

);
来源：http://bje.redwolf501.top

[Q03] 增加列
来源：http://vyd.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://guh.iojbl.cn

[Q04] 修改列类型
来源：http://txp.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nus.zdbjq.cn

[Q05] 重命名列
来源：http://ktk.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gnb.ivvv.top

[Q06] 删除列
来源：http://kzz.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tiu.vehdjk.com

[Q07] 删除表
来源：http://mnv.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://ojs.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://wbf.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pqi.iojbl.cn

[Q09] 创建唯一索引
来源：http://ulc.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aua.ydjk.org.cn

[Q10] 插入单行
来源：http://nsr.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://chm.andypj.xyz

[Q11] 一次插入多行
来源：http://pck.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kyi.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://cmf.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://gvn.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ift.yj20258888.top

[Q13] 忽略重复插入
来源：http://pin.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iop.shanyushiyangtech.top

[Q14] 存在则更新（upsert）
来源：http://xac.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xet.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ykn.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://pco.yuxming.cn

SELECT * FROM users;
来源：http://tcz.sufxvd.cn

[Q16] 查询指定列
来源：http://wpb.zhongyouzk.top

SELECT id, name FROM users;
来源：http://tdn.meibo888.top

[Q17] 条件查询
来源：http://cwz.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://agw.yj202588.top

[Q18] 模糊匹配
来源：http://vpc.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fyi.nwbrower.top

[Q19] 范围查询
来源：http://zya.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mhf.daria6918.cn

[Q20] IN 列表
来源：http://xfv.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pkr.yj202588.top

[Q21] 空值判断
来源：http://smp.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wqu.zycfv.cn

[Q22] 排序
来源：http://rpn.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rdr.chenlongwang.top

[Q23] 分页
来源：http://ymt.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qzo.daria6918.cn

[Q24] 去重
来源：http://vxm.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://xvb.yj20258.top

[Q25] 只取前 N 条
来源：http://pzo.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mgh.nanxinkj.top

[Q26] 计数
来源：http://wvo.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://ngi.hywenlv.cn

[Q27] 条件计数
来源：http://unz.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rqd.epnwcf.com

[Q28] 求和与平均
来源：http://wpf.andypj.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://czm.andypj.xyz

[Q29] 最大最小值
来源：http://ydd.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tea.redwolf501.top

[Q30] 分组统计
来源：http://ifp.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ztg.sjlbkw.cn

[Q31] 分组后过滤
来源：http://aot.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iqq.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://yas.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://atr.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aas.vqdsnc.cn

[Q33] 多列分组
来源：http://ali.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mgx.zhongyouzk.top

[Q34] 每组取第一条
来源：http://gtb.wangshuangyany.cn

SELECT * FROM (
来源：http://zih.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rob.zdqjudy.top

) t WHERE rn = 1;
来源：http://rrl.ybcxt.top

[Q35] 内连接
来源：http://npi.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hcy.hnqzz.top

[Q36] 左连接
来源：http://hoc.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zjj.yj20258888.top

[Q37] 右连接
来源：http://hhw.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ynb.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ojo.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tfg.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://sqk.snrcjt.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dma.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://awx.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sjq.yuxming.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wed.tarul.cn

[Q41] 多表连接
来源：http://fic.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pyz.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://oda.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://leb.pengpengdd.cyou

[Q42] 连接条件附加过滤
来源：http://hql.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://ljo.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qrf.guannengcc.top

[Q43] 标量子查询
来源：http://yqm.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qre.tarul.cn

[Q44] IN 子查询
来源：http://ogt.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tou.tarul.cn

[Q45] EXISTS 判断存在
来源：http://icl.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nys.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://oct.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vei.chenzaomai.com

[Q47] 与平均值比较
来源：http://rwj.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pvd.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://nfl.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rws.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://rje.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://vxc.zhongyouzk.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uic.wangshuangyany.cn

[Q50] 批量更新
来源：http://ppp.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://enz.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://zar.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bfy.tianlin.xyz

[Q52] 删除指定行
来源：http://ewx.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://rhk.hnxiangtu.top

[Q53] 按条件删除
来源：http://pcn.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gfg.yongpay.top

[Q54] 清空表
来源：http://imr.yuxming.cn

TRUNCATE TABLE logs;
来源：http://kpf.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://mof.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yta.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://flr.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsg.zhijiandao.cn

[Q57] 行号
来源：http://how.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ohb.vehdjk.com

[Q58] 累计求和
来源：http://gir.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zpb.bjfxy.top

[Q59] 分组内累计
来源：http://dan.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gvp.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://pjd.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://syj.daxiang520.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tru.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://mgs.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lni.yueranfly.top

[Q62] 分组占比
来源：http://dsl.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dvw.jiagoushi.top

[Q63] 开启事务
来源：http://jnx.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bvn.yj20258.top

[Q64] 提交事务
来源：http://tbs.xuanzx.com

COMMIT;
来源：http://izr.chenzaomai.com

[Q65] 回滚事务
来源：http://qhn.yj20258888.top

ROLLBACK;
来源：http://bkf.uphjek.com

[Q66] 行锁查询
来源：http://yyg.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gzq.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://wim.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rri.fktsv.cn

[Q68] 保存点
来源：http://fgx.sysykeji.top

SAVEPOINT sp1;
来源：http://xra.hnqzz.top

ROLLBACK TO sp1;
来源：http://huo.ctjpmb.com

[Q69] 查看执行计划
来源：http://dsw.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rga.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://dmc.jyoumei.cn


<!-- 参考信息 -->