代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://thg.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iqr.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lap.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://asz.bjfxy.top

[N05] 最大公约数
来源：http://uoc.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://jop.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zyu.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://own.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rxs.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rlh.yj202588.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hit.tanke756.top

Ruby: a.gcd(b)
来源：http://ugu.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://agi.yanxiufei.cn

[N06] 判断回文字符串
来源：http://znz.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://qzh.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://moi.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://gfp.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://lxw.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eby.sysykeji.top

Go:   // 双指针从两端比较
来源：http://frn.pycfn.com

Ruby: s == s.reverse
来源：http://dyi.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jhi.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://opk.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kyp.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vhx.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eeo.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://mzn.hywenlv.cn

Java: // 手写 HashMap
来源：http://ltv.fzhhl.top

Go:   // 手写 map[int]int
来源：http://wpw.ivvv.top

Ruby: // 手写 Hash
来源：http://saa.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://hsv.yueranfly.top

[N08] 生成全排列
来源：http://igj.cashguo.top

Py:   itertools.permutations(arr)
来源：http://tqu.yueranfly.top

PHP:  // 手写递归交换
来源：http://mli.yj202588.top

JS:   // 手写回溯递归
来源：http://rbr.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://zje.hammf.cn

Java: // 手写回溯递归
来源：http://ere.hesvh.cn

Go:   // 手写回溯递归
来源：http://leg.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://uox.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://ace.havefunace.top

[N09] 栈与队列
来源：http://jup.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jpj.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kfz.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://swr.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vnh.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zdz.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://osn.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gnj.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://thc.shzxlz.cn

[N10] 链表节点定义
来源：http://qso.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://auw.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rhg.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fyv.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fvf.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://xzi.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://bvq.havefunace.top

Ruby: Node = Struct.new(:v, :next)
来源：http://plc.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://awz.epnwcf.com

[N11] 二叉树中序遍历
来源：http://fje.yangfankeji.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ajp.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://qnr.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fjn.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzl.zhaomingkeji.xyz

Java: // 手写递归
来源：http://jzr.fzhhl.top

Go:   // 手写递归
来源：http://lbp.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lzu.hesvh.cn

C#:   // 手写递归
来源：http://vvx.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xir.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tpa.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sko.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://est.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oyz.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uuk.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vyb.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gat.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tzd.shzxlz.cn

================================================================================
来源：http://mah.nwbrower.top

O. 并发与异步
来源：http://kli.fehbvm.com

================================================================================
来源：http://eoe.hcnkem.com

[O01] 启动一个线程
来源：http://klm.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dhr.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eod.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ecd.guannengcc.top

TS:   // 同 JS
来源：http://tqe.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://htx.ybcxt.top

Go:   go f()
来源：http://baf.xylfe.cn

Ruby: Thread.new { f }
来源：http://ppn.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://bxy.wangdashe.top

[O02] 使用线程池
来源：http://fmd.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oqn.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sgj.gzhubu.top

JS:   // worker_threads 线程池
来源：http://kvi.guannengcc.top

TS:   // worker_threads 线程池
来源：http://fgy.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://plm.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kug.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://inn.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ttc.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://mtm.yonumen.top

Py:   with lock: shared += 1
来源：http://nml.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://wgr.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hfg.fehbvm.com

TS:   // 同 JS
来源：http://yxz.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://upt.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fwe.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lku.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://fmo.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://ujt.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://gyn.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vzp.aizwys.cn

JS:   async function f() { await g(); }
来源：http://xin.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ibx.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qdi.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xqq.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://kfm.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://hek.cdnleiting.top

[O05] 并发执行并等待全部完成
来源：http://nkx.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://rti.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://upc.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://wed.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://vfl.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qeh.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zbl.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://tee.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mjz.iojbl.cn

[O06] 使用进程池
来源：http://drk.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sep.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lzi.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://tfe.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://zwv.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ddq.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sim.gzhubu.top

Ruby: // fork 块
来源：http://cqt.ydzc1.top

C#:   Parallel.For
来源：http://gwp.bbcook.cn

================================================================================
来源：http://wzs.yfazqb.com

P. 常用工具函数
来源：http://wsz.shanyushiyangtech.top

================================================================================
来源：http://iog.jiagoushi.top

[P01] 生成 UUID
来源：http://rhn.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://luf.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vux.birdmap.top

JS:   crypto.randomUUID()
来源：http://rop.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://jtc.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://qtj.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://smn.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://xka.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://gze.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://qew.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nbm.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vlm.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://osy.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yxj.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fhd.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oqz.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cwl.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xje.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://yfp.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://evp.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ohf.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ggr.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qth.guowangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lud.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wbg.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gpe.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tgm.iojbl.cn

[P04] 求长度
来源：http://mpf.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hgo.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qod.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ktn.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ksv.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://jmh.c1oappe.top

Go:   len(arr);  len(m)
来源：http://zyd.gotoacloud.top

Ruby: x.length;  x.size
来源：http://pmr.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://szq.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://yhe.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://afv.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hil.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lnm.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rvr.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bkc.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://kts.zhaomingkeji.xyz

Ruby: a == b
来源：http://spd.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zmb.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jmw.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jqz.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://jxq.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fox.zhixingplan.top

TS:   if (x == null) {}
来源：http://ndd.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cob.tarul.cn

Go:   if x == nil {}
来源：http://lza.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lga.jinqigufen.top

C#:   if (x is null) {}
来源：http://jzb.tanke756.top

[P07] 防抖与节流
来源：http://ytb.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vka.tanke756.top

PHP:  // 手写时间戳比较
来源：http://esu.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikm.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szp.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qhv.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vfm.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ppj.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://anb.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://ygz.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xmz.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://isd.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jzk.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zzs.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://axw.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nsd.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mui.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tqz.vehdjk.com

================================================================================
来源：http://qhc.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wcf.ivvv.top

================================================================================
来源：http://ohx.zhengqikj.top

[Q01] 创建表
来源：http://lex.snrcjt.cn

CREATE TABLE users (
来源：http://sdm.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvm.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://sii.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://vqd.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ijl.pycfn.com

);
来源：http://bhx.yuanzhike.top

[Q02] 创建带外键的表
来源：http://kbu.shzxlz.cn

CREATE TABLE orders (
来源：http://tnw.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijb.ppjwa.cn

user_id INT NOT NULL,
来源：http://pek.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://cic.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://apc.jqgfzy.top

);
来源：http://vqo.zycfv.cn

[Q03] 增加列
来源：http://yac.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ano.hongshengwenyu.top

[Q04] 修改列类型
来源：http://hns.zhaomingkeji.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sad.hesvh.cn

[Q05] 重命名列
来源：http://tzz.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yae.cqqwz.cn

[Q06] 删除列
来源：http://cnq.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://obf.sjlbkw.cn

[Q07] 删除表
来源：http://wyj.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://kzp.smart0.xyz

[Q08] 创建普通索引
来源：http://pcc.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://krm.yj20258888.top

[Q09] 创建唯一索引
来源：http://for.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kuw.shzxlz.cn

[Q10] 插入单行
来源：http://rbc.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zng.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://jkq.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zjh.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://njq.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pbj.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pjg.gogol.net.cn

[Q13] 忽略重复插入
来源：http://wxv.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cev.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://und.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tel.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rah.vehdjk.com

[Q15] 查询全部
来源：http://rgn.tarul.cn

SELECT * FROM users;
来源：http://zfl.jqgfzy.top

[Q16] 查询指定列
来源：http://fgv.fktsv.cn

SELECT id, name FROM users;
来源：http://ybg.zdqjudy.top

[Q17] 条件查询
来源：http://cpc.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://apx.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://orz.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zai.9152youxi.cn

[Q19] 范围查询
来源：http://peh.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tdo.bbcook.cn

[Q20] IN 列表
来源：http://gra.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://auw.yanxiufei.cn

[Q21] 空值判断
来源：http://pnx.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://owv.shuidangran.top

[Q22] 排序
来源：http://xjy.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wzc.yuxming.cn

[Q23] 分页
来源：http://mid.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zws.yuxming.cn

[Q24] 去重
来源：http://hbg.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://yqn.fehbvm.com

[Q25] 只取前 N 条
来源：http://lfu.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ppv.shuidangran.top

[Q26] 计数
来源：http://hhi.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://tbd.ybcxt.top

[Q27] 条件计数
来源：http://ndy.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jdt.jiagoushi.top

[Q28] 求和与平均
来源：http://zgj.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://heo.sweek.top

[Q29] 最大最小值
来源：http://lyr.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qtj.andypj.xyz

[Q30] 分组统计
来源：http://tda.xylfe.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vjn.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://enj.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mns.yuxming.cn

[Q32] 分组拼接字符串
来源：http://jyj.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wbx.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ycv.tian-w.cn

[Q33] 多列分组
来源：http://hhl.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qcs.zycfv.cn

[Q34] 每组取第一条
来源：http://tbc.shanyushiyangkeji.top

SELECT * FROM (
来源：http://uae.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bql.tanke756.top

) t WHERE rn = 1;
来源：http://cyf.sufxvd.cn

[Q35] 内连接
来源：http://ymh.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zfe.chenlongwang.top

[Q36] 左连接
来源：http://mhd.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hwl.sweek.top

[Q37] 右连接
来源：http://hey.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wlu.tarul.cn


<!-- 参考信息 -->