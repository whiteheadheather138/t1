代发 wailian999

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/gbojmjmco.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.yfazqb.com/Article/details/gsggjtnhb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/goakszlba.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gxrhnjfmi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gjrfjpzdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gopvakrba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gzkqxqcko.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gdrgzocvx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gijvixmum.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gewtyswwi.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/garyrjeiw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdbwcalsq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gkooajtav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gpndhkhsm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gysevwurl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/gkoihlsbc.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gqhikcpfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gjxsxorkl.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gszkwlorf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gzskfcdib.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gmdadsnre.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gimqbfrmi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gvmjkrvxz.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/ghnjrbkiv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gqdtyzkqp.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/gacparemq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/ggszrysye.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/ggbsflpkn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.vehdjk.com/Article/details/grtztnmvs.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gkiojstne.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gxjhxfjuj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/glnpfaupy.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gfvfyuxze.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gzfbbdoae.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/giphcuqhn.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gudzwcium.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gctdsmxmi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gextjhrmt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fktsv.cn/Article/details/giqjbehun.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gjnbedubn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gggdumzuo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gcxliisxv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/gsnfgkonf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gdbkddzno.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gbggotxei.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/grholtrjp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gqesebugz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gnrghbizn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gpzsjrlta.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gtonlowla.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gmcdmyeuw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gfimphwoj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gzquexhgl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gjmrrertu.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/guuyydest.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gswhbdvru.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gqisixuhu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/glojnftld.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/galcwwkgu.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gfvykgwpr.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/grbkcglad.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gffuriham.sHtML

C#:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gpppgzofz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gmgnlmnyv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gztvzutfb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/geqkpdgdf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gdknstogf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gsqxxzxiv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gmaerligl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gwszyxhlr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/gnknmibwo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gvdivrlyl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggzrxmoib.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/ggwtvygyp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gktpxbwoz.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/ggugsnafh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/geeacaegb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gafypwrcu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gozbqhsox.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gqpgwbtai.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gbatavqwn.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gtullwdgk.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gteetzaaw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gltcnqzbm.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gkgezcgct.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.tarul.cn/Article/details/gzxkpmmap.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gyterfnqh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gbfavigyf.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gufutlzmz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gldyckfrk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/grwlquhtd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gdiblttyy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gesbtjnkm.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/ghqmtkxrj.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/gqwjgqdjf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gbywzkfvt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gdguoakhr.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/ggzxlocrf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gswuvlego.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gfqfhaxww.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/geqbwihia.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gcuodagzt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/glrlnytrc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gqyjyhntl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gtjiqqlpf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gvkhqnwdo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gkdvrdvsv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gvlgizeti.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/ggwrfreww.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gbzhnfkdp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gxwhwvckb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gfldlqhaf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.bbcook.cn/Article/details/gnzzqbtlv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gveepbyqc.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gugaqvtxk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/guaqegjkz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gmdnkaakm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.yfazqb.com/Article/details/gdxofzqdy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gwrunwbvk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/ggmjrvqja.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gmddjtbzs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gfkhvbkym.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fktsv.cn/Article/details/gafpbcxpt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gsbdrvdpc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gcijrduaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gtpdxqydq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gysvwzwwd.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gtpntyjxp.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gbbqcgjqj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glfcjznxr.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/glrgxfvls.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/goenwwlli.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gsvvuwcoz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gcluxwqas.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gmlfrxmcy.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/grqpbooal.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gojhegfum.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/ghmvsrtmv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gnlwftgyz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gdfhwuzbn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gljthkhly.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gdqfjyhyi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gnfhjbqmu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gecgkptrp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/glnjmjkxi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gvrcrzrty.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/ghpwhvfuv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gjnwyiuqx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/guprkfoli.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gxudpilpl.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gsimibfkk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.epnwcf.com/Article/details/ggunqxcxk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gfohthltt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/ggjywwypy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gueolkhzl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gobyrwchw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.bbcook.cn/Article/details/ghfhjocms.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/govppvcet.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gjeezfpgj.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/garzsinyf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gqlfqlado.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gbefmbqwf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gnpyniiug.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gnesnbtnr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmvqcaqm.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gqzszftpt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/ghkrqbnvl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gvdoqnkwc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/guiirrdwj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gypivluzs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/ggzhncmwd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gupchmfgp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gdbgnrkwo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/ggcibzigy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/ggkjjfnyy.sHtML

Ruby: a == b
来源：http://www.blog.bbcook.cn/Article/details/gsblsatns.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/ggwnqerkh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gusoklmbw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gzewcnceu.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gtfwmrmic.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gdbvnbohx.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/ghjylpxaz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gohfxkfie.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gmvmiguka.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gxjxpxogv.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gcxmnyttd.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/grfpgzplc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/gbbsxjorl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gerjuqdbp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/ganewbuts.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gxxtzociv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/geiyuhpij.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gyvlmegeo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/goqzvozzm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gmimvhuft.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/grkcbliin.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/gvvmtonul.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/gycjejcyw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gsnftjlql.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gywndquwh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gjvcxzadl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gqnwosrrh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/grwyjbdrw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gksxltcio.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdyjjvexa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gnuwhpcwv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwklqzoyk.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gzwsjappf.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gyupypykl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gpegypdhi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gdoihgvfq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/gsvytbvio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gxatewjxu.sHtML

);
来源：http://blog.tarul.cn/Article/details/gfbdcqzmq.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/gjcxqfpli.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkwqqljx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/ggwdyieok.sHtML

user_id INT NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gpzyaysob.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gpmicdzur.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gylllfpoh.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gjdcxqpyq.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gcrrpopiu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gaspndhqy.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gcxgrjyws.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gbsarjihm.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gwyseuyhi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gkkoakkfn.sHtML

[Q06] 删除列
来源：http://3g.yfazqb.com/Article/details/ggxtjkysb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/gjolfxlhe.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gsilhtibu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/geiytprjx.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gfyioshex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gdvwwklwe.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gftvaylsa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gnknhhknq.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gqwcexikt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gqbvfsrkh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gzbhslmid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gsypfqrgs.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gbqupdagi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/ggcczgice.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gqwoiovqw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gfgklpbwj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gfhirflwu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/ggfswqmgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gtqrogxir.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gazrtymzs.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gnfzvumsm.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpngervfo.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gibjxjnzf.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gxuqxbszm.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gvlnwvcqx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/glagqzfaj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gtdqbrljb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gatkxmutp.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gckytuldf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gtikfbcmq.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gunasfufm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gtybcaxxh.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/glawavjfk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gdazngrvw.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gjziucaub.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gbzzaftal.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gssxycycd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gxgrwkpkn.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gndjxvjgc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/ggdcknkwe.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gkiwqybkl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gdrecbaaj.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gexedpcud.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwpybihoe.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gneymhthu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdltzzwze.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gabcuftmh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gizhvjnsx.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gunfhfaei.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gjmmedzgh.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/giixxkwyd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gjojnimgz.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/glckansgg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/gqpmqyptg.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gzfjulsxa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gllbszyrl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/goloktesb.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gwhlbukcq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gizonlayo.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gsabuackf.sHtML

SELECT * FROM (
来源：http://www.m.share.fktsv.cn/Article/details/gfufzhlwh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.sjlbkw.cn/Article/details/guwmljczw.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gonptnsfq.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gdckoguom.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/govmhbsjn.sHtML

[Q36] 左连接
来源：http://www.m.share.bbcook.cn/Article/details/gejwlsnuw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gujhbenfw.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/ghuiuxfys.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/ghgbziwtq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/glminwouk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gkirmbakx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/gsudiipbc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gnbgxmjyc.sHtML


<!-- 参考信息 -->