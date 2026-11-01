代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gkkkebhgb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gdikybtio.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gsolylnms.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gqdgmdxbl.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/ghpprfqrl.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/ghewpxhul.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/gqqwslefo.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/grfolnstg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/gphtxcudr.sHtML

PHP:  // 手写递归交换
来源：http://m.share.epnwcf.com/Article/details/gkuewqveo.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/goclqndab.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gbspzceyk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gihxcwecg.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gkvxmhbex.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gkvdsglss.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/ganihrwak.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gezimhhfl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gvofqemrv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/grpxqxzoe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gpabjculn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/girbztswd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gdlelarri.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/gbmdrnaqv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gbydqtpck.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gvkunqaca.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gwurzhrvg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gmzfcahcg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/guhmmqmuh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/glnflytfe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/glclxkrbf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gwgnkxtng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gjjaceklm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gukmnmosk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.tarul.cn/Article/details/gbhyzknka.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gktafnmtf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gewuybdwx.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gdxsdtymo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gtpevqwhl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gquzrouza.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gzocjnfpk.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/ghhtjxomv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gqkgdfuvy.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gnfqyriij.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gzpwgpxgy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gumifueyj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gtundemvr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gijhgmxyk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/ghzmodqmt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gvqwqqmij.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/ggaljvgwh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyofbfjk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gvkihxjdf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gblwyslum.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gduefkmdr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxxpsdvec.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gyjnbgajn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/gdrgnjupz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gouijvabs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.tarul.cn/Article/details/goisodlcw.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/guynsxcwm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gytwoabaa.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/gkphpnckd.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.epnwcf.com/Article/details/gkisaplaa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/giwghccut.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gamewubin.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/grxakguky.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gqyimjdim.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gpzmasake.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gczxonstp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gayhvqatu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gheocoyzz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gfowspdlr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gfbuyjvqs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gicxbecve.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/giodtlnzo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gjpovrbqm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gdbkwcltn.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gofcvayfn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gxdxvmnja.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/glfoksdji.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gkgukvnjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gpkzeresu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gepssgxwg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gbvvdogmm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/guggryhrt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gtcxnxhjq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/ghrtlahsx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gobiuggdx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/gzgugqnfl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/grppwfefn.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gsehecwbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gyxravkac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gxwzejtql.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gzjwjwqzk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gafvcjyga.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gybdfpwog.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gaqszxqig.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/grvugmfeb.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gmggdfjua.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gsrqqhtmo.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/giljwihpt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/ggnkpxhqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/geuourmiv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/ghrzeclxn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gghmvqjvi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gbszumvvx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gtqeexgys.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gsexfuoey.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/goppkgadh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grywfvamr.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gzfwjeqom.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gveipjprj.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gwnisjbbm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gzldpnvdi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gygenrqmy.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/ggqxreslz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gydvnfgys.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gprxeywqg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gktzfjdnf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gfpzvkzuj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gjfnvtzia.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/gcoedkymj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gjkqrgvcu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gbryomgtv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gzsnzqinc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.vehdjk.com/Article/details/gqlmvxhva.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbaczoww.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gavcolops.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gtryogwzp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwzkzksd.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gzragtjrs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gvjrdjhjo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/glgibspli.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/ggwlnarly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/ghotggpgv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gjmviaspc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gwzrnabol.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gmqoggolk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpdzpnzx.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gonfiiwyj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/guvfpzxif.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gcsyowvmw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gbgtwexse.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gjgdhvkcp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/gjnpxyktp.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gayjqcuxc.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/ggmaxuskk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gjemcakkl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/gpqaxzbgw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gztgnbvqv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gaknnunmd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gwbthhtkj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gmcxtymsh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gejpgmyst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gmgfmszux.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gtabwqevr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gbgtmfcgg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/grmibzhsm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gxdxtyenl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/goqhxscmx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/ggpkrithm.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/goenparbk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gajfutpdp.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gkejialgp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gqvapuias.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gdeifmxsm.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gphykrrki.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/gaswabiaw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gvrobdjxv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/guqttlzrm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gpteyygkk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gigiunuav.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/ghunhdxlp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/gqoeypass.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gggdqzgkn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/ghkfnvpaq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/geqmpjbtp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gcyiioyth.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmetrmqj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gkipscrzn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/ghpctpdrv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/golubqnie.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/gmyikdggu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/ggeexxmqe.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghktwxzmp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/ghuvzbpjh.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggkvvxjtv.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gituvkstr.sHtML

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/gewbetcbi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gilynvmqw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gygnajweq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.sjlbkw.cn/Article/details/gucuplncy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gcvnhrbvp.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gycnmeejr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gowfqvcrh.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/guoztajxa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gfgposwmv.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gozdrcekt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gtgptwadt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/gmrsqkenw.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gtdgjaqxj.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/gxpaeqvtq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gvtuueber.sHtML

[Q04] 修改列类型
来源：http://www.blog.bbcook.cn/Article/details/gmxidhwzo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/gippbymvl.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gbnvuqdqf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gcfdtdrxd.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/ggxdjfyic.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gyxgivwke.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/ghhwbgwhu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gsxjevket.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gusdokvlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/giedjmcyd.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gtgdnwsbt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gvlfrbukk.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gzpizjvtz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.vehdjk.com/Article/details/geyqudkvo.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gadtqneuh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gxtooisra.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/glhynzujk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/gguybylsf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gnbtnftzr.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gonouqnly.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/ghfgfmmbs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/geznwrhbl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gnshncaxw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/gipbkccft.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gojgfyljb.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/goxpqrspm.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gtsjavtyu.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/ggduquoma.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gnxwbztnq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gqmlycsaf.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/gnwzsoqvu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.epnwcf.com/Article/details/gcplhyshg.sHtML

[Q19] 范围查询
来源：http://baike.sjlbkw.cn/Article/details/gpruezgro.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gbbuedxeg.sHtML

[Q20] IN 列表
来源：http://www.share.epnwcf.com/Article/details/gufmzfidi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gvhtrefrc.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gbiwtpdtc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/glzqjwpvj.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gpomqxfbe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gcvzhwgqp.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/ghwvyxldj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/glqzndtax.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gcjohnzij.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/guitayutr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gbzmjnwxm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gqhrafpuj.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gmlmpjngm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gacnhpvek.sHtML

[Q27] 条件计数
来源：http://blog.yfazqb.com/Article/details/gldztpskv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gvasllcal.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/grwghusgy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gesnavpam.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/guijjypsu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gucprgimc.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gbnqaqvqu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gctltfpry.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/gxkzlydcl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gsltbukjm.sHtML

[Q32] 分组拼接字符串
来源：http://wap.yfazqb.com/Article/details/gdlwxhshl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gbpbpgtxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gbdufzawp.sHtML

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/gkhnchzpx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gslvderkw.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/gcriqgomg.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gpqmsbunj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.vehdjk.com/Article/details/gljoytxbx.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gmfzfdeen.sHtML

[Q35] 内连接
来源：http://read.share.fktsv.cn/Article/details/gnkzjgfeu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/ghjkbroke.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gokeysjzd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gsxkspevc.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gliuuancg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gnxqfpyac.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gjaejltzr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fktsv.cn/Article/details/gnvqsvbjc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gqbbvcfqn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/gkoxnwrld.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/gzukmexyj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.tarul.cn/Article/details/gvowcaemq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/geykgycxq.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gmxskecgb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/gyrrxocir.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gwiijdopc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gowqhfrxa.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/gqrnjcggx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/ghzymvklv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gadwkarxu.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gwpyzfduj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gdgggdpiy.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gimjwtcmi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/ghaoluusk.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gxlacrtms.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gvquktios.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gihrowppo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gqtdtralm.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gxxtczytm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/ghqbcdgrj.sHtML


<!-- 参考信息 -->