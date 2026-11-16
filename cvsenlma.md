代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lea.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ilo.guannengcc.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fwi.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://diq.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vkm.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wkq.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://opb.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://lil.mhx1999.top

[M04] 获取当前工作目录
来源：http://lqf.yueranfly.top

Py:   os.getcwd()
来源：http://vim.zdqjudy.top

PHP:  getcwd();
来源：http://tap.vehdjk.com

JS:   process.cwd()
来源：http://wcd.chenjidiqi.icu

TS:   process.cwd()
来源：http://mkd.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://ymb.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://kdr.yuanzhike.top

Ruby: Dir.pwd
来源：http://wxn.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oar.pycfn.com

[M05] 设置退出码
来源：http://pou.svipenyu.cn

Py:   sys.exit(1)
来源：http://dge.yueranfly.top

PHP:  exit(1);
来源：http://gez.jyoumei.cn

JS:   process.exit(1)
来源：http://sof.xziqi.cn

TS:   process.exit(1)
来源：http://pbp.jinghuilouyu.cn

Java: System.exit(1)
来源：http://giz.chenzaomai.com

Go:   os.Exit(1)
来源：http://pyk.cucudq.cn

Ruby: exit 1
来源：http://dlr.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ovk.jinqigfzy.top

[M06] 向标准错误输出
来源：http://yqj.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://ors.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://kwp.gotoacloud.top

JS:   console.error("err")
来源：http://knu.tarul.cn

TS:   console.error("err")
来源：http://hxq.quarkkingdee.top

Java: System.err.println("err")
来源：http://zpa.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nzy.daria6918.cn

Ruby: warn "err"
来源：http://jer.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://dtm.tarul.cn

[M07] 判断是否为主入口
来源：http://ekx.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://elk.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uib.meibo888.top

JS:   require.main === module
来源：http://jsb.birdmap.top

TS:   require.main === module
来源：http://fdu.aibaodan.cn

Java: public static void main(String[] args)
来源：http://ztd.vqdsnc.cn

Go:   func main()
来源：http://uks.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lbf.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://xza.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://iip.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://ytk.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://sxy.redwolf501.top

JS:   process.platform;  process.version
来源：http://zyf.yuanzhike.top

TS:   process.platform;  process.version
来源：http://ckf.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ckd.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ugz.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oiw.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ihd.zhongyouzk.top

================================================================================
来源：http://zfx.jianghu66.top

N. 数据结构与算法
来源：http://khe.sufxvd.cn

================================================================================
来源：http://cuh.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://cdz.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://vtv.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cjk.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bso.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rxs.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://ymd.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://cuf.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://niq.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://dcd.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://anr.hesvh.cn

Py:   sorted(arr);  arr.sort()
来源：http://xdm.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wpe.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://flr.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wqg.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ydc.yonumen.top

Go:   slices.Sort(arr)
来源：http://pea.sufxvd.cn

Ruby: arr.sort
来源：http://swh.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ohl.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://vmq.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tdi.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://yrx.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ohl.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kss.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bnd.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cvb.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tcz.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pms.sjlbkw.cn

[N04] 斐波那契数列
来源：http://rth.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dpl.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eor.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gld.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ijh.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://khh.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gzy.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yqz.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zlc.tanke756.top

[N05] 最大公约数
来源：http://iew.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://ihi.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hjg.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymz.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osy.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gwu.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://leh.sufxvd.cn

Ruby: a.gcd(b)
来源：http://cmy.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kzt.sufxvd.cn

[N06] 判断回文字符串
来源：http://huy.gogol.net.cn

Py:   s == s[::-1]
来源：http://hau.redwolf501.top

PHP:  $s === strrev($s);
来源：http://uvn.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://fev.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://wkx.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rid.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://gep.tianlin.xyz

Ruby: s == s.reverse
来源：http://rze.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://znd.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://xxs.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iwu.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://voz.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cqh.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://iwx.jqgufenzy.top

Java: // 手写 HashMap
来源：http://tax.52xcode.cn

Go:   // 手写 map[int]int
来源：http://esc.zdbjq.cn

Ruby: // 手写 Hash
来源：http://ixa.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://lbx.shzxlz.cn

[N08] 生成全排列
来源：http://vwb.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://cqw.sxryk.cn

PHP:  // 手写递归交换
来源：http://eae.ivvv.top

JS:   // 手写回溯递归
来源：http://iom.chenzaomai.com

TS:   // 手写回溯递归
来源：http://cyd.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://xea.ctjpmb.com

Go:   // 手写回溯递归
来源：http://net.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://kow.dianchejie.cn

C#:   // 手写回溯递归
来源：http://kwe.feifeiyinyue.top

[N09] 栈与队列
来源：http://wbd.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nhn.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wlh.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htv.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xaj.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://brk.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://emb.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ebd.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://osa.gogol.net.cn

[N10] 链表节点定义
来源：http://lkd.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gvi.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qne.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://plw.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tyy.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://bum.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://klt.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mhd.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://okq.tanke756.top

[N11] 二叉树中序遍历
来源：http://zjj.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ddy.uphjek.com

PHP:  // 手写递归函数
来源：http://dzg.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://odg.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cny.shuidangran.top

Java: // 手写递归
来源：http://anr.9152youxi.cn

Go:   // 手写递归
来源：http://mqg.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdk.ydzc1.top

C#:   // 手写递归
来源：http://aga.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kvr.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://beh.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xiw.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pyl.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxx.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gmm.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kir.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vuk.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://upy.jinyuanbaomall.cn

================================================================================
来源：http://vei.aibaodan.cn

O. 并发与异步
来源：http://drt.aizwys.cn

================================================================================
来源：http://sei.bjfxy.top

[O01] 启动一个线程
来源：http://sgk.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uin.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ifo.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hvx.daxiang520.top

TS:   // 同 JS
来源：http://oty.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://lfa.shuidangran.top

Go:   go f()
来源：http://kdc.cheryme.top

Ruby: Thread.new { f }
来源：http://xtp.yvedp.cn

C#:   Task.Run(() => F());
来源：http://piw.smart0.xyz

[O02] 使用线程池
来源：http://qxh.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxu.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kul.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://wlb.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://dlh.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://hfg.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rig.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://awf.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jvv.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://jto.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://ryo.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://wrp.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rah.jiagoushi.top

TS:   // 同 JS
来源：http://vpj.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://gye.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dsf.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zby.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://vyg.yueranfly.top

[O04] 定义异步函数并等待
来源：http://uiw.meibo888.top

Py:   async def f():⏎    await g()
来源：http://erf.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mps.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://zee.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hbx.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tcw.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vng.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://axt.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://ejz.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://jvi.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://cog.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jqo.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://yqu.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://ccu.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fkc.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jos.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://lyc.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ath.shangyingyoupin.top

[O06] 使用进程池
来源：http://dur.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dya.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gon.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://wen.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://dua.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gsr.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://arw.jinghuilouyu.cn

Ruby: // fork 块
来源：http://izj.shangyingyoupin.top

C#:   Parallel.For
来源：http://nao.tian-w.cn

================================================================================
来源：http://luc.yfazqb.com

P. 常用工具函数
来源：http://asp.zdbjq.cn

================================================================================
来源：http://why.cdnleiting.top

[P01] 生成 UUID
来源：http://csq.tanke756.top

Py:   str(uuid.uuid4())
来源：http://yhb.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fif.uphjek.com

JS:   crypto.randomUUID()
来源：http://lpl.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://wkq.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://snp.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://wsh.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://hjj.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://vow.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://rlc.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tjz.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ygy.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cpg.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mux.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sdw.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gwo.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upx.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uiw.chenlongwang.top

[P03] 生成短随机字符串
来源：http://uxw.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lyb.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hgp.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gqt.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://agk.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nfa.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hak.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wbx.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zrt.c1oappe.top

[P04] 求长度
来源：http://oia.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jgf.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xbj.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dne.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tft.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://qjd.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://bsv.sxryk.cn

Ruby: x.length;  x.size
来源：http://dhv.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mkx.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://xye.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://pos.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bau.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nbv.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wkg.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iqs.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://fsh.ppjwa.cn

Ruby: a == b
来源：http://ugk.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qby.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ymt.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gjh.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://vdn.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fcb.meibo888.top

TS:   if (x == null) {}
来源：http://ewx.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://azl.hnqzz.top

Go:   if x == nil {}
来源：http://cew.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xap.yj20258.top

C#:   if (x is null) {}
来源：http://jko.jiagoushi.top

[P07] 防抖与节流
来源：http://ypn.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tqx.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://ahh.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dkv.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xds.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lfl.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://brn.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jrw.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vdr.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://mkb.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dar.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wjt.hnqzz.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://san.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xla.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xxq.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iki.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccf.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yjr.bjfxy.top

================================================================================
来源：http://qcf.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sqi.chenjidiqi.icu

================================================================================
来源：http://gzw.shanyushiyangkeji.top

[Q01] 创建表
来源：http://nxg.316326.xyz


<!-- 参考信息 -->