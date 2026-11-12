代发 wailian999

[L03] 设置自定义请求头
来源：http://iur.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hqk.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hkh.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfe.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amk.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jhk.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lvt.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jla.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ida.redwolf501.top

[L04] 设置超时
来源：http://igu.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://bvi.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xyi.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lxc.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhr.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bqn.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pyi.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://itc.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ycg.0kj1m.cn

[L05] 上传文件（multipart）
来源：http://aag.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yck.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aos.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xnn.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mgp.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ayw.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rjb.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://avw.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eag.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://chd.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://sqz.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://wul.cqqwz.cn

JS:   await resp.json()
来源：http://lqv.yj202588.top

TS:   await resp.json()
来源：http://vmo.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gue.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://utx.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://trk.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cgd.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://vam.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vgy.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pkn.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://bxr.meibo888.top

TS:   resp.ok;  resp.status
来源：http://uwj.aizwys.cn

Java: resp.statusCode()
来源：http://fqr.xylfe.cn

Go:   resp.StatusCode
来源：http://uqx.0kj1m.cn

Ruby: resp.code.to_i
来源：http://nsy.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://wrr.9152youxi.cn

[L08] 并发请求多个地址
来源：http://dfr.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jyw.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://rvk.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dha.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jtm.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hye.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cfa.chenzaomai.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xoj.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vwh.epnwcf.com

================================================================================
来源：http://sow.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://zls.hnqzz.top

================================================================================
来源：http://gtt.zhixingplan.top

[M01] 读取命令行参数
来源：http://aoq.ydzc1.top

Py:   sys.argv[1:]
来源：http://mnn.316326.xyz

PHP:  $argv;  $argc;
来源：http://rrw.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://qtr.aizwys.cn

TS:   process.argv.slice(2)
来源：http://rpb.sweek.top

Java: args 数组（main 方法参数）
来源：http://lmp.iojbl.cn

Go:   os.Args[1:]
来源：http://zef.meibo888.top

Ruby: ARGV
来源：http://bii.jiagoushi.top

C#:   args 数组（Main 方法参数）
来源：http://kab.jqgufenzy.top

[M02] 读取环境变量
来源：http://ueu.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://htu.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zdv.nwbrower.top

JS:   process.env.HOME
来源：http://mvl.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://pvj.chenlongwang.top

Java: System.getenv("HOME")
来源：http://geq.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iki.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://grh.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://elf.meibo888.top

[M03] 执行外部命令
来源：http://wwq.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://umf.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dee.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://leo.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sab.zdbjq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vpp.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wrc.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://xwi.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://uej.zdqjudy.top

[M04] 获取当前工作目录
来源：http://xdn.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://une.ybcxt.top

PHP:  getcwd();
来源：http://cba.tian-w.cn

JS:   process.cwd()
来源：http://mbs.ehwqpu.com

TS:   process.cwd()
来源：http://lmv.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://wsf.mhx1999.top

Go:   os.Getwd()
来源：http://wbw.quarkkingdee.top

Ruby: Dir.pwd
来源：http://udc.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qcv.guowangkeji.top

[M05] 设置退出码
来源：http://mig.jinqigufen.top

Py:   sys.exit(1)
来源：http://bwu.ppjwa.cn

PHP:  exit(1);
来源：http://mqt.316326.xyz

JS:   process.exit(1)
来源：http://mzv.guowangkeji.top

TS:   process.exit(1)
来源：http://xwt.guowangkeji.top

Java: System.exit(1)
来源：http://dcj.sufxvd.cn

Go:   os.Exit(1)
来源：http://gvi.aizwys.cn

Ruby: exit 1
来源：http://xmo.gzhubu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aio.c1oappe.top

[M06] 向标准错误输出
来源：http://fiu.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://zvr.shangyingyoupin.top

PHP:  fwrite(STDERR, "err\n");
来源：http://won.yfazqb.com

JS:   console.error("err")
来源：http://usb.daria6918.cn

TS:   console.error("err")
来源：http://zme.guannengcc.top

Java: System.err.println("err")
来源：http://vhc.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qkd.bbcook.cn

Ruby: warn "err"
来源：http://qje.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://oxn.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://xvg.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://mpc.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pfh.snrcjt.cn

JS:   require.main === module
来源：http://klq.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://oun.yj20258.top

Java: public static void main(String[] args)
来源：http://njn.hcnkem.com

Go:   func main()
来源：http://eii.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://puj.yj20258.top

C#:   static void Main(string[] args)
来源：http://maz.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://iqc.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://dlx.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://ggm.gzhubu.top

JS:   process.platform;  process.version
来源：http://ans.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://fjq.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pic.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zzt.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bcn.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nvh.zhongyouzk.top

================================================================================
来源：http://aev.jianghu66.top

N. 数据结构与算法
来源：http://vuf.hfpthk.cn

================================================================================
来源：http://nli.yonumen.top

[N01] 二分查找（有序数组）
来源：http://ael.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://lom.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://unx.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkh.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkh.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://anf.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://fjf.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lxh.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uow.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://lmz.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://aix.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fzz.yonumen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://esv.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cjg.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mpo.yj20258888.top

Go:   slices.Sort(arr)
来源：http://uyb.cashguo.top

Ruby: arr.sort
来源：http://iug.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fod.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://qgg.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wmr.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://xqe.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btp.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ast.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vge.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxd.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fae.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vrr.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://slg.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qdu.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbv.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knw.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbt.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jed.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrg.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icb.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gmp.aibaodan.cn

[N05] 最大公约数
来源：http://vfh.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://xdq.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ksq.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bwq.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyt.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbc.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zwu.fengsongda.top

Ruby: a.gcd(b)
来源：http://qxa.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rob.ehwqpu.com

[N06] 判断回文字符串
来源：http://yfz.uphjek.com

Py:   s == s[::-1]
来源：http://tdw.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://vjc.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://pqd.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://jvn.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wit.yongpay.top

Go:   // 双指针从两端比较
来源：http://cja.sufxvd.cn

Ruby: s == s.reverse
来源：http://cyl.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xho.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://pez.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yce.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yhu.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vys.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://uck.nanxuanxn.top

Java: // 手写 HashMap
来源：http://sgo.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://ygc.sysykeji.top

Ruby: // 手写 Hash
来源：http://puh.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://lwh.ctjpmb.com

[N08] 生成全排列
来源：http://hcz.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://ibj.yj20258.top

PHP:  // 手写递归交换
来源：http://lns.sufxvd.cn

JS:   // 手写回溯递归
来源：http://uhi.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://shc.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://aam.yongpay.top

Go:   // 手写回溯递归
来源：http://tcm.cheryme.top

Ruby: arr.permutation.to_a
来源：http://lin.fehbvm.com

C#:   // 手写回溯递归
来源：http://bnc.cdnleiting.top

[N09] 栈与队列
来源：http://rxs.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tzy.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zxh.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ixx.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xhl.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://osk.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qdg.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qnl.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tcc.havefunace.top

[N10] 链表节点定义
来源：http://lbp.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yag.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cbx.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bsv.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rhb.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://mip.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ico.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qat.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aph.yfazqb.com

[N11] 二叉树中序遍历
来源：http://ogb.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ywy.smart0.xyz

PHP:  // 手写递归函数
来源：http://qkq.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jxh.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hzb.sweek.top

Java: // 手写递归
来源：http://wyu.andypj.xyz

Go:   // 手写递归
来源：http://lac.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jsk.zhiwuduotai.top

C#:   // 手写递归
来源：http://fxy.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vrj.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xyf.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gao.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eny.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzb.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gsz.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cqq.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vsk.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wzr.yueranfly.top

================================================================================
来源：http://upy.xinyue.icu

O. 并发与异步
来源：http://qyk.mhx1999.top

================================================================================
来源：http://drj.hcnkem.com

[O01] 启动一个线程
来源：http://txy.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vzi.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yui.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aah.sysykeji.top

TS:   // 同 JS
来源：http://qeu.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://wyc.jiagoushi.top

Go:   go f()
来源：http://cpz.fzhhl.top

Ruby: Thread.new { f }
来源：http://tbz.jinghuilouyu.cn

C#:   Task.Run(() => F());
来源：http://ird.jqgfzy.top

[O02] 使用线程池
来源：http://ttj.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fbh.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bsu.ivvv.top

JS:   // worker_threads 线程池
来源：http://enp.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ass.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://njq.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wqx.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yze.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zcg.hammf.cn

[O03] 加锁保护共享数据
来源：http://qsa.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://jgb.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://pug.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ceo.bjfxy.top

TS:   // 同 JS
来源：http://kue.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://rnw.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dcu.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://muf.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://iwa.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://grb.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://oox.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ddq.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://sgf.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rda.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iia.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://daf.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yoh.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://fyc.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://dvm.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://npi.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zlm.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://cxt.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://iat.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cex.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cwh.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://glx.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pdk.guowangkeji.top

[O06] 使用进程池
来源：http://vrg.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jlo.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://grm.ivvv.top

JS:   // child_process / cluster 模块
来源：http://hzb.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://bit.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cms.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qvw.kuanghao11.cn

Ruby: // fork 块
来源：http://asr.yj20258888.top

C#:   Parallel.For
来源：http://cqz.tian-w.cn

================================================================================
来源：http://ivc.yuxming.cn

P. 常用工具函数
来源：http://cwr.vqdsnc.cn

================================================================================
来源：http://hni.jinyuanbaomall.cn


<!-- 参考信息 -->