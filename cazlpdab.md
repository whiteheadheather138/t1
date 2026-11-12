代发 wailian999

Go:   encoding/gob
来源：http://wti.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://bey.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gub.zhengqikj.top

================================================================================
来源：http://qps.aizwys.cn

L. 网络请求
来源：http://nwb.sufxvd.cn

================================================================================
来源：http://xgp.snrcjt.cn

[L01] 发送 GET 请求
来源：http://huh.wangshuangyany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ggx.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zpb.yuanzhike.top

JS:   await fetch(url)
来源：http://mzy.sweek.top

TS:   await fetch(url)
来源：http://hew.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uui.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://ahh.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wwb.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rzz.tianlin.xyz

[L02] 发送 POST JSON
来源：http://lgy.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://nki.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://atw.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ebp.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xfv.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ckf.snrcjt.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mlw.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tzs.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nzp.aibaodan.cn

[L03] 设置自定义请求头
来源：http://zwa.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jos.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mza.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tio.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vaq.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://oni.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xbe.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dlc.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tgc.hongshengwenyu.top

[L04] 设置超时
来源：http://qkz.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://hou.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://toa.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ieh.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pfp.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fji.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mtq.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qff.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ytl.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://ptb.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zqu.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ovf.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jeh.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uak.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bqr.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zof.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hre.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mfa.cashguo.top

[L06] 解析响应为 JSON
来源：http://ppa.vqdsnc.cn

Py:   resp.json()
来源：http://qia.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://tnz.cqqwz.cn

JS:   await resp.json()
来源：http://cok.sjlbkw.cn

TS:   await resp.json()
来源：http://iwt.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyf.shangyingyoupin.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wlq.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://rqz.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nop.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://nzi.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ivv.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://klc.yj20258.top

JS:   resp.ok;  resp.status
来源：http://yju.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://xyz.cdnleiting.top

Java: resp.statusCode()
来源：http://kzd.cheryme.top

Go:   resp.StatusCode
来源：http://exx.0kj1m.cn

Ruby: resp.code.to_i
来源：http://hvs.zdqjudy.top

C#:   (int)resp.StatusCode
来源：http://mrh.ydzc1.top

[L08] 并发请求多个地址
来源：http://fyj.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zcn.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://bdq.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tkw.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yoc.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fps.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zzu.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://upb.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ouu.yonumen.top

================================================================================
来源：http://yub.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://xia.zycfv.cn

================================================================================
来源：http://loj.ppjwa.cn

[M01] 读取命令行参数
来源：http://nxt.tanke756.top

Py:   sys.argv[1:]
来源：http://fez.yonumen.top

PHP:  $argv;  $argc;
来源：http://quc.guannengcc.top

JS:   process.argv.slice(2)
来源：http://gjq.mhx1999.top

TS:   process.argv.slice(2)
来源：http://jmp.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://dzh.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://auq.hywenlv.cn

Ruby: ARGV
来源：http://hwq.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://gee.pengpengdd.cyou

[M02] 读取环境变量
来源：http://oak.bbcook.cn

Py:   os.environ.get("HOME")
来源：http://pnc.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rvm.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://woz.zdqjudy.top

TS:   process.env.HOME
来源：http://dxq.yueranfly.top

Java: System.getenv("HOME")
来源：http://tqz.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://saw.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://fuz.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dwd.0kj1m.cn

[M03] 执行外部命令
来源：http://sxj.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://veg.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dac.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xhx.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nic.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zlj.fzhhl.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xod.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://iod.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://mxu.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://xfc.jinqigfzy.top

Py:   os.getcwd()
来源：http://iwb.hammf.cn

PHP:  getcwd();
来源：http://tqh.xziqi.cn

JS:   process.cwd()
来源：http://gog.fanxiaobao.xyz

TS:   process.cwd()
来源：http://tme.jinghuilouyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://bzv.chenlongwang.top

Go:   os.Getwd()
来源：http://eys.jianghu66.top

Ruby: Dir.pwd
来源：http://rwk.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://mbc.yuanzhike.top

[M05] 设置退出码
来源：http://pkd.zdqjudy.top

Py:   sys.exit(1)
来源：http://ilh.zdqjudy.top

PHP:  exit(1);
来源：http://geh.jinqigfzy.top

JS:   process.exit(1)
来源：http://bfc.nanxinkj.top

TS:   process.exit(1)
来源：http://ufm.sxryk.cn

Java: System.exit(1)
来源：http://xuk.fehbvm.com

Go:   os.Exit(1)
来源：http://uwh.zdbjq.cn

Ruby: exit 1
来源：http://erv.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wgq.xinyue.icu

[M06] 向标准错误输出
来源：http://zre.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://qri.jinqigfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xwa.jinqigfzy.top

JS:   console.error("err")
来源：http://ihv.ctjpmb.com

TS:   console.error("err")
来源：http://kda.xuanzx.com

Java: System.err.println("err")
来源：http://hms.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bnd.haohaochexian.top

Ruby: warn "err"
来源：http://kqj.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://ejl.dashuyun.cn

[M07] 判断是否为主入口
来源：http://zem.tarul.cn

Py:   if __name__ == "__main__":
来源：http://len.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://szx.andypj.xyz

JS:   require.main === module
来源：http://cki.xylfe.cn

TS:   require.main === module
来源：http://dzc.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://xsa.yj20258888.top

Go:   func main()
来源：http://vsn.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nbf.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://hhp.yongpay.top

[M08] 获取系统与运行时信息
来源：http://skr.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://xjl.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://xxp.ppjwa.cn

JS:   process.platform;  process.version
来源：http://ijg.mhx1999.top

TS:   process.platform;  process.version
来源：http://cmg.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yxu.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ikk.ywan-chungtsiang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fac.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qkl.tarul.cn

================================================================================
来源：http://iev.hesvh.cn

N. 数据结构与算法
来源：http://wrw.bjfxy.top

================================================================================
来源：http://kvz.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://xgt.jianghu66.top

Py:   bisect.bisect_left(arr, x)
来源：http://xoi.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lkq.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izw.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fyt.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://gmw.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://lxd.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cjj.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://srk.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://imm.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://gab.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dyb.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://atd.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tvu.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wlk.yj20258.top

Go:   slices.Sort(arr)
来源：http://hys.ivvv.top

Ruby: arr.sort
来源：http://fbu.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://etd.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://uuo.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uzp.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://wio.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozf.zhengqikj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eef.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pis.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yco.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://njz.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lpe.hfpthk.cn

[N04] 斐波那契数列
来源：http://hhq.cdnleiting.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zty.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dsd.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://npt.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bid.yj202588.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ezd.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yyw.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gmm.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zei.yj20258.top

[N05] 最大公约数
来源：http://ybv.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://rmh.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eln.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wxx.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogl.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hun.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ngq.zycfv.cn

Ruby: a.gcd(b)
来源：http://xyw.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mme.nanxuanxn.top

[N06] 判断回文字符串
来源：http://ift.zdqjudy.top

Py:   s == s[::-1]
来源：http://gxn.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://iym.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://lji.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://ann.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://anr.yj20258888.top

Go:   // 双指针从两端比较
来源：http://oxh.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://sww.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qjb.jiagoushi.top

[N07] 两数之和（返回下标）
来源：http://jgf.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yxq.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pod.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gwx.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://ipq.dashuyun.cn

Java: // 手写 HashMap
来源：http://vri.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://fxq.fzhhl.top

Ruby: // 手写 Hash
来源：http://pjo.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sgc.meibo888.top

[N08] 生成全排列
来源：http://vhj.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://caq.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://ygm.zhixingplan.top

JS:   // 手写回溯递归
来源：http://iek.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://tap.sufxvd.cn

Java: // 手写回溯递归
来源：http://iqt.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://ebd.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://xhc.xinyue.icu

C#:   // 手写回溯递归
来源：http://hos.xziqi.cn

[N09] 栈与队列
来源：http://vip.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wzk.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qzd.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fhl.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nle.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rrs.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wmk.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zbg.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sdh.zhengqikj.top

[N10] 链表节点定义
来源：http://wgt.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://miw.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://gte.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vui.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yur.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://bgz.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://zgi.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cqz.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kdz.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://dfu.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cdr.yj202588.top

PHP:  // 手写递归函数
来源：http://jtu.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pvd.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yol.gzhubu.top

Java: // 手写递归
来源：http://mpk.316326.xyz

Go:   // 手写递归
来源：http://ejh.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nly.hfpthk.cn

C#:   // 手写递归
来源：http://ynt.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lxc.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mah.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yum.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqu.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wvy.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lmd.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gft.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ule.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://goo.yuanzhike.top

================================================================================
来源：http://hrk.guannengcc.top

O. 并发与异步
来源：http://fvm.hfpthk.cn

================================================================================
来源：http://smr.ppjwa.cn

[O01] 启动一个线程
来源：http://pmb.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cas.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nnj.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qgp.jlsjyb.cn

TS:   // 同 JS
来源：http://hmd.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://etg.sweek.top

Go:   go f()
来源：http://ypc.nwbrower.top

Ruby: Thread.new { f }
来源：http://jcu.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://tpz.nanxuanxn.top

[O02] 使用线程池
来源：http://hsv.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://srk.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uxn.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://ocu.bjfxy.top

TS:   // worker_threads 线程池
来源：http://ymf.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mdm.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://guo.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qtw.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vjq.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://rqc.shzxlz.cn

Py:   with lock: shared += 1
来源：http://ymd.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://srx.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jyx.tarul.cn

TS:   // 同 JS
来源：http://fho.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://hrj.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iyp.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eko.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://vcr.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://rei.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://tef.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uyc.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://qto.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jvs.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://muj.ivvv.top


<!-- 参考信息 -->