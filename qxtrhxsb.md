代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gir.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bnz.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kkk.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://twf.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lqk.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ovq.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gqb.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://hxz.hnxiangtu.top

Py:   resp.json()
来源：http://opq.ybcxt.top

PHP:  json_decode($body, true);
来源：http://eqs.nwbrower.top

JS:   await resp.json()
来源：http://bdk.daxiang520.top

TS:   await resp.json()
来源：http://azw.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ond.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://six.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://lbt.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://guz.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://sbq.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vro.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://juc.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://dpf.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://wnp.shzxlz.cn

Java: resp.statusCode()
来源：http://xhs.hesvh.cn

Go:   resp.StatusCode
来源：http://zqe.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://xyz.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://rjy.yfazqb.com

[L08] 并发请求多个地址
来源：http://sqg.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eml.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://lpz.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jdj.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dot.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://swd.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lrm.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nuy.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ujy.yuanzhike.top

================================================================================
来源：http://kll.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://adl.fengsongda.top

================================================================================
来源：http://sfo.xylfe.cn

[M01] 读取命令行参数
来源：http://hpc.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://ndm.yueranfly.top

PHP:  $argv;  $argc;
来源：http://pkn.yonumen.top

JS:   process.argv.slice(2)
来源：http://qsp.tanke756.top

TS:   process.argv.slice(2)
来源：http://wxd.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://ubt.gaohongyu789.top

Go:   os.Args[1:]
来源：http://amv.jinqigufen.top

Ruby: ARGV
来源：http://upq.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://mwf.sufxvd.cn

[M02] 读取环境变量
来源：http://lrv.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://una.ctjpmb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xwi.xuanzx.com

JS:   process.env.HOME
来源：http://yhb.c1oappe.top

TS:   process.env.HOME
来源：http://jwg.gotoacloud.top

Java: System.getenv("HOME")
来源：http://sit.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ecj.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://arr.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mzw.cdnleiting.top

[M03] 执行外部命令
来源：http://mtu.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://utx.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://end.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fno.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ccq.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kua.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qlh.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ima.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://rcd.jiagoushi.top

[M04] 获取当前工作目录
来源：http://wbd.cdnleiting.top

Py:   os.getcwd()
来源：http://pxw.gogol.net.cn

PHP:  getcwd();
来源：http://cuf.zhixingplan.top

JS:   process.cwd()
来源：http://dek.hcnkem.com

TS:   process.cwd()
来源：http://cxy.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://cos.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://bsa.jianghu66.top

Ruby: Dir.pwd
来源：http://bol.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zgo.yj202588.top

[M05] 设置退出码
来源：http://cfw.ehwqpu.com

Py:   sys.exit(1)
来源：http://mmk.xuetiantiany.cn

PHP:  exit(1);
来源：http://ojn.nanxuanxn.top

JS:   process.exit(1)
来源：http://dwx.hfpthk.cn

TS:   process.exit(1)
来源：http://uuy.jqgufenzy.top

Java: System.exit(1)
来源：http://adn.gzhubu.top

Go:   os.Exit(1)
来源：http://fzo.pengpengdd.cyou

Ruby: exit 1
来源：http://zyu.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://etn.dianchejie.cn

[M06] 向标准错误输出
来源：http://ggi.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://wmk.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nzp.shangyingyoupin.top

JS:   console.error("err")
来源：http://tdm.feifeiyinyue.top

TS:   console.error("err")
来源：http://xtz.zhongyouzk.top

Java: System.err.println("err")
来源：http://pve.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hcy.jinghuilouyu.cn

Ruby: warn "err"
来源：http://lxx.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://bra.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://kga.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://kma.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ghq.yanxiufei.cn

JS:   require.main === module
来源：http://zkl.zhaomingkeji.xyz

TS:   require.main === module
来源：http://ijm.smart0.xyz

Java: public static void main(String[] args)
来源：http://rmk.hywenlv.cn

Go:   func main()
来源：http://hie.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bzl.shuidangran.top

C#:   static void Main(string[] args)
来源：http://dwl.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://emu.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://ktd.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://fxy.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://rmg.zdbjq.cn

TS:   process.platform;  process.version
来源：http://xkt.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wym.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://epd.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dnu.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://xcu.9152youxi.cn

================================================================================
来源：http://kpl.fengsongda.top

N. 数据结构与算法
来源：http://dsj.yongpay.top

================================================================================
来源：http://xlv.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://vad.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://opo.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zlb.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kil.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksu.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vlp.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://rlw.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://prl.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vhn.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://kmd.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://tvz.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://orn.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dro.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vrw.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dpj.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://qek.sweek.top

Ruby: arr.sort
来源：http://pbb.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cqb.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://alq.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wtf.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://vvh.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxv.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyw.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dpj.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bpy.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://svu.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zuw.yonumen.top

[N04] 斐波那契数列
来源：http://ekg.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lsb.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cou.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://llv.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pnc.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ehq.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sjq.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tty.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gbf.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://ppa.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://dbe.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqt.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://toa.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iab.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bak.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tkt.aibaodan.cn

Ruby: a.gcd(b)
来源：http://rmh.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uah.chenlongwang.top

[N06] 判断回文字符串
来源：http://vma.pycfn.com

Py:   s == s[::-1]
来源：http://reu.xylfe.cn

PHP:  $s === strrev($s);
来源：http://mfg.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://ggo.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://pqh.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ark.yfazqb.com

Go:   // 双指针从两端比较
来源：http://yem.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://too.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxp.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://upw.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kqd.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ygj.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hve.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://emz.fehbvm.com

Java: // 手写 HashMap
来源：http://btr.meibo888.top

Go:   // 手写 map[int]int
来源：http://gsa.zhixingplan.top

Ruby: // 手写 Hash
来源：http://mwh.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://zut.fengsongda.top

[N08] 生成全排列
来源：http://hsv.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://kyj.jinqigufen.top

PHP:  // 手写递归交换
来源：http://ffh.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://ilj.bjfxy.top

TS:   // 手写回溯递归
来源：http://dfr.yonumen.top

Java: // 手写回溯递归
来源：http://jfl.andypj.xyz

Go:   // 手写回溯递归
来源：http://lsp.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://mtj.jqgfzy.top

C#:   // 手写回溯递归
来源：http://ucm.yj20258.top

[N09] 栈与队列
来源：http://awq.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oqd.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ozb.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://shh.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qyp.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fdq.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pnb.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://izb.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://emd.yangfankeji.com

[N10] 链表节点定义
来源：http://dmz.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ypk.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sys.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tpx.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dts.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://xyp.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://trc.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://uft.zhiwuduotai.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ylj.bjfxy.top

[N11] 二叉树中序遍历
来源：http://mne.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gkv.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://nye.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byf.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://trb.pycfn.com

Java: // 手写递归
来源：http://nss.cqqwz.cn

Go:   // 手写递归
来源：http://zpr.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bgi.jyoumei.cn

C#:   // 手写递归
来源：http://yyk.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hnf.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://giv.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uto.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnj.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://viu.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sew.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://idl.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://czm.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gxx.hnxiangtu.top

================================================================================
来源：http://hxw.xylfe.cn

O. 并发与异步
来源：http://hwf.dianchejie.cn

================================================================================
来源：http://yfi.bjfxy.top

[O01] 启动一个线程
来源：http://pbc.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jxk.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wop.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://esw.andypj.xyz

TS:   // 同 JS
来源：http://ksg.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://txc.hywenlv.cn

Go:   go f()
来源：http://fvo.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://vjl.ivvv.top

C#:   Task.Run(() => F());
来源：http://xgf.yfazqb.com

[O02] 使用线程池
来源：http://ekk.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tps.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vej.fzhhl.top

JS:   // worker_threads 线程池
来源：http://svz.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://xfk.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tpg.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ece.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bbg.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fdu.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://efh.meibo888.top

Py:   with lock: shared += 1
来源：http://rdk.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://ori.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://egl.haohaochexian.top

TS:   // 同 JS
来源：http://rbb.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://iad.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://umz.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qjj.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://xcy.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://zzb.yj202588.top

Py:   async def f():⏎    await g()
来源：http://zzn.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yeg.hcnkem.com

JS:   async function f() { await g(); }
来源：http://ylf.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://prq.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qak.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aka.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qku.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://iiw.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://nkd.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://vzd.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jbh.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://fuf.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://abz.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://luw.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uer.pycfn.com

Ruby: threads.map(&:join)
来源：http://zsg.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pxa.andypj.xyz

[O06] 使用进程池
来源：http://nyu.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hzh.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zrg.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://ets.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://nlb.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tpg.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lik.cucudq.cn

Ruby: // fork 块
来源：http://gkc.tanke756.top

C#:   Parallel.For
来源：http://kwh.yuxming.cn

================================================================================
来源：http://ruf.vqdsnc.cn

P. 常用工具函数
来源：http://vui.hammf.cn

================================================================================
来源：http://fax.pycfn.com

[P01] 生成 UUID
来源：http://oer.yonumen.top

Py:   str(uuid.uuid4())
来源：http://qhj.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wao.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://wgv.c1oappe.top

TS:   crypto.randomUUID()
来源：http://znm.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://mke.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://qoc.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://vco.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://lwq.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://sve.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jhv.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hce.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aqt.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oqx.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ona.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bco.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ved.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bsr.gogol.net.cn

[P03] 生成短随机字符串
来源：http://zza.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gjx.zhixingplan.top


<!-- 参考信息 -->