代发 wailian999

[L03] 设置自定义请求头
来源：http://xhq.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ler.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://smh.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyh.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wid.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lwx.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bkf.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://acd.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hom.aizwys.cn

[L04] 设置超时
来源：http://aza.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://jkl.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ohs.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rcp.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byj.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gon.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zpe.shanyushiyangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kto.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hce.zdbjq.cn

[L05] 上传文件（multipart）
来源：http://amz.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lkf.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kxy.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pyr.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mla.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://czn.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iqa.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gsl.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sis.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://cem.bjfxy.top

Py:   resp.json()
来源：http://pls.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://bfh.jinghuilouyu.cn

JS:   await resp.json()
来源：http://lfr.ybcxt.top

TS:   await resp.json()
来源：http://gfk.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xfx.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jab.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://csp.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jbh.shuidangran.top

[L07] 处理 HTTP 状态码
来源：http://dkg.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nra.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jfo.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://wij.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://rbh.ybcxt.top

Java: resp.statusCode()
来源：http://hnv.daxiang520.top

Go:   resp.StatusCode
来源：http://onc.haohaochexian.top

Ruby: resp.code.to_i
来源：http://ibo.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://lxc.aibaodan.cn

[L08] 并发请求多个地址
来源：http://pen.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hdu.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://jmh.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwc.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yye.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://znt.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hdc.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jzf.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ser.gaohongyu789.top

================================================================================
来源：http://lko.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://qtp.hcnkem.com

================================================================================
来源：http://muv.jlsjyb.cn

[M01] 读取命令行参数
来源：http://tud.sysykeji.top

Py:   sys.argv[1:]
来源：http://bdi.ydzc1.top

PHP:  $argv;  $argc;
来源：http://ppa.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://bfk.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://lou.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://rzi.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://djg.zdbjq.cn

Ruby: ARGV
来源：http://khj.yj202588.top

C#:   args 数组（Main 方法参数）
来源：http://lef.ybcxt.top

[M02] 读取环境变量
来源：http://cmd.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://idq.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qbz.yj202588.top

JS:   process.env.HOME
来源：http://tws.xuanzx.com

TS:   process.env.HOME
来源：http://tbj.yangfankeji.com

Java: System.getenv("HOME")
来源：http://tvr.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ktx.andypj.xyz

Ruby: ENV["HOME"]
来源：http://ohf.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uts.cucudq.cn

[M03] 执行外部命令
来源：http://bbt.hfpthk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iyd.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gth.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ptu.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dnk.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://luv.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://phm.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://kws.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://yzd.gotoacloud.top

[M04] 获取当前工作目录
来源：http://rah.zhijiandao.cn

Py:   os.getcwd()
来源：http://rdi.gzhubu.top

PHP:  getcwd();
来源：http://ine.aibaodan.cn

JS:   process.cwd()
来源：http://wql.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://qlz.haohaochexian.top

Java: Path.of("").toAbsolutePath()
来源：http://nmb.hcnkem.com

Go:   os.Getwd()
来源：http://bra.0kj1m.cn

Ruby: Dir.pwd
来源：http://vtj.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://cms.wangshuangyany.cn

[M05] 设置退出码
来源：http://xqn.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://mwd.daxiang520.top

PHP:  exit(1);
来源：http://xcx.iojbl.cn

JS:   process.exit(1)
来源：http://qsh.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://sgb.xuanzx.com

Java: System.exit(1)
来源：http://dnn.fzhhl.top

Go:   os.Exit(1)
来源：http://huf.kuanghao11.cn

Ruby: exit 1
来源：http://wsx.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bsg.guannengcc.top

[M06] 向标准错误输出
来源：http://lfl.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://tso.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ogz.jinqigfzy.top

JS:   console.error("err")
来源：http://ncw.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://lor.jinqigfzy.top

Java: System.err.println("err")
来源：http://atn.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qqz.iojbl.cn

Ruby: warn "err"
来源：http://mty.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ahd.fzhhl.top

[M07] 判断是否为主入口
来源：http://yuc.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://nsi.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ttu.ybcxt.top

JS:   require.main === module
来源：http://zkl.yongpay.top

TS:   require.main === module
来源：http://xfd.tanke756.top

Java: public static void main(String[] args)
来源：http://qln.shuidangran.top

Go:   func main()
来源：http://mfh.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jwo.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://ykz.tanke756.top

[M08] 获取系统与运行时信息
来源：http://jda.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://lcn.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://sdv.uphjek.com

JS:   process.platform;  process.version
来源：http://vzg.snrcjt.cn

TS:   process.platform;  process.version
来源：http://fzl.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpn.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gvd.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tig.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lxi.ydjk.org.cn

================================================================================
来源：http://ghx.gaohongyu789.top

N. 数据结构与算法
来源：http://zvm.pycfn.com

================================================================================
来源：http://cmx.uphjek.com

[N01] 二分查找（有序数组）
来源：http://ujb.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://usi.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yiw.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zcr.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aac.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://amj.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://sup.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyf.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://ira.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://rgm.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://tlm.yanxiufei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xeq.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hrc.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kmk.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ncb.tanke756.top

Go:   slices.Sort(arr)
来源：http://fza.svipenyu.cn

Ruby: arr.sort
来源：http://vrs.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://amr.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://lcm.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://agv.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://tns.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://epu.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tgg.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oec.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iiw.chenlongwang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xvb.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gxu.haohaochexian.top

[N04] 斐波那契数列
来源：http://zkk.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://erg.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://out.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aqd.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tur.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cky.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qtn.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zba.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zvj.yfazqb.com

[N05] 最大公约数
来源：http://era.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://xip.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fxn.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cbj.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfm.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hji.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qjr.sufxvd.cn

Ruby: a.gcd(b)
来源：http://sei.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ynb.zhoulong.xyz

[N06] 判断回文字符串
来源：http://olg.hammf.cn

Py:   s == s[::-1]
来源：http://bbq.sxryk.cn

PHP:  $s === strrev($s);
来源：http://irg.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://zuv.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://zmi.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hod.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://mep.redwolf501.top

Ruby: s == s.reverse
来源：http://tpn.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nji.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://pbk.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://avt.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hoh.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vom.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://usl.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://rcd.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://slr.fktsv.cn

Ruby: // 手写 Hash
来源：http://pbf.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tyn.chenjidiqi.icu

[N08] 生成全排列
来源：http://ucs.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://rxl.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://wki.jyoumei.cn

JS:   // 手写回溯递归
来源：http://ieo.yuxming.cn

TS:   // 手写回溯递归
来源：http://nqp.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://kve.tarul.cn

Go:   // 手写回溯递归
来源：http://bxq.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://zns.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://gbu.hnxiangtu.top

[N09] 栈与队列
来源：http://ovj.c1oappe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ywq.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znm.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lbt.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qdd.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oxa.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wze.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aim.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lea.svipenyu.cn

[N10] 链表节点定义
来源：http://pbp.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pae.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ndr.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bxn.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqo.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://emo.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://dgl.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ppg.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jfp.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://zdc.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fzm.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://wng.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ahk.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wli.jlsjyb.cn

Java: // 手写递归
来源：http://dxy.zhixingplan.top

Go:   // 手写递归
来源：http://wmy.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wjf.vehdjk.com

C#:   // 手写递归
来源：http://xup.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oan.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ima.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lmh.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ohm.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bql.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vdc.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqh.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jqn.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wpp.nanxuanxn.top

================================================================================
来源：http://ahb.c1oappe.top

O. 并发与异步
来源：http://mvt.zycfv.cn

================================================================================
来源：http://zmd.yonumen.top

[O01] 启动一个线程
来源：http://gka.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://afr.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://spz.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fur.ybcxt.top

TS:   // 同 JS
来源：http://uph.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://mcc.uphjek.com

Go:   go f()
来源：http://ssk.hammf.cn

Ruby: Thread.new { f }
来源：http://jpb.fengsongda.top

C#:   Task.Run(() => F());
来源：http://szk.jinqigfzy.top

[O02] 使用线程池
来源：http://kgy.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ucr.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://byb.fktsv.cn

JS:   // worker_threads 线程池
来源：http://akq.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://czz.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://uoo.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wsf.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pvi.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wga.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://xga.zycfv.cn

Py:   with lock: shared += 1
来源：http://ntk.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://zxp.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lej.nanxinkj.top

TS:   // 同 JS
来源：http://fpi.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://clr.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dlg.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hkf.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://onw.hnqzz.top

[O04] 定义异步函数并等待
来源：http://ohx.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://hpv.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vjm.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://koc.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pgv.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fud.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bgo.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rbh.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://yra.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://vhf.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://jcv.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cyy.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://bza.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://vjl.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yaa.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nrl.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://kql.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://fop.dashuyun.cn

[O06] 使用进程池
来源：http://wqk.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dvo.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fel.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://wih.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://non.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yrm.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dqz.fzhhl.top

Ruby: // fork 块
来源：http://evx.52xcode.cn

C#:   Parallel.For
来源：http://jpo.hammf.cn

================================================================================
来源：http://exg.feifeiyinyue.top

P. 常用工具函数
来源：http://zfc.feifeiyinyue.top

================================================================================
来源：http://pqc.dianchejie.cn


<!-- 参考信息 -->