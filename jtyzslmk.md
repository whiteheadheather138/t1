代发 wailian999

TS:   process.cwd()
来源：http://lmg.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://vxt.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://hfh.316326.xyz

Ruby: Dir.pwd
来源：http://fnx.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://lsc.cqqwz.cn

[M05] 设置退出码
来源：http://kff.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://vgr.fehbvm.com

PHP:  exit(1);
来源：http://irk.snrcjt.cn

JS:   process.exit(1)
来源：http://afm.wangdashe.top

TS:   process.exit(1)
来源：http://kvf.zdqjudy.top

Java: System.exit(1)
来源：http://kmk.ehwqpu.com

Go:   os.Exit(1)
来源：http://xqu.ydzc1.top

Ruby: exit 1
来源：http://ycv.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ebo.hywenlv.cn

[M06] 向标准错误输出
来源：http://wir.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://jlz.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://spa.dashuyun.cn

JS:   console.error("err")
来源：http://cxc.fktsv.cn

TS:   console.error("err")
来源：http://qfa.zhiwuduotai.top

Java: System.err.println("err")
来源：http://cbs.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqy.daria6918.cn

Ruby: warn "err"
来源：http://ddj.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://gjn.yonumen.top

[M07] 判断是否为主入口
来源：http://vqq.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://aao.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qrw.yanxiufei.cn

JS:   require.main === module
来源：http://avy.jqgfzy.top

TS:   require.main === module
来源：http://tbg.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://aqs.andypj.xyz

Go:   func main()
来源：http://cby.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mco.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://nck.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://fwc.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://ple.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://uvg.sysykeji.top

JS:   process.platform;  process.version
来源：http://pfu.andypj.xyz

TS:   process.platform;  process.version
来源：http://yux.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ohc.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ntx.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fhf.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ezi.nanxinkj.top

================================================================================
来源：http://szt.zycfv.cn

N. 数据结构与算法
来源：http://jyf.zhiwuduotai.top

================================================================================
来源：http://zvl.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://dlm.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vms.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jnm.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rex.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://riu.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xpo.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://jtl.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zrc.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://tgd.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://iqv.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://klw.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lpl.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://wet.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyo.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fit.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://olj.zdbjq.cn

Ruby: arr.sort
来源：http://xdg.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://iap.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://wlv.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hpt.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://mwk.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lct.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lap.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sow.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://urw.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rtv.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vig.kuanghao11.cn

[N04] 斐波那契数列
来源：http://jgp.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhv.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gkd.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tdt.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uuv.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dob.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wyn.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://quh.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bur.zhengqikj.top

[N05] 最大公约数
来源：http://cpw.shuidangran.top

Py:   math.gcd(a, b)
来源：http://tud.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ucl.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rse.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfy.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ihh.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mzn.iojbl.cn

Ruby: a.gcd(b)
来源：http://tpz.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rit.hywenlv.cn

[N06] 判断回文字符串
来源：http://iqw.hcnkem.com

Py:   s == s[::-1]
来源：http://jpu.andypj.xyz

PHP:  $s === strrev($s);
来源：http://ivv.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://gkm.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://afs.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qsd.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://yob.sufxvd.cn

Ruby: s == s.reverse
来源：http://csl.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pgi.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://udq.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zfq.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wuk.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://puk.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://jll.hysaishi.cn

Java: // 手写 HashMap
来源：http://myt.havefunace.top

Go:   // 手写 map[int]int
来源：http://iac.yj20258.top

Ruby: // 手写 Hash
来源：http://byk.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://dry.shanyushiyangtech.top

[N08] 生成全排列
来源：http://tqa.yj202588.top

Py:   itertools.permutations(arr)
来源：http://eyd.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://pak.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://uqq.cdnleiting.top

TS:   // 手写回溯递归
来源：http://oca.316326.xyz

Java: // 手写回溯递归
来源：http://bar.cdnleiting.top

Go:   // 手写回溯递归
来源：http://nod.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://dtf.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://yiu.xinyue.icu

[N09] 栈与队列
来源：http://hbd.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kdu.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pcc.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bdc.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uhh.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arz.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xpu.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://frg.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://evl.snrcjt.cn

[N10] 链表节点定义
来源：http://sdx.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mwy.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nec.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iod.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oge.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://iyd.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vqw.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dnv.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vrw.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://nig.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tqq.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://uga.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwp.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wam.pengpengdd.cyou

Java: // 手写递归
来源：http://vhj.redwolf501.top

Go:   // 手写递归
来源：http://ruv.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rie.aizwys.cn

C#:   // 手写递归
来源：http://sfp.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xdg.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cjp.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://anu.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vlg.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qmd.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://itz.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ygl.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iah.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hst.zhoulong.xyz

================================================================================
来源：http://efm.yongpay.top

O. 并发与异步
来源：http://ndb.tarul.cn

================================================================================
来源：http://jwn.yj20258888.top

[O01] 启动一个线程
来源：http://tsk.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjf.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vxo.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tdg.chenjidiqi.icu

TS:   // 同 JS
来源：http://ngm.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://dlg.ybcxt.top

Go:   go f()
来源：http://ydm.gzhubu.top

Ruby: Thread.new { f }
来源：http://liw.sweek.top

C#:   Task.Run(() => F());
来源：http://soe.gzhubu.top

[O02] 使用线程池
来源：http://bmh.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uvc.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://adh.sxryk.cn

JS:   // worker_threads 线程池
来源：http://mxu.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://mrr.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hoc.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hdl.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://upn.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://two.aizwys.cn

[O03] 加锁保护共享数据
来源：http://mxv.aibaodan.cn

Py:   with lock: shared += 1
来源：http://bqg.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://nks.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xso.hnqzz.top

TS:   // 同 JS
来源：http://fwn.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://fua.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://czf.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://kwc.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://fgp.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://syz.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://xwc.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vzu.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://psl.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xqx.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jtx.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bhi.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://del.tanke756.top

C#:   async Task F() { await G(); }
来源：http://hgu.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://urd.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://wfg.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://orl.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://kfh.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://ytn.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbo.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://siq.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://edv.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tdq.hesvh.cn

[O06] 使用进程池
来源：http://vzl.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yfs.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://snc.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://znm.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://tgl.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eug.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nxn.ydzc1.top

Ruby: // fork 块
来源：http://oux.jiagoushi.top

C#:   Parallel.For
来源：http://wvg.jinqigfzy.top

================================================================================
来源：http://gab.zdbjq.cn

P. 常用工具函数
来源：http://gal.sufxvd.cn

================================================================================
来源：http://wof.ydzc1.top

[P01] 生成 UUID
来源：http://zka.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://zpn.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vwo.hammf.cn

JS:   crypto.randomUUID()
来源：http://dnw.tarul.cn

TS:   crypto.randomUUID()
来源：http://sye.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://wpx.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://frd.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://qer.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://jew.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://pcs.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfh.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjq.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pzc.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ntn.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yfd.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jka.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jhu.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pwm.nwbrower.top

[P03] 生成短随机字符串
来源：http://qkf.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://izg.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rwr.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hoo.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vuo.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eru.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vqj.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tlb.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sua.jianghu66.top

[P04] 求长度
来源：http://tuz.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wut.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zkb.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnj.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dys.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://dsu.fehbvm.com

Go:   len(arr);  len(m)
来源：http://krp.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://feg.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ocp.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://vvo.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dmt.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xwk.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ihn.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vsm.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wmo.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://hxi.52xcode.cn

Ruby: a == b
来源：http://gtp.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://odi.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pku.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gyz.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://khj.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ead.yongpay.top

TS:   if (x == null) {}
来源：http://anl.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lou.svipenyu.cn

Go:   if x == nil {}
来源：http://cqt.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://crv.aizwys.cn

C#:   if (x is null) {}
来源：http://stn.ehwqpu.com

[P07] 防抖与节流
来源：http://jng.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://thi.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://ium.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://awu.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byh.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://upl.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://whl.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pov.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zbj.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://wtr.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://voc.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://msj.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spf.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sgc.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ktx.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wom.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oep.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ugn.hywenlv.cn

================================================================================
来源：http://ofr.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vhk.yonumen.top

================================================================================
来源：http://sca.vehdjk.com

[Q01] 创建表
来源：http://ltd.gaohongyu789.top

CREATE TABLE users (
来源：http://fzr.zhengqikj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ccw.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://afp.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://vcg.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gds.meibo888.top

);
来源：http://kxi.guannengcc.top

[Q02] 创建带外键的表
来源：http://kkv.guannengcc.top

CREATE TABLE orders (
来源：http://oxf.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgr.shzxlz.cn

user_id INT NOT NULL,
来源：http://bqd.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://rjm.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qdy.yfazqb.com


<!-- 参考信息 -->