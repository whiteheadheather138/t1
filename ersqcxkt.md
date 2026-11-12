代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oah.cashguo.top

Ruby: warn "err"
来源：http://ggl.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://tnd.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://jbi.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://qqe.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eiq.yj20258888.top

JS:   require.main === module
来源：http://lor.daxiang520.top

TS:   require.main === module
来源：http://edy.yuanzhike.top

Java: public static void main(String[] args)
来源：http://qhk.yangfankeji.com

Go:   func main()
来源：http://cje.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mtf.jianghu66.top

C#:   static void Main(string[] args)
来源：http://lqw.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://bzh.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://ikk.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://vrv.aibaodan.cn

JS:   process.platform;  process.version
来源：http://khv.sweek.top

TS:   process.platform;  process.version
来源：http://ygs.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bzw.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mqi.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://shr.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qzu.mhx1999.top

================================================================================
来源：http://gnk.shanyushiyangtech.top

N. 数据结构与算法
来源：http://skf.sjlbkw.cn

================================================================================
来源：http://dbt.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://trm.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://asw.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lqa.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vml.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yox.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://kpt.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://zsh.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hif.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tdc.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://ida.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://ryq.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://upn.daxiang520.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pmi.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mgf.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mwk.fzhhl.top

Go:   slices.Sort(arr)
来源：http://kpg.aizwys.cn

Ruby: arr.sort
来源：http://zzj.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://nmj.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://txq.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jck.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://xaj.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccd.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfx.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gxd.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kga.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jgl.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://jgc.haohaochexian.top

[N04] 斐波那契数列
来源：http://npm.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bqc.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gkc.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://flp.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnz.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nsv.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rma.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lub.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nef.cheryme.top

[N05] 最大公约数
来源：http://eys.redwolf501.top

Py:   math.gcd(a, b)
来源：http://bnq.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nvv.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvh.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcv.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://myf.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://smi.yfazqb.com

Ruby: a.gcd(b)
来源：http://vnn.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://loj.sweek.top

[N06] 判断回文字符串
来源：http://kqa.uphjek.com

Py:   s == s[::-1]
来源：http://pwh.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://sec.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://vzl.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://dmo.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ctr.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://yoj.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://qek.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wlb.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://iao.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oct.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgz.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rdg.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://ovd.zhoulong.xyz

Java: // 手写 HashMap
来源：http://vep.gzhubu.top

Go:   // 手写 map[int]int
来源：http://igd.smart0.xyz

Ruby: // 手写 Hash
来源：http://aau.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gah.yfazqb.com

[N08] 生成全排列
来源：http://sdg.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://zwv.fzhhl.top

PHP:  // 手写递归交换
来源：http://vgs.cqqwz.cn

JS:   // 手写回溯递归
来源：http://jnq.birdmap.top

TS:   // 手写回溯递归
来源：http://gcb.uphjek.com

Java: // 手写回溯递归
来源：http://gqa.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://fhd.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://wzw.yvedp.cn

C#:   // 手写回溯递归
来源：http://egd.hysaishi.cn

[N09] 栈与队列
来源：http://yok.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xny.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zos.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrc.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ppf.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzf.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://elx.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hyj.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://usw.ivvv.top

[N10] 链表节点定义
来源：http://ryu.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nti.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://ucz.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mnr.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fbe.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://zbg.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nzf.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xag.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vmc.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://rpc.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nqc.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://sxo.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nni.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otu.hongshengwenyu.top

Java: // 手写递归
来源：http://uai.gzhubu.top

Go:   // 手写递归
来源：http://ygy.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iuq.shanyushiyangkeji.top

C#:   // 手写递归
来源：http://zti.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://grr.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ojz.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ytw.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxk.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ifq.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ezp.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rox.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fjv.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jhd.epnwcf.com

================================================================================
来源：http://vke.sweek.top

O. 并发与异步
来源：http://fiu.hammf.cn

================================================================================
来源：http://lpk.hywenlv.cn

[O01] 启动一个线程
来源：http://ejj.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gic.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ojm.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aaa.sjlbkw.cn

TS:   // 同 JS
来源：http://thd.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://lha.fengsongda.top

Go:   go f()
来源：http://mqy.vehdjk.com

Ruby: Thread.new { f }
来源：http://ojq.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://mda.jinghuilouyu.cn

[O02] 使用线程池
来源：http://nun.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://amd.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://clg.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://pyz.52xcode.cn

TS:   // worker_threads 线程池
来源：http://quq.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://kzn.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ukf.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sur.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bxm.bjfxy.top

[O03] 加锁保护共享数据
来源：http://qog.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://mon.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://ltt.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cfk.birdmap.top

TS:   // 同 JS
来源：http://efd.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://chq.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://srx.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://psg.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://urc.yj202588.top

[O04] 定义异步函数并等待
来源：http://uqh.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://fjz.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhn.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://wrb.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://epj.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbu.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yod.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://bor.havefunace.top

C#:   async Task F() { await G(); }
来源：http://yxp.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://aka.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://hpf.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fmg.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://lnr.tanke756.top

TS:   await Promise.all(tasks)
来源：http://lxm.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://avu.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hlx.sweek.top

Ruby: threads.map(&:join)
来源：http://ess.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://gvf.yj202588.top

[O06] 使用进程池
来源：http://qzb.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zxx.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://qgu.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://ogj.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://jmz.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://scu.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jmt.cheryme.top

Ruby: // fork 块
来源：http://vrt.yj20258888.top

C#:   Parallel.For
来源：http://beh.guowangkeji.top

================================================================================
来源：http://kzz.zhijiandao.cn

P. 常用工具函数
来源：http://zwq.ppjwa.cn

================================================================================
来源：http://ssi.fktsv.cn

[P01] 生成 UUID
来源：http://rkm.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://kkp.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mua.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://vdc.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://tbp.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://sed.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://slf.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://ycb.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://tjo.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://oil.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccc.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tzf.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ngb.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qwf.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzm.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qsm.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kgr.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zek.nanxinkj.top

[P03] 生成短随机字符串
来源：http://zzj.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fnl.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yjw.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ooz.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mew.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tkm.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zlx.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qey.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oga.zycfv.cn

[P04] 求长度
来源：http://oee.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yju.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://itb.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vil.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okp.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://fau.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://qlf.xylfe.cn

Ruby: x.length;  x.size
来源：http://nap.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pdd.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://wle.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cwb.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vkm.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jhl.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nct.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://drs.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gzx.yueranfly.top

Ruby: a == b
来源：http://prf.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ecb.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bng.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://neq.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://nzv.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fct.ctjpmb.com

TS:   if (x == null) {}
来源：http://ymj.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xnn.fehbvm.com

Go:   if x == nil {}
来源：http://yaq.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbc.zhoulong.xyz

C#:   if (x is null) {}
来源：http://ern.shangyingyoupin.top

[P07] 防抖与节流
来源：http://zsu.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rzn.cheryme.top

PHP:  // 手写时间戳比较
来源：http://rrv.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irx.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgp.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dfn.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wbj.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kyg.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qte.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://udd.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yky.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vwv.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://axf.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nyi.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kxi.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vqd.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cko.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jnq.sjlbkw.cn

================================================================================
来源：http://urx.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wtd.quarkkingdee.top

================================================================================
来源：http://kms.yuanzhike.top

[Q01] 创建表
来源：http://oif.sufxvd.cn

CREATE TABLE users (
来源：http://ijz.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://okv.quarkkingdee.top

name VARCHAR(50) NOT NULL,
来源：http://qgx.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://ygl.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jzj.shangyingyoupin.top

);
来源：http://cny.yfazqb.com

[Q02] 创建带外键的表
来源：http://vvf.uphjek.com

CREATE TABLE orders (
来源：http://ebr.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ein.ivvv.top

user_id INT NOT NULL,
来源：http://ftm.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://vlh.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://alo.jlsjyb.cn

);
来源：http://pxk.hcnkem.com

[Q03] 增加列
来源：http://wyz.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aty.fzhhl.top

[Q04] 修改列类型
来源：http://fnd.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uem.hfpthk.cn

[Q05] 重命名列
来源：http://zao.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://swd.xziqi.cn

[Q06] 删除列
来源：http://jpc.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://ccd.hesvh.cn

[Q07] 删除表
来源：http://ghq.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://inv.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://klf.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pki.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://dum.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rdy.pycfn.com

[Q10] 插入单行
来源：http://mxw.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gzo.yj20258888.top

[Q11] 一次插入多行
来源：http://ezi.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vmh.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://gip.daxiang520.top


<!-- 参考信息 -->