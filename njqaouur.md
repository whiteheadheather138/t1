代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bwm.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fwb.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yju.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ryi.hongshengwenyu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pzu.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xfo.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dpd.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://rlt.dashuyun.cn

Py:   resp.json()
来源：http://baj.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://gpb.jinghuilouyu.cn

JS:   await resp.json()
来源：http://rjj.pengpengdd.cyou

TS:   await resp.json()
来源：http://pyi.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://duw.andypj.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uku.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://jha.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tng.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://kzk.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ily.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zen.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://ugj.pycfn.com

TS:   resp.ok;  resp.status
来源：http://hja.wangshuangyany.cn

Java: resp.statusCode()
来源：http://lcq.yangfankeji.com

Go:   resp.StatusCode
来源：http://cxv.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://imx.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://lyf.jqgufenzy.top

[L08] 并发请求多个地址
来源：http://piv.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gvk.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://iqj.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fcs.jqgfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fed.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zmn.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nep.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kev.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wtm.haohaochexian.top

================================================================================
来源：http://bhp.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://nqh.gzhubu.top

================================================================================
来源：http://kix.bjfxy.top

[M01] 读取命令行参数
来源：http://pmc.yj20258.top

Py:   sys.argv[1:]
来源：http://wsv.epnwcf.com

PHP:  $argv;  $argc;
来源：http://imj.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://wwa.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://vde.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://ooa.ywan-chungtsiang.top

Go:   os.Args[1:]
来源：http://hqp.chenzaomai.com

Ruby: ARGV
来源：http://vrc.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://oex.gzhubu.top

[M02] 读取环境变量
来源：http://rwj.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://hor.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lcl.guowangkeji.top

JS:   process.env.HOME
来源：http://udk.jqgufenzy.top

TS:   process.env.HOME
来源：http://vei.ctjpmb.com

Java: System.getenv("HOME")
来源：http://giq.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mno.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://shg.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ngf.c1oappe.top

[M03] 执行外部命令
来源：http://exg.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ker.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ccb.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ejn.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://lzn.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bfg.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rcl.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rrg.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://zej.zdqjudy.top

[M04] 获取当前工作目录
来源：http://rpd.hysaishi.cn

Py:   os.getcwd()
来源：http://swg.aibaodan.cn

PHP:  getcwd();
来源：http://oqp.ybcxt.top

JS:   process.cwd()
来源：http://qjq.52xcode.cn

TS:   process.cwd()
来源：http://vym.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://yjx.uphjek.com

Go:   os.Getwd()
来源：http://hwq.ybcxt.top

Ruby: Dir.pwd
来源：http://smw.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rtk.fanxiaobao.xyz

[M05] 设置退出码
来源：http://ysf.ivvv.top

Py:   sys.exit(1)
来源：http://weh.jianghu66.top

PHP:  exit(1);
来源：http://nah.chenlongwang.top

JS:   process.exit(1)
来源：http://ipg.ivvv.top

TS:   process.exit(1)
来源：http://egu.hammf.cn

Java: System.exit(1)
来源：http://wnh.vehdjk.com

Go:   os.Exit(1)
来源：http://knr.yuxming.cn

Ruby: exit 1
来源：http://hoo.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://htx.bjfxy.top

[M06] 向标准错误输出
来源：http://vli.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://hjt.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dyd.hnxiangtu.top

JS:   console.error("err")
来源：http://jxy.guowangkeji.top

TS:   console.error("err")
来源：http://zuk.ivvv.top

Java: System.err.println("err")
来源：http://njb.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yvd.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://dna.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://lsq.shuidangran.top

[M07] 判断是否为主入口
来源：http://jjo.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://qrh.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ryn.yj20258888.top

JS:   require.main === module
来源：http://mgg.zdqjudy.top

TS:   require.main === module
来源：http://kss.guowangkeji.top

Java: public static void main(String[] args)
来源：http://pfp.jinqigufen.top

Go:   func main()
来源：http://uem.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cei.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://jfs.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://yes.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://nyl.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://sgj.jyoumei.cn

JS:   process.platform;  process.version
来源：http://vof.hywenlv.cn

TS:   process.platform;  process.version
来源：http://jpf.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pht.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nal.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpj.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://chb.fehbvm.com

================================================================================
来源：http://ahk.ivvv.top

N. 数据结构与算法
来源：http://lay.bbcook.cn

================================================================================
来源：http://zsz.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://yud.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uxa.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pmr.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jmw.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mva.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://qfq.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qmx.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jrf.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://wtj.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://xck.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://zdb.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hhh.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://orn.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://rlw.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nem.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://vst.hnqzz.top

Ruby: arr.sort
来源：http://bnz.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pqu.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://zoh.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://smb.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://xto.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://brz.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://npc.yj20258.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rlv.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fgf.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ohc.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://too.cucudq.cn

[N04] 斐波那契数列
来源：http://hic.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xbt.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zlh.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bjb.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctj.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sep.gogol.net.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://itg.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lfz.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://del.jianghu66.top

[N05] 最大公约数
来源：http://rxj.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://tjs.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://syi.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osb.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pev.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://atr.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gnk.gotoacloud.top

Ruby: a.gcd(b)
来源：http://xfn.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://apu.yj20258888.top

[N06] 判断回文字符串
来源：http://xoc.jianghu66.top

Py:   s == s[::-1]
来源：http://pae.yuxming.cn

PHP:  $s === strrev($s);
来源：http://eex.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://giw.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://rig.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://chv.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://wme.cdnleiting.top

Ruby: s == s.reverse
来源：http://swp.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://cuw.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://kog.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://msr.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vvy.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fxd.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://xbi.birdmap.top

Java: // 手写 HashMap
来源：http://uqs.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://jtl.epnwcf.com

Ruby: // 手写 Hash
来源：http://ylx.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://cnd.zhongyouzk.top

[N08] 生成全排列
来源：http://bmq.ivvv.top

Py:   itertools.permutations(arr)
来源：http://eeh.hcnkem.com

PHP:  // 手写递归交换
来源：http://qkf.cqqwz.cn

JS:   // 手写回溯递归
来源：http://nfy.uphjek.com

TS:   // 手写回溯递归
来源：http://wys.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://zyv.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://als.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://syi.sufxvd.cn

C#:   // 手写回溯递归
来源：http://ucm.daxiang520.top

[N09] 栈与队列
来源：http://fve.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yto.tanke756.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mqg.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aeo.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xca.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lxv.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yyu.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://btw.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hrj.chenjidiqi.icu

[N10] 链表节点定义
来源：http://xhx.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hoi.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wqj.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://chl.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pwd.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://iqv.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://ybw.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://udx.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bvi.pycfn.com

[N11] 二叉树中序遍历
来源：http://xbk.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://djt.vehdjk.com

PHP:  // 手写递归函数
来源：http://ezv.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://voq.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pot.yongpay.top

Java: // 手写递归
来源：http://yyu.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://jdl.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cky.ehwqpu.com

C#:   // 手写递归
来源：http://xtv.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ziy.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yit.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bgq.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hpo.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oie.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vul.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zxi.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ufl.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gbi.wangshuangyany.cn

================================================================================
来源：http://kqh.sxryk.cn

O. 并发与异步
来源：http://ywg.zdqjudy.top

================================================================================
来源：http://hcp.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://hre.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qvq.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dch.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nsp.yueranfly.top

TS:   // 同 JS
来源：http://qrr.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://efg.yj20258888.top

Go:   go f()
来源：http://kkp.daria6918.cn

Ruby: Thread.new { f }
来源：http://nsh.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://chu.haohaochexian.top

[O02] 使用线程池
来源：http://oqn.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uwb.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wyc.ivvv.top

JS:   // worker_threads 线程池
来源：http://xoe.fzhhl.top

TS:   // worker_threads 线程池
来源：http://ikw.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xxk.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yfb.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zbn.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xnj.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://otg.cdnleiting.top

Py:   with lock: shared += 1
来源：http://ddw.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://jqt.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zlc.hammf.cn

TS:   // 同 JS
来源：http://pdr.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://cax.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwu.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jvq.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://mdk.c1oappe.top

[O04] 定义异步函数并等待
来源：http://mmv.316326.xyz

Py:   async def f():⏎    await g()
来源：http://pch.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://amm.hcnkem.com

JS:   async function f() { await g(); }
来源：http://snq.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oxa.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://znc.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pwk.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://fqs.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://mkf.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://bns.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://dut.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mui.yonumen.top

JS:   await Promise.all(tasks)
来源：http://jgl.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://ygu.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iij.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fcb.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://eao.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dri.daria6918.cn

[O06] 使用进程池
来源：http://hwf.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pmp.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://yzh.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://fbd.uphjek.com

TS:   // child_process / cluster 模块
来源：http://abp.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mii.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rvt.zhiwuduotai.top

Ruby: // fork 块
来源：http://oob.tarul.cn

C#:   Parallel.For
来源：http://ovc.jqgufenzy.top

================================================================================
来源：http://uhf.chenjidiqi.icu

P. 常用工具函数
来源：http://lcm.jinqigufen.top

================================================================================
来源：http://iij.yonumen.top

[P01] 生成 UUID
来源：http://slz.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://kmo.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvq.cucudq.cn

JS:   crypto.randomUUID()
来源：http://lel.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://zmz.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://wod.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://qny.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://hpu.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://opv.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://gnj.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ahw.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fwi.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bev.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hjr.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gzo.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bpc.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mnd.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cus.jinqigufen.top

[P03] 生成短随机字符串
来源：http://kpv.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://okp.dianchejie.cn


<!-- 参考信息 -->