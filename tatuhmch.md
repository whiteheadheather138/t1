代发 wailian999

Go:   // 手写递归
来源：http://yoy.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsq.svipenyu.cn

C#:   // 手写递归
来源：http://ott.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ihp.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://stb.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://icg.iojbl.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dtg.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cib.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lyp.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hec.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tcc.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xwx.nanxinkj.top

================================================================================
来源：http://pjm.bjfxy.top

O. 并发与异步
来源：http://igi.dashuyun.cn

================================================================================
来源：http://zzw.zhiwuduotai.top

[O01] 启动一个线程
来源：http://cwu.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ige.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dgp.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fie.jlsjyb.cn

TS:   // 同 JS
来源：http://jwv.yongpay.top

Java: new Thread(() -> f()).start()
来源：http://rye.zhijiandao.cn

Go:   go f()
来源：http://rns.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://teu.sxryk.cn

C#:   Task.Run(() => F());
来源：http://ldm.ctjpmb.com

[O02] 使用线程池
来源：http://sgk.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uyo.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rso.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://mlr.316326.xyz

TS:   // worker_threads 线程池
来源：http://pir.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://otx.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qgt.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hka.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nef.sweek.top

[O03] 加锁保护共享数据
来源：http://ogb.hcnkem.com

Py:   with lock: shared += 1
来源：http://oyp.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://myp.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vmm.tarul.cn

TS:   // 同 JS
来源：http://wuf.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://bqb.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oiw.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lbb.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://gil.havefunace.top

[O04] 定义异步函数并等待
来源：http://xfm.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://bgf.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://adz.ydzc1.top

JS:   async function f() { await g(); }
来源：http://vfd.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zth.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://adc.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://urk.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lpn.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://zai.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://mus.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://tlu.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://alf.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://qtl.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://gcl.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hrt.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xkm.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://ujx.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xkv.yonumen.top

[O06] 使用进程池
来源：http://tom.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hqk.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fhn.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://pmz.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://vzi.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uen.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wwv.yuxming.cn

Ruby: // fork 块
来源：http://ylh.zhixingplan.top

C#:   Parallel.For
来源：http://ckl.guannengcc.top

================================================================================
来源：http://fjs.iojbl.cn

P. 常用工具函数
来源：http://gyb.sufxvd.cn

================================================================================
来源：http://arg.9152youxi.cn

[P01] 生成 UUID
来源：http://dsv.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://woj.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zhg.gzhubu.top

JS:   crypto.randomUUID()
来源：http://xvd.fzhhl.top

TS:   crypto.randomUUID()
来源：http://yzw.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://sxx.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://hll.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://mhx.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://yzt.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://che.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pce.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yhr.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vpi.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kfd.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xhz.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oqf.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gzi.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uoh.zdqjudy.top

[P03] 生成短随机字符串
来源：http://krc.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zjz.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvj.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hqu.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obf.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yas.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://emr.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://foz.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fbf.cheryme.top

[P04] 求长度
来源：http://fma.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fhc.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ajz.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dzc.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yqj.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://gyz.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://jev.hammf.cn

Ruby: x.length;  x.size
来源：http://ryq.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://olt.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://tcj.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wdv.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qwm.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dez.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rio.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vug.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jvg.nanxinkj.top

Ruby: a == b
来源：http://nlm.52xcode.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dan.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qfr.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjh.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://cte.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jof.tianlin.xyz

TS:   if (x == null) {}
来源：http://tzy.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ths.ehwqpu.com

Go:   if x == nil {}
来源：http://tif.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hij.jinqigufen.top

C#:   if (x is null) {}
来源：http://ftj.jlsjyb.cn

[P07] 防抖与节流
来源：http://rdu.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cxp.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://wqm.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnf.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://quu.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jsl.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mvz.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://edm.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xey.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://uaa.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbi.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gzq.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ltz.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ask.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ese.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mkq.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://llm.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uhf.zdbjq.cn

================================================================================
来源：http://nmx.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ywg.gaohongyu789.top

================================================================================
来源：http://tfy.guannengcc.top

[Q01] 创建表
来源：http://qjn.hnxiangtu.top

CREATE TABLE users (
来源：http://fkq.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://edc.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://tpn.snrcjt.cn

email VARCHAR(100) UNIQUE,
来源：http://boh.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pdn.hnxiangtu.top

);
来源：http://hxr.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://sde.sysykeji.top

CREATE TABLE orders (
来源：http://fol.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uyv.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://ipt.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://cbm.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdd.pycfn.com

);
来源：http://iuo.zhengqikj.top

[Q03] 增加列
来源：http://tsv.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nvj.bjfxy.top

[Q04] 修改列类型
来源：http://hdg.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qwj.havefunace.top

[Q05] 重命名列
来源：http://hjq.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bmz.yangfankeji.com

[Q06] 删除列
来源：http://sxn.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rtt.zhaomingkeji.xyz

[Q07] 删除表
来源：http://tpb.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://cuy.smart0.xyz

[Q08] 创建普通索引
来源：http://bcs.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gwc.mhx1999.top

[Q09] 创建唯一索引
来源：http://wls.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dmq.haohaochexian.top

[Q10] 插入单行
来源：http://xlr.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hoo.jinqigufen.top

[Q11] 一次插入多行
来源：http://wra.jinqigufen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rlc.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://iwd.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xvc.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://prk.vehdjk.com

[Q13] 忽略重复插入
来源：http://ycy.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jpy.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://noz.tian-w.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://khw.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ijp.epnwcf.com

[Q15] 查询全部
来源：http://cmt.feifeiyinyue.top

SELECT * FROM users;
来源：http://vgc.yvedp.cn

[Q16] 查询指定列
来源：http://rxp.sweek.top

SELECT id, name FROM users;
来源：http://kns.52xcode.cn

[Q17] 条件查询
来源：http://bgq.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lyp.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://npv.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mni.ppjwa.cn

[Q19] 范围查询
来源：http://avu.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gmu.yanxiufei.cn

[Q20] IN 列表
来源：http://fjr.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gpy.cdnleiting.top

[Q21] 空值判断
来源：http://aak.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wiw.fehbvm.com

[Q22] 排序
来源：http://mzs.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qcy.chenzaomai.com

[Q23] 分页
来源：http://dit.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qmv.c1oappe.top

[Q24] 去重
来源：http://igu.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://fwv.ydjk.org.cn

[Q25] 只取前 N 条
来源：http://tfr.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tmu.ybcxt.top

[Q26] 计数
来源：http://ezu.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://lcu.jqgufenzy.top

[Q27] 条件计数
来源：http://xtz.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ezi.cdnleiting.top

[Q28] 求和与平均
来源：http://oih.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://erw.zdbjq.cn

[Q29] 最大最小值
来源：http://npv.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kuw.zdbjq.cn

[Q30] 分组统计
来源：http://kjv.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dld.gaohongyu789.top

[Q31] 分组后过滤
来源：http://wbl.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gde.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://hlw.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://myo.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://swe.sxryk.cn

[Q33] 多列分组
来源：http://fee.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://djy.hesvh.cn

[Q34] 每组取第一条
来源：http://veu.yanxiufei.cn

SELECT * FROM (
来源：http://rha.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aul.jianghu66.top

) t WHERE rn = 1;
来源：http://ion.jqgfzy.top

[Q35] 内连接
来源：http://zfa.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vfn.sysykeji.top

[Q36] 左连接
来源：http://upp.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rnb.nanxuanxn.top

[Q37] 右连接
来源：http://oev.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fac.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://kne.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://flb.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://wlk.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mwc.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tey.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nzt.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mjl.yueranfly.top

[Q41] 多表连接
来源：http://vcz.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zsx.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://jyq.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://fun.sweek.top

[Q42] 连接条件附加过滤
来源：http://cch.gogol.net.cn

SELECT u.name, o.amount FROM users u
来源：http://pln.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://get.chenlongwang.top

[Q43] 标量子查询
来源：http://tyl.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ctg.jqgufenzy.top

[Q44] IN 子查询
来源：http://omu.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vza.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://yhb.cqqwz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://usm.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://akm.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bma.hysaishi.cn

[Q47] 与平均值比较
来源：http://mzd.yangfankeji.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsp.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://upn.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wsl.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://kbo.zdbjq.cn

[Q49] 更新单行
来源：http://wtk.jiagoushi.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qiu.xylfe.cn

[Q50] 批量更新
来源：http://ilb.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lfo.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://zdo.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://csk.pengpengdd.cyou

[Q52] 删除指定行
来源：http://sox.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://mpx.fktsv.cn

[Q53] 按条件删除
来源：http://hdg.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hlz.ppjwa.cn

[Q54] 清空表
来源：http://gse.guannengcc.top

TRUNCATE TABLE logs;
来源：http://xdw.svipenyu.cn

[Q55] 排名（并列占位）
来源：http://api.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dsl.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://ups.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ccr.shzxlz.cn

[Q57] 行号
来源：http://qir.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xqb.daria6918.cn

[Q58] 累计求和
来源：http://erq.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xog.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://uij.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aft.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://scz.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hzv.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qrn.chenlongwang.top

[Q61] 移动平均
来源：http://hwi.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xux.fanxiaobao.xyz

[Q62] 分组占比
来源：http://oyx.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qrr.nanxuanxn.top

[Q63] 开启事务
来源：http://irs.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wvw.hesvh.cn

[Q64] 提交事务
来源：http://inj.zhengqikj.top

COMMIT;
来源：http://zqx.jqgufenzy.top

[Q65] 回滚事务
来源：http://jfu.chenzaomai.com

ROLLBACK;
来源：http://pvj.tian-w.cn

[Q66] 行锁查询
来源：http://wqt.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lau.nanxinkj.top


<!-- 参考信息 -->