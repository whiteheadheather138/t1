代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://flz.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://idx.zycfv.cn

Py:   s == s[::-1]
来源：http://uwv.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://aqz.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://bkf.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://nes.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://soe.tanke756.top

Go:   // 双指针从两端比较
来源：http://xsk.jlsjyb.cn

Ruby: s == s.reverse
来源：http://fyb.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rve.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://dru.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bvm.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wkx.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lfr.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://kum.yueranfly.top

Java: // 手写 HashMap
来源：http://uqo.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://ftf.hywenlv.cn

Ruby: // 手写 Hash
来源：http://wgg.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zua.jianghu66.top

[N08] 生成全排列
来源：http://bfc.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://xmr.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://dbp.zycfv.cn

JS:   // 手写回溯递归
来源：http://xcp.yfazqb.com

TS:   // 手写回溯递归
来源：http://bao.nwbrower.top

Java: // 手写回溯递归
来源：http://nkd.vehdjk.com

Go:   // 手写回溯递归
来源：http://mvf.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://aou.hammf.cn

C#:   // 手写回溯递归
来源：http://wbr.zhongyouzk.top

[N09] 栈与队列
来源：http://cbi.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rew.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hll.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dmj.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ugi.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dbz.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xct.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ypk.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://whs.cucudq.cn

[N10] 链表节点定义
来源：http://amc.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jef.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://huf.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lpe.zhongyouzk.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://brd.cashguo.top

Java: class Node { int v; Node next; }
来源：http://tqh.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://eeo.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ejw.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bfb.wangdashe.top

[N11] 二叉树中序遍历
来源：http://nnn.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hup.wangdashe.top

PHP:  // 手写递归函数
来源：http://vnb.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xpw.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zde.iojbl.cn

Java: // 手写递归
来源：http://pqv.jianghu66.top

Go:   // 手写递归
来源：http://dlj.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dhq.xziqi.cn

C#:   // 手写递归
来源：http://uhi.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gxe.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iqh.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pex.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnh.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ftm.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ckf.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://thj.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wbl.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rct.birdmap.top

================================================================================
来源：http://aqi.aibaodan.cn

O. 并发与异步
来源：http://eif.ehwqpu.com

================================================================================
来源：http://qlv.xinyue.icu

[O01] 启动一个线程
来源：http://jwp.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ihp.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rox.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tgf.jlsjyb.cn

TS:   // 同 JS
来源：http://rns.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://rbt.jqgufenzy.top

Go:   go f()
来源：http://zmn.iojbl.cn

Ruby: Thread.new { f }
来源：http://wra.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://uvh.sweek.top

[O02] 使用线程池
来源：http://wlr.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pcr.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://unn.cheryme.top

JS:   // worker_threads 线程池
来源：http://nnn.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://jwz.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://wct.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oom.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jaz.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uqc.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://zxy.52xcode.cn

Py:   with lock: shared += 1
来源：http://gbu.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://sun.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://apb.xuanzx.com

TS:   // 同 JS
来源：http://dew.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://odz.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fmp.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zse.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://voz.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://mad.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://xsh.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://asq.yongpay.top

JS:   async function f() { await g(); }
来源：http://zht.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zgb.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xoq.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zyi.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pnb.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://cic.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://kmi.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://xgl.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gvh.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://qwv.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://ccf.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uvc.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nll.cashguo.top

Ruby: threads.map(&:join)
来源：http://umw.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ymm.vqdsnc.cn

[O06] 使用进程池
来源：http://ets.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hff.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zlq.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://hqo.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://lac.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zno.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bjh.meibo888.top

Ruby: // fork 块
来源：http://mqs.fehbvm.com

C#:   Parallel.For
来源：http://rkk.ivvv.top

================================================================================
来源：http://ctg.shzxlz.cn

P. 常用工具函数
来源：http://rpz.jqgfzy.top

================================================================================
来源：http://amh.zhongyouzk.top

[P01] 生成 UUID
来源：http://nfm.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://lox.epnwcf.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mib.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://zfk.bjfxy.top

TS:   crypto.randomUUID()
来源：http://uof.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://ymq.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://vpz.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://ejw.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://bgt.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://nqu.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cnd.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ilu.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ntk.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sbw.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qms.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uxg.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mzc.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kso.ydzc1.top

[P03] 生成短随机字符串
来源：http://ulg.xinyue.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nmk.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tcg.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vla.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://emk.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cnz.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://spe.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cxx.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eub.hfpthk.cn

[P04] 求长度
来源：http://iop.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fng.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvx.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nyh.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dff.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://zcd.birdmap.top

Go:   len(arr);  len(m)
来源：http://yio.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://swq.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mog.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://ryc.mhx1999.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bao.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zuo.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jae.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uan.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ixc.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://yon.guowangkeji.top

Ruby: a == b
来源：http://urz.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://obk.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rhz.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ztn.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://iyh.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://njl.tarul.cn

TS:   if (x == null) {}
来源：http://ubg.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cbr.sxryk.cn

Go:   if x == nil {}
来源：http://ewg.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yob.yueranfly.top

C#:   if (x is null) {}
来源：http://xgr.andypj.xyz

[P07] 防抖与节流
来源：http://jrc.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://svq.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://eld.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pmf.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hdm.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nzc.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lzr.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://voa.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sqj.gaohongyu789.top

[P08] 处理浮点精度问题
来源：http://wjo.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ynv.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://png.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mvn.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hgs.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://das.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oem.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iot.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qlb.hongshengwenyu.top

================================================================================
来源：http://zuy.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://voo.cdnleiting.top

================================================================================
来源：http://vps.tanke756.top

[Q01] 创建表
来源：http://mis.c1oappe.top

CREATE TABLE users (
来源：http://zxh.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ytk.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://evs.jqgfzy.top

email VARCHAR(100) UNIQUE,
来源：http://ely.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jpl.yvedp.cn

);
来源：http://opp.xylfe.cn

[Q02] 创建带外键的表
来源：http://odb.dashuyun.cn

CREATE TABLE orders (
来源：http://zny.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxp.redwolf501.top

user_id INT NOT NULL,
来源：http://oql.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://zjw.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yhz.sysykeji.top

);
来源：http://rng.cashguo.top

[Q03] 增加列
来源：http://mij.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kkj.snrcjt.cn

[Q04] 修改列类型
来源：http://ssb.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rmp.sjlbkw.cn

[Q05] 重命名列
来源：http://gwk.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sgo.dashuyun.cn

[Q06] 删除列
来源：http://ptp.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://pex.pycfn.com

[Q07] 删除表
来源：http://nrq.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://hzl.jinqigufen.top

[Q08] 创建普通索引
来源：http://rdf.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://zrz.hammf.cn

[Q09] 创建唯一索引
来源：http://buz.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mer.chenzaomai.com

[Q10] 插入单行
来源：http://lmp.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vde.zhongyouzk.top

[Q11] 一次插入多行
来源：http://dxn.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://juo.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://sxw.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://yek.shuidangran.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wqm.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://ncy.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pxh.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://jra.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://chx.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ytf.shanyushiyangtech.top

[Q15] 查询全部
来源：http://fdm.hongshengwenyu.top

SELECT * FROM users;
来源：http://ycl.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://exb.meibo888.top

SELECT id, name FROM users;
来源：http://ngf.gaohongyu789.top

[Q17] 条件查询
来源：http://wmd.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://azy.yfazqb.com

[Q18] 模糊匹配
来源：http://scb.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vqo.nanxinkj.top

[Q19] 范围查询
来源：http://bon.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mbi.quarkkingdee.top

[Q20] IN 列表
来源：http://rrj.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pah.zhongyouzk.top

[Q21] 空值判断
来源：http://cng.iojbl.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eja.cucudq.cn

[Q22] 排序
来源：http://mep.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yey.jinyuanbaomall.cn

[Q23] 分页
来源：http://cxr.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gix.jqgufenzy.top

[Q24] 去重
来源：http://ykr.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://tba.xziqi.cn

[Q25] 只取前 N 条
来源：http://ofd.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pxn.pengpengdd.cyou

[Q26] 计数
来源：http://lhf.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://nln.meibo888.top

[Q27] 条件计数
来源：http://roh.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yhj.ehwqpu.com

[Q28] 求和与平均
来源：http://wbd.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tjk.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://gcs.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iwx.wangdashe.top

[Q30] 分组统计
来源：http://eaq.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vuy.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://qyi.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gfi.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://tcf.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rko.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://icy.mhx1999.top

[Q33] 多列分组
来源：http://ssq.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kma.zhengqikj.top

[Q34] 每组取第一条
来源：http://cmi.cucudq.cn

SELECT * FROM (
来源：http://oxw.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://voh.cheryme.top

) t WHERE rn = 1;
来源：http://hqh.mhx1999.top

[Q35] 内连接
来源：http://zva.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hwe.chenlongwang.top

[Q36] 左连接
来源：http://hjt.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mhg.fehbvm.com

[Q37] 右连接
来源：http://adi.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvx.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kkw.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rie.tanke756.top

[Q39] 自连接（查上下级）
来源：http://scm.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://adn.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cbz.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qfd.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mlj.gaohongyu789.top

[Q41] 多表连接
来源：http://cjc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dab.epnwcf.com

JOIN users u ON u.id = o.user_id
来源：http://nlg.quarkkingdee.top

JOIN products p ON p.id = o.product_id;
来源：http://uxe.cheryme.top

[Q42] 连接条件附加过滤
来源：http://jdg.zhaomingkeji.xyz


<!-- 参考信息 -->