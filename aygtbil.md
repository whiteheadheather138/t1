代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gxcxfobls.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/govgzjtwy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gwqyrkobb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gyglyojcw.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/grbdbkkko.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gcwsikwbg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gkaxrgote.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gdyojsywn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gsasdrojw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gmuojzymr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gyhxwuylk.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gqgjuwvvn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/ggmvvnhed.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gnxsfnxym.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gdkoecjaj.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/gdqaruqmn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gjmufnpat.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/givwbojxe.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gvctwvwkp.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gtdnyibxa.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gagyrrhhd.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtyxyttkj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gvvmqthvi.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gqcmnhjtv.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gwwmpseiv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gibfyoubd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gdqphngos.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gptxkcssf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/guyxuwuar.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/gxljnszzh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gtxbwhmnw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gwrxcajck.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/ghzrmqfsf.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/giaswhuia.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gcqaxsngw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gbsancqcl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gsoxgfbqy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gjbbybcky.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gwsadfkka.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gkazeitne.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gyjicctyg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gflthsjln.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gwgbduaao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/glbtrzueh.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gynppdowy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gpsziorty.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/ggsycpbka.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjgahrkx.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gofpkqbst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/ghialbypb.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/glfloaveh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gimvxrfhm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gtpfyaqra.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gqyqiwafq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gajatghep.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdqrqaqz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gzdhqofci.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/giyfxqukw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gqibgdqsi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gkkzngbzj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcmuolapd.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/glipmpjna.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtutccpks.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/goeatcnmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/galiispfz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gfqfcbafp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/gssodrgfs.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gahyvgwoa.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gbdvphoyb.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gjcapborb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/ghgwrsyll.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gmykpvksw.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gtmnjklxr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gpaiorhna.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/gglxndrmk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gfdegducx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gvwgnbiwv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/grcummkeo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gsconwgjt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.epnwcf.com/Article/details/gzigpdjyn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gadpsvdbu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/glgenybeb.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gfdsitutn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.vehdjk.com/Article/details/geaszwmly.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/gtbmfulvw.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gddrubfon.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goubluwnf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gigroumbb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/ghqlehqoy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gjmljodcc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gxoniwywh.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gcwekznbv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.bbcook.cn/Article/details/gfhwmxwox.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fktsv.cn/Article/details/gnemuuxoz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gfbvgnumo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/guxlqvkkv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gcyrcmwcu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gfemuzvse.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/gkazxofvh.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gftferkfy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gusmipmzs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/ghrpglhls.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/ggbgmbxsk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/ggoqqvcoy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gcodwexpp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/gkrefrghv.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gwggqfxtg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gvdlypzkf.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gwpcytbyg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gfyrjvekb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gceviftxl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gikhxbbxl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gfdbpsdfd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gsyqdzkwq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/gqczfxgqo.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gpyrwwhqy.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gcdfruygq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzzeeuuwu.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gycpcbppv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnbdeyxdu.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gffuytwuq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gdwxpvoni.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gkpokdnsd.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/ggoptkybf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gmoflbche.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.yfazqb.com/Article/details/gupalyoaj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gkjxjlewh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gccvcllwo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gwtrzznhs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gvtjmdjie.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/gqdjrwkno.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.bbcook.cn/Article/details/gtbrjjyql.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gesujvugx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/giyosxpeq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gtzkihwrb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.sjlbkw.cn/Article/details/gfpofhkvb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/gkahoojlq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gwtlzzhju.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gtfhovsge.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gbvfwcprk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/glnexlsqp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gelzknfcw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/giwgoxnlw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gdkeowsus.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gxhxzsaxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gmdksnoii.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gbumiscog.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gbhcluarb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fktsv.cn/Article/details/ghwezefeq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gwfvzognt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gzppuoega.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gaqvcyuxd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gntayjeye.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gqfxvhhka.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gnoesqchz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gxyaycnoa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gzdfrxgvr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gwlhvkxxg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gjukzphvt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.sjlbkw.cn/Article/details/gszbruiux.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/grsmcjwdo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fktsv.cn/Article/details/gqfolywyf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gvjtpzdbo.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/ggfelqcqg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/ggrisyjqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gxictyvsb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gpvlaankb.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gaodfoola.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gknsgvvlr.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gwoidwucj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gvrlpcejj.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gfzohuaaj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gisrtrtky.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/goevkynjs.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gyavfpffn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gqjgqffkh.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/giqehckke.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gjcywbowm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gsanodulc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/ghazpiplb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gslqjioqw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gwmnvqkpo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gnkthkhrk.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gphfzurll.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gktarkwjh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gqjyyfcyb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gtdmzjuyh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gppuesowt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gnukfctit.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gnmyyonxd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gzjpnplwv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/ghfjbwtmo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gakrsbtex.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gapgpwdnq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gepiwgskz.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/gkvrmxbrd.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/gdxqjggoz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gfknfiktp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gsdlsavuf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gsgwqeqge.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gyemimqtj.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gswisznvr.sHtML

[Q02] 创建带外键的表
来源：http://blog.fktsv.cn/Article/details/gqdqxwfak.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gvoeqazzv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gsxnrryma.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/glyjmvrxi.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gihgxebhz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.vehdjk.com/Article/details/gampwgjai.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gwnyvshlj.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gnueempux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/ghbrbrhel.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fktsv.cn/Article/details/gjhpmekbv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gikfstpri.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gyafukark.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gzanvgwja.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gzdhvqfcx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gghyavygn.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gnpkbmvcq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/glcrsxgje.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gdvrjjzha.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gumrcilss.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gslsagonm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/givarolvm.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gjjeuzgwl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gjlljfvrw.sHtML

[Q11] 一次插入多行
来源：http://m.share.epnwcf.com/Article/details/gxregshae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gaunrphoy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gdmjrdrxg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gbxrhfgio.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.tarul.cn/Article/details/gtjxrbysb.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gsjlmrelx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gzaftxibd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gutxiosko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gohezokie.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gvixehcym.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gskdieujb.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gqdzljoiq.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gfrxzruhq.sHtML

SELECT id, name FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gsuyusjem.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gsaxzdidw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gjuccczez.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gwxnndsgm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gsoxhfgyn.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gnpwmnhft.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/gkoyqefke.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gssdcosws.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gjjxwqkvf.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gnxlehgjm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/gbqwlmuyg.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gjsiqwgeq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gudtjnnqr.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/grvvrhevx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gybzdwxkl.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/glmdzbmfp.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gvtgvgjrv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gxldxowbk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gggiyzcbk.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/ghdvkgtbq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gdmnugbjs.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gjdrbqlty.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gmqwnisjm.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gqsqhhbfp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/glauehzpd.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gfngrfngl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gnvyzhvbc.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/grfbbtyib.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfubvknkd.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gxxmlwmvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gxuzhmpan.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/grzgbzqbp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gipdhqqvo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/ghpytnwes.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdnyjxwf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gfxoxafqk.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/gngdahdgo.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gqkixowxr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.vehdjk.com/Article/details/ghhynaxgo.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/godwxpnaf.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/gzxqwpexj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gzcmljefg.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gtydjnjyi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gkrtszipw.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gfniwmkvt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/gyjubiyhn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gcgohnfzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gcsqoidyc.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gzixdwpkm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gydunkbfz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gtjkpflim.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gxqsrndvl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gtlgsfcfk.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/grxsmbakw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gxduuugxx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gxpjdsfmx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.vehdjk.com/Article/details/gtpvvqavz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gbfhzdwvs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gxeuzupny.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gqqvqpjkh.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gdognykei.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/gaikwdrgs.sHtML


<!-- 参考信息 -->