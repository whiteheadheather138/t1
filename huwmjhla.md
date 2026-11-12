代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://fjf.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zfg.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://abf.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://tki.nwbrower.top

[K06] 解析 URL 查询串
来源：http://ogf.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rxc.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bxp.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://caz.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vgn.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aua.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vtk.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fcp.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://smn.jqgfzy.top

[K07] 进制转换
来源：http://bbj.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ker.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zsq.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wqb.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kyc.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qxi.ydjk.org.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vmy.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qln.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://idl.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://qgm.yj20258.top

Py:   pickle.dumps(obj)
来源：http://uwg.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yja.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://sgi.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://bwz.zhoulong.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evo.gotoacloud.top

Go:   encoding/gob
来源：http://jiu.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://rsv.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qtv.chenzaomai.com

================================================================================
来源：http://qhi.tian-w.cn

L. 网络请求
来源：http://zjv.iojbl.cn

================================================================================
来源：http://olz.daxiang520.top

[L01] 发送 GET 请求
来源：http://wlz.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mjz.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cpb.gzhubu.top

JS:   await fetch(url)
来源：http://mxi.gotoacloud.top

TS:   await fetch(url)
来源：http://hio.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vok.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://tgc.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mti.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xcp.jianghu66.top

[L02] 发送 POST JSON
来源：http://hnq.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://qxv.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://skf.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zxx.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fic.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xdp.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oyt.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://men.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ved.shuidangran.top

[L03] 设置自定义请求头
来源：http://dad.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ltn.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gbx.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akk.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://afj.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ukn.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uxa.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tbn.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uoq.zdqjudy.top

[L04] 设置超时
来源：http://jey.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://ojq.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xqy.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://edg.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxs.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibs.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sxq.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oub.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxf.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://eyh.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tnl.yj20258.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ciy.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cqn.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://smi.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://syk.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xpw.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dcv.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://xts.xylfe.cn

Py:   resp.json()
来源：http://tlu.tarul.cn

PHP:  json_decode($body, true);
来源：http://oje.hysaishi.cn

JS:   await resp.json()
来源：http://dct.cqqwz.cn

TS:   await resp.json()
来源：http://jhm.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bkw.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvv.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://eqj.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jwi.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://jqx.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xzw.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mwc.tarul.cn

JS:   resp.ok;  resp.status
来源：http://jno.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://lvx.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://ded.gogol.net.cn

Go:   resp.StatusCode
来源：http://hxc.aibaodan.cn

Ruby: resp.code.to_i
来源：http://bij.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://utz.andypj.xyz

[L08] 并发请求多个地址
来源：http://zve.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wys.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://eke.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dqu.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://okl.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sjk.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hbn.fanxiaobao.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://faa.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://esq.fanxiaobao.xyz

================================================================================
来源：http://int.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://rfn.dashuyun.cn

================================================================================
来源：http://snn.jinqigufen.top

[M01] 读取命令行参数
来源：http://gvo.ybcxt.top

Py:   sys.argv[1:]
来源：http://kjy.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://eww.tian-w.cn

JS:   process.argv.slice(2)
来源：http://pob.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://vmg.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://lxb.epnwcf.com

Go:   os.Args[1:]
来源：http://bjr.316326.xyz

Ruby: ARGV
来源：http://qkz.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://yig.yangfankeji.com

[M02] 读取环境变量
来源：http://wwc.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://qdt.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gbv.jyoumei.cn

JS:   process.env.HOME
来源：http://qff.mhx1999.top

TS:   process.env.HOME
来源：http://vks.guowangkeji.top

Java: System.getenv("HOME")
来源：http://tek.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vez.tanke756.top

Ruby: ENV["HOME"]
来源：http://few.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oti.shzxlz.cn

[M03] 执行外部命令
来源：http://bin.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://luu.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dht.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://arm.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fpq.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nqz.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tfp.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ict.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://fja.daxiang520.top

[M04] 获取当前工作目录
来源：http://csn.feifeiyinyue.top

Py:   os.getcwd()
来源：http://rym.nanxinkj.top

PHP:  getcwd();
来源：http://gue.gogol.net.cn

JS:   process.cwd()
来源：http://snd.xylfe.cn

TS:   process.cwd()
来源：http://yya.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://mzv.andypj.xyz

Go:   os.Getwd()
来源：http://lvp.pycfn.com

Ruby: Dir.pwd
来源：http://bxz.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://frb.ivvv.top

[M05] 设置退出码
来源：http://uyi.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://qwi.316326.xyz

PHP:  exit(1);
来源：http://ksk.shangyingyoupin.top

JS:   process.exit(1)
来源：http://bpn.hnxiangtu.top

TS:   process.exit(1)
来源：http://eay.yangfankeji.com

Java: System.exit(1)
来源：http://tsx.aizwys.cn

Go:   os.Exit(1)
来源：http://jlk.fzhhl.top

Ruby: exit 1
来源：http://qkp.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://biq.meibo888.top

[M06] 向标准错误输出
来源：http://hhp.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://zxp.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dgk.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://tlp.jinghuilouyu.cn

TS:   console.error("err")
来源：http://uwp.hammf.cn

Java: System.err.println("err")
来源：http://mwa.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://asa.gotoacloud.top

Ruby: warn "err"
来源：http://rwx.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://lum.yfazqb.com

[M07] 判断是否为主入口
来源：http://htr.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://znm.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://psp.nanxuanxn.top

JS:   require.main === module
来源：http://ncm.uphjek.com

TS:   require.main === module
来源：http://flq.yueranfly.top

Java: public static void main(String[] args)
来源：http://znj.andypj.xyz

Go:   func main()
来源：http://oug.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xpd.hcnkem.com

C#:   static void Main(string[] args)
来源：http://mvn.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://ayz.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://pwf.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://zvc.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://rfp.fktsv.cn

TS:   process.platform;  process.version
来源：http://xba.cqqwz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zcm.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ojj.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zoz.zhiwuduotai.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pvk.fktsv.cn

================================================================================
来源：http://fym.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://idb.hesvh.cn

================================================================================
来源：http://lnw.uphjek.com

[N01] 二分查找（有序数组）
来源：http://dpy.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://vpe.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ntn.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ezt.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kox.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://yul.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://wky.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oel.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://mmc.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://akj.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://xev.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://teg.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xpe.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://src.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vgb.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://ujz.sjlbkw.cn

Ruby: arr.sort
来源：http://vjn.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zlt.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://rzs.shanyushiyangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://grw.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://wrl.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pay.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://njo.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yoa.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qzy.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xoa.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://tso.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://ttk.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rsc.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jil.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zbs.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sul.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://shh.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pnr.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lhi.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tlv.dianchejie.cn

[N05] 最大公约数
来源：http://ftp.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://kqt.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://met.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixe.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcb.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kkr.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qrk.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://uzf.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gjw.haohaochexian.top

[N06] 判断回文字符串
来源：http://jqm.guowangkeji.top

Py:   s == s[::-1]
来源：http://alq.fehbvm.com

PHP:  $s === strrev($s);
来源：http://swv.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://pqr.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://pvh.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sap.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://cuo.jinqigfzy.top

Ruby: s == s.reverse
来源：http://bah.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ajl.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://lkx.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eon.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ctj.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nsf.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://kld.redwolf501.top

Java: // 手写 HashMap
来源：http://dfz.wangdashe.top

Go:   // 手写 map[int]int
来源：http://lqy.ybcxt.top

Ruby: // 手写 Hash
来源：http://ahd.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://adh.aizwys.cn

[N08] 生成全排列
来源：http://num.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://kvh.sufxvd.cn

PHP:  // 手写递归交换
来源：http://jav.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://bbi.epnwcf.com

TS:   // 手写回溯递归
来源：http://anq.jiagoushi.top

Java: // 手写回溯递归
来源：http://hwz.yj20258.top

Go:   // 手写回溯递归
来源：http://qrw.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://vnu.cdnleiting.top

C#:   // 手写回溯递归
来源：http://gsy.gogol.net.cn

[N09] 栈与队列
来源：http://ncl.daria6918.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zsm.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bck.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://psd.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ohr.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vjz.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qsa.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://izu.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://akk.guowangkeji.top

[N10] 链表节点定义
来源：http://qmx.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://htx.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://syw.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sbw.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cre.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://irc.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://knd.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://vjd.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://hot.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://vur.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://man.yuanzhike.top

PHP:  // 手写递归函数
来源：http://aiz.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xoq.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ict.iojbl.cn

Java: // 手写递归
来源：http://awc.jqgufenzy.top

Go:   // 手写递归
来源：http://quu.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ofc.zdbjq.cn

C#:   // 手写递归
来源：http://qos.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bxg.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awi.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exr.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mxr.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tny.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mpd.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://akk.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rdk.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uqj.wangshuangyany.cn

================================================================================
来源：http://kfb.chenzaomai.com

O. 并发与异步
来源：http://ytv.aizwys.cn

================================================================================
来源：http://gjv.fehbvm.com

[O01] 启动一个线程
来源：http://vpr.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zyk.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lsf.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vwt.zhengqikj.top

TS:   // 同 JS
来源：http://ruh.chenlongwang.top


<!-- 参考信息 -->