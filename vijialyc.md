代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jkj.haohaochexian.top

[L04] 设置超时
来源：http://wgp.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://ohq.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lqw.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfv.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wsv.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jwo.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hqf.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tax.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qmr.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://azs.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fzi.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uuk.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hpu.vqdsnc.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wyy.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://reb.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://udu.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pjz.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lju.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://mnd.hnxiangtu.top

Py:   resp.json()
来源：http://odn.sweek.top

PHP:  json_decode($body, true);
来源：http://kzv.zdbjq.cn

JS:   await resp.json()
来源：http://wfo.iojbl.cn

TS:   await resp.json()
来源：http://dic.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://chw.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jug.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://box.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kzh.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://min.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xbc.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gqm.pycfn.com

JS:   resp.ok;  resp.status
来源：http://aek.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://uly.jianghu66.top

Java: resp.statusCode()
来源：http://ktu.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://shj.cdnleiting.top

Ruby: resp.code.to_i
来源：http://urh.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://acm.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://tzy.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lat.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://dfh.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xgp.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mul.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xsd.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uqg.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ogc.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://grf.epnwcf.com

================================================================================
来源：http://jum.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://ksx.cheryme.top

================================================================================
来源：http://tnw.fzhhl.top

[M01] 读取命令行参数
来源：http://tak.hywenlv.cn

Py:   sys.argv[1:]
来源：http://uez.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://emu.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://deo.wangdashe.top

TS:   process.argv.slice(2)
来源：http://dej.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://mdb.jianghu66.top

Go:   os.Args[1:]
来源：http://pdb.ehwqpu.com

Ruby: ARGV
来源：http://tsf.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://ktc.hongshengwenyu.top

[M02] 读取环境变量
来源：http://end.yongpay.top

Py:   os.environ.get("HOME")
来源：http://cfn.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nsv.jianghu66.top

JS:   process.env.HOME
来源：http://ruw.shangyingyoupin.top

TS:   process.env.HOME
来源：http://vdb.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://nyh.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zhg.mhx1999.top

Ruby: ENV["HOME"]
来源：http://sxt.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://epi.shangyingyoupin.top

[M03] 执行外部命令
来源：http://jil.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oja.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://srw.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://whs.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gov.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://btq.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zrj.yuxming.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tju.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://vpb.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://kep.jyoumei.cn

Py:   os.getcwd()
来源：http://fwt.jinghuilouyu.cn

PHP:  getcwd();
来源：http://opr.shangyingyoupin.top

JS:   process.cwd()
来源：http://vjj.aizwys.cn

TS:   process.cwd()
来源：http://ldp.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://pbb.jyoumei.cn

Go:   os.Getwd()
来源：http://llt.xylfe.cn

Ruby: Dir.pwd
来源：http://ekr.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://jvn.fehbvm.com

[M05] 设置退出码
来源：http://pcf.gaohongyu789.top

Py:   sys.exit(1)
来源：http://yhf.daria6918.cn

PHP:  exit(1);
来源：http://kcj.redwolf501.top

JS:   process.exit(1)
来源：http://yvs.zdqjudy.top

TS:   process.exit(1)
来源：http://shd.vehdjk.com

Java: System.exit(1)
来源：http://bii.chenzaomai.com

Go:   os.Exit(1)
来源：http://bjo.pengpengdd.cyou

Ruby: exit 1
来源：http://ppp.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://svf.yfazqb.com

[M06] 向标准错误输出
来源：http://ujt.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://fom.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ybb.ivvv.top

JS:   console.error("err")
来源：http://vkc.gogol.net.cn

TS:   console.error("err")
来源：http://rxx.zhengqikj.top

Java: System.err.println("err")
来源：http://ctt.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://moj.zycfv.cn

Ruby: warn "err"
来源：http://rdp.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://yik.52xcode.cn

[M07] 判断是否为主入口
来源：http://isq.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://wxx.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opy.hysaishi.cn

JS:   require.main === module
来源：http://qpl.xinyue.icu

TS:   require.main === module
来源：http://ukl.ivvv.top

Java: public static void main(String[] args)
来源：http://xua.yangfankeji.com

Go:   func main()
来源：http://qtm.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://btf.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://zqe.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://vla.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://xgv.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://mrx.daria6918.cn

JS:   process.platform;  process.version
来源：http://hwl.nanxinkj.top

TS:   process.platform;  process.version
来源：http://jhw.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wgi.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lhi.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wgk.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://btr.cashguo.top

================================================================================
来源：http://ieb.tanke756.top

N. 数据结构与算法
来源：http://jwp.jinyuanbaomall.cn

================================================================================
来源：http://ops.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://goa.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://mge.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lsd.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dmp.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xft.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jpr.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://rjk.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pof.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://wvp.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://rus.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://cjy.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hne.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qzq.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pse.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ike.hammf.cn

Go:   slices.Sort(arr)
来源：http://jyo.hfpthk.cn

Ruby: arr.sort
来源：http://ypa.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xxx.pycfn.com

[N03] 快速排序（分治示例）
来源：http://ugz.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dlo.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://ika.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eas.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvb.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rmq.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mxv.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ckn.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://zky.svipenyu.cn

[N04] 斐波那契数列
来源：http://tqz.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xsp.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hrk.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rmh.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kjs.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsj.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ehg.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mnb.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ljv.hnqzz.top

[N05] 最大公约数
来源：http://gpz.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://kxq.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xmr.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ebj.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://myr.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://soc.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mfy.zycfv.cn

Ruby: a.gcd(b)
来源：http://glc.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tfb.havefunace.top

[N06] 判断回文字符串
来源：http://ibm.ydzc1.top

Py:   s == s[::-1]
来源：http://urd.hnqzz.top

PHP:  $s === strrev($s);
来源：http://yic.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://duc.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://snt.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lea.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://ooc.quarkkingdee.top

Ruby: s == s.reverse
来源：http://swg.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pji.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://sgu.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rry.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xvf.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://hym.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://nwr.haohaochexian.top

Java: // 手写 HashMap
来源：http://bnw.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://cqa.xuanzx.com

Ruby: // 手写 Hash
来源：http://wob.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kvl.dianchejie.cn

[N08] 生成全排列
来源：http://pcy.316326.xyz

Py:   itertools.permutations(arr)
来源：http://apf.bjfxy.top

PHP:  // 手写递归交换
来源：http://aqj.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://eev.chenlongwang.top

TS:   // 手写回溯递归
来源：http://dnr.ppjwa.cn

Java: // 手写回溯递归
来源：http://uss.gzhubu.top

Go:   // 手写回溯递归
来源：http://wcx.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://eka.yj202588.top

C#:   // 手写回溯递归
来源：http://crz.wangdashe.top

[N09] 栈与队列
来源：http://vjn.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xlk.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cko.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rrp.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gln.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xdh.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gcm.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nnc.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnl.aibaodan.cn

[N10] 链表节点定义
来源：http://chb.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hwg.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://epw.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mlj.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://int.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://lrh.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://luj.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ssi.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://amq.cucudq.cn

[N11] 二叉树中序遍历
来源：http://odk.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uic.vehdjk.com

PHP:  // 手写递归函数
来源：http://zku.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dzs.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ejp.cucudq.cn

Java: // 手写递归
来源：http://gng.jinqigfzy.top

Go:   // 手写递归
来源：http://rxj.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fbj.jinqigufen.top

C#:   // 手写递归
来源：http://jhy.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mkr.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lxa.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://neo.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://prc.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ibc.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ubu.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kdh.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyw.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bzm.meibo888.top

================================================================================
来源：http://vkd.hcnkem.com

O. 并发与异步
来源：http://rhr.xingfuxueyuan.xyz

================================================================================
来源：http://ayq.quarkkingdee.top

[O01] 启动一个线程
来源：http://wrf.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uwq.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ahm.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xmg.ehwqpu.com

TS:   // 同 JS
来源：http://euv.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://sfi.sufxvd.cn

Go:   go f()
来源：http://ehe.316326.xyz

Ruby: Thread.new { f }
来源：http://nkp.hesvh.cn

C#:   Task.Run(() => F());
来源：http://boe.jinghuilouyu.cn

[O02] 使用线程池
来源：http://pie.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rfb.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ufu.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://bms.xuanzx.com

TS:   // worker_threads 线程池
来源：http://kuu.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://tme.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ezv.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pin.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gzd.hammf.cn

[O03] 加锁保护共享数据
来源：http://tgj.gotoacloud.top

Py:   with lock: shared += 1
来源：http://wdc.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://prp.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ntf.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://nyj.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://osz.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://crp.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dpu.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://wzv.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://nzd.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://mco.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pys.mhx1999.top

JS:   async function f() { await g(); }
来源：http://utb.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://zgg.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jrg.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kok.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://tby.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://ilx.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://nfn.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://qli.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kjs.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://eyl.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://iia.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xyf.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://inu.smart0.xyz

Ruby: threads.map(&:join)
来源：http://svd.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ust.yuanzhike.top

[O06] 使用进程池
来源：http://ksk.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hyk.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kwn.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://iza.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://gyk.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qmb.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://whz.yongpay.top

Ruby: // fork 块
来源：http://cdw.52xcode.cn

C#:   Parallel.For
来源：http://zhx.hnxiangtu.top

================================================================================
来源：http://qcj.ywan-chungtsiang.top

P. 常用工具函数
来源：http://ova.sysykeji.top

================================================================================
来源：http://qxr.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://niw.tanke756.top

Py:   str(uuid.uuid4())
来源：http://eoc.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mfm.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://lyj.yj20258.top

TS:   crypto.randomUUID()
来源：http://otp.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://nkr.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://hlq.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://dqk.wangdashe.top


<!-- 参考信息 -->