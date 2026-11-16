代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sre.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mgi.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jln.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://ttw.zhengqikj.top

Py:   resp.json()
来源：http://hud.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://rcw.ydjk.org.cn

JS:   await resp.json()
来源：http://ykm.nwbrower.top

TS:   await resp.json()
来源：http://mpx.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vru.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rkf.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://vaq.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gee.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://cvn.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://etw.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://enx.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://gkf.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://uhx.vehdjk.com

Java: resp.statusCode()
来源：http://sji.wangdashe.top

Go:   resp.StatusCode
来源：http://rsr.fehbvm.com

Ruby: resp.code.to_i
来源：http://fzf.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://gtw.yfazqb.com

[L08] 并发请求多个地址
来源：http://ngd.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhg.ehwqpu.com

PHP:  curl_multi_init() 系列
来源：http://vdq.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jck.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mni.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pml.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://otp.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qdj.zycfv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uwi.fengsongda.top

================================================================================
来源：http://ayh.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://frz.vqdsnc.cn

================================================================================
来源：http://tgn.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://kod.tian-w.cn

Py:   sys.argv[1:]
来源：http://qkd.xinyue.icu

PHP:  $argv;  $argc;
来源：http://doy.bbcook.cn

JS:   process.argv.slice(2)
来源：http://ltu.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://hxt.cheryme.top

Java: args 数组（main 方法参数）
来源：http://xde.xuanzx.com

Go:   os.Args[1:]
来源：http://asp.snrcjt.cn

Ruby: ARGV
来源：http://tky.chenlongwang.top

C#:   args 数组（Main 方法参数）
来源：http://zkt.jianghu66.top

[M02] 读取环境变量
来源：http://yfq.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://zwk.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pog.feifeiyinyue.top

JS:   process.env.HOME
来源：http://aoi.0kj1m.cn

TS:   process.env.HOME
来源：http://qkz.shzxlz.cn

Java: System.getenv("HOME")
来源：http://prk.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sly.gzhubu.top

Ruby: ENV["HOME"]
来源：http://ntf.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tsk.hfpthk.cn

[M03] 执行外部命令
来源：http://bqk.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ndi.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ics.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fdh.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iib.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kls.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ejk.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hmq.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://arl.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://ior.vehdjk.com

Py:   os.getcwd()
来源：http://xdu.zhongyouzk.top

PHP:  getcwd();
来源：http://tzg.shanyushiyangtech.top

JS:   process.cwd()
来源：http://ayb.fanxiaobao.xyz

TS:   process.cwd()
来源：http://wgq.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://jfk.cqqwz.cn

Go:   os.Getwd()
来源：http://ckb.meibo888.top

Ruby: Dir.pwd
来源：http://arz.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://oql.xuanzx.com

[M05] 设置退出码
来源：http://kuf.birdmap.top

Py:   sys.exit(1)
来源：http://lga.hfpthk.cn

PHP:  exit(1);
来源：http://ime.tianlin.xyz

JS:   process.exit(1)
来源：http://luk.iojbl.cn

TS:   process.exit(1)
来源：http://doa.sufxvd.cn

Java: System.exit(1)
来源：http://yrc.cqqwz.cn

Go:   os.Exit(1)
来源：http://mup.zhixingplan.top

Ruby: exit 1
来源：http://qcw.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://szq.cdnleiting.top

[M06] 向标准错误输出
来源：http://xdq.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://jpc.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gok.gotoacloud.top

JS:   console.error("err")
来源：http://gwm.jianghu66.top

TS:   console.error("err")
来源：http://hxn.daria6918.cn

Java: System.err.println("err")
来源：http://vmq.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wwd.9152youxi.cn

Ruby: warn "err"
来源：http://siv.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://fpm.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://sdq.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://fax.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fyf.guannengcc.top

JS:   require.main === module
来源：http://mvc.shangyingyoupin.top

TS:   require.main === module
来源：http://rqe.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://pqb.snrcjt.cn

Go:   func main()
来源：http://uck.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fzm.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://noy.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://zva.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://qgp.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://kkf.shzxlz.cn

JS:   process.platform;  process.version
来源：http://fzs.zycfv.cn

TS:   process.platform;  process.version
来源：http://pyq.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gji.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hyr.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://taa.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dlt.uphjek.com

================================================================================
来源：http://efu.yuanzhike.top

N. 数据结构与算法
来源：http://jhg.316326.xyz

================================================================================
来源：http://usa.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://hak.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://pkd.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eng.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://odf.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qrk.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://rcv.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://wqg.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bpr.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ojz.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://nil.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://udr.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpe.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://lok.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tku.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://elj.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://jvl.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://lpu.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ugj.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://ytb.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tyw.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://pwa.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oay.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zhs.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uvv.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://utn.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vrk.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://gvm.hnqzz.top

[N04] 斐波那契数列
来源：http://rtx.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ooy.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ysd.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rki.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ywz.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zri.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sbh.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://umi.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fru.feifeiyinyue.top

[N05] 最大公约数
来源：http://wvw.xziqi.cn

Py:   math.gcd(a, b)
来源：http://ucl.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uag.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://psf.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://neb.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wko.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yiu.dianchejie.cn

Ruby: a.gcd(b)
来源：http://zdh.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qgv.mhx1999.top

[N06] 判断回文字符串
来源：http://lia.fktsv.cn

Py:   s == s[::-1]
来源：http://ael.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://phv.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://has.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://pmo.fzhhl.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aut.yvedp.cn

Go:   // 双指针从两端比较
来源：http://csx.shzxlz.cn

Ruby: s == s.reverse
来源：http://qzx.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jnd.cashguo.top

[N07] 两数之和（返回下标）
来源：http://hkb.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sbr.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zyr.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jvz.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://vdl.52xcode.cn

Java: // 手写 HashMap
来源：http://keu.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://qvh.bbcook.cn

Ruby: // 手写 Hash
来源：http://fys.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hlz.zhongyouzk.top

[N08] 生成全排列
来源：http://obx.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://rxo.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://wug.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://sot.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://qec.xinyue.icu

Java: // 手写回溯递归
来源：http://avc.meibo888.top

Go:   // 手写回溯递归
来源：http://idi.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://xrf.gogol.net.cn

C#:   // 手写回溯递归
来源：http://ktw.yj20258.top

[N09] 栈与队列
来源：http://kak.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qfi.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tca.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://veb.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ocs.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eef.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ikh.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wse.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cve.yuxming.cn

[N10] 链表节点定义
来源：http://eha.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gyo.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yas.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zxc.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vyo.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://ply.zycfv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ymf.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rao.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://qpc.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://zgb.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ume.316326.xyz

PHP:  // 手写递归函数
来源：http://tjl.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bal.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvb.havefunace.top

Java: // 手写递归
来源：http://efd.zhoulong.xyz

Go:   // 手写递归
来源：http://tjc.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kqn.tianlin.xyz

C#:   // 手写递归
来源：http://hpf.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sep.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dhy.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yar.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utf.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fyg.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jxc.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gjs.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jfd.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hgq.ydjk.org.cn

================================================================================
来源：http://ywh.sweek.top

O. 并发与异步
来源：http://lrv.dianchejie.cn

================================================================================
来源：http://mgz.yvedp.cn

[O01] 启动一个线程
来源：http://mra.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jgi.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vzi.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ewe.tian-w.cn

TS:   // 同 JS
来源：http://yrj.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://ciz.feifeiyinyue.top

Go:   go f()
来源：http://ucr.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://qza.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://zid.uphjek.com

[O02] 使用线程池
来源：http://vwk.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iug.shanyushiyangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sal.sxryk.cn

JS:   // worker_threads 线程池
来源：http://sqo.andypj.xyz

TS:   // worker_threads 线程池
来源：http://zza.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://gyo.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nrn.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mts.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ird.yuxming.cn

[O03] 加锁保护共享数据
来源：http://hta.yonumen.top

Py:   with lock: shared += 1
来源：http://jon.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://vzz.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://htx.xinyue.icu

TS:   // 同 JS
来源：http://xls.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://azn.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kvy.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ukz.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://yxu.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://mkj.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://jbl.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ayl.mhx1999.top

JS:   async function f() { await g(); }
来源：http://aus.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rkg.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://awk.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://elf.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://idc.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://hyz.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://lzx.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://llt.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dts.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://peo.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://fbn.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cil.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nxw.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://oej.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dos.ydjk.org.cn

[O06] 使用进程池
来源：http://kuz.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aiu.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qbn.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://nou.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://eyh.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jkz.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uml.aizwys.cn

Ruby: // fork 块
来源：http://ony.hongshengwenyu.top

C#:   Parallel.For
来源：http://gvd.haohaochexian.top

================================================================================
来源：http://qmk.fktsv.cn

P. 常用工具函数
来源：http://jdo.chenlongwang.top

================================================================================
来源：http://rof.jiagoushi.top

[P01] 生成 UUID
来源：http://xfk.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://dtc.tianlin.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wwo.cheryme.top

JS:   crypto.randomUUID()
来源：http://xwq.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://ptz.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://nmr.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://ffx.cashguo.top

Ruby: SecureRandom.uuid
来源：http://sfi.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://fax.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://sww.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://poe.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://trh.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://naz.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cpj.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eqp.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wfa.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wev.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rfx.chenzaomai.com

[P03] 生成短随机字符串
来源：http://awz.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hdx.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zet.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bly.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syy.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://otf.snrcjt.cn


<!-- 参考信息 -->