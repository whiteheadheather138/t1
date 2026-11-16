代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rlv.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wlo.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lus.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zas.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://prp.c1oappe.top

[K07] 进制转换
来源：http://ila.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tke.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://arq.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ejv.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xal.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vsi.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipr.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qdu.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kud.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://moq.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://nel.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pbb.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://zxi.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://ell.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hnp.zhijiandao.cn

Go:   encoding/gob
来源：http://xes.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://zmc.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uua.xingfuxueyuan.xyz

================================================================================
来源：http://emb.yueranfly.top

L. 网络请求
来源：http://wqa.gaohongyu789.top

================================================================================
来源：http://wxr.xziqi.cn

[L01] 发送 GET 请求
来源：http://enr.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ybg.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://did.jyoumei.cn

JS:   await fetch(url)
来源：http://oud.tarul.cn

TS:   await fetch(url)
来源：http://zlj.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lik.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://fev.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mya.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://crq.nanxinkj.top

[L02] 发送 POST JSON
来源：http://ccd.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://inv.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qbd.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hss.guowangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xli.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xgh.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wjf.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://awh.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sey.nwbrower.top

[L03] 设置自定义请求头
来源：http://tte.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://awl.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ylg.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://koj.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://boa.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jcc.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://suj.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gdr.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wsx.yanxiufei.cn

[L04] 设置超时
来源：http://tmt.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://hly.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wel.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://veo.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmr.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://abw.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yph.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xla.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nyr.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://rkg.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://laz.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://smw.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ygb.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nil.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zxr.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mxc.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ctr.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dos.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://nfp.ybcxt.top

Py:   resp.json()
来源：http://kmk.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://emx.zdbjq.cn

JS:   await resp.json()
来源：http://ghq.jlsjyb.cn

TS:   await resp.json()
来源：http://zmt.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tcm.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rzb.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://bju.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ufi.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://gih.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tbn.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rku.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://nyh.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://dbn.gzhubu.top

Java: resp.statusCode()
来源：http://wqe.epnwcf.com

Go:   resp.StatusCode
来源：http://bnl.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://huj.hesvh.cn

C#:   (int)resp.StatusCode
来源：http://ihs.nwbrower.top

[L08] 并发请求多个地址
来源：http://knc.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cef.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://fom.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://che.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://owm.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yio.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jow.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rgw.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ccw.aizwys.cn

================================================================================
来源：http://svu.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://syk.ybcxt.top

================================================================================
来源：http://kac.jianghu66.top

[M01] 读取命令行参数
来源：http://hur.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://jbt.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://exf.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://vaq.uphjek.com

TS:   process.argv.slice(2)
来源：http://kpw.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://vko.quarkkingdee.top

Go:   os.Args[1:]
来源：http://wjl.smart0.xyz

Ruby: ARGV
来源：http://fxi.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://rwv.sweek.top

[M02] 读取环境变量
来源：http://rye.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://kvf.vqdsnc.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jcb.tian-w.cn

JS:   process.env.HOME
来源：http://wwy.hongshengwenyu.top

TS:   process.env.HOME
来源：http://spy.jianghu66.top

Java: System.getenv("HOME")
来源：http://hno.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ygz.xinyue.icu

Ruby: ENV["HOME"]
来源：http://eoq.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nlu.jianghu66.top

[M03] 执行外部命令
来源：http://fjs.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vhb.cdnleiting.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hge.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uii.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://aer.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xyt.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mre.xziqi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ujh.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://gtj.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://knv.gzhubu.top

Py:   os.getcwd()
来源：http://vmc.sxryk.cn

PHP:  getcwd();
来源：http://ldc.haohaochexian.top

JS:   process.cwd()
来源：http://som.hongshengwenyu.top

TS:   process.cwd()
来源：http://nhj.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://ghs.cucudq.cn

Go:   os.Getwd()
来源：http://uxm.jlsjyb.cn

Ruby: Dir.pwd
来源：http://koy.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://jxr.bbcook.cn

[M05] 设置退出码
来源：http://ssd.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://ouy.feifeiyinyue.top

PHP:  exit(1);
来源：http://edr.aizwys.cn

JS:   process.exit(1)
来源：http://flr.zhixingplan.top

TS:   process.exit(1)
来源：http://vzl.haohaochexian.top

Java: System.exit(1)
来源：http://ulb.smart0.xyz

Go:   os.Exit(1)
来源：http://nwo.dianchejie.cn

Ruby: exit 1
来源：http://dlf.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vap.ppjwa.cn

[M06] 向标准错误输出
来源：http://paq.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://tmm.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xdj.aibaodan.cn

JS:   console.error("err")
来源：http://gbc.zhoulong.xyz

TS:   console.error("err")
来源：http://kcm.xylfe.cn

Java: System.err.println("err")
来源：http://etp.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqg.sysykeji.top

Ruby: warn "err"
来源：http://lkd.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://zxl.zdbjq.cn

[M07] 判断是否为主入口
来源：http://eru.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://kjk.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://adl.havefunace.top

JS:   require.main === module
来源：http://uvc.zycfv.cn

TS:   require.main === module
来源：http://mlo.9152youxi.cn

Java: public static void main(String[] args)
来源：http://rxi.ybcxt.top

Go:   func main()
来源：http://nhh.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ifp.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://qhp.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://jeo.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://tnm.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://oqz.xziqi.cn

JS:   process.platform;  process.version
来源：http://odl.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://ksz.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cjm.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wfs.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zta.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wrr.zhengqikj.top

================================================================================
来源：http://rpn.cheryme.top

N. 数据结构与算法
来源：http://mci.zhiwuduotai.top

================================================================================
来源：http://abh.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://gjv.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://mjn.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ihw.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://izc.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fjf.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://adc.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://fmv.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kgx.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://odr.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://ubh.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://lst.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mit.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://glr.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpn.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yiq.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://uma.jianghu66.top

Ruby: arr.sort
来源：http://iek.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mco.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://swl.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uhp.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://nrw.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xun.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdw.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://awn.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hxq.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jqj.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://hea.jqgufenzy.top

[N04] 斐波那契数列
来源：http://tzu.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tsn.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ghk.feifeiyinyue.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://get.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://prn.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sek.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jsf.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zfz.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tqq.tarul.cn

[N05] 最大公约数
来源：http://vqw.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://oom.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gea.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejc.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ose.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://niy.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gph.yuxming.cn

Ruby: a.gcd(b)
来源：http://vvk.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://unb.guowangkeji.top

[N06] 判断回文字符串
来源：http://ebz.nanxinkj.top

Py:   s == s[::-1]
来源：http://zjv.vehdjk.com

PHP:  $s === strrev($s);
来源：http://hwl.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://bdp.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://kfr.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sew.birdmap.top

Go:   // 双指针从两端比较
来源：http://lhg.tanke756.top

Ruby: s == s.reverse
来源：http://led.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nhx.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://npc.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://amz.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cia.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xxb.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://vtx.nanxuanxn.top

Java: // 手写 HashMap
来源：http://xfu.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://har.svipenyu.cn

Ruby: // 手写 Hash
来源：http://nyv.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eea.jinqigufen.top

[N08] 生成全排列
来源：http://nho.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://qea.c1oappe.top

PHP:  // 手写递归交换
来源：http://evu.ybcxt.top

JS:   // 手写回溯递归
来源：http://zmb.jinghuilouyu.cn

TS:   // 手写回溯递归
来源：http://hix.hesvh.cn

Java: // 手写回溯递归
来源：http://qaq.fzhhl.top

Go:   // 手写回溯递归
来源：http://lcf.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://lyt.hesvh.cn

C#:   // 手写回溯递归
来源：http://kff.birdmap.top

[N09] 栈与队列
来源：http://mgj.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzd.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://boi.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tuz.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tbr.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ftl.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hwa.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wvl.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://psf.yuanzhike.top

[N10] 链表节点定义
来源：http://ehs.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bgn.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://tsh.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aro.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jda.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://pnh.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wbv.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sry.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pvh.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://ibp.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jzd.meibo888.top

PHP:  // 手写递归函数
来源：http://mil.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbh.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmg.hnqzz.top

Java: // 手写递归
来源：http://nyc.chenzaomai.com

Go:   // 手写递归
来源：http://lbm.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zxb.pycfn.com

C#:   // 手写递归
来源：http://ozn.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hgq.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://enl.yongpay.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvw.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pms.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dqc.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ovj.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uca.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jbj.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppw.fehbvm.com

================================================================================
来源：http://rrh.xingfuxueyuan.xyz

O. 并发与异步
来源：http://wow.vehdjk.com

================================================================================
来源：http://lmy.xuetiantiany.cn

[O01] 启动一个线程
来源：http://syi.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://umo.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zwh.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pyw.wangshuangyany.cn

TS:   // 同 JS
来源：http://nsr.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://gew.tanke756.top

Go:   go f()
来源：http://xao.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ryu.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://kcr.redwolf501.top

[O02] 使用线程池
来源：http://bmt.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ebw.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://loc.hnqzz.top

JS:   // worker_threads 线程池
来源：http://qog.316326.xyz


<!-- 参考信息 -->