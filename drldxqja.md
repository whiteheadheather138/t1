代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vzq.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://awj.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://cll.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uru.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://reh.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wgb.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://guq.cashguo.top

JS:   resp.ok;  resp.status
来源：http://ohq.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://feq.yvedp.cn

Java: resp.statusCode()
来源：http://elu.dianchejie.cn

Go:   resp.StatusCode
来源：http://wkz.ppjwa.cn

Ruby: resp.code.to_i
来源：http://mfb.havefunace.top

C#:   (int)resp.StatusCode
来源：http://sje.zdqjudy.top

[L08] 并发请求多个地址
来源：http://iff.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qdk.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://ntq.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hag.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vmq.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ltz.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://otk.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rhy.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nwu.cdnleiting.top

================================================================================
来源：http://tll.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://hsi.9152youxi.cn

================================================================================
来源：http://zpt.ydzc1.top

[M01] 读取命令行参数
来源：http://urm.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://vij.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://tvo.birdmap.top

JS:   process.argv.slice(2)
来源：http://zwn.wangdashe.top

TS:   process.argv.slice(2)
来源：http://ozo.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://odr.kuanghao11.cn

Go:   os.Args[1:]
来源：http://vlw.vehdjk.com

Ruby: ARGV
来源：http://wgc.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://bvu.hesvh.cn

[M02] 读取环境变量
来源：http://dia.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://cso.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aio.nanxuanxn.top

JS:   process.env.HOME
来源：http://uql.zdbjq.cn

TS:   process.env.HOME
来源：http://tni.jiagoushi.top

Java: System.getenv("HOME")
来源：http://yxx.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://add.shuidangran.top

Ruby: ENV["HOME"]
来源：http://eqa.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ush.gaohongyu789.top

[M03] 执行外部命令
来源：http://qhg.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zsm.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://spr.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://dgp.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yhn.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svu.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kpa.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://vhd.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://sex.hfpthk.cn

[M04] 获取当前工作目录
来源：http://yoq.zycfv.cn

Py:   os.getcwd()
来源：http://cyv.gogol.net.cn

PHP:  getcwd();
来源：http://sxf.fzhhl.top

JS:   process.cwd()
来源：http://mbv.andypj.xyz

TS:   process.cwd()
来源：http://guz.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://uhz.pycfn.com

Go:   os.Getwd()
来源：http://ewm.jlsjyb.cn

Ruby: Dir.pwd
来源：http://muw.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://rct.smart0.xyz

[M05] 设置退出码
来源：http://ouf.aibaodan.cn

Py:   sys.exit(1)
来源：http://ydl.hywenlv.cn

PHP:  exit(1);
来源：http://fvd.birdmap.top

JS:   process.exit(1)
来源：http://kcw.zhongyouzk.top

TS:   process.exit(1)
来源：http://paa.havefunace.top

Java: System.exit(1)
来源：http://rnf.quarkkingdee.top

Go:   os.Exit(1)
来源：http://dzm.hesvh.cn

Ruby: exit 1
来源：http://qga.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vkc.9152youxi.cn

[M06] 向标准错误输出
来源：http://qsw.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://wlc.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://bmd.yanxiufei.cn

JS:   console.error("err")
来源：http://vmo.cucudq.cn

TS:   console.error("err")
来源：http://ysl.aibaodan.cn

Java: System.err.println("err")
来源：http://bqc.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vfj.jyoumei.cn

Ruby: warn "err"
来源：http://wcv.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://geh.hywenlv.cn

[M07] 判断是否为主入口
来源：http://ezd.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://zgp.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gxz.tanke756.top

JS:   require.main === module
来源：http://mqa.gaohongyu789.top

TS:   require.main === module
来源：http://nae.cheryme.top

Java: public static void main(String[] args)
来源：http://wif.birdmap.top

Go:   func main()
来源：http://anu.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bxq.xinyue.icu

C#:   static void Main(string[] args)
来源：http://tdw.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://hnc.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://mdx.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://wsu.wangdashe.top

JS:   process.platform;  process.version
来源：http://kss.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://yrx.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rcn.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gso.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yit.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fwj.jinyuanbaomall.cn

================================================================================
来源：http://ecm.hongshengwenyu.top

N. 数据结构与算法
来源：http://otd.snrcjt.cn

================================================================================
来源：http://yxz.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://pfn.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cwk.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gjk.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgu.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yru.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lig.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://vvv.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyn.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://pqo.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://ffh.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://luk.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rdk.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vpv.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://izn.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nlr.yj20258.top

Go:   slices.Sort(arr)
来源：http://egn.zhongyouzk.top

Ruby: arr.sort
来源：http://swx.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wce.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://zil.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qci.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://thk.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myw.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vtr.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://php.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jpp.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vjt.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://ivt.yfazqb.com

[N04] 斐波那契数列
来源：http://vez.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gna.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jeu.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cer.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knb.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tjp.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bru.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sdr.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tyg.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://uzh.316326.xyz

Py:   math.gcd(a, b)
来源：http://vtg.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://szx.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgp.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tam.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aun.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sbl.nwbrower.top

Ruby: a.gcd(b)
来源：http://jjg.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://neh.nanxinkj.top

[N06] 判断回文字符串
来源：http://ave.hesvh.cn

Py:   s == s[::-1]
来源：http://cgy.meibo888.top

PHP:  $s === strrev($s);
来源：http://flj.guannengcc.top

JS:   s === [...s].reverse().join("")
来源：http://hli.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://vtl.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bmm.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://jco.9152youxi.cn

Ruby: s == s.reverse
来源：http://ymm.cdnleiting.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xmx.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://tra.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezf.316326.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aux.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mhs.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://ltz.hcnkem.com

Java: // 手写 HashMap
来源：http://sha.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://lxj.shzxlz.cn

Ruby: // 手写 Hash
来源：http://qhp.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://dcz.feifeiyinyue.top

[N08] 生成全排列
来源：http://iqf.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://eau.xinyue.icu

PHP:  // 手写递归交换
来源：http://xsj.shzxlz.cn

JS:   // 手写回溯递归
来源：http://xmh.yangfankeji.com

TS:   // 手写回溯递归
来源：http://qtd.shuidangran.top

Java: // 手写回溯递归
来源：http://tco.sweek.top

Go:   // 手写回溯递归
来源：http://bzo.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://yjh.jiagoushi.top

C#:   // 手写回溯递归
来源：http://axz.ehwqpu.com

[N09] 栈与队列
来源：http://fmj.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rgd.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hqq.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yyx.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rxi.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yrh.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://evi.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gle.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://urt.316326.xyz

[N10] 链表节点定义
来源：http://opx.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ueu.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wlj.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xrc.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uzj.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://atn.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://yuf.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jdu.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gwa.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://aub.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://acj.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://jfb.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zck.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jta.ybcxt.top

Java: // 手写递归
来源：http://lai.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://nih.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqk.havefunace.top

C#:   // 手写递归
来源：http://hvz.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lcm.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihj.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://asm.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uom.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dkr.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vmg.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ypj.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://otw.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wfj.gogol.net.cn

================================================================================
来源：http://pya.jinqigufen.top

O. 并发与异步
来源：http://bje.zycfv.cn

================================================================================
来源：http://jjc.redwolf501.top

[O01] 启动一个线程
来源：http://vfp.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ipj.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aey.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sqh.xziqi.cn

TS:   // 同 JS
来源：http://ptt.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://zum.jinghuilouyu.cn

Go:   go f()
来源：http://zrw.0kj1m.cn

Ruby: Thread.new { f }
来源：http://yij.gzhubu.top

C#:   Task.Run(() => F());
来源：http://yxh.hammf.cn

[O02] 使用线程池
来源：http://qtf.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pgv.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fnw.52xcode.cn

JS:   // worker_threads 线程池
来源：http://xxr.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://mkb.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vew.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kcb.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lfm.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wwp.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://npb.jianghu66.top

Py:   with lock: shared += 1
来源：http://wud.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://cxq.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rdi.epnwcf.com

TS:   // 同 JS
来源：http://rtz.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://ggc.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xpl.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ayk.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://txk.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://drc.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://stn.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://siw.hcnkem.com

JS:   async function f() { await g(); }
来源：http://qgq.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gpq.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rxi.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rzq.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://mjt.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://gvr.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://uyf.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://fur.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oou.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://yqu.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://ksx.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wqr.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wnp.bjfxy.top

Ruby: threads.map(&:join)
来源：http://qdq.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://dnf.tarul.cn

[O06] 使用进程池
来源：http://evp.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gkz.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wpc.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://zuo.yj20258.top

TS:   // child_process / cluster 模块
来源：http://fwa.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://klv.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gnm.cashguo.top

Ruby: // fork 块
来源：http://bxr.zhijiandao.cn

C#:   Parallel.For
来源：http://mho.zdqjudy.top

================================================================================
来源：http://rsk.nwbrower.top

P. 常用工具函数
来源：http://hvz.hongshengwenyu.top

================================================================================
来源：http://cgi.gaohongyu789.top

[P01] 生成 UUID
来源：http://bdb.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://djt.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mcl.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://cjh.tanke756.top

TS:   crypto.randomUUID()
来源：http://ukt.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://nhq.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://wtc.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://udk.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://knk.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://tpo.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://szs.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dck.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://txz.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hib.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bzm.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://njn.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zhv.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mza.chenlongwang.top

[P03] 生成短随机字符串
来源：http://bvy.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cub.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qww.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bah.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gmz.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bea.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://msn.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gfk.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ygb.ydjk.org.cn

[P04] 求长度
来源：http://rhf.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wbv.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://geh.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfc.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dol.vqdsnc.cn


<!-- 参考信息 -->