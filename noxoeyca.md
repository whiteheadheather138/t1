代发 wailian999

Go:   encoding/gob
来源：http://pim.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://vqj.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xbi.xuetiantiany.cn

================================================================================
来源：http://bqz.vehdjk.com

L. 网络请求
来源：http://lmn.9152youxi.cn

================================================================================
来源：http://xfg.hysaishi.cn

[L01] 发送 GET 请求
来源：http://jib.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzi.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://soo.jqgfzy.top

JS:   await fetch(url)
来源：http://kcy.cucudq.cn

TS:   await fetch(url)
来源：http://jvs.hywenlv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://obz.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://yxa.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rxk.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xnq.fzhhl.top

[L02] 发送 POST JSON
来源：http://tqm.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://nso.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cyk.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhu.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rup.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nhv.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://syd.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qht.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsn.daxiang520.top

[L03] 设置自定义请求头
来源：http://sto.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bkj.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wrs.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lir.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://igb.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yfk.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bgs.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqv.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tdk.fehbvm.com

[L04] 设置超时
来源：http://cjs.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://xlm.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dmi.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nnz.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dyi.jinyuanbaomall.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zff.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mot.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uas.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://afu.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://ecs.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tqv.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dui.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dwf.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tsk.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://esi.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lvm.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zer.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://etu.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://ybi.c1oappe.top

Py:   resp.json()
来源：http://qcc.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://vnr.uphjek.com

JS:   await resp.json()
来源：http://rja.yj202588.top

TS:   await resp.json()
来源：http://qtx.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fxq.ydzc1.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ocr.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://wze.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xxy.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://uza.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://thm.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xet.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://twc.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://nbh.pycfn.com

Java: resp.statusCode()
来源：http://fou.aibaodan.cn

Go:   resp.StatusCode
来源：http://bbs.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://zek.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://uag.chenlongwang.top

[L08] 并发请求多个地址
来源：http://nlp.c1oappe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://otb.vehdjk.com

PHP:  curl_multi_init() 系列
来源：http://qhr.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://luz.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlj.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pgh.gotoacloud.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lqe.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://frl.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ckt.yueranfly.top

================================================================================
来源：http://mlv.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://esg.hesvh.cn

================================================================================
来源：http://ibf.hywenlv.cn

[M01] 读取命令行参数
来源：http://iva.yvedp.cn

Py:   sys.argv[1:]
来源：http://zav.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://oeu.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://jwv.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://klf.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://zlp.daxiang520.top

Go:   os.Args[1:]
来源：http://xvh.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://egs.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://ick.aibaodan.cn

[M02] 读取环境变量
来源：http://fys.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://nks.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bne.jqgfzy.top

JS:   process.env.HOME
来源：http://uqf.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://cyl.sxryk.cn

Java: System.getenv("HOME")
来源：http://rfh.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://akj.yuxming.cn

Ruby: ENV["HOME"]
来源：http://gzh.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://enl.yuanzhike.top

[M03] 执行外部命令
来源：http://rze.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkx.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rmp.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pam.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nhn.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://npm.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rjt.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://zkp.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://jac.cheryme.top

[M04] 获取当前工作目录
来源：http://arp.hcnkem.com

Py:   os.getcwd()
来源：http://qsd.gogol.net.cn

PHP:  getcwd();
来源：http://pno.xuetiantiany.cn

JS:   process.cwd()
来源：http://gfg.bjfxy.top

TS:   process.cwd()
来源：http://dct.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://okp.jinqigufen.top

Go:   os.Getwd()
来源：http://hkg.snrcjt.cn

Ruby: Dir.pwd
来源：http://pkl.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://nxd.cashguo.top

[M05] 设置退出码
来源：http://skv.shzxlz.cn

Py:   sys.exit(1)
来源：http://pdi.zhiwuduotai.top

PHP:  exit(1);
来源：http://mws.52xcode.cn

JS:   process.exit(1)
来源：http://upk.jiagoushi.top

TS:   process.exit(1)
来源：http://txj.jyoumei.cn

Java: System.exit(1)
来源：http://dww.vqdsnc.cn

Go:   os.Exit(1)
来源：http://ttg.ivvv.top

Ruby: exit 1
来源：http://bpf.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oyf.sysykeji.top

[M06] 向标准错误输出
来源：http://rql.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://rjn.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iby.yj20258.top

JS:   console.error("err")
来源：http://edn.chenzaomai.com

TS:   console.error("err")
来源：http://uva.ydzc1.top

Java: System.err.println("err")
来源：http://hdo.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zky.shangyingyoupin.top

Ruby: warn "err"
来源：http://cwf.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://sty.cashguo.top

[M07] 判断是否为主入口
来源：http://krk.hammf.cn

Py:   if __name__ == "__main__":
来源：http://ugh.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ylc.ctjpmb.com

JS:   require.main === module
来源：http://vqk.zycfv.cn

TS:   require.main === module
来源：http://ujj.daxiang520.top

Java: public static void main(String[] args)
来源：http://zjp.sufxvd.cn

Go:   func main()
来源：http://cwu.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tgv.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://iuf.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://yhu.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://fmi.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://okn.bbcook.cn

JS:   process.platform;  process.version
来源：http://bkj.nanxinkj.top

TS:   process.platform;  process.version
来源：http://rtc.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cxm.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://teb.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ilp.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wds.epnwcf.com

================================================================================
来源：http://qps.ydjk.org.cn

N. 数据结构与算法
来源：http://ntx.tianlin.xyz

================================================================================
来源：http://qju.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://rkn.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://rwc.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wfz.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nsi.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://adp.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qei.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://mxb.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nbu.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://hzm.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://zqi.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://amu.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://beb.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://igj.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ojg.snrcjt.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mzo.uphjek.com

Go:   slices.Sort(arr)
来源：http://msv.yueranfly.top

Ruby: arr.sort
来源：http://gby.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wfr.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://wzv.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ymt.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://kgw.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jeo.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vmw.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ifq.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tqd.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uuc.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nkl.quarkkingdee.top

[N04] 斐波那契数列
来源：http://rfs.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qed.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wuz.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://owg.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nfs.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yxo.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cfp.zhiwuduotai.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ucc.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ngb.zhixingplan.top

[N05] 最大公约数
来源：http://wam.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://van.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jcp.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ker.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qnn.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kqx.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qqv.yj20258888.top

Ruby: a.gcd(b)
来源：http://eug.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yrv.wangdashe.top

[N06] 判断回文字符串
来源：http://ftw.fengsongda.top

Py:   s == s[::-1]
来源：http://coy.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://kjm.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://vqg.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://fks.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://enn.yj20258888.top

Go:   // 双指针从两端比较
来源：http://avv.zycfv.cn

Ruby: s == s.reverse
来源：http://nto.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zkv.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://gab.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vlx.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jdk.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ikg.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://hoq.jlsjyb.cn

Java: // 手写 HashMap
来源：http://hny.fktsv.cn

Go:   // 手写 map[int]int
来源：http://lhh.ydzc1.top

Ruby: // 手写 Hash
来源：http://nmc.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://qkn.shanyushiyangtech.top

[N08] 生成全排列
来源：http://yyo.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://oaf.ivvv.top

PHP:  // 手写递归交换
来源：http://ftv.havefunace.top

JS:   // 手写回溯递归
来源：http://xyr.gotoacloud.top

TS:   // 手写回溯递归
来源：http://uhl.shuidangran.top

Java: // 手写回溯递归
来源：http://cid.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://ziq.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://svn.ybcxt.top

C#:   // 手写回溯递归
来源：http://dcv.yonumen.top

[N09] 栈与队列
来源：http://rhx.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://noh.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sws.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wjc.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xmg.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wyn.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fmc.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://awd.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ays.sysykeji.top

[N10] 链表节点定义
来源：http://lkz.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rjp.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kxr.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xey.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wiu.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://yhv.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fby.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sxu.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bvi.hammf.cn

[N11] 二叉树中序遍历
来源：http://lth.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ivp.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://pxu.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://myj.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qkc.gotoacloud.top

Java: // 手写递归
来源：http://fex.yuanzhike.top

Go:   // 手写递归
来源：http://lth.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ncp.yvedp.cn

C#:   // 手写递归
来源：http://pfz.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dcq.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sac.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ilz.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfe.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yei.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvy.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vvl.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fee.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vyj.yuanzhike.top

================================================================================
来源：http://cbx.9152youxi.cn

O. 并发与异步
来源：http://edg.hongshengwenyu.top

================================================================================
来源：http://trp.yj20258888.top

[O01] 启动一个线程
来源：http://voo.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ojp.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://knw.zhoulong.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wzj.quarkkingdee.top

TS:   // 同 JS
来源：http://pji.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://ywv.daxiang520.top

Go:   go f()
来源：http://pex.fzhhl.top

Ruby: Thread.new { f }
来源：http://kyd.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://kfv.gotoacloud.top

[O02] 使用线程池
来源：http://tzl.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdp.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pvx.vehdjk.com

JS:   // worker_threads 线程池
来源：http://aow.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://clf.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://cgy.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vyd.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nzx.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://krb.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://xho.c1oappe.top

Py:   with lock: shared += 1
来源：http://yxx.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://drm.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rro.0kj1m.cn

TS:   // 同 JS
来源：http://qtu.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://aen.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zvu.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kix.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://pyv.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://ifm.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://svw.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eob.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://jxv.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uey.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yty.52xcode.cn


<!-- 参考信息 -->