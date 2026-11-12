代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://moj.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gwv.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pru.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vkr.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://zdc.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mly.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xch.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bca.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://scx.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qlu.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jsk.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://exm.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hlj.cashguo.top

[K07] 进制转换
来源：http://rya.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oax.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kkz.mhx1999.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://byx.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dxu.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xre.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vxi.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tyq.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://skg.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://vjq.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://max.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://hzc.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://yxp.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://hhz.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kof.jyoumei.cn

Go:   encoding/gob
来源：http://pmd.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://qgu.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://idi.zhixingplan.top

================================================================================
来源：http://skz.hesvh.cn

L. 网络请求
来源：http://egf.guannengcc.top

================================================================================
来源：http://ope.hnqzz.top

[L01] 发送 GET 请求
来源：http://dei.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://has.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://frp.nanxinkj.top

JS:   await fetch(url)
来源：http://aqs.gaohongyu789.top

TS:   await fetch(url)
来源：http://ljs.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dkm.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://oqr.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://foc.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dnk.gotoacloud.top

[L02] 发送 POST JSON
来源：http://wry.yj20258.top

Py:   requests.post(url, json={"a": 1})
来源：http://tnp.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://buh.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ait.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sco.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hkw.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lfd.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gxd.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ogk.redwolf501.top

[L03] 设置自定义请求头
来源：http://vlj.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mcf.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qvt.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zlc.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wcj.birdmap.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ddk.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zfu.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nwo.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pfk.52xcode.cn

[L04] 设置超时
来源：http://igc.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://nut.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sdj.yj20258888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://orf.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xad.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://svh.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uah.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kcz.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pfv.svipenyu.cn

[L05] 上传文件（multipart）
来源：http://ttp.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://soc.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://msy.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mwv.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vuw.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mjy.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nvj.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sul.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pfi.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://qgd.zhaomingkeji.xyz

Py:   resp.json()
来源：http://ibt.52xcode.cn

PHP:  json_decode($body, true);
来源：http://wpc.jqgfzy.top

JS:   await resp.json()
来源：http://xrn.tarul.cn

TS:   await resp.json()
来源：http://ppl.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zfy.xingfuxueyuan.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jvz.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://rab.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bsu.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://mco.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vwe.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cga.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://ahl.pycfn.com

TS:   resp.ok;  resp.status
来源：http://ipu.feifeiyinyue.top

Java: resp.statusCode()
来源：http://dsz.snrcjt.cn

Go:   resp.StatusCode
来源：http://xye.cucudq.cn

Ruby: resp.code.to_i
来源：http://ulp.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://ksb.dashuyun.cn

[L08] 并发请求多个地址
来源：http://zil.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vmb.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://veg.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bvf.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqq.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://voc.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cdr.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xtg.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jte.ybcxt.top

================================================================================
来源：http://abf.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://sig.vqdsnc.cn

================================================================================
来源：http://rtn.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://mnf.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://bfp.aizwys.cn

PHP:  $argv;  $argc;
来源：http://nil.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://riz.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://ywp.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://dao.bjfxy.top

Go:   os.Args[1:]
来源：http://imh.fanxiaobao.xyz

Ruby: ARGV
来源：http://wwl.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://kgz.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://nej.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://ldt.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uer.kuanghao11.cn

JS:   process.env.HOME
来源：http://fxu.ybcxt.top

TS:   process.env.HOME
来源：http://xwt.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://gcp.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mzs.pycfn.com

Ruby: ENV["HOME"]
来源：http://ybi.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pop.jlsjyb.cn

[M03] 执行外部命令
来源：http://cyf.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hgc.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hdu.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ncf.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://osn.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ews.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bfk.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wrr.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://idh.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://xnz.jqgufenzy.top

Py:   os.getcwd()
来源：http://aoo.vqdsnc.cn

PHP:  getcwd();
来源：http://ouc.yangfankeji.com

JS:   process.cwd()
来源：http://cff.daxiang520.top

TS:   process.cwd()
来源：http://yls.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://ooj.xylfe.cn

Go:   os.Getwd()
来源：http://btg.zhijiandao.cn

Ruby: Dir.pwd
来源：http://duk.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://thv.nanxinkj.top

[M05] 设置退出码
来源：http://bfa.hfpthk.cn

Py:   sys.exit(1)
来源：http://vox.jinqigfzy.top

PHP:  exit(1);
来源：http://jkz.shuidangran.top

JS:   process.exit(1)
来源：http://puw.bbcook.cn

TS:   process.exit(1)
来源：http://zup.xziqi.cn

Java: System.exit(1)
来源：http://evm.xylfe.cn

Go:   os.Exit(1)
来源：http://iha.hcnkem.com

Ruby: exit 1
来源：http://avo.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rvk.fehbvm.com

[M06] 向标准错误输出
来源：http://uuv.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://brq.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cdi.meibo888.top

JS:   console.error("err")
来源：http://msz.0kj1m.cn

TS:   console.error("err")
来源：http://qta.aizwys.cn

Java: System.err.println("err")
来源：http://amm.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://izh.havefunace.top

Ruby: warn "err"
来源：http://ujc.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://hsk.chenzaomai.com

[M07] 判断是否为主入口
来源：http://ynu.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://bre.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://egs.jlsjyb.cn

JS:   require.main === module
来源：http://mep.hongshengwenyu.top

TS:   require.main === module
来源：http://eco.hcnkem.com

Java: public static void main(String[] args)
来源：http://hbx.hesvh.cn

Go:   func main()
来源：http://nal.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nij.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://ule.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://rbq.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://etn.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://chq.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://zco.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://ene.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vnp.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gsv.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://umq.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://asy.smart0.xyz

================================================================================
来源：http://bvx.cdnleiting.top

N. 数据结构与算法
来源：http://mqh.zhiwuduotai.top

================================================================================
来源：http://ahm.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://vko.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://tdu.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qzd.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wku.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wru.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dof.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://srx.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xtw.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://ahx.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://sxf.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://igk.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kdp.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://npo.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hrl.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sri.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://hiz.havefunace.top

Ruby: arr.sort
来源：http://cjk.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nls.tanke756.top

[N03] 快速排序（分治示例）
来源：http://wri.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tsj.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://amk.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oxp.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qtl.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nlw.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lke.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pnv.quarkkingdee.top

C#:   // 手写递归，或 Array.Sort
来源：http://rwc.hesvh.cn

[N04] 斐波那契数列
来源：http://twa.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xdm.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fnp.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ynq.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pes.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gne.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nky.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lxn.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eyz.yj202588.top

[N05] 最大公约数
来源：http://wbb.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://oyr.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kjz.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cxl.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvg.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eow.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://esr.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://ftu.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nhr.yj202588.top

[N06] 判断回文字符串
来源：http://wri.zycfv.cn

Py:   s == s[::-1]
来源：http://shc.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://asy.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://pzf.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://ypu.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bdv.sxryk.cn

Go:   // 双指针从两端比较
来源：http://fhl.ybcxt.top

Ruby: s == s.reverse
来源：http://mph.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://nqg.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://rmb.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nft.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uqy.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fnp.tanke756.top

TS:   // 手写 Map<string, number>
来源：http://den.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://vpc.fzhhl.top

Go:   // 手写 map[int]int
来源：http://eav.dianchejie.cn

Ruby: // 手写 Hash
来源：http://qxn.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vzo.sjlbkw.cn

[N08] 生成全排列
来源：http://fyv.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://pbl.9152youxi.cn

PHP:  // 手写递归交换
来源：http://ybm.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://hlx.sysykeji.top

TS:   // 手写回溯递归
来源：http://miz.zhengqikj.top

Java: // 手写回溯递归
来源：http://cjd.c1oappe.top

Go:   // 手写回溯递归
来源：http://ijz.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://heu.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://kvg.andypj.xyz

[N09] 栈与队列
来源：http://zhf.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gfi.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uzv.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wbi.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmw.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uhq.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jzn.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uwe.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nya.pycfn.com

[N10] 链表节点定义
来源：http://hub.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bel.gzhubu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qox.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jgp.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hwc.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://skm.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://utr.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ria.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zmt.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://anl.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zat.jqgfzy.top

PHP:  // 手写递归函数
来源：http://vzs.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qou.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ljt.hongshengwenyu.top

Java: // 手写递归
来源：http://okk.zdbjq.cn

Go:   // 手写递归
来源：http://ska.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wkz.cqqwz.cn

C#:   // 手写递归
来源：http://dhy.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lou.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mqd.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blg.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dzj.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://day.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zhg.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://okw.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aep.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yvc.jianghu66.top

================================================================================
来源：http://vnx.sweek.top

O. 并发与异步
来源：http://crt.zhongyouzk.top

================================================================================
来源：http://fnc.svipenyu.cn

[O01] 启动一个线程
来源：http://cle.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xjr.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nah.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nve.chenzaomai.com

TS:   // 同 JS
来源：http://jnk.ybcxt.top


<!-- 参考信息 -->