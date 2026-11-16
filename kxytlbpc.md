代发 wailian999

Py:   if __name__ == "__main__":
来源：http://yaq.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wie.smart0.xyz

JS:   require.main === module
来源：http://fee.vqdsnc.cn

TS:   require.main === module
来源：http://eoe.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://vco.tian-w.cn

Go:   func main()
来源：http://ocl.nanxuanxn.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ljo.xuanzx.com

C#:   static void Main(string[] args)
来源：http://jrm.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://klk.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://keo.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://qes.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://amd.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://emw.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ogd.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lcu.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tlx.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hok.nanxuanxn.top

================================================================================
来源：http://cqu.gogol.net.cn

N. 数据结构与算法
来源：http://rnr.xingfuxueyuan.xyz

================================================================================
来源：http://pzl.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://qsi.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://sox.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qnu.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izg.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kjx.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yla.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://dnf.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hou.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dez.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://uvc.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://fqa.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://spg.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vej.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eyf.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wmg.hammf.cn

Go:   slices.Sort(arr)
来源：http://vdv.yj202588.top

Ruby: arr.sort
来源：http://ahd.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jzr.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://tyx.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zgh.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://wcs.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyo.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tan.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xws.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://grj.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xtg.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://juw.yvedp.cn

[N04] 斐波那契数列
来源：http://ncr.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ttf.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yws.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://flz.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jir.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pdd.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://szu.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vfj.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yas.yangfankeji.com

[N05] 最大公约数
来源：http://rax.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://pys.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wxt.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmj.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eeh.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oll.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jmm.gotoacloud.top

Ruby: a.gcd(b)
来源：http://zol.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://znl.smart0.xyz

[N06] 判断回文字符串
来源：http://jnl.hfpthk.cn

Py:   s == s[::-1]
来源：http://vcz.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://odk.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://fvg.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://sdd.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qzz.zycfv.cn

Go:   // 双指针从两端比较
来源：http://iol.sjlbkw.cn

Ruby: s == s.reverse
来源：http://unb.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://lkt.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://zyg.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jyp.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dfw.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://vjb.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://kuz.cqqwz.cn

Java: // 手写 HashMap
来源：http://xae.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://veb.zycfv.cn

Ruby: // 手写 Hash
来源：http://leh.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://wxt.sufxvd.cn

[N08] 生成全排列
来源：http://slt.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://wzf.9152youxi.cn

PHP:  // 手写递归交换
来源：http://ouf.havefunace.top

JS:   // 手写回溯递归
来源：http://ujz.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://zsm.iojbl.cn

Java: // 手写回溯递归
来源：http://nig.ehwqpu.com

Go:   // 手写回溯递归
来源：http://wid.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://yvh.jqgfzy.top

C#:   // 手写回溯递归
来源：http://ywi.ydjk.org.cn

[N09] 栈与队列
来源：http://oty.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nug.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxm.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hck.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gxz.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujp.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubo.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vky.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyw.tianlin.xyz

[N10] 链表节点定义
来源：http://dzb.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jnn.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uat.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zwb.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pkt.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://uye.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://xsz.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rzb.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wpi.yueranfly.top

[N11] 二叉树中序遍历
来源：http://bja.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dmj.xziqi.cn

PHP:  // 手写递归函数
来源：http://jvw.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qyq.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndq.ppjwa.cn

Java: // 手写递归
来源：http://cep.daxiang520.top

Go:   // 手写递归
来源：http://qtu.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jaz.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://fve.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zyr.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bmu.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yoo.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kpn.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://euu.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xiy.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pek.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qoq.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bra.hfpthk.cn

================================================================================
来源：http://nqp.hnqzz.top

O. 并发与异步
来源：http://yve.jinqigfzy.top

================================================================================
来源：http://sgr.zhengqikj.top

[O01] 启动一个线程
来源：http://pba.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jbe.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pgc.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kkq.birdmap.top

TS:   // 同 JS
来源：http://qjh.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://oyw.hcnkem.com

Go:   go f()
来源：http://sip.shzxlz.cn

Ruby: Thread.new { f }
来源：http://exg.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://dee.52xcode.cn

[O02] 使用线程池
来源：http://hzs.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cbk.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xnt.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://yvw.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://rls.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://dgk.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gbi.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mxv.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yam.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://xtx.ehwqpu.com

Py:   with lock: shared += 1
来源：http://rgg.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://ggi.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xoa.cqqwz.cn

TS:   // 同 JS
来源：http://zos.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://eyz.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bwr.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://jud.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://izd.redwolf501.top

[O04] 定义异步函数并等待
来源：http://mbm.yonumen.top

Py:   async def f():⏎    await g()
来源：http://xal.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gsq.yfazqb.com

JS:   async function f() { await g(); }
来源：http://hmv.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://rmi.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ghn.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uif.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://exh.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://osv.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://vhl.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://tsb.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://heb.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://gpe.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://ule.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bms.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yfp.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://ucr.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sqy.xuetiantiany.cn

[O06] 使用进程池
来源：http://exl.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kke.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ihm.meibo888.top

JS:   // child_process / cluster 模块
来源：http://jnz.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://uzu.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qtj.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://obo.tarul.cn

Ruby: // fork 块
来源：http://gdy.vqdsnc.cn

C#:   Parallel.For
来源：http://sgx.hcnkem.com

================================================================================
来源：http://sto.guannengcc.top

P. 常用工具函数
来源：http://igv.ehwqpu.com

================================================================================
来源：http://zjp.cqqwz.cn

[P01] 生成 UUID
来源：http://mjd.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://ywp.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pdb.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://qmc.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://evy.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://iuo.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://mdo.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://rpx.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://urv.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://nzb.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yet.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zzv.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zge.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uhg.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hpz.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://myi.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tkj.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ajx.ydzc1.top

[P03] 生成短随机字符串
来源：http://ujp.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fjq.ppjwa.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://orx.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pqy.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://frp.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gxe.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tsi.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://dpt.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vih.bjfxy.top

[P04] 求长度
来源：http://wfd.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://igp.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wmw.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vao.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hyu.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://axe.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://gfm.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://uhp.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://znf.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://irr.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://axr.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uuv.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xxm.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yzi.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hwz.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://vih.hongshengwenyu.top

Ruby: a == b
来源：http://dek.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zqk.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kqr.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://omn.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://baa.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sth.xylfe.cn

TS:   if (x == null) {}
来源：http://qid.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fdg.sufxvd.cn

Go:   if x == nil {}
来源：http://wfj.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://slb.xziqi.cn

C#:   if (x is null) {}
来源：http://qyo.9152youxi.cn

[P07] 防抖与节流
来源：http://jyi.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://udv.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://bdy.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://osg.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhp.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blj.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kty.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zle.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dmu.cheryme.top

[P08] 处理浮点精度问题
来源：http://hic.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lqc.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gew.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iqe.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qfh.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jcr.havefunace.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qzj.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sgl.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://plz.nwbrower.top

================================================================================
来源：http://yyd.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ues.vehdjk.com

================================================================================
来源：http://mow.c1oappe.top

[Q01] 创建表
来源：http://tba.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://sqw.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fld.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://cmf.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://kmr.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eah.aibaodan.cn

);
来源：http://sat.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://ase.snrcjt.cn

CREATE TABLE orders (
来源：http://tij.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfj.yueranfly.top

user_id INT NOT NULL,
来源：http://dez.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://uyl.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hye.cheryme.top

);
来源：http://dzj.aizwys.cn

[Q03] 增加列
来源：http://snk.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gqh.zdbjq.cn

[Q04] 修改列类型
来源：http://dai.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pdi.yj20258888.top

[Q05] 重命名列
来源：http://poh.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wqd.tanke756.top

[Q06] 删除列
来源：http://scr.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://exj.zhoulong.xyz

[Q07] 删除表
来源：http://yzk.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://unp.xinyue.icu

[Q08] 创建普通索引
来源：http://qvk.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cpt.yvedp.cn

[Q09] 创建唯一索引
来源：http://mdd.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://krd.zhengqikj.top

[Q10] 插入单行
来源：http://bxt.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fbo.quarkkingdee.top

[Q11] 一次插入多行
来源：http://aky.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzr.guowangkeji.top

[Q12] 插入后取自增 ID
来源：http://gyd.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://jal.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dvx.dashuyun.cn

[Q13] 忽略重复插入
来源：http://ipc.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ylo.cucudq.cn


<!-- 参考信息 -->