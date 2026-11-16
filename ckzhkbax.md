代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lms.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dci.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ywe.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qiy.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dxx.shuidangran.top

[L04] 设置超时
来源：http://uxh.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://goo.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgf.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tsg.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://msn.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://chg.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://usn.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wds.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mfi.wangdashe.top

[L05] 上传文件（multipart）
来源：http://uav.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qew.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mhg.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gic.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oau.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ymj.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jxe.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vbh.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zch.ydzc1.top

[L06] 解析响应为 JSON
来源：http://jyb.xinyue.icu

Py:   resp.json()
来源：http://bfr.sxryk.cn

PHP:  json_decode($body, true);
来源：http://pto.shanyushiyangtech.top

JS:   await resp.json()
来源：http://tcy.yueranfly.top

TS:   await resp.json()
来源：http://wju.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://luq.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dhp.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://awp.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqv.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://gvk.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hop.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ogg.birdmap.top

JS:   resp.ok;  resp.status
来源：http://obo.uphjek.com

TS:   resp.ok;  resp.status
来源：http://xij.jiagoushi.top

Java: resp.statusCode()
来源：http://err.jlsjyb.cn

Go:   resp.StatusCode
来源：http://inr.xylfe.cn

Ruby: resp.code.to_i
来源：http://uid.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://szb.ehwqpu.com

[L08] 并发请求多个地址
来源：http://nxy.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ryz.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://agv.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://atq.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uog.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vlv.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hnb.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wub.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qbd.sxryk.cn

================================================================================
来源：http://qwu.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://odk.sufxvd.cn

================================================================================
来源：http://xlu.hysaishi.cn

[M01] 读取命令行参数
来源：http://uca.xylfe.cn

Py:   sys.argv[1:]
来源：http://rko.ydzc1.top

PHP:  $argv;  $argc;
来源：http://gsu.vehdjk.com

JS:   process.argv.slice(2)
来源：http://arf.jianghu66.top

TS:   process.argv.slice(2)
来源：http://lio.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://uyk.zdbjq.cn

Go:   os.Args[1:]
来源：http://dwy.hesvh.cn

Ruby: ARGV
来源：http://bmi.nwbrower.top

C#:   args 数组（Main 方法参数）
来源：http://prj.jqgfzy.top

[M02] 读取环境变量
来源：http://vhf.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://xpy.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://osk.gogol.net.cn

JS:   process.env.HOME
来源：http://dym.jqgufenzy.top

TS:   process.env.HOME
来源：http://tij.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://loq.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://awf.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://rxi.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nak.dianchejie.cn

[M03] 执行外部命令
来源：http://zan.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sef.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bpp.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://fbs.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jtx.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lst.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://noa.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://bsq.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://xuu.yfazqb.com

[M04] 获取当前工作目录
来源：http://kdv.jiagoushi.top

Py:   os.getcwd()
来源：http://gvy.yj202588.top

PHP:  getcwd();
来源：http://bll.zhixingplan.top

JS:   process.cwd()
来源：http://ghn.zhongyouzk.top

TS:   process.cwd()
来源：http://dmg.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://oyo.chenjidiqi.icu

Go:   os.Getwd()
来源：http://sqr.fehbvm.com

Ruby: Dir.pwd
来源：http://yyk.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gvn.svipenyu.cn

[M05] 设置退出码
来源：http://gvk.fengsongda.top

Py:   sys.exit(1)
来源：http://ocg.smart0.xyz

PHP:  exit(1);
来源：http://ziq.cashguo.top

JS:   process.exit(1)
来源：http://cet.gaohongyu789.top

TS:   process.exit(1)
来源：http://gww.wangshuangyany.cn

Java: System.exit(1)
来源：http://onf.c1oappe.top

Go:   os.Exit(1)
来源：http://mkd.nanxinkj.top

Ruby: exit 1
来源：http://ivn.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jee.cashguo.top

[M06] 向标准错误输出
来源：http://xzn.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://slb.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://chl.cdnleiting.top

JS:   console.error("err")
来源：http://nty.quarkkingdee.top

TS:   console.error("err")
来源：http://ipc.zhongyouzk.top

Java: System.err.println("err")
来源：http://ijx.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yde.jlsjyb.cn

Ruby: warn "err"
来源：http://fzf.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://mxc.redwolf501.top

[M07] 判断是否为主入口
来源：http://mbw.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://btk.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hzr.nwbrower.top

JS:   require.main === module
来源：http://anw.xuetiantiany.cn

TS:   require.main === module
来源：http://ctp.cashguo.top

Java: public static void main(String[] args)
来源：http://cqo.chenzaomai.com

Go:   func main()
来源：http://qko.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://clo.epnwcf.com

C#:   static void Main(string[] args)
来源：http://brb.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://zmg.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://fwp.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://uiu.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://amy.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://sha.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pbz.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cbf.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cit.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qhk.jqgufenzy.top

================================================================================
来源：http://jsq.nanxinkj.top

N. 数据结构与算法
来源：http://jce.gzhubu.top

================================================================================
来源：http://xcp.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://bkl.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fbx.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iep.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oez.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kir.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cgz.uphjek.com

Go:   sort.SearchInts(arr, x)
来源：http://hur.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yzs.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://brh.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://dwh.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://cqy.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pcs.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xlg.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbi.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://diq.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://twh.xuanzx.com

Ruby: arr.sort
来源：http://sqh.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ktu.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://giq.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zbw.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://opm.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hru.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://twg.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pnk.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nnu.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hzx.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dwx.zdbjq.cn

[N04] 斐波那契数列
来源：http://wyh.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uwo.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rhr.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eor.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pel.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lwo.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yjy.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bmu.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mfd.yuxming.cn

[N05] 最大公约数
来源：http://rir.sweek.top

Py:   math.gcd(a, b)
来源：http://wik.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kic.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyf.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mfu.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zdy.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tqf.hesvh.cn

Ruby: a.gcd(b)
来源：http://paq.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kjf.ivvv.top

[N06] 判断回文字符串
来源：http://acq.jianghu66.top

Py:   s == s[::-1]
来源：http://abg.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://dal.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://mur.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://sel.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nry.tanke756.top

Go:   // 双指针从两端比较
来源：http://ceq.shuidangran.top

Ruby: s == s.reverse
来源：http://atw.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xag.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://xaq.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vjc.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tmq.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sao.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://pax.iojbl.cn

Java: // 手写 HashMap
来源：http://lus.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://nhz.chenzaomai.com

Ruby: // 手写 Hash
来源：http://fov.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kop.ydzc1.top

[N08] 生成全排列
来源：http://agw.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://zer.hywenlv.cn

PHP:  // 手写递归交换
来源：http://wqf.ydzc1.top

JS:   // 手写回溯递归
来源：http://gws.daxiang520.top

TS:   // 手写回溯递归
来源：http://tom.hammf.cn

Java: // 手写回溯递归
来源：http://bkm.sufxvd.cn

Go:   // 手写回溯递归
来源：http://pkb.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://qot.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://sxq.ppjwa.cn

[N09] 栈与队列
来源：http://jhv.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tqg.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mhh.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzi.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nwd.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://shs.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwa.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fnd.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ykd.shzxlz.cn

[N10] 链表节点定义
来源：http://uof.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qcm.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://env.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bcx.fengsongda.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lwf.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://ixf.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vch.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://fji.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ppj.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://bzg.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lpa.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://onb.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bne.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjg.jianghu66.top

Java: // 手写递归
来源：http://ops.snrcjt.cn

Go:   // 手写递归
来源：http://xay.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kor.xuanzx.com

C#:   // 手写递归
来源：http://sit.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jzc.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://apn.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhk.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tyq.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://edn.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gig.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kit.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pus.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qdy.cashguo.top

================================================================================
来源：http://npo.vehdjk.com

O. 并发与异步
来源：http://scq.gzhubu.top

================================================================================
来源：http://dcy.zhengqikj.top

[O01] 启动一个线程
来源：http://ovr.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://izr.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iar.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://meg.aibaodan.cn

TS:   // 同 JS
来源：http://ltl.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://yqa.jqgufenzy.top

Go:   go f()
来源：http://qqa.chenzaomai.com

Ruby: Thread.new { f }
来源：http://gpm.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://umi.snrcjt.cn

[O02] 使用线程池
来源：http://tcb.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xmp.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wvx.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://dhr.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://yid.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://qgm.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xca.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cst.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://scj.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://gjh.yuxming.cn

Py:   with lock: shared += 1
来源：http://jvd.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://mio.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tww.haohaochexian.top

TS:   // 同 JS
来源：http://mqz.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://ezy.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gsg.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://urg.dianchejie.cn

C#:   lock (gate) { shared++; }
来源：http://aus.shuidangran.top

[O04] 定义异步函数并等待
来源：http://zab.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://onq.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rpo.xuanzx.com

JS:   async function f() { await g(); }
来源：http://nwz.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wkc.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tzz.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rul.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://bqv.yonumen.top

C#:   async Task F() { await G(); }
来源：http://kcm.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://roj.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://lap.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ajo.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://clu.ivvv.top

TS:   await Promise.all(tasks)
来源：http://chd.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://day.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kic.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://zeg.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bcp.pycfn.com

[O06] 使用进程池
来源：http://ycq.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jpd.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ouw.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://rwi.sweek.top

TS:   // child_process / cluster 模块
来源：http://xkf.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nmg.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hyo.guowangkeji.top

Ruby: // fork 块
来源：http://feb.jinghuilouyu.cn

C#:   Parallel.For
来源：http://znh.hcnkem.com

================================================================================
来源：http://lal.yuxming.cn

P. 常用工具函数
来源：http://llu.sufxvd.cn

================================================================================
来源：http://ots.jianghu66.top

[P01] 生成 UUID
来源：http://zis.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://xnt.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ski.yfazqb.com

JS:   crypto.randomUUID()
来源：http://dfq.bjfxy.top


<!-- 参考信息 -->