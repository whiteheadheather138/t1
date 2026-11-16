代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://iuz.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iut.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pbe.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://ulp.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://ptn.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aga.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhw.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zev.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nne.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssf.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jin.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rzg.jianghu66.top

[L03] 设置自定义请求头
来源：http://xxg.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cfp.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jhg.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ior.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qww.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://plj.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oov.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rxi.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cyy.zdbjq.cn

[L04] 设置超时
来源：http://cds.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://cah.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zxe.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://few.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zim.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ggr.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jih.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvn.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://clw.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://uus.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vhy.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vlo.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jbn.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jhb.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oyc.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mvq.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://shs.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pil.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://zwi.shanyushiyangkeji.top

Py:   resp.json()
来源：http://qcs.fzhhl.top

PHP:  json_decode($body, true);
来源：http://mfw.hongshengwenyu.top

JS:   await resp.json()
来源：http://mvc.yfazqb.com

TS:   await resp.json()
来源：http://ogg.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rin.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://scf.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://qxj.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fco.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://erg.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://svf.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aho.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://dmi.hesvh.cn

TS:   resp.ok;  resp.status
来源：http://lnd.zhongyouzk.top

Java: resp.statusCode()
来源：http://thc.yangfankeji.com

Go:   resp.StatusCode
来源：http://bfv.daria6918.cn

Ruby: resp.code.to_i
来源：http://mql.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://gnb.svipenyu.cn

[L08] 并发请求多个地址
来源：http://rre.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vpo.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://xpn.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ztm.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bsb.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fmz.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wqt.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tja.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ulc.316326.xyz

================================================================================
来源：http://dyz.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://vux.sjlbkw.cn

================================================================================
来源：http://aij.jyoumei.cn

[M01] 读取命令行参数
来源：http://eqw.shzxlz.cn

Py:   sys.argv[1:]
来源：http://rhq.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://kuv.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://nen.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://hum.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://uit.meibo888.top

Go:   os.Args[1:]
来源：http://jop.gaohongyu789.top

Ruby: ARGV
来源：http://zxn.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://jlf.yj20258.top

[M02] 读取环境变量
来源：http://drq.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://kmm.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://klo.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://ssn.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://klw.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://ycm.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://elv.tanke756.top

Ruby: ENV["HOME"]
来源：http://bdn.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mvj.daria6918.cn

[M03] 执行外部命令
来源：http://ktz.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://its.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nbp.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rii.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://uks.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yua.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://imv.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://xsr.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://hho.hysaishi.cn

[M04] 获取当前工作目录
来源：http://bcz.vqdsnc.cn

Py:   os.getcwd()
来源：http://rbv.ctjpmb.com

PHP:  getcwd();
来源：http://jdy.hywenlv.cn

JS:   process.cwd()
来源：http://jnh.zhixingplan.top

TS:   process.cwd()
来源：http://iou.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://cqx.haohaochexian.top

Go:   os.Getwd()
来源：http://yqk.zhixingplan.top

Ruby: Dir.pwd
来源：http://zrh.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://zyx.wangshuangyany.cn

[M05] 设置退出码
来源：http://ylo.vqdsnc.cn

Py:   sys.exit(1)
来源：http://pmd.yfazqb.com

PHP:  exit(1);
来源：http://ack.gogol.net.cn

JS:   process.exit(1)
来源：http://cxr.jqgfzy.top

TS:   process.exit(1)
来源：http://wpc.gotoacloud.top

Java: System.exit(1)
来源：http://okl.guowangkeji.top

Go:   os.Exit(1)
来源：http://hpp.andypj.xyz

Ruby: exit 1
来源：http://tfs.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccr.vehdjk.com

[M06] 向标准错误输出
来源：http://rwc.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://hij.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rzn.yuxming.cn

JS:   console.error("err")
来源：http://ozz.0kj1m.cn

TS:   console.error("err")
来源：http://xip.jinqigufen.top

Java: System.err.println("err")
来源：http://xfa.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vmd.zhengqikj.top

Ruby: warn "err"
来源：http://efv.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://uuz.tarul.cn

[M07] 判断是否为主入口
来源：http://lyj.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://ura.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xgn.jiagoushi.top

JS:   require.main === module
来源：http://qke.yongpay.top

TS:   require.main === module
来源：http://prs.ehwqpu.com

Java: public static void main(String[] args)
来源：http://gxu.hongshengwenyu.top

Go:   func main()
来源：http://juz.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://trt.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://dwc.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://voz.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://who.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://wrg.tian-w.cn

JS:   process.platform;  process.version
来源：http://mkg.yueranfly.top

TS:   process.platform;  process.version
来源：http://lfo.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rgy.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ovx.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yya.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qme.hnxiangtu.top

================================================================================
来源：http://fad.hammf.cn

N. 数据结构与算法
来源：http://zkd.wangdashe.top

================================================================================
来源：http://aaw.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://hpf.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://mfv.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qak.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iej.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://orh.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pvo.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://hfp.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uby.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://zvq.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://wsa.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://jel.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://obu.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bcx.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjo.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jao.vehdjk.com

Go:   slices.Sort(arr)
来源：http://lrf.sufxvd.cn

Ruby: arr.sort
来源：http://phk.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tqp.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://ohw.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://elr.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://gfp.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eur.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ifg.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ppp.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dyv.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aav.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://ddv.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://kos.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ilg.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lma.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nuz.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bua.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ykq.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iqd.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hqh.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://okk.pengpengdd.cyou

[N05] 最大公约数
来源：http://vnj.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://ksf.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zln.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bey.shzxlz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sab.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yle.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ace.jianghu66.top

Ruby: a.gcd(b)
来源：http://xvh.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oxr.gotoacloud.top

[N06] 判断回文字符串
来源：http://jwp.shuidangran.top

Py:   s == s[::-1]
来源：http://mtr.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://ihi.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://bil.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://mox.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://frv.wangdashe.top

Go:   // 双指针从两端比较
来源：http://gzn.ydjk.org.cn

Ruby: s == s.reverse
来源：http://cuk.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkg.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://twv.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yld.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xyi.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xpx.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://sek.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://zxi.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://xmk.xuanzx.com

Ruby: // 手写 Hash
来源：http://ige.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hvy.0kj1m.cn

[N08] 生成全排列
来源：http://lef.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://zww.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://idg.xuanzx.com

JS:   // 手写回溯递归
来源：http://taq.yuanzhike.top

TS:   // 手写回溯递归
来源：http://alk.zhijiandao.cn

Java: // 手写回溯递归
来源：http://ftc.birdmap.top

Go:   // 手写回溯递归
来源：http://biz.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://ste.316326.xyz

C#:   // 手写回溯递归
来源：http://all.xuetiantiany.cn

[N09] 栈与队列
来源：http://gbe.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mib.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rbt.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jxk.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xhc.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://enb.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wol.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cet.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wav.mhx1999.top

[N10] 链表节点定义
来源：http://xtv.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jmr.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bsn.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nit.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iwr.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://zob.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://rfl.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qfg.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://qlq.birdmap.top

[N11] 二叉树中序遍历
来源：http://mlb.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pka.yonumen.top

PHP:  // 手写递归函数
来源：http://mkd.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgl.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://urt.vehdjk.com

Java: // 手写递归
来源：http://gzj.feifeiyinyue.top

Go:   // 手写递归
来源：http://vxx.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bzi.gotoacloud.top

C#:   // 手写递归
来源：http://oib.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wcn.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wlv.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://efp.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fej.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdo.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yij.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uyj.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jvh.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yul.aibaodan.cn

================================================================================
来源：http://smo.jianghu66.top

O. 并发与异步
来源：http://yrm.sxryk.cn

================================================================================
来源：http://myv.jqgufenzy.top

[O01] 启动一个线程
来源：http://pzv.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pol.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cpq.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fpn.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://yen.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://mnz.ydjk.org.cn

Go:   go f()
来源：http://nkx.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://vog.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://sbu.meibo888.top

[O02] 使用线程池
来源：http://abr.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ttu.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jlf.fzhhl.top

JS:   // worker_threads 线程池
来源：http://ati.hammf.cn

TS:   // worker_threads 线程池
来源：http://kqr.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hud.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lct.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://duv.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://loe.xinyue.icu

[O03] 加锁保护共享数据
来源：http://ier.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://xky.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://llk.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ovx.vqdsnc.cn

TS:   // 同 JS
来源：http://vnm.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://mon.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lbs.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vrz.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://vwf.redwolf501.top

[O04] 定义异步函数并等待
来源：http://fla.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://cyg.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pyi.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://pat.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xdz.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://udf.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jud.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://avn.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://qxk.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://jvp.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://msg.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bzi.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://cxj.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://dzs.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ksm.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jtv.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://ohr.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tyh.jinqigufen.top


<!-- 参考信息 -->