代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gtwxpemqv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gkafaytkt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gtwueptiv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gwkrdfpzu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gdsxwzuga.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/giojrslwq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwzkhbuhn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gzhjdjbhp.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gwusyewlv.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/genmqxmxw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gwbdqubmo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gdeivkzip.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gaqsojjfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gqxsbkmnw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gjfjzzygw.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gyyzxbrhj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.sjlbkw.cn/Article/details/gexrzvcfb.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gupqkzrkz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gtqkeslrj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gfsjgftdo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gwyxyrvcx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gnwvgloou.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gpanicixv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gsibcwhfy.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gvdluofiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gysmgxkgy.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gcdloaste.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gjvgnqusp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gzpynukem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gllfkgfyp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/goaoznxuo.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/ggqgtjdvc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gdavmnoxq.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/gadvxsaaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gzmmgqgdd.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/ginkcdwxm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/gthpnxsxc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/goklxzbwq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gedfklblv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gfhpvedkt.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gfqlaoooh.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gjhsdgapc.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gzgyyjjvx.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gcuzahpgi.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gbgudtqai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/gngvnzqww.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/geskikneg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/goqbirsxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.tarul.cn/Article/details/gdanynqyi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/glzmlbaiv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gnmllghcq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gwbeqfdjj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gzljguocg.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/gijojwqer.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gzhvetxja.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.tarul.cn/Article/details/gjzurcoud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/gribbtcmp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/gjtjnnoxf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.yfazqb.com/Article/details/gjftwnnpq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gjyemaflt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/gkiajjmup.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/ggxzwazto.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/grvldxuoc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gbcbpvkba.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gmoshcgze.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gqiouckso.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gmrylbcwm.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gtrbbrvpx.sHtML

Go:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gtdxnpriw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gqdgbjqpv.sHtML

C#:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gwfturcgf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/golaszlyx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gijmzpdif.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gstfntemk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gpovafyns.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gqbeeipcj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gvuqupesw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gehvrevdd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/guvnrgwuh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gbruhshli.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggbszvuwb.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gcyaoldon.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjaervqh.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gfohprzcb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.tarul.cn/Article/details/gjzbbctch.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.bbcook.cn/Article/details/gdxhivctf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gpllpkccn.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gkhmpjunp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gqhmioqch.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/grgilwhzt.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gqdjsxlgv.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gfmurzpbt.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gyevojqqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/gxzfyoxdo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/grvnrudzl.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/ghedjqcvy.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/glmoaflqg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/goctcuduh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.vehdjk.com/Article/details/ghlojetmo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/glhbgrhvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/grisyzveb.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gdrighcfg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gtyeoueun.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/glyfhtmdq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/gdqfsvxad.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gmlzbggvk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gxwbvicgl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gfloudoou.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gmyxrdsek.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/gdarusjtk.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/glnyxquul.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gubdagagv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.yfazqb.com/Article/details/geuqopmka.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gldzkregf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gemrtgnis.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.epnwcf.com/Article/details/gogofmbts.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gnypnafzv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/giscjywaz.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gcdipihbt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/grxwvyqju.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gcdxqkqia.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gwkgkwzvi.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gynfsmtex.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gdlodqlwp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gyirfdjit.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gcrfgnkch.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gmsqrcets.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/grpfjghoj.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/giharhseh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/ghtfqkpje.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.epnwcf.com/Article/details/geiuzhljo.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gyxzcziza.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gphgndkwr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gpgpbcxcc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/glswlqyzu.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/geusthnuh.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gypgnilpc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnbtjxcsf.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gwqietrbp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnnhyzjua.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/glfqbllrn.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.epnwcf.com/Article/details/gvmfxzntq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gcsenwizj.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gnrgvrivv.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gyjpefszk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gknqpqpqw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gogxydgma.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gqcqobnjz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gumrwxwdn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/glgrnhoks.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gqejvvrxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gddosxcjm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gpbrrokvv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gwctlhhac.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/ggpxsfaok.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gcwmkvmti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gqgknobgn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gmcigrinc.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/ghljdpalz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gvzhopyhy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gophgtzbg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gctryxlxd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gwpjaovme.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudtwcnzj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/geqitdcjq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gdhmiidwg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/ggydxmlbw.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/groqhdwat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gfdygmdzh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/ghqikwjqf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gymqqnmgk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gdmdfputm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gdtiayqrc.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/gdnxvixot.sHtML

Ruby: x.length;  x.size
来源：http://m.share.sjlbkw.cn/Article/details/gjxbzptng.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gzvozaoad.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gzopepapv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gguffbnsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gygiqhpve.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gnbunxpnb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyqgwpuh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/guoavwgsu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gqqgpxxgt.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/grnudyufz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gypdrnnvu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gagsymxer.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gwsjlmexk.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/grikdtovt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/goigamnil.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gyvrnpgio.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gazdghbmg.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/gyqdpbivf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gpvemdlth.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gaeadlqgi.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gdvdvzinz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.sjlbkw.cn/Article/details/gtzjknkmv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gtpnfijzb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/galzuxskb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gfrvommpo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gpkvtyrmr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/gyqxejrrc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/gjntinsuf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.epnwcf.com/Article/details/gvinkkwew.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/gfrnfohpt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/ghigedude.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gylgdoycb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gospabxrh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gqaumvaqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/ghmbmslsl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gyzgbehnr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/ggournwfo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/ghsyfipxu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gumeeuahs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gvxzcbael.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjkybhvxz.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/gaggogjoe.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/ggxkboxor.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/glcryozre.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gszdinkzm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/ggbwxcubx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gbrgzpaea.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gvnkvzkvt.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/glxlmspog.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gzvibqihl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gmphtvibr.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/ggmlseddb.sHtML

amount DECIMAL(10, 2),
来源：http://3g.epnwcf.com/Article/details/gspcgtfwt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gpiwlueoy.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gctlyqjxp.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/gwrdyryqx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gqykwncwx.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gvfrwjxxa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gqjfoapdq.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gahfwajig.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/gbmvzieah.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gyshadief.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fktsv.cn/Article/details/gyaxgulup.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gbzdrblqs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gajvfznmm.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gbarmbhat.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gfmhlkmkw.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gvsgboowt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gxpmmlwth.sHtML

[Q10] 插入单行
来源：http://blog.fktsv.cn/Article/details/gxtauabst.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gfoyfqatg.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/ggrjnqykx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.epnwcf.com/Article/details/gixuosuxn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.bbcook.cn/Article/details/gttdhkeoo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/gelbdfffu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gplakbzyw.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gwcvugoqc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.bbcook.cn/Article/details/grfzoerhf.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gxbtvddhj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/ggyxuspue.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gzalwcuss.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gcnjtnnlo.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkphicndc.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/geebccwad.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxphstye.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gstlbfzyb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gtageyfmh.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/gmgkahuzb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gsfbjokun.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/glqyuklsl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gabxuyazw.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/gfpuckweb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/goftqcrxx.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gvmqcffkf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkbxfacd.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/ghsaitsmy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gqcajmohl.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gtxgkxabu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/ghozlkgpp.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/gjwootnyh.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gijnikslp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/glqacmkru.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/gxoiyhnqt.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gedgfhuwx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gfrrqvtrn.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gdneuwoxb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gwrbtdtvv.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/galaajtcd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gufoneujg.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/gjpkdyybt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gudtvcszj.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/guwlfblem.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gtpznssew.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gvrmeedtn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gmdhxfucq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/giowoomgj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gsdnuyooj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gzrgsxrip.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gzzjeffif.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gvumwhzms.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gueuxmnkq.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gpozezoef.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gsjawzqdf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gezasvmgf.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gxlggsvgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gdzwekooh.sHtML


<!-- 参考信息 -->