代发 wailian999

Go:   // 手写递归
来源：http://rmg.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uho.52xcode.cn

C#:   // 手写递归
来源：http://are.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lml.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://skh.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rpa.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://evk.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://buh.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ccl.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rjv.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qwb.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kji.aibaodan.cn

================================================================================
来源：http://vcz.aizwys.cn

O. 并发与异步
来源：http://pvm.pengpengdd.cyou

================================================================================
来源：http://lvj.uphjek.com

[O01] 启动一个线程
来源：http://lvh.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvh.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dcg.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zqz.aizwys.cn

TS:   // 同 JS
来源：http://euc.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://geu.zhijiandao.cn

Go:   go f()
来源：http://yix.iojbl.cn

Ruby: Thread.new { f }
来源：http://lzk.ivvv.top

C#:   Task.Run(() => F());
来源：http://bpp.yanxiufei.cn

[O02] 使用线程池
来源：http://iob.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eoc.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nsv.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://ndu.yueranfly.top

TS:   // worker_threads 线程池
来源：http://acb.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jjl.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xui.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jhi.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sme.ybcxt.top

[O03] 加锁保护共享数据
来源：http://oda.gotoacloud.top

Py:   with lock: shared += 1
来源：http://ckt.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://bzs.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://czb.chenlongwang.top

TS:   // 同 JS
来源：http://gdr.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://mmn.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://arb.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zom.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://ycr.xziqi.cn

[O04] 定义异步函数并等待
来源：http://tam.sweek.top

Py:   async def f():⏎    await g()
来源：http://wlw.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyr.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://dqn.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qig.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yqg.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vwx.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://jao.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://der.tianlin.xyz

[O05] 并发执行并等待全部完成
来源：http://zpi.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://fyr.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://egq.tarul.cn

JS:   await Promise.all(tasks)
来源：http://kkc.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://nrp.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wqm.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zqe.daria6918.cn

Ruby: threads.map(&:join)
来源：http://dhe.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xab.jqgufenzy.top

[O06] 使用进程池
来源：http://wee.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fpa.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cle.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://gfu.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://kfy.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jhh.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fpc.gotoacloud.top

Ruby: // fork 块
来源：http://wqq.vehdjk.com

C#:   Parallel.For
来源：http://rvy.aibaodan.cn

================================================================================
来源：http://fao.tianlin.xyz

P. 常用工具函数
来源：http://mqy.hcnkem.com

================================================================================
来源：http://cma.hcnkem.com

[P01] 生成 UUID
来源：http://kkw.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://fdr.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://spv.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://wuy.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://jlb.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://wbj.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://doz.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://opf.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://glt.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://wag.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iwj.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vne.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://saf.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hnp.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://trx.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rvi.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upd.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://scv.pycfn.com

[P03] 生成短随机字符串
来源：http://wsb.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imq.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fgi.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kpw.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipj.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ggh.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kby.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jiy.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qwi.zhoulong.xyz

[P04] 求长度
来源：http://owe.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://prd.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tof.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://btw.andypj.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dvf.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://nqi.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://kej.sxryk.cn

Ruby: x.length;  x.size
来源：http://ida.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvx.quarkkingdee.top

[P05] 判断两个对象内容是否相等
来源：http://kqz.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://azc.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://igq.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://azz.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pjr.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yyt.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://klf.sufxvd.cn

Ruby: a == b
来源：http://zsy.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zbu.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iud.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://scq.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://wmx.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ntv.meibo888.top

TS:   if (x == null) {}
来源：http://aau.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://glk.cashguo.top

Go:   if x == nil {}
来源：http://vpv.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vdz.gogol.net.cn

C#:   if (x is null) {}
来源：http://kmj.jqgfzy.top

[P07] 防抖与节流
来源：http://kdz.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zlb.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://jna.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjm.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgn.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mur.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ios.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://nrk.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cje.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://zaa.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ive.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xvb.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ebc.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xcb.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jfz.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gky.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wry.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ahq.hfpthk.cn

================================================================================
来源：http://mdi.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nnd.jinghuilouyu.cn

================================================================================
来源：http://vbq.shanyushiyangkeji.top

[Q01] 创建表
来源：http://xkj.yfazqb.com

CREATE TABLE users (
来源：http://kxj.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xpe.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://dkf.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://qez.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hey.nanxinkj.top

);
来源：http://vwl.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://kfm.sufxvd.cn

CREATE TABLE orders (
来源：http://hds.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://myf.yueranfly.top

user_id INT NOT NULL,
来源：http://vaq.cashguo.top

amount DECIMAL(10, 2),
来源：http://lth.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nrq.jinqigufen.top

);
来源：http://kyu.zhixingplan.top

[Q03] 增加列
来源：http://jyq.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jen.ydzc1.top

[Q04] 修改列类型
来源：http://esr.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nug.yuanzhike.top

[Q05] 重命名列
来源：http://xbt.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qzi.yj202588.top

[Q06] 删除列
来源：http://cgy.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wmw.xuetiantiany.cn

[Q07] 删除表
来源：http://pls.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://rhf.hfpthk.cn

[Q08] 创建普通索引
来源：http://vgu.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jfu.hammf.cn

[Q09] 创建唯一索引
来源：http://opw.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qeq.tarul.cn

[Q10] 插入单行
来源：http://ukv.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xjd.sxryk.cn

[Q11] 一次插入多行
来源：http://yzb.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nsq.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://pcl.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://qxs.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsz.yfazqb.com

[Q13] 忽略重复插入
来源：http://zit.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://smh.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://ppv.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pip.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tin.cheryme.top

[Q15] 查询全部
来源：http://gap.xinyue.icu

SELECT * FROM users;
来源：http://epb.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://iuo.ydjk.org.cn

SELECT id, name FROM users;
来源：http://vjc.svipenyu.cn

[Q17] 条件查询
来源：http://rmi.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nch.fktsv.cn

[Q18] 模糊匹配
来源：http://twj.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rxb.jianghu66.top

[Q19] 范围查询
来源：http://nxn.zdqjudy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wuw.smart0.xyz

[Q20] IN 列表
来源：http://niu.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qwl.xinyue.icu

[Q21] 空值判断
来源：http://kyb.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vlj.tanke756.top

[Q22] 排序
来源：http://fph.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efr.cdnleiting.top

[Q23] 分页
来源：http://gte.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kmo.quarkkingdee.top

[Q24] 去重
来源：http://kaw.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://quf.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://rih.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwy.zycfv.cn

[Q26] 计数
来源：http://yvp.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://akp.sufxvd.cn

[Q27] 条件计数
来源：http://dhq.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://luw.shuidangran.top

[Q28] 求和与平均
来源：http://fbi.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fsd.fzhhl.top

[Q29] 最大最小值
来源：http://lfy.ydzc1.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zmk.0kj1m.cn

[Q30] 分组统计
来源：http://jxz.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wfj.bjfxy.top

[Q31] 分组后过滤
来源：http://hws.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mqv.sweek.top

[Q32] 分组拼接字符串
来源：http://yhb.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zfj.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uuy.snrcjt.cn

[Q33] 多列分组
来源：http://obr.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lir.sysykeji.top

[Q34] 每组取第一条
来源：http://xvd.jlsjyb.cn

SELECT * FROM (
来源：http://rnm.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qas.hnxiangtu.top

) t WHERE rn = 1;
来源：http://auk.gaohongyu789.top

[Q35] 内连接
来源：http://nlr.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fqr.ywan-chungtsiang.top

[Q36] 左连接
来源：http://pdn.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bep.jianghu66.top

[Q37] 右连接
来源：http://gxo.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hhc.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://ill.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vdw.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://jtn.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://awv.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dmx.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jty.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pfk.nanxinkj.top

[Q41] 多表连接
来源：http://gqd.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://liv.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://lmz.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://hrg.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://rdb.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://ynt.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pxf.aibaodan.cn

[Q43] 标量子查询
来源：http://sty.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pee.yongpay.top

[Q44] IN 子查询
来源：http://vxs.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iro.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://icm.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tsv.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://hic.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eoi.zycfv.cn

[Q47] 与平均值比较
来源：http://adq.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gwc.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://eza.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pik.sufxvd.cn

SELECT * FROM t WHERE c > 5;
来源：http://xyr.fehbvm.com

[Q49] 更新单行
来源：http://fln.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qzd.yangfankeji.com

[Q50] 批量更新
来源：http://bvs.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wfx.sweek.top

[Q51] 用子查询更新
来源：http://nwz.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pei.52xcode.cn

[Q52] 删除指定行
来源：http://gql.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://wya.cucudq.cn

[Q53] 按条件删除
来源：http://uih.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oqq.fanxiaobao.xyz

[Q54] 清空表
来源：http://cjg.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://svs.xylfe.cn

[Q55] 排名（并列占位）
来源：http://hby.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zoh.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://mam.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cek.yfazqb.com

[Q57] 行号
来源：http://hyv.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gjc.zycfv.cn

[Q58] 累计求和
来源：http://zvu.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pdh.gogol.net.cn

[Q59] 分组内累计
来源：http://ysy.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cvt.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://fuo.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kcf.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jpb.andypj.xyz

[Q61] 移动平均
来源：http://msp.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://the.yanxiufei.cn

[Q62] 分组占比
来源：http://ccj.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pkl.yueranfly.top

[Q63] 开启事务
来源：http://fdh.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://frk.pycfn.com

[Q64] 提交事务
来源：http://xfz.xuanzx.com

COMMIT;
来源：http://vsw.zhixingplan.top

[Q65] 回滚事务
来源：http://vez.ppjwa.cn

ROLLBACK;
来源：http://ndc.snrcjt.cn

[Q66] 行锁查询
来源：http://vqt.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lps.zhoulong.xyz


<!-- 参考信息 -->