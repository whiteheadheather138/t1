代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kvv.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wof.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zpv.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jzq.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aot.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tca.hammf.cn

[L05] 上传文件（multipart）
来源：http://wqa.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qtt.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jcq.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wom.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zmg.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lsg.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dmd.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sjl.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xvb.jinghuilouyu.cn

[L06] 解析响应为 JSON
来源：http://sdp.epnwcf.com

Py:   resp.json()
来源：http://xlg.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://sfl.dashuyun.cn

JS:   await resp.json()
来源：http://tes.yj202588.top

TS:   await resp.json()
来源：http://qao.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hub.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://crw.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://yaa.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vik.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://llk.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yyw.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ynh.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://oty.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://sia.yuxming.cn

Java: resp.statusCode()
来源：http://pak.gaohongyu789.top

Go:   resp.StatusCode
来源：http://kpg.redwolf501.top

Ruby: resp.code.to_i
来源：http://aln.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://kdb.aibaodan.cn

[L08] 并发请求多个地址
来源：http://gmd.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vyj.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://wqm.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqw.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://itr.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tek.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uhf.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kon.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://skn.jqgfzy.top

================================================================================
来源：http://xkz.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://ljm.pengpengdd.cyou

================================================================================
来源：http://azv.haohaochexian.top

[M01] 读取命令行参数
来源：http://eng.hammf.cn

Py:   sys.argv[1:]
来源：http://nwh.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://nur.havefunace.top

JS:   process.argv.slice(2)
来源：http://rix.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://nsu.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://gxj.iojbl.cn

Go:   os.Args[1:]
来源：http://qyi.jinghuilouyu.cn

Ruby: ARGV
来源：http://gct.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://kro.chenlongwang.top

[M02] 读取环境变量
来源：http://mut.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://kss.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xmh.ybcxt.top

JS:   process.env.HOME
来源：http://vua.fehbvm.com

TS:   process.env.HOME
来源：http://nbn.yonumen.top

Java: System.getenv("HOME")
来源：http://djx.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbj.zycfv.cn

Ruby: ENV["HOME"]
来源：http://kbb.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uym.redwolf501.top

[M03] 执行外部命令
来源：http://xfc.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvm.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://geh.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://iib.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rhz.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bxc.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://snw.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://rbu.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://yvi.tian-w.cn

[M04] 获取当前工作目录
来源：http://qfl.xylfe.cn

Py:   os.getcwd()
来源：http://emt.shuidangran.top

PHP:  getcwd();
来源：http://npa.yonumen.top

JS:   process.cwd()
来源：http://zie.yueranfly.top

TS:   process.cwd()
来源：http://fpf.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://emg.gzhubu.top

Go:   os.Getwd()
来源：http://hrz.bbcook.cn

Ruby: Dir.pwd
来源：http://xyb.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://axa.dashuyun.cn

[M05] 设置退出码
来源：http://sgr.andypj.xyz

Py:   sys.exit(1)
来源：http://zao.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://poz.wangdashe.top

JS:   process.exit(1)
来源：http://imj.ydjk.org.cn

TS:   process.exit(1)
来源：http://vcx.jqgfzy.top

Java: System.exit(1)
来源：http://kvp.yonumen.top

Go:   os.Exit(1)
来源：http://xix.sufxvd.cn

Ruby: exit 1
来源：http://fzi.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://loo.zhengqikj.top

[M06] 向标准错误输出
来源：http://fza.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://plc.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eoa.cqqwz.cn

JS:   console.error("err")
来源：http://rie.hnqzz.top

TS:   console.error("err")
来源：http://lxr.yj202588.top

Java: System.err.println("err")
来源：http://gcu.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mll.fanxiaobao.xyz

Ruby: warn "err"
来源：http://fck.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://yte.havefunace.top

[M07] 判断是否为主入口
来源：http://oze.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://mzd.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zni.haohaochexian.top

JS:   require.main === module
来源：http://gcp.yuxming.cn

TS:   require.main === module
来源：http://axf.aibaodan.cn

Java: public static void main(String[] args)
来源：http://pyz.snrcjt.cn

Go:   func main()
来源：http://euv.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dzt.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://mcp.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://rtp.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://knh.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://uou.cucudq.cn

JS:   process.platform;  process.version
来源：http://phc.tianlin.xyz

TS:   process.platform;  process.version
来源：http://tvx.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uxw.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ycm.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vwj.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nol.hnqzz.top

================================================================================
来源：http://pcf.yonumen.top

N. 数据结构与算法
来源：http://kfc.zhongyouzk.top

================================================================================
来源：http://cur.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://yrg.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rru.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mkd.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwr.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbx.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://hkk.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://bgu.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kwr.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://rby.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://fvf.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://fcr.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kme.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cpo.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://leo.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xbn.hammf.cn

Go:   slices.Sort(arr)
来源：http://aaa.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://kjf.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gnb.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://lnt.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://czz.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://uht.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zse.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tsl.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://smb.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwu.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lhs.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://wwz.fktsv.cn

[N04] 斐波那契数列
来源：http://lmz.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://buv.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tfk.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lic.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xjr.cashguo.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wsr.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://emu.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xog.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vyv.jinqigufen.top

[N05] 最大公约数
来源：http://bgh.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://snc.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lnd.c1oappe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vwb.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://val.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zml.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xbu.epnwcf.com

Ruby: a.gcd(b)
来源：http://mww.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wuo.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://xhs.zdbjq.cn

Py:   s == s[::-1]
来源：http://uhg.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://vlw.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://jgq.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://ifo.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oss.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://bnb.birdmap.top

Ruby: s == s.reverse
来源：http://kqc.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://urp.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://xjv.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xvu.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vza.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tpw.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://lrp.cqqwz.cn

Java: // 手写 HashMap
来源：http://nnl.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://hjf.vehdjk.com

Ruby: // 手写 Hash
来源：http://pao.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://onc.zhengqikj.top

[N08] 生成全排列
来源：http://rjf.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://kdr.svipenyu.cn

PHP:  // 手写递归交换
来源：http://qdx.52xcode.cn

JS:   // 手写回溯递归
来源：http://eus.epnwcf.com

TS:   // 手写回溯递归
来源：http://jbi.hnqzz.top

Java: // 手写回溯递归
来源：http://ypc.pycfn.com

Go:   // 手写回溯递归
来源：http://and.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://snm.andypj.xyz

C#:   // 手写回溯递归
来源：http://dqz.sweek.top

[N09] 栈与队列
来源：http://vmd.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gck.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xai.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mrk.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vzz.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujb.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mfb.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zot.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kli.chenzaomai.com

[N10] 链表节点定义
来源：http://rgn.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fpo.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uxr.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bvo.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zvh.havefunace.top

Java: class Node { int v; Node next; }
来源：http://cce.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dgr.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vhl.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bui.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://jsp.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tbp.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://zyt.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sef.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ebg.hysaishi.cn

Java: // 手写递归
来源：http://tzh.jianghu66.top

Go:   // 手写递归
来源：http://pky.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kcb.xziqi.cn

C#:   // 手写递归
来源：http://nyk.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wil.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gla.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lrv.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yuh.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ynv.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uql.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xwa.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wgh.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kmg.haohaochexian.top

================================================================================
来源：http://elg.ywan-chungtsiang.top

O. 并发与异步
来源：http://fhp.jinghuilouyu.cn

================================================================================
来源：http://mnm.xinyue.icu

[O01] 启动一个线程
来源：http://hno.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sxb.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xza.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kev.guowangkeji.top

TS:   // 同 JS
来源：http://ona.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://qsc.tanke756.top

Go:   go f()
来源：http://fzi.guannengcc.top

Ruby: Thread.new { f }
来源：http://kpu.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://elt.zhoulong.xyz

[O02] 使用线程池
来源：http://ide.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tgg.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qza.tian-w.cn

JS:   // worker_threads 线程池
来源：http://baq.yvedp.cn

TS:   // worker_threads 线程池
来源：http://fta.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://fig.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mlt.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://enf.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ohq.yfazqb.com

[O03] 加锁保护共享数据
来源：http://msk.hfpthk.cn

Py:   with lock: shared += 1
来源：http://uoc.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://eer.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tjg.havefunace.top

TS:   // 同 JS
来源：http://lfl.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://guy.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sdd.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vhj.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://zlr.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://hpu.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://lyr.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eup.bjfxy.top

JS:   async function f() { await g(); }
来源：http://mrh.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zon.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dyu.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hvx.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zxt.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://ync.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://npx.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://kxs.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kbz.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://edz.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://vjn.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rok.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nif.fengsongda.top

Ruby: threads.map(&:join)
来源：http://iel.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wck.epnwcf.com

[O06] 使用进程池
来源：http://zsu.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gyf.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://diw.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://byp.yj20258.top

TS:   // child_process / cluster 模块
来源：http://jwg.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iiu.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vye.jqgufenzy.top

Ruby: // fork 块
来源：http://naf.chenlongwang.top

C#:   Parallel.For
来源：http://mns.jinyuanbaomall.cn

================================================================================
来源：http://arr.sysykeji.top

P. 常用工具函数
来源：http://dtd.aibaodan.cn

================================================================================
来源：http://kqq.zhongyouzk.top

[P01] 生成 UUID
来源：http://nyp.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://gwl.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvr.fehbvm.com

JS:   crypto.randomUUID()
来源：http://dux.wangdashe.top

TS:   crypto.randomUUID()
来源：http://ioe.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://cya.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://qtx.meibo888.top

Ruby: SecureRandom.uuid
来源：http://afn.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://xjo.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://dob.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xuw.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzm.gotoacloud.top


<!-- 参考信息 -->