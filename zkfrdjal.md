代发 wailian999

L. 网络请求
来源：http://hyr.0kj1m.cn

================================================================================
来源：http://vrb.yfazqb.com

[L01] 发送 GET 请求
来源：http://ide.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://djh.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xoc.ivvv.top

JS:   await fetch(url)
来源：http://ogy.svipenyu.cn

TS:   await fetch(url)
来源：http://aso.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qzn.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://bfy.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rmv.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ica.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://sbt.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hla.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rdt.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dww.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wdf.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kfa.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://csw.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hua.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://elv.hywenlv.cn

[L03] 设置自定义请求头
来源：http://bzx.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hqx.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sdo.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbd.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dab.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uac.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ymp.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xwr.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cng.zhijiandao.cn

[L04] 设置超时
来源：http://ufa.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://plj.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qij.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swz.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyb.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://raa.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rrk.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://akb.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zyj.ppjwa.cn

[L05] 上传文件（multipart）
来源：http://njd.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://huy.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qjv.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zrx.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wdw.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mea.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jdp.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oql.meibo888.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iev.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://jfu.sysykeji.top

Py:   resp.json()
来源：http://stb.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://zdr.fzhhl.top

JS:   await resp.json()
来源：http://jhr.gogol.net.cn

TS:   await resp.json()
来源：http://nlk.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zyj.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jdj.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://uyo.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hfk.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://gsg.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://act.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hpf.316326.xyz

JS:   resp.ok;  resp.status
来源：http://vee.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://ovs.shuidangran.top

Java: resp.statusCode()
来源：http://ghe.zhixingplan.top

Go:   resp.StatusCode
来源：http://jse.gotoacloud.top

Ruby: resp.code.to_i
来源：http://yqa.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://knk.ctjpmb.com

[L08] 并发请求多个地址
来源：http://mlo.uphjek.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ioy.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://xys.0kj1m.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pyd.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imo.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eso.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jjl.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://egn.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ygw.cheryme.top

================================================================================
来源：http://kmn.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://hje.fanxiaobao.xyz

================================================================================
来源：http://pap.gaohongyu789.top

[M01] 读取命令行参数
来源：http://tdz.yuxming.cn

Py:   sys.argv[1:]
来源：http://fgg.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://yjb.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://acv.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://rro.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://zjr.tarul.cn

Go:   os.Args[1:]
来源：http://qia.yj20258.top

Ruby: ARGV
来源：http://cuy.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://qcs.zhijiandao.cn

[M02] 读取环境变量
来源：http://nnp.tanke756.top

Py:   os.environ.get("HOME")
来源：http://trk.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bnv.bjfxy.top

JS:   process.env.HOME
来源：http://gdt.tian-w.cn

TS:   process.env.HOME
来源：http://yzl.yangfankeji.com

Java: System.getenv("HOME")
来源：http://kei.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eci.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://vqm.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kos.snrcjt.cn

[M03] 执行外部命令
来源：http://cgi.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://swk.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://buz.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cgg.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://elj.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kno.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gfp.ctjpmb.com

Ruby: system("ls -l");  `ls -l`
来源：http://lnr.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://ukb.yj202588.top

[M04] 获取当前工作目录
来源：http://dmv.daria6918.cn

Py:   os.getcwd()
来源：http://bns.zhongyouzk.top

PHP:  getcwd();
来源：http://oan.daria6918.cn

JS:   process.cwd()
来源：http://ofg.zhengqikj.top

TS:   process.cwd()
来源：http://emn.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://sjt.yonumen.top

Go:   os.Getwd()
来源：http://vkk.guannengcc.top

Ruby: Dir.pwd
来源：http://lto.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://xmi.yvedp.cn

[M05] 设置退出码
来源：http://yko.hammf.cn

Py:   sys.exit(1)
来源：http://lvw.52xcode.cn

PHP:  exit(1);
来源：http://chx.xuetiantiany.cn

JS:   process.exit(1)
来源：http://yvp.shzxlz.cn

TS:   process.exit(1)
来源：http://xnq.kuanghao11.cn

Java: System.exit(1)
来源：http://dpj.fengsongda.top

Go:   os.Exit(1)
来源：http://hbh.tian-w.cn

Ruby: exit 1
来源：http://uxu.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kfr.hnqzz.top

[M06] 向标准错误输出
来源：http://ofq.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://lsi.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://okm.tianlin.xyz

JS:   console.error("err")
来源：http://mjf.yfazqb.com

TS:   console.error("err")
来源：http://ndm.hnxiangtu.top

Java: System.err.println("err")
来源：http://tse.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bsu.sufxvd.cn

Ruby: warn "err"
来源：http://nkn.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://xqt.jianghu66.top

[M07] 判断是否为主入口
来源：http://fhl.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://jlw.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://von.nanxinkj.top

JS:   require.main === module
来源：http://wnp.feifeiyinyue.top

TS:   require.main === module
来源：http://paa.fktsv.cn

Java: public static void main(String[] args)
来源：http://uyg.yj20258888.top

Go:   func main()
来源：http://ghx.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lvt.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://zhm.316326.xyz

[M08] 获取系统与运行时信息
来源：http://hco.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://suk.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://fzv.shzxlz.cn

JS:   process.platform;  process.version
来源：http://ejn.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://izy.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ecy.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lbd.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wik.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nde.hongshengwenyu.top

================================================================================
来源：http://hye.52xcode.cn

N. 数据结构与算法
来源：http://hrd.xuanzx.com

================================================================================
来源：http://tvd.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://qyw.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mah.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ccd.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gxa.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsu.vqdsnc.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yqu.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://udk.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://duy.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://ikm.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://ues.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://lit.shangyingyoupin.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uwd.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rrc.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dws.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://all.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://dgb.yangfankeji.com

Ruby: arr.sort
来源：http://ega.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qfq.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://rlm.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dzu.tian-w.cn

PHP:  // 递归实现，或用 usort
来源：http://krr.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppo.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fab.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gpg.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pmk.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mqu.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://fpp.shuidangran.top

[N04] 斐波那契数列
来源：http://hzk.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qrb.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bza.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vtr.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dft.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gwv.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iva.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ggx.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gda.wangdashe.top

[N05] 最大公约数
来源：http://zob.daria6918.cn

Py:   math.gcd(a, b)
来源：http://zeq.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hqi.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mmc.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdm.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kth.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uwt.fktsv.cn

Ruby: a.gcd(b)
来源：http://fxn.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zim.gotoacloud.top

[N06] 判断回文字符串
来源：http://rie.tian-w.cn

Py:   s == s[::-1]
来源：http://riy.bjfxy.top

PHP:  $s === strrev($s);
来源：http://kha.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://jjo.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://psm.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://arq.gzhubu.top

Go:   // 双指针从两端比较
来源：http://dfc.yj20258888.top

Ruby: s == s.reverse
来源：http://btm.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ehv.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://bym.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://huy.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pac.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gvf.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://pcv.yvedp.cn

Java: // 手写 HashMap
来源：http://ejb.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://upa.uphjek.com

Ruby: // 手写 Hash
来源：http://vfk.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://fee.sysykeji.top

[N08] 生成全排列
来源：http://fvt.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://lwc.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://drq.nanxinkj.top

JS:   // 手写回溯递归
来源：http://ban.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://btl.52xcode.cn

Java: // 手写回溯递归
来源：http://qcv.ehwqpu.com

Go:   // 手写回溯递归
来源：http://exx.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://cdq.aizwys.cn

C#:   // 手写回溯递归
来源：http://gcg.tian-w.cn

[N09] 栈与队列
来源：http://hyo.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://txy.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vhd.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cfi.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://klp.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aqb.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jlq.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hau.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tjj.svipenyu.cn

[N10] 链表节点定义
来源：http://hua.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tmd.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xak.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qke.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxb.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://laa.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://fsu.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nbn.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pwx.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://tnl.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lua.zycfv.cn

PHP:  // 手写递归函数
来源：http://zso.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gtv.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xoi.sweek.top

Java: // 手写递归
来源：http://yrp.daxiang520.top

Go:   // 手写递归
来源：http://cby.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jvr.zhijiandao.cn

C#:   // 手写递归
来源：http://qic.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gxi.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fux.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gpb.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rlv.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qcx.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mtb.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rwp.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xvn.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pin.zhaomingkeji.xyz

================================================================================
来源：http://lfu.yangfankeji.com

O. 并发与异步
来源：http://tjx.shuidangran.top

================================================================================
来源：http://tdw.redwolf501.top

[O01] 启动一个线程
来源：http://oom.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://agn.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lvn.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mbx.fanxiaobao.xyz

TS:   // 同 JS
来源：http://hde.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://ufd.jlsjyb.cn

Go:   go f()
来源：http://jjj.tanke756.top

Ruby: Thread.new { f }
来源：http://rpo.jianghu66.top

C#:   Task.Run(() => F());
来源：http://fdn.hnxiangtu.top

[O02] 使用线程池
来源：http://xcc.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wzf.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hsx.fehbvm.com

JS:   // worker_threads 线程池
来源：http://cis.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://bhy.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://yxb.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cjw.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oki.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://saw.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://ume.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://two.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://qxc.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://knz.cheryme.top

TS:   // 同 JS
来源：http://rol.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://ckn.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bsj.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lms.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://rrx.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://nby.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://ppf.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bau.uphjek.com

JS:   async function f() { await g(); }
来源：http://vau.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uez.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://whl.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lpa.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://alm.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://qrq.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://ykx.fktsv.cn


<!-- 参考信息 -->