代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ddx.chenzaomai.com

[K07] 进制转换
来源：http://jcw.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jhg.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qxz.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tlr.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iks.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bkv.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yah.haohaochexian.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dyx.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rmx.tian-w.cn

[K08] 二进制序列化（非 JSON）
来源：http://imn.havefunace.top

Py:   pickle.dumps(obj)
来源：http://jzi.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pip.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://gyw.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://gaf.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wlg.yanxiufei.cn

Go:   encoding/gob
来源：http://var.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://cgb.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://miz.jlsjyb.cn

================================================================================
来源：http://iqb.pengpengdd.cyou

L. 网络请求
来源：http://kaz.zycfv.cn

================================================================================
来源：http://jtg.hywenlv.cn

[L01] 发送 GET 请求
来源：http://jsp.chenjidiqi.icu

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lmq.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vnk.bjfxy.top

JS:   await fetch(url)
来源：http://nhf.iojbl.cn

TS:   await fetch(url)
来源：http://jpx.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zvv.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://cne.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uxe.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ygw.shuidangran.top

[L02] 发送 POST JSON
来源：http://xeg.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xch.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxb.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsx.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgv.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yqr.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://scr.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://way.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lzi.zhixingplan.top

[L03] 设置自定义请求头
来源：http://hqs.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ugz.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oqt.shzxlz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gnj.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ene.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pzv.jqgufenzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wpc.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://byp.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqt.sjlbkw.cn

[L04] 设置超时
来源：http://pqd.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://yzr.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgw.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqk.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgw.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eoi.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sso.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dbz.yongpay.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wyk.daria6918.cn

[L05] 上传文件（multipart）
来源：http://soa.xuanzx.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://guc.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fjv.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://efd.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fjc.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ypl.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://enc.jinghuilouyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kcl.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://edw.epnwcf.com

[L06] 解析响应为 JSON
来源：http://qam.zhijiandao.cn

Py:   resp.json()
来源：http://xcj.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://qfi.jiagoushi.top

JS:   await resp.json()
来源：http://yfp.guannengcc.top

TS:   await resp.json()
来源：http://luw.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nnd.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://knr.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://rej.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mxb.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://neq.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tmc.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vdi.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://pqh.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://hsd.haohaochexian.top

Java: resp.statusCode()
来源：http://uxi.gzhubu.top

Go:   resp.StatusCode
来源：http://hff.ctjpmb.com

Ruby: resp.code.to_i
来源：http://htj.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://fkn.vehdjk.com

[L08] 并发请求多个地址
来源：http://pai.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fkk.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://glw.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cen.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olu.jlsjyb.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkl.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://src.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uyz.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://koq.cdnleiting.top

================================================================================
来源：http://ksc.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://lck.gogol.net.cn

================================================================================
来源：http://gjo.redwolf501.top

[M01] 读取命令行参数
来源：http://opr.hammf.cn

Py:   sys.argv[1:]
来源：http://mip.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://swr.bbcook.cn

JS:   process.argv.slice(2)
来源：http://kzk.hammf.cn

TS:   process.argv.slice(2)
来源：http://doj.havefunace.top

Java: args 数组（main 方法参数）
来源：http://snq.jqgfzy.top

Go:   os.Args[1:]
来源：http://ptj.gaohongyu789.top

Ruby: ARGV
来源：http://qen.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://miv.fehbvm.com

[M02] 读取环境变量
来源：http://jgj.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://lol.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://non.shangyingyoupin.top

JS:   process.env.HOME
来源：http://ltn.snrcjt.cn

TS:   process.env.HOME
来源：http://qrb.wangdashe.top

Java: System.getenv("HOME")
来源：http://bqq.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://auk.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://ngj.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dmf.nanxuanxn.top

[M03] 执行外部命令
来源：http://dgo.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://auw.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mqq.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hbi.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ceo.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vwg.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tdi.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qaa.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://sow.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://xjj.nwbrower.top

Py:   os.getcwd()
来源：http://fiw.cheryme.top

PHP:  getcwd();
来源：http://zhk.zycfv.cn

JS:   process.cwd()
来源：http://ieh.sufxvd.cn

TS:   process.cwd()
来源：http://ahk.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cre.fehbvm.com

Go:   os.Getwd()
来源：http://dca.andypj.xyz

Ruby: Dir.pwd
来源：http://uyg.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yno.nwbrower.top

[M05] 设置退出码
来源：http://tnc.jqgufenzy.top

Py:   sys.exit(1)
来源：http://gom.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://qpm.xylfe.cn

JS:   process.exit(1)
来源：http://uyw.cashguo.top

TS:   process.exit(1)
来源：http://uqu.shanyushiyangtech.top

Java: System.exit(1)
来源：http://ebx.ehwqpu.com

Go:   os.Exit(1)
来源：http://mnw.svipenyu.cn

Ruby: exit 1
来源：http://thz.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tcn.fehbvm.com

[M06] 向标准错误输出
来源：http://yrt.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://gtk.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uwu.nwbrower.top

JS:   console.error("err")
来源：http://wfx.shanyushiyangtech.top

TS:   console.error("err")
来源：http://cua.hysaishi.cn

Java: System.err.println("err")
来源：http://vnq.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sio.fktsv.cn

Ruby: warn "err"
来源：http://eah.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://gge.guowangkeji.top

[M07] 判断是否为主入口
来源：http://slu.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://ozw.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zwe.jinqigufen.top

JS:   require.main === module
来源：http://wcm.zhongyouzk.top

TS:   require.main === module
来源：http://udx.yueranfly.top

Java: public static void main(String[] args)
来源：http://gko.dashuyun.cn

Go:   func main()
来源：http://vur.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vag.kuanghao11.cn

C#:   static void Main(string[] args)
来源：http://hjo.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://ywy.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://xjf.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://uhr.sweek.top

JS:   process.platform;  process.version
来源：http://ezj.yangfankeji.com

TS:   process.platform;  process.version
来源：http://cvb.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wpd.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rhk.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cxq.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://edp.cdnleiting.top

================================================================================
来源：http://hwb.uphjek.com

N. 数据结构与算法
来源：http://iif.yuxming.cn

================================================================================
来源：http://zym.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://nhr.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://ezx.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qso.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kve.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vne.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://nod.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://bod.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://eih.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://jxn.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://ymk.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ibv.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ujb.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dvo.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xvh.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hfm.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://mey.sjlbkw.cn

Ruby: arr.sort
来源：http://bge.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nkv.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://gjb.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gtd.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://kub.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ykx.jqgfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdv.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gva.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zdo.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qqr.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://gob.gaohongyu789.top

[N04] 斐波那契数列
来源：http://vez.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cwu.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmp.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yhj.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpq.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ost.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dle.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nup.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nmq.hnqzz.top

[N05] 最大公约数
来源：http://hbe.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://aeo.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hlv.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://swn.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wgh.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://krq.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zpl.dianchejie.cn

Ruby: a.gcd(b)
来源：http://skk.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tjg.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://wcj.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://ehl.chenlongwang.top

PHP:  $s === strrev($s);
来源：http://hqs.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://vza.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://vms.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cps.yj20258.top

Go:   // 双指针从两端比较
来源：http://twg.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://kqg.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sdy.cheryme.top

[N07] 两数之和（返回下标）
来源：http://bpo.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rjw.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mso.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hlh.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://jho.yuxming.cn

Java: // 手写 HashMap
来源：http://ltz.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://akf.tarul.cn

Ruby: // 手写 Hash
来源：http://ooq.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://twn.nwbrower.top

[N08] 生成全排列
来源：http://evr.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://opx.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://tss.wangdashe.top

JS:   // 手写回溯递归
来源：http://ewu.smart0.xyz

TS:   // 手写回溯递归
来源：http://zsn.yj20258888.top

Java: // 手写回溯递归
来源：http://bpn.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://isc.birdmap.top

Ruby: arr.permutation.to_a
来源：http://zgz.snrcjt.cn

C#:   // 手写回溯递归
来源：http://fev.vqdsnc.cn

[N09] 栈与队列
来源：http://evi.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://drl.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hcl.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eci.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kzh.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mjh.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cdm.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zyg.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://loc.zhijiandao.cn

[N10] 链表节点定义
来源：http://rgo.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mnc.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ilu.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iey.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wjj.sweek.top

Java: class Node { int v; Node next; }
来源：http://jyb.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sbv.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://doo.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kbg.smart0.xyz

[N11] 二叉树中序遍历
来源：http://uta.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mih.ctjpmb.com

PHP:  // 手写递归函数
来源：http://uwe.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wco.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpf.guowangkeji.top

Java: // 手写递归
来源：http://bvw.yueranfly.top

Go:   // 手写递归
来源：http://lud.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fem.guannengcc.top

C#:   // 手写递归
来源：http://lba.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ilp.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bxf.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tyi.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjy.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yud.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://clh.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nrj.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qct.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://unt.ppjwa.cn

================================================================================
来源：http://yon.xylfe.cn

O. 并发与异步
来源：http://mes.hammf.cn

================================================================================
来源：http://bbn.hywenlv.cn

[O01] 启动一个线程
来源：http://ahz.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cgr.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xrq.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nlg.xuanzx.com

TS:   // 同 JS
来源：http://rjr.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://kol.jinghuilouyu.cn

Go:   go f()
来源：http://kcl.yj20258.top

Ruby: Thread.new { f }
来源：http://sfk.wangdashe.top

C#:   Task.Run(() => F());
来源：http://akk.zhiwuduotai.top

[O02] 使用线程池
来源：http://dba.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ism.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://urc.yj20258.top

JS:   // worker_threads 线程池
来源：http://rby.xziqi.cn

TS:   // worker_threads 线程池
来源：http://utt.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://iay.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kto.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uwo.birdmap.top


<!-- 参考信息 -->