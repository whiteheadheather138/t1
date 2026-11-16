代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kab.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ssi.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://poh.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aqw.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://swn.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zgb.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rbm.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xch.zdbjq.cn

[N05] 最大公约数
来源：http://ury.sweek.top

Py:   math.gcd(a, b)
来源：http://gzj.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://axn.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydq.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eob.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://znt.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zta.xuanzx.com

Ruby: a.gcd(b)
来源：http://mvx.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhy.uphjek.com

[N06] 判断回文字符串
来源：http://fzw.hfpthk.cn

Py:   s == s[::-1]
来源：http://unz.smart0.xyz

PHP:  $s === strrev($s);
来源：http://cag.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://lbe.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://esm.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zve.sysykeji.top

Go:   // 双指针从两端比较
来源：http://elf.xziqi.cn

Ruby: s == s.reverse
来源：http://mqw.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lrv.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://amt.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mzq.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://stp.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://nqh.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://lpe.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://wtw.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://hon.0kj1m.cn

Ruby: // 手写 Hash
来源：http://squ.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://lhn.yuanzhike.top

[N08] 生成全排列
来源：http://wdr.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://wnd.zdqjudy.top

PHP:  // 手写递归交换
来源：http://qpx.zhengqikj.top

JS:   // 手写回溯递归
来源：http://wwy.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://neu.birdmap.top

Java: // 手写回溯递归
来源：http://bvw.havefunace.top

Go:   // 手写回溯递归
来源：http://ggn.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://bcu.yangfankeji.com

C#:   // 手写回溯递归
来源：http://fkf.chenjidiqi.icu

[N09] 栈与队列
来源：http://vuq.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://huz.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oge.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kpi.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ykn.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ocx.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ofy.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zkp.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nsg.yuanzhike.top

[N10] 链表节点定义
来源：http://rgk.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xtn.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cnq.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://snj.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jpq.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://xac.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://qyb.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://gfa.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mao.ivvv.top

[N11] 二叉树中序遍历
来源：http://qno.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://npg.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://lhw.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zeq.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fos.hesvh.cn

Java: // 手写递归
来源：http://ygv.redwolf501.top

Go:   // 手写递归
来源：http://afo.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nmb.gzhubu.top

C#:   // 手写递归
来源：http://dzo.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wpo.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ves.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pcc.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuc.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aop.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zlj.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uhd.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vvv.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mli.ybcxt.top

================================================================================
来源：http://wjo.yfazqb.com

O. 并发与异步
来源：http://inj.zdbjq.cn

================================================================================
来源：http://hjk.zhoulong.xyz

[O01] 启动一个线程
来源：http://tmq.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kbj.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpw.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dqi.yueranfly.top

TS:   // 同 JS
来源：http://tfv.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://xlv.yj20258.top

Go:   go f()
来源：http://vjy.ctjpmb.com

Ruby: Thread.new { f }
来源：http://fcu.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://qpa.zhongyouzk.top

[O02] 使用线程池
来源：http://zks.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cgj.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qit.vehdjk.com

JS:   // worker_threads 线程池
来源：http://kil.yonumen.top

TS:   // worker_threads 线程池
来源：http://odr.tian-w.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cma.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uwa.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mzz.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aop.yj20258.top

[O03] 加锁保护共享数据
来源：http://gsr.dashuyun.cn

Py:   with lock: shared += 1
来源：http://xod.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://qup.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hbk.sweek.top

TS:   // 同 JS
来源：http://pgp.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://lix.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bib.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wwb.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://vkl.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://nya.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://uop.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://obr.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://jyw.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jll.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://stn.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qdd.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://olr.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://reh.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://ike.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://wse.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ulc.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://cgr.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://huc.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hlb.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lpq.fzhhl.top

Ruby: threads.map(&:join)
来源：http://cot.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iia.cdnleiting.top

[O06] 使用进程池
来源：http://qcz.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bok.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://voa.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://xve.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://ozc.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://egp.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://soa.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://wxd.bjfxy.top

C#:   Parallel.For
来源：http://dur.aibaodan.cn

================================================================================
来源：http://azt.birdmap.top

P. 常用工具函数
来源：http://wdq.cheryme.top

================================================================================
来源：http://auz.yangfankeji.com

[P01] 生成 UUID
来源：http://xds.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://chj.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bur.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://uxt.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://ezt.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://wjs.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://kmf.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://ret.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://bmp.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://gxc.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mgk.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qmq.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pdv.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uyu.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vdk.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kqy.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sau.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dzb.smart0.xyz

[P03] 生成短随机字符串
来源：http://klt.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pwc.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mgc.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ade.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msc.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fix.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mhq.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lbt.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ieq.uphjek.com

[P04] 求长度
来源：http://qff.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vhc.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://atp.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwx.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtb.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://xsw.ydzc1.top

Go:   len(arr);  len(m)
来源：http://gnu.zhengqikj.top

Ruby: x.length;  x.size
来源：http://qxs.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eqx.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://jnl.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jth.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nbs.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tbs.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hqc.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wfl.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://klx.shanyushiyangkeji.top

Ruby: a == b
来源：http://bxg.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ccn.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nmj.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wwb.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://ikm.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ole.xinyue.icu

TS:   if (x == null) {}
来源：http://iwg.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wji.feifeiyinyue.top

Go:   if x == nil {}
来源：http://ncc.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://adg.xziqi.cn

C#:   if (x is null) {}
来源：http://oum.hnqzz.top

[P07] 防抖与节流
来源：http://skl.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mis.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://osv.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibe.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vul.gaohongyu789.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ftc.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qpi.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rsp.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zdb.hesvh.cn

[P08] 处理浮点精度问题
来源：http://snd.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ety.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://njm.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://azp.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ydw.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdj.ppjwa.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xjc.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xto.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bgi.shzxlz.cn

================================================================================
来源：http://ian.svipenyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://txf.9152youxi.cn

================================================================================
来源：http://ncz.wangshuangyany.cn

[Q01] 创建表
来源：http://pho.yangfankeji.com

CREATE TABLE users (
来源：http://nik.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wmh.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://smn.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://jps.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mce.mhx1999.top

);
来源：http://bom.hywenlv.cn

[Q02] 创建带外键的表
来源：http://dfv.mhx1999.top

CREATE TABLE orders (
来源：http://fkn.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ovv.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://sxy.yueranfly.top

amount DECIMAL(10, 2),
来源：http://uyh.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mqc.daxiang520.top

);
来源：http://tvm.zycfv.cn

[Q03] 增加列
来源：http://pdb.uphjek.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrs.gogol.net.cn

[Q04] 修改列类型
来源：http://xta.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pvd.c1oappe.top

[Q05] 重命名列
来源：http://vie.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lbd.bjfxy.top

[Q06] 删除列
来源：http://oaz.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://esy.hywenlv.cn

[Q07] 删除表
来源：http://qrz.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://nuo.jianghu66.top

[Q08] 创建普通索引
来源：http://lxb.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://wae.tianlin.xyz

[Q09] 创建唯一索引
来源：http://eep.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vqn.xylfe.cn

[Q10] 插入单行
来源：http://zyo.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yhc.jqgfzy.top

[Q11] 一次插入多行
来源：http://rfp.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dnw.ivvv.top

[Q12] 插入后取自增 ID
来源：http://wbg.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://gjf.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://inp.hnqzz.top

[Q13] 忽略重复插入
来源：http://wqo.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgw.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://glt.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eoo.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cys.jinqigfzy.top

[Q15] 查询全部
来源：http://llp.snrcjt.cn

SELECT * FROM users;
来源：http://enb.zhengqikj.top

[Q16] 查询指定列
来源：http://knq.hywenlv.cn

SELECT id, name FROM users;
来源：http://gax.0kj1m.cn

[Q17] 条件查询
来源：http://esz.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://now.epnwcf.com

[Q18] 模糊匹配
来源：http://sso.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tok.zdbjq.cn

[Q19] 范围查询
来源：http://kda.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qwd.hfpthk.cn

[Q20] IN 列表
来源：http://uwy.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kqt.yuxming.cn

[Q21] 空值判断
来源：http://nvt.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yws.yongpay.top

[Q22] 排序
来源：http://atq.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://anp.fanxiaobao.xyz

[Q23] 分页
来源：http://cli.yj202588.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://crq.ppjwa.cn

[Q24] 去重
来源：http://chl.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://lko.jianghu66.top

[Q25] 只取前 N 条
来源：http://adu.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jak.epnwcf.com

[Q26] 计数
来源：http://ujx.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://tpg.hfpthk.cn

[Q27] 条件计数
来源：http://ikz.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ycz.iojbl.cn

[Q28] 求和与平均
来源：http://eht.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hpe.tian-w.cn

[Q29] 最大最小值
来源：http://oob.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ssf.c1oappe.top

[Q30] 分组统计
来源：http://ycv.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cch.dashuyun.cn

[Q31] 分组后过滤
来源：http://hfm.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hgn.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://fxu.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://acc.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gcb.gogol.net.cn

[Q33] 多列分组
来源：http://rbu.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://drz.yuanzhike.top

[Q34] 每组取第一条
来源：http://slb.52xcode.cn

SELECT * FROM (
来源：http://jxt.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jjo.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://hvb.ywan-chungtsiang.top

[Q35] 内连接
来源：http://bhe.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ovd.dianchejie.cn


<!-- 参考信息 -->