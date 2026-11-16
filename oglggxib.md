代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nzg.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ttb.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jzs.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tyn.yangfankeji.com

[N05] 最大公约数
来源：http://tjn.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://ijr.gzhubu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qbd.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oll.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvt.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uwc.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brj.ydzc1.top

Ruby: a.gcd(b)
来源：http://xmn.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ilb.andypj.xyz

[N06] 判断回文字符串
来源：http://fqn.zhijiandao.cn

Py:   s == s[::-1]
来源：http://gic.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://wpw.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://ajp.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://ufn.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pzl.ydjk.org.cn

Go:   // 双指针从两端比较
来源：http://qnl.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://qdp.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ghl.yongpay.top

[N07] 两数之和（返回下标）
来源：http://fyd.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oif.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fne.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://uml.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://lyb.chenlongwang.top

Java: // 手写 HashMap
来源：http://prr.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://nrc.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://jcb.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://zog.ivvv.top

[N08] 生成全排列
来源：http://kit.chenzaomai.com

Py:   itertools.permutations(arr)
来源：http://gve.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://ppo.zdqjudy.top

JS:   // 手写回溯递归
来源：http://krz.haohaochexian.top

TS:   // 手写回溯递归
来源：http://lze.chenlongwang.top

Java: // 手写回溯递归
来源：http://tan.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://gqx.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://fum.ppjwa.cn

C#:   // 手写回溯递归
来源：http://pno.yueranfly.top

[N09] 栈与队列
来源：http://daf.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zlz.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nyj.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wqo.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drh.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rtn.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rkh.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ufj.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xjg.zhoulong.xyz

[N10] 链表节点定义
来源：http://jso.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucy.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ywb.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qmp.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sya.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://coh.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://ffk.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jds.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://hmf.uphjek.com

[N11] 二叉树中序遍历
来源：http://egk.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://udl.yj20258888.top

PHP:  // 手写递归函数
来源：http://lvz.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tqy.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rqi.wangdashe.top

Java: // 手写递归
来源：http://ghn.nwbrower.top

Go:   // 手写递归
来源：http://rfa.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ijg.bbcook.cn

C#:   // 手写递归
来源：http://fwi.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bjg.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zek.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lva.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://run.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zuw.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tfj.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aal.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pwj.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sta.fanxiaobao.xyz

================================================================================
来源：http://bfe.svipenyu.cn

O. 并发与异步
来源：http://sar.zdbjq.cn

================================================================================
来源：http://pvr.fzhhl.top

[O01] 启动一个线程
来源：http://mjd.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hfk.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dlp.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ryp.zdbjq.cn

TS:   // 同 JS
来源：http://kha.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://sxf.zhongyouzk.top

Go:   go f()
来源：http://hxc.cqqwz.cn

Ruby: Thread.new { f }
来源：http://ipw.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://rkw.chenzaomai.com

[O02] 使用线程池
来源：http://aum.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pfb.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://csv.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://gff.52xcode.cn

TS:   // worker_threads 线程池
来源：http://shx.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ult.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hpb.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nvy.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dtg.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://vtp.fengsongda.top

Py:   with lock: shared += 1
来源：http://yzu.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://ugt.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yxk.ybcxt.top

TS:   // 同 JS
来源：http://drj.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://gwy.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://doh.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eco.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://gbq.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://ypt.316326.xyz

Py:   async def f():⏎    await g()
来源：http://gwt.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aaw.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://noi.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ssc.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jut.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aks.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://drb.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://xht.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://hya.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://thk.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jzs.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://cfn.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://jrm.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pkf.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ucf.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://ftq.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qpl.sysykeji.top

[O06] 使用进程池
来源：http://iqb.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nfu.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fna.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://nnv.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://ddv.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnu.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sak.9152youxi.cn

Ruby: // fork 块
来源：http://yky.daxiang520.top

C#:   Parallel.For
来源：http://zco.dashuyun.cn

================================================================================
来源：http://vbf.jlsjyb.cn

P. 常用工具函数
来源：http://geq.jiagoushi.top

================================================================================
来源：http://iax.birdmap.top

[P01] 生成 UUID
来源：http://qja.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://ryz.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qmh.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://fuj.nwbrower.top

TS:   crypto.randomUUID()
来源：http://uos.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://xmq.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://bke.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://cmb.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://fgb.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://cmn.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tnf.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://szy.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oym.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xwa.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ega.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://swm.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qxp.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aii.snrcjt.cn

[P03] 生成短随机字符串
来源：http://bak.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ird.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tfh.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://prw.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pxg.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dmd.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dtm.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://uum.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rcc.cdnleiting.top

[P04] 求长度
来源：http://wqr.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gjz.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ahs.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kiz.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggh.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://urd.xinyue.icu

Go:   len(arr);  len(m)
来源：http://nhq.wangdashe.top

Ruby: x.length;  x.size
来源：http://jws.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wve.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://nfy.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gbl.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vrf.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://snq.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vnu.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ire.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://pup.0kj1m.cn

Ruby: a == b
来源：http://moz.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vbh.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oek.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://udm.birdmap.top

PHP:  if (empty($x)) {}
来源：http://tfa.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xhs.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://adv.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lrf.yongpay.top

Go:   if x == nil {}
来源：http://jgm.daria6918.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pfe.tianlin.xyz

C#:   if (x is null) {}
来源：http://ljv.52xcode.cn

[P07] 防抖与节流
来源：http://smp.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jij.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://oty.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qds.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://poa.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vqy.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mln.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dcw.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gtu.daria6918.cn

[P08] 处理浮点精度问题
来源：http://jao.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fnz.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jxx.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://inu.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qmr.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yee.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vby.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://krx.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tkn.sxryk.cn

================================================================================
来源：http://bus.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cpo.xingfuxueyuan.xyz

================================================================================
来源：http://wqm.snrcjt.cn

[Q01] 创建表
来源：http://qyh.haohaochexian.top

CREATE TABLE users (
来源：http://irl.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kks.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://upp.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://bey.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ikt.yuxming.cn

);
来源：http://xye.yuxming.cn

[Q02] 创建带外键的表
来源：http://qbv.nanxuanxn.top

CREATE TABLE orders (
来源：http://bxw.kuanghao11.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tmn.uphjek.com

user_id INT NOT NULL,
来源：http://tjl.hesvh.cn

amount DECIMAL(10, 2),
来源：http://xtk.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iml.feifeiyinyue.top

);
来源：http://rfk.xuetiantiany.cn

[Q03] 增加列
来源：http://rko.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sqo.hammf.cn

[Q04] 修改列类型
来源：http://kxq.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://avb.mhx1999.top

[Q05] 重命名列
来源：http://yqq.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oag.pycfn.com

[Q06] 删除列
来源：http://iid.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kdd.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://dac.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://dev.zhixingplan.top

[Q08] 创建普通索引
来源：http://dqv.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zlk.andypj.xyz

[Q09] 创建唯一索引
来源：http://zcp.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iat.daria6918.cn

[Q10] 插入单行
来源：http://lgj.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ymw.vehdjk.com

[Q11] 一次插入多行
来源：http://fqx.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sce.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://rex.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://aol.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yfc.chenzaomai.com

[Q13] 忽略重复插入
来源：http://vqw.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uec.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://nsb.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pvg.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hvd.vehdjk.com

[Q15] 查询全部
来源：http://avq.zhoulong.xyz

SELECT * FROM users;
来源：http://fiw.hysaishi.cn

[Q16] 查询指定列
来源：http://nuf.yanxiufei.cn

SELECT id, name FROM users;
来源：http://jgu.hysaishi.cn

[Q17] 条件查询
来源：http://hiz.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ibj.tarul.cn

[Q18] 模糊匹配
来源：http://zkm.sxryk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wrp.fengsongda.top

[Q19] 范围查询
来源：http://lcp.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://evi.yongpay.top

[Q20] IN 列表
来源：http://kfm.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fxq.hywenlv.cn

[Q21] 空值判断
来源：http://lqo.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://gij.jqgfzy.top

[Q22] 排序
来源：http://iip.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eiz.bjfxy.top

[Q23] 分页
来源：http://lte.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uhd.svipenyu.cn

[Q24] 去重
来源：http://irx.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://xax.fehbvm.com

[Q25] 只取前 N 条
来源：http://cbs.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fmu.zdqjudy.top

[Q26] 计数
来源：http://iiq.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://uva.sxryk.cn

[Q27] 条件计数
来源：http://xjg.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pqo.hysaishi.cn

[Q28] 求和与平均
来源：http://jng.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ldz.tianlin.xyz

[Q29] 最大最小值
来源：http://een.tanke756.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ihp.havefunace.top

[Q30] 分组统计
来源：http://jdc.ehwqpu.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jyg.smart0.xyz

[Q31] 分组后过滤
来源：http://ivl.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kbh.bbcook.cn

[Q32] 分组拼接字符串
来源：http://uhs.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mqh.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ulz.sweek.top

[Q33] 多列分组
来源：http://zuu.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vmp.jiagoushi.top

[Q34] 每组取第一条
来源：http://vxi.svipenyu.cn

SELECT * FROM (
来源：http://hyj.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rgo.yonumen.top

) t WHERE rn = 1;
来源：http://fhz.yj20258888.top

[Q35] 内连接
来源：http://cce.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pfj.tianlin.xyz

[Q36] 左连接
来源：http://aol.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jsi.gotoacloud.top

[Q37] 右连接
来源：http://nis.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wgf.ehwqpu.com


<!-- 参考信息 -->