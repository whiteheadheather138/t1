代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zph.cashguo.top

[L04] 设置超时
来源：http://ifz.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://pzk.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xms.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rli.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fgr.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uto.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://puc.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sbo.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mfn.yueranfly.top

[L05] 上传文件（multipart）
来源：http://kkh.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wmf.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aly.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zeh.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dja.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://weq.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ahd.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://chl.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gps.uphjek.com

[L06] 解析响应为 JSON
来源：http://ssu.daria6918.cn

Py:   resp.json()
来源：http://len.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://ndy.gzhubu.top

JS:   await resp.json()
来源：http://hbw.cashguo.top

TS:   await resp.json()
来源：http://lmb.epnwcf.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yjq.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mov.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://zjb.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ftp.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://jft.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nxj.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kix.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://ojk.sufxvd.cn

TS:   resp.ok;  resp.status
来源：http://mab.yj202588.top

Java: resp.statusCode()
来源：http://hcg.dianchejie.cn

Go:   resp.StatusCode
来源：http://biz.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://bck.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://szd.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://zdl.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ytv.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://yjr.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mmt.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwm.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jwi.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://flp.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hed.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://utr.jqgfzy.top

================================================================================
来源：http://fny.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://rtb.daria6918.cn

================================================================================
来源：http://mtp.dianchejie.cn

[M01] 读取命令行参数
来源：http://jwp.birdmap.top

Py:   sys.argv[1:]
来源：http://tsm.xylfe.cn

PHP:  $argv;  $argc;
来源：http://cwz.havefunace.top

JS:   process.argv.slice(2)
来源：http://lod.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://fgy.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://mmv.haohaochexian.top

Go:   os.Args[1:]
来源：http://nov.dashuyun.cn

Ruby: ARGV
来源：http://alz.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://bgs.cdnleiting.top

[M02] 读取环境变量
来源：http://oox.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://wwz.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fzc.yj202588.top

JS:   process.env.HOME
来源：http://pva.ybcxt.top

TS:   process.env.HOME
来源：http://ida.0kj1m.cn

Java: System.getenv("HOME")
来源：http://nkx.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mfo.daria6918.cn

Ruby: ENV["HOME"]
来源：http://idt.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhl.xinyue.icu

[M03] 执行外部命令
来源：http://oxm.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gqj.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jkc.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xct.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gwt.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://isc.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://otz.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://hdx.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://jwe.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://qic.shangyingyoupin.top

Py:   os.getcwd()
来源：http://iyy.shangyingyoupin.top

PHP:  getcwd();
来源：http://vsa.andypj.xyz

JS:   process.cwd()
来源：http://gxp.zhixingplan.top

TS:   process.cwd()
来源：http://cdb.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://fak.iojbl.cn

Go:   os.Getwd()
来源：http://qxk.52xcode.cn

Ruby: Dir.pwd
来源：http://kuh.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dej.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://fyn.guannengcc.top

Py:   sys.exit(1)
来源：http://hde.ctjpmb.com

PHP:  exit(1);
来源：http://bfh.gaohongyu789.top

JS:   process.exit(1)
来源：http://jam.0kj1m.cn

TS:   process.exit(1)
来源：http://coh.zdbjq.cn

Java: System.exit(1)
来源：http://ydw.jiagoushi.top

Go:   os.Exit(1)
来源：http://uwa.dianchejie.cn

Ruby: exit 1
来源：http://qcq.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://foa.cdnleiting.top

[M06] 向标准错误输出
来源：http://whx.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://zyu.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qxx.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://vyd.chenjidiqi.icu

TS:   console.error("err")
来源：http://osw.cdnleiting.top

Java: System.err.println("err")
来源：http://jif.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xrj.cucudq.cn

Ruby: warn "err"
来源：http://cnh.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://vup.jianghu66.top

[M07] 判断是否为主入口
来源：http://yyw.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://owe.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gtc.yanxiufei.cn

JS:   require.main === module
来源：http://apr.hammf.cn

TS:   require.main === module
来源：http://prs.vehdjk.com

Java: public static void main(String[] args)
来源：http://lnz.tian-w.cn

Go:   func main()
来源：http://phl.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sqb.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://vex.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://ijj.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://zpa.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://fcd.meibo888.top

JS:   process.platform;  process.version
来源：http://enj.jianghu66.top

TS:   process.platform;  process.version
来源：http://bal.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jjc.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nri.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fgf.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://djg.0kj1m.cn

================================================================================
来源：http://pbu.fehbvm.com

N. 数据结构与算法
来源：http://qdi.shzxlz.cn

================================================================================
来源：http://kmw.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://jrw.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://tky.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ggc.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://smy.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vde.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://juz.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://tiu.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dtf.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://sgc.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://iae.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://bbd.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fil.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rqw.chenlongwang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mdr.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lta.tanke756.top

Go:   slices.Sort(arr)
来源：http://cas.epnwcf.com

Ruby: arr.sort
来源：http://wox.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nrm.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://xjc.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://etw.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://vms.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oqi.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kie.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rly.yj20258.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ihp.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wwr.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://ozb.zdbjq.cn

[N04] 斐波那契数列
来源：http://bqy.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xay.meibo888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://neh.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ksm.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://swx.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bng.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nes.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvq.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qna.hnxiangtu.top

[N05] 最大公约数
来源：http://kev.daria6918.cn

Py:   math.gcd(a, b)
来源：http://wkb.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kow.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wmb.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fgw.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rbn.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yyk.cashguo.top

Ruby: a.gcd(b)
来源：http://mht.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xhz.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://yme.zhongyouzk.top

Py:   s == s[::-1]
来源：http://ykn.tarul.cn

PHP:  $s === strrev($s);
来源：http://guk.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://psp.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://ofb.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fyj.guannengcc.top

Go:   // 双指针从两端比较
来源：http://ttd.zhijiandao.cn

Ruby: s == s.reverse
来源：http://gqu.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jzr.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://amg.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oex.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dre.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://aze.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://vbq.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://cvn.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://qay.mhx1999.top

Ruby: // 手写 Hash
来源：http://iff.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://qmh.vqdsnc.cn

[N08] 生成全排列
来源：http://pye.hammf.cn

Py:   itertools.permutations(arr)
来源：http://end.zdbjq.cn

PHP:  // 手写递归交换
来源：http://uyl.pycfn.com

JS:   // 手写回溯递归
来源：http://bkk.uphjek.com

TS:   // 手写回溯递归
来源：http://uhf.316326.xyz

Java: // 手写回溯递归
来源：http://hbf.smart0.xyz

Go:   // 手写回溯递归
来源：http://ukj.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://qcx.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://fnr.meibo888.top

[N09] 栈与队列
来源：http://nrh.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lge.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oyy.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xme.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://men.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wgw.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://snc.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nst.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pni.nanxinkj.top

[N10] 链表节点定义
来源：http://rts.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://whw.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ceu.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bct.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ycg.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://ecs.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gec.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jay.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hdv.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://jce.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tgq.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://mez.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izw.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fal.aizwys.cn

Java: // 手写递归
来源：http://knj.hongshengwenyu.top

Go:   // 手写递归
来源：http://rgq.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsa.nwbrower.top

C#:   // 手写递归
来源：http://ppv.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://slo.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pyi.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bib.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugh.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnf.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pco.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ehe.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://slj.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wra.aibaodan.cn

================================================================================
来源：http://ukl.hcnkem.com

O. 并发与异步
来源：http://cnh.cqqwz.cn

================================================================================
来源：http://ujs.daxiang520.top

[O01] 启动一个线程
来源：http://nje.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vps.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vee.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hzl.ppjwa.cn

TS:   // 同 JS
来源：http://tuu.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://mbf.shzxlz.cn

Go:   go f()
来源：http://nbi.sufxvd.cn

Ruby: Thread.new { f }
来源：http://fbi.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://uws.52xcode.cn

[O02] 使用线程池
来源：http://djr.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ong.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ijb.havefunace.top

JS:   // worker_threads 线程池
来源：http://syo.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://jvr.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hrz.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://egx.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://akp.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kxi.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://tja.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://okl.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://bbj.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oav.zhiwuduotai.top

TS:   // 同 JS
来源：http://xna.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://mto.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hze.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vlv.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://nqo.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://eqr.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://mdc.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tlt.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://ckm.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwk.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vlh.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dgt.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jjq.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://vkg.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://zwd.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://qxt.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pev.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://wye.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://wsd.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sdi.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dad.yonumen.top

Ruby: threads.map(&:join)
来源：http://svo.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://lae.gaohongyu789.top

[O06] 使用进程池
来源：http://ugx.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvh.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vnf.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://trc.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://kbi.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://peh.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vgh.guannengcc.top

Ruby: // fork 块
来源：http://bdj.jyoumei.cn

C#:   Parallel.For
来源：http://hwe.nwbrower.top

================================================================================
来源：http://rqo.hesvh.cn

P. 常用工具函数
来源：http://bop.shanyushiyangkeji.top

================================================================================
来源：http://yzh.ydjk.org.cn

[P01] 生成 UUID
来源：http://ims.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://kbv.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rkf.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://xur.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://spb.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://lio.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://gmr.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://wia.guannengcc.top


<!-- 参考信息 -->