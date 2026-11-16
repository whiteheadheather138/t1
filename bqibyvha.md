代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://izw.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://phc.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://twy.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ffn.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://gej.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gbr.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zyv.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vfz.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jbq.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wxn.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qqt.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zqt.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nqg.hysaishi.cn

[K07] 进制转换
来源：http://bjw.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://msr.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://okd.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rko.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dbu.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ycq.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kyi.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xmr.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ifl.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://rek.ivvv.top

Py:   pickle.dumps(obj)
来源：http://fgu.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://aaq.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://tgo.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://gsx.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xei.nanxuanxn.top

Go:   encoding/gob
来源：http://pqw.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://edx.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bkx.hcnkem.com

================================================================================
来源：http://imo.tianlin.xyz

L. 网络请求
来源：http://pwf.jqgfzy.top

================================================================================
来源：http://ngo.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://nuz.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ulo.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://srs.chenlongwang.top

JS:   await fetch(url)
来源：http://yep.zhixingplan.top

TS:   await fetch(url)
来源：http://syt.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qeu.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://ykd.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jps.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hkh.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://dgf.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://rje.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gwo.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ulv.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nbh.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nwo.shzxlz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mcj.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ook.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dsh.mhx1999.top

[L03] 设置自定义请求头
来源：http://mik.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://llb.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fnk.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lww.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdm.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ymn.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yio.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mbs.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xln.hysaishi.cn

[L04] 设置超时
来源：http://idu.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://mmc.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cgs.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sri.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rbu.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://urt.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://det.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vdg.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xhw.havefunace.top

[L05] 上传文件（multipart）
来源：http://omp.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eic.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kzs.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ssh.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fto.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wfb.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://swz.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jmq.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qaw.hcnkem.com

[L06] 解析响应为 JSON
来源：http://daw.yj202588.top

Py:   resp.json()
来源：http://sge.fengsongda.top

PHP:  json_decode($body, true);
来源：http://scc.fzhhl.top

JS:   await resp.json()
来源：http://xlw.fehbvm.com

TS:   await resp.json()
来源：http://lmj.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wjx.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dad.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://vki.shuidangran.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://udg.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://man.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xvh.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpl.birdmap.top

JS:   resp.ok;  resp.status
来源：http://lto.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://xls.0kj1m.cn

Java: resp.statusCode()
来源：http://arc.xylfe.cn

Go:   resp.StatusCode
来源：http://mgd.xuanzx.com

Ruby: resp.code.to_i
来源：http://adj.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://aik.redwolf501.top

[L08] 并发请求多个地址
来源：http://dyp.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fhg.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://xnv.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfw.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kje.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zuk.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sma.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://czn.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gtg.mhx1999.top

================================================================================
来源：http://shw.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://evs.haohaochexian.top

================================================================================
来源：http://jfp.uphjek.com

[M01] 读取命令行参数
来源：http://fut.dianchejie.cn

Py:   sys.argv[1:]
来源：http://osv.yfazqb.com

PHP:  $argv;  $argc;
来源：http://ati.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://dpm.cashguo.top

TS:   process.argv.slice(2)
来源：http://hae.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://ucb.iojbl.cn

Go:   os.Args[1:]
来源：http://eyg.andypj.xyz

Ruby: ARGV
来源：http://gdm.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://mlb.xuanzx.com

[M02] 读取环境变量
来源：http://vuj.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://lwp.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ldl.zhongyouzk.top

JS:   process.env.HOME
来源：http://jnm.feifeiyinyue.top

TS:   process.env.HOME
来源：http://iqz.jinqigufen.top

Java: System.getenv("HOME")
来源：http://lqb.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fgf.316326.xyz

Ruby: ENV["HOME"]
来源：http://nfs.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mpb.gzhubu.top

[M03] 执行外部命令
来源：http://rug.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vsz.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vnt.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://afy.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yff.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nen.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fnq.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uoc.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://dys.yangfankeji.com

[M04] 获取当前工作目录
来源：http://foi.hnqzz.top

Py:   os.getcwd()
来源：http://pdt.dianchejie.cn

PHP:  getcwd();
来源：http://ied.chenlongwang.top

JS:   process.cwd()
来源：http://nzs.jqgufenzy.top

TS:   process.cwd()
来源：http://eqp.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://lyr.bbcook.cn

Go:   os.Getwd()
来源：http://zdd.hcnkem.com

Ruby: Dir.pwd
来源：http://roc.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://pho.shanyushiyangtech.top

[M05] 设置退出码
来源：http://xir.nwbrower.top

Py:   sys.exit(1)
来源：http://jqd.wangshuangyany.cn

PHP:  exit(1);
来源：http://qui.chenlongwang.top

JS:   process.exit(1)
来源：http://okw.hnxiangtu.top

TS:   process.exit(1)
来源：http://jkd.vqdsnc.cn

Java: System.exit(1)
来源：http://bke.hcnkem.com

Go:   os.Exit(1)
来源：http://eux.svipenyu.cn

Ruby: exit 1
来源：http://fzi.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gbj.zhoulong.xyz

[M06] 向标准错误输出
来源：http://ixi.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://apn.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wcp.zdbjq.cn

JS:   console.error("err")
来源：http://rog.yuanzhike.top

TS:   console.error("err")
来源：http://osq.yvedp.cn

Java: System.err.println("err")
来源：http://bfi.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dco.fzhhl.top

Ruby: warn "err"
来源：http://zkj.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://lkc.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://ccm.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://djg.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vlh.jlsjyb.cn

JS:   require.main === module
来源：http://owb.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://auy.jianghu66.top

Java: public static void main(String[] args)
来源：http://vpd.feifeiyinyue.top

Go:   func main()
来源：http://vwh.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://muu.pycfn.com

C#:   static void Main(string[] args)
来源：http://tah.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://nsy.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://qfj.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://jon.gogol.net.cn

JS:   process.platform;  process.version
来源：http://qxx.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://jwq.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jon.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ser.zdqjudy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qud.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kmk.ehwqpu.com

================================================================================
来源：http://gdt.hnxiangtu.top

N. 数据结构与算法
来源：http://jbd.havefunace.top

================================================================================
来源：http://smk.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://qns.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://kfb.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bcf.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cgj.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lic.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lux.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://ocn.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jdi.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://luj.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://isl.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://ioa.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kch.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://git.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://dfz.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://him.yj202588.top

Go:   slices.Sort(arr)
来源：http://yip.quarkkingdee.top

Ruby: arr.sort
来源：http://fjz.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qnh.hammf.cn

[N03] 快速排序（分治示例）
来源：http://lyt.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fwa.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://cie.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dqy.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wai.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://axu.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hbz.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://grw.gotoacloud.top

C#:   // 手写递归，或 Array.Sort
来源：http://mhv.redwolf501.top

[N04] 斐波那契数列
来源：http://vlo.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://otf.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fpi.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nxj.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bhq.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jsq.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cks.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wad.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pum.shuidangran.top

[N05] 最大公约数
来源：http://epj.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://hrt.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zqa.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kas.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rhi.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ear.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekp.tianlin.xyz

Ruby: a.gcd(b)
来源：http://oru.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ald.hywenlv.cn

[N06] 判断回文字符串
来源：http://qks.yanxiufei.cn

Py:   s == s[::-1]
来源：http://ksz.316326.xyz

PHP:  $s === strrev($s);
来源：http://zhm.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://rmi.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://zbd.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://isx.tanke756.top

Go:   // 双指针从两端比较
来源：http://ldz.52xcode.cn

Ruby: s == s.reverse
来源：http://elr.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uxh.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://twb.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zoc.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tok.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://edv.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://zuv.uphjek.com

Java: // 手写 HashMap
来源：http://yjn.xziqi.cn

Go:   // 手写 map[int]int
来源：http://wbc.dianchejie.cn

Ruby: // 手写 Hash
来源：http://jjh.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://gmb.0kj1m.cn

[N08] 生成全排列
来源：http://iwc.yongpay.top

Py:   itertools.permutations(arr)
来源：http://nim.cucudq.cn

PHP:  // 手写递归交换
来源：http://uex.sxryk.cn

JS:   // 手写回溯递归
来源：http://ban.yj202588.top

TS:   // 手写回溯递归
来源：http://wss.jiagoushi.top

Java: // 手写回溯递归
来源：http://ewf.yangfankeji.com

Go:   // 手写回溯递归
来源：http://xbe.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://ukc.ydzc1.top

C#:   // 手写回溯递归
来源：http://gdb.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://wsy.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xks.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dit.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vxg.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eqq.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gsx.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iiz.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vev.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://isf.birdmap.top

[N10] 链表节点定义
来源：http://ggx.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jmn.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wav.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://woy.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxe.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://xsl.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://pmx.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ezw.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dqz.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://csz.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jha.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://gzb.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wut.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlr.guannengcc.top

Java: // 手写递归
来源：http://urq.haohaochexian.top

Go:   // 手写递归
来源：http://hhv.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://onv.nanxinkj.top

C#:   // 手写递归
来源：http://foo.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rqj.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iqp.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mns.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xvw.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtl.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nkt.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kkd.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://egd.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gqq.yj202588.top

================================================================================
来源：http://ijv.nanxinkj.top

O. 并发与异步
来源：http://aex.c1oappe.top

================================================================================
来源：http://rsf.cashguo.top

[O01] 启动一个线程
来源：http://xlg.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jae.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qtu.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bha.jlsjyb.cn

TS:   // 同 JS
来源：http://ujv.zdqjudy.top


<!-- 参考信息 -->