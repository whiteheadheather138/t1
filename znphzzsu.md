代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://liw.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kaa.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cef.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nqq.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxa.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ede.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://czu.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://tym.zhongyouzk.top

Py:   resp.json()
来源：http://zsy.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://gcc.wangshuangyany.cn

JS:   await resp.json()
来源：http://cnb.cheryme.top

TS:   await resp.json()
来源：http://cxf.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dia.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mvw.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://afe.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hle.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://dys.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wba.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://clg.ydjk.org.cn

JS:   resp.ok;  resp.status
来源：http://ody.meibo888.top

TS:   resp.ok;  resp.status
来源：http://udu.fktsv.cn

Java: resp.statusCode()
来源：http://hje.nwbrower.top

Go:   resp.StatusCode
来源：http://yyx.sysykeji.top

Ruby: resp.code.to_i
来源：http://ufe.meibo888.top

C#:   (int)resp.StatusCode
来源：http://kvb.hfpthk.cn

[L08] 并发请求多个地址
来源：http://pqs.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cbn.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://lmc.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gzm.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mcn.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uvs.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wfb.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://req.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qho.hfpthk.cn

================================================================================
来源：http://iqv.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://ivn.pycfn.com

================================================================================
来源：http://vao.ppjwa.cn

[M01] 读取命令行参数
来源：http://wya.sysykeji.top

Py:   sys.argv[1:]
来源：http://pfs.yfazqb.com

PHP:  $argv;  $argc;
来源：http://xuj.bbcook.cn

JS:   process.argv.slice(2)
来源：http://rvi.xuanzx.com

TS:   process.argv.slice(2)
来源：http://bdw.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://nkp.guannengcc.top

Go:   os.Args[1:]
来源：http://xes.yj202588.top

Ruby: ARGV
来源：http://fii.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://fhn.hysaishi.cn

[M02] 读取环境变量
来源：http://mjt.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://jxv.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpn.yonumen.top

JS:   process.env.HOME
来源：http://rvf.birdmap.top

TS:   process.env.HOME
来源：http://bdw.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://rtp.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://inh.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://bho.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ezr.yuanzhike.top

[M03] 执行外部命令
来源：http://dbf.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zfy.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ocq.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vik.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rxf.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ren.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://bvi.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://ioz.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://pof.yfazqb.com

[M04] 获取当前工作目录
来源：http://hsj.zdqjudy.top

Py:   os.getcwd()
来源：http://aej.ctjpmb.com

PHP:  getcwd();
来源：http://obl.xziqi.cn

JS:   process.cwd()
来源：http://upx.fengsongda.top

TS:   process.cwd()
来源：http://ann.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://rfw.guowangkeji.top

Go:   os.Getwd()
来源：http://nqx.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://rto.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://tks.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://our.zhixingplan.top

Py:   sys.exit(1)
来源：http://dvd.nanxuanxn.top

PHP:  exit(1);
来源：http://blu.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://ftw.zycfv.cn

TS:   process.exit(1)
来源：http://plv.nwbrower.top

Java: System.exit(1)
来源：http://egq.yueranfly.top

Go:   os.Exit(1)
来源：http://pcl.zhengqikj.top

Ruby: exit 1
来源：http://rgx.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pqy.guannengcc.top

[M06] 向标准错误输出
来源：http://yno.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://scl.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://qvr.gzhubu.top

JS:   console.error("err")
来源：http://hbe.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://krj.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ooh.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kck.andypj.xyz

Ruby: warn "err"
来源：http://wca.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://wfb.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://iil.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://jei.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tul.sxryk.cn

JS:   require.main === module
来源：http://tfo.feifeiyinyue.top

TS:   require.main === module
来源：http://lil.316326.xyz

Java: public static void main(String[] args)
来源：http://taa.ydzc1.top

Go:   func main()
来源：http://ywk.pengpengdd.cyou

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://txi.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://rml.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://jix.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://zvx.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://req.nwbrower.top

JS:   process.platform;  process.version
来源：http://oxf.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://kpj.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nlr.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gsb.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uiw.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qnk.nwbrower.top

================================================================================
来源：http://sqr.jlsjyb.cn

N. 数据结构与算法
来源：http://wme.chenzaomai.com

================================================================================
来源：http://jyd.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://pqm.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lqv.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://itg.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abb.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggl.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://grf.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://exm.zdqjudy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fzr.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://fzm.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://tno.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://oym.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://stm.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ejr.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bfm.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ren.uphjek.com

Go:   slices.Sort(arr)
来源：http://zcj.cheryme.top

Ruby: arr.sort
来源：http://mxw.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gnq.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://his.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://puz.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://xvv.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbf.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jnu.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gbk.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qxs.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iue.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://woh.gogol.net.cn

[N04] 斐波那契数列
来源：http://tsp.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jfv.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zfe.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jjc.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://osg.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://knd.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uwu.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://akk.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://igd.snrcjt.cn

[N05] 最大公约数
来源：http://esv.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://zfg.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rne.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmh.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zop.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://let.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfa.chenzaomai.com

Ruby: a.gcd(b)
来源：http://ube.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rmc.jqgufenzy.top

[N06] 判断回文字符串
来源：http://mdq.jiagoushi.top

Py:   s == s[::-1]
来源：http://gvk.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://qxn.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://qlv.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://tpr.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://njq.cheryme.top

Go:   // 双指针从两端比较
来源：http://nnz.kuanghao11.cn

Ruby: s == s.reverse
来源：http://cir.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uyv.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://npn.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://awx.jlsjyb.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xii.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ikd.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://xsw.xziqi.cn

Java: // 手写 HashMap
来源：http://lav.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://vra.daxiang520.top

Ruby: // 手写 Hash
来源：http://jlc.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jyz.52xcode.cn

[N08] 生成全排列
来源：http://qrs.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://pcc.uphjek.com

PHP:  // 手写递归交换
来源：http://qow.yfazqb.com

JS:   // 手写回溯递归
来源：http://kvf.xziqi.cn

TS:   // 手写回溯递归
来源：http://zzx.yonumen.top

Java: // 手写回溯递归
来源：http://mtp.iojbl.cn

Go:   // 手写回溯递归
来源：http://hgh.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://vvp.pycfn.com

C#:   // 手写回溯递归
来源：http://ntv.ehwqpu.com

[N09] 栈与队列
来源：http://ykg.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bci.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nks.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mzp.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gmp.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://naa.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bxb.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://atm.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxv.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://sxo.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cmn.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mus.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sdv.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dqm.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://srd.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ofn.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ioh.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://elc.cheryme.top

[N11] 二叉树中序遍历
来源：http://nms.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nle.cheryme.top

PHP:  // 手写递归函数
来源：http://cpm.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbe.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sda.guowangkeji.top

Java: // 手写递归
来源：http://ygt.ppjwa.cn

Go:   // 手写递归
来源：http://fnt.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zio.gzhubu.top

C#:   // 手写递归
来源：http://ern.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xli.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xki.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zhi.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ezr.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xku.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kdr.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://irr.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nuv.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqk.svipenyu.cn

================================================================================
来源：http://tlk.cucudq.cn

O. 并发与异步
来源：http://pch.guannengcc.top

================================================================================
来源：http://dwv.zycfv.cn

[O01] 启动一个线程
来源：http://kpw.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kdc.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nua.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rtn.yj20258888.top

TS:   // 同 JS
来源：http://sue.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://rud.zycfv.cn

Go:   go f()
来源：http://kxt.ehwqpu.com

Ruby: Thread.new { f }
来源：http://nch.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://non.shanyushiyangtech.top

[O02] 使用线程池
来源：http://uuy.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgm.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://czp.redwolf501.top

JS:   // worker_threads 线程池
来源：http://zps.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://lyw.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://agk.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lhv.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://shy.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gaj.sweek.top

[O03] 加锁保护共享数据
来源：http://grt.yueranfly.top

Py:   with lock: shared += 1
来源：http://dok.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://lgz.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xmk.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://fco.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://qxx.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ojv.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cid.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://gys.fengsongda.top

[O04] 定义异步函数并等待
来源：http://alr.tanke756.top

Py:   async def f():⏎    await g()
来源：http://kbc.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://phr.xuanzx.com

JS:   async function f() { await g(); }
来源：http://wmw.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ran.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sdq.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eni.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://xzx.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://bpr.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://zfm.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://iws.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kzo.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://hrd.tarul.cn

TS:   await Promise.all(tasks)
来源：http://ipv.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dmx.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qlf.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://jzr.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sbg.wangdashe.top

[O06] 使用进程池
来源：http://urp.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eno.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xux.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://auc.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://xdq.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tqp.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqs.yueranfly.top

Ruby: // fork 块
来源：http://vyr.tarul.cn

C#:   Parallel.For
来源：http://xnf.hcnkem.com

================================================================================
来源：http://ofs.kuanghao11.cn

P. 常用工具函数
来源：http://otf.xuetiantiany.cn

================================================================================
来源：http://kkp.cucudq.cn

[P01] 生成 UUID
来源：http://ygb.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://cee.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jwt.nwbrower.top

JS:   crypto.randomUUID()
来源：http://awc.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://vtz.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://xyq.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://uuz.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://usv.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://vts.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://sma.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qod.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kbh.zycfv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lra.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tbw.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://szp.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fym.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uxq.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fmt.52xcode.cn

[P03] 生成短随机字符串
来源：http://vfy.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qpc.xingfuxueyuan.xyz


<!-- 参考信息 -->