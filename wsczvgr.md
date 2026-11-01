代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gutmcqtlj.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/ghkyuknzh.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gnphjjexe.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/ggwwvfzqn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gtpeobrlz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gdvsfleph.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gwlufaqqd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gbgizaanj.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gfotdnlqf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/glgflxhto.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gopjjmgdh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gdmbpbypm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/ggibwivkb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gshpblsck.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gxzjaxbix.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gepmskcxv.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gjbusadjp.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gfpccodwz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gsznuffkv.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gmawcmrwp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gkjxcuwoi.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/ggyexumwf.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/glzznpqdv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gjyysuqxg.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gbfqamtlc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gnrfarvrb.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gmxlovspp.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gsvhdldct.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gyhbofpsg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gxlxdrsay.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.vehdjk.com/Article/details/gsiiqvega.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gmsjvtlsh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gitywyljw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/gkmzbjlav.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gijbdverj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gtoyihgeq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gqauoxpkz.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gnkdcluwb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gbxxwsvak.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.sjlbkw.cn/Article/details/gcpphclto.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gmxaoshty.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gxirlseoe.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gsufvhotw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gtbbzpand.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/glveergkb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gbygwfyra.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gfngdnkhn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gjvrimwgg.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gmecrnuac.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/grhqnyhwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gyryrdtnv.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/goirotvzi.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/ggolclsxd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/ggldzmggd.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gqxzjbilo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gnskbtuco.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gvdgjgqix.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/ggrhdotqc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gzyemglqq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/ginplsayu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/godsikqpe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/guvfyttgz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gdznhrpzs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/grrjyfrnq.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzfoqkaxz.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/guazwjnbe.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjtglfksv.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gfmdsdejx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/genfuzzbk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gzmsgffgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gxxogrgec.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gibsmvccz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/guxcsahaa.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gmgexgnjt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gquwtfidw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/geeypbdsg.sHtML

[O02] 使用线程池
来源：http://www.m.share.yfazqb.com/Article/details/gytzigidz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/ggmnlcuzf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gjbtwuxhe.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gkqqcodlk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gvqazskrg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/ggufqhwpm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gemwrjccd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/giaosajdq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gmdnoekcg.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gwncydygs.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gnbbazkkb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.yfazqb.com/Article/details/glmibursd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.bbcook.cn/Article/details/giffhcgoa.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gjtnubqvc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtbllremz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gfpfkanxu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gggblmxlp.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gyuupcxur.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gnbtosxpf.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gpohvgscf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/grrhdhkok.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gdjgoosya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gexdetvnc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gkpviuoks.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/gffwivzfc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/ghewhflkh.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.bbcook.cn/Article/details/gjosjshll.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gqgcndsuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/ggnqazthz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/ghtdzjsaf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/glwiniige.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gmhteaife.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/giwtookvt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gcjmyamfe.sHtML

Ruby: threads.map(&:join)
来源：http://wap.vehdjk.com/Article/details/grmybuumc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gnttfxiak.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gwvgfkiuf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gxalsowvp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gdqzrgtet.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gdvsovxqp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gzrgxgtjv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.epnwcf.com/Article/details/giyvateln.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.vehdjk.com/Article/details/gnhjsiwpq.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/gwxyqfhzx.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/glwtykygq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvshywpee.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gzggvwajl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbdizwdix.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gzotnpovo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/gdvddzhds.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gkgmuayoi.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gnamfghex.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gdmlnzogj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gjywehwgo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gsnuuwrxw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/glkcekieh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gppkjacfs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gmrvtjfut.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/gapyxwoyx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gfwwizhkf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/gpkcqxlkf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gcsslaepm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/gdzggqofo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/gfdkllrus.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtlovdros.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gvzzvimti.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gjunwumkt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gvvvtzzfo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gtwvumoms.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gpgywfytm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/giwtzzfee.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/ghwwidevn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gvdbiojfy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gfvjtmuta.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gyysplzqb.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gfrhzujct.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/gqtnrhwmz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gzkikssuf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/glvkzlmoq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gyzgsumdi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gyvkcwkmv.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gaufazdtv.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/guxqzanhe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gtjaqqkbj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.epnwcf.com/Article/details/gatowtiwd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.epnwcf.com/Article/details/gypyaeeip.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/glenrkiwa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.tarul.cn/Article/details/glwibewqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gtbzsszwi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/ghsmlfdyp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gyksistbb.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gpqgtivlt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gnkpeywqp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gssfqebvw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/gzkclblvr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/gseexkodh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gwayfoldt.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/glrljowuq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gspcjqftj.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gwptgcnrv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/gckvtcfpm.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gththklmi.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gquydafhl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.bbcook.cn/Article/details/ghwrujkbu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/gezifynxg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gglzjlaox.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gxgtmfwcu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.tarul.cn/Article/details/gvfnuysha.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsaibjel.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gxnnyatcy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gloedsgll.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.yfazqb.com/Article/details/gscsymkuy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/ggaxhoilx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gxobwmgoh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gvrnpxcgl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/glkhmcloz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gibcwsfrf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/gpyimgjpf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gxxlapdur.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/gslicfooi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnkxwpdyc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gefhfvvet.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzhotzewv.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gxuyijqmp.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gygpmjrab.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gxtradjsh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/ggrevzzjx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/guvtaxctv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gbtvbxhzl.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofflaovp.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/giieopqks.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gbxkdyxgb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gwensotnq.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gwhdpuzem.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gvkvbrbze.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gcrcghemq.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/ghctlhrby.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/guqrjpcmr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/guwjtnpuu.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/ghbsutisc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gunehszmy.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gjmpsjgjb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gbwphyjjm.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/ggagxwxma.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fktsv.cn/Article/details/gzykqaggv.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gkztjqpde.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gqnqzqzsb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gtgfzsxqz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gnivwglcq.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/gqhiausbf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gvaadxawy.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gomjmgeqg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gcdmlgprs.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gktmestol.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/grnjykots.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gmcltbuma.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gzpmhkjar.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/glpjemwlc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gjyjdkhka.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gjndheicf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gtlgbrcta.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gynddzirg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.sjlbkw.cn/Article/details/giuvenrvb.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gcbkblkxm.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gsjncmdky.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gbkwqrmxt.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gnakwdmrv.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/ggthaobfx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gmoxcfquk.sHtML

[Q18] 模糊匹配
来源：http://baike.fktsv.cn/Article/details/gmnauhsji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gsancrzkj.sHtML

[Q19] 范围查询
来源：http://mobile.sjlbkw.cn/Article/details/grdnuskxa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/ggcpfasne.sHtML

[Q20] IN 列表
来源：http://m.share.fktsv.cn/Article/details/gnjawdove.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gumvbydyc.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/goyhvpuco.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/guwwfpybe.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/ggcoycwme.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.bbcook.cn/Article/details/gdmknmpit.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gmdqywlns.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gxofppehw.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gyuxoaflb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gaurpbjfg.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/ghvuzohyf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gyiutdkot.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/goftgbazx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/ghttarnkp.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gflmignpq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gbjiurzal.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gqfhuqdzv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gxkvcyvrz.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/ggeluotqm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/givybxqri.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gerecakqo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gyublkbme.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/giheztfry.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gizjhnnxr.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/glmymphub.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gxiedgfik.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gifaixwjq.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/glxbvdjrb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gyrhskwxa.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gtsttlcft.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/glbimwfyg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gqqgyrluq.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/ghhthpflz.sHtML

[Q35] 内连接
来源：http://read.share.bbcook.cn/Article/details/gtpijaryu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gdlxpyosq.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gpelnvksj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gvcnazsnf.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gorebtwva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/ggqzbjjeg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.bbcook.cn/Article/details/gjevaofge.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gpwvctoyv.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/givlqmnph.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gqfviqczb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gyaidfhgt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/geiykqwhx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.vehdjk.com/Article/details/gockwolna.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gqwxmfdjr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gglpzswjw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gddtijoia.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gjhspwhju.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/ggcbcjvbf.sHtML


<!-- 参考信息 -->