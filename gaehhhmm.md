代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://qta.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://zgl.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://oeo.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://whq.zhoulong.xyz

Go:   encoding/gob
来源：http://vgu.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://osh.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oma.jlsjyb.cn

================================================================================
来源：http://ldt.ehwqpu.com

L. 网络请求
来源：http://twu.cheryme.top

================================================================================
来源：http://spu.xziqi.cn

[L01] 发送 GET 请求
来源：http://nuc.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fbf.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://twy.xziqi.cn

JS:   await fetch(url)
来源：http://sqt.jinqigufen.top

TS:   await fetch(url)
来源：http://qwq.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pbx.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://pco.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sla.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ukj.cheryme.top

[L02] 发送 POST JSON
来源：http://hhh.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://cwo.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bqx.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mnl.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://egp.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmt.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfy.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ary.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lwv.guannengcc.top

[L03] 设置自定义请求头
来源：http://gjj.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cna.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nbf.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fad.yuanzhike.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://owk.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xrf.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oog.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://txz.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://izh.yuxming.cn

[L04] 设置超时
来源：http://win.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://yrt.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://res.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gsd.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nne.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://umo.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ljf.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yuu.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qmm.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://yvr.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ixi.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lyn.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lmj.316326.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tms.wangdashe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gbh.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tqe.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fpz.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lyl.bjfxy.top

[L06] 解析响应为 JSON
来源：http://yuq.cdnleiting.top

Py:   resp.json()
来源：http://hcp.birdmap.top

PHP:  json_decode($body, true);
来源：http://yor.shangyingyoupin.top

JS:   await resp.json()
来源：http://fwf.xuanzx.com

TS:   await resp.json()
来源：http://tfy.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jvj.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vcd.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://pex.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lrs.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://myv.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itr.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rnb.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://snh.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://dgc.iojbl.cn

Java: resp.statusCode()
来源：http://kce.tanke756.top

Go:   resp.StatusCode
来源：http://ljr.yj202588.top

Ruby: resp.code.to_i
来源：http://cfa.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://qmw.sweek.top

[L08] 并发请求多个地址
来源：http://qga.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dit.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://rqi.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryy.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fuh.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cwp.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nkt.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gbq.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tte.vqdsnc.cn

================================================================================
来源：http://rii.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://pmu.jianghu66.top

================================================================================
来源：http://wgx.jinqigufen.top

[M01] 读取命令行参数
来源：http://rbs.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://ypn.pycfn.com

PHP:  $argv;  $argc;
来源：http://tft.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://jfs.vehdjk.com

TS:   process.argv.slice(2)
来源：http://nrw.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://kbt.yueranfly.top

Go:   os.Args[1:]
来源：http://dkw.hfpthk.cn

Ruby: ARGV
来源：http://eil.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://ckh.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://xrf.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://zli.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mhy.zhixingplan.top

JS:   process.env.HOME
来源：http://van.shzxlz.cn

TS:   process.env.HOME
来源：http://ldm.zhengqikj.top

Java: System.getenv("HOME")
来源：http://uzv.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nkd.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://seb.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ioq.zhijiandao.cn

[M03] 执行外部命令
来源：http://rtc.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gem.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvj.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gev.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://jgp.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bzh.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wue.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://xox.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://hbk.zdbjq.cn

[M04] 获取当前工作目录
来源：http://ial.hywenlv.cn

Py:   os.getcwd()
来源：http://kel.jianghu66.top

PHP:  getcwd();
来源：http://pxw.hammf.cn

JS:   process.cwd()
来源：http://sja.shanyushiyangtech.top

TS:   process.cwd()
来源：http://djt.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://dji.316326.xyz

Go:   os.Getwd()
来源：http://euh.xuanzx.com

Ruby: Dir.pwd
来源：http://zlo.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://ntr.fktsv.cn

[M05] 设置退出码
来源：http://eip.xziqi.cn

Py:   sys.exit(1)
来源：http://xsu.gogol.net.cn

PHP:  exit(1);
来源：http://npy.tian-w.cn

JS:   process.exit(1)
来源：http://itm.yueranfly.top

TS:   process.exit(1)
来源：http://dwx.fanxiaobao.xyz

Java: System.exit(1)
来源：http://gxh.yangfankeji.com

Go:   os.Exit(1)
来源：http://vnj.yfazqb.com

Ruby: exit 1
来源：http://npd.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xab.smart0.xyz

[M06] 向标准错误输出
来源：http://frm.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://lpn.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://saz.jiagoushi.top

JS:   console.error("err")
来源：http://hrn.tian-w.cn

TS:   console.error("err")
来源：http://loz.jqgufenzy.top

Java: System.err.println("err")
来源：http://mso.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eel.hfpthk.cn

Ruby: warn "err"
来源：http://yzy.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://uck.ehwqpu.com

[M07] 判断是否为主入口
来源：http://zfz.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://hfe.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yfu.pycfn.com

JS:   require.main === module
来源：http://wcq.snrcjt.cn

TS:   require.main === module
来源：http://ilt.ctjpmb.com

Java: public static void main(String[] args)
来源：http://sed.kuanghao11.cn

Go:   func main()
来源：http://sml.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wko.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://iap.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://jks.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://ccl.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://lkj.bjfxy.top

JS:   process.platform;  process.version
来源：http://mzr.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://wke.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tqz.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vtg.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qtz.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ycl.vqdsnc.cn

================================================================================
来源：http://jgt.haohaochexian.top

N. 数据结构与算法
来源：http://gjc.guowangkeji.top

================================================================================
来源：http://lhi.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://xim.andypj.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://gxa.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cal.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tli.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fer.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bvb.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://csj.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://arq.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://bbd.bjfxy.top

[N02] 排序（工程实践用内置实现）
来源：http://wpd.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://bit.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kgd.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://syi.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bsz.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lmj.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://fnj.havefunace.top

Ruby: arr.sort
来源：http://ggh.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jgm.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://igx.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ivr.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://itg.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jwh.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xvi.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://btu.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iac.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://llz.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ntp.shuidangran.top

[N04] 斐波那契数列
来源：http://qvo.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zme.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://esc.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wao.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lax.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yld.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cgh.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tia.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qla.iojbl.cn

[N05] 最大公约数
来源：http://sjn.yongpay.top

Py:   math.gcd(a, b)
来源：http://lag.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pwg.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbx.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zzd.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xii.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bax.hfpthk.cn

Ruby: a.gcd(b)
来源：http://eeo.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mgn.zhongyouzk.top

[N06] 判断回文字符串
来源：http://egi.zhongyouzk.top

Py:   s == s[::-1]
来源：http://msu.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://rvx.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://xvs.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://sef.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hhz.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://sxb.chenzaomai.com

Ruby: s == s.reverse
来源：http://lse.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://rom.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://szo.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://esj.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tdh.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://wtv.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://ymc.pycfn.com

Java: // 手写 HashMap
来源：http://oku.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://fav.yj202588.top

Ruby: // 手写 Hash
来源：http://uxl.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://bxk.jiagoushi.top

[N08] 生成全排列
来源：http://xsj.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://ylz.yuanzhike.top

PHP:  // 手写递归交换
来源：http://wgn.fzhhl.top

JS:   // 手写回溯递归
来源：http://rox.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://tuv.52xcode.cn

Java: // 手写回溯递归
来源：http://bhk.hysaishi.cn

Go:   // 手写回溯递归
来源：http://emk.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://jfe.fengsongda.top

C#:   // 手写回溯递归
来源：http://dbg.fzhhl.top

[N09] 栈与队列
来源：http://xfa.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vtd.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://edf.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bcp.zhengqikj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mdm.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tmw.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://asu.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dck.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdi.tian-w.cn

[N10] 链表节点定义
来源：http://jfh.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ueg.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wpt.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kfa.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://prd.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://gjd.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ufb.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vmb.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hih.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://hev.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tzx.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://ifh.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psq.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fkt.mhx1999.top

Java: // 手写递归
来源：http://ttg.sxryk.cn

Go:   // 手写递归
来源：http://rxs.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ybn.kuanghao11.cn

C#:   // 手写递归
来源：http://arb.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hyg.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jhc.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xpy.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cqz.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tgr.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://euf.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aus.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tta.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ycg.yuxming.cn

================================================================================
来源：http://cez.nwbrower.top

O. 并发与异步
来源：http://zqh.zycfv.cn

================================================================================
来源：http://xlv.zhengqikj.top

[O01] 启动一个线程
来源：http://aqo.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lyg.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hyi.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cdc.yvedp.cn

TS:   // 同 JS
来源：http://cym.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://btg.0kj1m.cn

Go:   go f()
来源：http://ned.ehwqpu.com

Ruby: Thread.new { f }
来源：http://hor.yueranfly.top

C#:   Task.Run(() => F());
来源：http://ygt.chenlongwang.top

[O02] 使用线程池
来源：http://rot.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vlj.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ddn.sxryk.cn

JS:   // worker_threads 线程池
来源：http://fdi.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://azj.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://rbx.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cby.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jyp.shzxlz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mez.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://mwm.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://qxl.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://wex.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rdu.ybcxt.top

TS:   // 同 JS
来源：http://tjm.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://nue.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://isn.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nvr.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://hvb.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://yqy.havefunace.top

Py:   async def f():⏎    await g()
来源：http://aoz.hfpthk.cn


<!-- 参考信息 -->