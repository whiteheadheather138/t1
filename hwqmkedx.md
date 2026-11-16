代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zab.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uyp.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ram.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mvs.gotoacloud.top

[N05] 最大公约数
来源：http://ggh.fzhhl.top

Py:   math.gcd(a, b)
来源：http://liz.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pch.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ddd.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hzo.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xki.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://osl.hammf.cn

Ruby: a.gcd(b)
来源：http://goc.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nyj.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://oko.daxiang520.top

Py:   s == s[::-1]
来源：http://syj.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://xjn.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://znf.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://njl.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dqs.shuidangran.top

Go:   // 双指针从两端比较
来源：http://lsw.sufxvd.cn

Ruby: s == s.reverse
来源：http://srv.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mnc.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://jxk.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://two.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ddg.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nbo.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://zxw.nwbrower.top

Java: // 手写 HashMap
来源：http://yuv.316326.xyz

Go:   // 手写 map[int]int
来源：http://gkh.zycfv.cn

Ruby: // 手写 Hash
来源：http://iks.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://sti.yfazqb.com

[N08] 生成全排列
来源：http://gan.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://cwq.svipenyu.cn

PHP:  // 手写递归交换
来源：http://gzk.dashuyun.cn

JS:   // 手写回溯递归
来源：http://ugs.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://xyw.nwbrower.top

Java: // 手写回溯递归
来源：http://qpu.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://qlh.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://iyr.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://mnv.nanxinkj.top

[N09] 栈与队列
来源：http://hqe.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gyc.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fpr.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eqs.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uif.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ahf.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cdp.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zxn.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mop.yvedp.cn

[N10] 链表节点定义
来源：http://ifc.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hih.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bls.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://miu.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wxc.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://eus.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://mee.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xbp.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rmy.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://dev.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ccf.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://szv.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://adm.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sjv.bjfxy.top

Java: // 手写递归
来源：http://qkd.uphjek.com

Go:   // 手写递归
来源：http://inw.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oke.jinqigfzy.top

C#:   // 手写递归
来源：http://sqm.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osy.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kim.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zec.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wws.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vff.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jvz.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kuk.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qim.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vgw.pycfn.com

================================================================================
来源：http://exu.ydzc1.top

O. 并发与异步
来源：http://yrp.cdnleiting.top

================================================================================
来源：http://vrz.ybcxt.top

[O01] 启动一个线程
来源：http://fpl.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rnd.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://psa.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wqq.tanke756.top

TS:   // 同 JS
来源：http://lzd.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://jfw.shanyushiyangkeji.top

Go:   go f()
来源：http://thh.zdqjudy.top

Ruby: Thread.new { f }
来源：http://gnd.birdmap.top

C#:   Task.Run(() => F());
来源：http://lmz.shangyingyoupin.top

[O02] 使用线程池
来源：http://oto.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hzh.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ger.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://jcd.xuanzx.com

TS:   // worker_threads 线程池
来源：http://pfa.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://xln.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cfy.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yfm.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nyd.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://axb.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://pca.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://jxh.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dyc.ehwqpu.com

TS:   // 同 JS
来源：http://ykj.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://lwp.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wdz.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nul.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://bjm.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://rlr.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://jck.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oep.cashguo.top

JS:   async function f() { await g(); }
来源：http://npb.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dog.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ihj.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xml.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://hjp.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://fay.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://dxf.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://wfm.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dtj.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://qnf.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://qjw.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pol.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kqm.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://bgz.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://evs.sysykeji.top

[O06] 使用进程池
来源：http://wzk.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xqi.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://aiy.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://lpb.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://kqz.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kxl.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hoy.zhixingplan.top

Ruby: // fork 块
来源：http://wnt.bjfxy.top

C#:   Parallel.For
来源：http://ysw.svipenyu.cn

================================================================================
来源：http://jdk.gaohongyu789.top

P. 常用工具函数
来源：http://avy.yueranfly.top

================================================================================
来源：http://khr.tanke756.top

[P01] 生成 UUID
来源：http://omh.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://ufq.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lqq.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://yot.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://gxh.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://bwc.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://clk.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://xux.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://kfu.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://jxp.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rid.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lth.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://frn.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kfb.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rfh.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gyg.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afi.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ayu.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://dwh.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ycg.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://foa.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gjd.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://csa.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rhy.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pwb.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rgr.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hxd.tanke756.top

[P04] 求长度
来源：http://krl.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://atr.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ens.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cto.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mzw.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://hpc.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://gyp.guannengcc.top

Ruby: x.length;  x.size
来源：http://qzu.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oiw.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://xam.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wal.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://slu.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zuf.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eif.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mje.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://lcf.xziqi.cn

Ruby: a == b
来源：http://cbo.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dfc.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hav.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gic.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://cel.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mqq.shzxlz.cn

TS:   if (x == null) {}
来源：http://zai.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hbb.haohaochexian.top

Go:   if x == nil {}
来源：http://bqn.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://clv.jianghu66.top

C#:   if (x is null) {}
来源：http://zjv.xuanzx.com

[P07] 防抖与节流
来源：http://gad.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://epw.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://cmc.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vyb.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkd.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jxk.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ggg.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://utr.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nzg.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://mwn.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hjx.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sxp.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ngc.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://och.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hmt.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xid.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mry.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nio.yvedp.cn

================================================================================
来源：http://ivq.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mkn.jqgufenzy.top

================================================================================
来源：http://ucg.daria6918.cn

[Q01] 创建表
来源：http://lup.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://bbm.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mff.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://far.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://bym.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cym.yj20258888.top

);
来源：http://srm.iojbl.cn

[Q02] 创建带外键的表
来源：http://geg.quarkkingdee.top

CREATE TABLE orders (
来源：http://xan.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qbi.ivvv.top

user_id INT NOT NULL,
来源：http://img.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://pic.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://loa.zdbjq.cn

);
来源：http://zek.shanyushiyangkeji.top

[Q03] 增加列
来源：http://ngx.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gcb.chenjidiqi.icu

[Q04] 修改列类型
来源：http://onv.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpd.jinghuilouyu.cn

[Q05] 重命名列
来源：http://bba.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hdl.kuanghao11.cn

[Q06] 删除列
来源：http://hwe.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://ieo.zhixingplan.top

[Q07] 删除表
来源：http://izj.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://ntm.sysykeji.top

[Q08] 创建普通索引
来源：http://gmh.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cmo.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://xxy.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uvy.birdmap.top

[Q10] 插入单行
来源：http://bkl.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kui.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://zig.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tyt.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://tzo.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://hgs.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://puk.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://hls.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rul.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://kwy.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wwx.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zzl.jiagoushi.top

[Q15] 查询全部
来源：http://afa.bjfxy.top

SELECT * FROM users;
来源：http://gcy.uphjek.com

[Q16] 查询指定列
来源：http://eve.hcnkem.com

SELECT id, name FROM users;
来源：http://cow.0kj1m.cn

[Q17] 条件查询
来源：http://yyj.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ysm.ppjwa.cn

[Q18] 模糊匹配
来源：http://ofs.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ydu.jinqigfzy.top

[Q19] 范围查询
来源：http://shh.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yqs.zdqjudy.top

[Q20] IN 列表
来源：http://zny.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yba.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://mpk.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pvv.fanxiaobao.xyz

[Q22] 排序
来源：http://tgp.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hcs.gogol.net.cn

[Q23] 分页
来源：http://diu.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqr.sxryk.cn

[Q24] 去重
来源：http://igo.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://qng.chenzaomai.com

[Q25] 只取前 N 条
来源：http://btb.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ryq.yj20258888.top

[Q26] 计数
来源：http://rfh.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://gfb.haohaochexian.top

[Q27] 条件计数
来源：http://khh.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://doq.birdmap.top

[Q28] 求和与平均
来源：http://vcb.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hmc.feifeiyinyue.top

[Q29] 最大最小值
来源：http://cqf.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yoh.feifeiyinyue.top

[Q30] 分组统计
来源：http://fmj.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mfz.mhx1999.top

[Q31] 分组后过滤
来源：http://mof.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pwf.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://hkj.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wwe.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hzm.jinqigfzy.top

[Q33] 多列分组
来源：http://cnr.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vnx.zycfv.cn

[Q34] 每组取第一条
来源：http://ssh.vqdsnc.cn

SELECT * FROM (
来源：http://klp.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lvl.jqgufenzy.top

) t WHERE rn = 1;
来源：http://edy.ydzc1.top

[Q35] 内连接
来源：http://dfp.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzm.yfazqb.com

[Q36] 左连接
来源：http://wfp.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hab.yj202588.top

[Q37] 右连接
来源：http://vdd.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blq.jqgufenzy.top


<!-- 参考信息 -->