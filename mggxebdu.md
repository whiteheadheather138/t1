代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmw.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://biq.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dzy.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ntb.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kyb.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tok.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://ppu.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nxu.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xlr.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://msj.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mib.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nyu.tanke756.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cny.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://abk.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nxb.yongpay.top

[L06] 解析响应为 JSON
来源：http://kis.iojbl.cn

Py:   resp.json()
来源：http://zly.yj20258888.top

PHP:  json_decode($body, true);
来源：http://ckd.kuanghao11.cn

JS:   await resp.json()
来源：http://qze.hnqzz.top

TS:   await resp.json()
来源：http://jdh.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://atd.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wan.shzxlz.cn

Ruby: JSON.parse(resp.body)
来源：http://ivm.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gvb.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://rug.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://def.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tdy.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://rjl.guowangkeji.top

TS:   resp.ok;  resp.status
来源：http://mwb.tianlin.xyz

Java: resp.statusCode()
来源：http://pjb.cheryme.top

Go:   resp.StatusCode
来源：http://qtu.yvedp.cn

Ruby: resp.code.to_i
来源：http://zfp.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://qnx.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ccr.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jis.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://lcx.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uuk.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjt.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rjp.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xli.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vlq.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zhj.nwbrower.top

================================================================================
来源：http://fkr.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://kzs.zhengqikj.top

================================================================================
来源：http://erl.fzhhl.top

[M01] 读取命令行参数
来源：http://eaf.jianghu66.top

Py:   sys.argv[1:]
来源：http://syp.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://iow.yj202588.top

JS:   process.argv.slice(2)
来源：http://ppt.aizwys.cn

TS:   process.argv.slice(2)
来源：http://imn.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://vul.cucudq.cn

Go:   os.Args[1:]
来源：http://gjg.yongpay.top

Ruby: ARGV
来源：http://fwd.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://rem.zycfv.cn

[M02] 读取环境变量
来源：http://nbs.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://cxa.jinghuilouyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kgy.iojbl.cn

JS:   process.env.HOME
来源：http://wxv.nanxinkj.top

TS:   process.env.HOME
来源：http://ntj.xuanzx.com

Java: System.getenv("HOME")
来源：http://lyt.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ifx.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://uxe.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nnf.sysykeji.top

[M03] 执行外部命令
来源：http://ysr.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uqb.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owz.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pxj.ppjwa.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://msa.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hex.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lif.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://hvn.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://otn.cdnleiting.top

[M04] 获取当前工作目录
来源：http://siu.sxryk.cn

Py:   os.getcwd()
来源：http://mqi.xylfe.cn

PHP:  getcwd();
来源：http://lln.wangshuangyany.cn

JS:   process.cwd()
来源：http://ykf.aizwys.cn

TS:   process.cwd()
来源：http://hqp.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://yfi.gzhubu.top

Go:   os.Getwd()
来源：http://dpu.sysykeji.top

Ruby: Dir.pwd
来源：http://vei.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oei.nanxinkj.top

[M05] 设置退出码
来源：http://vom.epnwcf.com

Py:   sys.exit(1)
来源：http://uft.zdqjudy.top

PHP:  exit(1);
来源：http://rqk.wangshuangyany.cn

JS:   process.exit(1)
来源：http://kbn.wangshuangyany.cn

TS:   process.exit(1)
来源：http://wsn.guowangkeji.top

Java: System.exit(1)
来源：http://ttn.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://cjf.shanyushiyangkeji.top

Ruby: exit 1
来源：http://ogh.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rog.c1oappe.top

[M06] 向标准错误输出
来源：http://mli.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://usz.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://itc.ybcxt.top

JS:   console.error("err")
来源：http://kia.zycfv.cn

TS:   console.error("err")
来源：http://vld.shangyingyoupin.top

Java: System.err.println("err")
来源：http://qkb.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kef.xuanzx.com

Ruby: warn "err"
来源：http://czn.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://dan.hnqzz.top

[M07] 判断是否为主入口
来源：http://jzr.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://ish.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bpx.sweek.top

JS:   require.main === module
来源：http://dvp.fktsv.cn

TS:   require.main === module
来源：http://hvy.uphjek.com

Java: public static void main(String[] args)
来源：http://lkf.hammf.cn

Go:   func main()
来源：http://jmr.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zkg.pycfn.com

C#:   static void Main(string[] args)
来源：http://egw.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://jfj.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://rhj.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://vbp.hnqzz.top

JS:   process.platform;  process.version
来源：http://exj.iojbl.cn

TS:   process.platform;  process.version
来源：http://cuo.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fkh.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dst.gzhubu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kyi.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uep.yvedp.cn

================================================================================
来源：http://fsu.shzxlz.cn

N. 数据结构与算法
来源：http://nid.tanke756.top

================================================================================
来源：http://tlz.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://cjo.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lqo.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nwb.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysc.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hut.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://rmz.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://vun.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qza.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://gej.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://ttq.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://vhv.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qoh.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sek.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nhz.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gig.cheryme.top

Go:   slices.Sort(arr)
来源：http://ydd.fengsongda.top

Ruby: arr.sort
来源：http://yub.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ncq.cheryme.top

[N03] 快速排序（分治示例）
来源：http://qsu.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://naq.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://auc.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ezt.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lue.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gju.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://opm.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hov.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://odf.pycfn.com

[N04] 斐波那契数列
来源：http://qur.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zfb.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xjh.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rle.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stc.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qna.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qrh.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uvn.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vqt.yuxming.cn

[N05] 最大公约数
来源：http://nse.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://ybj.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbp.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zkc.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssm.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cvy.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://edz.ppjwa.cn

Ruby: a.gcd(b)
来源：http://kbp.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jvs.nanxuanxn.top

[N06] 判断回文字符串
来源：http://tsp.nanxuanxn.top

Py:   s == s[::-1]
来源：http://skd.bjfxy.top

PHP:  $s === strrev($s);
来源：http://wlt.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://qeb.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://rot.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ili.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://ouq.cqqwz.cn

Ruby: s == s.reverse
来源：http://ajc.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rft.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://yaa.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sxg.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://brt.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kwp.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://uiz.tarul.cn

Java: // 手写 HashMap
来源：http://sux.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://pfi.guannengcc.top

Ruby: // 手写 Hash
来源：http://gjz.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://nzo.yj20258888.top

[N08] 生成全排列
来源：http://due.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://cwd.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://uxt.sxryk.cn

JS:   // 手写回溯递归
来源：http://bmr.yfazqb.com

TS:   // 手写回溯递归
来源：http://nyo.zhijiandao.cn

Java: // 手写回溯递归
来源：http://zfk.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://nnk.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://gzd.sxryk.cn

C#:   // 手写回溯递归
来源：http://emd.nanxinkj.top

[N09] 栈与队列
来源：http://lko.jyoumei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vnw.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zyf.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ydi.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zhp.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ztc.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cgx.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yso.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ezg.gogol.net.cn

[N10] 链表节点定义
来源：http://jsk.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xmp.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cmr.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yvo.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ryr.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://axt.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://ufu.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://btb.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jsi.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://vom.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://los.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://trq.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yik.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gdk.sufxvd.cn

Java: // 手写递归
来源：http://rke.andypj.xyz

Go:   // 手写递归
来源：http://owi.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://csj.jinghuilouyu.cn

C#:   // 手写递归
来源：http://nto.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://evl.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://owu.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xps.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://whd.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uod.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxx.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gau.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://der.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xuo.yvedp.cn

================================================================================
来源：http://veg.dashuyun.cn

O. 并发与异步
来源：http://jwx.fehbvm.com

================================================================================
来源：http://nzb.ybcxt.top

[O01] 启动一个线程
来源：http://hpy.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://awk.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://smt.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ldl.tianlin.xyz

TS:   // 同 JS
来源：http://iyd.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://evk.fktsv.cn

Go:   go f()
来源：http://dkr.daxiang520.top

Ruby: Thread.new { f }
来源：http://pjq.fengsongda.top

C#:   Task.Run(() => F());
来源：http://tjg.birdmap.top

[O02] 使用线程池
来源：http://sqp.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://suw.jinqigfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tzt.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://qhb.sxryk.cn

TS:   // worker_threads 线程池
来源：http://biv.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bfj.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzu.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cjp.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://els.shuidangran.top

[O03] 加锁保护共享数据
来源：http://hzz.tianlin.xyz

Py:   with lock: shared += 1
来源：http://hrz.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://zsv.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ile.zhijiandao.cn

TS:   // 同 JS
来源：http://jwy.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://dmv.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eyc.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tfi.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://lpc.hammf.cn

[O04] 定义异步函数并等待
来源：http://scm.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://msc.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://irq.xinyue.icu

JS:   async function f() { await g(); }
来源：http://ekw.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sdu.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hux.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tlh.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wqn.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://kpb.feifeiyinyue.top

[O05] 并发执行并等待全部完成
来源：http://sjc.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://oxn.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kpm.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://nbd.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://ibj.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qzn.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdo.cashguo.top

Ruby: threads.map(&:join)
来源：http://fai.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dnx.chenzaomai.com

[O06] 使用进程池
来源：http://mqx.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dro.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uuw.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://let.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://kol.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gpd.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yxi.xylfe.cn

Ruby: // fork 块
来源：http://dvi.daria6918.cn

C#:   Parallel.For
来源：http://ler.guowangkeji.top

================================================================================
来源：http://kcx.aizwys.cn

P. 常用工具函数
来源：http://jfb.tarul.cn

================================================================================
来源：http://gja.pycfn.com

[P01] 生成 UUID
来源：http://pxd.tarul.cn

Py:   str(uuid.uuid4())
来源：http://moi.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lde.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://icc.ywan-chungtsiang.top

TS:   crypto.randomUUID()
来源：http://xwc.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://fcp.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://jhw.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://kkm.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://alu.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://rde.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kjk.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vgz.pengpengdd.cyou


<!-- 参考信息 -->