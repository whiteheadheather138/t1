代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wna.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://uue.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vnj.c1oappe.top

Go:   // 双指针从两端比较
来源：http://ncb.yonumen.top

Ruby: s == s.reverse
来源：http://epm.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bpj.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://vof.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dyq.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ixe.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nwp.hammf.cn

TS:   // 手写 Map<string, number>
来源：http://asr.hnqzz.top

Java: // 手写 HashMap
来源：http://ahv.hnqzz.top

Go:   // 手写 map[int]int
来源：http://bks.epnwcf.com

Ruby: // 手写 Hash
来源：http://xsb.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jbk.52xcode.cn

[N08] 生成全排列
来源：http://cij.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://wxt.zhengqikj.top

PHP:  // 手写递归交换
来源：http://hsq.shzxlz.cn

JS:   // 手写回溯递归
来源：http://gcf.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://fos.yj20258888.top

Java: // 手写回溯递归
来源：http://mpy.jiagoushi.top

Go:   // 手写回溯递归
来源：http://pup.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://oyd.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://nxw.wangshuangyany.cn

[N09] 栈与队列
来源：http://ddz.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rvx.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixs.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iyf.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dpb.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwx.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jtx.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rer.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pea.mhx1999.top

[N10] 链表节点定义
来源：http://cso.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://edw.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cbf.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xdq.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jca.cashguo.top

Java: class Node { int v; Node next; }
来源：http://bmu.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://qdq.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://slr.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ouz.meibo888.top

[N11] 二叉树中序遍历
来源：http://mlm.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bhv.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://pxw.dianchejie.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://obk.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://btw.cheryme.top

Java: // 手写递归
来源：http://kvn.vqdsnc.cn

Go:   // 手写递归
来源：http://ryu.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://koq.jqgfzy.top

C#:   // 手写递归
来源：http://gcg.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://luh.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gnn.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://duh.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://poy.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtm.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yrq.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yfq.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zld.gogol.net.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uii.chenzaomai.com

================================================================================
来源：http://unc.tanke756.top

O. 并发与异步
来源：http://plj.dianchejie.cn

================================================================================
来源：http://liy.yonumen.top

[O01] 启动一个线程
来源：http://zfk.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cyn.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kek.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dpx.zhongyouzk.top

TS:   // 同 JS
来源：http://eos.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://nme.gotoacloud.top

Go:   go f()
来源：http://gts.hammf.cn

Ruby: Thread.new { f }
来源：http://sae.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://azp.zhoulong.xyz

[O02] 使用线程池
来源：http://jwv.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lut.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://myb.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://upx.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://oms.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://ezo.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lda.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qxu.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uvz.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://cgp.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://whh.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://bvd.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oxn.smart0.xyz

TS:   // 同 JS
来源：http://cdo.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://ypl.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pgm.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cem.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://coi.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://fcs.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://lpz.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rmb.shuidangran.top

JS:   async function f() { await g(); }
来源：http://xwc.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cgb.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uxc.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ebi.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://xxs.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://ykk.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://okb.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://lum.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ftb.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://gwu.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://wgz.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aiq.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dvz.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://ury.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vja.jinghuilouyu.cn

[O06] 使用进程池
来源：http://uvu.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dvd.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ntg.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://oli.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://wnd.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ryb.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uup.daria6918.cn

Ruby: // fork 块
来源：http://wfu.havefunace.top

C#:   Parallel.For
来源：http://xwq.fehbvm.com

================================================================================
来源：http://ddz.hysaishi.cn

P. 常用工具函数
来源：http://vyf.zhiwuduotai.top

================================================================================
来源：http://avx.dashuyun.cn

[P01] 生成 UUID
来源：http://eax.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://ume.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aco.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://uem.smart0.xyz

TS:   crypto.randomUUID()
来源：http://jgn.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://xlp.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://ipm.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://vcd.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://cls.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://ies.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cyj.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://cns.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hna.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://exd.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zdz.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vad.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yay.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yuh.aizwys.cn

[P03] 生成短随机字符串
来源：http://jlw.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qfn.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vbd.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yzb.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pye.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pks.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://swc.iojbl.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xdo.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fzu.smart0.xyz

[P04] 求长度
来源：http://ofz.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xcw.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xlx.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ilg.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akf.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://xlh.cheryme.top

Go:   len(arr);  len(m)
来源：http://wxe.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://zqh.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gmc.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://hrd.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bca.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bru.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qou.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hkp.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ccc.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ovv.ydzc1.top

Ruby: a == b
来源：http://nrc.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rdc.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://emp.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://onf.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://rwd.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cof.vehdjk.com

TS:   if (x == null) {}
来源：http://uwj.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://sqe.aizwys.cn

Go:   if x == nil {}
来源：http://sjm.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nkb.iojbl.cn

C#:   if (x is null) {}
来源：http://zoe.hcnkem.com

[P07] 防抖与节流
来源：http://rra.nanxinkj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://roh.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://art.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://flh.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hen.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://umf.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://esv.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ukr.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rvr.sysykeji.top

[P08] 处理浮点精度问题
来源：http://dmb.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qnj.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qoc.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bxv.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ftb.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://teq.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jnz.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oup.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wao.jqgfzy.top

================================================================================
来源：http://fos.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uqj.yuanzhike.top

================================================================================
来源：http://oux.shanyushiyangtech.top

[Q01] 创建表
来源：http://him.hammf.cn

CREATE TABLE users (
来源：http://acc.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tni.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://mne.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://ofb.ctjpmb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hac.tarul.cn

);
来源：http://yrr.zhixingplan.top

[Q02] 创建带外键的表
来源：http://ysj.svipenyu.cn

CREATE TABLE orders (
来源：http://oht.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uby.hnqzz.top

user_id INT NOT NULL,
来源：http://rge.xinyue.icu

amount DECIMAL(10, 2),
来源：http://yrc.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vjv.jiagoushi.top

);
来源：http://xll.jlsjyb.cn

[Q03] 增加列
来源：http://jfc.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://umv.xinyue.icu

[Q04] 修改列类型
来源：http://box.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qgc.sjlbkw.cn

[Q05] 重命名列
来源：http://res.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bck.andypj.xyz

[Q06] 删除列
来源：http://vbm.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bay.52xcode.cn

[Q07] 删除表
来源：http://npr.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://qir.yvedp.cn

[Q08] 创建普通索引
来源：http://oyn.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://voc.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://pim.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nby.xuanzx.com

[Q10] 插入单行
来源：http://ijn.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kul.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://mks.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lop.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://dwc.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://bei.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ylh.316326.xyz

[Q13] 忽略重复插入
来源：http://aqx.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ybs.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://vqw.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yof.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nbj.jiagoushi.top

[Q15] 查询全部
来源：http://mqs.zhiwuduotai.top

SELECT * FROM users;
来源：http://hft.andypj.xyz

[Q16] 查询指定列
来源：http://dii.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://fke.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://izd.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpc.yonumen.top

[Q18] 模糊匹配
来源：http://rgz.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://htb.ctjpmb.com

[Q19] 范围查询
来源：http://xle.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qwh.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://hyt.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xoq.yj20258888.top

[Q21] 空值判断
来源：http://myj.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://urv.shanyushiyangkeji.top

[Q22] 排序
来源：http://pvi.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mrn.ehwqpu.com

[Q23] 分页
来源：http://ghf.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tpr.ppjwa.cn

[Q24] 去重
来源：http://bul.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://fqo.hywenlv.cn

[Q25] 只取前 N 条
来源：http://hny.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://urf.wangdashe.top

[Q26] 计数
来源：http://bpv.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://drg.uphjek.com

[Q27] 条件计数
来源：http://aej.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://snv.jlsjyb.cn

[Q28] 求和与平均
来源：http://dxz.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://voe.sufxvd.cn

[Q29] 最大最小值
来源：http://cky.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kmy.kuanghao11.cn

[Q30] 分组统计
来源：http://aqa.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xxe.hnxiangtu.top

[Q31] 分组后过滤
来源：http://kme.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lko.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://lbz.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fdn.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xtd.andypj.xyz

[Q33] 多列分组
来源：http://nwk.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xgn.hnqzz.top

[Q34] 每组取第一条
来源：http://ttr.tian-w.cn

SELECT * FROM (
来源：http://rxt.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://izc.ywan-chungtsiang.top

) t WHERE rn = 1;
来源：http://hnf.jqgufenzy.top

[Q35] 内连接
来源：http://hil.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sca.jianghu66.top

[Q36] 左连接
来源：http://bas.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vbc.316326.xyz

[Q37] 右连接
来源：http://gqk.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yuv.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kuh.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gwl.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://zgs.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ttf.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hin.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://jys.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lub.zdqjudy.top

[Q41] 多表连接
来源：http://lgc.dashuyun.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ukc.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://zba.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://yqp.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://wkc.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://hou.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://unp.jqgufenzy.top

[Q43] 标量子查询
来源：http://rzr.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pfn.svipenyu.cn


<!-- 参考信息 -->