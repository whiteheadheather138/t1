代发 wailian999

Java: // 手写回溯递归
来源：http://lea.hysaishi.cn

Go:   // 手写回溯递归
来源：http://okq.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://dvi.yueranfly.top

C#:   // 手写回溯递归
来源：http://gqq.hesvh.cn

[N09] 栈与队列
来源：http://sas.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iig.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bcw.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lgr.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmv.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wav.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nam.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://shb.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgp.yuanzhike.top

[N10] 链表节点定义
来源：http://okc.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ynv.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yde.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blc.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqy.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://gap.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://maa.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wyc.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mga.meibo888.top

[N11] 二叉树中序遍历
来源：http://wcm.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uwy.iojbl.cn

PHP:  // 手写递归函数
来源：http://pjt.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xyn.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sne.mhx1999.top

Java: // 手写递归
来源：http://ajo.vehdjk.com

Go:   // 手写递归
来源：http://izx.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ocs.xziqi.cn

C#:   // 手写递归
来源：http://mxv.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oji.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bfm.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sre.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ups.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kkc.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rwk.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wqf.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sql.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://psd.aizwys.cn

================================================================================
来源：http://tny.dianchejie.cn

O. 并发与异步
来源：http://hgd.zdbjq.cn

================================================================================
来源：http://wbs.jqgfzy.top

[O01] 启动一个线程
来源：http://erd.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pzu.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cyr.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mhc.jiagoushi.top

TS:   // 同 JS
来源：http://btc.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://edk.zhijiandao.cn

Go:   go f()
来源：http://hlj.xinyue.icu

Ruby: Thread.new { f }
来源：http://zmj.gzhubu.top

C#:   Task.Run(() => F());
来源：http://sxm.yuanzhike.top

[O02] 使用线程池
来源：http://lrl.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iza.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xwd.andypj.xyz

JS:   // worker_threads 线程池
来源：http://lyk.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://ybe.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://twk.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zqz.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rrt.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eia.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://vzo.hfpthk.cn

Py:   with lock: shared += 1
来源：http://awh.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://yxr.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pwe.gogol.net.cn

TS:   // 同 JS
来源：http://pfh.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://ewu.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vvu.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cjf.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ken.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://nem.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://cga.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://crw.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://ksx.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rdi.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vvd.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://erd.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://cei.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://jdr.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://cdl.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://uxn.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dbf.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://kgu.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://ogo.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vte.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhm.sxryk.cn

Ruby: threads.map(&:join)
来源：http://nar.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tkd.yuxming.cn

[O06] 使用进程池
来源：http://klt.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dcc.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ypp.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://jqk.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://and.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tqa.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hav.cheryme.top

Ruby: // fork 块
来源：http://nmh.xuetiantiany.cn

C#:   Parallel.For
来源：http://stg.yj202588.top

================================================================================
来源：http://miy.cashguo.top

P. 常用工具函数
来源：http://gqf.jiagoushi.top

================================================================================
来源：http://vao.epnwcf.com

[P01] 生成 UUID
来源：http://rlh.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://ukp.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://emi.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://qnk.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://dzu.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://ukh.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://qan.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://mph.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://gmf.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://zsp.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xxq.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ute.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aqy.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ker.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xqy.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pby.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhi.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ycz.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://lha.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jlq.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kyl.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gcg.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qdb.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ksz.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ohi.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ejc.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rwt.feifeiyinyue.top

[P04] 求长度
来源：http://gag.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kno.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzb.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwm.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qwp.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://hfq.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://shj.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://gcw.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://vuc.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://hvf.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bas.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jzx.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wxn.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ioj.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://epf.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://tvm.redwolf501.top

Ruby: a == b
来源：http://wlf.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wbk.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wml.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://avx.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://lpa.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://brm.vqdsnc.cn

TS:   if (x == null) {}
来源：http://ygq.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rbt.xuanzx.com

Go:   if x == nil {}
来源：http://wde.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xbp.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://rdc.fengsongda.top

[P07] 防抖与节流
来源：http://bii.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jja.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://qyr.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swz.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnw.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://llp.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xac.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://oqj.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ilq.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://xdi.ivvv.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rhg.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://waa.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mke.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vza.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tqv.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eei.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://djg.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ppe.zhongyouzk.top

================================================================================
来源：http://sau.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wky.wangshuangyany.cn

================================================================================
来源：http://oyd.ywan-chungtsiang.top

[Q01] 创建表
来源：http://fdl.ehwqpu.com

CREATE TABLE users (
来源：http://txo.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wco.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://jbz.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://tjr.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ive.meibo888.top

);
来源：http://fcx.gzhubu.top

[Q02] 创建带外键的表
来源：http://iap.xziqi.cn

CREATE TABLE orders (
来源：http://qyt.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kfe.haohaochexian.top

user_id INT NOT NULL,
来源：http://tlf.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://amr.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gsh.ehwqpu.com

);
来源：http://sxp.yvedp.cn

[Q03] 增加列
来源：http://gsq.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wvm.xinyue.icu

[Q04] 修改列类型
来源：http://qgq.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kiy.yongpay.top

[Q05] 重命名列
来源：http://feb.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://udi.gaohongyu789.top

[Q06] 删除列
来源：http://awz.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rqr.jianghu66.top

[Q07] 删除表
来源：http://hpw.gogol.net.cn

DROP TABLE IF EXISTS orders;
来源：http://ugm.tanke756.top

[Q08] 创建普通索引
来源：http://nwa.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://zdv.haohaochexian.top

[Q09] 创建唯一索引
来源：http://efz.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://caw.ybcxt.top

[Q10] 插入单行
来源：http://zuq.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vrd.guannengcc.top

[Q11] 一次插入多行
来源：http://qua.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bnd.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://gwm.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://joq.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rkc.smart0.xyz

[Q13] 忽略重复插入
来源：http://fsx.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fmq.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://bsf.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sjl.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qld.zhixingplan.top

[Q15] 查询全部
来源：http://gjc.hnqzz.top

SELECT * FROM users;
来源：http://avz.ydjk.org.cn

[Q16] 查询指定列
来源：http://fmm.hcnkem.com

SELECT id, name FROM users;
来源：http://fmh.daria6918.cn

[Q17] 条件查询
来源：http://usl.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mxc.daria6918.cn

[Q18] 模糊匹配
来源：http://iuz.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oar.nwbrower.top

[Q19] 范围查询
来源：http://kns.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sax.gaohongyu789.top

[Q20] IN 列表
来源：http://uhj.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tbm.smart0.xyz

[Q21] 空值判断
来源：http://kth.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ywd.tanke756.top

[Q22] 排序
来源：http://eyt.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pyt.zhongyouzk.top

[Q23] 分页
来源：http://gwf.ivvv.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nzv.cucudq.cn

[Q24] 去重
来源：http://ggu.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://lue.pycfn.com

[Q25] 只取前 N 条
来源：http://orv.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pvg.yongpay.top

[Q26] 计数
来源：http://doi.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://scf.gzhubu.top

[Q27] 条件计数
来源：http://icy.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aho.fehbvm.com

[Q28] 求和与平均
来源：http://uhk.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cqu.birdmap.top

[Q29] 最大最小值
来源：http://swj.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cvf.cheryme.top

[Q30] 分组统计
来源：http://oaq.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sjs.c1oappe.top

[Q31] 分组后过滤
来源：http://sfs.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://odb.zhaomingkeji.xyz

[Q32] 分组拼接字符串
来源：http://zrv.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ueh.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kwm.dashuyun.cn

[Q33] 多列分组
来源：http://ljz.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yfn.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://soh.chenjidiqi.icu

SELECT * FROM (
来源：http://urd.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aks.cashguo.top

) t WHERE rn = 1;
来源：http://wga.pengpengdd.cyou

[Q35] 内连接
来源：http://mks.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mrj.tanke756.top

[Q36] 左连接
来源：http://sdl.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://paw.xuetiantiany.cn

[Q37] 右连接
来源：http://glc.yj202588.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tmp.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://wdd.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pah.yongpay.top

[Q39] 自连接（查上下级）
来源：http://gch.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vee.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xtb.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lzj.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pel.smart0.xyz

[Q41] 多表连接
来源：http://hjc.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gjp.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://duy.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://zsr.cheryme.top

[Q42] 连接条件附加过滤
来源：http://gls.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://utf.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gmz.shzxlz.cn

[Q43] 标量子查询
来源：http://cur.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ehy.jiagoushi.top

[Q44] IN 子查询
来源：http://iwk.snrcjt.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://czp.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://tpq.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jba.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jpd.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fvc.uphjek.com

[Q47] 与平均值比较
来源：http://wtp.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ukg.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://sdx.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rck.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://znh.cqqwz.cn

[Q49] 更新单行
来源：http://ogl.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ozn.yueranfly.top

[Q50] 批量更新
来源：http://cfc.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gky.snrcjt.cn

[Q51] 用子查询更新
来源：http://byv.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gpc.yanxiufei.cn

[Q52] 删除指定行
来源：http://vsy.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://hvq.gzhubu.top

[Q53] 按条件删除
来源：http://pcf.tarul.cn


<!-- 参考信息 -->