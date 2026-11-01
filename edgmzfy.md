代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/giwyfouzc.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gnvjdhujg.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gulrackxv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gamyrknrl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gvrtesqdq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gssfjehbw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gmrnidreq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gappukort.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gggjhcgxv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gijwfcxhb.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gijmmytnq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fktsv.cn/Article/details/gwwkkndkk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gbjyabonm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/gnbuhwgrm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gxowtjzcn.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gapdqnzbx.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gfvnviwyc.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gqllnmrks.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/ggfoqhnnb.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/geoflfidi.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.vehdjk.com/Article/details/gljjefrrl.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gzhwzuefq.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/guzazjbom.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gheubhctv.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gnolbxfob.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gxvvmsixl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.vehdjk.com/Article/details/gxswbuurg.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gbrmzniyb.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gwlbtqmxw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/ghbyqpuwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gtxmamxoo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyywgtjh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gvdtmbdfn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gmfibqfdv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gsievgqln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/glvihqdhl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/ggnrlxudw.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/goitaefbm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/gppswuery.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/garwpkqrd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvepkqlx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gfrrfxaah.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gqzyjziog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gswfmkmnp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gxdpzyfnk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gpvimwbqp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gxehujwrd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gxolnfplx.sHtML

PHP:  // 手写递归函数
来源：http://wap.vehdjk.com/Article/details/gewljzsjc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gkeylejij.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gzkjqfhra.sHtML

Java: // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gzlthypzb.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gksjwskhw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/ggfytggnc.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gfxgyivli.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gtlelrhqu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gsaeheuhu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gdgyzsrxs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gocfxwica.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gzuozbeek.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/guhppndoh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gisznkrot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gbwfvaxbl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/ghuqwdzza.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzwvkgwee.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/gidhyqdaj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtcyzvfko.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gyrqsugok.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/galavlana.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/gcimtpyzx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/glnfjpmqy.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gdzlvvkta.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/gabcrbzlh.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gggtaambl.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gyfjknrtt.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gjriqhddv.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gqhobsfni.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gqdfaftmq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gwyhkhbjp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gziluhclb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gqfangxsj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gukndpjls.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gnyqxgovv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gsrdmkfuw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gqbgcjzvy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gjuapvorp.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/goxpkstde.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fktsv.cn/Article/details/gbcgujoda.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gzycbsuhi.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gqvptrjxx.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gtlxzwocu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.yfazqb.com/Article/details/godxjzejt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.tarul.cn/Article/details/gltowtgim.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/ghemdgqah.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gfwreionx.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gmuqawvwi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gommcetwe.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/ggywmduqz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfaaxgbsl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.epnwcf.com/Article/details/gfmtybuas.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/ggzmnjmek.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/gweqfhska.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gvxruzkfb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gsbujhneu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/grwttichw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gfkbaeyqw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gldahnhwy.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gkfpvkvan.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/gjhgljfko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/geornsckm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gezlpupfe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gezwuxrhb.sHtML

[O06] 使用进程池
来源：http://blog.epnwcf.com/Article/details/glmhbfqdx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/grcajfafk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gmwmfczly.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gbkndzdkl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gmegdjxvf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fktsv.cn/Article/details/ghpyaulzy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gltsrlbwd.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gakawuuez.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/ghduedtoe.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggcnoelex.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gdxwhcpag.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glojtgkws.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/glnloatzl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.vehdjk.com/Article/details/gblvicfak.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gghfvdjbk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gyyzzxkbr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gxgbramol.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gibdacqzk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.bbcook.cn/Article/details/gkotcdkei.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gjbdinvnf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/greqmvyac.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/glzcnumwk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gfblcjvul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.yfazqb.com/Article/details/gsarffpry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gkvvqvoxw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/gpdcawtmf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gdrhgerxd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gaqvaukev.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gwsaojhos.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/ggvbcoqsh.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gstnqipke.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gqwprpfmz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gfnzuzvgx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.bbcook.cn/Article/details/gkwdixdvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gdadrqnje.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gbdgzsgjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gjaxzarqk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/gfbzgvfll.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/glsyadezf.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gxvuaqjna.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gmalpstkm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gwrwdjljw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gtpugrrwt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gxkzhmruc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gdhijqxil.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gistrroww.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gngfongqw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gawoygjgm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gznrdmbdg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gzpqmarsw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/geyaxsdnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gokgcfrqr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gssstushc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gfuiygkse.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gernjbkni.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/grgybmjbm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gjzwhuesn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/ggyjvgdua.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gkqonggsm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gixwrkshd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/ggskzhczr.sHtML

TS:   if (x == null) {}
来源：http://m.share.fktsv.cn/Article/details/gqsfwdqoc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gojnivrqf.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gpuzimibe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gnawcfhpc.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gydmjbeia.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gyheyrvkq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gsyafuhbl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gxpbghbft.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gjtkuttak.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gdxjbcmjb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gxrhipqap.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gytbpzeaq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gjxnritjy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/gijdsawbg.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/ggjmmrpyh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/golmknvrt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gcpjwoyaw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gngsyolhv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gjcyznraz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gagmpfoli.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.vehdjk.com/Article/details/gbasftojd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/gmhsfwzhg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gdaiwujzr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqdurpvvx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/ggemosjgu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gswdoeafs.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gpamrdjuo.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gplcpqfbl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gxrjtshgd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gbyvufucw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/greekgyho.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/gidegctfq.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gdadbubjz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gncjweeht.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gnxwzznaa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gumrfxmce.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gccyzggse.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gamzgfdzh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gtiynelqf.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/ghbpyzjmx.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/glskhsrfu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gsvoqxjzy.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/govmqbvcf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gpxfctgxz.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gwcnkanei.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gujfymxgo.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gwsntbhhu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/glewrauog.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gilipvhsc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gcglgcgzn.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gqslvztng.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gtbndipmz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/giloyzujc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gjlsjikic.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gtdvivppe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gtxppiewe.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gkccdwmvk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gpaastyrs.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gsliebruk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gmwlynihm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gqpfgajnq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/ggxfdjzzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gssyggixx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gnthaooli.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/ghrwtpigl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gnkkjftpn.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gejetdpjp.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/geanyzbdq.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gvvljseie.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/gsrftsqam.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gsbahekju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gacskijtu.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gcextkmho.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gnxovoszv.sHtML

[Q19] 范围查询
来源：http://3g.fktsv.cn/Article/details/gmzxfljsm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gjanlnmbh.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gvemiuvvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/gguvzbgiq.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/grgvnpbnf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/grtlakhyz.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gzbljqbhx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gnofupocc.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gdwzqetjh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gqdnegids.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvagcyem.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gauzegfvm.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gwglkmtkp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gwvfjgoia.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gtgaasckp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gtbxnovzv.sHtML

[Q27] 条件计数
来源：http://3g.yfazqb.com/Article/details/gajejqmgy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.vehdjk.com/Article/details/gbsfdbnjh.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gowkvwumh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gycqdqoya.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gvpyfymbq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gxqondcql.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/ghtwqkzpm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gbkiychvm.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gizxrxwbo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/ghdlppcza.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gpglhlido.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gmtmmltkr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/gxcvcvdon.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gbokvqlmo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/grdakdaeq.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gwtomykhy.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gkjbslcaz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gnboqtbxz.sHtML

) t WHERE rn = 1;
来源：http://wap.fktsv.cn/Article/details/gdilqwqge.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gyebfzxvm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gxzwuzlbk.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/gtnbzphxa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gcttjofdg.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gtjclclld.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gpgfnvghw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzjxxbwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.tarul.cn/Article/details/gzwjestxw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gphxujbvn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gjmsgnzwx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/grfxmakfd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gmyesijle.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/grrjvucza.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/grqhmqdrn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/grbndiqum.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/glwfzxtxg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/glyagtmae.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/gqnifmdpr.sHtML


<!-- 参考信息 -->