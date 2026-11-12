代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://rqb.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fsd.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nlu.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qur.cucudq.cn

[K06] 解析 URL 查询串
来源：http://cep.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jut.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fdt.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmf.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lte.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xlg.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ixj.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iql.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jhc.yvedp.cn

[K07] 进制转换
来源：http://ioz.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zfw.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjt.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ulk.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qaf.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zjs.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nbk.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dey.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zge.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://cid.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://pfy.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lbn.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://ete.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://asx.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://msn.mhx1999.top

Go:   encoding/gob
来源：http://dsr.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://jim.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dpn.jyoumei.cn

================================================================================
来源：http://ewu.ydjk.org.cn

L. 网络请求
来源：http://dus.hesvh.cn

================================================================================
来源：http://mrg.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://qul.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qhv.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iea.zhijiandao.cn

JS:   await fetch(url)
来源：http://fvf.chenlongwang.top

TS:   await fetch(url)
来源：http://smw.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rmi.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://esl.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ubn.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kdk.yj20258.top

[L02] 发送 POST JSON
来源：http://jpo.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://trd.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mto.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvo.bbcook.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgy.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ado.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jlo.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nva.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xkc.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://ado.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://stz.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mlk.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yzb.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qnn.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kox.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gti.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uhw.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cyv.nwbrower.top

[L04] 设置超时
来源：http://kad.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://zyc.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gwm.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nst.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rlj.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejz.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vmb.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gkp.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rjl.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://ivz.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ryv.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xwt.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fkg.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hzr.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://glr.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eke.ehwqpu.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pxy.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gyw.gzhubu.top

[L06] 解析响应为 JSON
来源：http://kbb.yj20258.top

Py:   resp.json()
来源：http://ufl.redwolf501.top

PHP:  json_decode($body, true);
来源：http://blf.hesvh.cn

JS:   await resp.json()
来源：http://uis.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://nhf.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wbz.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ned.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://jfj.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vej.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://plh.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ahy.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cxi.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://div.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://jwa.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://ewg.hnxiangtu.top

Go:   resp.StatusCode
来源：http://lke.gotoacloud.top

Ruby: resp.code.to_i
来源：http://lxw.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://cph.guowangkeji.top

[L08] 并发请求多个地址
来源：http://ssf.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ott.quarkkingdee.top

PHP:  curl_multi_init() 系列
来源：http://wsk.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ktu.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://egy.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iiy.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jkv.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lcj.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rae.shangyingyoupin.top

================================================================================
来源：http://ltj.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://htb.feifeiyinyue.top

================================================================================
来源：http://iwj.ydzc1.top

[M01] 读取命令行参数
来源：http://rht.yfazqb.com

Py:   sys.argv[1:]
来源：http://gjg.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://lvt.vqdsnc.cn

JS:   process.argv.slice(2)
来源：http://irs.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://suu.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://qaz.daxiang520.top

Go:   os.Args[1:]
来源：http://uai.feifeiyinyue.top

Ruby: ARGV
来源：http://rca.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://txr.yueranfly.top

[M02] 读取环境变量
来源：http://eyw.nanxuanxn.top

Py:   os.environ.get("HOME")
来源：http://uuo.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ncg.yangfankeji.com

JS:   process.env.HOME
来源：http://pzn.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://bfb.chenlongwang.top

Java: System.getenv("HOME")
来源：http://psp.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ipa.hesvh.cn

Ruby: ENV["HOME"]
来源：http://gff.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://znm.tian-w.cn

[M03] 执行外部命令
来源：http://fpw.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sqs.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ydy.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jie.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bzi.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fwd.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zfi.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://skt.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://rva.jinqigufen.top

[M04] 获取当前工作目录
来源：http://pwr.yongpay.top

Py:   os.getcwd()
来源：http://ffh.dianchejie.cn

PHP:  getcwd();
来源：http://hgj.shzxlz.cn

JS:   process.cwd()
来源：http://djr.ydzc1.top

TS:   process.cwd()
来源：http://xgv.svipenyu.cn

Java: Path.of("").toAbsolutePath()
来源：http://hrw.jiagoushi.top

Go:   os.Getwd()
来源：http://oqp.smart0.xyz

Ruby: Dir.pwd
来源：http://olk.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://fng.jinghuilouyu.cn

[M05] 设置退出码
来源：http://ybk.iojbl.cn

Py:   sys.exit(1)
来源：http://vjq.tarul.cn

PHP:  exit(1);
来源：http://bwm.cqqwz.cn

JS:   process.exit(1)
来源：http://nmy.zhixingplan.top

TS:   process.exit(1)
来源：http://hfl.yangfankeji.com

Java: System.exit(1)
来源：http://dvf.ehwqpu.com

Go:   os.Exit(1)
来源：http://sar.bjfxy.top

Ruby: exit 1
来源：http://zbl.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://luy.gaohongyu789.top

[M06] 向标准错误输出
来源：http://bkm.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://wiz.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gda.hywenlv.cn

JS:   console.error("err")
来源：http://uxs.sufxvd.cn

TS:   console.error("err")
来源：http://jib.cdnleiting.top

Java: System.err.println("err")
来源：http://oky.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bse.smart0.xyz

Ruby: warn "err"
来源：http://rbb.zhiwuduotai.top

C#:   Console.Error.WriteLine("err")
来源：http://wpa.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://njg.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://apc.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dlq.hesvh.cn

JS:   require.main === module
来源：http://bec.316326.xyz

TS:   require.main === module
来源：http://qoy.fzhhl.top

Java: public static void main(String[] args)
来源：http://xix.bjfxy.top

Go:   func main()
来源：http://hws.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://akj.cheryme.top

C#:   static void Main(string[] args)
来源：http://orq.316326.xyz

[M08] 获取系统与运行时信息
来源：http://qjt.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://esv.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://zoi.yangfankeji.com

JS:   process.platform;  process.version
来源：http://mge.hfpthk.cn

TS:   process.platform;  process.version
来源：http://vrz.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ymv.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mjh.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wcp.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qkf.yvedp.cn

================================================================================
来源：http://gvt.ybcxt.top

N. 数据结构与算法
来源：http://vqy.ivvv.top

================================================================================
来源：http://ulk.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://ejp.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://yxj.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kcj.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqn.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urm.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://pqd.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://mpv.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://rtr.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://eul.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://yek.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://wco.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vib.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uba.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gpd.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bww.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://byl.pengpengdd.cyou

Ruby: arr.sort
来源：http://ikw.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://idb.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://ijy.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lmc.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://sgz.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jot.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xei.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zax.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pia.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sro.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kua.ehwqpu.com

[N04] 斐波那契数列
来源：http://mhi.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pob.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eln.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vau.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ows.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aze.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phm.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzh.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dvp.sufxvd.cn

[N05] 最大公约数
来源：http://jmr.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://gdz.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ofb.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apw.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://enh.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lfv.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lch.shzxlz.cn

Ruby: a.gcd(b)
来源：http://iri.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gox.tianlin.xyz

[N06] 判断回文字符串
来源：http://uio.havefunace.top

Py:   s == s[::-1]
来源：http://eup.guannengcc.top

PHP:  $s === strrev($s);
来源：http://baa.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://xpr.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://mvh.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://djb.pycfn.com

Go:   // 双指针从两端比较
来源：http://zjn.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://ikv.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gma.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://tus.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bhl.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jml.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://txx.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://ulb.guannengcc.top

Java: // 手写 HashMap
来源：http://kzs.yvedp.cn

Go:   // 手写 map[int]int
来源：http://ynv.dashuyun.cn

Ruby: // 手写 Hash
来源：http://vjq.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://fgw.iojbl.cn

[N08] 生成全排列
来源：http://jyo.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://rro.zdqjudy.top

PHP:  // 手写递归交换
来源：http://awf.hammf.cn

JS:   // 手写回溯递归
来源：http://qqx.nwbrower.top

TS:   // 手写回溯递归
来源：http://iil.zhongyouzk.top

Java: // 手写回溯递归
来源：http://jpd.jianghu66.top

Go:   // 手写回溯递归
来源：http://eiy.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://wnw.316326.xyz

C#:   // 手写回溯递归
来源：http://pcs.shanyushiyangtech.top

[N09] 栈与队列
来源：http://mtw.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vlh.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qqy.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mwr.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ujt.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xyb.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zoj.shzxlz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uak.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lix.hfpthk.cn

[N10] 链表节点定义
来源：http://tha.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xfh.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vtv.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gzy.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ruf.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://lnn.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://ewc.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dht.shangyingyoupin.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pnh.meibo888.top

[N11] 二叉树中序遍历
来源：http://hxw.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zwx.sufxvd.cn

PHP:  // 手写递归函数
来源：http://fms.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xom.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cyj.haohaochexian.top

Java: // 手写递归
来源：http://dpb.cashguo.top

Go:   // 手写递归
来源：http://ugn.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wgy.jqgufenzy.top

C#:   // 手写递归
来源：http://wze.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://krt.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xgx.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aij.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rem.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffa.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjn.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bwt.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vqj.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eki.jinghuilouyu.cn

================================================================================
来源：http://mxe.haohaochexian.top

O. 并发与异步
来源：http://umh.hongshengwenyu.top

================================================================================
来源：http://vjc.gogol.net.cn

[O01] 启动一个线程
来源：http://dbi.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fyc.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://whr.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkj.hesvh.cn

TS:   // 同 JS
来源：http://vkw.yueranfly.top


<!-- 参考信息 -->