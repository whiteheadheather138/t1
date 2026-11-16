代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://imy.tarul.cn

JS:   console.error("err")
来源：http://gew.fehbvm.com

TS:   console.error("err")
来源：http://lww.316326.xyz

Java: System.err.println("err")
来源：http://aqj.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yvj.tian-w.cn

Ruby: warn "err"
来源：http://dtp.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://xjw.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://sdg.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://nru.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ftp.yonumen.top

JS:   require.main === module
来源：http://qpp.vehdjk.com

TS:   require.main === module
来源：http://tex.birdmap.top

Java: public static void main(String[] args)
来源：http://obp.pycfn.com

Go:   func main()
来源：http://dhm.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mnz.tian-w.cn

C#:   static void Main(string[] args)
来源：http://prk.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://kwr.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://uww.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://cos.ybcxt.top

JS:   process.platform;  process.version
来源：http://brp.cucudq.cn

TS:   process.platform;  process.version
来源：http://wnk.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wly.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://orv.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uhh.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wsv.xingfuxueyuan.xyz

================================================================================
来源：http://ppn.52xcode.cn

N. 数据结构与算法
来源：http://fid.hfpthk.cn

================================================================================
来源：http://wuv.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://bcd.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dps.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nvw.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mlp.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ffm.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://xpf.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://uxw.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://koq.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sbb.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://tsb.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://fbl.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bet.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ndr.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ffn.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rqh.fktsv.cn

Go:   slices.Sort(arr)
来源：http://dnx.316326.xyz

Ruby: arr.sort
来源：http://nwv.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zem.cashguo.top

[N03] 快速排序（分治示例）
来源：http://hky.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kut.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://zlw.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcg.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgv.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yid.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zko.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nnh.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://nrk.haohaochexian.top

[N04] 斐波那契数列
来源：http://uvq.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zph.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xge.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://odz.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzh.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qhu.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gfa.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://buv.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wtl.yfazqb.com

[N05] 最大公约数
来源：http://kcx.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://oij.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wwa.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ors.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zoa.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ekm.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ajy.9152youxi.cn

Ruby: a.gcd(b)
来源：http://sor.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xzd.yj202588.top

[N06] 判断回文字符串
来源：http://sfk.meibo888.top

Py:   s == s[::-1]
来源：http://djc.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://fyd.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://vah.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://qfv.kuanghao11.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kkj.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://bhm.sjlbkw.cn

Ruby: s == s.reverse
来源：http://isw.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://syx.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://vre.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xgv.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lps.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kun.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://jma.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://ztn.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://qvl.0kj1m.cn

Ruby: // 手写 Hash
来源：http://ypl.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://vwg.andypj.xyz

[N08] 生成全排列
来源：http://mfs.yj20258.top

Py:   itertools.permutations(arr)
来源：http://hrj.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://tjt.daria6918.cn

JS:   // 手写回溯递归
来源：http://toe.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://fmo.xinyue.icu

Java: // 手写回溯递归
来源：http://dox.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://kqe.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://wqf.yueranfly.top

C#:   // 手写回溯递归
来源：http://ehi.shuidangran.top

[N09] 栈与队列
来源：http://gch.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qge.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gsj.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://spi.bbcook.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jbg.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eru.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://opa.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ocq.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cdp.yangfankeji.com

[N10] 链表节点定义
来源：http://igq.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nhy.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cvx.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofr.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxu.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://dgc.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xoi.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ziw.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xrl.hesvh.cn

[N11] 二叉树中序遍历
来源：http://ssu.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tgv.jiagoushi.top

PHP:  // 手写递归函数
来源：http://mdz.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vfd.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pgt.cdnleiting.top

Java: // 手写递归
来源：http://gde.hesvh.cn

Go:   // 手写递归
来源：http://sby.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ghw.jinghuilouyu.cn

C#:   // 手写递归
来源：http://gnd.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dyf.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dbg.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oow.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bhz.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hdf.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oit.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://imp.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qkx.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jji.kuanghao11.cn

================================================================================
来源：http://tjo.fktsv.cn

O. 并发与异步
来源：http://qcp.pengpengdd.cyou

================================================================================
来源：http://oye.316326.xyz

[O01] 启动一个线程
来源：http://sad.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ssi.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qls.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wmr.ppjwa.cn

TS:   // 同 JS
来源：http://cxo.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://eui.havefunace.top

Go:   go f()
来源：http://qkm.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://fnv.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://dnh.chenzaomai.com

[O02] 使用线程池
来源：http://ukz.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pco.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://crs.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://bue.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://hxd.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://dzy.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ywc.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://abw.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uwk.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://yhx.sysykeji.top

Py:   with lock: shared += 1
来源：http://sdl.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://uto.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jpf.hnxiangtu.top

TS:   // 同 JS
来源：http://rww.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://dqz.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nti.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hye.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://qee.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://rlu.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://bcs.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ivy.tanke756.top

JS:   async function f() { await g(); }
来源：http://tey.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ldh.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lhu.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyg.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://uon.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://scz.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://rup.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://xig.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zyu.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://znk.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://tae.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dop.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mwv.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://pgr.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zfi.zhijiandao.cn

[O06] 使用进程池
来源：http://pbw.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pac.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vji.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://azj.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://mlx.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uhb.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bek.mhx1999.top

Ruby: // fork 块
来源：http://uma.gotoacloud.top

C#:   Parallel.For
来源：http://crz.jinqigufen.top

================================================================================
来源：http://yzm.cdnleiting.top

P. 常用工具函数
来源：http://brx.gotoacloud.top

================================================================================
来源：http://zoj.cheryme.top

[P01] 生成 UUID
来源：http://por.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://uqv.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ebt.ybcxt.top

JS:   crypto.randomUUID()
来源：http://ywb.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://klu.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://ckc.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://gxi.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://bvm.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://uzz.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://ojz.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dks.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lgb.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ruy.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nag.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ddz.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zzb.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svb.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://emi.chenzaomai.com

[P03] 生成短随机字符串
来源：http://dsh.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slw.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eve.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qph.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flb.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dwh.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mnh.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://uiu.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dcf.yangfankeji.com

[P04] 求长度
来源：http://epb.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gop.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfr.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uvi.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fys.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://pjv.yj202588.top

Go:   len(arr);  len(m)
来源：http://nxp.jqgfzy.top

Ruby: x.length;  x.size
来源：http://uyt.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://slb.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://yks.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mxl.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wcb.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hcp.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zjo.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jtp.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://hos.tian-w.cn

Ruby: a == b
来源：http://ali.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://idh.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cis.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bdt.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://fmr.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mui.jqgufenzy.top

TS:   if (x == null) {}
来源：http://kkd.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kwt.jlsjyb.cn

Go:   if x == nil {}
来源：http://kfx.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bxm.zhongyouzk.top

C#:   if (x is null) {}
来源：http://xzd.tarul.cn

[P07] 防抖与节流
来源：http://vhn.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aqx.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://xrd.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtm.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mrc.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ban.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fld.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pye.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kug.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://gva.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dal.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fya.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ntk.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qdw.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jwq.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xae.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mea.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ulz.yueranfly.top

================================================================================
来源：http://hap.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wge.xuetiantiany.cn

================================================================================
来源：http://wcn.vqdsnc.cn

[Q01] 创建表
来源：http://exf.316326.xyz

CREATE TABLE users (
来源：http://dhs.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://feh.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://ncr.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://atq.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://noc.quarkkingdee.top

);
来源：http://vrp.jinqigufen.top

[Q02] 创建带外键的表
来源：http://yps.jinqigufen.top

CREATE TABLE orders (
来源：http://sov.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrw.chenlongwang.top

user_id INT NOT NULL,
来源：http://bin.316326.xyz

amount DECIMAL(10, 2),
来源：http://iid.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tjp.cucudq.cn

);
来源：http://jmz.zhaomingkeji.xyz

[Q03] 增加列
来源：http://eka.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ezm.ydjk.org.cn

[Q04] 修改列类型
来源：http://qaw.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://okd.tarul.cn

[Q05] 重命名列
来源：http://qbl.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ydj.sweek.top

[Q06] 删除列
来源：http://fuy.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ect.yj20258888.top

[Q07] 删除表
来源：http://acy.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://rqq.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://pjo.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pdg.xuanzx.com

[Q09] 创建唯一索引
来源：http://hrg.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://apc.pengpengdd.cyou

[Q10] 插入单行
来源：http://rjw.shzxlz.cn


<!-- 参考信息 -->