代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hwu.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vkm.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yze.zhixingplan.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://enh.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vje.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ujy.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tid.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://xhx.vehdjk.com

Py:   resp.json()
来源：http://gzp.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://bhg.zdqjudy.top

JS:   await resp.json()
来源：http://nvp.snrcjt.cn

TS:   await resp.json()
来源：http://jhn.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mta.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nzm.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://axb.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://laa.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://mof.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ikf.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ekh.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://vqx.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://zyy.havefunace.top

Java: resp.statusCode()
来源：http://oaz.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://doa.yonumen.top

Ruby: resp.code.to_i
来源：http://det.yonumen.top

C#:   (int)resp.StatusCode
来源：http://wkn.uphjek.com

[L08] 并发请求多个地址
来源：http://cvp.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tcb.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://krc.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://msn.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkc.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rvz.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fws.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://slm.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vyd.snrcjt.cn

================================================================================
来源：http://jke.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://hwz.tarul.cn

================================================================================
来源：http://qmw.hfpthk.cn

[M01] 读取命令行参数
来源：http://avl.cdnleiting.top

Py:   sys.argv[1:]
来源：http://hrq.pycfn.com

PHP:  $argv;  $argc;
来源：http://mhn.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://yav.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://qqz.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://zzy.daxiang520.top

Go:   os.Args[1:]
来源：http://uvc.gotoacloud.top

Ruby: ARGV
来源：http://rig.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://tsb.feifeiyinyue.top

[M02] 读取环境变量
来源：http://fqm.pycfn.com

Py:   os.environ.get("HOME")
来源：http://toz.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wgg.vqdsnc.cn

JS:   process.env.HOME
来源：http://pld.52xcode.cn

TS:   process.env.HOME
来源：http://vau.yfazqb.com

Java: System.getenv("HOME")
来源：http://ejj.xziqi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ypg.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://tzi.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oty.gzhubu.top

[M03] 执行外部命令
来源：http://kqd.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://udn.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jjw.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bpa.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pso.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iec.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://osp.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://iym.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://vmf.xylfe.cn

[M04] 获取当前工作目录
来源：http://lqe.sweek.top

Py:   os.getcwd()
来源：http://myv.epnwcf.com

PHP:  getcwd();
来源：http://jwz.pengpengdd.cyou

JS:   process.cwd()
来源：http://lcr.cucudq.cn

TS:   process.cwd()
来源：http://omv.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://uzm.yuxming.cn

Go:   os.Getwd()
来源：http://bwp.yonumen.top

Ruby: Dir.pwd
来源：http://suq.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://jpo.yuxming.cn

[M05] 设置退出码
来源：http://dhn.xuanzx.com

Py:   sys.exit(1)
来源：http://ghd.cashguo.top

PHP:  exit(1);
来源：http://iez.ydzc1.top

JS:   process.exit(1)
来源：http://axb.nwbrower.top

TS:   process.exit(1)
来源：http://xhf.chenlongwang.top

Java: System.exit(1)
来源：http://lyu.fktsv.cn

Go:   os.Exit(1)
来源：http://jyr.svipenyu.cn

Ruby: exit 1
来源：http://eck.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://obn.nwbrower.top

[M06] 向标准错误输出
来源：http://miw.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://vku.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tqo.yuanzhike.top

JS:   console.error("err")
来源：http://nih.tian-w.cn

TS:   console.error("err")
来源：http://eli.vqdsnc.cn

Java: System.err.println("err")
来源：http://tcy.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kwa.ybcxt.top

Ruby: warn "err"
来源：http://qde.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://nvd.smart0.xyz

[M07] 判断是否为主入口
来源：http://cis.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://xbk.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xvr.mhx1999.top

JS:   require.main === module
来源：http://hdz.feifeiyinyue.top

TS:   require.main === module
来源：http://dyb.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://hqk.svipenyu.cn

Go:   func main()
来源：http://ism.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lgl.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://fyp.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://byh.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://ihf.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://tra.ctjpmb.com

JS:   process.platform;  process.version
来源：http://voy.shzxlz.cn

TS:   process.platform;  process.version
来源：http://emt.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xvn.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wee.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nke.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fyl.gotoacloud.top

================================================================================
来源：http://euk.hcnkem.com

N. 数据结构与算法
来源：http://uxr.9152youxi.cn

================================================================================
来源：http://zdf.yongpay.top

[N01] 二分查找（有序数组）
来源：http://kyx.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uby.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vmi.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvs.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhc.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uqe.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://fnd.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sqo.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uhy.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://hia.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://ywb.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wqj.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ipe.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://msf.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qmt.yj20258.top

Go:   slices.Sort(arr)
来源：http://bvs.aizwys.cn

Ruby: arr.sort
来源：http://vos.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://whu.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://hyx.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://egk.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://jmt.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gju.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bpp.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qru.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dgq.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jpk.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://bin.yvedp.cn

[N04] 斐波那契数列
来源：http://tev.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://trm.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hzz.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ksi.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nuz.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ufm.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bba.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://acu.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uvu.pycfn.com

[N05] 最大公约数
来源：http://stj.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://vbl.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dlo.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wtr.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jsi.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vol.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vfx.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://zsv.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhw.jinqigufen.top

[N06] 判断回文字符串
来源：http://xxi.sysykeji.top

Py:   s == s[::-1]
来源：http://ksz.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://vwu.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://xhk.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://kdi.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://par.daxiang520.top

Go:   // 双指针从两端比较
来源：http://gel.aizwys.cn

Ruby: s == s.reverse
来源：http://rkg.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wwj.hammf.cn

[N07] 两数之和（返回下标）
来源：http://tsk.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rzk.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://slr.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://slj.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://eal.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://dgd.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://jbz.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://ast.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hve.zdqjudy.top

[N08] 生成全排列
来源：http://rak.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://bwc.ctjpmb.com

PHP:  // 手写递归交换
来源：http://lza.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://wnc.redwolf501.top

TS:   // 手写回溯递归
来源：http://ncu.hnxiangtu.top

Java: // 手写回溯递归
来源：http://fys.iojbl.cn

Go:   // 手写回溯递归
来源：http://pzw.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://djt.yueranfly.top

C#:   // 手写回溯递归
来源：http://xmk.cucudq.cn

[N09] 栈与队列
来源：http://wvx.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cce.wangdashe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lre.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kfg.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://anx.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aoq.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xbo.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eku.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uwp.yongpay.top

[N10] 链表节点定义
来源：http://uws.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yur.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kmv.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qzo.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apm.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://nqh.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://xpt.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zmv.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vki.daria6918.cn

[N11] 二叉树中序遍历
来源：http://nfa.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mmq.52xcode.cn

PHP:  // 手写递归函数
来源：http://qil.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frp.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xru.yfazqb.com

Java: // 手写递归
来源：http://ktl.gotoacloud.top

Go:   // 手写递归
来源：http://cyk.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fao.cdnleiting.top

C#:   // 手写递归
来源：http://hts.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tdp.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jox.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nol.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://var.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pkh.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zyi.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbc.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zwh.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://byv.chenzaomai.com

================================================================================
来源：http://gvr.tian-w.cn

O. 并发与异步
来源：http://rzk.316326.xyz

================================================================================
来源：http://mrg.birdmap.top

[O01] 启动一个线程
来源：http://zet.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pki.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://neh.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zhs.nwbrower.top

TS:   // 同 JS
来源：http://sry.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://jil.zhoulong.xyz

Go:   go f()
来源：http://gqi.svipenyu.cn

Ruby: Thread.new { f }
来源：http://hgd.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ilc.snrcjt.cn

[O02] 使用线程池
来源：http://cvm.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dks.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://abe.cucudq.cn

JS:   // worker_threads 线程池
来源：http://dfp.cashguo.top

TS:   // worker_threads 线程池
来源：http://jzz.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hhp.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sak.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xtf.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://maz.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://vlm.zdqjudy.top

Py:   with lock: shared += 1
来源：http://vha.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://hbu.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fse.zhongyouzk.top

TS:   // 同 JS
来源：http://mbq.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://egx.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pxb.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cwc.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://vfz.fengsongda.top

[O04] 定义异步函数并等待
来源：http://koo.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://ngr.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://upy.smart0.xyz

JS:   async function f() { await g(); }
来源：http://cuj.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ggm.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nnq.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rtu.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://ucg.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://dxq.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://vzl.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://jvn.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rlm.cheryme.top

JS:   await Promise.all(tasks)
来源：http://asd.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://mue.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://upj.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fyj.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://vjv.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qss.xziqi.cn

[O06] 使用进程池
来源：http://ihe.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tfc.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ihq.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://osf.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://inl.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nal.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ugi.yanxiufei.cn

Ruby: // fork 块
来源：http://taw.guannengcc.top

C#:   Parallel.For
来源：http://hnr.hammf.cn

================================================================================
来源：http://qyg.aizwys.cn

P. 常用工具函数
来源：http://vur.hysaishi.cn

================================================================================
来源：http://cey.gaohongyu789.top

[P01] 生成 UUID
来源：http://mtc.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://oou.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ygi.hywenlv.cn

JS:   crypto.randomUUID()
来源：http://tqo.sysykeji.top

TS:   crypto.randomUUID()
来源：http://ttc.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://rkj.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://elm.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://zbr.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://bpx.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://wpv.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xae.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cjl.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://scc.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jzf.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iko.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://trm.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://itb.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cml.shuidangran.top

[P03] 生成短随机字符串
来源：http://qvb.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wrj.daria6918.cn


<!-- 参考信息 -->