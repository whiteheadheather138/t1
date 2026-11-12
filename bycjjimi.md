代发 wailian999

TS:   process.cwd()
来源：http://lxy.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://bcf.epnwcf.com

Go:   os.Getwd()
来源：http://fce.sxryk.cn

Ruby: Dir.pwd
来源：http://eac.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tuz.cheryme.top

[M05] 设置退出码
来源：http://sjc.dashuyun.cn

Py:   sys.exit(1)
来源：http://azr.zdqjudy.top

PHP:  exit(1);
来源：http://wiq.tian-w.cn

JS:   process.exit(1)
来源：http://jqz.cheryme.top

TS:   process.exit(1)
来源：http://hct.guannengcc.top

Java: System.exit(1)
来源：http://uca.gotoacloud.top

Go:   os.Exit(1)
来源：http://mqf.iojbl.cn

Ruby: exit 1
来源：http://zyv.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uxk.xylfe.cn

[M06] 向标准错误输出
来源：http://sno.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://gpl.cdnleiting.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xly.gotoacloud.top

JS:   console.error("err")
来源：http://jlr.zhongyouzk.top

TS:   console.error("err")
来源：http://ahs.xziqi.cn

Java: System.err.println("err")
来源：http://atg.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dwq.cashguo.top

Ruby: warn "err"
来源：http://spi.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://skb.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://aeu.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://kcx.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qqo.meibo888.top

JS:   require.main === module
来源：http://jrc.yuxming.cn

TS:   require.main === module
来源：http://hzq.hywenlv.cn

Java: public static void main(String[] args)
来源：http://inw.gogol.net.cn

Go:   func main()
来源：http://wiz.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psw.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://kzs.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://vwh.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://rov.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://vak.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://waq.ppjwa.cn

TS:   process.platform;  process.version
来源：http://pvs.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dxn.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bvr.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hbc.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xdn.guannengcc.top

================================================================================
来源：http://eew.jinghuilouyu.cn

N. 数据结构与算法
来源：http://lce.sxryk.cn

================================================================================
来源：http://idu.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://eac.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://amq.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wbr.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://asv.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bde.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rev.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://bis.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://llz.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://acj.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://hph.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gcp.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gnr.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpo.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://irz.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cho.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://jbb.jyoumei.cn

Ruby: arr.sort
来源：http://awm.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oqw.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://bsz.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bno.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://rpl.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kse.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vby.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://not.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cpb.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fak.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://ker.fehbvm.com

[N04] 斐波那契数列
来源：http://nzb.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jyi.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lyk.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vdh.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://atj.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uap.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eaq.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://adx.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cix.zhixingplan.top

[N05] 最大公约数
来源：http://axz.xuanzx.com

Py:   math.gcd(a, b)
来源：http://zko.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kux.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jnt.chenlongwang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zuq.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://acm.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixz.aizwys.cn

Ruby: a.gcd(b)
来源：http://tzd.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uee.yvedp.cn

[N06] 判断回文字符串
来源：http://qaf.chenzaomai.com

Py:   s == s[::-1]
来源：http://fqp.daria6918.cn

PHP:  $s === strrev($s);
来源：http://xmw.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://dzd.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://jww.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gqm.hesvh.cn

Go:   // 双指针从两端比较
来源：http://pbq.yuanzhike.top

Ruby: s == s.reverse
来源：http://fre.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dqd.zhiwuduotai.top

[N07] 两数之和（返回下标）
来源：http://aip.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vds.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nrk.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qri.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://ayq.hammf.cn

Java: // 手写 HashMap
来源：http://jos.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://xgs.sysykeji.top

Ruby: // 手写 Hash
来源：http://fgz.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://ada.yongpay.top

[N08] 生成全排列
来源：http://sbr.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://qdd.hesvh.cn

PHP:  // 手写递归交换
来源：http://njr.shuidangran.top

JS:   // 手写回溯递归
来源：http://jns.tianlin.xyz

TS:   // 手写回溯递归
来源：http://khx.vqdsnc.cn

Java: // 手写回溯递归
来源：http://rlj.gzhubu.top

Go:   // 手写回溯递归
来源：http://ych.hammf.cn

Ruby: arr.permutation.to_a
来源：http://ide.ybcxt.top

C#:   // 手写回溯递归
来源：http://kfv.zycfv.cn

[N09] 栈与队列
来源：http://teq.gogol.net.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kmp.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nxg.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ksd.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jco.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://puo.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewz.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yea.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xrn.birdmap.top

[N10] 链表节点定义
来源：http://qcb.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfi.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sel.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rut.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mrv.yj202588.top

Java: class Node { int v; Node next; }
来源：http://uzi.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://aeg.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kvq.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://msw.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://ajj.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://enb.jianghu66.top

PHP:  // 手写递归函数
来源：http://jci.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qah.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cob.hywenlv.cn

Java: // 手写递归
来源：http://fft.meibo888.top

Go:   // 手写递归
来源：http://inb.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yvz.cdnleiting.top

C#:   // 手写递归
来源：http://gho.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iac.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fta.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xes.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erp.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bzy.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xpc.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aqr.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://szy.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ebb.chenzaomai.com

================================================================================
来源：http://umw.havefunace.top

O. 并发与异步
来源：http://pwp.cdnleiting.top

================================================================================
来源：http://npk.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://jji.yueranfly.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kgl.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wtl.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzl.shangyingyoupin.top

TS:   // 同 JS
来源：http://nts.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://ytv.yongpay.top

Go:   go f()
来源：http://qyy.gogol.net.cn

Ruby: Thread.new { f }
来源：http://zxe.bbcook.cn

C#:   Task.Run(() => F());
来源：http://cpn.zhijiandao.cn

[O02] 使用线程池
来源：http://zbr.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rrm.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ayk.shuidangran.top

JS:   // worker_threads 线程池
来源：http://mvk.316326.xyz

TS:   // worker_threads 线程池
来源：http://jqc.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://ubg.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pwm.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://axn.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vuo.tanke756.top

[O03] 加锁保护共享数据
来源：http://hqh.pycfn.com

Py:   with lock: shared += 1
来源：http://uqw.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://roa.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hkl.52xcode.cn

TS:   // 同 JS
来源：http://mpf.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://wxa.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zji.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yjb.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://vrd.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://fkq.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://hui.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pdc.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://gjt.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tiu.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mdg.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xzb.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://bgm.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://ukq.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://fhk.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://bxl.fengsongda.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ecu.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://tmk.cashguo.top

TS:   await Promise.all(tasks)
来源：http://qxr.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wbv.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kwl.epnwcf.com

Ruby: threads.map(&:join)
来源：http://vie.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jpu.epnwcf.com

[O06] 使用进程池
来源：http://bny.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vcy.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://wwn.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://kpe.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://hmy.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ghv.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yjp.zycfv.cn

Ruby: // fork 块
来源：http://wvy.nwbrower.top

C#:   Parallel.For
来源：http://mbo.tianlin.xyz

================================================================================
来源：http://dgb.svipenyu.cn

P. 常用工具函数
来源：http://azp.snrcjt.cn

================================================================================
来源：http://vcx.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://mxx.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://aqs.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ive.xziqi.cn

JS:   crypto.randomUUID()
来源：http://roy.xuanzx.com

TS:   crypto.randomUUID()
来源：http://ppt.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://pwx.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://mxi.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://isb.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://ryf.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://yzu.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://chs.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://icn.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zka.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://udk.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cie.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gli.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aes.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://psg.hnqzz.top

[P03] 生成短随机字符串
来源：http://lrt.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kwh.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jan.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://orz.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nhd.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lda.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ylq.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cow.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ait.nanxuanxn.top

[P04] 求长度
来源：http://awk.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rhm.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mlp.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jra.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://daf.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://dfn.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://xtt.sysykeji.top

Ruby: x.length;  x.size
来源：http://flp.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jwn.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://jji.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hpy.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qsl.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://waq.gaohongyu789.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://avm.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cxt.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://uyt.hysaishi.cn

Ruby: a == b
来源：http://qkz.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bth.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://umb.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agv.birdmap.top

PHP:  if (empty($x)) {}
来源：http://lut.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cjr.ydzc1.top

TS:   if (x == null) {}
来源：http://obb.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://avh.tianlin.xyz

Go:   if x == nil {}
来源：http://geu.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yyg.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://oeu.pycfn.com

[P07] 防抖与节流
来源：http://ahu.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gba.tarul.cn

PHP:  // 手写时间戳比较
来源：http://igb.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iur.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixh.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yrs.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bub.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ept.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lnk.wangdashe.top

[P08] 处理浮点精度问题
来源：http://bgj.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://usg.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uie.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pys.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kaf.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fvi.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cmt.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xeb.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iqk.zdqjudy.top

================================================================================
来源：http://ysd.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iom.zhixingplan.top

================================================================================
来源：http://wmp.hysaishi.cn

[Q01] 创建表
来源：http://wup.daxiang520.top

CREATE TABLE users (
来源：http://ljw.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggw.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://out.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://not.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghb.ybcxt.top

);
来源：http://ifk.aibaodan.cn

[Q02] 创建带外键的表
来源：http://pbj.shuidangran.top

CREATE TABLE orders (
来源：http://oow.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ubk.iojbl.cn

user_id INT NOT NULL,
来源：http://lgo.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://uhd.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kxe.jianghu66.top


<!-- 参考信息 -->