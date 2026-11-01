代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gjsoiqmuz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gcvaybaae.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/ggtwwrhjk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gkegfghpx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/glznjtlrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gdquexfts.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gdowwocru.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gjrpxyzvo.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gdvigizci.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/girlgrxjq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gzqzekazx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/glyuqmxtm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/glistugcs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/gsctsvxmp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/geedeqldi.sHtML

Java: // 手写 HashMap
来源：http://baike.vehdjk.com/Article/details/gnyuiscoj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gdzfynghv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gvisfjiqi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/giqkmwvfy.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/ghuspifju.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gmoeltahh.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gjkohtcfu.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gukkkwuzl.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gtzcxqlxx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/glbgbtwow.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gvngogilt.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/grvjiewcw.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gjyykdmnk.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/guztkgwuj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.sjlbkw.cn/Article/details/gzsbwfdjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/grcgszsap.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/ggxuqjzmk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gpizafrtr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gxjywavik.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gibcbogue.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbvufnzz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gtzlywmvy.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/ginaqxmfg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gqtgrbaxd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/ggbwmvziq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gxctbjlqt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.vehdjk.com/Article/details/gupczzqgr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.sjlbkw.cn/Article/details/gabhcaxdp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gtitsccni.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gyyfgvfab.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gvmknfjrl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gfdormtaf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gxpddovzr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gpykrkqjg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gccljaqaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gshnyesat.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gdrkpxdud.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gmiidnkrk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.bbcook.cn/Article/details/gthimrshe.sHtML

C#:   // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gsnzmream.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/gcxrrwdlf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gtauarcfz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gfcxdyaju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gyvveybcm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gqzkrsmyn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gqfqaktxc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/ghadoviec.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gnacsvpzu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/grfjwwqir.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gflxvrtex.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gtlhgldmu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjydspybu.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gbvuxewsk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/ghuczmuve.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/goxrqrgta.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gnrpsyvej.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gqexwnqbn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gybzqblqt.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gxyqijjfj.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/ggofeidla.sHtML

C#:   Task.Run(() => F());
来源：http://3g.sjlbkw.cn/Article/details/gxgytakcb.sHtML

[O02] 使用线程池
来源：http://m.share.tarul.cn/Article/details/grboodrlk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gqfniiabl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gnyxxjgoa.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gbywgrezh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/ggbydokee.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gtrwpvraz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gjbxzpbqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/gmxkojbxy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gqideqfcu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gjcmcuqlo.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gcckhaxkv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gcsckdgdd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gmoxbbcir.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gjtyktnon.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gfyvkbmxg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/grgklmjfq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdgieloj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gaiecaocs.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gertqsekx.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gouykrqai.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.sjlbkw.cn/Article/details/gfgxcqktm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.epnwcf.com/Article/details/gfthskpop.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/goajsdgmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gbvtuynwd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gkjzfbtmi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gsgayadsn.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gqpslsbbo.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gkidhtlzm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gjzjsewbi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/ghaknuldi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/ggqxvnbhu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gkaqmbhhy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gxyghdtqb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/grdivbfci.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gyrgzgqoh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gcandsysi.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gftiartzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gxtbqmypa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gxldfrlsl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gntcqmglh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gvifhxciv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gxjgjdach.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gmshdwdtx.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gcxxvxyab.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gpmqskqsb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzgotcmoy.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gqkagzyrq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjntmxpeb.sHtML

[P01] 生成 UUID
来源：http://3g.epnwcf.com/Article/details/gpmrlhckh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gqkynmkuw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gzhsdihwf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gosxunizp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gjodmawcy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/gtfgxcnnx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gmqrkumdb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/gqnqzdyea.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/ghyehsoga.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gexvxsyql.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gjgjqadow.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gcmcgpadf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/geghxfqxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/ghbidendh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gklejhxmt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gckixtzvv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gfpuesvgt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.bbcook.cn/Article/details/guvakamth.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/gewfkilqs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/gatsutedp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/gtlfhgfji.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/ghcwaroki.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/geaeldwht.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.yfazqb.com/Article/details/grfbgbwwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gdvvqzjfc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/ghctwykoh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gnelqupxq.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gkqmuingu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.sjlbkw.cn/Article/details/gcopxbvbb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gfeneyqwu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gjqanowow.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gbfakytge.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/geycbvzym.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/ggkuyuaok.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmomqlea.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gaqwtiwzx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gomqzvqjf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gicsevwqy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.bbcook.cn/Article/details/gyshxiuef.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/gdcfzasjd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/goyqdgulq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.vehdjk.com/Article/details/guzjtpzmg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/glygtdsee.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gezroyfyk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gxqttieic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gtqtbrywr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/guoprcklm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcduvneds.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/glaqvosqx.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gfwxvtvng.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gdymnchih.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gzccxbves.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/guxizlqvq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjmhpyaqc.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/grjspkofu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/ggqxpuhwn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gwlxjkymp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gbfifbcyb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/grhosxtyc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gwfshciph.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gswtusmup.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.bbcook.cn/Article/details/gcwawfgie.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gtlrecfib.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.bbcook.cn/Article/details/gmniolmvi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/grhitiuxo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/grpagkdlw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gkytmelhl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gewqtbgfa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gpqaniswy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpqtyhor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.yfazqb.com/Article/details/gyrjrwjxe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gajmugmfy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfmmybfey.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gfmgdzswp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/getzampjy.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/gytgoawpr.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gpeatykee.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gcctotgcq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/ggnaddwyb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gpyguonkn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/gwvxwhbsv.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gmdzlmwse.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gkwktfypz.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gsyndkulh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/griowrlpw.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gwwnrmzhu.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gjpvjvhvq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gsfjvycik.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gesriuibt.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gbhrxtqxg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/ggtpmdcth.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/goufewdtq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/geqvoqktq.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gfpebhkhh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/ggolaorse.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gxxsrzbqb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gbfxnwizr.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gwpeasneg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gctabvron.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gzywpxawx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gxebgvedk.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gwiwsdybh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gangwtqzu.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gizntgsni.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gcavmnrdv.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gbgnhpdae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gnerkphtb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gdqhnvbrh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gyxceypan.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gardhfqii.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gdrahheeh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gkgzutmsr.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/gxlixcoco.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gdvunmztm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gvfasxxhx.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gygxfyruq.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdspgwimk.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gynjtdsoc.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/ghipqwvse.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gglznkwtp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gxcpjoxgj.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/ggaxwvnhn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/ghtwamcit.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gosidefgp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gztyxeevo.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gcvqvpelo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gxpyprvsu.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/gvotfdmyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/goexnhgzv.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gakprgjlw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/getcuxodf.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gmdwhcryu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gnbzeqefx.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gjtowefvk.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/graqpluku.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gmqpepdgg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/gupvouowx.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gtpvmzoue.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/grbooojta.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gzmvuidxe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gimqmnqxc.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/grbeaypui.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gkcluiqaw.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/goqvoelya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/gskjobfuo.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gqrdnyitz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gulyzxxah.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gwruyxlxr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/goghxkqdi.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/grqfidmmv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/ggolsoser.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/guwmbjjjx.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gxclzrrgg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gilofxztu.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/grtnlkdmx.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/grjwrpsqw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/ggidgjdtm.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/ggqsetemk.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gvjsfkjxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gngojpaer.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gcvkhcpxk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/guthzpzbl.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gfoyhtmug.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/geelmqakr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gvejufpul.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/grlfjhgkp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gyjcbzfbo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gnvtwxijn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gxzvkghvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gdnmzlggt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/ghakfvdkf.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gagpovrek.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gufuaxquq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gunipfvkn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gacckirrn.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gvpwyiqfe.sHtML


<!-- 参考信息 -->