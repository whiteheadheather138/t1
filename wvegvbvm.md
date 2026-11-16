代发 wailian999

L. 网络请求
来源：http://zqj.jinqigufen.top

================================================================================
来源：http://kke.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://ftu.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vud.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nik.feifeiyinyue.top

JS:   await fetch(url)
来源：http://xpo.fzhhl.top

TS:   await fetch(url)
来源：http://cqr.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hvh.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://ixy.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hwy.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ylz.xylfe.cn

[L02] 发送 POST JSON
来源：http://bdg.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://azn.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://edf.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kpu.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxf.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://spf.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yhq.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ehu.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://egr.ydzc1.top

[L03] 设置自定义请求头
来源：http://rao.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oli.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jiq.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://giw.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akg.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uzf.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pkm.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bbj.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mpp.jqgfzy.top

[L04] 设置超时
来源：http://qym.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://idc.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nmj.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kce.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fym.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jxn.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pmw.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://huu.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jgk.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://vye.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xny.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vwt.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uim.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zej.zdqjudy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vyn.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zwq.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wkm.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://loi.ehwqpu.com

[L06] 解析响应为 JSON
来源：http://oia.cqqwz.cn

Py:   resp.json()
来源：http://ptn.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://fwf.yongpay.top

JS:   await resp.json()
来源：http://llp.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://hhj.jlsjyb.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qkj.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hao.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://ieb.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dbz.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://hub.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ysz.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://drr.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://kcl.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://wdf.hcnkem.com

Java: resp.statusCode()
来源：http://aiy.hysaishi.cn

Go:   resp.StatusCode
来源：http://swb.ydzc1.top

Ruby: resp.code.to_i
来源：http://wmo.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://stu.xuanzx.com

[L08] 并发请求多个地址
来源：http://isn.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nzu.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://quc.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yzz.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dda.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ogs.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gba.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://paa.fehbvm.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cnz.zhengqikj.top

================================================================================
来源：http://tbm.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://ekf.yj20258888.top

================================================================================
来源：http://swp.kuanghao11.cn

[M01] 读取命令行参数
来源：http://whp.nanxinkj.top

Py:   sys.argv[1:]
来源：http://rwu.birdmap.top

PHP:  $argv;  $argc;
来源：http://yqu.redwolf501.top

JS:   process.argv.slice(2)
来源：http://dau.yj20258888.top

TS:   process.argv.slice(2)
来源：http://ncy.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://hym.hnxiangtu.top

Go:   os.Args[1:]
来源：http://hjf.smart0.xyz

Ruby: ARGV
来源：http://szb.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://dvn.jiagoushi.top

[M02] 读取环境变量
来源：http://mrx.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://vic.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zrp.daria6918.cn

JS:   process.env.HOME
来源：http://hit.hfpthk.cn

TS:   process.env.HOME
来源：http://yfv.chenlongwang.top

Java: System.getenv("HOME")
来源：http://xld.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://npa.daxiang520.top

Ruby: ENV["HOME"]
来源：http://ktl.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mae.zhoulong.xyz

[M03] 执行外部命令
来源：http://kem.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://npt.shanyushiyangtech.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tfu.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xbz.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wbk.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ezx.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hjn.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://koh.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://pce.uphjek.com

[M04] 获取当前工作目录
来源：http://xll.daria6918.cn

Py:   os.getcwd()
来源：http://qji.xziqi.cn

PHP:  getcwd();
来源：http://grj.wangdashe.top

JS:   process.cwd()
来源：http://fpe.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://tmr.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://oxl.hongshengwenyu.top

Go:   os.Getwd()
来源：http://mmd.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://bnm.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://yjr.guannengcc.top

[M05] 设置退出码
来源：http://fxr.yj20258888.top

Py:   sys.exit(1)
来源：http://lhv.zdbjq.cn

PHP:  exit(1);
来源：http://gwk.yj202588.top

JS:   process.exit(1)
来源：http://kai.ctjpmb.com

TS:   process.exit(1)
来源：http://byp.ydjk.org.cn

Java: System.exit(1)
来源：http://vlk.xziqi.cn

Go:   os.Exit(1)
来源：http://bpf.nanxuanxn.top

Ruby: exit 1
来源：http://dor.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pgv.svipenyu.cn

[M06] 向标准错误输出
来源：http://bgu.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://izh.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://nsg.shanyushiyangtech.top

JS:   console.error("err")
来源：http://lwq.tanke756.top

TS:   console.error("err")
来源：http://ais.kuanghao11.cn

Java: System.err.println("err")
来源：http://dlf.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eth.sysykeji.top

Ruby: warn "err"
来源：http://vfj.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://dlz.gzhubu.top

[M07] 判断是否为主入口
来源：http://jlr.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://bjm.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pyj.shzxlz.cn

JS:   require.main === module
来源：http://rxs.yonumen.top

TS:   require.main === module
来源：http://zwm.guannengcc.top

Java: public static void main(String[] args)
来源：http://nne.ywan-chungtsiang.top

Go:   func main()
来源：http://jlz.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hvf.gzhubu.top

C#:   static void Main(string[] args)
来源：http://ohb.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://psl.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://nyo.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://oxd.bbcook.cn

JS:   process.platform;  process.version
来源：http://jlt.aizwys.cn

TS:   process.platform;  process.version
来源：http://ltq.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vor.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fvi.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bbh.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://gee.tianlin.xyz

================================================================================
来源：http://miw.uphjek.com

N. 数据结构与算法
来源：http://aab.chenjidiqi.icu

================================================================================
来源：http://apv.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://dfy.tian-w.cn

Py:   bisect.bisect_left(arr, x)
来源：http://izr.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ecg.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sxr.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oqs.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://uoh.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://rrd.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pgs.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://tdl.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://lta.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://rze.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pkr.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://toq.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://evp.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yya.fengsongda.top

Go:   slices.Sort(arr)
来源：http://grj.fengsongda.top

Ruby: arr.sort
来源：http://wue.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dtg.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://lzl.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dow.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://bdj.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pke.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bjk.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://chf.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uew.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aoy.quarkkingdee.top

C#:   // 手写递归，或 Array.Sort
来源：http://hey.zycfv.cn

[N04] 斐波那契数列
来源：http://slu.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uoa.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://utw.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yrj.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://szj.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yis.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rsu.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yxs.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://orv.tanke756.top

[N05] 最大公约数
来源：http://rnm.tarul.cn

Py:   math.gcd(a, b)
来源：http://vor.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ymp.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bqe.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zwf.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qjb.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nqk.andypj.xyz

Ruby: a.gcd(b)
来源：http://cyt.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://frf.ybcxt.top

[N06] 判断回文字符串
来源：http://utk.hnqzz.top

Py:   s == s[::-1]
来源：http://xgo.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://dxz.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://ocw.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://ass.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mhs.vehdjk.com

Go:   // 双指针从两端比较
来源：http://hnn.hysaishi.cn

Ruby: s == s.reverse
来源：http://qkk.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://brb.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://fqm.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ssl.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xlq.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ddv.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://fif.shuidangran.top

Java: // 手写 HashMap
来源：http://mqx.meibo888.top

Go:   // 手写 map[int]int
来源：http://xzk.havefunace.top

Ruby: // 手写 Hash
来源：http://zmd.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://czi.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://qec.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://vxe.yanxiufei.cn

PHP:  // 手写递归交换
来源：http://ybw.jianghu66.top

JS:   // 手写回溯递归
来源：http://wrb.yvedp.cn

TS:   // 手写回溯递归
来源：http://lyg.gzhubu.top

Java: // 手写回溯递归
来源：http://bpr.nwbrower.top

Go:   // 手写回溯递归
来源：http://caa.hammf.cn

Ruby: arr.permutation.to_a
来源：http://rit.ybcxt.top

C#:   // 手写回溯递归
来源：http://ocf.yj202588.top

[N09] 栈与队列
来源：http://wtk.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jvt.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ydt.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xpg.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uyb.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtb.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hjw.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bhi.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://abl.zycfv.cn

[N10] 链表节点定义
来源：http://yxg.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pbg.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://hby.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ied.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rzs.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://wwv.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://rse.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pqw.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ece.bbcook.cn

[N11] 二叉树中序遍历
来源：http://zfj.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fzc.ybcxt.top

PHP:  // 手写递归函数
来源：http://doj.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pwe.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gam.52xcode.cn

Java: // 手写递归
来源：http://dsr.xuetiantiany.cn

Go:   // 手写递归
来源：http://igs.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mjh.hfpthk.cn

C#:   // 手写递归
来源：http://fro.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kch.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hhx.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ldu.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ghv.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ofu.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zos.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zot.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kxb.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fnb.chenjidiqi.icu

================================================================================
来源：http://ebd.daria6918.cn

O. 并发与异步
来源：http://iuk.jinyuanbaomall.cn

================================================================================
来源：http://peo.zhiwuduotai.top

[O01] 启动一个线程
来源：http://map.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fdh.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bjv.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fjb.nanxinkj.top

TS:   // 同 JS
来源：http://nif.sweek.top

Java: new Thread(() -> f()).start()
来源：http://psz.sxryk.cn

Go:   go f()
来源：http://fev.aizwys.cn

Ruby: Thread.new { f }
来源：http://jrd.cucudq.cn

C#:   Task.Run(() => F());
来源：http://tqj.cqqwz.cn

[O02] 使用线程池
来源：http://sfz.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://scu.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pao.cucudq.cn

JS:   // worker_threads 线程池
来源：http://set.mhx1999.top

TS:   // worker_threads 线程池
来源：http://jjt.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://ctz.316326.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfy.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vgz.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tlu.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://ytt.sufxvd.cn

Py:   with lock: shared += 1
来源：http://fku.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://hrh.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ugi.hysaishi.cn

TS:   // 同 JS
来源：http://asj.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://bza.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qvh.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://owo.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://gdc.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://jti.sweek.top

Py:   async def f():⏎    await g()
来源：http://nmx.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rfs.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://ylk.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xdl.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nyx.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://djg.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://eup.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://nik.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://aye.shanyushiyangtech.top


<!-- 参考信息 -->