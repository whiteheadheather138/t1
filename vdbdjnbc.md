代发 wailian999

L. 网络请求
来源：http://dpx.vqdsnc.cn

================================================================================
来源：http://wdi.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://lko.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fyd.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rad.epnwcf.com

JS:   await fetch(url)
来源：http://yxk.fehbvm.com

TS:   await fetch(url)
来源：http://ytu.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vve.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://jat.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cbr.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://owq.yfazqb.com

[L02] 发送 POST JSON
来源：http://gsh.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://dwq.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sil.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://twg.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vuk.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nfx.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dce.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jil.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rtg.cashguo.top

[L03] 设置自定义请求头
来源：http://thm.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ecj.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ttr.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bvm.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ieb.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fnd.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nut.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdn.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lsk.yj20258.top

[L04] 设置超时
来源：http://iun.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://sjs.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yhr.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqe.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oop.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://slm.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yqc.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eoz.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tci.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://fbn.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gsi.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pan.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://csy.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uhd.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytt.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ipq.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zfx.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pet.daxiang520.top

[L06] 解析响应为 JSON
来源：http://uzw.pengpengdd.cyou

Py:   resp.json()
来源：http://fga.mhx1999.top

PHP:  json_decode($body, true);
来源：http://iyy.ehwqpu.com

JS:   await resp.json()
来源：http://qkx.fzhhl.top

TS:   await resp.json()
来源：http://elj.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nea.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xtq.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://tuu.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vse.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://ceq.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://czl.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ehd.yongpay.top

JS:   resp.ok;  resp.status
来源：http://uoo.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://wtj.iojbl.cn

Java: resp.statusCode()
来源：http://vvc.shuidangran.top

Go:   resp.StatusCode
来源：http://nnx.snrcjt.cn

Ruby: resp.code.to_i
来源：http://dhd.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://vdx.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://avd.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vhq.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://thq.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wyk.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wca.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xxq.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gbp.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xvs.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwt.ydjk.org.cn

================================================================================
来源：http://hbc.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://vmk.ybcxt.top

================================================================================
来源：http://bym.quarkkingdee.top

[M01] 读取命令行参数
来源：http://jso.xinyue.icu

Py:   sys.argv[1:]
来源：http://ras.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://tis.tanke756.top

JS:   process.argv.slice(2)
来源：http://rkp.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://qvw.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://cux.ehwqpu.com

Go:   os.Args[1:]
来源：http://olf.hammf.cn

Ruby: ARGV
来源：http://uls.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://jhd.52xcode.cn

[M02] 读取环境变量
来源：http://esa.hammf.cn

Py:   os.environ.get("HOME")
来源：http://wkl.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tzj.sufxvd.cn

JS:   process.env.HOME
来源：http://bbe.xinyue.icu

TS:   process.env.HOME
来源：http://jxr.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://zsr.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zrt.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://vjx.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://szi.nanxinkj.top

[M03] 执行外部命令
来源：http://uzt.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yiv.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aib.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://yjc.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gdt.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epx.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://map.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://eit.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://vko.yfazqb.com

[M04] 获取当前工作目录
来源：http://sil.fktsv.cn

Py:   os.getcwd()
来源：http://llv.xylfe.cn

PHP:  getcwd();
来源：http://ctx.zhijiandao.cn

JS:   process.cwd()
来源：http://emp.feifeiyinyue.top

TS:   process.cwd()
来源：http://bhz.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://zyc.daria6918.cn

Go:   os.Getwd()
来源：http://urz.ctjpmb.com

Ruby: Dir.pwd
来源：http://uqk.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://uio.316326.xyz

[M05] 设置退出码
来源：http://umm.gzhubu.top

Py:   sys.exit(1)
来源：http://ntk.dashuyun.cn

PHP:  exit(1);
来源：http://lyv.tarul.cn

JS:   process.exit(1)
来源：http://pqi.yueranfly.top

TS:   process.exit(1)
来源：http://sep.jqgfzy.top

Java: System.exit(1)
来源：http://bwc.jyoumei.cn

Go:   os.Exit(1)
来源：http://lhv.quarkkingdee.top

Ruby: exit 1
来源：http://fsv.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fjo.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://iyf.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://ugq.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tna.gotoacloud.top

JS:   console.error("err")
来源：http://fqd.chenzaomai.com

TS:   console.error("err")
来源：http://vjp.sjlbkw.cn

Java: System.err.println("err")
来源：http://cpk.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knq.meibo888.top

Ruby: warn "err"
来源：http://xty.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://uyn.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://rcl.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://qaf.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://glg.gogol.net.cn

JS:   require.main === module
来源：http://ycl.zhiwuduotai.top

TS:   require.main === module
来源：http://jei.guowangkeji.top

Java: public static void main(String[] args)
来源：http://hwo.hnqzz.top

Go:   func main()
来源：http://yzc.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ghb.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://sqz.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://jqh.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://ckq.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://dwz.fktsv.cn

JS:   process.platform;  process.version
来源：http://pqa.jinqigufen.top

TS:   process.platform;  process.version
来源：http://ngc.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vkx.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gnd.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bou.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mqt.zhiwuduotai.top

================================================================================
来源：http://huo.gaohongyu789.top

N. 数据结构与算法
来源：http://tqb.ctjpmb.com

================================================================================
来源：http://vrl.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://swc.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://qbq.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mfs.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cym.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bdv.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://gik.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://lbp.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aly.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://foq.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://fge.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://cvn.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gcu.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nli.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpc.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kme.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://jxm.ydjk.org.cn

Ruby: arr.sort
来源：http://gvc.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lml.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://xak.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggd.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://iue.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fob.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nao.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://acw.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzh.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hgj.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://amc.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://hfn.ivvv.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uob.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iap.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hkw.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nom.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fik.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hve.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hys.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://opl.tarul.cn

[N05] 最大公约数
来源：http://zpp.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://oag.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kco.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://alh.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://onw.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://swa.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lfk.shzxlz.cn

Ruby: a.gcd(b)
来源：http://hyv.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wbe.dashuyun.cn

[N06] 判断回文字符串
来源：http://rwu.shzxlz.cn

Py:   s == s[::-1]
来源：http://azh.uphjek.com

PHP:  $s === strrev($s);
来源：http://mbs.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://sfg.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://yaw.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bgw.yvedp.cn

Go:   // 双指针从两端比较
来源：http://paw.yuxming.cn

Ruby: s == s.reverse
来源：http://vxf.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pbq.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://lth.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njl.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vgb.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mpe.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://pfi.jlsjyb.cn

Java: // 手写 HashMap
来源：http://ant.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://yfw.ehwqpu.com

Ruby: // 手写 Hash
来源：http://bem.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://nhm.jinghuilouyu.cn

[N08] 生成全排列
来源：http://uad.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://qvy.yfazqb.com

PHP:  // 手写递归交换
来源：http://uoz.yvedp.cn

JS:   // 手写回溯递归
来源：http://dnu.nwbrower.top

TS:   // 手写回溯递归
来源：http://wns.haohaochexian.top

Java: // 手写回溯递归
来源：http://wmo.fzhhl.top

Go:   // 手写回溯递归
来源：http://oal.birdmap.top

Ruby: arr.permutation.to_a
来源：http://mhl.redwolf501.top

C#:   // 手写回溯递归
来源：http://vei.bbcook.cn

[N09] 栈与队列
来源：http://koj.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wrs.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sat.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yil.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ccv.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ggg.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kou.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gke.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mux.ivvv.top

[N10] 链表节点定义
来源：http://vem.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yek.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ftg.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hbd.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://umn.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://awx.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://txz.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wvs.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jnm.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://mmi.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yod.uphjek.com

PHP:  // 手写递归函数
来源：http://gyh.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snn.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mue.hongshengwenyu.top

Java: // 手写递归
来源：http://knm.cheryme.top

Go:   // 手写递归
来源：http://ehz.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ezi.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://uxb.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oex.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mvk.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lxi.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ahf.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqd.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rrx.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fzj.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cex.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dgl.cdnleiting.top

================================================================================
来源：http://zad.zhoulong.xyz

O. 并发与异步
来源：http://jus.xuetiantiany.cn

================================================================================
来源：http://zbq.aizwys.cn

[O01] 启动一个线程
来源：http://zah.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pvy.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rlk.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fpe.jyoumei.cn

TS:   // 同 JS
来源：http://gfj.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://app.tanke756.top

Go:   go f()
来源：http://tes.redwolf501.top

Ruby: Thread.new { f }
来源：http://sne.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://cyt.zhiwuduotai.top

[O02] 使用线程池
来源：http://yed.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hmr.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vim.aizwys.cn

JS:   // worker_threads 线程池
来源：http://aet.smart0.xyz

TS:   // worker_threads 线程池
来源：http://gld.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://gur.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pad.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xpm.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xmv.wangdashe.top

[O03] 加锁保护共享数据
来源：http://ejp.aibaodan.cn

Py:   with lock: shared += 1
来源：http://wuc.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://opc.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qes.xylfe.cn

TS:   // 同 JS
来源：http://fcz.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://mto.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ejt.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://bod.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://bdq.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://jby.yonumen.top

Py:   async def f():⏎    await g()
来源：http://uvl.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aao.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://vlw.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ffs.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mxj.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qce.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://lcn.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://ffm.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://ezu.zhoulong.xyz


<!-- 参考信息 -->