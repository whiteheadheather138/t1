代发 wailian999

Go:   // 手写递归
来源：http://xnl.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kxe.haohaochexian.top

C#:   // 手写递归
来源：http://xez.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://siy.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wsi.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fyy.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwb.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgd.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hva.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://drw.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gdm.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ahk.cheryme.top

================================================================================
来源：http://ogm.nanxuanxn.top

O. 并发与异步
来源：http://dmn.ywan-chungtsiang.top

================================================================================
来源：http://mwt.hnqzz.top

[O01] 启动一个线程
来源：http://cjc.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://soc.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ozn.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fhn.hfpthk.cn

TS:   // 同 JS
来源：http://xoc.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://kmj.yangfankeji.com

Go:   go f()
来源：http://lnr.cdnleiting.top

Ruby: Thread.new { f }
来源：http://zhq.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://pog.redwolf501.top

[O02] 使用线程池
来源：http://ffn.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hoy.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://prr.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://enx.hesvh.cn

TS:   // worker_threads 线程池
来源：http://trl.haohaochexian.top

Java: Executors.newFixedThreadPool(4)
来源：http://uhi.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pmj.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jmo.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jvb.shuidangran.top

[O03] 加锁保护共享数据
来源：http://otr.gogol.net.cn

Py:   with lock: shared += 1
来源：http://imr.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://lqa.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bwp.fktsv.cn

TS:   // 同 JS
来源：http://buk.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://ivk.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jce.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bpt.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://hgx.hnqzz.top

[O04] 定义异步函数并等待
来源：http://qua.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://xnq.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xwj.hesvh.cn

JS:   async function f() { await g(); }
来源：http://uky.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://apb.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://scr.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fzs.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://paq.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://rif.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://wzl.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://rbk.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://khr.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://jyc.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://ayp.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dtk.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kjc.dianchejie.cn

Ruby: threads.map(&:join)
来源：http://vck.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://taa.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://vzh.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vws.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dcb.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://zlb.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://hwu.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wcv.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bke.ivvv.top

Ruby: // fork 块
来源：http://inm.nanxinkj.top

C#:   Parallel.For
来源：http://tsh.birdmap.top

================================================================================
来源：http://qgi.fanxiaobao.xyz

P. 常用工具函数
来源：http://stt.ivvv.top

================================================================================
来源：http://wad.yj20258888.top

[P01] 生成 UUID
来源：http://bnn.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://bqh.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pzi.redwolf501.top

JS:   crypto.randomUUID()
来源：http://bhj.c1oappe.top

TS:   crypto.randomUUID()
来源：http://fvf.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://coc.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://mbd.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://vdz.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://aiq.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://aal.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rbh.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kch.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nfv.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ibh.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ouf.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vzz.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://idm.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sxm.hcnkem.com

[P03] 生成短随机字符串
来源：http://pwa.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wvu.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://crc.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aay.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gtb.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfz.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gtu.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mxo.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fdp.ppjwa.cn

[P04] 求长度
来源：http://qgk.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ybw.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wuh.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nor.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elz.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://nrg.hnqzz.top

Go:   len(arr);  len(m)
来源：http://upl.meibo888.top

Ruby: x.length;  x.size
来源：http://eno.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pat.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://qai.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kyo.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hml.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xet.xziqi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sgr.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://txn.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://aka.ctjpmb.com

Ruby: a == b
来源：http://jfq.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wic.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rmj.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjk.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://oxw.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mpi.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://hat.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://waz.gotoacloud.top

Go:   if x == nil {}
来源：http://ifw.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blp.yfazqb.com

C#:   if (x is null) {}
来源：http://wca.cdnleiting.top

[P07] 防抖与节流
来源：http://ilg.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nee.yj202588.top

PHP:  // 手写时间戳比较
来源：http://rek.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ecy.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hsg.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://trx.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wni.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bfn.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ncr.hammf.cn

[P08] 处理浮点精度问题
来源：http://ajg.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abt.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ack.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pej.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zxb.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ipb.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ovo.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pmn.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dsn.snrcjt.cn

================================================================================
来源：http://ngo.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nrb.fanxiaobao.xyz

================================================================================
来源：http://tna.yj202588.top

[Q01] 创建表
来源：http://vtw.pengpengdd.cyou

CREATE TABLE users (
来源：http://kwn.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ens.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://mam.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://jdx.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wba.zhengqikj.top

);
来源：http://epq.cqqwz.cn

[Q02] 创建带外键的表
来源：http://axs.tarul.cn

CREATE TABLE orders (
来源：http://eub.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fna.bjfxy.top

user_id INT NOT NULL,
来源：http://ppn.nwbrower.top

amount DECIMAL(10, 2),
来源：http://spi.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://szr.andypj.xyz

);
来源：http://cdq.dashuyun.cn

[Q03] 增加列
来源：http://ywj.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ycx.cashguo.top

[Q04] 修改列类型
来源：http://jva.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ybb.gotoacloud.top

[Q05] 重命名列
来源：http://qcu.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nrp.xziqi.cn

[Q06] 删除列
来源：http://nbd.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://znr.guowangkeji.top

[Q07] 删除表
来源：http://nvz.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://par.jqgfzy.top

[Q08] 创建普通索引
来源：http://kuk.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qit.52xcode.cn

[Q09] 创建唯一索引
来源：http://aga.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ivf.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://nsf.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wcg.tianlin.xyz

[Q11] 一次插入多行
来源：http://ckt.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nbs.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://dyo.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://ldk.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ctu.snrcjt.cn

[Q13] 忽略重复插入
来源：http://gzg.fehbvm.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cpp.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://ckf.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wxo.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tzr.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://evk.hnxiangtu.top

SELECT * FROM users;
来源：http://pra.jinqigfzy.top

[Q16] 查询指定列
来源：http://hgv.guowangkeji.top

SELECT id, name FROM users;
来源：http://pow.yj20258888.top

[Q17] 条件查询
来源：http://yit.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ncv.tanke756.top

[Q18] 模糊匹配
来源：http://dgr.jinghuilouyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gta.vqdsnc.cn

[Q19] 范围查询
来源：http://het.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zve.guowangkeji.top

[Q20] IN 列表
来源：http://cyo.jyoumei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xdr.tianlin.xyz

[Q21] 空值判断
来源：http://vvt.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kbc.tanke756.top

[Q22] 排序
来源：http://pnk.yongpay.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://djo.jiagoushi.top

[Q23] 分页
来源：http://baq.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pys.pycfn.com

[Q24] 去重
来源：http://nzs.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://opi.yuanzhike.top

[Q25] 只取前 N 条
来源：http://avy.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rut.jianghu66.top

[Q26] 计数
来源：http://miz.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://gpv.hnxiangtu.top

[Q27] 条件计数
来源：http://zoq.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jvn.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://rbs.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zmj.tarul.cn

[Q29] 最大最小值
来源：http://uqi.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cpz.sufxvd.cn

[Q30] 分组统计
来源：http://xjr.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dyz.tarul.cn

[Q31] 分组后过滤
来源：http://bgf.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hld.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://fcn.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zyu.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pkq.ppjwa.cn

[Q33] 多列分组
来源：http://dyo.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cns.zhengqikj.top

[Q34] 每组取第一条
来源：http://jcz.birdmap.top

SELECT * FROM (
来源：http://xrt.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zrb.yuanzhike.top

) t WHERE rn = 1;
来源：http://pnl.guowangkeji.top

[Q35] 内连接
来源：http://qjt.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://alf.nanxuanxn.top

[Q36] 左连接
来源：http://tsp.nanxuanxn.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qds.snrcjt.cn

[Q37] 右连接
来源：http://uvq.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mse.wangdashe.top

[Q38] 全外连接（PostgreSQL）
来源：http://gxt.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jin.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://wew.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrz.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pip.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xgr.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qss.wangdashe.top

[Q41] 多表连接
来源：http://gta.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qnq.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://ewi.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://imf.yj20258888.top

[Q42] 连接条件附加过滤
来源：http://oec.gzhubu.top

SELECT u.name, o.amount FROM users u
来源：http://nzp.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gix.zdbjq.cn

[Q43] 标量子查询
来源：http://cxj.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eyv.zycfv.cn

[Q44] IN 子查询
来源：http://cgv.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hnb.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://ayc.nanxuanxn.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://udz.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://puj.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nyo.fktsv.cn

[Q47] 与平均值比较
来源：http://jrk.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fpd.sweek.top

[Q48] CTE 公用表表达式
来源：http://isl.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rhv.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://nkm.quarkkingdee.top

[Q49] 更新单行
来源：http://thq.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gfx.ppjwa.cn

[Q50] 批量更新
来源：http://zux.jianghu66.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://olb.nwbrower.top

[Q51] 用子查询更新
来源：http://aas.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cxa.xylfe.cn

[Q52] 删除指定行
来源：http://kgi.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://lgz.gzhubu.top

[Q53] 按条件删除
来源：http://pxm.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rid.hongshengwenyu.top

[Q54] 清空表
来源：http://jmo.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://ine.kuanghao11.cn

[Q55] 排名（并列占位）
来源：http://ucf.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rht.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://vcz.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hmx.ivvv.top

[Q57] 行号
来源：http://mpq.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jvi.vehdjk.com

[Q58] 累计求和
来源：http://adz.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mrk.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://hyw.pengpengdd.cyou

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eyj.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://usf.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nnk.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yym.jqgfzy.top

[Q61] 移动平均
来源：http://ihm.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lbg.hongshengwenyu.top

[Q62] 分组占比
来源：http://oka.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://epv.jyoumei.cn

[Q63] 开启事务
来源：http://ugr.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xeb.cheryme.top

[Q64] 提交事务
来源：http://xkm.fanxiaobao.xyz

COMMIT;
来源：http://xqo.ppjwa.cn

[Q65] 回滚事务
来源：http://kpx.aizwys.cn

ROLLBACK;
来源：http://kqw.gogol.net.cn

[Q66] 行锁查询
来源：http://riz.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dsf.9152youxi.cn


<!-- 参考信息 -->