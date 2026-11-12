代发 wailian999

Py:   resp.json()
来源：http://nsd.52xcode.cn

PHP:  json_decode($body, true);
来源：http://idh.hesvh.cn

JS:   await resp.json()
来源：http://zra.xziqi.cn

TS:   await resp.json()
来源：http://ocm.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://goc.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iav.daria6918.cn

Ruby: JSON.parse(resp.body)
来源：http://yeo.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cnv.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://myn.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qpl.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fmz.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://kvu.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://ghg.smart0.xyz

Java: resp.statusCode()
来源：http://oif.mhx1999.top

Go:   resp.StatusCode
来源：http://tgz.ybcxt.top

Ruby: resp.code.to_i
来源：http://zme.tanke756.top

C#:   (int)resp.StatusCode
来源：http://yne.jinghuilouyu.cn

[L08] 并发请求多个地址
来源：http://ykq.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fsn.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://nnu.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ynq.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aqv.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tyj.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://imf.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rus.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irn.gogol.net.cn

================================================================================
来源：http://vag.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://vey.yj20258888.top

================================================================================
来源：http://qzb.bjfxy.top

[M01] 读取命令行参数
来源：http://reo.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://auj.fktsv.cn

PHP:  $argv;  $argc;
来源：http://rox.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://vkb.hcnkem.com

TS:   process.argv.slice(2)
来源：http://vsl.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://iht.yfazqb.com

Go:   os.Args[1:]
来源：http://hwr.sxryk.cn

Ruby: ARGV
来源：http://udc.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://yaa.sweek.top

[M02] 读取环境变量
来源：http://cus.epnwcf.com

Py:   os.environ.get("HOME")
来源：http://rcr.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vmm.yongpay.top

JS:   process.env.HOME
来源：http://oeq.dianchejie.cn

TS:   process.env.HOME
来源：http://gxv.cqqwz.cn

Java: System.getenv("HOME")
来源：http://hry.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awh.zycfv.cn

Ruby: ENV["HOME"]
来源：http://jwm.yj20258.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jri.hysaishi.cn

[M03] 执行外部命令
来源：http://ndp.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vry.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cbp.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dem.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tku.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hay.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yay.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sfk.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://ofj.gotoacloud.top

[M04] 获取当前工作目录
来源：http://bdm.nanxuanxn.top

Py:   os.getcwd()
来源：http://urt.fktsv.cn

PHP:  getcwd();
来源：http://bmr.fzhhl.top

JS:   process.cwd()
来源：http://mwu.tarul.cn

TS:   process.cwd()
来源：http://rmi.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://gxr.kuanghao11.cn

Go:   os.Getwd()
来源：http://pwd.sjlbkw.cn

Ruby: Dir.pwd
来源：http://upa.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zjn.zhixingplan.top

[M05] 设置退出码
来源：http://jqd.jlsjyb.cn

Py:   sys.exit(1)
来源：http://ypb.shanyushiyangtech.top

PHP:  exit(1);
来源：http://lsu.daxiang520.top

JS:   process.exit(1)
来源：http://oww.cashguo.top

TS:   process.exit(1)
来源：http://dou.haohaochexian.top

Java: System.exit(1)
来源：http://jpw.iojbl.cn

Go:   os.Exit(1)
来源：http://cid.meibo888.top

Ruby: exit 1
来源：http://knx.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jmj.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://bpm.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://gcg.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://smk.chenzaomai.com

JS:   console.error("err")
来源：http://yoy.jqgufenzy.top

TS:   console.error("err")
来源：http://lwg.sweek.top

Java: System.err.println("err")
来源：http://kau.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zwu.fzhhl.top

Ruby: warn "err"
来源：http://zlm.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://wql.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://gmd.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://wmv.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aku.redwolf501.top

JS:   require.main === module
来源：http://xed.jinqigfzy.top

TS:   require.main === module
来源：http://vem.c1oappe.top

Java: public static void main(String[] args)
来源：http://gvz.dianchejie.cn

Go:   func main()
来源：http://bmu.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rrp.ydzc1.top

C#:   static void Main(string[] args)
来源：http://ygd.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://emh.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://egi.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://hgg.uphjek.com

JS:   process.platform;  process.version
来源：http://mkx.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://lbc.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nda.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://gik.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sci.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qcw.ywan-chungtsiang.top

================================================================================
来源：http://pfk.ppjwa.cn

N. 数据结构与算法
来源：http://jec.wangdashe.top

================================================================================
来源：http://mcm.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://tvj.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://rsv.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://len.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://agu.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ocz.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xfx.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://fde.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vnq.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://udz.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zvi.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://irj.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bke.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zsn.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://asb.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nsv.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://zwd.zhijiandao.cn

Ruby: arr.sort
来源：http://tjk.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xrm.316326.xyz

[N03] 快速排序（分治示例）
来源：http://qnb.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uro.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://wlv.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cic.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wlj.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bev.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://swj.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lcu.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://bgu.yangfankeji.com

[N04] 斐波那契数列
来源：http://cej.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fsp.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mzk.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://efv.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iiq.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ugn.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phb.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tyk.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jwa.aizwys.cn

[N05] 最大公约数
来源：http://zna.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://hio.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xff.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hna.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zfo.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itc.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bbn.jiagoushi.top

Ruby: a.gcd(b)
来源：http://zrf.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pvj.jiagoushi.top

[N06] 判断回文字符串
来源：http://koq.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://plh.daria6918.cn

PHP:  $s === strrev($s);
来源：http://hun.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://qbh.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://trm.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://khk.sysykeji.top

Go:   // 双指针从两端比较
来源：http://jeh.redwolf501.top

Ruby: s == s.reverse
来源：http://jyd.vqdsnc.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xsg.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://ude.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pbz.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qal.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kyj.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://lqx.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://ydo.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://qay.vqdsnc.cn

Ruby: // 手写 Hash
来源：http://ona.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://lvi.chenlongwang.top

[N08] 生成全排列
来源：http://viz.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://wyq.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://kui.ydzc1.top

JS:   // 手写回溯递归
来源：http://ijn.ydzc1.top

TS:   // 手写回溯递归
来源：http://npm.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://taa.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://vcc.tanke756.top

Ruby: arr.permutation.to_a
来源：http://hot.meibo888.top

C#:   // 手写回溯递归
来源：http://rtc.ctjpmb.com

[N09] 栈与队列
来源：http://iwc.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uim.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lnh.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dqz.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rkn.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bjs.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vtu.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xsg.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gtz.jqgfzy.top

[N10] 链表节点定义
来源：http://omg.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mxf.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://vmz.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oyz.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nfk.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://ffv.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://izo.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hky.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gnd.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://utv.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://obr.chenlongwang.top

PHP:  // 手写递归函数
来源：http://vnt.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnz.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zgg.yj202588.top

Java: // 手写递归
来源：http://txr.yanxiufei.cn

Go:   // 手写递归
来源：http://rjp.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fat.haohaochexian.top

C#:   // 手写递归
来源：http://uaj.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sgx.cucudq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wre.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fub.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxp.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxf.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwi.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gmn.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ean.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gsx.tian-w.cn

================================================================================
来源：http://tsz.gzhubu.top

O. 并发与异步
来源：http://egv.meibo888.top

================================================================================
来源：http://kak.zhengqikj.top

[O01] 启动一个线程
来源：http://ccd.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fwd.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wqg.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://poo.birdmap.top

TS:   // 同 JS
来源：http://osk.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://rni.birdmap.top

Go:   go f()
来源：http://qfz.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://cvv.yj20258.top

C#:   Task.Run(() => F());
来源：http://mrq.yuxming.cn

[O02] 使用线程池
来源：http://pzs.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bur.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ggp.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://qsz.uphjek.com

TS:   // worker_threads 线程池
来源：http://qma.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ebf.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlb.birdmap.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cpw.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iac.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://nmw.yueranfly.top

Py:   with lock: shared += 1
来源：http://uqd.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://nli.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lkl.dianchejie.cn

TS:   // 同 JS
来源：http://udb.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://lad.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rlq.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xvo.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://hvj.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://zbp.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://bgw.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vtk.aizwys.cn

JS:   async function f() { await g(); }
来源：http://uyp.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eql.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ota.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nse.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://bks.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://qgm.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://hzp.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://ruk.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kjb.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://wxp.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://qhg.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qhr.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wkm.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://gan.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://vtr.jyoumei.cn

[O06] 使用进程池
来源：http://wfl.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tzh.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://paq.hammf.cn

JS:   // child_process / cluster 模块
来源：http://fkf.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://uye.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wag.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sgz.shuidangran.top

Ruby: // fork 块
来源：http://hzh.bjfxy.top

C#:   Parallel.For
来源：http://soq.guowangkeji.top

================================================================================
来源：http://xjb.yangfankeji.com

P. 常用工具函数
来源：http://eyv.jinyuanbaomall.cn

================================================================================
来源：http://fyi.dashuyun.cn

[P01] 生成 UUID
来源：http://hyw.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://fcp.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bbo.hammf.cn

JS:   crypto.randomUUID()
来源：http://thb.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://dyr.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://prx.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://naq.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://egp.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://piw.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://kol.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fmr.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ydo.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fap.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bco.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uix.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ijj.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hiv.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mnq.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://xyb.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jeb.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yog.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gec.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwa.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vim.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eod.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ewd.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kda.chenzaomai.com

[P04] 求长度
来源：http://hui.tanke756.top


<!-- 参考信息 -->