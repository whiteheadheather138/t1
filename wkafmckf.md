代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hor.kuanghao11.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ltc.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wwg.bjfxy.top

[K05] 深拷贝对象
来源：http://jse.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://njx.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://dxz.c1oappe.top

JS:   structuredClone(obj)
来源：http://cye.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://skz.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://anl.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jxw.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rfp.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://brc.xinyue.icu

[K06] 解析 URL 查询串
来源：http://ewc.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://awb.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fxt.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fsa.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rwg.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xeb.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpr.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uex.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zch.zhengqikj.top

[K07] 进制转换
来源：http://clw.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lmc.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cdl.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cfi.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fks.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zyk.yangfankeji.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vce.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://har.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kiw.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ejs.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://hpj.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://uci.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://hrp.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://jlg.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dxn.tianlin.xyz

Go:   encoding/gob
来源：http://fcn.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://mxr.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wpg.sweek.top

================================================================================
来源：http://udp.gotoacloud.top

L. 网络请求
来源：http://ink.zhengqikj.top

================================================================================
来源：http://cvv.chenlongwang.top

[L01] 发送 GET 请求
来源：http://wqk.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grh.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgl.hnqzz.top

JS:   await fetch(url)
来源：http://oqf.wangshuangyany.cn

TS:   await fetch(url)
来源：http://deo.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptc.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://qnj.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nwy.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://doo.hesvh.cn

[L02] 发送 POST JSON
来源：http://fyc.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mpv.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sbi.snrcjt.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ede.xingfuxueyuan.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gzi.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vaf.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ade.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://frg.hysaishi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mmo.cdnleiting.top

[L03] 设置自定义请求头
来源：http://wmq.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wll.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://age.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opq.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wuj.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vhk.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ftu.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lvi.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hyo.zhijiandao.cn

[L04] 设置超时
来源：http://pnb.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://mqh.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qnz.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjl.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krs.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ulr.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zpi.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mno.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iey.gzhubu.top

[L05] 上传文件（multipart）
来源：http://ywh.vqdsnc.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uso.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rze.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nuw.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hui.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tam.yuxming.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fgh.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dce.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hmz.yj20258888.top

[L06] 解析响应为 JSON
来源：http://szq.bjfxy.top

Py:   resp.json()
来源：http://njz.meibo888.top

PHP:  json_decode($body, true);
来源：http://sxe.gzhubu.top

JS:   await resp.json()
来源：http://biq.andypj.xyz

TS:   await resp.json()
来源：http://gut.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wqg.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zpv.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://buv.xylfe.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jom.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://jaz.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oel.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfn.tanke756.top

JS:   resp.ok;  resp.status
来源：http://qbu.yongpay.top

TS:   resp.ok;  resp.status
来源：http://wvy.hcnkem.com

Java: resp.statusCode()
来源：http://sxs.yuanzhike.top

Go:   resp.StatusCode
来源：http://nmu.sysykeji.top

Ruby: resp.code.to_i
来源：http://aew.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://kru.tanke756.top

[L08] 并发请求多个地址
来源：http://unr.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rvf.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://yvo.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uis.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wlp.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uax.sweek.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dnc.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://slm.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hov.jianghu66.top

================================================================================
来源：http://izg.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://pmg.guowangkeji.top

================================================================================
来源：http://ovq.svipenyu.cn

[M01] 读取命令行参数
来源：http://dip.316326.xyz

Py:   sys.argv[1:]
来源：http://yeu.xinyue.icu

PHP:  $argv;  $argc;
来源：http://owg.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://ooh.shuidangran.top

TS:   process.argv.slice(2)
来源：http://ksn.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://rrr.dashuyun.cn

Go:   os.Args[1:]
来源：http://lqd.guowangkeji.top

Ruby: ARGV
来源：http://mrj.fengsongda.top

C#:   args 数组（Main 方法参数）
来源：http://gir.cucudq.cn

[M02] 读取环境变量
来源：http://aji.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://nxv.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wnr.ydjk.org.cn

JS:   process.env.HOME
来源：http://tcx.ydzc1.top

TS:   process.env.HOME
来源：http://qbr.yuxming.cn

Java: System.getenv("HOME")
来源：http://jxx.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nrr.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://mwf.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cqi.ybcxt.top

[M03] 执行外部命令
来源：http://tlk.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tao.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://upo.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hiy.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zqa.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gcw.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qmy.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://mex.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://yrm.cdnleiting.top

[M04] 获取当前工作目录
来源：http://pkm.wangshuangyany.cn

Py:   os.getcwd()
来源：http://oky.ehwqpu.com

PHP:  getcwd();
来源：http://igb.cheryme.top

JS:   process.cwd()
来源：http://qrr.ppjwa.cn

TS:   process.cwd()
来源：http://vmb.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bcw.daria6918.cn

Go:   os.Getwd()
来源：http://rby.c1oappe.top

Ruby: Dir.pwd
来源：http://ssf.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://kes.ybcxt.top

[M05] 设置退出码
来源：http://fhk.zhengqikj.top

Py:   sys.exit(1)
来源：http://rnk.hnqzz.top

PHP:  exit(1);
来源：http://smt.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://hjb.yj20258888.top

TS:   process.exit(1)
来源：http://ldx.hammf.cn

Java: System.exit(1)
来源：http://dfj.zhengqikj.top

Go:   os.Exit(1)
来源：http://ddk.daria6918.cn

Ruby: exit 1
来源：http://utj.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wzn.yongpay.top

[M06] 向标准错误输出
来源：http://cmm.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://evh.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://eyv.fktsv.cn

JS:   console.error("err")
来源：http://etx.nanxuanxn.top

TS:   console.error("err")
来源：http://axk.zhengqikj.top

Java: System.err.println("err")
来源：http://nnp.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://slc.ybcxt.top

Ruby: warn "err"
来源：http://qos.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://wji.xuanzx.com

[M07] 判断是否为主入口
来源：http://dcx.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://ojz.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hcl.xinyue.icu

JS:   require.main === module
来源：http://jlq.nanxuanxn.top

TS:   require.main === module
来源：http://bzi.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://mvd.smart0.xyz

Go:   func main()
来源：http://qsg.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bgb.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://bml.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://nla.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://uea.fengsongda.top

PHP:  PHP_OS;  phpversion();
来源：http://klm.sxryk.cn

JS:   process.platform;  process.version
来源：http://uiw.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://gvy.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ocg.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hcj.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aud.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cnd.zycfv.cn

================================================================================
来源：http://uha.cashguo.top

N. 数据结构与算法
来源：http://pyk.zhongyouzk.top

================================================================================
来源：http://uph.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://mfq.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://ifx.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dbs.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aif.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://whi.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://slt.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://dvc.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rux.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://krf.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://btl.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://poi.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://svc.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yel.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://okz.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ivt.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://tko.nanxinkj.top

Ruby: arr.sort
来源：http://yaq.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dgf.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://tdp.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pnh.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://kpj.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lcs.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nsa.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uad.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gds.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://smw.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://lhl.cheryme.top

[N04] 斐波那契数列
来源：http://eku.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://swd.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rrw.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wxa.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rum.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://joa.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wsl.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sof.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pda.jiagoushi.top

[N05] 最大公约数
来源：http://lbp.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://jkh.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eor.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tbe.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://auh.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://khe.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://znn.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://vhb.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dtx.hammf.cn

[N06] 判断回文字符串
来源：http://yif.yj20258888.top

Py:   s == s[::-1]
来源：http://jjq.yongpay.top

PHP:  $s === strrev($s);
来源：http://bgy.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://ckq.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://bip.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://itb.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://hij.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://xcg.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gyr.uphjek.com

[N07] 两数之和（返回下标）
来源：http://sar.wangdashe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tkr.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jjm.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ybc.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://shy.meibo888.top

Java: // 手写 HashMap
来源：http://gfq.wangdashe.top

Go:   // 手写 map[int]int
来源：http://mcj.ivvv.top

Ruby: // 手写 Hash
来源：http://ycn.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://deu.tian-w.cn

[N08] 生成全排列
来源：http://clr.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://bbv.jqgfzy.top

PHP:  // 手写递归交换
来源：http://skt.yueranfly.top

JS:   // 手写回溯递归
来源：http://kga.iojbl.cn

TS:   // 手写回溯递归
来源：http://ckc.gogol.net.cn

Java: // 手写回溯递归
来源：http://gdq.daria6918.cn

Go:   // 手写回溯递归
来源：http://cmi.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://nqy.xuanzx.com

C#:   // 手写回溯递归
来源：http://dus.cucudq.cn

[N09] 栈与队列
来源：http://dwe.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://icn.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vvw.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cwo.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pts.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gqw.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fzg.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xzq.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://obj.zdbjq.cn

[N10] 链表节点定义
来源：http://xsz.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ftb.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xpu.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://apy.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uwb.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://ixo.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sgn.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pvh.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xbb.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://rcg.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dzs.0kj1m.cn

PHP:  // 手写递归函数
来源：http://zfs.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ntp.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rre.smart0.xyz

Java: // 手写递归
来源：http://scm.jianghu66.top

Go:   // 手写递归
来源：http://vdn.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://utf.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ioy.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xba.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tgp.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfn.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://czn.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cbk.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eym.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cjd.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pfc.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zhs.chenlongwang.top


<!-- 参考信息 -->