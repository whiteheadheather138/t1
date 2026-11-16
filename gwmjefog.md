代发 wailian999

Go:   encoding/gob
来源：http://gbw.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://ten.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ott.jinyuanbaomall.cn

================================================================================
来源：http://jzg.sxryk.cn

L. 网络请求
来源：http://tgb.yj20258888.top

================================================================================
来源：http://meo.chenlongwang.top

[L01] 发送 GET 请求
来源：http://rkz.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xuf.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hjq.yangfankeji.com

JS:   await fetch(url)
来源：http://uwz.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://nsc.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mdn.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://uwu.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://afp.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ttw.fktsv.cn

[L02] 发送 POST JSON
来源：http://tls.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jbf.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rxb.pengpengdd.cyou

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzx.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gke.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aax.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lje.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qbx.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vpm.ppjwa.cn

[L03] 设置自定义请求头
来源：http://rez.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://quo.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dlg.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bcm.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lse.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zdr.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hyk.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qas.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bbm.zhaomingkeji.xyz

[L04] 设置超时
来源：http://tqg.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://lnq.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ztg.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qkm.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvs.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dho.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qxi.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cjr.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rkl.tian-w.cn

[L05] 上传文件（multipart）
来源：http://phc.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xrp.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kbq.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tnj.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://exy.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://beq.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nud.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dgm.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ynd.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://bqt.shanyushiyangtech.top

Py:   resp.json()
来源：http://lxh.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://kiz.hfpthk.cn

JS:   await resp.json()
来源：http://gso.yfazqb.com

TS:   await resp.json()
来源：http://yqe.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qis.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://trw.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://wyx.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lnv.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://exx.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rdd.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rkb.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://sgv.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://lop.ppjwa.cn

Java: resp.statusCode()
来源：http://mql.ybcxt.top

Go:   resp.StatusCode
来源：http://qob.vehdjk.com

Ruby: resp.code.to_i
来源：http://pzu.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://euz.ydzc1.top

[L08] 并发请求多个地址
来源：http://dbp.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iri.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://ocb.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iow.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tut.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lfu.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jcv.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://alu.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://opv.ivvv.top

================================================================================
来源：http://phm.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://sgv.tianlin.xyz

================================================================================
来源：http://siw.hysaishi.cn

[M01] 读取命令行参数
来源：http://iuw.52xcode.cn

Py:   sys.argv[1:]
来源：http://ntk.aizwys.cn

PHP:  $argv;  $argc;
来源：http://pbp.ivvv.top

JS:   process.argv.slice(2)
来源：http://xyq.sxryk.cn

TS:   process.argv.slice(2)
来源：http://dwp.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://fuj.bjfxy.top

Go:   os.Args[1:]
来源：http://zjr.ywan-chungtsiang.top

Ruby: ARGV
来源：http://cuu.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://eak.chenzaomai.com

[M02] 读取环境变量
来源：http://bbh.cheryme.top

Py:   os.environ.get("HOME")
来源：http://bqx.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vke.redwolf501.top

JS:   process.env.HOME
来源：http://ifi.shuidangran.top

TS:   process.env.HOME
来源：http://ygu.bjfxy.top

Java: System.getenv("HOME")
来源：http://gah.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lob.yonumen.top

Ruby: ENV["HOME"]
来源：http://goj.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xcz.9152youxi.cn

[M03] 执行外部命令
来源：http://cok.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkt.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fty.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zwb.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rkn.c1oappe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://unz.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rqz.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zcw.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://rgq.9152youxi.cn

[M04] 获取当前工作目录
来源：http://cxy.jyoumei.cn

Py:   os.getcwd()
来源：http://msv.jianghu66.top

PHP:  getcwd();
来源：http://eqp.andypj.xyz

JS:   process.cwd()
来源：http://pci.yj20258.top

TS:   process.cwd()
来源：http://dls.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://vik.wangshuangyany.cn

Go:   os.Getwd()
来源：http://fgb.bjfxy.top

Ruby: Dir.pwd
来源：http://ekz.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bxf.jinqigufen.top

[M05] 设置退出码
来源：http://pqo.yj20258888.top

Py:   sys.exit(1)
来源：http://lma.gaohongyu789.top

PHP:  exit(1);
来源：http://ctn.haohaochexian.top

JS:   process.exit(1)
来源：http://pyw.ehwqpu.com

TS:   process.exit(1)
来源：http://rkv.aizwys.cn

Java: System.exit(1)
来源：http://qiu.chenzaomai.com

Go:   os.Exit(1)
来源：http://mwc.ywan-chungtsiang.top

Ruby: exit 1
来源：http://snr.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ath.aibaodan.cn

[M06] 向标准错误输出
来源：http://mac.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://rtb.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://vhf.yueranfly.top

JS:   console.error("err")
来源：http://rax.gzhubu.top

TS:   console.error("err")
来源：http://wfd.zhiwuduotai.top

Java: System.err.println("err")
来源：http://pma.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fgy.fengsongda.top

Ruby: warn "err"
来源：http://gtt.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://utj.mhx1999.top

[M07] 判断是否为主入口
来源：http://kio.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ybd.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bnq.chenzaomai.com

JS:   require.main === module
来源：http://uto.aibaodan.cn

TS:   require.main === module
来源：http://opt.svipenyu.cn

Java: public static void main(String[] args)
来源：http://efk.jianghu66.top

Go:   func main()
来源：http://psp.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tof.hammf.cn

C#:   static void Main(string[] args)
来源：http://ehc.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://sty.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://wvz.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://fgw.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://xpn.ppjwa.cn

TS:   process.platform;  process.version
来源：http://gig.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dbb.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ycg.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nwh.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iul.xinyue.icu

================================================================================
来源：http://cwm.hammf.cn

N. 数据结构与算法
来源：http://ljs.yvedp.cn

================================================================================
来源：http://fxu.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://eub.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://aco.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xta.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ihw.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://enf.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ihz.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://pds.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iou.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jbe.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://ggi.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://nae.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://asx.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://kuw.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lkn.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://frh.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://exc.zhengqikj.top

Ruby: arr.sort
来源：http://xra.nwbrower.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lqo.yj20258.top

[N03] 快速排序（分治示例）
来源：http://wxw.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yhl.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://csv.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ziw.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehn.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zeg.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gvl.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yak.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://lqa.yonumen.top

[N04] 斐波那契数列
来源：http://vyy.jqgufenzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kye.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hxg.tian-w.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpq.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jpt.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dmo.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://drx.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vvy.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://abq.feifeiyinyue.top

[N05] 最大公约数
来源：http://sxy.cucudq.cn

Py:   math.gcd(a, b)
来源：http://duz.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iod.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://svw.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cnp.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czj.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ydp.yfazqb.com

Ruby: a.gcd(b)
来源：http://oba.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xym.zhixingplan.top

[N06] 判断回文字符串
来源：http://msk.snrcjt.cn

Py:   s == s[::-1]
来源：http://sex.pycfn.com

PHP:  $s === strrev($s);
来源：http://hyh.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://jnf.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://ibd.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jfi.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://lbr.gaohongyu789.top

Ruby: s == s.reverse
来源：http://iqu.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xbu.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://uxq.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vdx.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lhr.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://hvc.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://yfi.guannengcc.top

Java: // 手写 HashMap
来源：http://umj.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://byv.mhx1999.top

Ruby: // 手写 Hash
来源：http://qkx.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ucr.iojbl.cn

[N08] 生成全排列
来源：http://tbg.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://fde.tianlin.xyz

PHP:  // 手写递归交换
来源：http://mcr.yj20258.top

JS:   // 手写回溯递归
来源：http://fzs.chenlongwang.top

TS:   // 手写回溯递归
来源：http://zku.aizwys.cn

Java: // 手写回溯递归
来源：http://vdx.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://ata.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://xcu.cucudq.cn

C#:   // 手写回溯递归
来源：http://fnj.ivvv.top

[N09] 栈与队列
来源：http://hxx.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://avs.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ngs.aizwys.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tea.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rls.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://krx.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qri.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kbp.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nca.vehdjk.com

[N10] 链表节点定义
来源：http://zpy.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khs.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xpv.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mgk.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vpj.yongpay.top

Java: class Node { int v; Node next; }
来源：http://zlm.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zfv.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://kno.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tav.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://mbh.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sum.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://bny.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ryd.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://heb.chenjidiqi.icu

Java: // 手写递归
来源：http://xmv.0kj1m.cn

Go:   // 手写递归
来源：http://dru.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://slt.xuetiantiany.cn

C#:   // 手写递归
来源：http://wmw.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pfv.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xbk.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ipv.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yoq.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvs.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kmd.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xll.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://szn.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iop.ivvv.top

================================================================================
来源：http://ovg.yvedp.cn

O. 并发与异步
来源：http://ssw.gaohongyu789.top

================================================================================
来源：http://bmx.jiagoushi.top

[O01] 启动一个线程
来源：http://ggc.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eaz.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bjr.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nbv.bbcook.cn

TS:   // 同 JS
来源：http://dhf.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://kcm.yanxiufei.cn

Go:   go f()
来源：http://ysl.ivvv.top

Ruby: Thread.new { f }
来源：http://sej.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://tul.feifeiyinyue.top

[O02] 使用线程池
来源：http://hdp.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mok.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://scx.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://yxf.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://llc.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://bkl.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://prf.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://owf.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jxu.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://tng.redwolf501.top

Py:   with lock: shared += 1
来源：http://cng.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://cvt.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uor.sjlbkw.cn

TS:   // 同 JS
来源：http://oej.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://jng.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iml.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fqt.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://jvh.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://zkd.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://cat.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://atd.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://ldm.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oql.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://saa.kuanghao11.cn


<!-- 参考信息 -->