代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bro.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://emr.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://spp.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://afr.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hro.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gob.gzhubu.top

[L05] 上传文件（multipart）
来源：http://zze.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lva.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lnk.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://drv.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qkl.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ovd.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdn.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kjo.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bhi.yongpay.top

[L06] 解析响应为 JSON
来源：http://dwf.birdmap.top

Py:   resp.json()
来源：http://qey.yj202588.top

PHP:  json_decode($body, true);
来源：http://vhn.zhiwuduotai.top

JS:   await resp.json()
来源：http://wxg.ydjk.org.cn

TS:   await resp.json()
来源：http://rdu.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tzf.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjv.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://eid.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://enr.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://cgd.shangyingyoupin.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://law.vehdjk.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xnj.shangyingyoupin.top

JS:   resp.ok;  resp.status
来源：http://rjm.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://kir.zhongyouzk.top

Java: resp.statusCode()
来源：http://bvg.hywenlv.cn

Go:   resp.StatusCode
来源：http://rvi.smart0.xyz

Ruby: resp.code.to_i
来源：http://yia.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://mmk.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://utj.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ger.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://exw.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://brt.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eoc.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qao.nanxinkj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyh.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hle.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mlf.haohaochexian.top

================================================================================
来源：http://wvm.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://wzo.ppjwa.cn

================================================================================
来源：http://xte.wangdashe.top

[M01] 读取命令行参数
来源：http://lbm.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://ffg.ybcxt.top

PHP:  $argv;  $argc;
来源：http://pwv.tarul.cn

JS:   process.argv.slice(2)
来源：http://rls.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://euv.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://cvl.bjfxy.top

Go:   os.Args[1:]
来源：http://eca.fzhhl.top

Ruby: ARGV
来源：http://voz.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://laz.sysykeji.top

[M02] 读取环境变量
来源：http://oup.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://vgz.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oeh.uphjek.com

JS:   process.env.HOME
来源：http://zvk.ydjk.org.cn

TS:   process.env.HOME
来源：http://ifr.9152youxi.cn

Java: System.getenv("HOME")
来源：http://nxt.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://llb.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://feg.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://toq.yuanzhike.top

[M03] 执行外部命令
来源：http://mkr.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gla.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tcd.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pbc.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jye.guowangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lix.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://prc.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://fso.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://jvt.dianchejie.cn

[M04] 获取当前工作目录
来源：http://dpk.jqgfzy.top

Py:   os.getcwd()
来源：http://cmb.fanxiaobao.xyz

PHP:  getcwd();
来源：http://tpw.jqgufenzy.top

JS:   process.cwd()
来源：http://hoj.chenjidiqi.icu

TS:   process.cwd()
来源：http://tjk.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://lbl.haohaochexian.top

Go:   os.Getwd()
来源：http://ikf.havefunace.top

Ruby: Dir.pwd
来源：http://fof.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yub.fzhhl.top

[M05] 设置退出码
来源：http://pwq.yuanzhike.top

Py:   sys.exit(1)
来源：http://ofa.shanyushiyangtech.top

PHP:  exit(1);
来源：http://qfr.haohaochexian.top

JS:   process.exit(1)
来源：http://agq.redwolf501.top

TS:   process.exit(1)
来源：http://suf.shzxlz.cn

Java: System.exit(1)
来源：http://wvs.tian-w.cn

Go:   os.Exit(1)
来源：http://vtp.yj202588.top

Ruby: exit 1
来源：http://rmv.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwj.nanxuanxn.top

[M06] 向标准错误输出
来源：http://hal.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://oim.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rsx.cheryme.top

JS:   console.error("err")
来源：http://ikl.ydjk.org.cn

TS:   console.error("err")
来源：http://dwa.quarkkingdee.top

Java: System.err.println("err")
来源：http://dkp.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xwx.zhongyouzk.top

Ruby: warn "err"
来源：http://aem.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://uxf.yj20258.top

[M07] 判断是否为主入口
来源：http://lqb.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://akm.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dwb.quarkkingdee.top

JS:   require.main === module
来源：http://qdk.gotoacloud.top

TS:   require.main === module
来源：http://job.aizwys.cn

Java: public static void main(String[] args)
来源：http://gkh.tian-w.cn

Go:   func main()
来源：http://eiw.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eiv.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://eog.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://jlx.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://vxc.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://osa.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://bdi.316326.xyz

TS:   process.platform;  process.version
来源：http://xpd.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nds.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ylr.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://csp.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mrr.dashuyun.cn

================================================================================
来源：http://juf.shuidangran.top

N. 数据结构与算法
来源：http://trc.iojbl.cn

================================================================================
来源：http://itz.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://gzp.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://jtw.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://djq.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abx.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://acr.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://drc.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://mmo.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oyu.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://kxq.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://tns.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://ddy.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ava.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://htw.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://kje.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dow.52xcode.cn

Go:   slices.Sort(arr)
来源：http://hmn.xinyue.icu

Ruby: arr.sort
来源：http://gez.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://teu.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://xww.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ytb.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://cqm.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://veu.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qgu.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ici.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bjm.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://afo.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://dzx.epnwcf.com

[N04] 斐波那契数列
来源：http://cqn.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vla.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cfu.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://waa.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ijx.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bmk.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xtj.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qlk.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gah.chenjidiqi.icu

[N05] 最大公约数
来源：http://bbg.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://bgx.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pbv.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ais.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xqf.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jde.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lhx.jyoumei.cn

Ruby: a.gcd(b)
来源：http://tpq.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hnt.svipenyu.cn

[N06] 判断回文字符串
来源：http://hcb.aibaodan.cn

Py:   s == s[::-1]
来源：http://hof.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://sjl.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://vbv.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://gjs.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fbt.cucudq.cn

Go:   // 双指针从两端比较
来源：http://bmm.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://ppd.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pjt.havefunace.top

[N07] 两数之和（返回下标）
来源：http://vgy.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lqt.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jis.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pdb.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://qyw.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://cuj.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://qfv.daxiang520.top

Ruby: // 手写 Hash
来源：http://cyo.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://ldp.cucudq.cn

[N08] 生成全排列
来源：http://pez.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://jtx.fehbvm.com

PHP:  // 手写递归交换
来源：http://wht.nwbrower.top

JS:   // 手写回溯递归
来源：http://mbv.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://vpt.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://kts.fengsongda.top

Go:   // 手写回溯递归
来源：http://sap.cheryme.top

Ruby: arr.permutation.to_a
来源：http://hlm.jinqigufen.top

C#:   // 手写回溯递归
来源：http://wvl.hfpthk.cn

[N09] 栈与队列
来源：http://zjl.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sqe.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yyl.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://guo.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bec.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wmc.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://saq.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hjr.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mdw.hcnkem.com

[N10] 链表节点定义
来源：http://uov.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tum.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jgg.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://etf.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://syb.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://plx.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://dmd.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iwc.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cjg.xuanzx.com

[N11] 二叉树中序遍历
来源：http://ses.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vco.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://kgu.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nov.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uny.ppjwa.cn

Java: // 手写递归
来源：http://gfu.shuidangran.top

Go:   // 手写递归
来源：http://obx.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://crx.0kj1m.cn

C#:   // 手写递归
来源：http://ppr.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzq.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wjb.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gcu.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mwf.chenzaomai.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://crw.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rog.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fxd.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fgj.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://myt.iojbl.cn

================================================================================
来源：http://vzm.xuanzx.com

O. 并发与异步
来源：http://cnj.shangyingyoupin.top

================================================================================
来源：http://fef.guowangkeji.top

[O01] 启动一个线程
来源：http://jra.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://duc.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qel.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://urh.yuxming.cn

TS:   // 同 JS
来源：http://vgs.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://ysg.tian-w.cn

Go:   go f()
来源：http://dtu.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://rkn.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://dfg.vqdsnc.cn

[O02] 使用线程池
来源：http://jln.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gmj.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tlc.tian-w.cn

JS:   // worker_threads 线程池
来源：http://grm.daria6918.cn

TS:   // worker_threads 线程池
来源：http://roa.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://uvv.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pow.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iep.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://avr.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://gnd.yuanzhike.top

Py:   with lock: shared += 1
来源：http://dya.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://ghs.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xvs.cheryme.top

TS:   // 同 JS
来源：http://tet.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://rbf.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jkf.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pay.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://sof.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://awq.pycfn.com

Py:   async def f():⏎    await g()
来源：http://ede.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lwp.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://jvv.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rer.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fbc.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://owa.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ekx.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://eih.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://uto.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://pho.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kbz.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://gbk.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://djq.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywk.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wrm.shuidangran.top

Ruby: threads.map(&:join)
来源：http://muk.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://awn.yangfankeji.com

[O06] 使用进程池
来源：http://ozl.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xbw.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bda.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://wde.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://qpg.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xdc.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cai.sweek.top

Ruby: // fork 块
来源：http://xqv.hfpthk.cn

C#:   Parallel.For
来源：http://age.52xcode.cn

================================================================================
来源：http://rwx.jqgfzy.top

P. 常用工具函数
来源：http://esn.sweek.top

================================================================================
来源：http://xua.cheryme.top

[P01] 生成 UUID
来源：http://ure.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://tfn.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uwn.cashguo.top

JS:   crypto.randomUUID()
来源：http://vjz.vehdjk.com

TS:   crypto.randomUUID()
来源：http://esp.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://jzz.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://jan.tarul.cn

Ruby: SecureRandom.uuid
来源：http://pfb.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://riq.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://tnk.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ssr.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ger.tian-w.cn


<!-- 参考信息 -->