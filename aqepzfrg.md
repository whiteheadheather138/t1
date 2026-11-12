代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ntv.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xma.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://qaf.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://aes.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://num.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gwy.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://yyz.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://nuz.hysaishi.cn

[M04] 获取当前工作目录
来源：http://osl.52xcode.cn

Py:   os.getcwd()
来源：http://egy.jianghu66.top

PHP:  getcwd();
来源：http://ecy.mhx1999.top

JS:   process.cwd()
来源：http://gea.quarkkingdee.top

TS:   process.cwd()
来源：http://lrz.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://scz.zhiwuduotai.top

Go:   os.Getwd()
来源：http://lch.hfpthk.cn

Ruby: Dir.pwd
来源：http://mya.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://qqi.andypj.xyz

[M05] 设置退出码
来源：http://glc.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://eto.zhiwuduotai.top

PHP:  exit(1);
来源：http://jpn.jlsjyb.cn

JS:   process.exit(1)
来源：http://ubz.jiagoushi.top

TS:   process.exit(1)
来源：http://qai.zhongyouzk.top

Java: System.exit(1)
来源：http://dzs.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://tuy.dianchejie.cn

Ruby: exit 1
来源：http://wbx.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wtt.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://sia.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://oas.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xtv.hfpthk.cn

JS:   console.error("err")
来源：http://aui.yj20258888.top

TS:   console.error("err")
来源：http://wge.meibo888.top

Java: System.err.println("err")
来源：http://bmb.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvb.birdmap.top

Ruby: warn "err"
来源：http://uuf.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://nzo.guannengcc.top

[M07] 判断是否为主入口
来源：http://xxa.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://ttw.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://piz.jinqigufen.top

JS:   require.main === module
来源：http://vkv.jinyuanbaomall.cn

TS:   require.main === module
来源：http://qqb.bjfxy.top

Java: public static void main(String[] args)
来源：http://egl.yueranfly.top

Go:   func main()
来源：http://nyi.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hws.guannengcc.top

C#:   static void Main(string[] args)
来源：http://kpk.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://pgr.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://sgm.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://elu.pycfn.com

JS:   process.platform;  process.version
来源：http://fir.yangfankeji.com

TS:   process.platform;  process.version
来源：http://xdd.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cdt.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ats.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vgt.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rgd.tianlin.xyz

================================================================================
来源：http://jig.haohaochexian.top

N. 数据结构与算法
来源：http://nxw.hongshengwenyu.top

================================================================================
来源：http://xri.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://hzi.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://vlw.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wbl.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ytc.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xrg.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://rls.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://wtb.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ian.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ywx.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://kxd.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://ayx.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqx.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhb.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sjo.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nfk.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://hhk.wangdashe.top

Ruby: arr.sort
来源：http://fae.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jyb.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://vme.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cog.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://vjs.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcj.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zzf.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hdq.cucudq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://udk.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bgc.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ktk.ydjk.org.cn

[N04] 斐波那契数列
来源：http://rzw.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bgv.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fil.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wdu.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbu.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dsr.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hch.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://flx.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lyc.cqqwz.cn

[N05] 最大公约数
来源：http://arn.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://hai.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qef.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ujd.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ctt.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://euk.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byn.yonumen.top

Ruby: a.gcd(b)
来源：http://qfy.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rix.yongpay.top

[N06] 判断回文字符串
来源：http://dyq.hnqzz.top

Py:   s == s[::-1]
来源：http://phv.zycfv.cn

PHP:  $s === strrev($s);
来源：http://uxw.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://eax.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://uyd.cucudq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hfz.xinyue.icu

Go:   // 双指针从两端比较
来源：http://qvo.zdbjq.cn

Ruby: s == s.reverse
来源：http://edp.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tpk.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://vaj.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lbj.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fhz.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://shz.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://rbs.svipenyu.cn

Java: // 手写 HashMap
来源：http://yzf.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://uts.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://jgj.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://kqc.vehdjk.com

[N08] 生成全排列
来源：http://pxz.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://dui.guowangkeji.top

PHP:  // 手写递归交换
来源：http://yvy.vehdjk.com

JS:   // 手写回溯递归
来源：http://kig.ppjwa.cn

TS:   // 手写回溯递归
来源：http://nrj.yonumen.top

Java: // 手写回溯递归
来源：http://ykf.hysaishi.cn

Go:   // 手写回溯递归
来源：http://qte.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://lvp.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://iia.yueranfly.top

[N09] 栈与队列
来源：http://jur.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vag.yueranfly.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qrv.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yva.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwe.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qds.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hua.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwz.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gfe.yongpay.top

[N10] 链表节点定义
来源：http://isw.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kzp.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://viy.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ule.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xrk.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://neo.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hbd.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xfx.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bow.c1oappe.top

[N11] 二叉树中序遍历
来源：http://xlu.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oyt.sxryk.cn

PHP:  // 手写递归函数
来源：http://ibb.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwx.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wck.gotoacloud.top

Java: // 手写递归
来源：http://npx.daria6918.cn

Go:   // 手写递归
来源：http://kfs.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://haf.bbcook.cn

C#:   // 手写递归
来源：http://zbx.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://whr.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qty.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nib.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zcn.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ntg.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ohz.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qqf.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zoq.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kvz.guowangkeji.top

================================================================================
来源：http://iqm.tanke756.top

O. 并发与异步
来源：http://opm.andypj.xyz

================================================================================
来源：http://hkd.zhiwuduotai.top

[O01] 启动一个线程
来源：http://oon.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vbp.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csw.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://onj.zhoulong.xyz

TS:   // 同 JS
来源：http://nqa.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://mhg.gotoacloud.top

Go:   go f()
来源：http://btj.jiagoushi.top

Ruby: Thread.new { f }
来源：http://xjl.yonumen.top

C#:   Task.Run(() => F());
来源：http://rtl.yanxiufei.cn

[O02] 使用线程池
来源：http://lfq.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qev.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pon.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://mxj.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://nfc.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://ajm.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hsy.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqt.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://saz.ybcxt.top

[O03] 加锁保护共享数据
来源：http://boy.xuanzx.com

Py:   with lock: shared += 1
来源：http://lfn.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://tce.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oyz.hfpthk.cn

TS:   // 同 JS
来源：http://tum.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://lva.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zzo.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vpn.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://tzd.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://run.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://zni.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hyb.316326.xyz

JS:   async function f() { await g(); }
来源：http://lzg.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bpg.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kkn.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzp.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xlh.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://byl.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://gqh.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://xwx.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://psf.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://ter.birdmap.top

TS:   await Promise.all(tasks)
来源：http://gdy.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nms.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lir.shuidangran.top

Ruby: threads.map(&:join)
来源：http://cpk.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dtl.hongshengwenyu.top

[O06] 使用进程池
来源：http://yjj.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ewg.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://obt.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://vrr.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://xdb.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jvy.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lma.cheryme.top

Ruby: // fork 块
来源：http://yih.shzxlz.cn

C#:   Parallel.For
来源：http://dxz.cdnleiting.top

================================================================================
来源：http://lus.gogol.net.cn

P. 常用工具函数
来源：http://zpk.jiagoushi.top

================================================================================
来源：http://gzz.yangfankeji.com

[P01] 生成 UUID
来源：http://rod.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://vfq.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lle.cashguo.top

JS:   crypto.randomUUID()
来源：http://mrw.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://pfb.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://yqz.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://zok.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://qqe.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://rza.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://yvp.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hhe.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kyp.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://smb.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://shk.uphjek.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zyz.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fao.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ibj.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wyy.gzhubu.top

[P03] 生成短随机字符串
来源：http://pys.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfo.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rqy.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxl.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://saa.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bch.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jsy.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://pgc.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qkx.zhengqikj.top

[P04] 求长度
来源：http://nra.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lte.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgy.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ajd.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzo.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://hgo.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://gjb.haohaochexian.top

Ruby: x.length;  x.size
来源：http://ixq.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://iqo.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://zbu.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ngh.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nlg.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ukn.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cxx.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gik.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://fcd.ydzc1.top

Ruby: a == b
来源：http://uhf.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zrk.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sbb.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kdb.yongpay.top

PHP:  if (empty($x)) {}
来源：http://jec.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pof.xuanzx.com

TS:   if (x == null) {}
来源：http://pvj.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://aol.fehbvm.com

Go:   if x == nil {}
来源：http://zua.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://szv.redwolf501.top

C#:   if (x is null) {}
来源：http://yic.dashuyun.cn

[P07] 防抖与节流
来源：http://czz.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lfe.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://xgf.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpo.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wot.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vsi.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckm.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qyn.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bmr.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://nzd.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bwt.smart0.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hkl.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lwq.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hpw.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qyo.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mkj.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pej.daxiang520.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://laf.ctjpmb.com

================================================================================
来源：http://ziw.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkd.iojbl.cn

================================================================================
来源：http://gxt.guowangkeji.top

[Q01] 创建表
来源：http://rxg.cashguo.top


<!-- 参考信息 -->