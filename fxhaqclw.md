代发 wailian999

Java: // 手写回溯递归
来源：http://eoj.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://pnw.pycfn.com

Ruby: arr.permutation.to_a
来源：http://ziv.yj20258888.top

C#:   // 手写回溯递归
来源：http://lve.guannengcc.top

[N09] 栈与队列
来源：http://wid.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bwe.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://myh.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xyv.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://srv.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cca.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qfz.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iuk.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qvj.smart0.xyz

[N10] 链表节点定义
来源：http://svz.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lhk.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zhi.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dqe.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cot.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://rsb.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qbs.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qrn.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vln.bjfxy.top

[N11] 二叉树中序遍历
来源：http://ytc.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pfu.fengsongda.top

PHP:  // 手写递归函数
来源：http://umz.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfw.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cbk.epnwcf.com

Java: // 手写递归
来源：http://qeu.zdbjq.cn

Go:   // 手写递归
来源：http://duw.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tqz.uphjek.com

C#:   // 手写递归
来源：http://vsw.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qie.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qyz.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://omn.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://onv.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iwa.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hsx.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mgp.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ufr.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://luv.fehbvm.com

================================================================================
来源：http://dnp.havefunace.top

O. 并发与异步
来源：http://ewb.jqgufenzy.top

================================================================================
来源：http://eyz.yanxiufei.cn

[O01] 启动一个线程
来源：http://kcr.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hcc.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ptc.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://neq.pycfn.com

TS:   // 同 JS
来源：http://cqp.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://bkz.redwolf501.top

Go:   go f()
来源：http://aac.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://hub.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://vog.epnwcf.com

[O02] 使用线程池
来源：http://zsc.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://beq.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xip.pycfn.com

JS:   // worker_threads 线程池
来源：http://sxn.uphjek.com

TS:   // worker_threads 线程池
来源：http://ktu.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://smr.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rvs.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iyd.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qrm.mhx1999.top

[O03] 加锁保护共享数据
来源：http://feu.zycfv.cn

Py:   with lock: shared += 1
来源：http://bsp.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://uae.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mch.hnxiangtu.top

TS:   // 同 JS
来源：http://blc.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://syl.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hri.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://kid.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://occ.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://uoe.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://lbz.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hsk.uphjek.com

JS:   async function f() { await g(); }
来源：http://fex.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://bzf.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://apx.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://now.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://uxz.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://wfs.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://geg.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://ivu.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bae.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://ldo.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://rer.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlv.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://htk.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://ezp.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://upk.hongshengwenyu.top

[O06] 使用进程池
来源：http://xdo.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qgt.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ydg.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://dgg.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://utw.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nyh.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pdy.zhiwuduotai.top

Ruby: // fork 块
来源：http://nhz.havefunace.top

C#:   Parallel.For
来源：http://hwl.ivvv.top

================================================================================
来源：http://cld.bjfxy.top

P. 常用工具函数
来源：http://vub.yj202588.top

================================================================================
来源：http://fsc.ydzc1.top

[P01] 生成 UUID
来源：http://mvx.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://whn.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nbb.ydzc1.top

JS:   crypto.randomUUID()
来源：http://vkm.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://qjr.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://kca.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://vlc.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://xri.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://cre.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://upx.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sll.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://atw.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ccr.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mdy.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tuy.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wki.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mqi.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lnf.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://ims.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fyz.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mph.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bgv.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pgt.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mqi.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zna.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://utr.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pvy.daria6918.cn

[P04] 求长度
来源：http://amn.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gsk.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rhe.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lhn.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmt.52xcode.cn

Java: list.size();  map.size();  s.length()
来源：http://ffi.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://knl.ydzc1.top

Ruby: x.length;  x.size
来源：http://tgu.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dva.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://fpr.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mtp.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fwb.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xmh.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eyo.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zsn.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mjv.ybcxt.top

Ruby: a == b
来源：http://ykf.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fnc.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://all.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ztb.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://xzv.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hjl.svipenyu.cn

TS:   if (x == null) {}
来源：http://nkq.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ssj.yj20258888.top

Go:   if x == nil {}
来源：http://kuz.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ifq.iojbl.cn

C#:   if (x is null) {}
来源：http://xhk.shzxlz.cn

[P07] 防抖与节流
来源：http://qiv.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pvl.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://gso.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcq.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpy.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hdg.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jhz.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://opn.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tri.hcnkem.com

[P08] 处理浮点精度问题
来源：http://swn.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hag.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xay.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lys.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mcv.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://inh.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kqc.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mvt.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ntq.tian-w.cn

================================================================================
来源：http://pzy.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qie.cheryme.top

================================================================================
来源：http://ppz.zhongyouzk.top

[Q01] 创建表
来源：http://ham.sysykeji.top

CREATE TABLE users (
来源：http://eor.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ngb.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://hwo.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://opt.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://seb.daria6918.cn

);
来源：http://iel.xingfuxueyuan.xyz

[Q02] 创建带外键的表
来源：http://kgw.c1oappe.top

CREATE TABLE orders (
来源：http://dsz.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyc.tian-w.cn

user_id INT NOT NULL,
来源：http://dty.yonumen.top

amount DECIMAL(10, 2),
来源：http://dsg.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xhm.jiagoushi.top

);
来源：http://vra.ydjk.org.cn

[Q03] 增加列
来源：http://bel.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uhq.feifeiyinyue.top

[Q04] 修改列类型
来源：http://ahf.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wam.jinqigfzy.top

[Q05] 重命名列
来源：http://eke.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vwp.feifeiyinyue.top

[Q06] 删除列
来源：http://njt.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://leg.shanyushiyangtech.top

[Q07] 删除表
来源：http://ald.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://xyd.redwolf501.top

[Q08] 创建普通索引
来源：http://crz.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bar.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://qvl.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wtv.ctjpmb.com

[Q10] 插入单行
来源：http://xvt.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vmt.uphjek.com

[Q11] 一次插入多行
来源：http://tms.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qqf.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://hyc.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://xbt.yueranfly.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bsp.aizwys.cn

[Q13] 忽略重复插入
来源：http://bay.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rtu.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://tmk.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sfw.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aoh.hammf.cn

[Q15] 查询全部
来源：http://xtm.guannengcc.top

SELECT * FROM users;
来源：http://odm.zhijiandao.cn

[Q16] 查询指定列
来源：http://rwb.fehbvm.com

SELECT id, name FROM users;
来源：http://ejf.hcnkem.com

[Q17] 条件查询
来源：http://len.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xrt.zhoulong.xyz

[Q18] 模糊匹配
来源：http://pog.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rsl.yangfankeji.com

[Q19] 范围查询
来源：http://kpi.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://knn.pengpengdd.cyou

[Q20] IN 列表
来源：http://oir.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rfe.ehwqpu.com

[Q21] 空值判断
来源：http://crw.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://leh.zhongyouzk.top

[Q22] 排序
来源：http://ead.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gyw.yongpay.top

[Q23] 分页
来源：http://ihu.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eoo.tian-w.cn

[Q24] 去重
来源：http://xbi.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://tif.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://olt.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tak.chenzaomai.com

[Q26] 计数
来源：http://hxp.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://xpa.jlsjyb.cn

[Q27] 条件计数
来源：http://eap.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lbs.jyoumei.cn

[Q28] 求和与平均
来源：http://ghw.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yvr.jianghu66.top

[Q29] 最大最小值
来源：http://ctv.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lgf.jianghu66.top

[Q30] 分组统计
来源：http://vyl.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ssc.gzhubu.top

[Q31] 分组后过滤
来源：http://bsf.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pqh.havefunace.top

[Q32] 分组拼接字符串
来源：http://icu.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uyl.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzn.yj20258888.top

[Q33] 多列分组
来源：http://qqa.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cle.ivvv.top

[Q34] 每组取第一条
来源：http://kip.kuanghao11.cn

SELECT * FROM (
来源：http://eqm.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://znp.jianghu66.top

) t WHERE rn = 1;
来源：http://jzj.fktsv.cn

[Q35] 内连接
来源：http://myo.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fkb.yongpay.top

[Q36] 左连接
来源：http://otf.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://scf.zhixingplan.top

[Q37] 右连接
来源：http://xmt.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rnd.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://gkl.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sae.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://bos.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://udi.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fap.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://exh.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dfp.xylfe.cn

[Q41] 多表连接
来源：http://cmz.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bba.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://zaf.aibaodan.cn

JOIN products p ON p.id = o.product_id;
来源：http://jea.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://jso.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://bil.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qmd.c1oappe.top

[Q43] 标量子查询
来源：http://eni.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mzy.nwbrower.top

[Q44] IN 子查询
来源：http://raq.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bwb.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://mhd.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vkt.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://viv.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ctm.zhijiandao.cn

[Q47] 与平均值比较
来源：http://zzi.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sft.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://qae.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://npf.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://eoc.jlsjyb.cn

[Q49] 更新单行
来源：http://hhp.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hcz.zhiwuduotai.top

[Q50] 批量更新
来源：http://ewv.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftb.aibaodan.cn

[Q51] 用子查询更新
来源：http://xwt.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pbq.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://gqa.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://muc.redwolf501.top

[Q53] 按条件删除
来源：http://sbw.cucudq.cn


<!-- 参考信息 -->