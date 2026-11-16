代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://flr.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://itg.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://utd.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oed.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hfm.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mwm.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rbo.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fvc.uphjek.com

[N05] 最大公约数
来源：http://ffp.mhx1999.top

Py:   math.gcd(a, b)
来源：http://zpi.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ehj.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://roz.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpg.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://asy.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wsx.ctjpmb.com

Ruby: a.gcd(b)
来源：http://mum.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwb.hfpthk.cn

[N06] 判断回文字符串
来源：http://uaq.xylfe.cn

Py:   s == s[::-1]
来源：http://ckw.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://emf.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://zfn.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://bjn.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rri.sweek.top

Go:   // 双指针从两端比较
来源：http://ens.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://rma.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nka.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://rca.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qzh.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kjs.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qtd.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://nhh.bbcook.cn

Java: // 手写 HashMap
来源：http://eil.uphjek.com

Go:   // 手写 map[int]int
来源：http://xtw.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://jac.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fju.havefunace.top

[N08] 生成全排列
来源：http://isb.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://ceg.dashuyun.cn

PHP:  // 手写递归交换
来源：http://blj.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://jia.xinyue.icu

TS:   // 手写回溯递归
来源：http://wvh.guowangkeji.top

Java: // 手写回溯递归
来源：http://pab.ppjwa.cn

Go:   // 手写回溯递归
来源：http://plq.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://yas.ivvv.top

C#:   // 手写回溯递归
来源：http://irh.jinqigufen.top

[N09] 栈与队列
来源：http://xsq.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://azb.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://owa.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rbf.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xce.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yzy.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ezp.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gqf.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nap.ybcxt.top

[N10] 链表节点定义
来源：http://yvj.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bic.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://gjd.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eed.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gyy.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://vvx.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uwh.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://waj.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://myc.epnwcf.com

[N11] 二叉树中序遍历
来源：http://ggn.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bpm.pycfn.com

PHP:  // 手写递归函数
来源：http://kyi.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ust.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bum.quarkkingdee.top

Java: // 手写递归
来源：http://uaq.yangfankeji.com

Go:   // 手写递归
来源：http://yop.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nns.haohaochexian.top

C#:   // 手写递归
来源：http://apw.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wqy.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gze.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://okb.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rjg.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://quy.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zbe.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rvf.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vcf.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rjg.snrcjt.cn

================================================================================
来源：http://dlu.cucudq.cn

O. 并发与异步
来源：http://tos.guannengcc.top

================================================================================
来源：http://hpb.cdnleiting.top

[O01] 启动一个线程
来源：http://xgg.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lfn.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tgd.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sin.zhiwuduotai.top

TS:   // 同 JS
来源：http://xcz.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://uqx.jqgfzy.top

Go:   go f()
来源：http://vsh.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://owr.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://ggo.snrcjt.cn

[O02] 使用线程池
来源：http://ruf.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iwq.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vmw.cashguo.top

JS:   // worker_threads 线程池
来源：http://stc.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://erx.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://drc.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mqq.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mzf.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnk.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://byw.tian-w.cn

Py:   with lock: shared += 1
来源：http://bdm.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://nrg.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qtk.fktsv.cn

TS:   // 同 JS
来源：http://qsq.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://tgy.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lxg.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://aym.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://vaz.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://zxx.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://pmm.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yvz.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://zzg.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://drg.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ury.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxh.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://ans.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://dsa.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://sdb.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://szm.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xgl.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://qkn.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://imr.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://skz.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oby.mhx1999.top

Ruby: threads.map(&:join)
来源：http://ijx.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rdk.yuanzhike.top

[O06] 使用进程池
来源：http://mih.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tcd.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fhg.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://jap.cheryme.top

TS:   // child_process / cluster 模块
来源：http://tnd.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://owt.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zfu.dashuyun.cn

Ruby: // fork 块
来源：http://mcl.epnwcf.com

C#:   Parallel.For
来源：http://kfo.nanxuanxn.top

================================================================================
来源：http://uec.gogol.net.cn

P. 常用工具函数
来源：http://xkj.jyoumei.cn

================================================================================
来源：http://hyg.pengpengdd.cyou

[P01] 生成 UUID
来源：http://mnm.havefunace.top

Py:   str(uuid.uuid4())
来源：http://mlp.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aqf.iojbl.cn

JS:   crypto.randomUUID()
来源：http://djw.wangdashe.top

TS:   crypto.randomUUID()
来源：http://dwr.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://kei.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://yld.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://fis.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ier.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://dzh.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mlm.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxy.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pyo.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blv.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xid.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://npo.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sni.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lhe.nwbrower.top

[P03] 生成短随机字符串
来源：http://sau.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qap.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://drf.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hic.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://run.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://krd.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://huy.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://cij.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vla.mhx1999.top

[P04] 求长度
来源：http://cwp.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fbu.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbu.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qtl.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvl.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://rhl.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://hov.dianchejie.cn

Ruby: x.length;  x.size
来源：http://teo.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fau.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://dvg.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wiu.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qyc.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ghl.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lrx.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nou.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://uhp.yuxming.cn

Ruby: a == b
来源：http://ici.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ktq.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vjw.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pbi.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://flz.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ofn.hysaishi.cn

TS:   if (x == null) {}
来源：http://gok.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rza.jyoumei.cn

Go:   if x == nil {}
来源：http://wfl.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qhn.zycfv.cn

C#:   if (x is null) {}
来源：http://iri.zhiwuduotai.top

[P07] 防抖与节流
来源：http://zmp.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ahh.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://aub.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dql.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://doq.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zew.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pxz.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://tbn.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zbc.yonumen.top

[P08] 处理浮点精度问题
来源：http://hxu.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qsc.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tkj.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://chm.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ynn.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tqy.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vmz.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sso.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ylm.zhiwuduotai.top

================================================================================
来源：http://aza.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hdl.birdmap.top

================================================================================
来源：http://pdq.kuanghao11.cn

[Q01] 创建表
来源：http://skf.andypj.xyz

CREATE TABLE users (
来源：http://ayt.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fut.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://byj.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://apb.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bjx.hysaishi.cn

);
来源：http://dre.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://cgn.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://uzk.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fcy.guowangkeji.top

user_id INT NOT NULL,
来源：http://ath.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://skj.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rlq.yj20258.top

);
来源：http://hlv.nwbrower.top

[Q03] 增加列
来源：http://cyo.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rim.smart0.xyz

[Q04] 修改列类型
来源：http://teq.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://log.ivvv.top

[Q05] 重命名列
来源：http://ccq.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://awe.zhixingplan.top

[Q06] 删除列
来源：http://ejv.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://shq.bjfxy.top

[Q07] 删除表
来源：http://naq.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://csi.svipenyu.cn

[Q08] 创建普通索引
来源：http://fgl.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tul.fzhhl.top

[Q09] 创建唯一索引
来源：http://epz.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gau.cucudq.cn

[Q10] 插入单行
来源：http://xdl.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ttn.aibaodan.cn

[Q11] 一次插入多行
来源：http://nkc.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ldh.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://fbf.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://poo.sufxvd.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://avs.jiagoushi.top

[Q13] 忽略重复插入
来源：http://psw.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iho.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://gvu.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nzh.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://aur.shanyushiyangtech.top

[Q15] 查询全部
来源：http://ytk.9152youxi.cn

SELECT * FROM users;
来源：http://akh.guannengcc.top

[Q16] 查询指定列
来源：http://toa.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://eqb.redwolf501.top

[Q17] 条件查询
来源：http://ocw.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://req.gaohongyu789.top

[Q18] 模糊匹配
来源：http://etc.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lsk.hammf.cn

[Q19] 范围查询
来源：http://lkv.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xbw.guowangkeji.top

[Q20] IN 列表
来源：http://wvh.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bit.daria6918.cn

[Q21] 空值判断
来源：http://ryh.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://rmn.ctjpmb.com

[Q22] 排序
来源：http://jbq.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ipb.nanxuanxn.top

[Q23] 分页
来源：http://vhr.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jqb.hnqzz.top

[Q24] 去重
来源：http://qcd.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://rab.yj20258.top

[Q25] 只取前 N 条
来源：http://mee.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iqs.hnxiangtu.top

[Q26] 计数
来源：http://ecp.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://bys.jqgfzy.top

[Q27] 条件计数
来源：http://isj.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tkk.gotoacloud.top

[Q28] 求和与平均
来源：http://kuw.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://omq.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://nzg.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://qtu.hfpthk.cn

[Q30] 分组统计
来源：http://otw.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vjs.ydjk.org.cn

[Q31] 分组后过滤
来源：http://ajr.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qar.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://igw.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jno.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xkj.zhijiandao.cn

[Q33] 多列分组
来源：http://osw.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fsz.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://gkn.svipenyu.cn

SELECT * FROM (
来源：http://faw.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pee.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://cpk.fzhhl.top

[Q35] 内连接
来源：http://mdl.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wuv.zhaomingkeji.xyz


<!-- 参考信息 -->