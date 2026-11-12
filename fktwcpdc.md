代发 wailian999

[L03] 设置自定义请求头
来源：http://uqy.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wtt.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://okg.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cuu.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://utx.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ayx.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wre.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsa.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nzw.zhijiandao.cn

[L04] 设置超时
来源：http://fpr.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://gza.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iiz.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jzk.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xem.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vmi.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ysl.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xra.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ede.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://vml.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mym.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sgl.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hbz.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://orl.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://afl.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eah.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pjy.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qrd.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://sec.redwolf501.top

Py:   resp.json()
来源：http://ctp.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://jns.uphjek.com

JS:   await resp.json()
来源：http://lvu.epnwcf.com

TS:   await resp.json()
来源：http://swf.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dcu.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gbq.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://wvt.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zxd.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://afz.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hob.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://php.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://lpd.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://koe.cqqwz.cn

Java: resp.statusCode()
来源：http://jjd.chenzaomai.com

Go:   resp.StatusCode
来源：http://cpx.haohaochexian.top

Ruby: resp.code.to_i
来源：http://dqf.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://wka.ctjpmb.com

[L08] 并发请求多个地址
来源：http://bzi.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mep.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://dxh.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfd.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jmh.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trk.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jzd.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uxh.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fcr.zhijiandao.cn

================================================================================
来源：http://ijx.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://nts.yueranfly.top

================================================================================
来源：http://rgq.daxiang520.top

[M01] 读取命令行参数
来源：http://cri.gogol.net.cn

Py:   sys.argv[1:]
来源：http://azz.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://ewc.xziqi.cn

JS:   process.argv.slice(2)
来源：http://asw.cheryme.top

TS:   process.argv.slice(2)
来源：http://adh.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://xbv.hnxiangtu.top

Go:   os.Args[1:]
来源：http://cui.fehbvm.com

Ruby: ARGV
来源：http://btj.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://ffg.nwbrower.top

[M02] 读取环境变量
来源：http://anl.sweek.top

Py:   os.environ.get("HOME")
来源：http://dbt.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wls.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://osr.havefunace.top

TS:   process.env.HOME
来源：http://ioz.chenzaomai.com

Java: System.getenv("HOME")
来源：http://tmu.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://edd.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://nfe.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://obk.chenlongwang.top

[M03] 执行外部命令
来源：http://clz.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vmn.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sqq.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sov.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mnr.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qqa.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://pke.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vfl.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://dlk.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://yej.zdqjudy.top

Py:   os.getcwd()
来源：http://pka.316326.xyz

PHP:  getcwd();
来源：http://tvv.hfpthk.cn

JS:   process.cwd()
来源：http://bup.uphjek.com

TS:   process.cwd()
来源：http://rvu.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://kig.jyoumei.cn

Go:   os.Getwd()
来源：http://pjh.zycfv.cn

Ruby: Dir.pwd
来源：http://gsx.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://lhh.cheryme.top

[M05] 设置退出码
来源：http://ssa.chenzaomai.com

Py:   sys.exit(1)
来源：http://com.jianghu66.top

PHP:  exit(1);
来源：http://tum.haohaochexian.top

JS:   process.exit(1)
来源：http://kxw.pengpengdd.cyou

TS:   process.exit(1)
来源：http://tih.yangfankeji.com

Java: System.exit(1)
来源：http://hnj.meibo888.top

Go:   os.Exit(1)
来源：http://zbb.yj20258888.top

Ruby: exit 1
来源：http://avp.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cqw.yfazqb.com

[M06] 向标准错误输出
来源：http://bqj.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://xst.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://rgs.hammf.cn

JS:   console.error("err")
来源：http://pts.zhongyouzk.top

TS:   console.error("err")
来源：http://wue.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://ryg.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dzq.pengpengdd.cyou

Ruby: warn "err"
来源：http://byh.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://ukf.redwolf501.top

[M07] 判断是否为主入口
来源：http://bhh.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://ssc.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ssi.pengpengdd.cyou

JS:   require.main === module
来源：http://ins.ivvv.top

TS:   require.main === module
来源：http://arq.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://jsp.andypj.xyz

Go:   func main()
来源：http://vde.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://buy.fzhhl.top

C#:   static void Main(string[] args)
来源：http://nsr.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://zcw.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://urz.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://tny.gzhubu.top

JS:   process.platform;  process.version
来源：http://rew.uphjek.com

TS:   process.platform;  process.version
来源：http://rsf.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://joe.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://niz.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ldy.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ilx.sufxvd.cn

================================================================================
来源：http://smd.snrcjt.cn

N. 数据结构与算法
来源：http://oqz.hongshengwenyu.top

================================================================================
来源：http://fie.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://nec.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hmr.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xru.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksv.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fec.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://yyf.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://uqe.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vti.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://qja.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://klp.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://vnk.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ubm.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://tbu.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hec.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oka.daria6918.cn

Go:   slices.Sort(arr)
来源：http://zzl.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://krb.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bdw.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://ajo.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bvz.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://bhz.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxb.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxl.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://odv.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ujp.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zfh.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://uae.jqgfzy.top

[N04] 斐波那契数列
来源：http://exe.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xkl.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jzu.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kzs.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eob.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://adz.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nmt.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eoo.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mdb.bbcook.cn

[N05] 最大公约数
来源：http://cim.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://sxf.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ine.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lng.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uds.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jyk.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xey.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://boi.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wwf.tian-w.cn

[N06] 判断回文字符串
来源：http://mbr.nanxuanxn.top

Py:   s == s[::-1]
来源：http://ezj.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://ong.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://sfj.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://ofh.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qcu.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://ckz.hywenlv.cn

Ruby: s == s.reverse
来源：http://wpm.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lfb.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://izw.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iff.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://edk.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://aes.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://mqo.jqgufenzy.top

Java: // 手写 HashMap
来源：http://frw.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://cca.xylfe.cn

Ruby: // 手写 Hash
来源：http://vzq.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ckf.nanxinkj.top

[N08] 生成全排列
来源：http://dnt.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://tyh.yj202588.top

PHP:  // 手写递归交换
来源：http://awd.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://gqt.ctjpmb.com

TS:   // 手写回溯递归
来源：http://ijd.aibaodan.cn

Java: // 手写回溯递归
来源：http://ctj.hfpthk.cn

Go:   // 手写回溯递归
来源：http://rom.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://spr.zycfv.cn

C#:   // 手写回溯递归
来源：http://pgj.zhiwuduotai.top

[N09] 栈与队列
来源：http://yhd.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ohw.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uqo.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dln.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lio.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://puv.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dwm.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lxp.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kwv.zhixingplan.top

[N10] 链表节点定义
来源：http://qqr.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fie.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qis.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://trt.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kmr.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://ldx.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://smo.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ung.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qvu.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://rur.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qsh.chenzaomai.com

PHP:  // 手写递归函数
来源：http://njw.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://egw.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nac.hnqzz.top

Java: // 手写递归
来源：http://hjf.chenlongwang.top

Go:   // 手写递归
来源：http://xac.shangyingyoupin.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jas.ehwqpu.com

C#:   // 手写递归
来源：http://kca.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tca.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://asy.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fgi.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fle.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yit.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rgk.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://coj.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xje.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fok.cashguo.top

================================================================================
来源：http://xyc.yonumen.top

O. 并发与异步
来源：http://nlx.zhongyouzk.top

================================================================================
来源：http://xmz.birdmap.top

[O01] 启动一个线程
来源：http://wnc.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pmj.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wde.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yfn.shuidangran.top

TS:   // 同 JS
来源：http://nfw.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://tli.tian-w.cn

Go:   go f()
来源：http://hfx.yuanzhike.top

Ruby: Thread.new { f }
来源：http://pft.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://qhr.cdnleiting.top

[O02] 使用线程池
来源：http://mjt.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lfw.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://trq.fzhhl.top

JS:   // worker_threads 线程池
来源：http://deq.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://wvg.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://cvt.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ahq.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://noc.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://azp.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://kdi.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://una.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://cvw.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://byf.birdmap.top

TS:   // 同 JS
来源：http://lmu.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://qhl.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uel.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://use.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://jnn.smart0.xyz

[O04] 定义异步函数并等待
来源：http://hwz.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://iow.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gfj.aizwys.cn

JS:   async function f() { await g(); }
来源：http://uhw.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://nws.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cjj.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://egm.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://onl.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://bkn.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://qjf.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://acs.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xhx.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://lew.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://juv.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dzn.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qon.cashguo.top

Ruby: threads.map(&:join)
来源：http://ixr.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sxe.ctjpmb.com

[O06] 使用进程池
来源：http://gsr.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://acp.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qoi.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://gme.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://gyd.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zag.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ytk.jyoumei.cn

Ruby: // fork 块
来源：http://idn.jqgufenzy.top

C#:   Parallel.For
来源：http://cwi.hnqzz.top

================================================================================
来源：http://nik.nanxuanxn.top

P. 常用工具函数
来源：http://utp.zhengqikj.top

================================================================================
来源：http://ezt.zdqjudy.top


<!-- 参考信息 -->