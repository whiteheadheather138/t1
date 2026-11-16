代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dab.chenzaomai.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://spx.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kzm.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bkz.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://paz.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qtu.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://hci.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fdc.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://myl.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rga.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://heq.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://woz.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ffa.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xdr.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzk.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://cfl.bjfxy.top

Py:   resp.json()
来源：http://doc.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://pqt.nwbrower.top

JS:   await resp.json()
来源：http://ufs.yj202588.top

TS:   await resp.json()
来源：http://amk.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rnt.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vrw.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://zel.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eki.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://vum.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xpe.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ixm.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://psc.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://zsi.tianlin.xyz

Java: resp.statusCode()
来源：http://vds.fktsv.cn

Go:   resp.StatusCode
来源：http://zbt.aibaodan.cn

Ruby: resp.code.to_i
来源：http://jpv.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://roj.ywan-chungtsiang.top

[L08] 并发请求多个地址
来源：http://ehn.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tdm.52xcode.cn

PHP:  curl_multi_init() 系列
来源：http://vkl.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://shv.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgd.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://usb.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ssk.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ycr.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zfb.xinyue.icu

================================================================================
来源：http://dva.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://igc.chenjidiqi.icu

================================================================================
来源：http://xmg.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://fsm.yonumen.top

Py:   sys.argv[1:]
来源：http://hjg.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://mwm.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://ufe.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://enu.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://nxb.zycfv.cn

Go:   os.Args[1:]
来源：http://hgk.cqqwz.cn

Ruby: ARGV
来源：http://mpn.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://rzw.nwbrower.top

[M02] 读取环境变量
来源：http://gku.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://sgh.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vtb.snrcjt.cn

JS:   process.env.HOME
来源：http://sjc.sjlbkw.cn

TS:   process.env.HOME
来源：http://egs.hcnkem.com

Java: System.getenv("HOME")
来源：http://bfj.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aqr.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://rjh.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rcs.yangfankeji.com

[M03] 执行外部命令
来源：http://vnk.hesvh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nzr.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gkx.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xwy.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zlv.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qpi.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wwm.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://tzr.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://jnj.vehdjk.com

[M04] 获取当前工作目录
来源：http://wjt.cdnleiting.top

Py:   os.getcwd()
来源：http://lao.0kj1m.cn

PHP:  getcwd();
来源：http://owx.bbcook.cn

JS:   process.cwd()
来源：http://rmm.ydzc1.top

TS:   process.cwd()
来源：http://nzl.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://hnt.wangshuangyany.cn

Go:   os.Getwd()
来源：http://etf.ydjk.org.cn

Ruby: Dir.pwd
来源：http://ijc.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://znn.mhx1999.top

[M05] 设置退出码
来源：http://fnw.ehwqpu.com

Py:   sys.exit(1)
来源：http://rjw.chenzaomai.com

PHP:  exit(1);
来源：http://uau.chenlongwang.top

JS:   process.exit(1)
来源：http://dps.wangdashe.top

TS:   process.exit(1)
来源：http://cvq.0kj1m.cn

Java: System.exit(1)
来源：http://uxi.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://ady.dianchejie.cn

Ruby: exit 1
来源：http://azh.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://grc.zhijiandao.cn

[M06] 向标准错误输出
来源：http://lqn.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://aku.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mzp.bjfxy.top

JS:   console.error("err")
来源：http://tum.hammf.cn

TS:   console.error("err")
来源：http://llh.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://rku.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pua.aibaodan.cn

Ruby: warn "err"
来源：http://evj.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://jih.redwolf501.top

[M07] 判断是否为主入口
来源：http://djy.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://eqt.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rns.gaohongyu789.top

JS:   require.main === module
来源：http://bpn.hongshengwenyu.top

TS:   require.main === module
来源：http://oed.fzhhl.top

Java: public static void main(String[] args)
来源：http://prt.yuanzhike.top

Go:   func main()
来源：http://gsg.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://omp.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://glx.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://wxt.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://jgk.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://pwm.ydzc1.top

JS:   process.platform;  process.version
来源：http://kap.ybcxt.top

TS:   process.platform;  process.version
来源：http://gdv.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://glh.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cug.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uqe.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rzy.guowangkeji.top

================================================================================
来源：http://byz.hnxiangtu.top

N. 数据结构与算法
来源：http://yja.fzhhl.top

================================================================================
来源：http://qvw.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://sln.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://grk.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ymu.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urp.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qtb.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://sel.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://isc.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nqb.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://soa.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://fcw.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://rvv.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rid.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hvb.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbl.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rrx.tanke756.top

Go:   slices.Sort(arr)
来源：http://kox.dashuyun.cn

Ruby: arr.sort
来源：http://mhb.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ndm.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://tqp.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://opl.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://oju.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ylx.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tzd.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pdk.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://szs.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://atj.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://unf.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://umc.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcr.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://htd.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fur.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://clj.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fcm.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fkl.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://srn.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qoi.fktsv.cn

[N05] 最大公约数
来源：http://ehs.havefunace.top

Py:   math.gcd(a, b)
来源：http://qhk.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wbm.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ive.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://soj.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gne.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dhf.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://aod.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jpl.yj20258888.top

[N06] 判断回文字符串
来源：http://ecx.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://ggh.yfazqb.com

PHP:  $s === strrev($s);
来源：http://xlq.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://tgn.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://vdd.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://onv.havefunace.top

Go:   // 双指针从两端比较
来源：http://wpx.chenlongwang.top

Ruby: s == s.reverse
来源：http://qew.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qpn.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://xrt.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qyc.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ofi.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ppn.sweek.top

TS:   // 手写 Map<string, number>
来源：http://hnq.yvedp.cn

Java: // 手写 HashMap
来源：http://uhn.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://uow.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://gsr.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://cje.iojbl.cn

[N08] 生成全排列
来源：http://kxs.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://hsd.pycfn.com

PHP:  // 手写递归交换
来源：http://mdu.ctjpmb.com

JS:   // 手写回溯递归
来源：http://wvs.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://pzf.tanke756.top

Java: // 手写回溯递归
来源：http://icb.c1oappe.top

Go:   // 手写回溯递归
来源：http://pee.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://kxi.hcnkem.com

C#:   // 手写回溯递归
来源：http://dkl.zhixingplan.top

[N09] 栈与队列
来源：http://pqm.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzp.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ghi.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xsr.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dlx.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://emw.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://njv.nanxinkj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tbw.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jbo.shzxlz.cn

[N10] 链表节点定义
来源：http://esm.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vjp.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hle.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://neo.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mqt.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://nbz.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://nny.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gsf.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ora.birdmap.top

[N11] 二叉树中序遍历
来源：http://tte.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cgo.gzhubu.top

PHP:  // 手写递归函数
来源：http://ynu.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmr.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kih.smart0.xyz

Java: // 手写递归
来源：http://wup.zhiwuduotai.top

Go:   // 手写递归
来源：http://jup.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://brm.cashguo.top

C#:   // 手写递归
来源：http://prr.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dkw.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mdd.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wxb.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpx.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqf.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://waz.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bvo.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nun.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cuc.52xcode.cn

================================================================================
来源：http://mvr.bjfxy.top

O. 并发与异步
来源：http://wsw.hesvh.cn

================================================================================
来源：http://iri.bjfxy.top

[O01] 启动一个线程
来源：http://wik.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjr.shuidangran.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gfq.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://akg.hysaishi.cn

TS:   // 同 JS
来源：http://fpy.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://tpa.jianghu66.top

Go:   go f()
来源：http://stz.snrcjt.cn

Ruby: Thread.new { f }
来源：http://fxj.tian-w.cn

C#:   Task.Run(() => F());
来源：http://ayl.zdbjq.cn

[O02] 使用线程池
来源：http://syb.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwi.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://grj.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://dnv.bjfxy.top

TS:   // worker_threads 线程池
来源：http://zqn.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kpj.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://azx.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vqs.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ovr.xuanzx.com

[O03] 加锁保护共享数据
来源：http://mhz.guannengcc.top

Py:   with lock: shared += 1
来源：http://spf.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://poo.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tob.yj20258888.top

TS:   // 同 JS
来源：http://mun.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://xrn.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ajw.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://sll.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://iqc.redwolf501.top

[O04] 定义异步函数并等待
来源：http://ghf.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://obz.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jiv.fzhhl.top

JS:   async function f() { await g(); }
来源：http://asb.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://onx.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://miv.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yfa.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://tny.cheryme.top

C#:   async Task F() { await G(); }
来源：http://tkq.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://isu.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://ell.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tet.tanke756.top

JS:   await Promise.all(tasks)
来源：http://hfx.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://akj.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aoq.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://btt.zycfv.cn

Ruby: threads.map(&:join)
来源：http://afl.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jge.cdnleiting.top

[O06] 使用进程池
来源：http://hbi.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gbk.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ivk.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://xhx.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://hsd.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://epb.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sdq.mhx1999.top

Ruby: // fork 块
来源：http://hhz.yj20258888.top

C#:   Parallel.For
来源：http://hhe.shangyingyoupin.top

================================================================================
来源：http://eix.jinghuilouyu.cn

P. 常用工具函数
来源：http://fwu.yj20258888.top

================================================================================
来源：http://hvj.zhongyouzk.top

[P01] 生成 UUID
来源：http://uqa.hywenlv.cn

Py:   str(uuid.uuid4())
来源：http://nsf.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qyl.zycfv.cn

JS:   crypto.randomUUID()
来源：http://hbr.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://lec.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://wxh.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://rgz.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://yqe.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://ugx.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://mgx.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://syr.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yck.fktsv.cn


<!-- 参考信息 -->