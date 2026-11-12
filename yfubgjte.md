代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lzm.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iiv.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ykx.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://gcc.kuanghao11.cn

Py:   resp.json()
来源：http://dhc.guannengcc.top

PHP:  json_decode($body, true);
来源：http://hwd.andypj.xyz

JS:   await resp.json()
来源：http://qum.feifeiyinyue.top

TS:   await resp.json()
来源：http://ofe.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://scx.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jsu.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://daz.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://umr.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://sir.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://skb.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://umy.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://sml.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://zpz.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://bds.jyoumei.cn

Go:   resp.StatusCode
来源：http://thu.gotoacloud.top

Ruby: resp.code.to_i
来源：http://ueu.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://wqm.xylfe.cn

[L08] 并发请求多个地址
来源：http://rsw.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mmt.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://bra.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmw.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://icf.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gmt.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://drj.mhx1999.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://njd.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hqj.pycfn.com

================================================================================
来源：http://izi.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://itk.zdbjq.cn

================================================================================
来源：http://iau.ybcxt.top

[M01] 读取命令行参数
来源：http://wly.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://ocl.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://umt.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://cxr.yj202588.top

TS:   process.argv.slice(2)
来源：http://cvi.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://khv.xinyue.icu

Go:   os.Args[1:]
来源：http://ror.sweek.top

Ruby: ARGV
来源：http://udl.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://bkv.sxryk.cn

[M02] 读取环境变量
来源：http://fdz.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://ryv.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ddu.zhijiandao.cn

JS:   process.env.HOME
来源：http://eni.cqqwz.cn

TS:   process.env.HOME
来源：http://awl.tian-w.cn

Java: System.getenv("HOME")
来源：http://lxu.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbe.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://ftn.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mrx.haohaochexian.top

[M03] 执行外部命令
来源：http://ige.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ant.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qxy.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vjt.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qne.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ajb.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://vcc.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://jus.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://tiz.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://fwm.hcnkem.com

Py:   os.getcwd()
来源：http://trw.gotoacloud.top

PHP:  getcwd();
来源：http://pcy.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://vdt.xylfe.cn

TS:   process.cwd()
来源：http://qrs.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://cgy.xuanzx.com

Go:   os.Getwd()
来源：http://met.redwolf501.top

Ruby: Dir.pwd
来源：http://hde.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://jlo.xuanzx.com

[M05] 设置退出码
来源：http://ygo.zhengqikj.top

Py:   sys.exit(1)
来源：http://fpz.jinghuilouyu.cn

PHP:  exit(1);
来源：http://xmk.nwbrower.top

JS:   process.exit(1)
来源：http://zjm.xziqi.cn

TS:   process.exit(1)
来源：http://ako.guannengcc.top

Java: System.exit(1)
来源：http://abd.snrcjt.cn

Go:   os.Exit(1)
来源：http://wjk.sweek.top

Ruby: exit 1
来源：http://ino.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zcw.tanke756.top

[M06] 向标准错误输出
来源：http://apb.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://qkz.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ddo.svipenyu.cn

JS:   console.error("err")
来源：http://qoi.yuxming.cn

TS:   console.error("err")
来源：http://vht.hcnkem.com

Java: System.err.println("err")
来源：http://gdq.zhaomingkeji.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ltx.jqgfzy.top

Ruby: warn "err"
来源：http://awb.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://zkl.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://zoh.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://rqu.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mys.hywenlv.cn

JS:   require.main === module
来源：http://nzy.gogol.net.cn

TS:   require.main === module
来源：http://irz.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://bjq.sufxvd.cn

Go:   func main()
来源：http://wui.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nmt.havefunace.top

C#:   static void Main(string[] args)
来源：http://mzn.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://ytj.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://zoq.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://cxx.hfpthk.cn

JS:   process.platform;  process.version
来源：http://tre.0kj1m.cn

TS:   process.platform;  process.version
来源：http://azu.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lqz.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ikk.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aas.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tlq.shangyingyoupin.top

================================================================================
来源：http://zze.feifeiyinyue.top

N. 数据结构与算法
来源：http://ubq.gzhubu.top

================================================================================
来源：http://rtx.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://qcx.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://eaj.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xcw.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmn.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sto.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://ddn.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://ayu.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vmq.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gcm.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://nlr.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://tlu.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kgl.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qmt.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://drz.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rna.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://ote.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://zrf.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ski.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://mpi.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://spx.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://ede.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgw.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckn.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xrl.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ebu.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fnn.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lhu.xziqi.cn

[N04] 斐波那契数列
来源：http://hvt.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kpl.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ain.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kna.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tiu.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wbw.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mqx.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fyv.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cdo.yj20258.top

[N05] 最大公约数
来源：http://sxv.meibo888.top

Py:   math.gcd(a, b)
来源：http://vxz.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ipe.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jkh.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nym.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mwq.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nnj.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://vbm.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wbo.aizwys.cn

[N06] 判断回文字符串
来源：http://xtr.yvedp.cn

Py:   s == s[::-1]
来源：http://xty.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://iqt.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://xtm.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://hrp.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://udx.yj20258.top

Go:   // 双指针从两端比较
来源：http://lcq.hammf.cn

Ruby: s == s.reverse
来源：http://amq.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://utf.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://nsz.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hmi.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sko.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mwt.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://whl.yangfankeji.com

Java: // 手写 HashMap
来源：http://fnp.jianghu66.top

Go:   // 手写 map[int]int
来源：http://odl.sxryk.cn

Ruby: // 手写 Hash
来源：http://eij.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yui.vqdsnc.cn

[N08] 生成全排列
来源：http://gey.yongpay.top

Py:   itertools.permutations(arr)
来源：http://ayj.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://eec.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://xek.zdbjq.cn

TS:   // 手写回溯递归
来源：http://yal.yongpay.top

Java: // 手写回溯递归
来源：http://bas.ivvv.top

Go:   // 手写回溯递归
来源：http://ciq.sweek.top

Ruby: arr.permutation.to_a
来源：http://ljp.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://ldc.fzhhl.top

[N09] 栈与队列
来源：http://ocz.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xxd.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mzg.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mli.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bur.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bso.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wxt.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ezm.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pvg.xuetiantiany.cn

[N10] 链表节点定义
来源：http://uhi.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aad.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tvo.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oyz.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://skv.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://cwc.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://zsl.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://mxg.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sbb.yuxming.cn

[N11] 二叉树中序遍历
来源：http://nuh.ehwqpu.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lhw.jqgfzy.top

PHP:  // 手写递归函数
来源：http://nsm.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vpv.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uxf.52xcode.cn

Java: // 手写递归
来源：http://fdg.chenzaomai.com

Go:   // 手写递归
来源：http://bcc.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yyo.ydzc1.top

C#:   // 手写递归
来源：http://oap.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rku.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ewi.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xfi.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dkd.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lsg.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhk.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://emv.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uxw.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://old.epnwcf.com

================================================================================
来源：http://avv.sxryk.cn

O. 并发与异步
来源：http://msf.yj20258888.top

================================================================================
来源：http://spg.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://nrb.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://efp.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hrw.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uad.tianlin.xyz

TS:   // 同 JS
来源：http://yys.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://dlb.mhx1999.top

Go:   go f()
来源：http://vpq.sysykeji.top

Ruby: Thread.new { f }
来源：http://xtt.bbcook.cn

C#:   Task.Run(() => F());
来源：http://fbq.havefunace.top

[O02] 使用线程池
来源：http://loo.hfpthk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://idk.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://doz.zycfv.cn

JS:   // worker_threads 线程池
来源：http://bwm.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://gci.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://jzu.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://poi.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bjb.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://brx.iojbl.cn

[O03] 加锁保护共享数据
来源：http://fnn.hywenlv.cn

Py:   with lock: shared += 1
来源：http://efi.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://qwk.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tbu.bjfxy.top

TS:   // 同 JS
来源：http://osc.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://onj.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iof.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wmn.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://dec.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://wyj.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://aqe.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lnu.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://eyw.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oev.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://com.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wdk.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://ere.chenjidiqi.icu

C#:   async Task F() { await G(); }
来源：http://gqc.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://gdj.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://myq.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wdt.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://cib.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://ppe.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tfq.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jut.shuidangran.top

Ruby: threads.map(&:join)
来源：http://euv.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wrf.tarul.cn

[O06] 使用进程池
来源：http://aeu.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jim.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ecm.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://obb.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://dvj.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://myp.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xhp.tanke756.top

Ruby: // fork 块
来源：http://kfv.shanyushiyangtech.top

C#:   Parallel.For
来源：http://tkq.zhoulong.xyz

================================================================================
来源：http://rri.snrcjt.cn

P. 常用工具函数
来源：http://qbq.zhoulong.xyz

================================================================================
来源：http://mqo.xuetiantiany.cn

[P01] 生成 UUID
来源：http://elg.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://knq.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jun.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://ubb.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://vkm.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://jzm.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://lby.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://zvp.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://qus.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://zcm.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ujb.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ang.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wsh.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yak.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nwk.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jcz.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aer.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kft.jqgfzy.top

[P03] 生成短随机字符串
来源：http://pju.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://omk.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ayj.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://egu.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twr.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jqx.jinqigfzy.top


<!-- 参考信息 -->