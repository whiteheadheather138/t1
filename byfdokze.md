代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://qwq.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bwp.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://jvs.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lnm.sysykeji.top

PHP:  // 手写递归函数
来源：http://zfj.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yni.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xqi.nanxuanxn.top

Java: // 手写递归
来源：http://ohw.ctjpmb.com

Go:   // 手写递归
来源：http://lqr.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rsw.jinqigufen.top

C#:   // 手写递归
来源：http://guc.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pdt.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ekh.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lwo.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vux.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zja.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xsh.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zqg.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://riz.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hqx.jinqigfzy.top

================================================================================
来源：http://hlz.redwolf501.top

O. 并发与异步
来源：http://boo.yj202588.top

================================================================================
来源：http://izb.hywenlv.cn

[O01] 启动一个线程
来源：http://baq.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjh.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://toi.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkt.guowangkeji.top

TS:   // 同 JS
来源：http://gpc.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://xgl.hnxiangtu.top

Go:   go f()
来源：http://shy.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://uuz.yj20258888.top

C#:   Task.Run(() => F());
来源：http://aen.cdnleiting.top

[O02] 使用线程池
来源：http://viu.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aya.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ayi.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://oyf.xinyue.icu

TS:   // worker_threads 线程池
来源：http://uzp.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://lsv.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ind.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aac.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nih.hammf.cn

[O03] 加锁保护共享数据
来源：http://rqq.hnqzz.top

Py:   with lock: shared += 1
来源：http://ayg.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://vsv.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jfq.xuanzx.com

TS:   // 同 JS
来源：http://alc.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://oof.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aot.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eso.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://bdl.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://skv.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://tey.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zvc.bbcook.cn

JS:   async function f() { await g(); }
来源：http://ben.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uhp.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jep.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qie.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://xli.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://dgg.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://olz.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://kho.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://efs.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://xbc.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://exs.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://olp.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qtp.bjfxy.top

Ruby: threads.map(&:join)
来源：http://sfv.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wdy.jinqigufen.top

[O06] 使用进程池
来源：http://cyz.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ccp.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kuq.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://afx.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://juo.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://imw.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mml.yj20258888.top

Ruby: // fork 块
来源：http://utv.0kj1m.cn

C#:   Parallel.For
来源：http://fyu.dianchejie.cn

================================================================================
来源：http://gdr.dashuyun.cn

P. 常用工具函数
来源：http://ubx.nwbrower.top

================================================================================
来源：http://ezj.guannengcc.top

[P01] 生成 UUID
来源：http://ltp.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://ahh.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cmv.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://slv.xziqi.cn

TS:   crypto.randomUUID()
来源：http://idj.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://lzk.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://zal.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://dja.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://sbe.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://iou.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://frn.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tok.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rso.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yil.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fdf.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://daf.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qcx.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zio.hnqzz.top

[P03] 生成短随机字符串
来源：http://tho.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tho.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vpg.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://erc.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mea.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hxb.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jzy.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bfl.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qtf.daxiang520.top

[P04] 求长度
来源：http://vds.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ftp.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ijw.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fze.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://plh.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://vyn.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://jux.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://mns.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ebq.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://acb.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ptx.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dxo.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qcc.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tvx.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ulo.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kld.ctjpmb.com

Ruby: a == b
来源：http://myj.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lzy.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hwv.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://apn.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://wgs.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eum.gzhubu.top

TS:   if (x == null) {}
来源：http://usf.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cyd.meibo888.top

Go:   if x == nil {}
来源：http://rnx.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eml.9152youxi.cn

C#:   if (x is null) {}
来源：http://wdc.jiagoushi.top

[P07] 防抖与节流
来源：http://lnx.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aid.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://qty.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zoi.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://prp.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kvj.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dve.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://odv.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ixg.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://yop.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rww.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rhr.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jbx.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pqp.uphjek.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oth.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://obf.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://noy.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rum.nwbrower.top

================================================================================
来源：http://tad.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wze.gaohongyu789.top

================================================================================
来源：http://vjn.fktsv.cn

[Q01] 创建表
来源：http://cvg.xziqi.cn

CREATE TABLE users (
来源：http://euk.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qzq.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://fxy.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://zif.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hot.daxiang520.top

);
来源：http://twj.yangfankeji.com

[Q02] 创建带外键的表
来源：http://dbq.bjfxy.top

CREATE TABLE orders (
来源：http://tab.cucudq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xhd.gzhubu.top

user_id INT NOT NULL,
来源：http://riv.52xcode.cn

amount DECIMAL(10, 2),
来源：http://izq.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jfb.hywenlv.cn

);
来源：http://rit.9152youxi.cn

[Q03] 增加列
来源：http://qil.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bac.xinyue.icu

[Q04] 修改列类型
来源：http://foy.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eje.aizwys.cn

[Q05] 重命名列
来源：http://vpe.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfl.jianghu66.top

[Q06] 删除列
来源：http://hwr.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://cqc.gzhubu.top

[Q07] 删除表
来源：http://cox.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://zgp.hcnkem.com

[Q08] 创建普通索引
来源：http://ncq.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://iqt.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://gqj.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nyj.jinghuilouyu.cn

[Q10] 插入单行
来源：http://wfs.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ghm.yuanzhike.top

[Q11] 一次插入多行
来源：http://mmr.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://peg.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://gbg.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://qui.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bar.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://qdf.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yvx.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://rjp.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://phb.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qnc.316326.xyz

[Q15] 查询全部
来源：http://hjs.shzxlz.cn

SELECT * FROM users;
来源：http://cqw.yfazqb.com

[Q16] 查询指定列
来源：http://hfh.aizwys.cn

SELECT id, name FROM users;
来源：http://kjt.zhijiandao.cn

[Q17] 条件查询
来源：http://ano.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oao.hcnkem.com

[Q18] 模糊匹配
来源：http://jjk.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ntk.52xcode.cn

[Q19] 范围查询
来源：http://wzt.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pus.ivvv.top

[Q20] IN 列表
来源：http://mke.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://trf.cdnleiting.top

[Q21] 空值判断
来源：http://dwp.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tmh.yueranfly.top

[Q22] 排序
来源：http://kiw.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ukm.0kj1m.cn

[Q23] 分页
来源：http://ewv.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://olr.xuanzx.com

[Q24] 去重
来源：http://llm.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://oap.jianghu66.top

[Q25] 只取前 N 条
来源：http://fwp.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sxd.sysykeji.top

[Q26] 计数
来源：http://tni.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://ywg.yfazqb.com

[Q27] 条件计数
来源：http://hnc.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lwm.meibo888.top

[Q28] 求和与平均
来源：http://uzl.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gzd.xuetiantiany.cn

[Q29] 最大最小值
来源：http://qra.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://xzc.zycfv.cn

[Q30] 分组统计
来源：http://nhk.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rst.gotoacloud.top

[Q31] 分组后过滤
来源：http://wxd.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jbx.uphjek.com

[Q32] 分组拼接字符串
来源：http://aua.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xvt.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oev.zhijiandao.cn

[Q33] 多列分组
来源：http://bsj.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jek.dashuyun.cn

[Q34] 每组取第一条
来源：http://dgh.cucudq.cn

SELECT * FROM (
来源：http://ool.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mdv.meibo888.top

) t WHERE rn = 1;
来源：http://sgi.havefunace.top

[Q35] 内连接
来源：http://hut.zhiwuduotai.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zbt.cashguo.top

[Q36] 左连接
来源：http://yxf.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qdo.zhongyouzk.top

[Q37] 右连接
来源：http://gae.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wia.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://zsg.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jwh.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://uny.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vnc.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nxj.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://anm.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lmo.guowangkeji.top

[Q41] 多表连接
来源：http://wee.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpi.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://pwj.vqdsnc.cn

JOIN products p ON p.id = o.product_id;
来源：http://nrf.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://usw.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://ftw.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jia.nanxinkj.top

[Q43] 标量子查询
来源：http://jrm.gogol.net.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pxk.hesvh.cn

[Q44] IN 子查询
来源：http://uvv.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rpi.nanxinkj.top

[Q45] EXISTS 判断存在
来源：http://bpc.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qbo.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://odp.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwn.hcnkem.com

[Q47] 与平均值比较
来源：http://aoz.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wqg.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://kle.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ljm.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://thj.shuidangran.top

[Q49] 更新单行
来源：http://dix.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wxs.jqgufenzy.top

[Q50] 批量更新
来源：http://kxz.hongshengwenyu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qgj.fzhhl.top

[Q51] 用子查询更新
来源：http://rzk.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://otj.316326.xyz

[Q52] 删除指定行
来源：http://ysx.andypj.xyz

DELETE FROM users WHERE id = 10;
来源：http://awx.c1oappe.top

[Q53] 按条件删除
来源：http://jqi.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://idp.andypj.xyz

[Q54] 清空表
来源：http://jog.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://her.havefunace.top

[Q55] 排名（并列占位）
来源：http://hol.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zzy.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://rcf.pengpengdd.cyou

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hxc.haohaochexian.top

[Q57] 行号
来源：http://egp.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wbk.yonumen.top

[Q58] 累计求和
来源：http://zjg.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yvr.zhoulong.xyz

[Q59] 分组内累计
来源：http://eyr.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vgk.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://ncj.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vxu.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nwf.wangdashe.top

[Q61] 移动平均
来源：http://cul.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zuw.9152youxi.cn

[Q62] 分组占比
来源：http://isk.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gth.sysykeji.top


<!-- 参考信息 -->