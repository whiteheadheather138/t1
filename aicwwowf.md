代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nmd.pycfn.com

JS:   await fetch(url)
来源：http://bxv.cdnleiting.top

TS:   await fetch(url)
来源：http://ixy.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://olk.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://sus.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wig.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vxv.0kj1m.cn

[L02] 发送 POST JSON
来源：http://rmh.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://glg.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zzt.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ckr.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lof.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hcn.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wan.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gsn.jinyuanbaomall.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vvy.tarul.cn

[L03] 设置自定义请求头
来源：http://ike.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sjd.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sjw.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ccz.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nje.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ltw.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://trh.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ggo.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fdd.fzhhl.top

[L04] 设置超时
来源：http://sld.sjlbkw.cn

Py:   requests.get(url, timeout=5)
来源：http://buy.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rig.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uru.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfy.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lfp.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qpf.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qkv.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://afl.fengsongda.top

[L05] 上传文件（multipart）
来源：http://wik.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rmh.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://utr.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cgo.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cdh.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ofx.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dek.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jvo.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vxy.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://btf.316326.xyz

Py:   resp.json()
来源：http://jct.redwolf501.top

PHP:  json_decode($body, true);
来源：http://zwl.vqdsnc.cn

JS:   await resp.json()
来源：http://bqk.tarul.cn

TS:   await resp.json()
来源：http://zxj.shangyingyoupin.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ahg.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xfl.meibo888.top

Ruby: JSON.parse(resp.body)
来源：http://tnh.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vpz.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://bad.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gmi.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lqa.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://jht.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://nfx.nanxuanxn.top

Java: resp.statusCode()
来源：http://slu.chenlongwang.top

Go:   resp.StatusCode
来源：http://dtb.redwolf501.top

Ruby: resp.code.to_i
来源：http://bpu.meibo888.top

C#:   (int)resp.StatusCode
来源：http://xlx.guowangkeji.top

[L08] 并发请求多个地址
来源：http://fhj.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dvg.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://lau.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ytn.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vlf.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tla.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dnc.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eep.chenzaomai.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ctz.fanxiaobao.xyz

================================================================================
来源：http://kxm.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://hbh.ppjwa.cn

================================================================================
来源：http://xwf.epnwcf.com

[M01] 读取命令行参数
来源：http://lbb.zycfv.cn

Py:   sys.argv[1:]
来源：http://ndy.52xcode.cn

PHP:  $argv;  $argc;
来源：http://len.hnqzz.top

JS:   process.argv.slice(2)
来源：http://roa.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://fea.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://wzh.shangyingyoupin.top

Go:   os.Args[1:]
来源：http://ymv.yvedp.cn

Ruby: ARGV
来源：http://kcy.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://dcy.zdbjq.cn

[M02] 读取环境变量
来源：http://ygs.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://wzy.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yge.ydjk.org.cn

JS:   process.env.HOME
来源：http://awr.fehbvm.com

TS:   process.env.HOME
来源：http://pzj.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://szs.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xgn.yonumen.top

Ruby: ENV["HOME"]
来源：http://epq.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://clo.shzxlz.cn

[M03] 执行外部命令
来源：http://gom.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://whq.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qog.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://coi.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lvc.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ulv.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://spd.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://cup.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://igy.sufxvd.cn

[M04] 获取当前工作目录
来源：http://sck.hfpthk.cn

Py:   os.getcwd()
来源：http://pte.hongshengwenyu.top

PHP:  getcwd();
来源：http://wpo.yangfankeji.com

JS:   process.cwd()
来源：http://amf.gzhubu.top

TS:   process.cwd()
来源：http://lwi.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://sua.zhoulong.xyz

Go:   os.Getwd()
来源：http://bcv.guannengcc.top

Ruby: Dir.pwd
来源：http://vxx.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://ifo.yonumen.top

[M05] 设置退出码
来源：http://yyb.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://uyc.zhixingplan.top

PHP:  exit(1);
来源：http://ggx.uphjek.com

JS:   process.exit(1)
来源：http://qnv.c1oappe.top

TS:   process.exit(1)
来源：http://few.chenzaomai.com

Java: System.exit(1)
来源：http://xmy.vehdjk.com

Go:   os.Exit(1)
来源：http://wjf.xziqi.cn

Ruby: exit 1
来源：http://zgn.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sot.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://tzy.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://yfy.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gff.gaohongyu789.top

JS:   console.error("err")
来源：http://gqx.jianghu66.top

TS:   console.error("err")
来源：http://jpa.fengsongda.top

Java: System.err.println("err")
来源：http://dtt.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufg.havefunace.top

Ruby: warn "err"
来源：http://rni.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://qdw.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://bxy.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://thd.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aco.hongshengwenyu.top

JS:   require.main === module
来源：http://hkt.sxryk.cn

TS:   require.main === module
来源：http://ycg.cashguo.top

Java: public static void main(String[] args)
来源：http://dho.tianlin.xyz

Go:   func main()
来源：http://jwv.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xni.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://uas.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://dtc.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://fly.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://xdi.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://ntn.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://dct.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://szs.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://joh.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxq.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wwe.jlsjyb.cn

================================================================================
来源：http://wxm.yueranfly.top

N. 数据结构与算法
来源：http://zlm.yanxiufei.cn

================================================================================
来源：http://dgz.yuanzhike.top

[N01] 二分查找（有序数组）
来源：http://pbp.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://cxk.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fhu.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhu.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgj.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://bbr.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://etu.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nrz.yj202588.top

C#:   Array.BinarySearch(arr, x)
来源：http://djy.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ppf.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ief.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://buk.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://iez.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qiv.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bzz.smart0.xyz

Go:   slices.Sort(arr)
来源：http://izv.pengpengdd.cyou

Ruby: arr.sort
来源：http://zko.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rta.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://msb.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mfl.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://bnt.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://src.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pea.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dck.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ska.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tqr.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://xko.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://ats.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://clh.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmr.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gbq.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mqc.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wdh.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nni.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qud.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fql.kuanghao11.cn

[N05] 最大公约数
来源：http://wfy.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://dbh.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://soy.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lha.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npp.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sfc.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://omj.dashuyun.cn

Ruby: a.gcd(b)
来源：http://qfd.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xdl.jlsjyb.cn

[N06] 判断回文字符串
来源：http://qcq.daxiang520.top

Py:   s == s[::-1]
来源：http://san.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://ouj.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://zyk.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://tae.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jpj.ydzc1.top

Go:   // 双指针从两端比较
来源：http://zdm.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://wpn.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://tpb.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://kxf.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dvh.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hci.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zqo.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://wcf.jiagoushi.top

Java: // 手写 HashMap
来源：http://eyt.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://ryh.sweek.top

Ruby: // 手写 Hash
来源：http://yyx.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://kte.tian-w.cn

[N08] 生成全排列
来源：http://kji.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://pws.aibaodan.cn

PHP:  // 手写递归交换
来源：http://mru.chenlongwang.top

JS:   // 手写回溯递归
来源：http://qbb.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://rmc.hammf.cn

Java: // 手写回溯递归
来源：http://vss.chenlongwang.top

Go:   // 手写回溯递归
来源：http://iah.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://gzm.cashguo.top

C#:   // 手写回溯递归
来源：http://cjz.zdbjq.cn

[N09] 栈与队列
来源：http://zqs.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kld.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xnd.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://otp.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vgz.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ycl.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xkh.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kui.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hfv.cheryme.top

[N10] 链表节点定义
来源：http://mkx.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tuj.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gsn.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pgi.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rmx.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://ior.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://qph.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wvx.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wen.fehbvm.com

[N11] 二叉树中序遍历
来源：http://xbh.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zyy.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://csn.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nar.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jws.ivvv.top

Java: // 手写递归
来源：http://aoy.zhongyouzk.top

Go:   // 手写递归
来源：http://wcy.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eoz.hcnkem.com

C#:   // 手写递归
来源：http://iwv.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lsu.xuanzx.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pqu.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blk.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fki.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sja.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://auf.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://per.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://afk.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kpz.aizwys.cn

================================================================================
来源：http://elr.ivvv.top

O. 并发与异步
来源：http://joq.hysaishi.cn

================================================================================
来源：http://uzu.redwolf501.top

[O01] 启动一个线程
来源：http://uma.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xlt.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bxu.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ufp.c1oappe.top

TS:   // 同 JS
来源：http://mqu.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://tac.dashuyun.cn

Go:   go f()
来源：http://hme.zdbjq.cn

Ruby: Thread.new { f }
来源：http://fyw.bjfxy.top

C#:   Task.Run(() => F());
来源：http://mvq.sweek.top

[O02] 使用线程池
来源：http://tpo.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tif.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aaj.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://oms.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://geg.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://peg.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vvv.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rpa.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nfc.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://ffh.0kj1m.cn

Py:   with lock: shared += 1
来源：http://qdp.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://pwe.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdg.52xcode.cn

TS:   // 同 JS
来源：http://rtp.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://gdk.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://irb.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kzv.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://eqn.guannengcc.top

[O04] 定义异步函数并等待
来源：http://mzk.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://alf.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ued.yj20258.top

JS:   async function f() { await g(); }
来源：http://mcv.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bsg.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qrl.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zvo.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://tao.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://dbt.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://gja.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://elc.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcs.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://tcg.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://kgd.zdqjudy.top


<!-- 参考信息 -->