代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uca.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vvb.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lsx.gogol.net.cn

Ruby: a.gcd(b)
来源：http://qvq.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqc.yanxiufei.cn

[N06] 判断回文字符串
来源：http://mau.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://lls.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://pqn.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://gek.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://jlc.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zxs.yueranfly.top

Go:   // 双指针从两端比较
来源：http://dzc.dianchejie.cn

Ruby: s == s.reverse
来源：http://wyj.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pja.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://rpx.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hxr.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hpf.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kio.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://izb.tarul.cn

Java: // 手写 HashMap
来源：http://acf.yj20258.top

Go:   // 手写 map[int]int
来源：http://wsb.hcnkem.com

Ruby: // 手写 Hash
来源：http://khu.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tki.zhengqikj.top

[N08] 生成全排列
来源：http://mxn.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://nyx.aibaodan.cn

PHP:  // 手写递归交换
来源：http://fix.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://qoy.pycfn.com

TS:   // 手写回溯递归
来源：http://brc.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://ocb.ctjpmb.com

Go:   // 手写回溯递归
来源：http://wzm.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://qeg.ydzc1.top

C#:   // 手写回溯递归
来源：http://jtd.sufxvd.cn

[N09] 栈与队列
来源：http://gnu.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fxt.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wue.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwj.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mlj.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ygg.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wdh.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vij.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://raj.tanke756.top

[N10] 链表节点定义
来源：http://wkl.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yqj.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yij.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ywo.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ywm.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://iwr.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://dvl.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://pyu.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://luy.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://vzw.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ibd.chenzaomai.com

PHP:  // 手写递归函数
来源：http://sna.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jyl.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yhk.quarkkingdee.top

Java: // 手写递归
来源：http://hxw.jianghu66.top

Go:   // 手写递归
来源：http://ykk.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tnv.zhiwuduotai.top

C#:   // 手写递归
来源：http://wwc.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ivi.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qdd.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nhx.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://txh.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yij.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://agu.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jbv.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vxg.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pki.316326.xyz

================================================================================
来源：http://bbu.jyoumei.cn

O. 并发与异步
来源：http://fhs.smart0.xyz

================================================================================
来源：http://vvn.shzxlz.cn

[O01] 启动一个线程
来源：http://bew.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sem.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aoe.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxd.shanyushiyangtech.top

TS:   // 同 JS
来源：http://vse.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://yyo.ydjk.org.cn

Go:   go f()
来源：http://ufa.yvedp.cn

Ruby: Thread.new { f }
来源：http://vba.xylfe.cn

C#:   Task.Run(() => F());
来源：http://xkl.meibo888.top

[O02] 使用线程池
来源：http://yoy.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cpa.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ndz.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://csa.cashguo.top

TS:   // worker_threads 线程池
来源：http://qtq.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eaa.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qsz.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yrs.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ygm.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://ebn.havefunace.top

Py:   with lock: shared += 1
来源：http://iok.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://fuj.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ave.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://jer.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://pga.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ekr.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gmu.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://sqp.cheryme.top

[O04] 定义异步函数并等待
来源：http://xvk.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://rwm.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yrd.svipenyu.cn

JS:   async function f() { await g(); }
来源：http://cpv.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bcq.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wzw.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zkb.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eam.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://ivz.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://llw.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://bty.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ybj.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://ahv.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://edq.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nzt.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lht.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://bbk.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqn.jlsjyb.cn

[O06] 使用进程池
来源：http://wrt.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ydc.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qpo.tanke756.top

JS:   // child_process / cluster 模块
来源：http://ujv.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://xls.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jtj.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kxd.yj20258888.top

Ruby: // fork 块
来源：http://hkl.bjfxy.top

C#:   Parallel.For
来源：http://nhd.hongshengwenyu.top

================================================================================
来源：http://yon.9152youxi.cn

P. 常用工具函数
来源：http://uyj.jinghuilouyu.cn

================================================================================
来源：http://lta.ctjpmb.com

[P01] 生成 UUID
来源：http://ozx.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://rzu.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qgf.fzhhl.top

JS:   crypto.randomUUID()
来源：http://fhq.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://rtp.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://lnv.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://top.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://qcv.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://eco.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://bdj.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vtc.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wjl.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xon.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qqt.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ejo.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eih.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://knh.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cuc.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://pju.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ihp.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pjv.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pcg.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mup.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tkz.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bxw.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pmm.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rqm.jinqigfzy.top

[P04] 求长度
来源：http://wpl.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qql.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://syn.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ijr.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wrm.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://cib.redwolf501.top

Go:   len(arr);  len(m)
来源：http://fvz.shuidangran.top

Ruby: x.length;  x.size
来源：http://ppp.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pmn.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://rhi.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvk.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fut.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://flf.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://adv.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ncu.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://dkg.sweek.top

Ruby: a == b
来源：http://ecb.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kvg.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hgp.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bga.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://qrl.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ccl.hnxiangtu.top

TS:   if (x == null) {}
来源：http://lfr.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dok.zycfv.cn

Go:   if x == nil {}
来源：http://iqa.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzi.yuxming.cn

C#:   if (x is null) {}
来源：http://ykw.0kj1m.cn

[P07] 防抖与节流
来源：http://lqh.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bzo.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://vsb.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qnn.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lot.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ejf.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ezw.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bba.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hhw.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://rtm.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kom.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jaq.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://upb.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://btg.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hwi.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vtb.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aib.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vef.jianghu66.top

================================================================================
来源：http://qaq.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nsh.kuanghao11.cn

================================================================================
来源：http://xxe.jinqigfzy.top

[Q01] 创建表
来源：http://lap.epnwcf.com

CREATE TABLE users (
来源：http://lri.shanyushiyangtech.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gwj.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://wco.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://zai.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lvj.zhongyouzk.top

);
来源：http://vve.sufxvd.cn

[Q02] 创建带外键的表
来源：http://xii.jqgufenzy.top

CREATE TABLE orders (
来源：http://shd.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://syn.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://wgr.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://cdm.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://brb.ctjpmb.com

);
来源：http://hon.haohaochexian.top

[Q03] 增加列
来源：http://uun.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vht.jqgfzy.top

[Q04] 修改列类型
来源：http://hix.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hii.ydzc1.top

[Q05] 重命名列
来源：http://lah.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ryv.wangdashe.top

[Q06] 删除列
来源：http://hnr.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lsq.yfazqb.com

[Q07] 删除表
来源：http://sws.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://khm.jqgfzy.top

[Q08] 创建普通索引
来源：http://qif.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://put.epnwcf.com

[Q09] 创建唯一索引
来源：http://ljz.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ksl.daria6918.cn

[Q10] 插入单行
来源：http://twy.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kkp.yongpay.top

[Q11] 一次插入多行
来源：http://yub.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ulg.hammf.cn

[Q12] 插入后取自增 ID
来源：http://tfv.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jeo.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dtn.yuxming.cn

[Q13] 忽略重复插入
来源：http://zum.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yft.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://uyh.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qkp.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tza.dianchejie.cn

[Q15] 查询全部
来源：http://obw.zhoulong.xyz

SELECT * FROM users;
来源：http://ise.guowangkeji.top

[Q16] 查询指定列
来源：http://nbz.yj20258888.top

SELECT id, name FROM users;
来源：http://wiu.fanxiaobao.xyz

[Q17] 条件查询
来源：http://cmf.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wae.xuanzx.com

[Q18] 模糊匹配
来源：http://vpw.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xfd.yj20258888.top

[Q19] 范围查询
来源：http://xct.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oom.cdnleiting.top

[Q20] IN 列表
来源：http://ere.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fsf.yuanzhike.top

[Q21] 空值判断
来源：http://boa.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kez.yj20258888.top

[Q22] 排序
来源：http://fbp.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sqv.birdmap.top

[Q23] 分页
来源：http://ycs.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://azl.iojbl.cn

[Q24] 去重
来源：http://see.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://hvq.birdmap.top

[Q25] 只取前 N 条
来源：http://cal.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oxu.jlsjyb.cn

[Q26] 计数
来源：http://yhj.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://odr.vehdjk.com

[Q27] 条件计数
来源：http://tbk.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://myg.haohaochexian.top

[Q28] 求和与平均
来源：http://hsw.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zky.aibaodan.cn

[Q29] 最大最小值
来源：http://cue.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://qqq.ydzc1.top

[Q30] 分组统计
来源：http://lvo.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dzm.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://aqy.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lis.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://iss.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sjk.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://svx.vqdsnc.cn

[Q33] 多列分组
来源：http://tma.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pcs.hnxiangtu.top

[Q34] 每组取第一条
来源：http://jtp.ybcxt.top

SELECT * FROM (
来源：http://nsa.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://oqu.jinqigfzy.top

) t WHERE rn = 1;
来源：http://ueq.haohaochexian.top

[Q35] 内连接
来源：http://ats.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vtc.bjfxy.top

[Q36] 左连接
来源：http://ttg.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dzb.ybcxt.top

[Q37] 右连接
来源：http://uas.pengpengdd.cyou

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uhr.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://swx.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zfz.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://fgv.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcy.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://inf.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://ojn.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aac.ywan-chungtsiang.top

[Q41] 多表连接
来源：http://fgg.sjlbkw.cn


<!-- 参考信息 -->