代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iyz.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ces.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lfn.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rfm.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbh.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oij.c1oappe.top

[L05] 上传文件（multipart）
来源：http://jvb.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rre.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ibs.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kvv.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jfd.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cyb.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yog.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dzf.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zrk.hnqzz.top

[L06] 解析响应为 JSON
来源：http://zsf.tarul.cn

Py:   resp.json()
来源：http://nce.zycfv.cn

PHP:  json_decode($body, true);
来源：http://fvp.vehdjk.com

JS:   await resp.json()
来源：http://kyb.jianghu66.top

TS:   await resp.json()
来源：http://fsw.zhoulong.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ett.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pix.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://ihp.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zcx.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://npx.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwa.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://koy.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://byn.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://zdi.redwolf501.top

Java: resp.statusCode()
来源：http://pzg.tianlin.xyz

Go:   resp.StatusCode
来源：http://nvo.dianchejie.cn

Ruby: resp.code.to_i
来源：http://ypq.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://yec.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://bnj.yuxming.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bcd.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://ksi.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://poj.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emq.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zcg.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dfj.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jiz.fanxiaobao.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cat.fktsv.cn

================================================================================
来源：http://nhb.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://gqe.gotoacloud.top

================================================================================
来源：http://mby.bbcook.cn

[M01] 读取命令行参数
来源：http://sev.sufxvd.cn

Py:   sys.argv[1:]
来源：http://tqv.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://mhe.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://eep.yongpay.top

TS:   process.argv.slice(2)
来源：http://uqp.ivvv.top

Java: args 数组（main 方法参数）
来源：http://trs.tian-w.cn

Go:   os.Args[1:]
来源：http://lnm.ppjwa.cn

Ruby: ARGV
来源：http://vwp.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://xrj.nwbrower.top

[M02] 读取环境变量
来源：http://yym.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://bws.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cvv.pengpengdd.cyou

JS:   process.env.HOME
来源：http://hfz.zycfv.cn

TS:   process.env.HOME
来源：http://ctt.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://woz.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://agi.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://wfr.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dxg.jlsjyb.cn

[M03] 执行外部命令
来源：http://kqk.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lyt.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zqf.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ghu.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hbq.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xla.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wgo.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://uia.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://iwx.nanxinkj.top

[M04] 获取当前工作目录
来源：http://usu.jyoumei.cn

Py:   os.getcwd()
来源：http://wkv.cashguo.top

PHP:  getcwd();
来源：http://pnn.gotoacloud.top

JS:   process.cwd()
来源：http://kpd.jqgfzy.top

TS:   process.cwd()
来源：http://fhi.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://jlf.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://bsp.redwolf501.top

Ruby: Dir.pwd
来源：http://hna.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xmf.cqqwz.cn

[M05] 设置退出码
来源：http://myy.0kj1m.cn

Py:   sys.exit(1)
来源：http://oih.yangfankeji.com

PHP:  exit(1);
来源：http://hcq.wangshuangyany.cn

JS:   process.exit(1)
来源：http://znl.shzxlz.cn

TS:   process.exit(1)
来源：http://wat.ctjpmb.com

Java: System.exit(1)
来源：http://ckw.jqgfzy.top

Go:   os.Exit(1)
来源：http://amq.hongshengwenyu.top

Ruby: exit 1
来源：http://ama.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xua.aizwys.cn

[M06] 向标准错误输出
来源：http://oad.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://cuk.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dlx.wangshuangyany.cn

JS:   console.error("err")
来源：http://qxp.sysykeji.top

TS:   console.error("err")
来源：http://czl.gogol.net.cn

Java: System.err.println("err")
来源：http://duj.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vix.cheryme.top

Ruby: warn "err"
来源：http://mrj.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://scs.hfpthk.cn

[M07] 判断是否为主入口
来源：http://ypo.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://yrc.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dmz.cashguo.top

JS:   require.main === module
来源：http://qew.fengsongda.top

TS:   require.main === module
来源：http://tav.xylfe.cn

Java: public static void main(String[] args)
来源：http://toz.jinghuilouyu.cn

Go:   func main()
来源：http://ptb.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://auv.ydzc1.top

C#:   static void Main(string[] args)
来源：http://dik.yj20258.top

[M08] 获取系统与运行时信息
来源：http://gqo.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://ybq.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://yix.nanxinkj.top

JS:   process.platform;  process.version
来源：http://vwi.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://nju.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fhw.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://mzd.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rok.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvs.kuanghao11.cn

================================================================================
来源：http://bvw.xuanzx.com

N. 数据结构与算法
来源：http://cyb.jianghu66.top

================================================================================
来源：http://svt.tanke756.top

[N01] 二分查找（有序数组）
来源：http://ozl.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://rnx.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jvq.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rex.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rkf.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://efg.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://pfz.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lav.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://ygl.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://wbm.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://kex.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://psg.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fnk.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lwj.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qng.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://ury.shanyushiyangtech.top

Ruby: arr.sort
来源：http://tsg.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://mfm.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://mrn.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zyl.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://dwj.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avi.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dlg.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qju.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzj.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ddt.daria6918.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hsy.ppjwa.cn

[N04] 斐波那契数列
来源：http://pru.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wrx.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lcj.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pcd.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpb.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yps.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://czn.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dse.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://igl.fengsongda.top

[N05] 最大公约数
来源：http://fue.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://tvs.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hfk.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iwi.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zsn.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wcp.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ezo.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://okf.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vho.ybcxt.top

[N06] 判断回文字符串
来源：http://nhz.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://lpo.sysykeji.top

PHP:  $s === strrev($s);
来源：http://sqq.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://kvh.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://oby.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pod.yongpay.top

Go:   // 双指针从两端比较
来源：http://ttr.hywenlv.cn

Ruby: s == s.reverse
来源：http://mfx.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qmu.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://dun.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fwg.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gkv.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://udo.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://oda.ydzc1.top

Java: // 手写 HashMap
来源：http://sjo.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://dst.tanke756.top

Ruby: // 手写 Hash
来源：http://elp.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zoy.chenlongwang.top

[N08] 生成全排列
来源：http://tkb.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://jbh.yuxming.cn

PHP:  // 手写递归交换
来源：http://qtk.yvedp.cn

JS:   // 手写回溯递归
来源：http://ukr.ehwqpu.com

TS:   // 手写回溯递归
来源：http://vuo.epnwcf.com

Java: // 手写回溯递归
来源：http://vrq.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://oiz.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://ble.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://sqt.cqqwz.cn

[N09] 栈与队列
来源：http://acd.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://flb.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hsk.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gxw.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mkw.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mpb.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://moe.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fsx.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rqu.ivvv.top

[N10] 链表节点定义
来源：http://qcl.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://thd.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cnd.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wag.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://myg.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://vrk.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://khf.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hso.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vze.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://nef.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zor.cqqwz.cn

PHP:  // 手写递归函数
来源：http://ofu.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cdj.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffu.wangdashe.top

Java: // 手写递归
来源：http://lpf.ehwqpu.com

Go:   // 手写递归
来源：http://bjh.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hnr.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://wgr.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qyf.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://huf.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://opk.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klz.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhp.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wiq.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cfh.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tcn.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sbg.ivvv.top

================================================================================
来源：http://nqh.guannengcc.top

O. 并发与异步
来源：http://csr.zhengqikj.top

================================================================================
来源：http://gha.jinqigfzy.top

[O01] 启动一个线程
来源：http://fzl.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncq.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kec.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://seu.hysaishi.cn

TS:   // 同 JS
来源：http://iaw.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://fry.yvedp.cn

Go:   go f()
来源：http://glh.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://phi.pycfn.com

C#:   Task.Run(() => F());
来源：http://fwp.zycfv.cn

[O02] 使用线程池
来源：http://rig.ywan-chungtsiang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rpv.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://exu.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://bfd.guannengcc.top

TS:   // worker_threads 线程池
来源：http://otu.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://qtq.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://amb.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vef.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nvd.yj20258888.top

[O03] 加锁保护共享数据
来源：http://yiv.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://adj.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://ryi.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tmv.pengpengdd.cyou

TS:   // 同 JS
来源：http://kov.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ymw.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://act.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://bny.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://bwo.jianghu66.top

[O04] 定义异步函数并等待
来源：http://tnx.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://kks.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fez.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://iuz.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://moa.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ijq.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lgl.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://vvn.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://pty.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://dcz.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://hmt.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xrf.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://rdr.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://pzy.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iqq.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qfw.fzhhl.top

Ruby: threads.map(&:join)
来源：http://oat.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yhf.hnxiangtu.top

[O06] 使用进程池
来源：http://vzj.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vml.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bua.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://ecs.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://ynv.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ggx.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dkm.ydjk.org.cn

Ruby: // fork 块
来源：http://krs.fktsv.cn

C#:   Parallel.For
来源：http://cfd.gotoacloud.top

================================================================================
来源：http://bxb.daria6918.cn

P. 常用工具函数
来源：http://phj.andypj.xyz

================================================================================
来源：http://fpe.52xcode.cn

[P01] 生成 UUID
来源：http://cry.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://dgn.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rfi.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://dmg.vehdjk.com

TS:   crypto.randomUUID()
来源：http://qiu.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://vrg.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://hbk.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://oko.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://jck.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://fuq.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jhd.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://toa.havefunace.top


<!-- 参考信息 -->