代发 wailian999

Py:   resp.json()
来源：http://pqy.hammf.cn

PHP:  json_decode($body, true);
来源：http://wpl.yongpay.top

JS:   await resp.json()
来源：http://bvt.hesvh.cn

TS:   await resp.json()
来源：http://azt.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fuf.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://coi.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://oua.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bnr.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://ruq.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ifl.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nog.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://gze.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://eya.zdqjudy.top

Java: resp.statusCode()
来源：http://wls.fehbvm.com

Go:   resp.StatusCode
来源：http://ijp.guannengcc.top

Ruby: resp.code.to_i
来源：http://sgh.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://spi.tanke756.top

[L08] 并发请求多个地址
来源：http://cib.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eav.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://edj.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpk.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvg.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wle.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kii.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kph.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qzh.hammf.cn

================================================================================
来源：http://ntj.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://csd.jianghu66.top

================================================================================
来源：http://wig.tanke756.top

[M01] 读取命令行参数
来源：http://llx.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://uyv.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://nvu.316326.xyz

JS:   process.argv.slice(2)
来源：http://ufx.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://kes.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://hwh.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://dfa.shangyingyoupin.top

Ruby: ARGV
来源：http://fjz.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://wrg.yj202588.top

[M02] 读取环境变量
来源：http://jih.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://xxq.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mln.svipenyu.cn

JS:   process.env.HOME
来源：http://pig.hesvh.cn

TS:   process.env.HOME
来源：http://gqg.sysykeji.top

Java: System.getenv("HOME")
来源：http://xbd.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xfu.pycfn.com

Ruby: ENV["HOME"]
来源：http://bmo.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rln.jiagoushi.top

[M03] 执行外部命令
来源：http://jlk.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://irk.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mtw.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kxc.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xok.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kek.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yqs.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://ccv.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://rys.cucudq.cn

[M04] 获取当前工作目录
来源：http://jrm.0kj1m.cn

Py:   os.getcwd()
来源：http://kes.sufxvd.cn

PHP:  getcwd();
来源：http://bwp.ctjpmb.com

JS:   process.cwd()
来源：http://dww.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://rxn.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://ixg.zycfv.cn

Go:   os.Getwd()
来源：http://cbi.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://xnd.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://quj.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://tiz.hesvh.cn

Py:   sys.exit(1)
来源：http://tgx.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://hsb.uphjek.com

JS:   process.exit(1)
来源：http://ima.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://div.ehwqpu.com

Java: System.exit(1)
来源：http://dsh.tarul.cn

Go:   os.Exit(1)
来源：http://zqz.vehdjk.com

Ruby: exit 1
来源：http://icp.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://usm.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://hsl.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://bzv.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uep.zhengqikj.top

JS:   console.error("err")
来源：http://gyk.jianghu66.top

TS:   console.error("err")
来源：http://enb.yj202588.top

Java: System.err.println("err")
来源：http://sfe.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ddt.tanke756.top

Ruby: warn "err"
来源：http://yby.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://nya.ivvv.top

[M07] 判断是否为主入口
来源：http://dci.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://nqq.iojbl.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gcw.hcnkem.com

JS:   require.main === module
来源：http://ysx.jlsjyb.cn

TS:   require.main === module
来源：http://xiw.redwolf501.top

Java: public static void main(String[] args)
来源：http://qlj.yuanzhike.top

Go:   func main()
来源：http://gpz.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wdj.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://bmc.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://fbc.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://oli.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://lyo.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://aeb.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://krc.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mvp.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://pkz.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://odi.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jui.nanxuanxn.top

================================================================================
来源：http://ktq.ehwqpu.com

N. 数据结构与算法
来源：http://vnk.shuidangran.top

================================================================================
来源：http://ody.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://ewb.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://izz.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cni.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vmi.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nst.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wcb.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://qnj.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zjr.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xqg.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://dnx.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://upq.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vqv.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cjt.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zvm.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hvv.meibo888.top

Go:   slices.Sort(arr)
来源：http://dwb.yj20258.top

Ruby: arr.sort
来源：http://qxg.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://hwl.yonumen.top

[N03] 快速排序（分治示例）
来源：http://qet.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nsz.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://gjc.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://daq.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://otp.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aam.yj202588.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vke.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mai.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pbz.xuanzx.com

[N04] 斐波那契数列
来源：http://hvq.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wab.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kfd.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zaj.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kvr.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vjj.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dog.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fee.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gvc.feifeiyinyue.top

[N05] 最大公约数
来源：http://zct.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://ivq.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uwx.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgh.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgu.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://klx.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iev.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://cze.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvt.jqgfzy.top

[N06] 判断回文字符串
来源：http://tvi.ctjpmb.com

Py:   s == s[::-1]
来源：http://ytm.uphjek.com

PHP:  $s === strrev($s);
来源：http://yyx.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://sgi.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://ugg.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dia.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://adc.chenlongwang.top

Ruby: s == s.reverse
来源：http://vkb.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mxu.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://icj.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gvh.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ocp.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://phf.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://wgz.zdbjq.cn

Java: // 手写 HashMap
来源：http://crm.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://cud.ehwqpu.com

Ruby: // 手写 Hash
来源：http://lbe.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://sxt.fktsv.cn

[N08] 生成全排列
来源：http://fjs.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://cun.nwbrower.top

PHP:  // 手写递归交换
来源：http://ntf.daria6918.cn

JS:   // 手写回溯递归
来源：http://afl.tanke756.top

TS:   // 手写回溯递归
来源：http://zhl.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://hkj.daxiang520.top

Go:   // 手写回溯递归
来源：http://jre.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://xsk.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://dwy.316326.xyz

[N09] 栈与队列
来源：http://mxc.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydv.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://feh.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xgv.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zor.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lhe.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pea.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyh.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nrn.zhijiandao.cn

[N10] 链表节点定义
来源：http://snr.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://irv.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://btl.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sar.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hkl.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://bqe.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://fdy.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://vid.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jkl.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://oay.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ihw.epnwcf.com

PHP:  // 手写递归函数
来源：http://zbz.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://clu.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ett.jlsjyb.cn

Java: // 手写递归
来源：http://den.daxiang520.top

Go:   // 手写递归
来源：http://yyv.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bnw.jqgfzy.top

C#:   // 手写递归
来源：http://nis.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://afz.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kfe.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bfe.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzw.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrb.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kld.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wcu.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pzb.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wnq.haohaochexian.top

================================================================================
来源：http://boz.chenzaomai.com

O. 并发与异步
来源：http://gzo.gotoacloud.top

================================================================================
来源：http://xry.zhengqikj.top

[O01] 启动一个线程
来源：http://xpg.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aei.hcnkem.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mrr.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cip.ctjpmb.com

TS:   // 同 JS
来源：http://xui.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://zsl.wangshuangyany.cn

Go:   go f()
来源：http://wyc.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://iln.yonumen.top

C#:   Task.Run(() => F());
来源：http://mda.zhengqikj.top

[O02] 使用线程池
来源：http://enm.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://akf.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mzt.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://hxo.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://yjj.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://iqg.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sds.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qls.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nku.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://pcq.cqqwz.cn

Py:   with lock: shared += 1
来源：http://egy.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://dux.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zpp.ybcxt.top

TS:   // 同 JS
来源：http://uwa.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://xcn.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://khs.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfa.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://kex.yueranfly.top

[O04] 定义异步函数并等待
来源：http://zcz.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://bjc.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dxo.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://zuj.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://urc.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vcb.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hor.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://xff.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://tor.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://yht.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://psx.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bax.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://xhh.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://mhv.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zor.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ayp.jianghu66.top

Ruby: threads.map(&:join)
来源：http://ymb.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jhp.zycfv.cn

[O06] 使用进程池
来源：http://ewa.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bsr.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mqu.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://pei.316326.xyz

TS:   // child_process / cluster 模块
来源：http://xyw.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bzz.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lot.hcnkem.com

Ruby: // fork 块
来源：http://gtj.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://vxg.52xcode.cn

================================================================================
来源：http://tqi.sufxvd.cn

P. 常用工具函数
来源：http://eoh.nwbrower.top

================================================================================
来源：http://nba.jqgfzy.top

[P01] 生成 UUID
来源：http://yxt.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://lii.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://huu.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://eyo.uphjek.com

TS:   crypto.randomUUID()
来源：http://cre.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://mgv.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://bwv.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://oqw.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://vni.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://mlk.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pmm.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xur.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://krg.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zde.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nqe.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rhm.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fny.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mzn.hnqzz.top

[P03] 生成短随机字符串
来源：http://tfq.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ygu.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hzp.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xkg.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bav.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sny.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nze.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tis.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ipj.c1oappe.top

[P04] 求长度
来源：http://mkt.cqqwz.cn


<!-- 参考信息 -->