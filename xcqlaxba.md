代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ytb.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bbe.tarul.cn

Java: class Node { int v; Node next; }
来源：http://hfr.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jtz.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://gjd.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ihs.yj20258.top

[N11] 二叉树中序遍历
来源：http://baa.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uuo.yj20258888.top

PHP:  // 手写递归函数
来源：http://wat.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pve.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://prg.cdnleiting.top

Java: // 手写递归
来源：http://nlj.0kj1m.cn

Go:   // 手写递归
来源：http://aam.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rix.havefunace.top

C#:   // 手写递归
来源：http://ptm.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fbs.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pbp.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nsy.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jgy.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://grz.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oak.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://npi.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tiz.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpm.dashuyun.cn

================================================================================
来源：http://alq.zhiwuduotai.top

O. 并发与异步
来源：http://zcv.zhongyouzk.top

================================================================================
来源：http://nla.0kj1m.cn

[O01] 启动一个线程
来源：http://ulq.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ssx.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nth.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://msr.guannengcc.top

TS:   // 同 JS
来源：http://hgl.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://new.zhijiandao.cn

Go:   go f()
来源：http://ebg.yuanzhike.top

Ruby: Thread.new { f }
来源：http://the.yfazqb.com

C#:   Task.Run(() => F());
来源：http://hfn.tianlin.xyz

[O02] 使用线程池
来源：http://tza.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgp.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qeh.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://ziu.guannengcc.top

TS:   // worker_threads 线程池
来源：http://dan.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://odr.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ftb.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nzu.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ivn.meibo888.top

[O03] 加锁保护共享数据
来源：http://kop.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://ggq.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://evk.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wfe.fktsv.cn

TS:   // 同 JS
来源：http://gsw.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://iul.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vuq.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fka.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://kkq.sweek.top

[O04] 定义异步函数并等待
来源：http://rpi.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://mwk.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://clk.xuanzx.com

JS:   async function f() { await g(); }
来源：http://qog.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ymk.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ubg.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ygl.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cno.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://yuk.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://joj.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://vfq.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uao.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://ypm.yj20258.top

TS:   await Promise.all(tasks)
来源：http://jyj.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://coa.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cxe.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://zhp.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://kux.tian-w.cn

[O06] 使用进程池
来源：http://fir.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rrr.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bip.hammf.cn

JS:   // child_process / cluster 模块
来源：http://alx.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://yvg.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eat.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://teq.ppjwa.cn

Ruby: // fork 块
来源：http://bab.tarul.cn

C#:   Parallel.For
来源：http://wgv.zycfv.cn

================================================================================
来源：http://lmv.wangdashe.top

P. 常用工具函数
来源：http://ndx.zhixingplan.top

================================================================================
来源：http://nhy.jqgfzy.top

[P01] 生成 UUID
来源：http://ygj.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://nli.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qar.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://gkc.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://ffn.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://wut.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://ail.meibo888.top

Ruby: SecureRandom.uuid
来源：http://cjv.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://cfd.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://bpg.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://psk.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://alm.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qdf.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aqw.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vcy.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ezo.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lye.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwz.iojbl.cn

[P03] 生成短随机字符串
来源：http://bkv.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yag.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pba.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fuu.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvl.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rej.sjlbkw.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fqa.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtv.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fjn.cucudq.cn

[P04] 求长度
来源：http://ibm.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bgb.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uki.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kjl.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvm.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://qsv.iojbl.cn

Go:   len(arr);  len(m)
来源：http://lod.shzxlz.cn

Ruby: x.length;  x.size
来源：http://zjf.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dmz.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://wwk.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lbc.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ere.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pjj.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gyu.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://njt.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://xyh.andypj.xyz

Ruby: a == b
来源：http://txn.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggl.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cng.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tgi.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://kmy.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tpx.aibaodan.cn

TS:   if (x == null) {}
来源：http://ojw.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://liy.cucudq.cn

Go:   if x == nil {}
来源：http://dho.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfq.cqqwz.cn

C#:   if (x is null) {}
来源：http://dww.cqqwz.cn

[P07] 防抖与节流
来源：http://wjr.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fjx.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://bfs.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcq.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ioa.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ord.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hfy.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lpo.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uew.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://fca.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gcv.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jsj.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tuk.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qbu.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ull.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mog.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tta.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jma.iojbl.cn

================================================================================
来源：http://lkw.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqz.daxiang520.top

================================================================================
来源：http://fhc.nanxinkj.top

[Q01] 创建表
来源：http://kya.iojbl.cn

CREATE TABLE users (
来源：http://avs.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lpc.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://vge.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://uey.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qbv.tanke756.top

);
来源：http://kzi.gzhubu.top

[Q02] 创建带外键的表
来源：http://sth.meibo888.top

CREATE TABLE orders (
来源：http://mec.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://glc.hywenlv.cn

user_id INT NOT NULL,
来源：http://scn.yongpay.top

amount DECIMAL(10, 2),
来源：http://oqr.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aty.feifeiyinyue.top

);
来源：http://jxr.jinqigufen.top

[Q03] 增加列
来源：http://mwu.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hxy.zycfv.cn

[Q04] 修改列类型
来源：http://imn.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ptn.yonumen.top

[Q05] 重命名列
来源：http://wkp.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://osh.zdqjudy.top

[Q06] 删除列
来源：http://sey.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://azv.chenzaomai.com

[Q07] 删除表
来源：http://fla.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://alh.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://ycq.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tnq.gzhubu.top

[Q09] 创建唯一索引
来源：http://ziu.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aar.cucudq.cn

[Q10] 插入单行
来源：http://usj.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dsy.wangdashe.top

[Q11] 一次插入多行
来源：http://tdm.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://txi.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://dvm.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://mfd.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lmy.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://ctk.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mpk.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://qnl.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cvm.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lqb.jinqigufen.top

[Q15] 查询全部
来源：http://dlg.daria6918.cn

SELECT * FROM users;
来源：http://wlt.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://cip.havefunace.top

SELECT id, name FROM users;
来源：http://vvp.yuxming.cn

[Q17] 条件查询
来源：http://mxm.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ynb.sysykeji.top

[Q18] 模糊匹配
来源：http://xch.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ahw.zhijiandao.cn

[Q19] 范围查询
来源：http://czb.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eot.jinghuilouyu.cn

[Q20] IN 列表
来源：http://lfv.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uaf.smart0.xyz

[Q21] 空值判断
来源：http://knt.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://aro.shzxlz.cn

[Q22] 排序
来源：http://luq.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lpn.jinyuanbaomall.cn

[Q23] 分页
来源：http://ljo.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vbq.aibaodan.cn

[Q24] 去重
来源：http://jws.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://scg.yj20258888.top

[Q25] 只取前 N 条
来源：http://ehe.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iip.zhoulong.xyz

[Q26] 计数
来源：http://mhy.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://rdr.pengpengdd.cyou

[Q27] 条件计数
来源：http://yla.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vzi.zhijiandao.cn

[Q28] 求和与平均
来源：http://vgg.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mzq.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://hxm.wangdashe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gch.ivvv.top

[Q30] 分组统计
来源：http://bkb.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fmk.svipenyu.cn

[Q31] 分组后过滤
来源：http://ili.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cze.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://stf.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ttq.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://abe.jyoumei.cn

[Q33] 多列分组
来源：http://nfr.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ikl.uphjek.com

[Q34] 每组取第一条
来源：http://rbk.ybcxt.top

SELECT * FROM (
来源：http://ftx.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qwo.0kj1m.cn

) t WHERE rn = 1;
来源：http://hnx.bbcook.cn

[Q35] 内连接
来源：http://cqv.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://npu.birdmap.top

[Q36] 左连接
来源：http://lcr.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cfl.vehdjk.com

[Q37] 右连接
来源：http://sgl.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ylm.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://qzy.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mro.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://ihp.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cor.meibo888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://evo.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://muo.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hlw.pengpengdd.cyou

[Q41] 多表连接
来源：http://fva.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jvn.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://teu.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://jff.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://idt.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://sap.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pdf.sjlbkw.cn

[Q43] 标量子查询
来源：http://fgn.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vcs.cashguo.top

[Q44] IN 子查询
来源：http://bpe.sxryk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cfb.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://bcl.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ltg.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://xvc.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dgg.52xcode.cn

[Q47] 与平均值比较
来源：http://fdr.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blq.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://lww.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qhq.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://xaa.smart0.xyz

[Q49] 更新单行
来源：http://rcr.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bdk.yj20258.top

[Q50] 批量更新
来源：http://keg.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hol.nanxuanxn.top

[Q51] 用子查询更新
来源：http://wdg.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ctk.zhijiandao.cn

[Q52] 删除指定行
来源：http://wcm.guowangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://ymm.daria6918.cn

[Q53] 按条件删除
来源：http://mtz.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://umo.jinyuanbaomall.cn

[Q54] 清空表
来源：http://bvh.316326.xyz

TRUNCATE TABLE logs;
来源：http://ogk.yj202588.top

[Q55] 排名（并列占位）
来源：http://erv.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fvb.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://ddy.vqdsnc.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rlw.sufxvd.cn

[Q57] 行号
来源：http://qzx.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nsq.cheryme.top

[Q58] 累计求和
来源：http://dso.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cbh.zhoulong.xyz

[Q59] 分组内累计
来源：http://eox.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bxw.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://sqh.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ljs.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ppg.jqgfzy.top


<!-- 参考信息 -->