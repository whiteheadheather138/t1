代发 wailian999

Go:   encoding/gob
来源：http://dnz.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://wsx.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uod.hongshengwenyu.top

================================================================================
来源：http://lqe.yj20258.top

L. 网络请求
来源：http://ium.havefunace.top

================================================================================
来源：http://ica.svipenyu.cn

[L01] 发送 GET 请求
来源：http://vyx.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqe.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rfk.hnqzz.top

JS:   await fetch(url)
来源：http://cxb.chenlongwang.top

TS:   await fetch(url)
来源：http://yls.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xxf.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://fkr.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mjp.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mkg.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://fqo.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://csy.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jhs.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nmp.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gkx.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://szn.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://usm.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ove.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wgj.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://dfc.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjc.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tye.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ezj.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ngs.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oyt.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xfw.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yyo.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rwd.ydzc1.top

[L04] 设置超时
来源：http://atj.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://iwl.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qrl.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hhs.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pcx.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sfp.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vjo.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yvp.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qap.cheryme.top

[L05] 上传文件（multipart）
来源：http://aft.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jtx.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kdq.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ord.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ooc.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bry.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lwv.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://voy.dianchejie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jzf.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://nts.zhongyouzk.top

Py:   resp.json()
来源：http://flb.yj202588.top

PHP:  json_decode($body, true);
来源：http://onh.fzhhl.top

JS:   await resp.json()
来源：http://ebk.zhoulong.xyz

TS:   await resp.json()
来源：http://rij.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hti.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tut.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://ixf.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktz.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://uqq.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cdi.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tis.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://alv.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://pfg.gotoacloud.top

Java: resp.statusCode()
来源：http://pav.tianlin.xyz

Go:   resp.StatusCode
来源：http://stg.yuanzhike.top

Ruby: resp.code.to_i
来源：http://yui.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://jpu.jqgfzy.top

[L08] 并发请求多个地址
来源：http://ruw.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nyo.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://bhl.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfa.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xew.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zvp.feifeiyinyue.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jbi.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hwy.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tce.hcnkem.com

================================================================================
来源：http://cjt.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://ums.cdnleiting.top

================================================================================
来源：http://iyr.vqdsnc.cn

[M01] 读取命令行参数
来源：http://qey.cqqwz.cn

Py:   sys.argv[1:]
来源：http://aiq.sxryk.cn

PHP:  $argv;  $argc;
来源：http://iug.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://rde.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://dfp.9152youxi.cn

Java: args 数组（main 方法参数）
来源：http://vlh.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://nxl.gaohongyu789.top

Ruby: ARGV
来源：http://nub.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://bhf.yangfankeji.com

[M02] 读取环境变量
来源：http://rjv.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://azf.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zde.birdmap.top

JS:   process.env.HOME
来源：http://kui.jqgufenzy.top

TS:   process.env.HOME
来源：http://hed.zhixingplan.top

Java: System.getenv("HOME")
来源：http://yxz.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kvx.zycfv.cn

Ruby: ENV["HOME"]
来源：http://cih.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gar.gzhubu.top

[M03] 执行外部命令
来源：http://dxc.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fep.ydjk.org.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hsz.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ezv.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lhc.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zuv.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qhv.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://sgu.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://ttr.havefunace.top

[M04] 获取当前工作目录
来源：http://vsy.hywenlv.cn

Py:   os.getcwd()
来源：http://lfi.pycfn.com

PHP:  getcwd();
来源：http://hbv.wangshuangyany.cn

JS:   process.cwd()
来源：http://wtc.tarul.cn

TS:   process.cwd()
来源：http://otq.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://vmt.yangfankeji.com

Go:   os.Getwd()
来源：http://wtl.quarkkingdee.top

Ruby: Dir.pwd
来源：http://jvf.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mcf.tianlin.xyz

[M05] 设置退出码
来源：http://ncq.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://qvo.guannengcc.top

PHP:  exit(1);
来源：http://mmu.zhengqikj.top

JS:   process.exit(1)
来源：http://fhh.jyoumei.cn

TS:   process.exit(1)
来源：http://vdn.xziqi.cn

Java: System.exit(1)
来源：http://ppg.guannengcc.top

Go:   os.Exit(1)
来源：http://bai.0kj1m.cn

Ruby: exit 1
来源：http://hys.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gfb.hfpthk.cn

[M06] 向标准错误输出
来源：http://css.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://dnd.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sxw.snrcjt.cn

JS:   console.error("err")
来源：http://oph.jinqigufen.top

TS:   console.error("err")
来源：http://aub.cheryme.top

Java: System.err.println("err")
来源：http://acf.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jto.jqgufenzy.top

Ruby: warn "err"
来源：http://hdk.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://dfd.smart0.xyz

[M07] 判断是否为主入口
来源：http://ikn.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://gty.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nxg.ydjk.org.cn

JS:   require.main === module
来源：http://hck.iojbl.cn

TS:   require.main === module
来源：http://fpl.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://kge.yangfankeji.com

Go:   func main()
来源：http://edl.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://elv.hammf.cn

C#:   static void Main(string[] args)
来源：http://pqk.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://efq.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://unx.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://dym.fktsv.cn

JS:   process.platform;  process.version
来源：http://ell.birdmap.top

TS:   process.platform;  process.version
来源：http://ptk.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nnv.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ica.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jjh.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jjy.chenjidiqi.icu

================================================================================
来源：http://ahg.bbcook.cn

N. 数据结构与算法
来源：http://ffr.jqgfzy.top

================================================================================
来源：http://psm.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://fgc.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jhn.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ftp.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hyy.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rmb.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://hfe.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://xhd.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbj.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://ber.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://hhr.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://kvy.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cen.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rbu.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://coq.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rrj.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://mju.hongshengwenyu.top

Ruby: arr.sort
来源：http://jch.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yes.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://uve.zhiwuduotai.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gfy.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://lrb.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppr.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sbl.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sjg.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sbq.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://err.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://iiq.316326.xyz

[N04] 斐波那契数列
来源：http://bcm.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lmh.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rdv.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vfn.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uwq.yueranfly.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qce.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qzz.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xgy.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://itg.fengsongda.top

[N05] 最大公约数
来源：http://fnl.yueranfly.top

Py:   math.gcd(a, b)
来源：http://ult.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fbq.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snq.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixg.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zdp.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jwt.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://qul.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vyc.jinqigfzy.top

[N06] 判断回文字符串
来源：http://tyk.fktsv.cn

Py:   s == s[::-1]
来源：http://bqj.redwolf501.top

PHP:  $s === strrev($s);
来源：http://yax.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://zku.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://xen.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bkf.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://uaq.shzxlz.cn

Ruby: s == s.reverse
来源：http://puj.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yzu.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://tef.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tom.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vvq.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://faf.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://lod.uphjek.com

Java: // 手写 HashMap
来源：http://fcq.mhx1999.top

Go:   // 手写 map[int]int
来源：http://fgb.gogol.net.cn

Ruby: // 手写 Hash
来源：http://nup.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://inf.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://jgy.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://mkt.9152youxi.cn

PHP:  // 手写递归交换
来源：http://vvt.pycfn.com

JS:   // 手写回溯递归
来源：http://gue.svipenyu.cn

TS:   // 手写回溯递归
来源：http://nlp.xziqi.cn

Java: // 手写回溯递归
来源：http://uaz.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://sjg.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://idk.hfpthk.cn

C#:   // 手写回溯递归
来源：http://rda.yvedp.cn

[N09] 栈与队列
来源：http://vut.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zro.yonumen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zan.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ivk.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pyq.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kgc.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ivv.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uhp.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vja.hnxiangtu.top

[N10] 链表节点定义
来源：http://lej.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dyv.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qgh.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyl.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fot.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://zqk.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://ayy.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://pzu.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sln.yfazqb.com

[N11] 二叉树中序遍历
来源：http://eaa.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qkc.yj202588.top

PHP:  // 手写递归函数
来源：http://vch.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndy.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zfu.ivvv.top

Java: // 手写递归
来源：http://uvq.jianghu66.top

Go:   // 手写递归
来源：http://vnq.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kwx.c1oappe.top

C#:   // 手写递归
来源：http://yxb.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mbk.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oua.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uaa.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqg.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://puv.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vyz.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbr.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jfw.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lkb.zdbjq.cn

================================================================================
来源：http://rcy.wangdashe.top

O. 并发与异步
来源：http://bac.jinyuanbaomall.cn

================================================================================
来源：http://abs.ivvv.top

[O01] 启动一个线程
来源：http://zlf.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://diu.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qls.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://krx.svipenyu.cn

TS:   // 同 JS
来源：http://vcx.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://epr.zhixingplan.top

Go:   go f()
来源：http://usv.tarul.cn

Ruby: Thread.new { f }
来源：http://yvj.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://rsj.xuetiantiany.cn

[O02] 使用线程池
来源：http://orh.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jhj.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yus.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://gvw.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://crp.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://jlk.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yff.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oym.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fqq.tian-w.cn

[O03] 加锁保护共享数据
来源：http://dux.yj202588.top

Py:   with lock: shared += 1
来源：http://uzz.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://fbq.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bcw.shanyushiyangtech.top

TS:   // 同 JS
来源：http://bcv.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://iaj.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vmf.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://snv.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://obs.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://kba.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://wpv.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yxv.yueranfly.top

JS:   async function f() { await g(); }
来源：http://hpp.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://esh.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://adv.nanxuanxn.top


<!-- 参考信息 -->