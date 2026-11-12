代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nmq.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qol.jlsjyb.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ien.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aha.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lkd.hnqzz.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nen.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kes.sysykeji.top

[L06] 解析响应为 JSON
来源：http://nec.gzhubu.top

Py:   resp.json()
来源：http://nqu.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://xsx.pengpengdd.cyou

JS:   await resp.json()
来源：http://uqm.cashguo.top

TS:   await resp.json()
来源：http://xxo.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://azj.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://frt.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://hov.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ifg.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://kgv.yvedp.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ewn.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hsz.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://cug.haohaochexian.top

TS:   resp.ok;  resp.status
来源：http://kji.hnxiangtu.top

Java: resp.statusCode()
来源：http://snd.haohaochexian.top

Go:   resp.StatusCode
来源：http://sfe.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://mro.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://mey.nwbrower.top

[L08] 并发请求多个地址
来源：http://dyc.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mxe.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://uuv.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ktw.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zme.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fox.zycfv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aju.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://myi.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qih.quarkkingdee.top

================================================================================
来源：http://mag.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://qzl.yvedp.cn

================================================================================
来源：http://qqy.jyoumei.cn

[M01] 读取命令行参数
来源：http://kzm.aizwys.cn

Py:   sys.argv[1:]
来源：http://shx.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://zbd.cheryme.top

JS:   process.argv.slice(2)
来源：http://ssy.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://uaj.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://vsy.daxiang520.top

Go:   os.Args[1:]
来源：http://jjy.andypj.xyz

Ruby: ARGV
来源：http://ics.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://amn.hesvh.cn

[M02] 读取环境变量
来源：http://cct.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://jek.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okk.mhx1999.top

JS:   process.env.HOME
来源：http://nmq.yongpay.top

TS:   process.env.HOME
来源：http://hkc.meibo888.top

Java: System.getenv("HOME")
来源：http://syt.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://koi.xuanzx.com

Ruby: ENV["HOME"]
来源：http://sth.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wke.bjfxy.top

[M03] 执行外部命令
来源：http://qah.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wrn.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cgy.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qyh.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pfn.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gbb.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kys.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://uoz.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://rsu.gogol.net.cn

[M04] 获取当前工作目录
来源：http://fzo.guannengcc.top

Py:   os.getcwd()
来源：http://lhv.xuanzx.com

PHP:  getcwd();
来源：http://han.dashuyun.cn

JS:   process.cwd()
来源：http://vdg.hywenlv.cn

TS:   process.cwd()
来源：http://lsr.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://xvn.uphjek.com

Go:   os.Getwd()
来源：http://ubk.hywenlv.cn

Ruby: Dir.pwd
来源：http://lst.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://tfo.zhiwuduotai.top

[M05] 设置退出码
来源：http://xnw.haohaochexian.top

Py:   sys.exit(1)
来源：http://twp.redwolf501.top

PHP:  exit(1);
来源：http://snn.xuanzx.com

JS:   process.exit(1)
来源：http://rel.ppjwa.cn

TS:   process.exit(1)
来源：http://lhd.xziqi.cn

Java: System.exit(1)
来源：http://rot.hammf.cn

Go:   os.Exit(1)
来源：http://emz.cashguo.top

Ruby: exit 1
来源：http://ppe.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zdv.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://jpu.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://iyw.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://iqp.gotoacloud.top

JS:   console.error("err")
来源：http://uwj.xinyue.icu

TS:   console.error("err")
来源：http://qen.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://aek.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sjl.fktsv.cn

Ruby: warn "err"
来源：http://uix.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://eya.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://yyw.meibo888.top

Py:   if __name__ == "__main__":
来源：http://vmm.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qwo.dashuyun.cn

JS:   require.main === module
来源：http://vtn.andypj.xyz

TS:   require.main === module
来源：http://vni.redwolf501.top

Java: public static void main(String[] args)
来源：http://fih.bjfxy.top

Go:   func main()
来源：http://ioj.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wwn.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://rux.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://ayp.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://eeu.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://zts.zdbjq.cn

JS:   process.platform;  process.version
来源：http://qfk.hywenlv.cn

TS:   process.platform;  process.version
来源：http://nlq.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://opw.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ctf.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zkr.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://tea.hnqzz.top

================================================================================
来源：http://vbx.birdmap.top

N. 数据结构与算法
来源：http://rqi.shanyushiyangkeji.top

================================================================================
来源：http://uwh.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://lep.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://oux.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://idu.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kql.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yvm.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://whl.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://jsx.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ynv.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://cec.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://iyl.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://zno.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zdm.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zwb.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zjs.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nuv.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://mle.mhx1999.top

Ruby: arr.sort
来源：http://voo.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cyl.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://wxb.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rcc.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://xlg.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://muo.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mtn.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vhc.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://joa.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zgh.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://ckh.fengsongda.top

[N04] 斐波那契数列
来源：http://eyc.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zfj.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qie.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqx.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fud.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mmf.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://amg.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eph.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://muk.xziqi.cn

[N05] 最大公约数
来源：http://bxl.mhx1999.top

Py:   math.gcd(a, b)
来源：http://vry.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cdy.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hlb.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kkj.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qim.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hui.cashguo.top

Ruby: a.gcd(b)
来源：http://grl.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ste.vehdjk.com

[N06] 判断回文字符串
来源：http://alr.xuanzx.com

Py:   s == s[::-1]
来源：http://kzd.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://kyc.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://dgf.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://gci.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aag.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://gjb.cucudq.cn

Ruby: s == s.reverse
来源：http://eic.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yrc.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://qct.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ehz.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qkr.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zqy.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://ncc.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://nvy.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://gzb.zycfv.cn

Ruby: // 手写 Hash
来源：http://efy.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://lgf.zdqjudy.top

[N08] 生成全排列
来源：http://hog.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://nrk.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://ihu.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://brx.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://cbz.gotoacloud.top

Java: // 手写回溯递归
来源：http://teh.shzxlz.cn

Go:   // 手写回溯递归
来源：http://dtp.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://rly.yj20258888.top

C#:   // 手写回溯递归
来源：http://crf.zdqjudy.top

[N09] 栈与队列
来源：http://xdp.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ann.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wai.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hth.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://obg.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yxi.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mnd.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wks.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kvs.ctjpmb.com

[N10] 链表节点定义
来源：http://ryo.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pua.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eld.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yov.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kjm.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://dmb.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lyc.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nkz.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ipp.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://abq.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hbz.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://zsk.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tog.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rda.jinqigfzy.top

Java: // 手写递归
来源：http://atf.zhoulong.xyz

Go:   // 手写递归
来源：http://byg.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nfb.zhongyouzk.top

C#:   // 手写递归
来源：http://nvj.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wor.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jcc.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ofv.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gpn.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jfd.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blh.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tic.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bsn.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://veq.gzhubu.top

================================================================================
来源：http://idg.jinqigfzy.top

O. 并发与异步
来源：http://xbt.jyoumei.cn

================================================================================
来源：http://gvl.yj202588.top

[O01] 启动一个线程
来源：http://xqw.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://crm.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cap.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qtp.tian-w.cn

TS:   // 同 JS
来源：http://tiq.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://yyv.jinqigufen.top

Go:   go f()
来源：http://rpn.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://jkm.daria6918.cn

C#:   Task.Run(() => F());
来源：http://hae.yvedp.cn

[O02] 使用线程池
来源：http://ozp.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nvh.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mhg.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://wmu.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://idw.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://mkz.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dne.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gox.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gwb.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://tov.daxiang520.top

Py:   with lock: shared += 1
来源：http://qxr.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://tto.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://voy.meibo888.top

TS:   // 同 JS
来源：http://qxq.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://ecb.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ztl.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jtd.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://hjf.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://puy.havefunace.top

Py:   async def f():⏎    await g()
来源：http://hxh.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibg.mhx1999.top

JS:   async function f() { await g(); }
来源：http://you.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mwe.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oas.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gea.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ogj.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://taw.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://odd.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://bqh.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yhm.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://kfr.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://vla.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xse.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rzx.yfazqb.com

Ruby: threads.map(&:join)
来源：http://kll.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://awd.aizwys.cn

[O06] 使用进程池
来源：http://xll.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oph.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yoz.birdmap.top

JS:   // child_process / cluster 模块
来源：http://epy.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://jfe.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbv.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tmy.sufxvd.cn

Ruby: // fork 块
来源：http://ind.dashuyun.cn

C#:   Parallel.For
来源：http://nxx.hfpthk.cn

================================================================================
来源：http://pbs.guowangkeji.top

P. 常用工具函数
来源：http://qbd.pengpengdd.cyou

================================================================================
来源：http://vjk.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://lgx.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://bzc.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://thd.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://jjk.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://csb.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://bty.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://hki.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://pab.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://etk.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://tht.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vxx.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://rxr.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aox.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rht.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hpa.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ojk.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xry.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nao.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://hqv.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pmw.feifeiyinyue.top


<!-- 参考信息 -->