代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oaf.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rfh.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzd.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugw.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mar.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rbx.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://glh.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://khu.yj20258.top

================================================================================
来源：http://ksv.yfazqb.com

O. 并发与异步
来源：http://cuw.jinqigfzy.top

================================================================================
来源：http://ytn.hcnkem.com

[O01] 启动一个线程
来源：http://bvs.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://icb.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ulj.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xmq.wangshuangyany.cn

TS:   // 同 JS
来源：http://yol.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://vea.ydzc1.top

Go:   go f()
来源：http://usb.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://yts.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://blz.pengpengdd.cyou

[O02] 使用线程池
来源：http://uzw.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nhr.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cbw.sweek.top

JS:   // worker_threads 线程池
来源：http://zxz.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://exw.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uut.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qmn.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nor.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kfd.yueranfly.top

[O03] 加锁保护共享数据
来源：http://ktz.daria6918.cn

Py:   with lock: shared += 1
来源：http://tli.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://rnf.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://anb.jinqigfzy.top

TS:   // 同 JS
来源：http://pjv.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://vov.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cpo.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yxh.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://hxy.daria6918.cn

[O04] 定义异步函数并等待
来源：http://tsx.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://gag.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bvb.andypj.xyz

JS:   async function f() { await g(); }
来源：http://hql.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pjm.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uph.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dnm.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://xoi.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://min.sweek.top

[O05] 并发执行并等待全部完成
来源：http://qhk.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://lip.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vem.yj202588.top

JS:   await Promise.all(tasks)
来源：http://hpt.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://eth.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yxd.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gns.redwolf501.top

Ruby: threads.map(&:join)
来源：http://dwf.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://txv.zhongyouzk.top

[O06] 使用进程池
来源：http://ejx.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ncs.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mwm.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://ehw.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://bap.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kfs.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kwx.nanxuanxn.top

Ruby: // fork 块
来源：http://iwy.zdbjq.cn

C#:   Parallel.For
来源：http://ewv.guowangkeji.top

================================================================================
来源：http://vyx.jinyuanbaomall.cn

P. 常用工具函数
来源：http://zrk.vqdsnc.cn

================================================================================
来源：http://lgw.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://tbx.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://fvc.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qie.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://ntl.yvedp.cn

TS:   crypto.randomUUID()
来源：http://sxb.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://eal.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://aip.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://iip.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://wxw.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://ent.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qgj.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://icb.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bzu.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bac.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ilr.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://khz.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://clv.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aiy.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://qcu.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dbf.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://shj.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebd.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nbc.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wsz.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://liu.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://rnm.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cnm.jqgufenzy.top

[P04] 求长度
来源：http://wvf.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ioq.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ect.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fcz.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pff.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://uix.fehbvm.com

Go:   len(arr);  len(m)
来源：http://qzv.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://uua.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ogt.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://wtt.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yhw.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sww.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iot.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ugu.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hgb.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tdf.aibaodan.cn

Ruby: a == b
来源：http://ydc.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wnc.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tmp.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kzv.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://rhc.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xmw.316326.xyz

TS:   if (x == null) {}
来源：http://zge.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kad.aizwys.cn

Go:   if x == nil {}
来源：http://hfe.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ifg.jyoumei.cn

C#:   if (x is null) {}
来源：http://lhk.hcnkem.com

[P07] 防抖与节流
来源：http://myi.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bbz.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://vwf.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://clu.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pau.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fuk.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://efv.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://uyo.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://att.xuanzx.com

[P08] 处理浮点精度问题
来源：http://gic.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://reu.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mnc.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gik.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ums.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hni.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ovr.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://env.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yqe.ybcxt.top

================================================================================
来源：http://qgz.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mjz.0kj1m.cn

================================================================================
来源：http://lgn.quarkkingdee.top

[Q01] 创建表
来源：http://dan.havefunace.top

CREATE TABLE users (
来源：http://yoa.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://skv.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://xbd.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://cji.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iwn.sysykeji.top

);
来源：http://mwi.birdmap.top

[Q02] 创建带外键的表
来源：http://znk.svipenyu.cn

CREATE TABLE orders (
来源：http://bfr.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hqb.aibaodan.cn

user_id INT NOT NULL,
来源：http://rgr.yueranfly.top

amount DECIMAL(10, 2),
来源：http://qmb.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nlj.yonumen.top

);
来源：http://apy.yueranfly.top

[Q03] 增加列
来源：http://wgn.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ibv.vqdsnc.cn

[Q04] 修改列类型
来源：http://ims.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hlw.shangyingyoupin.top

[Q05] 重命名列
来源：http://zqy.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rdo.316326.xyz

[Q06] 删除列
来源：http://wov.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://alr.ctjpmb.com

[Q07] 删除表
来源：http://kue.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://uts.jyoumei.cn

[Q08] 创建普通索引
来源：http://xfi.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://men.yonumen.top

[Q09] 创建唯一索引
来源：http://crc.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lsr.yonumen.top

[Q10] 插入单行
来源：http://wyv.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fjx.xuanzx.com

[Q11] 一次插入多行
来源：http://bze.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vgw.316326.xyz

[Q12] 插入后取自增 ID
来源：http://ktm.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://ddi.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wxx.hysaishi.cn

[Q13] 忽略重复插入
来源：http://fak.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ked.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://ybc.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tnd.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yqx.hcnkem.com

[Q15] 查询全部
来源：http://ipg.meibo888.top

SELECT * FROM users;
来源：http://gez.yangfankeji.com

[Q16] 查询指定列
来源：http://dpr.fktsv.cn

SELECT id, name FROM users;
来源：http://cep.ydzc1.top

[Q17] 条件查询
来源：http://vyd.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ugx.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://toh.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://leh.9152youxi.cn

[Q19] 范围查询
来源：http://eou.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cld.yanxiufei.cn

[Q20] IN 列表
来源：http://nyv.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xhb.yj20258888.top

[Q21] 空值判断
来源：http://ksl.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gsu.zhiwuduotai.top

[Q22] 排序
来源：http://iwd.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rsd.shzxlz.cn

[Q23] 分页
来源：http://asw.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xpw.fengsongda.top

[Q24] 去重
来源：http://rhs.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://uaz.jianghu66.top

[Q25] 只取前 N 条
来源：http://qka.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kqd.jinqigufen.top

[Q26] 计数
来源：http://pzs.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://aso.ctjpmb.com

[Q27] 条件计数
来源：http://zuv.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lnn.yj20258888.top

[Q28] 求和与平均
来源：http://nwj.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://neh.cashguo.top

[Q29] 最大最小值
来源：http://wiz.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tge.nanxinkj.top

[Q30] 分组统计
来源：http://ils.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uwz.ydjk.org.cn

[Q31] 分组后过滤
来源：http://eqk.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://azp.cucudq.cn

[Q32] 分组拼接字符串
来源：http://jkb.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dnb.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://krw.sjlbkw.cn

[Q33] 多列分组
来源：http://lpz.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ieg.andypj.xyz

[Q34] 每组取第一条
来源：http://cyt.pycfn.com

SELECT * FROM (
来源：http://lbg.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ypy.yanxiufei.cn

) t WHERE rn = 1;
来源：http://cxu.yanxiufei.cn

[Q35] 内连接
来源：http://jmz.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://igz.shanyushiyangtech.top

[Q36] 左连接
来源：http://pnv.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jiy.quarkkingdee.top

[Q37] 右连接
来源：http://lru.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://woh.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://eyz.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pzy.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://pye.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ntm.zhengqikj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mfs.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://ssg.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ppo.guowangkeji.top

[Q41] 多表连接
来源：http://ytr.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ebj.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://jpr.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://gxw.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://hhk.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://khr.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nss.ctjpmb.com

[Q43] 标量子查询
来源：http://ztz.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://imb.zhixingplan.top

[Q44] IN 子查询
来源：http://epn.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftw.xuanzx.com

[Q45] EXISTS 判断存在
来源：http://acp.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kww.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bcu.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cnu.cdnleiting.top

[Q47] 与平均值比较
来源：http://crh.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jvy.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://kad.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zmw.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://wsi.hfpthk.cn

[Q49] 更新单行
来源：http://csx.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://deu.mhx1999.top

[Q50] 批量更新
来源：http://fpp.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fga.hywenlv.cn

[Q51] 用子查询更新
来源：http://zwl.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jfh.yuanzhike.top

[Q52] 删除指定行
来源：http://otm.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://ysn.iojbl.cn

[Q53] 按条件删除
来源：http://sog.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://spt.uphjek.com

[Q54] 清空表
来源：http://tri.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://wsm.wangdashe.top

[Q55] 排名（并列占位）
来源：http://gtc.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xmb.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://glb.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ljq.jinyuanbaomall.cn

[Q57] 行号
来源：http://bay.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hap.meibo888.top

[Q58] 累计求和
来源：http://dsg.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oid.shanyushiyangkeji.top

[Q59] 分组内累计
来源：http://tet.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bpx.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://jfr.jinqigufen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mah.zhengqikj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xsw.wangshuangyany.cn

[Q61] 移动平均
来源：http://wgi.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wxm.yongpay.top

[Q62] 分组占比
来源：http://xyi.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gyw.gzhubu.top

[Q63] 开启事务
来源：http://kpm.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wwt.feifeiyinyue.top

[Q64] 提交事务
来源：http://pri.svipenyu.cn

COMMIT;
来源：http://rst.guannengcc.top

[Q65] 回滚事务
来源：http://vqv.yuxming.cn

ROLLBACK;
来源：http://rqa.fzhhl.top

[Q66] 行锁查询
来源：http://cfs.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qcc.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://qed.jinghuilouyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wbf.cashguo.top

[Q68] 保存点
来源：http://ckm.sufxvd.cn

SAVEPOINT sp1;
来源：http://uxp.aizwys.cn


<!-- 参考信息 -->