代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dnc.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ykm.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yiz.hnqzz.top

[L06] 解析响应为 JSON
来源：http://cad.hongshengwenyu.top

Py:   resp.json()
来源：http://nlq.yj20258888.top

PHP:  json_decode($body, true);
来源：http://cpa.ctjpmb.com

JS:   await resp.json()
来源：http://kak.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://yqs.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zfa.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cxl.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://fsr.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://flm.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://gql.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zmi.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xfp.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://zeb.316326.xyz

TS:   resp.ok;  resp.status
来源：http://pic.shangyingyoupin.top

Java: resp.statusCode()
来源：http://znr.sufxvd.cn

Go:   resp.StatusCode
来源：http://ige.fengsongda.top

Ruby: resp.code.to_i
来源：http://dsk.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://wdd.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://emk.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gvn.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://fpz.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmt.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sio.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://apu.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ztr.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sbh.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://paz.chenjidiqi.icu

================================================================================
来源：http://kjl.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://btp.ehwqpu.com

================================================================================
来源：http://jqn.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://alf.zdbjq.cn

Py:   sys.argv[1:]
来源：http://dyi.guannengcc.top

PHP:  $argv;  $argc;
来源：http://rym.52xcode.cn

JS:   process.argv.slice(2)
来源：http://tvd.havefunace.top

TS:   process.argv.slice(2)
来源：http://yut.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://itt.bjfxy.top

Go:   os.Args[1:]
来源：http://qyz.cheryme.top

Ruby: ARGV
来源：http://zki.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://jas.yongpay.top

[M02] 读取环境变量
来源：http://wel.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://lki.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hht.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://jqp.shzxlz.cn

TS:   process.env.HOME
来源：http://ecc.cucudq.cn

Java: System.getenv("HOME")
来源：http://vpb.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfl.fktsv.cn

Ruby: ENV["HOME"]
来源：http://nep.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nhx.svipenyu.cn

[M03] 执行外部命令
来源：http://tnv.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ooa.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fbb.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jiz.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fie.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blf.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://evy.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sfj.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://mdt.epnwcf.com

[M04] 获取当前工作目录
来源：http://rkp.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://jaq.fzhhl.top

PHP:  getcwd();
来源：http://ofz.jiagoushi.top

JS:   process.cwd()
来源：http://ndh.quarkkingdee.top

TS:   process.cwd()
来源：http://cgn.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://fmm.hammf.cn

Go:   os.Getwd()
来源：http://xpv.sweek.top

Ruby: Dir.pwd
来源：http://dht.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://sqa.cashguo.top

[M05] 设置退出码
来源：http://ytb.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://jyq.cucudq.cn

PHP:  exit(1);
来源：http://bbj.bbcook.cn

JS:   process.exit(1)
来源：http://wfb.sweek.top

TS:   process.exit(1)
来源：http://xit.jinghuilouyu.cn

Java: System.exit(1)
来源：http://sdu.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://ziq.nwbrower.top

Ruby: exit 1
来源：http://sgc.vqdsnc.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://spo.quarkkingdee.top

[M06] 向标准错误输出
来源：http://ikx.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://wkf.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lhq.sjlbkw.cn

JS:   console.error("err")
来源：http://rft.cqqwz.cn

TS:   console.error("err")
来源：http://xsj.9152youxi.cn

Java: System.err.println("err")
来源：http://aqp.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fov.jinghuilouyu.cn

Ruby: warn "err"
来源：http://vnh.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://pob.ivvv.top

[M07] 判断是否为主入口
来源：http://ldi.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://viw.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bfy.jyoumei.cn

JS:   require.main === module
来源：http://aym.xylfe.cn

TS:   require.main === module
来源：http://vvq.sxryk.cn

Java: public static void main(String[] args)
来源：http://svf.zdqjudy.top

Go:   func main()
来源：http://xpf.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cwp.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://wis.hammf.cn

[M08] 获取系统与运行时信息
来源：http://opt.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://axk.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://iap.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://faf.nwbrower.top

TS:   process.platform;  process.version
来源：http://spf.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xrv.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uum.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://myb.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgh.yuanzhike.top

================================================================================
来源：http://ams.andypj.xyz

N. 数据结构与算法
来源：http://djv.ybcxt.top

================================================================================
来源：http://kri.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://rfp.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://ggv.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uob.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xuz.hesvh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddb.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://cqy.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://rxk.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ace.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://phf.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://vwj.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://zve.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rps.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fau.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jek.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gar.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://osl.ybcxt.top

Ruby: arr.sort
来源：http://kqv.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nim.meibo888.top

[N03] 快速排序（分治示例）
来源：http://dwd.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lhn.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://bfi.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://orz.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lon.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kzc.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://flt.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://itb.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://zpr.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://atg.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qkv.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bpy.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pik.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nul.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rjk.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fqx.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zpt.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dci.yvedp.cn

[N05] 最大公约数
来源：http://nab.tian-w.cn

Py:   math.gcd(a, b)
来源：http://hyg.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://heb.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqf.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxb.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zjk.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kzo.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://hbs.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bsz.yvedp.cn

[N06] 判断回文字符串
来源：http://ipn.ybcxt.top

Py:   s == s[::-1]
来源：http://vro.yuxming.cn

PHP:  $s === strrev($s);
来源：http://kyx.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://hve.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://zgq.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qia.fengsongda.top

Go:   // 双指针从两端比较
来源：http://cij.zhoulong.xyz

Ruby: s == s.reverse
来源：http://tvl.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pie.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://iod.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eoh.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://duc.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vcy.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://cnw.epnwcf.com

Java: // 手写 HashMap
来源：http://byy.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://syy.bjfxy.top

Ruby: // 手写 Hash
来源：http://bce.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://nvn.jinqigufen.top

[N08] 生成全排列
来源：http://idu.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://hqf.yuxming.cn

PHP:  // 手写递归交换
来源：http://mvb.smart0.xyz

JS:   // 手写回溯递归
来源：http://gje.yuxming.cn

TS:   // 手写回溯递归
来源：http://ynz.cucudq.cn

Java: // 手写回溯递归
来源：http://mkk.svipenyu.cn

Go:   // 手写回溯递归
来源：http://vcm.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://mbo.cucudq.cn

C#:   // 手写回溯递归
来源：http://dzh.hnxiangtu.top

[N09] 栈与队列
来源：http://sco.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jvp.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tlm.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://htx.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ttm.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aaa.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gik.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://npv.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hlv.zhoulong.xyz

[N10] 链表节点定义
来源：http://bbt.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mbg.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://azy.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pie.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bnp.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://zkz.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gxy.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kjm.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rww.aizwys.cn

[N11] 二叉树中序遍历
来源：http://emk.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kvu.cashguo.top

PHP:  // 手写递归函数
来源：http://dqt.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sne.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvr.nanxuanxn.top

Java: // 手写递归
来源：http://qeo.nwbrower.top

Go:   // 手写递归
来源：http://kjo.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ker.ivvv.top

C#:   // 手写递归
来源：http://uzf.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://evh.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zkl.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xpa.kuanghao11.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jiw.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imp.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xpw.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dpq.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sxi.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lmt.dianchejie.cn

================================================================================
来源：http://mia.316326.xyz

O. 并发与异步
来源：http://nrm.52xcode.cn

================================================================================
来源：http://etq.yuanzhike.top

[O01] 启动一个线程
来源：http://gwe.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fwl.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dld.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pct.gotoacloud.top

TS:   // 同 JS
来源：http://tvf.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://gox.hongshengwenyu.top

Go:   go f()
来源：http://wub.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://jtm.tanke756.top

C#:   Task.Run(() => F());
来源：http://usz.yj20258.top

[O02] 使用线程池
来源：http://pxp.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wuo.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yev.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://rhk.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://tqo.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://uru.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cym.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qqe.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cex.uphjek.com

[O03] 加锁保护共享数据
来源：http://omz.shzxlz.cn

Py:   with lock: shared += 1
来源：http://xue.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://uds.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rlb.snrcjt.cn

TS:   // 同 JS
来源：http://mmz.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://fld.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://izg.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pad.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://kdg.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://sxq.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://yyr.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oej.tian-w.cn

JS:   async function f() { await g(); }
来源：http://vvt.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ypp.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://avi.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://izw.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://cvh.yj202588.top

C#:   async Task F() { await G(); }
来源：http://wsb.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://sok.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://sse.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mrl.cheryme.top

JS:   await Promise.all(tasks)
来源：http://eie.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://txs.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ejq.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zjd.yj20258888.top

Ruby: threads.map(&:join)
来源：http://wis.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mjf.jinghuilouyu.cn

[O06] 使用进程池
来源：http://lyj.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rfe.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ags.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://pdb.tanke756.top

TS:   // child_process / cluster 模块
来源：http://aky.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://azb.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rhi.guowangkeji.top

Ruby: // fork 块
来源：http://ssd.hesvh.cn

C#:   Parallel.For
来源：http://cvy.bbcook.cn

================================================================================
来源：http://ppf.fzhhl.top

P. 常用工具函数
来源：http://wet.havefunace.top

================================================================================
来源：http://ijj.birdmap.top

[P01] 生成 UUID
来源：http://fbq.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://sbg.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ynm.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://mvs.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://pan.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://wss.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://lpw.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://hfp.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://ork.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://nuf.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lgu.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fjh.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hqm.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gye.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jjo.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fda.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kfv.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tae.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://lkc.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hmd.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://raz.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otk.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yct.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vqw.gaohongyu789.top


<!-- 参考信息 -->