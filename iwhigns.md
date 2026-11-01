代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gilsapolm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gqwxtrrfz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gkfodjbuf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gexohrfjj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gmsoedxzq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gdzpkglud.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/grmhjvwpb.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gvmukxraa.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gtacirocf.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/glfxdyysw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/groinfemt.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gwhippvnb.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gnlahjwgs.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/guirmeqip.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gdaewmung.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjgizvghv.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/grwuhdfhg.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/ghgiyinfw.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gabtgxloh.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/goexocwwx.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gcakmgwpg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gxpstgoos.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gdmaamwid.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gzgwhcgdf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gacfwiohy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gidtrpfvr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gvvhmujca.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gfzdhgkev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/guerivmzj.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gqdudhbmw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/glocnyfgp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gxagoglyh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gwqlhgijs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/glwyjtkdp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gsjspkbfe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gdarcgalw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gppanyxdz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gositaagb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gpkmhyqtc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/gdzbqpavv.sHtML

PHP:  // 手写递归函数
来源：http://wap.epnwcf.com/Article/details/geqondabp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/ggtxtaarr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gqxfpnqat.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gnizlsdwz.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gcxaxuvea.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.sjlbkw.cn/Article/details/gabimdmey.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gbanhbfap.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gjzhmfupg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gcmuqqaqh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gealxqtaf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gqhobpdkz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gcuprtpaw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gdfaivksr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gsagtkjjp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.epnwcf.com/Article/details/gtaaiwzvy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gttpzfrss.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gynwasyja.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gupsxjlsc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gghsudomn.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/gjbeizgek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.bbcook.cn/Article/details/gnthzuqng.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/gvuakekrc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/gmbnzjqfq.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gglqijbes.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gwqrfeuwu.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gczeaulsk.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/gdsgxggdi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gvnjpcqeq.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gbgsjrcpq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.vehdjk.com/Article/details/gmmxznhhl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gwtlodxcn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gjnibgyyo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gnewxfdtc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/gofqqtrzu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gjgcbyfoz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gexzaesbz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gqumsguab.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gyiqcajtm.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gqylsjyde.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gxtnqqerf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/ghunvyzws.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/glrejzktl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gwdswpiza.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/geerrhluu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gtyoefsth.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gvqvysibm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gscamyzdm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.tarul.cn/Article/details/gdfnxzipx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gisczvkow.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gohuhhewm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gzgcyjxxt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/gcxcnwpoo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.vehdjk.com/Article/details/guytjakim.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.bbcook.cn/Article/details/ggfexiwas.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gemnotnap.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gcbpdsxjy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gghumlbxh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/geunjglsg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gdcvlsjzd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/ghudvgqyw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gwmreecxw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/ggtabgjpm.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fktsv.cn/Article/details/gqbfrbixu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.bbcook.cn/Article/details/glukqeqse.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gvvglqjdm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gddgjxgzg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gzvabbhem.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gphgliwzx.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gsswjwutr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gjrlmalqe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/glutwypkx.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gtctaoiep.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gplqzphoj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqfejkxvk.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gknjcawlf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdegybebv.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gdaudeqej.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.epnwcf.com/Article/details/goevkusnd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/ghntaqqnz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gwkiggfgi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gpgdzwxli.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gustnjgdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/genoqfwpv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gzuqpvcem.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gydjyillq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gxzplozpo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/gbdkvgucs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gslgkybol.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gmohgjsyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/grkkskxdo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gnnzsxjkk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gyqrfauah.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gpngyvdvy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gqbfckhty.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gkfdsghca.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gensuanbt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gsmqehcyj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gkjvfbpwo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gjyypyifu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gcnkqavlo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gypsrvbyn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gaxkczkig.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdfgyuog.sHtML

[P04] 求长度
来源：http://3g.epnwcf.com/Article/details/gilgcqvyn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gdsznsdrl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/grxbfjlqo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gecspbeoi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/gzxrbmqlb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gxvdimatz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/govybwgls.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/goovhybce.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/glqctoifv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.epnwcf.com/Article/details/gncrpphka.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gcqnojaly.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gkfeqjntg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.yfazqb.com/Article/details/ghkqzeqtg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/gwbjevvrz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gmqmoxxxg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqpyzxge.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/guzgfxkko.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gmpqhreof.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/gfxdfyxqk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.vehdjk.com/Article/details/gqydyewey.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.yfazqb.com/Article/details/gkevkvujv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gsgicciad.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gmlsdmkcu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/grhjykspx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gixmlptxq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/grjywxlxr.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/grikahtka.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gdjqxsgrr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/ghooarvus.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gifupbuaa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gcvydxkcp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gtpyrbnjk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/grzudhdaq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.yfazqb.com/Article/details/geczcrlwv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gqxuxxqlk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gzinzbhva.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gcgorcdjr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/gyewvxhmd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/gmfrpqglo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gdturqaal.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gaxaysosf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gcasfhugw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gqhwicakm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gcgpjoiwd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/guiiwailp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/garribqed.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/ggzavclxf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdmhfedcv.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gkiftiere.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gwqupzzxy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gsdtmsnny.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gnelvobbl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gfebiufjr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gbbxwvnab.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gzmhdppmk.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/grppajnut.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gplmssede.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gwvtazyki.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gutjlknhq.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gzaqocxfv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/guyjduhib.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gkixxnmwj.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gqqharrpd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gecdqlbwi.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/ghutaxgid.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gcugpxbgl.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gxcgrtgho.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gwoojgltx.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/gxwlpsbgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gyvtcblfs.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gzavkyhgc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gcarlvnqb.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gbjuingkv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gvkrzthvo.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/gnyrugcgy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/glvzwbamr.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gsngmfdqk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.tarul.cn/Article/details/gdbhybvhs.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/glyhgaduh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/giobflvcv.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gjvryhijh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gdzgunjxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/goqportyo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/gmqxqssed.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gptrwqgqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fktsv.cn/Article/details/glnaohlfh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gtxzxxsix.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gvgxxyxbk.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/ggcslncru.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gogmimgmp.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gglttczwk.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gjkydovmr.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gactbobvk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gfmrudpui.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gtoswhukw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gljeqimyk.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gtncsnqrf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gifglwtvf.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/ggaagfqcr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gkijtiqig.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/ghpghnpub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/gbssrcqir.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gwgdowmno.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fktsv.cn/Article/details/gfkhaotft.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gjzvgnfqw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gcqskadsy.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gnfmnlnbw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gkvaxlfkh.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gfhmczirp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gmzhfiniu.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gikmozmmo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gnpzzspih.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/gnxubmoym.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/geytsbljx.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gywewkylv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gtbqzkbbg.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/giwcblpyr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxbjmfubl.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/grhenrpyj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gywtouwji.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gooycwdvk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gbuknxljh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gmfamtsdc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gdeftzxin.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gsuwbuxne.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gshyetvjk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gdjjfrjsw.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/giidgvzqu.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gomavqwwe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gcxvfbffp.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/gwxrlbien.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gggegcvwo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/gmglwzxyg.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/gnrrxfwqc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gqwalqeuy.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/glhzutdtg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/grazofhgf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gegkqqvfs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghreytphy.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gpwkvuefb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gvevdqsnq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/ggbzojlsw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gzdrkzjvv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gvjlmkosp.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gekqfhmye.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gmgqemykf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gamztfuwx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/ghjdvsdaz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.epnwcf.com/Article/details/gvvttowrw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gykhpspnv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gsvacteko.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/gcerbomso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/goyvtnnkl.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/ggflsrpry.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gdcxajbls.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gnofaemrn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gcgpwpogz.sHtML


<!-- 参考信息 -->