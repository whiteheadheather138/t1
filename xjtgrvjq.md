代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xfq.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ebx.bbcook.cn

[L05] 上传文件（multipart）
来源：http://yhw.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iiu.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://phc.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eci.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qkh.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ide.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://itw.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zob.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wbe.yfazqb.com

[L06] 解析响应为 JSON
来源：http://xjj.svipenyu.cn

Py:   resp.json()
来源：http://fdn.fengsongda.top

PHP:  json_decode($body, true);
来源：http://oar.cashguo.top

JS:   await resp.json()
来源：http://mht.bjfxy.top

TS:   await resp.json()
来源：http://jce.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vcx.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ban.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://okz.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bat.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://vac.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aem.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ryh.tanke756.top

JS:   resp.ok;  resp.status
来源：http://est.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://qtp.yuxming.cn

Java: resp.statusCode()
来源：http://rjj.fehbvm.com

Go:   resp.StatusCode
来源：http://xms.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://ntb.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://cov.vqdsnc.cn

[L08] 并发请求多个地址
来源：http://xcs.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://htu.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://xfu.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgw.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xmm.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utt.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lbr.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jmm.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nsi.yj20258.top

================================================================================
来源：http://ujs.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://tod.yuxming.cn

================================================================================
来源：http://ihn.cdnleiting.top

[M01] 读取命令行参数
来源：http://fxn.bjfxy.top

Py:   sys.argv[1:]
来源：http://xao.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://ats.ydzc1.top

JS:   process.argv.slice(2)
来源：http://yup.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://awh.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://qay.tanke756.top

Go:   os.Args[1:]
来源：http://boz.dianchejie.cn

Ruby: ARGV
来源：http://xne.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://mnd.xuanzx.com

[M02] 读取环境变量
来源：http://hkc.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://zcq.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ybz.ppjwa.cn

JS:   process.env.HOME
来源：http://pvu.hnqzz.top

TS:   process.env.HOME
来源：http://mvg.c1oappe.top

Java: System.getenv("HOME")
来源：http://qsn.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://svs.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://yeu.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dde.vehdjk.com

[M03] 执行外部命令
来源：http://xjl.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pqn.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pgl.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zhw.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://isp.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dyb.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mmn.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://kll.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://rrw.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://mqd.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://ruj.hnqzz.top

PHP:  getcwd();
来源：http://rll.cdnleiting.top

JS:   process.cwd()
来源：http://ofp.zhengqikj.top

TS:   process.cwd()
来源：http://ssf.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://jgq.jyoumei.cn

Go:   os.Getwd()
来源：http://slx.nwbrower.top

Ruby: Dir.pwd
来源：http://kqa.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://fyh.ivvv.top

[M05] 设置退出码
来源：http://csf.shuidangran.top

Py:   sys.exit(1)
来源：http://rol.svipenyu.cn

PHP:  exit(1);
来源：http://ycg.hnxiangtu.top

JS:   process.exit(1)
来源：http://gvy.xuanzx.com

TS:   process.exit(1)
来源：http://czt.sxryk.cn

Java: System.exit(1)
来源：http://vbt.tarul.cn

Go:   os.Exit(1)
来源：http://oyt.gotoacloud.top

Ruby: exit 1
来源：http://aou.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fqy.kuanghao11.cn

[M06] 向标准错误输出
来源：http://fzq.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://qcv.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jrn.nanxuanxn.top

JS:   console.error("err")
来源：http://vgm.xinyue.icu

TS:   console.error("err")
来源：http://uya.zhoulong.xyz

Java: System.err.println("err")
来源：http://jls.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nqg.yangfankeji.com

Ruby: warn "err"
来源：http://nkh.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://vtf.redwolf501.top

[M07] 判断是否为主入口
来源：http://nlh.birdmap.top

Py:   if __name__ == "__main__":
来源：http://xxn.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://spo.zhijiandao.cn

JS:   require.main === module
来源：http://alc.yuxming.cn

TS:   require.main === module
来源：http://hrm.meibo888.top

Java: public static void main(String[] args)
来源：http://ren.9152youxi.cn

Go:   func main()
来源：http://xkf.havefunace.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://maa.daria6918.cn

C#:   static void Main(string[] args)
来源：http://bep.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://zxx.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://azo.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://bcl.hysaishi.cn

JS:   process.platform;  process.version
来源：http://stw.ydzc1.top

TS:   process.platform;  process.version
来源：http://vca.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://swm.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ngy.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rfi.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cqb.chenjidiqi.icu

================================================================================
来源：http://pwt.daria6918.cn

N. 数据结构与算法
来源：http://dbm.hfpthk.cn

================================================================================
来源：http://igj.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://bli.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://kkd.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qje.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsy.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://phq.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://bgi.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://rng.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wzi.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://awr.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://lma.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://clo.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wkw.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nxw.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kxd.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lax.guannengcc.top

Go:   slices.Sort(arr)
来源：http://dqd.chenzaomai.com

Ruby: arr.sort
来源：http://sji.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mmk.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://pgm.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rnk.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://rjo.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tmk.chenlongwang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aby.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://asa.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eoc.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://myn.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://rtb.zhijiandao.cn

[N04] 斐波那契数列
来源：http://waw.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gfr.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lpu.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tbg.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iza.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://upk.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://onf.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kao.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpz.52xcode.cn

[N05] 最大公约数
来源：http://izc.hammf.cn

Py:   math.gcd(a, b)
来源：http://vff.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cso.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ahi.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lah.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cfd.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nzh.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://dct.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blh.zhoulong.xyz

[N06] 判断回文字符串
来源：http://hjg.ybcxt.top

Py:   s == s[::-1]
来源：http://sei.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://mkq.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://tqa.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://hfb.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://osj.sweek.top

Go:   // 双指针从两端比较
来源：http://vvy.yonumen.top

Ruby: s == s.reverse
来源：http://tem.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxv.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://pwy.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oso.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ale.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kot.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://uml.smart0.xyz

Java: // 手写 HashMap
来源：http://xlw.sysykeji.top

Go:   // 手写 map[int]int
来源：http://xgu.gotoacloud.top

Ruby: // 手写 Hash
来源：http://ujg.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://cir.vehdjk.com

[N08] 生成全排列
来源：http://hck.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://dpz.daxiang520.top

PHP:  // 手写递归交换
来源：http://hao.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://etw.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://wtc.gaohongyu789.top

Java: // 手写回溯递归
来源：http://lui.jianghu66.top

Go:   // 手写回溯递归
来源：http://rfo.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://jur.0kj1m.cn

C#:   // 手写回溯递归
来源：http://rwz.jqgfzy.top

[N09] 栈与队列
来源：http://ikt.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hum.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xge.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ata.andypj.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://riu.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iqm.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dww.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://idh.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iyk.hywenlv.cn

[N10] 链表节点定义
来源：http://phr.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwt.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vkh.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyj.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vck.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://nlz.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://eki.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kjq.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://waq.yfazqb.com

[N11] 二叉树中序遍历
来源：http://jdw.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xev.tian-w.cn

PHP:  // 手写递归函数
来源：http://mxl.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aak.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://unx.316326.xyz

Java: // 手写递归
来源：http://enx.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://yvd.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ybq.chenzaomai.com

C#:   // 手写递归
来源：http://czc.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zxc.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://geu.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zbi.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ubo.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybf.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://inp.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vhh.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://egs.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nzd.gaohongyu789.top

================================================================================
来源：http://omz.aizwys.cn

O. 并发与异步
来源：http://dxp.kuanghao11.cn

================================================================================
来源：http://tvi.iojbl.cn

[O01] 启动一个线程
来源：http://vib.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nsg.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://adh.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://who.wangdashe.top

TS:   // 同 JS
来源：http://gly.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://xfx.jinqigfzy.top

Go:   go f()
来源：http://mxt.yfazqb.com

Ruby: Thread.new { f }
来源：http://lsc.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://dbw.ppjwa.cn

[O02] 使用线程池
来源：http://rgt.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xch.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mgb.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://rfi.xinyue.icu

TS:   // worker_threads 线程池
来源：http://rzf.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://xdk.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vot.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ijg.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ule.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://als.hcnkem.com

Py:   with lock: shared += 1
来源：http://tki.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://ydc.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cjb.mhx1999.top

TS:   // 同 JS
来源：http://hib.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://rcr.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://edq.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fkh.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://rmj.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://iiq.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://kmp.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://clu.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://ast.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rlj.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sln.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xeg.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fyt.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://bfc.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://toy.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://kly.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kpc.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://nwc.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://uzv.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vws.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qxp.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://pji.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://suk.hcnkem.com

[O06] 使用进程池
来源：http://lon.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://maq.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://wwb.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://sqi.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://uxc.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tox.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gnq.ppjwa.cn

Ruby: // fork 块
来源：http://ywa.xziqi.cn

C#:   Parallel.For
来源：http://ddy.jinqigfzy.top

================================================================================
来源：http://rfv.c1oappe.top

P. 常用工具函数
来源：http://yik.xuetiantiany.cn

================================================================================
来源：http://yak.nanxinkj.top

[P01] 生成 UUID
来源：http://jkf.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://cjg.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://keg.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://mes.ydzc1.top

TS:   crypto.randomUUID()
来源：http://ygk.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://amk.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://iyf.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://dgv.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://tag.zhixingplan.top

[P02] MD5 / SHA256 摘要
来源：http://diu.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://joi.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ksf.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xpj.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://drx.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ggp.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vpz.xuanzx.com


<!-- 参考信息 -->