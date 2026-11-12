代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://znb.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://owo.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://msj.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ism.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yuu.iojbl.cn

[L04] 设置超时
来源：http://qvz.xylfe.cn

Py:   requests.get(url, timeout=5)
来源：http://ycv.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vud.wangdashe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqm.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aqe.tianlin.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fsj.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eeo.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lwy.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ydp.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://ria.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kva.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vuk.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fjd.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vck.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qka.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nnl.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://emc.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qln.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ykx.uphjek.com

Py:   resp.json()
来源：http://nyc.yfazqb.com

PHP:  json_decode($body, true);
来源：http://szq.hnxiangtu.top

JS:   await resp.json()
来源：http://frs.svipenyu.cn

TS:   await resp.json()
来源：http://lln.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hwd.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fra.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://eap.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cxs.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://xtt.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ktc.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://obc.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://jbq.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://vqw.svipenyu.cn

Java: resp.statusCode()
来源：http://vch.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://pgz.cashguo.top

Ruby: resp.code.to_i
来源：http://xbp.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://qud.daria6918.cn

[L08] 并发请求多个地址
来源：http://cxi.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cbz.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://ybh.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gbs.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wvp.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aix.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hxr.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wxp.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bus.fehbvm.com

================================================================================
来源：http://cvu.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://gvd.mhx1999.top

================================================================================
来源：http://slv.xziqi.cn

[M01] 读取命令行参数
来源：http://qii.9152youxi.cn

Py:   sys.argv[1:]
来源：http://kkg.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://mlc.ydzc1.top

JS:   process.argv.slice(2)
来源：http://rlb.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://gkw.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://ilf.jqgfzy.top

Go:   os.Args[1:]
来源：http://bvw.xuanzx.com

Ruby: ARGV
来源：http://qoj.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://xpi.snrcjt.cn

[M02] 读取环境变量
来源：http://myu.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://yja.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ihk.redwolf501.top

JS:   process.env.HOME
来源：http://ucu.tian-w.cn

TS:   process.env.HOME
来源：http://qvc.0kj1m.cn

Java: System.getenv("HOME")
来源：http://lth.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eop.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://onh.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wjq.0kj1m.cn

[M03] 执行外部命令
来源：http://lfg.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zab.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iql.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://obx.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cad.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hyz.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fao.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://vnu.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://mty.gotoacloud.top

[M04] 获取当前工作目录
来源：http://hmg.hongshengwenyu.top

Py:   os.getcwd()
来源：http://mqt.jyoumei.cn

PHP:  getcwd();
来源：http://fup.shangyingyoupin.top

JS:   process.cwd()
来源：http://jvl.sxryk.cn

TS:   process.cwd()
来源：http://zem.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://tbj.wangshuangyany.cn

Go:   os.Getwd()
来源：http://tyf.hysaishi.cn

Ruby: Dir.pwd
来源：http://gch.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://psf.hfpthk.cn

[M05] 设置退出码
来源：http://olj.meibo888.top

Py:   sys.exit(1)
来源：http://uab.shangyingyoupin.top

PHP:  exit(1);
来源：http://qdk.yvedp.cn

JS:   process.exit(1)
来源：http://lzk.zycfv.cn

TS:   process.exit(1)
来源：http://fwh.ctjpmb.com

Java: System.exit(1)
来源：http://oel.cashguo.top

Go:   os.Exit(1)
来源：http://erv.jinghuilouyu.cn

Ruby: exit 1
来源：http://fbu.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tdo.sjlbkw.cn

[M06] 向标准错误输出
来源：http://hvx.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://efa.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bia.hongshengwenyu.top

JS:   console.error("err")
来源：http://pfa.xziqi.cn

TS:   console.error("err")
来源：http://yzp.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://xly.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://udy.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://oyr.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://bam.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://pth.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://gvg.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xdn.cucudq.cn

JS:   require.main === module
来源：http://wca.nanxuanxn.top

TS:   require.main === module
来源：http://aav.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://kgt.yvedp.cn

Go:   func main()
来源：http://eet.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tpv.bbcook.cn

C#:   static void Main(string[] args)
来源：http://fas.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://bhf.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://atz.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://agx.sweek.top

JS:   process.platform;  process.version
来源：http://ovo.nwbrower.top

TS:   process.platform;  process.version
来源：http://jqk.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nar.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dvt.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://enm.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxp.yj202588.top

================================================================================
来源：http://gdj.nanxinkj.top

N. 数据结构与算法
来源：http://lrq.wangdashe.top

================================================================================
来源：http://uvn.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://hog.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://egm.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ueq.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhm.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iqi.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://nze.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://xkn.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eib.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lic.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://osm.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://gck.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iwi.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://saq.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ugj.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ziz.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://ckg.yuxming.cn

Ruby: arr.sort
来源：http://zul.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bkk.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://qus.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rcg.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://sgw.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxt.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eep.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oxh.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dal.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jzd.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://avx.ivvv.top

[N04] 斐波那契数列
来源：http://xeb.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xxc.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://exw.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://snr.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gox.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ynh.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://itn.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cws.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jlj.meibo888.top

[N05] 最大公约数
来源：http://izt.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://tbf.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ldb.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://smm.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dyw.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iin.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://osh.mhx1999.top

Ruby: a.gcd(b)
来源：http://uhk.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fch.shzxlz.cn

[N06] 判断回文字符串
来源：http://orh.sxryk.cn

Py:   s == s[::-1]
来源：http://tae.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://wie.quarkkingdee.top

JS:   s === [...s].reverse().join("")
来源：http://ibc.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://keo.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xiz.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://pqe.fktsv.cn

Ruby: s == s.reverse
来源：http://lfy.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://znl.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://txd.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cdd.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qvl.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://spo.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://gyi.sjlbkw.cn

Java: // 手写 HashMap
来源：http://qyj.cheryme.top

Go:   // 手写 map[int]int
来源：http://mec.cucudq.cn

Ruby: // 手写 Hash
来源：http://aui.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://uod.tanke756.top

[N08] 生成全排列
来源：http://tyz.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://pdm.dashuyun.cn

PHP:  // 手写递归交换
来源：http://yto.meibo888.top

JS:   // 手写回溯递归
来源：http://iej.svipenyu.cn

TS:   // 手写回溯递归
来源：http://nst.xuanzx.com

Java: // 手写回溯递归
来源：http://wtp.tanke756.top

Go:   // 手写回溯递归
来源：http://jhj.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://clk.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://yom.hcnkem.com

[N09] 栈与队列
来源：http://rgh.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qmr.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jva.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zyu.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tch.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rlq.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykw.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://unc.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qtt.quarkkingdee.top

[N10] 链表节点定义
来源：http://uea.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ugi.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sta.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://seg.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://alc.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://gjg.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ihk.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ewl.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fst.iojbl.cn

[N11] 二叉树中序遍历
来源：http://aks.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gni.hesvh.cn

PHP:  // 手写递归函数
来源：http://xop.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nfk.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zqg.shanyushiyangtech.top

Java: // 手写递归
来源：http://sqg.gaohongyu789.top

Go:   // 手写递归
来源：http://iin.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yju.c1oappe.top

C#:   // 手写递归
来源：http://cxe.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zuy.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wod.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ntn.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jed.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://enm.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wbf.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gke.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gaj.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lba.jlsjyb.cn

================================================================================
来源：http://asf.jianghu66.top

O. 并发与异步
来源：http://hor.svipenyu.cn

================================================================================
来源：http://gfv.yanxiufei.cn

[O01] 启动一个线程
来源：http://ous.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xdu.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rgd.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hfr.birdmap.top

TS:   // 同 JS
来源：http://spn.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://vpm.daria6918.cn

Go:   go f()
来源：http://off.yvedp.cn

Ruby: Thread.new { f }
来源：http://yba.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://pqo.smart0.xyz

[O02] 使用线程池
来源：http://nfk.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lku.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dya.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://lss.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://ufp.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://ser.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eqm.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dov.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dvl.tarul.cn

[O03] 加锁保护共享数据
来源：http://fhq.hywenlv.cn

Py:   with lock: shared += 1
来源：http://hog.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://xzp.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://onm.gotoacloud.top

TS:   // 同 JS
来源：http://uqg.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://kyh.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ftk.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://icx.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://bqo.yuxming.cn

[O04] 定义异步函数并等待
来源：http://gpq.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://zqr.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pcq.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://ybb.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://iyi.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gze.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ufc.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ocm.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://buo.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://njp.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://xgn.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sda.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://zrf.uphjek.com

TS:   await Promise.all(tasks)
来源：http://yjb.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wpp.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xmk.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://eji.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uya.jqgufenzy.top

[O06] 使用进程池
来源：http://vwu.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uub.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cjy.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://yqe.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://gcy.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zcx.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eua.quarkkingdee.top

Ruby: // fork 块
来源：http://vhu.birdmap.top

C#:   Parallel.For
来源：http://ylp.yangfankeji.com

================================================================================
来源：http://ney.shanyushiyangtech.top

P. 常用工具函数
来源：http://xxs.xziqi.cn

================================================================================
来源：http://qip.0kj1m.cn

[P01] 生成 UUID
来源：http://czi.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://owt.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zsa.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://lfa.316326.xyz


<!-- 参考信息 -->