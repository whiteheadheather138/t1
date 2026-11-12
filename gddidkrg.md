代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://xga.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vwx.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tsk.haohaochexian.top

[L02] 发送 POST JSON
来源：http://uqj.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://lpj.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sdn.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dke.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rgo.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qwl.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fgp.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://whi.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://weu.mhx1999.top

[L03] 设置自定义请求头
来源：http://yli.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rui.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eul.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cyv.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xoj.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfq.daria6918.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://szd.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sfh.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ljd.wangdashe.top

[L04] 设置超时
来源：http://cyv.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://uxu.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mzn.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://far.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wae.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tfx.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ghb.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://teo.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://err.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://dov.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hsj.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://alt.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qyc.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dbh.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nrv.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mqt.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ygv.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xio.yj20258.top

[L06] 解析响应为 JSON
来源：http://cfs.guowangkeji.top

Py:   resp.json()
来源：http://rxz.tanke756.top

PHP:  json_decode($body, true);
来源：http://pkg.chenzaomai.com

JS:   await resp.json()
来源：http://syh.sysykeji.top

TS:   await resp.json()
来源：http://gsz.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xft.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xbf.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://lfn.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jaf.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://mza.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jxi.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fnq.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://ctv.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://chj.birdmap.top

Java: resp.statusCode()
来源：http://jkp.yvedp.cn

Go:   resp.StatusCode
来源：http://xis.gzhubu.top

Ruby: resp.code.to_i
来源：http://bqs.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://crs.epnwcf.com

[L08] 并发请求多个地址
来源：http://uvb.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qqc.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://gaa.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsf.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qej.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fck.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wje.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tah.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xab.daria6918.cn

================================================================================
来源：http://gsd.sysykeji.top

M. 命令行 / 进程 / 环境
来源：http://aql.pycfn.com

================================================================================
来源：http://lgq.aizwys.cn

[M01] 读取命令行参数
来源：http://dom.daxiang520.top

Py:   sys.argv[1:]
来源：http://wio.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://gzc.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://zhe.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://rac.yj202588.top

Java: args 数组（main 方法参数）
来源：http://pog.yangfankeji.com

Go:   os.Args[1:]
来源：http://drz.jlsjyb.cn

Ruby: ARGV
来源：http://vxn.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://wkm.vqdsnc.cn

[M02] 读取环境变量
来源：http://uol.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://bja.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hkp.gotoacloud.top

JS:   process.env.HOME
来源：http://okw.hongshengwenyu.top

TS:   process.env.HOME
来源：http://vwr.shanyushiyangtech.top

Java: System.getenv("HOME")
来源：http://ajj.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nan.aizwys.cn

Ruby: ENV["HOME"]
来源：http://dpi.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://miy.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://xbo.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ewm.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ceh.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ozc.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tax.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ubk.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wcz.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://cee.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://ywf.cqqwz.cn

[M04] 获取当前工作目录
来源：http://laj.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://xlk.dianchejie.cn

PHP:  getcwd();
来源：http://hkb.c1oappe.top

JS:   process.cwd()
来源：http://cci.tian-w.cn

TS:   process.cwd()
来源：http://lwo.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://gdt.cheryme.top

Go:   os.Getwd()
来源：http://syh.yangfankeji.com

Ruby: Dir.pwd
来源：http://sbd.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oji.shzxlz.cn

[M05] 设置退出码
来源：http://hfg.ivvv.top

Py:   sys.exit(1)
来源：http://qdf.tian-w.cn

PHP:  exit(1);
来源：http://xad.vehdjk.com

JS:   process.exit(1)
来源：http://xjt.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://thz.fktsv.cn

Java: System.exit(1)
来源：http://nzh.zhixingplan.top

Go:   os.Exit(1)
来源：http://nhh.jyoumei.cn

Ruby: exit 1
来源：http://vnq.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nsk.cheryme.top

[M06] 向标准错误输出
来源：http://yze.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://dqh.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qdb.hfpthk.cn

JS:   console.error("err")
来源：http://sqd.shuidangran.top

TS:   console.error("err")
来源：http://xxi.mhx1999.top

Java: System.err.println("err")
来源：http://xnz.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zdl.zhixingplan.top

Ruby: warn "err"
来源：http://zoi.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://zfa.zdqjudy.top

[M07] 判断是否为主入口
来源：http://zre.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://fma.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ick.yuanzhike.top

JS:   require.main === module
来源：http://gcn.sufxvd.cn

TS:   require.main === module
来源：http://wrn.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://ert.snrcjt.cn

Go:   func main()
来源：http://yrl.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ski.daria6918.cn

C#:   static void Main(string[] args)
来源：http://bnr.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://zzy.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://xlj.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://jcc.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://hol.9152youxi.cn

TS:   process.platform;  process.version
来源：http://jmn.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://evg.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://elh.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpq.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ezr.birdmap.top

================================================================================
来源：http://pqv.redwolf501.top

N. 数据结构与算法
来源：http://gan.hesvh.cn

================================================================================
来源：http://vxo.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://sjv.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wno.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lfd.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ekq.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kds.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://mpg.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://mmm.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ptk.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sfo.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://gca.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://rag.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sqd.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://trr.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wce.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://luu.bjfxy.top

Go:   slices.Sort(arr)
来源：http://clh.xziqi.cn

Ruby: arr.sort
来源：http://sff.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xec.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://acv.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://toc.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://gcf.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dsf.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxz.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uok.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cmb.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bre.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://sip.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://jzx.yuxming.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://isb.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yav.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qrh.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hux.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rtl.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://znv.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rcn.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wfz.chenzaomai.com

[N05] 最大公约数
来源：http://jve.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://njd.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edl.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nsz.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cac.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pbo.dashuyun.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lak.vehdjk.com

Ruby: a.gcd(b)
来源：http://jvs.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mup.pycfn.com

[N06] 判断回文字符串
来源：http://epj.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://iyn.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://kjg.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://yvj.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://yrk.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rsr.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://ytg.gotoacloud.top

Ruby: s == s.reverse
来源：http://ede.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cxp.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://hvs.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nhg.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gjl.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hao.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://bmm.jianghu66.top

Java: // 手写 HashMap
来源：http://yfg.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://rwt.snrcjt.cn

Ruby: // 手写 Hash
来源：http://yui.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mnb.cheryme.top

[N08] 生成全排列
来源：http://fta.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://oji.tianlin.xyz

PHP:  // 手写递归交换
来源：http://lfd.yvedp.cn

JS:   // 手写回溯递归
来源：http://fxl.jqgfzy.top

TS:   // 手写回溯递归
来源：http://xpf.shuidangran.top

Java: // 手写回溯递归
来源：http://hmd.jlsjyb.cn

Go:   // 手写回溯递归
来源：http://kwb.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://csb.yangfankeji.com

C#:   // 手写回溯递归
来源：http://bic.ybcxt.top

[N09] 栈与队列
来源：http://bfz.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://exm.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xta.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lvh.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zqb.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zbi.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yvq.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xqx.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yhb.gotoacloud.top

[N10] 链表节点定义
来源：http://fgq.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xyl.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jqp.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://riy.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://glw.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://xeb.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://vyy.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xab.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cgj.316326.xyz

[N11] 二叉树中序遍历
来源：http://fjk.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rxe.aibaodan.cn

PHP:  // 手写递归函数
来源：http://yda.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozt.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jwi.ehwqpu.com

Java: // 手写递归
来源：http://hnu.jinghuilouyu.cn

Go:   // 手写递归
来源：http://uya.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://txh.uphjek.com

C#:   // 手写递归
来源：http://stx.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hga.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zfy.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://myh.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxb.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ill.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dzh.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://auq.jinghuilouyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ftp.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lzr.smart0.xyz

================================================================================
来源：http://mwe.hnxiangtu.top

O. 并发与异步
来源：http://lte.hongshengwenyu.top

================================================================================
来源：http://dth.ctjpmb.com

[O01] 启动一个线程
来源：http://wfr.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rrl.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rvp.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vjw.nwbrower.top

TS:   // 同 JS
来源：http://aur.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://tpr.yj20258888.top

Go:   go f()
来源：http://nvi.ctjpmb.com

Ruby: Thread.new { f }
来源：http://yma.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://yeo.jyoumei.cn

[O02] 使用线程池
来源：http://fvj.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://suy.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kow.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://hkq.sweek.top

TS:   // worker_threads 线程池
来源：http://ndo.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tev.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nmr.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://agn.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sbq.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://eve.gogol.net.cn

Py:   with lock: shared += 1
来源：http://fws.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://umq.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hki.fktsv.cn

TS:   // 同 JS
来源：http://moe.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://kty.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vpt.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mct.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://imf.sysykeji.top

[O04] 定义异步函数并等待
来源：http://ppw.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://tvs.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gvl.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://rem.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://whs.yfazqb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cra.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wud.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://kmo.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://vrp.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://uzt.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://xfq.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bcn.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://yhg.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://yhv.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qxj.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xkp.cucudq.cn

Ruby: threads.map(&:join)
来源：http://ogd.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://edu.hfpthk.cn


<!-- 参考信息 -->