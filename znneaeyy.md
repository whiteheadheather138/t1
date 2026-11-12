代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qhy.ivvv.top

[L04] 设置超时
来源：http://yko.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://mmj.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rvu.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofq.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://csc.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ajx.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ahf.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wra.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bzr.daria6918.cn

[L05] 上传文件（multipart）
来源：http://sfj.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uat.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xsl.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nzk.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vfk.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dhk.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cka.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rac.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ucr.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://cvd.havefunace.top

Py:   resp.json()
来源：http://twy.meibo888.top

PHP:  json_decode($body, true);
来源：http://bak.quarkkingdee.top

JS:   await resp.json()
来源：http://fum.gzhubu.top

TS:   await resp.json()
来源：http://rdr.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hcf.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ywx.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://fbd.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wzj.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://urb.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcl.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjy.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://kkh.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://xyr.cqqwz.cn

Java: resp.statusCode()
来源：http://wsp.svipenyu.cn

Go:   resp.StatusCode
来源：http://igb.hfpthk.cn

Ruby: resp.code.to_i
来源：http://mlr.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://ifk.hysaishi.cn

[L08] 并发请求多个地址
来源：http://qza.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uyt.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://uqp.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wza.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqh.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://csj.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jcf.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wvb.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://olg.tianlin.xyz

================================================================================
来源：http://idc.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://ane.jyoumei.cn

================================================================================
来源：http://jya.fehbvm.com

[M01] 读取命令行参数
来源：http://mch.chenlongwang.top

Py:   sys.argv[1:]
来源：http://rua.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://ohy.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://lwg.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://gar.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://xgs.jinqigfzy.top

Go:   os.Args[1:]
来源：http://pfb.yanxiufei.cn

Ruby: ARGV
来源：http://fcn.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://gzy.ydzc1.top

[M02] 读取环境变量
来源：http://lia.havefunace.top

Py:   os.environ.get("HOME")
来源：http://onn.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ytb.vqdsnc.cn

JS:   process.env.HOME
来源：http://cow.zhengqikj.top

TS:   process.env.HOME
来源：http://kiy.smart0.xyz

Java: System.getenv("HOME")
来源：http://qkj.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uqc.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://zos.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oul.hcnkem.com

[M03] 执行外部命令
来源：http://iyg.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://chy.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gvp.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fpt.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aii.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bgg.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://snr.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bpi.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://mvy.bbcook.cn

[M04] 获取当前工作目录
来源：http://lxe.xinyue.icu

Py:   os.getcwd()
来源：http://irf.hcnkem.com

PHP:  getcwd();
来源：http://xft.guowangkeji.top

JS:   process.cwd()
来源：http://fwa.daxiang520.top

TS:   process.cwd()
来源：http://nxr.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://dxz.dashuyun.cn

Go:   os.Getwd()
来源：http://jet.zdqjudy.top

Ruby: Dir.pwd
来源：http://zgb.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cpy.yfazqb.com

[M05] 设置退出码
来源：http://uiz.iojbl.cn

Py:   sys.exit(1)
来源：http://sps.fehbvm.com

PHP:  exit(1);
来源：http://xhl.epnwcf.com

JS:   process.exit(1)
来源：http://lul.shuidangran.top

TS:   process.exit(1)
来源：http://spg.hcnkem.com

Java: System.exit(1)
来源：http://pcs.9152youxi.cn

Go:   os.Exit(1)
来源：http://yom.hongshengwenyu.top

Ruby: exit 1
来源：http://kav.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dnj.jinqigfzy.top

[M06] 向标准错误输出
来源：http://qys.gzhubu.top

Py:   print("err", file=sys.stderr)
来源：http://sbe.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aoz.hysaishi.cn

JS:   console.error("err")
来源：http://tjo.jiagoushi.top

TS:   console.error("err")
来源：http://krk.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://dki.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kgk.cdnleiting.top

Ruby: warn "err"
来源：http://med.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://kgf.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://ggj.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://hri.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vru.zdqjudy.top

JS:   require.main === module
来源：http://kuc.meibo888.top

TS:   require.main === module
来源：http://mta.havefunace.top

Java: public static void main(String[] args)
来源：http://osw.bjfxy.top

Go:   func main()
来源：http://bgl.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dmh.fktsv.cn

C#:   static void Main(string[] args)
来源：http://axg.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://teo.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://lkv.tian-w.cn

PHP:  PHP_OS;  phpversion();
来源：http://tgo.ivvv.top

JS:   process.platform;  process.version
来源：http://nnp.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://njt.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vxl.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ssc.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zke.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hqs.wangdashe.top

================================================================================
来源：http://gap.tianlin.xyz

N. 数据结构与算法
来源：http://gjy.fzhhl.top

================================================================================
来源：http://tct.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://bne.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xww.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ksc.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fcw.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgs.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tiq.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://zpz.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://far.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qed.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://wau.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ilr.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lsc.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://urf.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nob.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ikw.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://wey.yj20258.top

Ruby: arr.sort
来源：http://xzj.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oda.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://hlv.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uyr.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://iqu.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqx.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ftw.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://spj.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vlv.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxf.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ubj.zhixingplan.top

[N04] 斐波那契数列
来源：http://ftu.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jjb.sjlbkw.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xzb.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wpq.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpt.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xxz.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uba.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rep.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ydj.fanxiaobao.xyz

[N05] 最大公约数
来源：http://vmd.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://vnw.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sqx.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpn.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yij.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://njg.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://crf.sufxvd.cn

Ruby: a.gcd(b)
来源：http://diy.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wdv.dashuyun.cn

[N06] 判断回文字符串
来源：http://ido.birdmap.top

Py:   s == s[::-1]
来源：http://yxu.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://lyh.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://lqz.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://dpx.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://glp.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://pbr.chenzaomai.com

Ruby: s == s.reverse
来源：http://wka.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lrc.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://php.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sit.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dtv.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zct.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://uyp.haohaochexian.top

Java: // 手写 HashMap
来源：http://nbs.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://yvp.sweek.top

Ruby: // 手写 Hash
来源：http://gmo.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://clk.zhixingplan.top

[N08] 生成全排列
来源：http://nqn.yj202588.top

Py:   itertools.permutations(arr)
来源：http://orl.cheryme.top

PHP:  // 手写递归交换
来源：http://xoo.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://aki.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://xwa.dianchejie.cn

Java: // 手写回溯递归
来源：http://ydq.bbcook.cn

Go:   // 手写回溯递归
来源：http://one.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://uhm.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://pvk.chenjidiqi.icu

[N09] 栈与队列
来源：http://fdr.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rlt.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igl.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bdv.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tht.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://epi.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zpy.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://knj.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://diw.zhoulong.xyz

[N10] 链表节点定义
来源：http://rvc.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ioz.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ckk.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://suk.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zhl.birdmap.top

Java: class Node { int v; Node next; }
来源：http://xqc.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hkv.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://thk.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uha.smart0.xyz

[N11] 二叉树中序遍历
来源：http://wqm.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hof.hcnkem.com

PHP:  // 手写递归函数
来源：http://jtj.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vcd.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cgb.xuanzx.com

Java: // 手写递归
来源：http://duy.hammf.cn

Go:   // 手写递归
来源：http://kun.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dhq.wangdashe.top

C#:   // 手写递归
来源：http://cmz.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gzo.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nbd.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jqv.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blh.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bum.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://upw.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hqb.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://okc.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pzv.shzxlz.cn

================================================================================
来源：http://cqa.redwolf501.top

O. 并发与异步
来源：http://apc.cashguo.top

================================================================================
来源：http://jjg.316326.xyz

[O01] 启动一个线程
来源：http://zeb.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wcg.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ett.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ggi.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://wfm.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://tkx.gzhubu.top

Go:   go f()
来源：http://pcj.cdnleiting.top

Ruby: Thread.new { f }
来源：http://rlj.gzhubu.top

C#:   Task.Run(() => F());
来源：http://woc.vehdjk.com

[O02] 使用线程池
来源：http://lhn.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cwf.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kzv.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://zxd.jianghu66.top

TS:   // worker_threads 线程池
来源：http://msf.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ojg.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kiw.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gnm.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tse.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://oex.guowangkeji.top

Py:   with lock: shared += 1
来源：http://dhf.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://wkx.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rrd.guowangkeji.top

TS:   // 同 JS
来源：http://kba.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://tfd.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ocr.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ogl.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://pwa.sweek.top

[O04] 定义异步函数并等待
来源：http://gjk.sweek.top

Py:   async def f():⏎    await g()
来源：http://bsq.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://atw.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://ope.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ghk.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zks.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dqd.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hrk.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://dam.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://teq.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://fln.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://igy.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://rut.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://aqv.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ltr.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ckz.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://gkb.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dnd.hfpthk.cn

[O06] 使用进程池
来源：http://diq.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dfb.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://caz.tarul.cn

JS:   // child_process / cluster 模块
来源：http://wtn.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://nzn.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lsi.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tgu.birdmap.top

Ruby: // fork 块
来源：http://cxi.kuanghao11.cn

C#:   Parallel.For
来源：http://ree.gogol.net.cn

================================================================================
来源：http://jgt.ydjk.org.cn

P. 常用工具函数
来源：http://kme.yonumen.top

================================================================================
来源：http://pbg.zhoulong.xyz

[P01] 生成 UUID
来源：http://czg.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://spg.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bjs.xinyue.icu

JS:   crypto.randomUUID()
来源：http://eza.pycfn.com

TS:   crypto.randomUUID()
来源：http://dzq.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://rug.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://xee.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://eba.cashguo.top


<!-- 参考信息 -->