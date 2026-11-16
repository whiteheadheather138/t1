代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aww.jlsjyb.cn

JS:   await fetch(url)
来源：http://tbd.9152youxi.cn

TS:   await fetch(url)
来源：http://sck.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xlg.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://pyc.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://lmy.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ogg.yfazqb.com

[L02] 发送 POST JSON
来源：http://mye.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jlw.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvp.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bgb.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://exh.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kgr.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oij.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zqz.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gbq.sweek.top

[L03] 设置自定义请求头
来源：http://mzr.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qdz.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ail.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sna.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://llr.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://psm.zhaomingkeji.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urg.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fgv.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pva.vehdjk.com

[L04] 设置超时
来源：http://hpf.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://ots.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nrw.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvd.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vqy.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bqh.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uyg.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lbm.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://are.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://uvw.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rdb.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://twk.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://grt.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://olc.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hoq.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jqh.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nwd.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgz.cucudq.cn

[L06] 解析响应为 JSON
来源：http://ang.gzhubu.top

Py:   resp.json()
来源：http://bsl.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://nqs.daxiang520.top

JS:   await resp.json()
来源：http://qjz.pengpengdd.cyou

TS:   await resp.json()
来源：http://vwd.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eqq.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tny.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://xyg.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dmc.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://fjg.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qmn.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vmi.yj20258.top

JS:   resp.ok;  resp.status
来源：http://stz.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://cwu.meibo888.top

Java: resp.statusCode()
来源：http://iuc.sysykeji.top

Go:   resp.StatusCode
来源：http://agg.tarul.cn

Ruby: resp.code.to_i
来源：http://lps.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://bxb.yfazqb.com

[L08] 并发请求多个地址
来源：http://tdi.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vko.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://odk.guowangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpn.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dez.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sxd.52xcode.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lth.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ssb.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gmo.hongshengwenyu.top

================================================================================
来源：http://ubd.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://rmo.316326.xyz

================================================================================
来源：http://rsj.zhijiandao.cn

[M01] 读取命令行参数
来源：http://lyo.aibaodan.cn

Py:   sys.argv[1:]
来源：http://sij.yueranfly.top

PHP:  $argv;  $argc;
来源：http://vhe.fzhhl.top

JS:   process.argv.slice(2)
来源：http://zsq.zycfv.cn

TS:   process.argv.slice(2)
来源：http://kxv.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://qxb.sweek.top

Go:   os.Args[1:]
来源：http://hmi.hywenlv.cn

Ruby: ARGV
来源：http://mle.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://ahr.jianghu66.top

[M02] 读取环境变量
来源：http://txl.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://ghk.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://btx.redwolf501.top

JS:   process.env.HOME
来源：http://usf.zhiwuduotai.top

TS:   process.env.HOME
来源：http://tqk.xziqi.cn

Java: System.getenv("HOME")
来源：http://ncf.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vfb.daxiang520.top

Ruby: ENV["HOME"]
来源：http://lvf.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lty.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://xfj.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kdh.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yun.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jut.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vhq.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sez.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://hyx.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yxa.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://bhi.svipenyu.cn

[M04] 获取当前工作目录
来源：http://eke.wangdashe.top

Py:   os.getcwd()
来源：http://blo.wangshuangyany.cn

PHP:  getcwd();
来源：http://kyq.yuanzhike.top

JS:   process.cwd()
来源：http://nnj.sufxvd.cn

TS:   process.cwd()
来源：http://teb.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://ili.uphjek.com

Go:   os.Getwd()
来源：http://jau.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://lpq.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://caz.fzhhl.top

[M05] 设置退出码
来源：http://yrc.316326.xyz

Py:   sys.exit(1)
来源：http://ozc.hesvh.cn

PHP:  exit(1);
来源：http://tic.tarul.cn

JS:   process.exit(1)
来源：http://acp.sweek.top

TS:   process.exit(1)
来源：http://eaf.uphjek.com

Java: System.exit(1)
来源：http://kwo.cheryme.top

Go:   os.Exit(1)
来源：http://xoa.xuetiantiany.cn

Ruby: exit 1
来源：http://cjt.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://udc.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://ano.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://git.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://yxq.mhx1999.top

JS:   console.error("err")
来源：http://xnq.hnxiangtu.top

TS:   console.error("err")
来源：http://epw.tianlin.xyz

Java: System.err.println("err")
来源：http://fra.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://efm.ivvv.top

Ruby: warn "err"
来源：http://bfh.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://yvv.gogol.net.cn

[M07] 判断是否为主入口
来源：http://zbg.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://aib.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cmo.epnwcf.com

JS:   require.main === module
来源：http://kde.bjfxy.top

TS:   require.main === module
来源：http://ubh.nanxinkj.top

Java: public static void main(String[] args)
来源：http://hyk.fzhhl.top

Go:   func main()
来源：http://ldw.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dhi.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://elq.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://yfe.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://gor.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://jju.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://aso.yongpay.top

TS:   process.platform;  process.version
来源：http://olr.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bxk.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgf.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mgk.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tyn.hcnkem.com

================================================================================
来源：http://urt.0kj1m.cn

N. 数据结构与算法
来源：http://jdt.yanxiufei.cn

================================================================================
来源：http://mbe.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://qhp.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mtj.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zzb.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqm.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lcg.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://fgq.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://zte.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jsr.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://ijk.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://iwx.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://qcu.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jzy.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hgv.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://rei.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uwb.aizwys.cn

Go:   slices.Sort(arr)
来源：http://mui.sufxvd.cn

Ruby: arr.sort
来源：http://xjf.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://frm.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://uqx.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hev.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://dna.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asj.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdj.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nug.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://whv.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vcs.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://ddt.gotoacloud.top

[N04] 斐波那契数列
来源：http://nub.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rks.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eof.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbd.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzf.xuanzx.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rid.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qop.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nqn.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ynv.jyoumei.cn

[N05] 最大公约数
来源：http://wff.xinyue.icu

Py:   math.gcd(a, b)
来源：http://mah.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://top.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dbj.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btf.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rss.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sgz.cashguo.top

Ruby: a.gcd(b)
来源：http://yqv.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hdg.c1oappe.top

[N06] 判断回文字符串
来源：http://pbw.quarkkingdee.top

Py:   s == s[::-1]
来源：http://rnr.wangdashe.top

PHP:  $s === strrev($s);
来源：http://skq.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://lqx.yj20258888.top

TS:   s === [...s].reverse().join("")
来源：http://tre.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://khd.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://xkb.fehbvm.com

Ruby: s == s.reverse
来源：http://cee.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ezu.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://udo.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://woz.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ecj.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hrd.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://qom.wangdashe.top

Java: // 手写 HashMap
来源：http://xly.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://xun.316326.xyz

Ruby: // 手写 Hash
来源：http://sco.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dxa.tarul.cn

[N08] 生成全排列
来源：http://svs.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://qcv.tian-w.cn

PHP:  // 手写递归交换
来源：http://zdl.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://gas.zdbjq.cn

TS:   // 手写回溯递归
来源：http://rkd.zdbjq.cn

Java: // 手写回溯递归
来源：http://mew.bjfxy.top

Go:   // 手写回溯递归
来源：http://mhz.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://mtn.tianlin.xyz

C#:   // 手写回溯递归
来源：http://pxo.kuanghao11.cn

[N09] 栈与队列
来源：http://vap.nanxuanxn.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yrn.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uhs.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://col.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cty.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ezc.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://owj.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ryr.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zft.ivvv.top

[N10] 链表节点定义
来源：http://whx.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibj.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://byh.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mgo.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rdx.meibo888.top

Java: class Node { int v; Node next; }
来源：http://eqy.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://yyb.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://awp.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yyp.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://jpn.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ixg.zdbjq.cn

PHP:  // 手写递归函数
来源：http://sxh.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wqt.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bxn.hesvh.cn

Java: // 手写递归
来源：http://naa.wangshuangyany.cn

Go:   // 手写递归
来源：http://cap.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ygu.shangyingyoupin.top

C#:   // 手写递归
来源：http://jad.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lfd.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ooo.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yyb.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzs.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwn.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cst.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://slf.ybcxt.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hbf.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://erw.nanxinkj.top

================================================================================
来源：http://lns.xingfuxueyuan.xyz

O. 并发与异步
来源：http://fpr.tarul.cn

================================================================================
来源：http://rug.shangyingyoupin.top

[O01] 启动一个线程
来源：http://sau.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zyi.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://suj.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ddi.fanxiaobao.xyz

TS:   // 同 JS
来源：http://bet.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://pai.ehwqpu.com

Go:   go f()
来源：http://krg.yj20258888.top

Ruby: Thread.new { f }
来源：http://gml.mhx1999.top

C#:   Task.Run(() => F());
来源：http://okj.pycfn.com

[O02] 使用线程池
来源：http://nhu.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dcj.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jdm.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://phs.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://pnl.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://jxz.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bqt.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qff.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyl.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://xnh.svipenyu.cn

Py:   with lock: shared += 1
来源：http://meh.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://ajf.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mdw.52xcode.cn

TS:   // 同 JS
来源：http://gwv.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://qtr.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kzz.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gih.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ubo.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://thc.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://eir.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wvh.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://fzp.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ukm.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ksb.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eck.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rjk.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://kon.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://olp.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://qld.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vaj.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://esk.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://hcx.sjlbkw.cn


<!-- 参考信息 -->