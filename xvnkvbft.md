代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nus.cheryme.top

[N10] 链表节点定义
来源：http://ill.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhn.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uio.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tob.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ffp.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://scg.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://dpg.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kfs.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uny.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://wnz.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://opo.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://tzm.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bxl.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wew.xziqi.cn

Java: // 手写递归
来源：http://hvs.meibo888.top

Go:   // 手写递归
来源：http://xxr.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ldw.ppjwa.cn

C#:   // 手写递归
来源：http://hah.dashuyun.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ipt.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cnn.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://myc.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dvd.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vhw.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bzn.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ehm.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ybm.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lhk.gogol.net.cn

================================================================================
来源：http://wtr.chenzaomai.com

O. 并发与异步
来源：http://kbb.bbcook.cn

================================================================================
来源：http://hfd.ydjk.org.cn

[O01] 启动一个线程
来源：http://ijs.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xwu.jlsjyb.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ons.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mdw.cashguo.top

TS:   // 同 JS
来源：http://awv.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://qdh.mhx1999.top

Go:   go f()
来源：http://ydn.jqgfzy.top

Ruby: Thread.new { f }
来源：http://nrv.cheryme.top

C#:   Task.Run(() => F());
来源：http://pei.xuanzx.com

[O02] 使用线程池
来源：http://dsy.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jny.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://igx.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://ach.hesvh.cn

TS:   // worker_threads 线程池
来源：http://gif.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://hgv.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uow.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mvz.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vci.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://lur.epnwcf.com

Py:   with lock: shared += 1
来源：http://oel.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://iby.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pup.hcnkem.com

TS:   // 同 JS
来源：http://kjc.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://auj.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sng.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vhx.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://zyh.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://sib.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://sxa.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://som.sysykeji.top

JS:   async function f() { await g(); }
来源：http://mqe.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ksy.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lsh.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fvd.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://hoc.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://sgl.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://qfe.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://tfh.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sdg.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://cqx.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://zxq.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://skh.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tvt.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://ean.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nfc.jqgfzy.top

[O06] 使用进程池
来源：http://zsy.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rsh.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cxs.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://ltz.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://rti.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ddc.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wcs.tian-w.cn

Ruby: // fork 块
来源：http://mea.zhoulong.xyz

C#:   Parallel.For
来源：http://lfy.guowangkeji.top

================================================================================
来源：http://qma.tian-w.cn

P. 常用工具函数
来源：http://xum.zhoulong.xyz

================================================================================
来源：http://xxh.cdnleiting.top

[P01] 生成 UUID
来源：http://sbg.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://nes.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wdr.hnqzz.top

JS:   crypto.randomUUID()
来源：http://owg.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://efu.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://kgk.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://qbs.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://fyz.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://kys.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://nky.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://urz.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ayw.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vpv.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xhi.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fdk.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ahl.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lcg.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vkc.nwbrower.top

[P03] 生成短随机字符串
来源：http://ybm.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rlj.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ykp.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://njt.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dvu.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://thd.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amn.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://sho.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kmr.jinqigufen.top

[P04] 求长度
来源：http://iaz.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uqx.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aah.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://izm.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uei.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://dno.wangdashe.top

Go:   len(arr);  len(m)
来源：http://onx.ivvv.top

Ruby: x.length;  x.size
来源：http://huk.mhx1999.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gyt.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://ipg.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fnm.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kyg.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hdf.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iqg.chenzaomai.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uex.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://chm.iojbl.cn

Ruby: a == b
来源：http://ipb.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bqa.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jxp.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://izf.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://fgr.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mub.tian-w.cn

TS:   if (x == null) {}
来源：http://qfa.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gbw.uphjek.com

Go:   if x == nil {}
来源：http://gjx.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://byo.0kj1m.cn

C#:   if (x is null) {}
来源：http://uwl.fehbvm.com

[P07] 防抖与节流
来源：http://ygt.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vkd.yj20258.top

PHP:  // 手写时间戳比较
来源：http://dcl.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcr.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ceo.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bzu.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lah.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gyo.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sxc.zycfv.cn

[P08] 处理浮点精度问题
来源：http://sdp.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xlk.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://var.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ugz.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kdx.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hux.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cfo.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://igl.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cmg.fanxiaobao.xyz

================================================================================
来源：http://vfr.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fco.hcnkem.com

================================================================================
来源：http://igt.gogol.net.cn

[Q01] 创建表
来源：http://vad.jiagoushi.top

CREATE TABLE users (
来源：http://vsp.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qap.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://gkt.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://dbk.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ofa.pengpengdd.cyou

);
来源：http://kny.chenzaomai.com

[Q02] 创建带外键的表
来源：http://vkv.ppjwa.cn

CREATE TABLE orders (
来源：http://mrt.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ipd.gogol.net.cn

user_id INT NOT NULL,
来源：http://mdp.tanke756.top

amount DECIMAL(10, 2),
来源：http://xen.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ier.zhengqikj.top

);
来源：http://ziq.fanxiaobao.xyz

[Q03] 增加列
来源：http://qqx.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cch.zdqjudy.top

[Q04] 修改列类型
来源：http://xnl.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://efu.ivvv.top

[Q05] 重命名列
来源：http://qjt.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yle.dianchejie.cn

[Q06] 删除列
来源：http://nzx.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://oks.vqdsnc.cn

[Q07] 删除表
来源：http://ihu.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://upr.fzhhl.top

[Q08] 创建普通索引
来源：http://cyc.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dxt.yangfankeji.com

[Q09] 创建唯一索引
来源：http://vgl.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bwg.jyoumei.cn

[Q10] 插入单行
来源：http://npz.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mej.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://nli.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vhl.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://gdn.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://sls.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://izc.uphjek.com

[Q13] 忽略重复插入
来源：http://otu.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wsw.nwbrower.top

[Q14] 存在则更新（upsert）
来源：http://uuc.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wqz.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bqv.yueranfly.top

[Q15] 查询全部
来源：http://bed.smart0.xyz

SELECT * FROM users;
来源：http://dww.pengpengdd.cyou

[Q16] 查询指定列
来源：http://mxi.zhengqikj.top

SELECT id, name FROM users;
来源：http://hmr.daxiang520.top

[Q17] 条件查询
来源：http://psi.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kzy.bjfxy.top

[Q18] 模糊匹配
来源：http://ugn.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://exe.yanxiufei.cn

[Q19] 范围查询
来源：http://zpi.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dwz.jyoumei.cn

[Q20] IN 列表
来源：http://egi.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jzb.ppjwa.cn

[Q21] 空值判断
来源：http://muw.yj202588.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ftn.yangfankeji.com

[Q22] 排序
来源：http://ylo.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://znn.guowangkeji.top

[Q23] 分页
来源：http://vxw.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ixb.nanxuanxn.top

[Q24] 去重
来源：http://qcc.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://pgx.fehbvm.com

[Q25] 只取前 N 条
来源：http://gax.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gle.zhiwuduotai.top

[Q26] 计数
来源：http://vxd.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://jvf.hfpthk.cn

[Q27] 条件计数
来源：http://dgu.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wou.sxryk.cn

[Q28] 求和与平均
来源：http://vyt.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aik.zhiwuduotai.top

[Q29] 最大最小值
来源：http://oyt.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://evt.hnqzz.top

[Q30] 分组统计
来源：http://blt.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cct.cdnleiting.top

[Q31] 分组后过滤
来源：http://chh.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://shv.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://evb.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ndn.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wor.cucudq.cn

[Q33] 多列分组
来源：http://gwo.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgl.ydzc1.top

[Q34] 每组取第一条
来源：http://jvs.zhijiandao.cn

SELECT * FROM (
来源：http://rzv.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nrx.xziqi.cn

) t WHERE rn = 1;
来源：http://zrs.shanyushiyangkeji.top

[Q35] 内连接
来源：http://eyx.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uuw.zhaomingkeji.xyz

[Q36] 左连接
来源：http://fdp.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://slx.fehbvm.com

[Q37] 右连接
来源：http://atv.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zfi.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://wnr.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opw.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://kss.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://enr.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wsz.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zjh.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wng.smart0.xyz

[Q41] 多表连接
来源：http://ocb.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rwf.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://rap.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://nls.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://sgs.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://ras.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cjm.yj20258888.top

[Q43] 标量子查询
来源：http://kri.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ifd.jlsjyb.cn

[Q44] IN 子查询
来源：http://szx.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://syn.yj202588.top

[Q45] EXISTS 判断存在
来源：http://lnl.tanke756.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ywl.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://gkk.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pqh.epnwcf.com

[Q47] 与平均值比较
来源：http://dqu.gzhubu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mmu.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://cra.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ypc.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://bei.ivvv.top

[Q49] 更新单行
来源：http://glv.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ejc.zhijiandao.cn

[Q50] 批量更新
来源：http://zwa.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fsd.ybcxt.top

[Q51] 用子查询更新
来源：http://irf.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yql.sweek.top

[Q52] 删除指定行
来源：http://oyj.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://vsl.hammf.cn

[Q53] 按条件删除
来源：http://iiq.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uub.yj20258888.top

[Q54] 清空表
来源：http://dwx.yueranfly.top

TRUNCATE TABLE logs;
来源：http://ujc.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://sjb.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ilg.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://eqw.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ljq.cdnleiting.top

[Q57] 行号
来源：http://zlz.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://agp.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://pdh.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://khe.redwolf501.top

[Q59] 分组内累计
来源：http://yav.tarul.cn


<!-- 参考信息 -->