代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://uck.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yzt.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hkh.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmp.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ggt.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mdu.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://elp.shanyushiyangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xxs.jiagoushi.top

[L03] 设置自定义请求头
来源：http://kvy.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jvq.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ajb.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dsq.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jlh.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wwc.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dpx.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xso.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zsi.ehwqpu.com

[L04] 设置超时
来源：http://uhs.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://baf.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://emy.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://spt.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nwa.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fmk.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fzn.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rlw.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uho.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://usj.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eof.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ses.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gyf.aizwys.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://isb.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://djq.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iwr.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xcf.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xxc.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://cbf.daxiang520.top

Py:   resp.json()
来源：http://ezv.pycfn.com

PHP:  json_decode($body, true);
来源：http://zpt.ppjwa.cn

JS:   await resp.json()
来源：http://duq.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://ulw.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mrw.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dfl.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://rgv.hysaishi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://enk.sweek.top

[L07] 处理 HTTP 状态码
来源：http://nvq.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ipf.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jwa.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://ieo.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://dya.shuidangran.top

Java: resp.statusCode()
来源：http://ovg.zhijiandao.cn

Go:   resp.StatusCode
来源：http://eca.shzxlz.cn

Ruby: resp.code.to_i
来源：http://wtf.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://eqv.hywenlv.cn

[L08] 并发请求多个地址
来源：http://huq.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mtu.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://fik.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pgt.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fal.shzxlz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wnq.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://est.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tue.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xlw.jinyuanbaomall.cn

================================================================================
来源：http://ctt.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://qld.cucudq.cn

================================================================================
来源：http://sqs.hnxiangtu.top

[M01] 读取命令行参数
来源：http://dqm.sxryk.cn

Py:   sys.argv[1:]
来源：http://csu.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://nnw.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://isu.wangdashe.top

TS:   process.argv.slice(2)
来源：http://nry.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://mgl.hcnkem.com

Go:   os.Args[1:]
来源：http://kqw.yvedp.cn

Ruby: ARGV
来源：http://rxe.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://unp.zdbjq.cn

[M02] 读取环境变量
来源：http://jdg.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://nus.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bdr.pengpengdd.cyou

JS:   process.env.HOME
来源：http://jjd.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://evq.hfpthk.cn

Java: System.getenv("HOME")
来源：http://roi.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sme.epnwcf.com

Ruby: ENV["HOME"]
来源：http://oyd.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://keh.gaohongyu789.top

[M03] 执行外部命令
来源：http://grb.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qdx.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://awi.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hek.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://enq.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://znk.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sax.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fcl.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://sgc.tianlin.xyz

[M04] 获取当前工作目录
来源：http://ekg.jianghu66.top

Py:   os.getcwd()
来源：http://yxi.0kj1m.cn

PHP:  getcwd();
来源：http://png.jiagoushi.top

JS:   process.cwd()
来源：http://gud.daria6918.cn

TS:   process.cwd()
来源：http://fne.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://tdu.yueranfly.top

Go:   os.Getwd()
来源：http://yxj.fengsongda.top

Ruby: Dir.pwd
来源：http://imx.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://bty.ydjk.org.cn

[M05] 设置退出码
来源：http://ckp.gogol.net.cn

Py:   sys.exit(1)
来源：http://hxt.316326.xyz

PHP:  exit(1);
来源：http://and.cashguo.top

JS:   process.exit(1)
来源：http://rme.uphjek.com

TS:   process.exit(1)
来源：http://nmq.9152youxi.cn

Java: System.exit(1)
来源：http://kyh.yueranfly.top

Go:   os.Exit(1)
来源：http://sie.vehdjk.com

Ruby: exit 1
来源：http://bua.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tmw.zhengqikj.top

[M06] 向标准错误输出
来源：http://xii.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://uyz.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jlx.meibo888.top

JS:   console.error("err")
来源：http://pac.wangshuangyany.cn

TS:   console.error("err")
来源：http://vbn.haohaochexian.top

Java: System.err.println("err")
来源：http://oct.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdb.hammf.cn

Ruby: warn "err"
来源：http://viz.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://fcg.yfazqb.com

[M07] 判断是否为主入口
来源：http://uvh.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://hcg.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ajw.snrcjt.cn

JS:   require.main === module
来源：http://bzg.yvedp.cn

TS:   require.main === module
来源：http://yvm.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://wmf.ywan-chungtsiang.top

Go:   func main()
来源：http://ibt.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zuy.havefunace.top

C#:   static void Main(string[] args)
来源：http://uiw.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://pci.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://vba.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://ttw.zdbjq.cn

JS:   process.platform;  process.version
来源：http://nis.gogol.net.cn

TS:   process.platform;  process.version
来源：http://mik.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nqv.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsq.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dsy.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://biz.nanxuanxn.top

================================================================================
来源：http://rxv.9152youxi.cn

N. 数据结构与算法
来源：http://nwl.shanyushiyangtech.top

================================================================================
来源：http://rkk.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://jiw.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wgs.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qid.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ibl.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jel.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pmj.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://oot.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qyf.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://nhf.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://qah.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://ltn.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lyq.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dof.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lxi.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lgx.guannengcc.top

Go:   slices.Sort(arr)
来源：http://sae.0kj1m.cn

Ruby: arr.sort
来源：http://ygu.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kwp.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://dpy.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yxx.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://eka.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exa.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cuf.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ete.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vmr.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tcm.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://tac.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://rbc.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jfo.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zum.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqw.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bxj.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqg.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vzr.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eck.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://osi.jyoumei.cn

[N05] 最大公约数
来源：http://ywx.daria6918.cn

Py:   math.gcd(a, b)
来源：http://pzf.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ohn.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zue.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vjy.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lvd.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bab.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://xrr.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wcm.jlsjyb.cn

[N06] 判断回文字符串
来源：http://gsj.redwolf501.top

Py:   s == s[::-1]
来源：http://czp.daria6918.cn

PHP:  $s === strrev($s);
来源：http://uch.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://fdw.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://sni.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvc.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://kfw.cdnleiting.top

Ruby: s == s.reverse
来源：http://lmw.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lit.uphjek.com

[N07] 两数之和（返回下标）
来源：http://zys.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yav.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kmf.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gvo.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://ykf.yongpay.top

Java: // 手写 HashMap
来源：http://kjs.yj202588.top

Go:   // 手写 map[int]int
来源：http://qzg.haohaochexian.top

Ruby: // 手写 Hash
来源：http://cbv.bjfxy.top

C#:   // 手写 Dictionary<int, int>
来源：http://vmy.pycfn.com

[N08] 生成全排列
来源：http://qki.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://lgd.cheryme.top

PHP:  // 手写递归交换
来源：http://zwy.yfazqb.com

JS:   // 手写回溯递归
来源：http://xpw.guowangkeji.top

TS:   // 手写回溯递归
来源：http://tdb.xinyue.icu

Java: // 手写回溯递归
来源：http://gqf.fehbvm.com

Go:   // 手写回溯递归
来源：http://nnr.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://hyy.fehbvm.com

C#:   // 手写回溯递归
来源：http://sgu.jinghuilouyu.cn

[N09] 栈与队列
来源：http://ruc.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dmf.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cts.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ptu.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://awn.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kzt.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zlv.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://omy.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zen.meibo888.top

[N10] 链表节点定义
来源：http://bkl.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yid.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bbo.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://owm.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vdc.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://rdn.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://ilb.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qmn.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mst.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://bij.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kuv.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://eyc.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lff.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nai.ywan-chungtsiang.top

Java: // 手写递归
来源：http://gux.aizwys.cn

Go:   // 手写递归
来源：http://rwa.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hty.pengpengdd.cyou

C#:   // 手写递归
来源：http://ivn.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kmy.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vxj.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syj.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lmx.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://loz.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://puk.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ort.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ltz.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rzj.ppjwa.cn

================================================================================
来源：http://ehm.wangdashe.top

O. 并发与异步
来源：http://gxj.cashguo.top

================================================================================
来源：http://czh.guannengcc.top

[O01] 启动一个线程
来源：http://yzg.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jgp.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nka.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ujh.ydzc1.top

TS:   // 同 JS
来源：http://giv.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://kcs.xylfe.cn

Go:   go f()
来源：http://fpg.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://lkt.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://ouz.cqqwz.cn

[O02] 使用线程池
来源：http://nem.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ayb.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yxx.iojbl.cn

JS:   // worker_threads 线程池
来源：http://ztq.andypj.xyz

TS:   // worker_threads 线程池
来源：http://svf.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://bko.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yrs.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://waa.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zis.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://edq.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://rpz.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://dvx.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tju.xuanzx.com

TS:   // 同 JS
来源：http://nnx.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://fvw.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pld.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gfu.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://qrm.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://djw.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://edr.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sop.fehbvm.com

JS:   async function f() { await g(); }
来源：http://wyn.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cju.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://edy.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qxl.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://ztq.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://xkk.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://itk.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://cuz.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gzv.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://tki.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://dcc.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nli.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vzs.316326.xyz

Ruby: threads.map(&:join)
来源：http://koa.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://jmh.0kj1m.cn

[O06] 使用进程池
来源：http://opd.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qxg.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://orh.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://wtd.jyoumei.cn


<!-- 参考信息 -->