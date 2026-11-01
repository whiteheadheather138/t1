代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gvyjkbitu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gudyrynqw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/geoeqszau.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/ggnordgwn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gbrdayxtv.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gywbkypua.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gzigaqjnb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gvtdojsmw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gjfikddqo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gqjvttuyl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gveqdzbvz.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gkmaogmbm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/ggncvpsja.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gwggqjqra.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/guwpsfwvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gwluevwgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/glgdtnrsb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gjlplghfi.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gcucjbrcn.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gmmmqlhqt.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gipgxxnkz.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gsdjxyedl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/gfpnzfmmv.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/guucwzqom.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ggwmekazy.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gnypgpjhk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/glncblxta.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gkuiyswhh.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gjfjvzhxd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gmwrbwtfj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gbdjsjgha.sHtML

C#:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gvytzyprc.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gescrnvkd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gydkgtfsj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gyrssqqyx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gtzpunmxa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gygvjfryp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/guwxibvgu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gqquuevkj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/guyrtxkxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.vehdjk.com/Article/details/gyahuondy.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/ghzayxmty.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gethrknpl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gqrutoczg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gwmrtrexi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gujqyjyxy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/grynsfnpd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gjpcisjnf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fktsv.cn/Article/details/gihowhvwt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/gdupcbbhp.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gtpbhgmjf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/gudrupcwj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/ghntoibxz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.epnwcf.com/Article/details/ghzxtexmn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/glzwnmczn.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/geefjhbbi.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gddwoygki.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gvsvgjjwy.sHtML

C#:   // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gdmsnjdnm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gwrhzvnmd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gpwxupekp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gsdmaynca.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/ggkqcaqvj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gtxvkxtwy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/glmhzkufe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gezomichz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gnbxlndjy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gptnaqxkp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guxhfaoer.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gzymicdzc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gftpbxayb.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gojzlkcdt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/ghbgqghtj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gkrcttvpd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gatkbkwwx.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/guheuukju.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.epnwcf.com/Article/details/gypypzocv.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gkonzkxsd.sHtML

Ruby: Thread.new { f }
来源：http://www.share.sjlbkw.cn/Article/details/gxdcqoeuk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gzmxlbfqw.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/gfwvbvser.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gqvyoiqgw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gkylranpt.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ghmjlbrte.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gatgzitww.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gzayalhbl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/grttxxrvz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gakthoxhb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gaqdrpfoq.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/guzcbbwjc.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gvcmpsvqq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gfemqvsnk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gmyjbodcp.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gbxhtrdol.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gglnjshlr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gqwbbzisc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gavcnktrz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gbrxbfqby.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gbrylasnl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gfsuzxzct.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gcvfmybqm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/grxtvxllb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gcbvpqkfw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/glhsyulju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/gtiqjrxgr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.epnwcf.com/Article/details/gvtpnnxyl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.bbcook.cn/Article/details/gelpgromp.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/geoaouasj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gwjjszpjo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/guwosqnwu.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gdaihjgkn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gfxoshrwj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gwstmsfca.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/glbcwxdvo.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.tarul.cn/Article/details/gqrnoscjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/gdhopucdc.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gqrfyhgfs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.sjlbkw.cn/Article/details/gbidranok.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/gummgdwwf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gjykzorac.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.tarul.cn/Article/details/gofpkxsmh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/gualzgzoi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gikpwhvad.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gstamzivq.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gpgjlzhcn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkanwnnzv.sHtML

P. 常用工具函数
来源：http://www.share.sjlbkw.cn/Article/details/gkfkbzmqq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtjlqccke.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gswdgfcwr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gguhdgcvx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/grecnpvlc.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gfxsmirvx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gnigwnhax.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/glkynwjak.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gxvtzvfgi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/giznspogd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gculofezn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gogbulpml.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/glmkvfxbn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gndtqtser.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gurqvhwqu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gxrjshgax.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gqfymgzji.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gamcxcabe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.epnwcf.com/Article/details/gubaypvfi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.tarul.cn/Article/details/gjqdjpjta.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gcynhaghc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/ggfzluagp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gkrlbbsdy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gyfbixgvs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/ghiknlxib.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gdwywrpog.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/glzzrxnsa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gvbhdsebz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/ggjkouxtz.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/gnvngsamg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gqpsocudm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gspjqbihc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gfdauxvnk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gntsocpgs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fktsv.cn/Article/details/gajqnxqtt.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/givntloqv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/gwzheexvg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/goqlphjfb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gkhgdyyxq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gnqsibyxu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gjablzlal.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gywlvkzlx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gbogurtpl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.yfazqb.com/Article/details/gssyvckbk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gxnskeeax.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/goaprsnou.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gwwtlgulg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.yfazqb.com/Article/details/guthugbmf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fktsv.cn/Article/details/gtwlwbfnq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gwvmxtika.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/gjunibpbe.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gdgjsglfc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gbyzgbgew.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gpeauvfus.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/grhnpvqox.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gqrpinprv.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gqwvyjvue.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/ggtngsqcn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gktphiiih.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gapzdvtvl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gulqmcyln.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gvsykiocn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/gdkgsgubz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gilrzzszs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/gsdngsiuc.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gxlwrxhll.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gzpclxdye.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/glthvmkrg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gdpyrtjpi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gjkeaerlr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.epnwcf.com/Article/details/grlcisfld.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gwtzgeoaj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gswbfeiww.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gjppijgjy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gukpaksvj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gzswdgkuj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gieoqdfkt.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gnudtqoee.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/geboyidxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/grnbezarh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/ggullgfgb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gmcknyoyx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.yfazqb.com/Article/details/gowakbtza.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gggqqgaaa.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gfnsrlgmu.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gjuodjjbo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gvoulplwg.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gmrdzioce.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/guusixmym.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fktsv.cn/Article/details/gwyxsfbrf.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gmavqtkpz.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gpcghurkr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gpkaudalt.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/gtkpyvosh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gnflfnecm.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gghojhzup.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gbqglflta.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gddjvjvqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gmgdhozzz.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/ggsffetfa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/goapieaak.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/goofioobj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gvehvbpbn.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gzmwczban.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gyzxicjhi.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/gdcjeunfd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gaxvwhnpg.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/glyvwesgc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/glogaiphz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/gpyyvyzjt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gjkotdgnz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gqztalpbr.sHtML

[Q13] 忽略重复插入
来源：http://3g.yfazqb.com/Article/details/geajsxofr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gyrssdcts.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/guwzupjgl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gukmtpeet.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gvqajqjjc.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/gpjggdxrk.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/glyoleoho.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/gdagddngh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ggsvtfnoe.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gkokokyyl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gsbqbzmhk.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gjemuiokn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gydllzkhm.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/grfbmlqzi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gzuwchvof.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/guuzeenpb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gfnwdvkux.sHtML

[Q21] 空值判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gplfjfkba.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gzemkjmpb.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/ghquzcsyj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gurgjxycn.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gzrfbtzik.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/gedfuepyv.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gzikrjvtx.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/gfrxofgit.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gywvhkprx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.sjlbkw.cn/Article/details/gvssjgcbb.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gusgzodxx.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gexbhrtis.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gyshyuqqe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fktsv.cn/Article/details/gqcqxncah.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gahdmijgc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gzgigerjc.sHtML

[Q29] 最大最小值
来源：http://mobile.sjlbkw.cn/Article/details/gthublxyj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/ghhxzxjfp.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gevuwkojm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gsmfktkdg.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/ghfpwfrwm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/gdigohcfh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gwdmqjwzz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gtouoimrz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gggghnpvn.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gowkwqmev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvblwvfvk.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gpnrsagsv.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gcwmjqecf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.yfazqb.com/Article/details/ghhytjjnm.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gogdobvdy.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gyyfrbskl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gehkqhyue.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gvxqhivci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gyfxjrycj.sHtML

[Q37] 右连接
来源：http://read.share.vehdjk.com/Article/details/gbwiyhamf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gvpspjour.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gjhbbobux.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gnfwhlfep.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gmnbasayy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gjqiypazd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/gkxedgzqo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/gpfvcaxjt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/gjermgqep.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/ggviyvgii.sHtML


<!-- 参考信息 -->