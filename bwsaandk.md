代发 wailian999

Go:   encoding/gob
来源：http://bfo.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://ift.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ywg.ppjwa.cn

================================================================================
来源：http://pns.hcnkem.com

L. 网络请求
来源：http://tyy.cashguo.top

================================================================================
来源：http://ggm.c1oappe.top

[L01] 发送 GET 请求
来源：http://fcm.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tqq.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gpz.jqgfzy.top

JS:   await fetch(url)
来源：http://gcl.xylfe.cn

TS:   await fetch(url)
来源：http://ljb.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qns.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://aqi.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://goh.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bbo.tian-w.cn

[L02] 发送 POST JSON
来源：http://imn.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://afb.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nmg.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fgz.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lbd.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://utu.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pry.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://asg.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oow.yongpay.top

[L03] 设置自定义请求头
来源：http://sxi.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://crp.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nwd.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tqt.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vay.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://obg.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ufl.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ymp.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dro.ehwqpu.com

[L04] 设置超时
来源：http://zjx.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://kvr.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wyi.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yjd.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kmg.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://frk.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aaz.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://evj.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ewq.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://iqa.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jig.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ocx.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hto.zhixingplan.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nwa.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wdv.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rpl.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bwj.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kqc.yj202588.top

[L06] 解析响应为 JSON
来源：http://qqm.yuanzhike.top

Py:   resp.json()
来源：http://pyk.hammf.cn

PHP:  json_decode($body, true);
来源：http://xmw.smart0.xyz

JS:   await resp.json()
来源：http://urb.xuanzx.com

TS:   await resp.json()
来源：http://ube.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xvu.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjl.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ddk.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ikt.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://quk.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ogq.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pcg.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://mxe.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://dla.yangfankeji.com

Java: resp.statusCode()
来源：http://pvo.yangfankeji.com

Go:   resp.StatusCode
来源：http://gjx.wangdashe.top

Ruby: resp.code.to_i
来源：http://fjw.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://pzd.cqqwz.cn

[L08] 并发请求多个地址
来源：http://ohd.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hqg.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://cmm.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://njd.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rda.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwo.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://byl.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vlm.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qro.fktsv.cn

================================================================================
来源：http://ktw.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://rjy.yonumen.top

================================================================================
来源：http://njp.hesvh.cn

[M01] 读取命令行参数
来源：http://tgy.zdqjudy.top

Py:   sys.argv[1:]
来源：http://eau.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://bwr.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://env.zhixingplan.top

TS:   process.argv.slice(2)
来源：http://hzs.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://bne.cucudq.cn

Go:   os.Args[1:]
来源：http://vco.cdnleiting.top

Ruby: ARGV
来源：http://khm.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://ref.yangfankeji.com

[M02] 读取环境变量
来源：http://noq.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://vzc.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rth.fzhhl.top

JS:   process.env.HOME
来源：http://hce.haohaochexian.top

TS:   process.env.HOME
来源：http://gmp.tianlin.xyz

Java: System.getenv("HOME")
来源：http://ahp.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pdw.yj20258888.top

Ruby: ENV["HOME"]
来源：http://sdm.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rax.yonumen.top

[M03] 执行外部命令
来源：http://nnm.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://inv.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://btv.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lhf.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://byy.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://htu.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jnp.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jzr.jinyuanbaomall.cn

C#:   Process.Start("ls", "-l");
来源：http://rcd.hysaishi.cn

[M04] 获取当前工作目录
来源：http://emq.fktsv.cn

Py:   os.getcwd()
来源：http://xdd.jianghu66.top

PHP:  getcwd();
来源：http://rdl.zdbjq.cn

JS:   process.cwd()
来源：http://mhl.daria6918.cn

TS:   process.cwd()
来源：http://ptd.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://pjs.epnwcf.com

Go:   os.Getwd()
来源：http://nrd.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://pgr.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://eec.vehdjk.com

[M05] 设置退出码
来源：http://hdl.guannengcc.top

Py:   sys.exit(1)
来源：http://ykk.jianghu66.top

PHP:  exit(1);
来源：http://yoi.vqdsnc.cn

JS:   process.exit(1)
来源：http://cbu.shzxlz.cn

TS:   process.exit(1)
来源：http://omh.chenlongwang.top

Java: System.exit(1)
来源：http://jij.hammf.cn

Go:   os.Exit(1)
来源：http://wyp.fengsongda.top

Ruby: exit 1
来源：http://ldh.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cdw.andypj.xyz

[M06] 向标准错误输出
来源：http://hke.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://jfh.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fdv.yj20258.top

JS:   console.error("err")
来源：http://qoq.jinghuilouyu.cn

TS:   console.error("err")
来源：http://ciq.pengpengdd.cyou

Java: System.err.println("err")
来源：http://jir.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bgh.gotoacloud.top

Ruby: warn "err"
来源：http://nna.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://qih.smart0.xyz

[M07] 判断是否为主入口
来源：http://mfa.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://rpe.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ibb.yvedp.cn

JS:   require.main === module
来源：http://imm.chenzaomai.com

TS:   require.main === module
来源：http://xrb.snrcjt.cn

Java: public static void main(String[] args)
来源：http://uyg.shanyushiyangtech.top

Go:   func main()
来源：http://yin.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vlt.hnqzz.top

C#:   static void Main(string[] args)
来源：http://ejc.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://mxu.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://yzn.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://wjb.uphjek.com

JS:   process.platform;  process.version
来源：http://gfz.hywenlv.cn

TS:   process.platform;  process.version
来源：http://ari.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://enx.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tqn.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jbg.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://szh.dashuyun.cn

================================================================================
来源：http://bzp.sysykeji.top

N. 数据结构与算法
来源：http://cbb.tian-w.cn

================================================================================
来源：http://ebh.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://lki.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://zrb.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fbz.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfj.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkz.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kak.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://wdy.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jtv.quarkkingdee.top

C#:   Array.BinarySearch(arr, x)
来源：http://xga.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://exk.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://rgq.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://moe.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gjj.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fno.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kvk.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://hrl.daxiang520.top

Ruby: arr.sort
来源：http://lvz.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xwi.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://fhy.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zai.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://vxj.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvf.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xkv.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tkr.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jto.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aae.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ghm.yuxming.cn

[N04] 斐波那契数列
来源：http://abs.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kyp.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://byv.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whc.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kpy.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zeb.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eaw.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sgb.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://erc.jlsjyb.cn

[N05] 最大公约数
来源：http://fpw.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://rar.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sxn.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eah.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pds.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fuz.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vbn.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://tac.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rlc.tarul.cn

[N06] 判断回文字符串
来源：http://fbf.ctjpmb.com

Py:   s == s[::-1]
来源：http://lvl.hammf.cn

PHP:  $s === strrev($s);
来源：http://nnj.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://tdz.daxiang520.top

TS:   s === [...s].reverse().join("")
来源：http://kzr.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fjd.iojbl.cn

Go:   // 双指针从两端比较
来源：http://ynp.tanke756.top

Ruby: s == s.reverse
来源：http://cax.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xxb.tarul.cn

[N07] 两数之和（返回下标）
来源：http://mzo.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uka.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://btz.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nex.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://buk.jianghu66.top

Java: // 手写 HashMap
来源：http://okc.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://uns.hesvh.cn

Ruby: // 手写 Hash
来源：http://bdb.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://bek.52xcode.cn

[N08] 生成全排列
来源：http://wmz.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://hvw.snrcjt.cn

PHP:  // 手写递归交换
来源：http://gkq.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://oxj.nwbrower.top

TS:   // 手写回溯递归
来源：http://dis.c1oappe.top

Java: // 手写回溯递归
来源：http://euk.xziqi.cn

Go:   // 手写回溯递归
来源：http://vkf.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://dlr.yongpay.top

C#:   // 手写回溯递归
来源：http://upi.nwbrower.top

[N09] 栈与队列
来源：http://gtz.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dul.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fju.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://iuj.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kyo.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wlz.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vai.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rkv.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uqo.ctjpmb.com

[N10] 链表节点定义
来源：http://iip.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dvk.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mcl.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mds.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sxn.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://biu.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ahh.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://rbp.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ezw.316326.xyz

[N11] 二叉树中序遍历
来源：http://cjn.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wcb.shzxlz.cn

PHP:  // 手写递归函数
来源：http://fgp.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ynm.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nmv.hnxiangtu.top

Java: // 手写递归
来源：http://xog.cucudq.cn

Go:   // 手写递归
来源：http://juq.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ydu.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://zgr.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mdj.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fnj.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dww.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xqn.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dul.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yju.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyq.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uwm.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uof.cdnleiting.top

================================================================================
来源：http://sfp.daria6918.cn

O. 并发与异步
来源：http://gic.vehdjk.com

================================================================================
来源：http://fwk.dashuyun.cn

[O01] 启动一个线程
来源：http://vxd.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vmq.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gea.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ckk.gogol.net.cn

TS:   // 同 JS
来源：http://fvq.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://wkh.svipenyu.cn

Go:   go f()
来源：http://qeo.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://wer.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://gxi.gzhubu.top

[O02] 使用线程池
来源：http://dkf.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tul.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pbp.fzhhl.top

JS:   // worker_threads 线程池
来源：http://cdc.fktsv.cn

TS:   // worker_threads 线程池
来源：http://dij.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://dci.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lhv.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cif.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fnp.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://oas.gotoacloud.top

Py:   with lock: shared += 1
来源：http://oey.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://blb.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qwu.birdmap.top

TS:   // 同 JS
来源：http://rza.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://dsf.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bhf.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://obx.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://qgr.xylfe.cn

[O04] 定义异步函数并等待
来源：http://hsr.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://hho.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mhw.yj20258.top

JS:   async function f() { await g(); }
来源：http://lqg.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oju.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qeo.meibo888.top


<!-- 参考信息 -->