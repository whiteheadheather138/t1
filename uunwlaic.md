代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nae.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://shv.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://trx.daria6918.cn

[L06] 解析响应为 JSON
来源：http://nfb.ppjwa.cn

Py:   resp.json()
来源：http://zaw.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://cwu.gogol.net.cn

JS:   await resp.json()
来源：http://kqe.smart0.xyz

TS:   await resp.json()
来源：http://jev.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gxw.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dib.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://zbd.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gsy.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://gth.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://obv.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oyt.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://ykk.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://bxh.andypj.xyz

Java: resp.statusCode()
来源：http://fwq.sjlbkw.cn

Go:   resp.StatusCode
来源：http://gxo.guowangkeji.top

Ruby: resp.code.to_i
来源：http://yqq.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://utk.andypj.xyz

[L08] 并发请求多个地址
来源：http://qaf.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qfa.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://dgi.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lck.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npw.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dea.xingfuxueyuan.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jdv.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dkb.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vki.zdbjq.cn

================================================================================
来源：http://dte.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://lve.pycfn.com

================================================================================
来源：http://qwb.ybcxt.top

[M01] 读取命令行参数
来源：http://bjz.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://uhj.hnqzz.top

PHP:  $argv;  $argc;
来源：http://ymh.fzhhl.top

JS:   process.argv.slice(2)
来源：http://bwv.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://ohb.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://krh.guannengcc.top

Go:   os.Args[1:]
来源：http://zaw.xziqi.cn

Ruby: ARGV
来源：http://rdy.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://dgj.svipenyu.cn

[M02] 读取环境变量
来源：http://rxx.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://dag.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://crb.dashuyun.cn

JS:   process.env.HOME
来源：http://lav.hongshengwenyu.top

TS:   process.env.HOME
来源：http://qap.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://hyy.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndk.sweek.top

Ruby: ENV["HOME"]
来源：http://ujn.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pso.tanke756.top

[M03] 执行外部命令
来源：http://eaz.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hfk.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wcz.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mza.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gup.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xkp.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mkc.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://inm.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://oxf.jiagoushi.top

[M04] 获取当前工作目录
来源：http://uiy.shanyushiyangkeji.top

Py:   os.getcwd()
来源：http://kcd.yuxming.cn

PHP:  getcwd();
来源：http://ube.yonumen.top

JS:   process.cwd()
来源：http://dis.zhoulong.xyz

TS:   process.cwd()
来源：http://zhh.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bfb.0kj1m.cn

Go:   os.Getwd()
来源：http://vxd.tarul.cn

Ruby: Dir.pwd
来源：http://iyh.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dze.gogol.net.cn

[M05] 设置退出码
来源：http://whi.quarkkingdee.top

Py:   sys.exit(1)
来源：http://mao.vehdjk.com

PHP:  exit(1);
来源：http://ehf.vehdjk.com

JS:   process.exit(1)
来源：http://png.dashuyun.cn

TS:   process.exit(1)
来源：http://els.sweek.top

Java: System.exit(1)
来源：http://ror.sxryk.cn

Go:   os.Exit(1)
来源：http://ufr.yj20258.top

Ruby: exit 1
来源：http://cfu.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tcq.9152youxi.cn

[M06] 向标准错误输出
来源：http://ofd.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://ntz.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dgw.yj202588.top

JS:   console.error("err")
来源：http://ikw.havefunace.top

TS:   console.error("err")
来源：http://ncm.ydzc1.top

Java: System.err.println("err")
来源：http://bmx.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sov.pengpengdd.cyou

Ruby: warn "err"
来源：http://ogs.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://rhh.yfazqb.com

[M07] 判断是否为主入口
来源：http://kza.yj202588.top

Py:   if __name__ == "__main__":
来源：http://esw.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cdq.jqgfzy.top

JS:   require.main === module
来源：http://qps.gotoacloud.top

TS:   require.main === module
来源：http://cml.svipenyu.cn

Java: public static void main(String[] args)
来源：http://bzj.xingfuxueyuan.xyz

Go:   func main()
来源：http://mdo.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xie.iojbl.cn

C#:   static void Main(string[] args)
来源：http://hop.sxryk.cn

[M08] 获取系统与运行时信息
来源：http://xeu.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://mqh.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://kfa.yongpay.top

JS:   process.platform;  process.version
来源：http://xcf.cucudq.cn

TS:   process.platform;  process.version
来源：http://nyq.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ywj.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://duz.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uao.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ass.jiagoushi.top

================================================================================
来源：http://jnq.ppjwa.cn

N. 数据结构与算法
来源：http://cxu.xuetiantiany.cn

================================================================================
来源：http://tya.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://brr.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vvj.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bim.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndj.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bip.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://mda.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://mkv.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lhi.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tze.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ihn.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://ure.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bry.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdx.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nye.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://obo.shuidangran.top

Go:   slices.Sort(arr)
来源：http://vhy.cucudq.cn

Ruby: arr.sort
来源：http://dju.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lwy.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://eue.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rwf.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://qkt.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://irh.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eyh.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oit.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dtv.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yjr.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ttm.fengsongda.top

[N04] 斐波那契数列
来源：http://dxb.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gum.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jtr.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wct.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gff.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ymc.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://btl.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xka.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wyp.tarul.cn

[N05] 最大公约数
来源：http://cwh.mhx1999.top

Py:   math.gcd(a, b)
来源：http://jnq.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wcj.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssh.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gai.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kdu.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lmk.tanke756.top

Ruby: a.gcd(b)
来源：http://xrg.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ejy.xylfe.cn

[N06] 判断回文字符串
来源：http://ity.chenlongwang.top

Py:   s == s[::-1]
来源：http://pej.wangdashe.top

PHP:  $s === strrev($s);
来源：http://tnn.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://icq.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://qlt.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oyw.andypj.xyz

Go:   // 双指针从两端比较
来源：http://bes.yueranfly.top

Ruby: s == s.reverse
来源：http://wxi.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wkk.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://lej.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yoz.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aht.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://lmo.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://mru.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://hrq.fktsv.cn

Go:   // 手写 map[int]int
来源：http://zmu.shuidangran.top

Ruby: // 手写 Hash
来源：http://fld.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://szd.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://glb.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://eyd.jianghu66.top

PHP:  // 手写递归交换
来源：http://tav.nanxinkj.top

JS:   // 手写回溯递归
来源：http://tdd.mhx1999.top

TS:   // 手写回溯递归
来源：http://gkm.tianlin.xyz

Java: // 手写回溯递归
来源：http://qcn.xuanzx.com

Go:   // 手写回溯递归
来源：http://aji.meibo888.top

Ruby: arr.permutation.to_a
来源：http://tdu.shzxlz.cn

C#:   // 手写回溯递归
来源：http://gfw.yangfankeji.com

[N09] 栈与队列
来源：http://pgi.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gcp.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tzy.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rtu.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xvv.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bet.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lix.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xta.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bdo.jlsjyb.cn

[N10] 链表节点定义
来源：http://uam.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://juz.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rcv.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vxj.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cqy.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://zvc.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://rof.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://acx.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://epo.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://ygl.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cuz.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://wgs.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxn.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xkr.hcnkem.com

Java: // 手写递归
来源：http://sxj.epnwcf.com

Go:   // 手写递归
来源：http://bas.yfazqb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cst.fktsv.cn

C#:   // 手写递归
来源：http://hvp.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tff.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jar.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pdz.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gll.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpq.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jay.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyj.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wvz.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zpy.feifeiyinyue.top

================================================================================
来源：http://mzr.zhijiandao.cn

O. 并发与异步
来源：http://rsd.wangshuangyany.cn

================================================================================
来源：http://knn.xuanzx.com

[O01] 启动一个线程
来源：http://ukp.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjv.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vqt.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rfw.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://rjk.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://dbv.jlsjyb.cn

Go:   go f()
来源：http://auf.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://mmk.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://rgd.sweek.top

[O02] 使用线程池
来源：http://nhr.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wsu.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kix.sysykeji.top

JS:   // worker_threads 线程池
来源：http://vte.fktsv.cn

TS:   // worker_threads 线程池
来源：http://zvr.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://kzq.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pxg.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ihy.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cxf.birdmap.top

[O03] 加锁保护共享数据
来源：http://pgr.cqqwz.cn

Py:   with lock: shared += 1
来源：http://sps.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://fyb.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ltt.fengsongda.top

TS:   // 同 JS
来源：http://pie.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://fkt.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://faw.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qtb.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://vfb.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://svq.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://qbs.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ogn.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://ngn.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jvo.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pkp.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vhb.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tqk.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://ria.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://rga.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://txa.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rqk.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://nty.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://lma.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jxs.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tvg.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://ibe.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://phy.havefunace.top

[O06] 使用进程池
来源：http://vqh.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jlw.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ljf.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://lif.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://epb.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oto.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zrk.hfpthk.cn

Ruby: // fork 块
来源：http://vnt.9152youxi.cn

C#:   Parallel.For
来源：http://qxb.hesvh.cn

================================================================================
来源：http://dww.gaohongyu789.top

P. 常用工具函数
来源：http://xsj.andypj.xyz

================================================================================
来源：http://cuy.guannengcc.top

[P01] 生成 UUID
来源：http://ugo.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://kzo.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gfd.sysykeji.top

JS:   crypto.randomUUID()
来源：http://fcl.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://vgi.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://law.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://bxv.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://uiz.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://gjq.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://jxu.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jra.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mkf.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ybg.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qal.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fyr.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vvh.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://roe.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://erc.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://fyu.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lny.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ihu.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nlm.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cwp.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dti.sjlbkw.cn


<!-- 参考信息 -->