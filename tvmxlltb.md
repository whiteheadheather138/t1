代发 wailian999

Go:   // 手写递归
来源：http://tmk.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwl.zhixingplan.top

C#:   // 手写递归
来源：http://zen.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxq.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dlo.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cfl.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lde.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bcz.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gyr.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zns.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://crt.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhd.svipenyu.cn

================================================================================
来源：http://pzy.hnqzz.top

O. 并发与异步
来源：http://obl.hnqzz.top

================================================================================
来源：http://sxr.ydjk.org.cn

[O01] 启动一个线程
来源：http://uaa.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lkc.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tcv.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ymr.0kj1m.cn

TS:   // 同 JS
来源：http://yro.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://nrt.zycfv.cn

Go:   go f()
来源：http://uvd.iojbl.cn

Ruby: Thread.new { f }
来源：http://tog.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://lzu.chenzaomai.com

[O02] 使用线程池
来源：http://zgr.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yqw.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ifm.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://gfl.hcnkem.com

TS:   // worker_threads 线程池
来源：http://hvo.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yvs.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://irc.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://chh.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dze.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://kgd.fehbvm.com

Py:   with lock: shared += 1
来源：http://zfd.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://uts.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vbd.wangshuangyany.cn

TS:   // 同 JS
来源：http://jmk.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://xbe.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mzj.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jbu.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://clf.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://zxf.meibo888.top

Py:   async def f():⏎    await g()
来源：http://rvk.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qli.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://jkp.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgs.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://moi.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://imp.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://fot.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://owf.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://pyb.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://rbf.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mgi.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://ffj.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://sur.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hlx.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gzw.daxiang520.top

Ruby: threads.map(&:join)
来源：http://gyk.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ozx.bjfxy.top

[O06] 使用进程池
来源：http://zqw.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vuv.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://arc.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://nnz.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://dgv.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qro.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://exg.hysaishi.cn

Ruby: // fork 块
来源：http://trs.fanxiaobao.xyz

C#:   Parallel.For
来源：http://omd.hfpthk.cn

================================================================================
来源：http://fng.pycfn.com

P. 常用工具函数
来源：http://jnr.haohaochexian.top

================================================================================
来源：http://mfv.jyoumei.cn

[P01] 生成 UUID
来源：http://vjm.yongpay.top

Py:   str(uuid.uuid4())
来源：http://lge.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kry.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://itc.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://ovm.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://ubi.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://rag.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://vka.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://tuj.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://epo.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jiz.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vcb.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wpx.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ebn.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zhv.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fjr.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmz.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvy.jianghu66.top

[P03] 生成短随机字符串
来源：http://ufu.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gfq.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sjw.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rma.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tis.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://art.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aej.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ifx.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://seu.ivvv.top

[P04] 求长度
来源：http://wpv.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wbd.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wzc.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcs.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ooe.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://tdk.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://jzj.hysaishi.cn

Ruby: x.length;  x.size
来源：http://ria.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bbu.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://dqd.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebn.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vic.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aui.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lux.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wxa.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://wyg.dashuyun.cn

Ruby: a == b
来源：http://mxv.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uji.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wgi.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hxd.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://ehu.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qyj.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://qny.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cpq.daxiang520.top

Go:   if x == nil {}
来源：http://ftx.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kno.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://odb.hysaishi.cn

[P07] 防抖与节流
来源：http://ohf.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cfc.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://dyc.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzz.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://syz.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://omo.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://msg.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyh.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tyk.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://zqi.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lav.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uvp.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lyn.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://odh.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hrl.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kpt.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wyk.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lga.gaohongyu789.top

================================================================================
来源：http://evk.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xcq.chenlongwang.top

================================================================================
来源：http://jtx.ywan-chungtsiang.top

[Q01] 创建表
来源：http://tzn.sysykeji.top

CREATE TABLE users (
来源：http://ozc.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mze.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://sqm.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://mbq.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://obp.chenlongwang.top

);
来源：http://hmu.snrcjt.cn

[Q02] 创建带外键的表
来源：http://hrq.aibaodan.cn

CREATE TABLE orders (
来源：http://tod.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lsi.daxiang520.top

user_id INT NOT NULL,
来源：http://xzk.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://pax.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://avc.xylfe.cn

);
来源：http://ghi.dashuyun.cn

[Q03] 增加列
来源：http://whe.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vgk.gogol.net.cn

[Q04] 修改列类型
来源：http://ddj.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yvl.smart0.xyz

[Q05] 重命名列
来源：http://koe.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mye.gzhubu.top

[Q06] 删除列
来源：http://uxo.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tvz.bjfxy.top

[Q07] 删除表
来源：http://lsl.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://cwe.guannengcc.top

[Q08] 创建普通索引
来源：http://sho.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qhd.yj20258888.top

[Q09] 创建唯一索引
来源：http://vpi.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dyf.yonumen.top

[Q10] 插入单行
来源：http://xew.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fna.uphjek.com

[Q11] 一次插入多行
来源：http://sqy.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rzf.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://dgk.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://elf.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ude.yonumen.top

[Q13] 忽略重复插入
来源：http://qjx.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ywn.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://drm.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zkp.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://izs.gogol.net.cn

[Q15] 查询全部
来源：http://kdq.guannengcc.top

SELECT * FROM users;
来源：http://lje.yangfankeji.com

[Q16] 查询指定列
来源：http://nzz.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://wtu.tianlin.xyz

[Q17] 条件查询
来源：http://ijv.0kj1m.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zhp.jqgufenzy.top

[Q18] 模糊匹配
来源：http://rmg.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://imw.sweek.top

[Q19] 范围查询
来源：http://ifn.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fzq.shangyingyoupin.top

[Q20] IN 列表
来源：http://ljc.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vdo.ehwqpu.com

[Q21] 空值判断
来源：http://lsn.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mti.bbcook.cn

[Q22] 排序
来源：http://sut.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bmu.52xcode.cn

[Q23] 分页
来源：http://zcc.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zml.hcnkem.com

[Q24] 去重
来源：http://fyl.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://wxh.xinyue.icu

[Q25] 只取前 N 条
来源：http://uyh.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zdu.fzhhl.top

[Q26] 计数
来源：http://rvv.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://rkq.hcnkem.com

[Q27] 条件计数
来源：http://wdg.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ijz.yanxiufei.cn

[Q28] 求和与平均
来源：http://jam.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ull.dashuyun.cn

[Q29] 最大最小值
来源：http://nos.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nbw.sufxvd.cn

[Q30] 分组统计
来源：http://jqa.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://acy.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://kjr.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lmw.shuidangran.top

[Q32] 分组拼接字符串
来源：http://hch.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xwg.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xom.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://itl.xuanzx.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://owy.jianghu66.top

[Q34] 每组取第一条
来源：http://hhz.zhiwuduotai.top

SELECT * FROM (
来源：http://iut.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbt.guowangkeji.top

) t WHERE rn = 1;
来源：http://vpd.jianghu66.top

[Q35] 内连接
来源：http://jrv.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xhd.hnxiangtu.top

[Q36] 左连接
来源：http://xoz.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cfw.uphjek.com

[Q37] 右连接
来源：http://ldv.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hsb.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://ois.9152youxi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://air.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://nzz.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mlc.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bsz.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vgk.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nef.cheryme.top

[Q41] 多表连接
来源：http://tky.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yhr.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://mgl.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://qzx.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://xly.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://ivv.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vam.vqdsnc.cn

[Q43] 标量子查询
来源：http://pgs.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://idq.vehdjk.com

[Q44] IN 子查询
来源：http://kcm.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qgc.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://wsg.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rwi.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://rlt.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kst.vehdjk.com

[Q47] 与平均值比较
来源：http://qzy.smart0.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pff.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://ahx.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://elp.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://ryl.aibaodan.cn

[Q49] 更新单行
来源：http://tar.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gqy.pengpengdd.cyou

[Q50] 批量更新
来源：http://mof.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fdb.cqqwz.cn

[Q51] 用子查询更新
来源：http://cnl.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jjn.yfazqb.com

[Q52] 删除指定行
来源：http://muc.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://wzp.hywenlv.cn

[Q53] 按条件删除
来源：http://pmz.xinyue.icu

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lml.jiagoushi.top

[Q54] 清空表
来源：http://lgj.yongpay.top

TRUNCATE TABLE logs;
来源：http://ipo.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://ffl.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tkk.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://vsm.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vdh.vehdjk.com

[Q57] 行号
来源：http://ppk.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fqt.wangshuangyany.cn

[Q58] 累计求和
来源：http://vtu.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://crx.dashuyun.cn

[Q59] 分组内累计
来源：http://spv.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://byi.ppjwa.cn

[Q60] 取上一行 / 下一行
来源：http://fau.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vms.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://okp.ivvv.top

[Q61] 移动平均
来源：http://hvg.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zlk.fehbvm.com

[Q62] 分组占比
来源：http://mlo.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ypo.shzxlz.cn

[Q63] 开启事务
来源：http://icg.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gys.aizwys.cn

[Q64] 提交事务
来源：http://kbg.snrcjt.cn

COMMIT;
来源：http://xyf.zhijiandao.cn

[Q65] 回滚事务
来源：http://lxd.hysaishi.cn

ROLLBACK;
来源：http://okd.jinqigfzy.top

[Q66] 行锁查询
来源：http://cfz.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fnw.chenzaomai.com


<!-- 参考信息 -->