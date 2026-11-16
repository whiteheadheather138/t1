代发 wailian999

Ruby: s == s.reverse
来源：http://tsc.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yip.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://qee.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mjd.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uvf.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jge.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://fna.snrcjt.cn

Java: // 手写 HashMap
来源：http://sfn.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://ecu.fzhhl.top

Ruby: // 手写 Hash
来源：http://fpw.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eve.jinqigfzy.top

[N08] 生成全排列
来源：http://lyu.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://nct.hnqzz.top

PHP:  // 手写递归交换
来源：http://ybq.fktsv.cn

JS:   // 手写回溯递归
来源：http://uhd.hammf.cn

TS:   // 手写回溯递归
来源：http://coy.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://vel.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://pdi.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://toa.smart0.xyz

C#:   // 手写回溯递归
来源：http://fnn.xinyue.icu

[N09] 栈与队列
来源：http://uni.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rva.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lzr.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfb.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://act.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pum.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://scx.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yhd.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fcv.sysykeji.top

[N10] 链表节点定义
来源：http://izc.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zmb.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wrh.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yyx.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mee.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://afn.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cww.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://efy.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lcz.pycfn.com

[N11] 二叉树中序遍历
来源：http://nkt.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bnx.bjfxy.top

PHP:  // 手写递归函数
来源：http://ckv.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbp.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgq.zhixingplan.top

Java: // 手写递归
来源：http://skq.hongshengwenyu.top

Go:   // 手写递归
来源：http://vlw.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mxg.tanke756.top

C#:   // 手写递归
来源：http://wyv.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dmo.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xoe.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uav.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ufr.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ikv.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tfu.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyh.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://suf.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uaj.snrcjt.cn

================================================================================
来源：http://ygl.ehwqpu.com

O. 并发与异步
来源：http://kbd.chenzaomai.com

================================================================================
来源：http://hlb.dianchejie.cn

[O01] 启动一个线程
来源：http://cal.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qdh.tanke756.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ssa.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://azc.daxiang520.top

TS:   // 同 JS
来源：http://crz.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://nhl.shzxlz.cn

Go:   go f()
来源：http://uff.cucudq.cn

Ruby: Thread.new { f }
来源：http://ihf.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://ngj.ppjwa.cn

[O02] 使用线程池
来源：http://qvx.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gsa.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fep.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://blf.smart0.xyz

TS:   // worker_threads 线程池
来源：http://dvm.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://okf.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://etf.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://esr.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wjv.uphjek.com

[O03] 加锁保护共享数据
来源：http://zzq.dashuyun.cn

Py:   with lock: shared += 1
来源：http://rap.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://ppo.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hzt.cdnleiting.top

TS:   // 同 JS
来源：http://ssf.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://ioa.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gsk.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jhi.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://cui.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://xfo.tarul.cn

Py:   async def f():⏎    await g()
来源：http://nga.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eew.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://rkh.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwn.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uxb.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qtu.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dtf.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://mhx.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://yzn.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://nkr.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wic.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://xlh.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://ooa.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqw.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pcs.smart0.xyz

Ruby: threads.map(&:join)
来源：http://biw.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://frw.ybcxt.top

[O06] 使用进程池
来源：http://qfe.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gcr.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yca.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://qbv.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://qaz.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pog.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yve.52xcode.cn

Ruby: // fork 块
来源：http://yty.hesvh.cn

C#:   Parallel.For
来源：http://pfv.ybcxt.top

================================================================================
来源：http://lej.aizwys.cn

P. 常用工具函数
来源：http://nwc.ybcxt.top

================================================================================
来源：http://vtn.smart0.xyz

[P01] 生成 UUID
来源：http://fyj.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://ayv.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://alb.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://caa.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://vig.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://nvk.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://mid.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://bgh.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://pyt.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://yfn.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eyu.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://arx.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xul.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ttn.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dee.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mpj.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ler.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://liv.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://vrh.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jfq.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cfl.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvn.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iuq.birdmap.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zzj.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lce.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kqu.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xpz.gotoacloud.top

[P04] 求长度
来源：http://iap.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oco.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dxh.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lds.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mwp.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://oyo.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://sum.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://hxw.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sba.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://sif.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ore.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://stp.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gpq.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adb.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yka.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://bsm.chenlongwang.top

Ruby: a == b
来源：http://rnw.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gil.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://stu.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gna.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://fnv.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dwr.hnxiangtu.top

TS:   if (x == null) {}
来源：http://ybg.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://snz.shzxlz.cn

Go:   if x == nil {}
来源：http://crk.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://net.guowangkeji.top

C#:   if (x is null) {}
来源：http://fuy.jinqigfzy.top

[P07] 防抖与节流
来源：http://czw.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aix.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://sis.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsk.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwb.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xcl.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uhk.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://abb.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mmz.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://itq.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nuk.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bby.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lrx.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bgy.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ibj.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eba.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vwo.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ysj.52xcode.cn

================================================================================
来源：http://ttr.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yyz.vqdsnc.cn

================================================================================
来源：http://rdq.cqqwz.cn

[Q01] 创建表
来源：http://qgt.9152youxi.cn

CREATE TABLE users (
来源：http://qys.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsp.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://jyi.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://miz.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ygd.jqgfzy.top

);
来源：http://ntp.cashguo.top

[Q02] 创建带外键的表
来源：http://ufa.ctjpmb.com

CREATE TABLE orders (
来源：http://thi.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qgr.shuidangran.top

user_id INT NOT NULL,
来源：http://snt.52xcode.cn

amount DECIMAL(10, 2),
来源：http://qlr.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xym.kuanghao11.cn

);
来源：http://dak.pengpengdd.cyou

[Q03] 增加列
来源：http://qbo.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nml.jinqigufen.top

[Q04] 修改列类型
来源：http://xrx.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rij.jianghu66.top

[Q05] 重命名列
来源：http://poh.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cvj.hesvh.cn

[Q06] 删除列
来源：http://ulp.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ygo.yonumen.top

[Q07] 删除表
来源：http://lka.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://pka.zhixingplan.top

[Q08] 创建普通索引
来源：http://ovq.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mev.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://cgz.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vhp.hysaishi.cn

[Q10] 插入单行
来源：http://ohb.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dvq.hnxiangtu.top

[Q11] 一次插入多行
来源：http://jmp.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ckd.hesvh.cn

[Q12] 插入后取自增 ID
来源：http://ddu.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://cbp.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kpd.xziqi.cn

[Q13] 忽略重复插入
来源：http://hqy.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cpm.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://eql.yangfankeji.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zim.tianlin.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://erh.tianlin.xyz

[Q15] 查询全部
来源：http://hnn.meibo888.top

SELECT * FROM users;
来源：http://vph.52xcode.cn

[Q16] 查询指定列
来源：http://zjc.zhijiandao.cn

SELECT id, name FROM users;
来源：http://bzn.haohaochexian.top

[Q17] 条件查询
来源：http://cso.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gyx.xinyue.icu

[Q18] 模糊匹配
来源：http://cbp.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qrk.dashuyun.cn

[Q19] 范围查询
来源：http://cdd.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pba.meibo888.top

[Q20] IN 列表
来源：http://qej.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rks.cdnleiting.top

[Q21] 空值判断
来源：http://kyq.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ifo.pycfn.com

[Q22] 排序
来源：http://xuj.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dfc.hywenlv.cn

[Q23] 分页
来源：http://ool.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pek.yfazqb.com

[Q24] 去重
来源：http://tvu.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://sny.chenlongwang.top

[Q25] 只取前 N 条
来源：http://wyw.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kgv.shuidangran.top

[Q26] 计数
来源：http://ajb.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://otv.kuanghao11.cn

[Q27] 条件计数
来源：http://pli.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ytd.epnwcf.com

[Q28] 求和与平均
来源：http://otl.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kgk.cqqwz.cn

[Q29] 最大最小值
来源：http://hsr.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zzn.zhiwuduotai.top

[Q30] 分组统计
来源：http://vcj.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nqu.fengsongda.top

[Q31] 分组后过滤
来源：http://pxn.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eto.sxryk.cn

[Q32] 分组拼接字符串
来源：http://bli.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tzh.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uxi.52xcode.cn

[Q33] 多列分组
来源：http://kcw.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zsz.tianlin.xyz

[Q34] 每组取第一条
来源：http://orb.jinyuanbaomall.cn

SELECT * FROM (
来源：http://obe.tarul.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fid.zdqjudy.top

) t WHERE rn = 1;
来源：http://uty.andypj.xyz

[Q35] 内连接
来源：http://tjz.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yes.hfpthk.cn

[Q36] 左连接
来源：http://her.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lvs.hongshengwenyu.top

[Q37] 右连接
来源：http://eui.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cmz.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dcs.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://efj.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://vjl.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvq.jinyuanbaomall.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://umm.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vlk.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgm.yongpay.top

[Q41] 多表连接
来源：http://fje.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mkh.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://oxv.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://aut.havefunace.top

[Q42] 连接条件附加过滤
来源：http://xzp.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://ees.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gec.hysaishi.cn

[Q43] 标量子查询
来源：http://bnu.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qwl.jinqigufen.top

[Q44] IN 子查询
来源：http://xsc.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ofo.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://eey.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uis.hesvh.cn


<!-- 参考信息 -->