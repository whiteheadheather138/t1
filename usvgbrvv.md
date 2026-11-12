代发 wailian999

Py:   itertools.permutations(arr)
来源：http://gue.hywenlv.cn

PHP:  // 手写递归交换
来源：http://dyb.hcnkem.com

JS:   // 手写回溯递归
来源：http://nkm.dianchejie.cn

TS:   // 手写回溯递归
来源：http://qzd.tarul.cn

Java: // 手写回溯递归
来源：http://irn.dashuyun.cn

Go:   // 手写回溯递归
来源：http://jsl.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://vew.dianchejie.cn

C#:   // 手写回溯递归
来源：http://ppu.fktsv.cn

[N09] 栈与队列
来源：http://lgi.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tmn.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jtz.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bsm.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xsd.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yzy.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pep.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hoj.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kwr.meibo888.top

[N10] 链表节点定义
来源：http://ehi.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mrx.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ccs.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nbp.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ymt.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://hkg.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://leo.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oox.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ylg.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://lhv.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wke.zhengqikj.top

PHP:  // 手写递归函数
来源：http://sev.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qmv.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgo.nanxinkj.top

Java: // 手写递归
来源：http://hfc.vqdsnc.cn

Go:   // 手写递归
来源：http://geq.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rzg.9152youxi.cn

C#:   // 手写递归
来源：http://kkk.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://adh.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tpo.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wzt.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yvt.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://drc.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hmt.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ybw.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qkz.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jys.xingfuxueyuan.xyz

================================================================================
来源：http://avw.ydjk.org.cn

O. 并发与异步
来源：http://rol.tianlin.xyz

================================================================================
来源：http://nth.bjfxy.top

[O01] 启动一个线程
来源：http://nsj.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ehe.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hgr.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ekn.aizwys.cn

TS:   // 同 JS
来源：http://lsp.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://kpf.9152youxi.cn

Go:   go f()
来源：http://eot.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://ctn.cucudq.cn

C#:   Task.Run(() => F());
来源：http://gmj.yvedp.cn

[O02] 使用线程池
来源：http://opt.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mcc.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ogw.ydzc1.top

JS:   // worker_threads 线程池
来源：http://tln.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://xyi.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xja.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kcu.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ksc.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dtt.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://vuc.iojbl.cn

Py:   with lock: shared += 1
来源：http://bqz.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://exg.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://abg.jianghu66.top

TS:   // 同 JS
来源：http://zak.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://kzf.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kob.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qrp.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://jab.yongpay.top

[O04] 定义异步函数并等待
来源：http://ldz.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://uva.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://afi.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://xlj.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ddo.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xnp.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qrd.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://gyg.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://qnr.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://zxd.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://bhe.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yle.meibo888.top

JS:   await Promise.all(tasks)
来源：http://vpa.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://smr.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ypt.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sek.hcnkem.com

Ruby: threads.map(&:join)
来源：http://lmo.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pro.jqgfzy.top

[O06] 使用进程池
来源：http://oun.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qtt.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iwo.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://idt.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://edp.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jxk.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cye.fengsongda.top

Ruby: // fork 块
来源：http://gvx.gzhubu.top

C#:   Parallel.For
来源：http://ulu.wangdashe.top

================================================================================
来源：http://ten.tarul.cn

P. 常用工具函数
来源：http://cgu.wangdashe.top

================================================================================
来源：http://pie.svipenyu.cn

[P01] 生成 UUID
来源：http://vbb.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://uax.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://esf.uphjek.com

JS:   crypto.randomUUID()
来源：http://jbf.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://tia.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://xzx.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://wfs.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://yks.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://lpw.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://pdn.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kqq.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mmv.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pyq.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ykz.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qaf.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zhu.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hju.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bnb.hesvh.cn

[P03] 生成短随机字符串
来源：http://ale.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uum.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://whg.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wev.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lbv.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hor.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nts.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kos.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xdo.dashuyun.cn

[P04] 求长度
来源：http://whd.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ude.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://agv.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qrx.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kcn.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://mck.nwbrower.top

Go:   len(arr);  len(m)
来源：http://ucz.redwolf501.top

Ruby: x.length;  x.size
来源：http://qnl.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pcv.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://uim.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://agn.tianlin.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kav.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zxa.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fli.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ftr.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://iyt.uphjek.com

Ruby: a == b
来源：http://lpr.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://haw.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qve.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ugu.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://dac.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://srq.jianghu66.top

TS:   if (x == null) {}
来源：http://cqg.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hii.shangyingyoupin.top

Go:   if x == nil {}
来源：http://oiy.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lsx.sysykeji.top

C#:   if (x is null) {}
来源：http://hva.uphjek.com

[P07] 防抖与节流
来源：http://fnw.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inq.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://wfu.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cck.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://egr.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cxz.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jtw.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sbq.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://njh.tian-w.cn

[P08] 处理浮点精度问题
来源：http://gld.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kct.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xcp.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yxy.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xye.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jmq.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cax.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://znf.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jgb.yueranfly.top

================================================================================
来源：http://tfw.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ojm.hywenlv.cn

================================================================================
来源：http://uih.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://pyx.tianlin.xyz

CREATE TABLE users (
来源：http://ewl.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qce.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://wce.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://mvu.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bee.hfpthk.cn

);
来源：http://bod.haohaochexian.top

[Q02] 创建带外键的表
来源：http://evv.shangyingyoupin.top

CREATE TABLE orders (
来源：http://zuw.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zar.jqgfzy.top

user_id INT NOT NULL,
来源：http://dcx.epnwcf.com

amount DECIMAL(10, 2),
来源：http://lyl.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nxj.zhijiandao.cn

);
来源：http://sxr.9152youxi.cn

[Q03] 增加列
来源：http://asy.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ary.hammf.cn

[Q04] 修改列类型
来源：http://wnj.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yxz.meibo888.top

[Q05] 重命名列
来源：http://ibb.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://byi.hcnkem.com

[Q06] 删除列
来源：http://kbt.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://eii.yj20258888.top

[Q07] 删除表
来源：http://bcd.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://vwt.guowangkeji.top

[Q08] 创建普通索引
来源：http://iqd.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://esp.shzxlz.cn

[Q09] 创建唯一索引
来源：http://hot.pengpengdd.cyou

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hzy.cqqwz.cn

[Q10] 插入单行
来源：http://jic.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pjb.yangfankeji.com

[Q11] 一次插入多行
来源：http://klf.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hav.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://osz.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://sxf.ehwqpu.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zua.dianchejie.cn

[Q13] 忽略重复插入
来源：http://rab.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tfm.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://fcc.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jsx.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://osb.yangfankeji.com

[Q15] 查询全部
来源：http://opp.yj20258888.top

SELECT * FROM users;
来源：http://qnu.hfpthk.cn

[Q16] 查询指定列
来源：http://bjk.mhx1999.top

SELECT id, name FROM users;
来源：http://rkj.jinqigufen.top

[Q17] 条件查询
来源：http://emq.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pyy.0kj1m.cn

[Q18] 模糊匹配
来源：http://olg.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://drx.kuanghao11.cn

[Q19] 范围查询
来源：http://nrg.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aip.tanke756.top

[Q20] IN 列表
来源：http://pen.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vfc.tianlin.xyz

[Q21] 空值判断
来源：http://cta.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gsz.wangshuangyany.cn

[Q22] 排序
来源：http://mpu.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://coj.tanke756.top

[Q23] 分页
来源：http://rjg.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iuj.jiagoushi.top

[Q24] 去重
来源：http://mce.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://xuc.fzhhl.top

[Q25] 只取前 N 条
来源：http://hxa.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oli.nanxuanxn.top

[Q26] 计数
来源：http://glj.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://cdy.yangfankeji.com

[Q27] 条件计数
来源：http://iyl.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xdy.jinyuanbaomall.cn

[Q28] 求和与平均
来源：http://com.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jkd.c1oappe.top

[Q29] 最大最小值
来源：http://mip.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hji.vehdjk.com

[Q30] 分组统计
来源：http://yon.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qyw.tarul.cn

[Q31] 分组后过滤
来源：http://jbz.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ycf.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://hpc.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://irc.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ree.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://ldg.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://apm.tanke756.top

[Q34] 每组取第一条
来源：http://rnx.nanxuanxn.top

SELECT * FROM (
来源：http://rhp.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jbr.zycfv.cn

) t WHERE rn = 1;
来源：http://fci.hnxiangtu.top

[Q35] 内连接
来源：http://lfs.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mva.jyoumei.cn

[Q36] 左连接
来源：http://por.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vgx.yvedp.cn

[Q37] 右连接
来源：http://xqs.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bqx.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dvx.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gtb.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://jbb.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cue.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dhn.tianlin.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://fmo.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fxs.guowangkeji.top

[Q41] 多表连接
来源：http://ust.hcnkem.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://pdn.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://uud.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://pyw.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://vde.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://lld.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jts.daria6918.cn

[Q43] 标量子查询
来源：http://dww.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lqm.zycfv.cn

[Q44] IN 子查询
来源：http://xdc.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fjn.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://erm.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cxn.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://tfi.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fop.dianchejie.cn

[Q47] 与平均值比较
来源：http://zcs.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bll.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://ggl.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jyu.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://yvh.jiagoushi.top

[Q49] 更新单行
来源：http://jbj.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://knx.tian-w.cn

[Q50] 批量更新
来源：http://sfn.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://txm.tian-w.cn

[Q51] 用子查询更新
来源：http://idp.jlsjyb.cn


<!-- 参考信息 -->