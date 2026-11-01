代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gmbuqyhxs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gdjkjmaty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gbtnpjefv.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gnwqppeit.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/ghlhwvwrg.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/gzbobceug.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/glnrxlrdy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/girmckbnq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/geiersnnj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gkffptypk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/gvmgkwaxv.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/getyenwul.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gycrugguh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gxrxcaqso.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gqtyuatzv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gebgfwazo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/glufngvab.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gepunemum.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gmwbkihvg.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gedvbgifv.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gvzswpbpq.sHtML

Ruby: // 手写 Hash
来源：http://mobile.yfazqb.com/Article/details/gvbjbaqys.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/glpdmznja.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/gckjntgca.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gkpdquywq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gzjxpdwpx.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gvykmgkxs.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gnsmmyolf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gjxgoipby.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gnvpooddo.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.tarul.cn/Article/details/gsvaqtduo.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gxvvdnvvr.sHtML

[N09] 栈与队列
来源：http://read.share.vehdjk.com/Article/details/giudkagdq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gricneyez.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/guhpogliw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsifuvxqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fktsv.cn/Article/details/gyhtepnyj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.tarul.cn/Article/details/gskxuxngu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.sjlbkw.cn/Article/details/gutkbqpiw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gzycxtnpd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.tarul.cn/Article/details/givpkgial.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gvevfdeqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gskxflqmb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/guwwepaty.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gmkhlhucr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gyyjyuokw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gnmbxbsql.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gguumalmy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gtlcoapvn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/ggfkowivt.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gnolotmag.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gvwlueyyz.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gqiqlewku.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gjbwdewhx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/gkqnvrpvy.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gsghckkzp.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjxzxubj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gcsqgqwcc.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gobqinvwf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.sjlbkw.cn/Article/details/gxjurbnmu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gwxebdinr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gvbtomysh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/ghbgtnvac.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gibizarcs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gyzbwquwt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/govtwvdxr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fktsv.cn/Article/details/gawptfcab.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gqxsaiqwr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggbtjppgr.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/giafxpwmy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gailzjpal.sHtML

[O01] 启动一个线程
来源：http://read.share.epnwcf.com/Article/details/gmkyiybgm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gsjfqpwpc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gypjiqavm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gcnuloasp.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gvpgomghp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/guvuqrkrg.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/gjylenzzl.sHtML

Ruby: Thread.new { f }
来源：http://wap.fktsv.cn/Article/details/gxnhvyfne.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gxzecnxzm.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gckbropzv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gzyuwzedn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gnfvldpws.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gzyqjzdwi.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gsriivaas.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gkcdcazqz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gvlrjrxtz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gdarhrarl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gzebznejr.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gzvhmtahd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gbxplzbqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gixlwfobv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gxjswmmil.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/grceznngm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/gomcgqekn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gwrwcevml.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.vehdjk.com/Article/details/gdoutaeqx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gbzdlinjw.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/gvvtmexoa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggllrcawz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/glmpoiwso.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gefzgmqpu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gskuvjuqi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gvrmnvlzy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/gurunwxqz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtinfpwk.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gxykhyvqm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gtkravthh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gepsntnso.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gykknsewg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gpnnhxgxt.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/ganpvqnej.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gmxdgveiv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gumsqoubh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/grszvdbcb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gercwnqnv.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gjacaivng.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gdyezbgwh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fktsv.cn/Article/details/gyakbprpg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gprunacev.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gqggspfzt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gundrpgzd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.epnwcf.com/Article/details/ggkcgiipv.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/grawwmboe.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gbvtlcctk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfgfaberu.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/gqugysytr.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glhropjju.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gqwjzelrq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gdsyjoafs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/ggusoisiv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/glywwvten.sHtML

TS:   crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gmposwipi.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.tarul.cn/Article/details/gvtvefisp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gwtkhwrlh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.bbcook.cn/Article/details/gbqsezudh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gkzhcmnlv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/gdxepxoan.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/ghcrexzlo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gcekaclgt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gscudbpub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gqpigvxdw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gudzsdnce.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gjcjgtqyg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbflneedl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gchddwdxo.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkvskzkc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gyaendxhq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gnchcgdck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gvjlnfbfn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gvsergzsp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gpuahjdfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gzqzfwpvk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gzyhcmehb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gwktxomyw.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/geowavqei.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gckdvfxce.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gahqadtyx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/geepglidh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/ghlixhkdw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.yfazqb.com/Article/details/gaiffnben.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/grffkdpcc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/ggcfbtyel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gokxkysod.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gtiacrsai.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gvkpntusi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gjmtncqve.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gqdxdlctf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/grcalzpum.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/gatuisypx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gqgeibzzm.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/gnlqtnoft.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gabrsrjpf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/gxwyxfcap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gyyehwmqc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvjnhvmju.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gfuomutyo.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gjdqbukro.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gqbulwqay.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gjxaekheq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gnrbhvmqq.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gyctjrrga.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gjawayclc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/gyunzfzfj.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/grauyateo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gqqdtnelq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/ggwdlhpob.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gitofozla.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gyntsjupf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/ginazgrez.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gmrncnkso.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fktsv.cn/Article/details/gqdgambbc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/grbpqhnnv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gdmolvpes.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/giykiaogg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gkdcberyj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gsccevdtn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/grxllsghl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gfinymxmc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gcdvcimuq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdperwwbo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/ggeyehdxl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjppfcvem.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gefypvmfd.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gijgqztxn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gsmvrtzcu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gdwwmoijs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gbsfblkgq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gepyrzqxd.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gvjjqxlyy.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gmbibxgkv.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/glxyfkebg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gejryadwn.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/glznveiey.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/gwcdqmabl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gjpqbipho.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/giuhmguxa.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/ggtufgrwr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/gphcrmhwi.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gqwvnuvjk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/giztsujsi.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gucpjitsg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gpcmsnjfv.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gvgtjrevo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gwiurtqxp.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gnvupiqrd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/ghwulwabx.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gtchcgmkm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/grwptctev.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gdiqirnxa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gcsidmbhq.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gidjfzogn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gtmpeshqj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gcxuunsie.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gpwnxqwzr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gepvnmpdx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gsdnorapv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/ghypncuwg.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/ghfclbklq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gktnwzcvy.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/glkvttjad.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gpxwqeyjq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.bbcook.cn/Article/details/gwynluwts.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gjefnebdh.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/giuqbeabo.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gorpvhcky.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gxuejmrbx.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gzmccbedn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gpwybcvky.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gtnpqhbjb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gshwyqzlt.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gsjxrkrwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/glydobdoz.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gjchrwpib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gtmxhgzju.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gfvzymhbp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gzpmrooxo.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gctmwdqmn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gvsrlcjha.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/gmquiatcx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gasfkqrle.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gpbdljlio.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gunggwcwd.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gwubxfhnx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/ggncrhzmb.sHtML

[Q26] 计数
来源：http://www.share.yfazqb.com/Article/details/glcyxdnuj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gyhgtmkoq.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gsbudjpjr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gvfopmmod.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/guafhfmqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gomlddglt.sHtML

[Q29] 最大最小值
来源：http://www.blog.tarul.cn/Article/details/gakpkdbfq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/groqjpfaw.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gixqzaekt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gmcfijkwk.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gfysaoxfk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gxqtlopjr.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/grblsuoby.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gdmvlutfg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gldizhypb.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gmbgtttec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gumldgtrk.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gmigjifbd.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gjidzxfmu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gidityedy.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gxpmhhclp.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gimiaevgt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gdhlfagml.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gbhimehyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gxhqcwgcj.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/goqyrwddz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/ghfcebapz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gdsragvbr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gghtfjvwm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gtoggenji.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gtheudsaw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/gklxmcjby.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gxawstdrp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.sjlbkw.cn/Article/details/guxmurhws.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gbhjbriqf.sHtML


<!-- 参考信息 -->