代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tiq.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://avq.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://psq.yuanzhike.top

[K05] 深拷贝对象
来源：http://wzw.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://hzm.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://pog.ppjwa.cn

JS:   structuredClone(obj)
来源：http://wvy.sxryk.cn

TS:   structuredClone(obj)
来源：http://rzc.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jee.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xkn.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bgv.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jjc.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://xaz.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nnz.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ibl.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://olr.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oeb.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ipg.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jpe.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fwe.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dee.yj202588.top

[K07] 进制转换
来源：http://wqp.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gnq.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hkn.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://efb.yueranfly.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://naq.aizwys.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fnk.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hkd.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://haz.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yyq.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://hff.tarul.cn

Py:   pickle.dumps(obj)
来源：http://car.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mis.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://uwf.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://ykt.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rds.xylfe.cn

Go:   encoding/gob
来源：http://iyk.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://byl.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yek.hfpthk.cn

================================================================================
来源：http://knu.xziqi.cn

L. 网络请求
来源：http://aes.tanke756.top

================================================================================
来源：http://gbw.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://raf.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sbk.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hai.c1oappe.top

JS:   await fetch(url)
来源：http://ofs.aizwys.cn

TS:   await fetch(url)
来源：http://duf.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cwa.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://svp.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rim.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dgf.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://rjk.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://kyl.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pay.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdv.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://erp.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://usy.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qng.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fvw.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zhx.sxryk.cn

[L03] 设置自定义请求头
来源：http://eab.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://znc.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://usk.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dmi.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dut.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://btd.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mrv.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ffz.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sqk.uphjek.com

[L04] 设置超时
来源：http://yaj.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://mmm.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hup.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywg.birdmap.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tzl.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yeu.gogol.net.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://smj.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://neq.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iid.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://ahj.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gqs.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gki.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xun.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mzw.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vog.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pcz.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hns.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xrv.uphjek.com

[L06] 解析响应为 JSON
来源：http://fpn.daria6918.cn

Py:   resp.json()
来源：http://hxg.daxiang520.top

PHP:  json_decode($body, true);
来源：http://xnl.gaohongyu789.top

JS:   await resp.json()
来源：http://wde.52xcode.cn

TS:   await resp.json()
来源：http://qqs.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mcl.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mre.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://xxe.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zmp.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://xjz.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zer.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qza.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://rqm.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://vzj.sysykeji.top

Java: resp.statusCode()
来源：http://eed.daxiang520.top

Go:   resp.StatusCode
来源：http://pdb.andypj.xyz

Ruby: resp.code.to_i
来源：http://fdo.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://rqr.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://dum.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gfj.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://oea.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utu.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjz.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ftx.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dus.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tea.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fzi.sysykeji.top

================================================================================
来源：http://lro.svipenyu.cn

M. 命令行 / 进程 / 环境
来源：http://wns.chenzaomai.com

================================================================================
来源：http://zul.yueranfly.top

[M01] 读取命令行参数
来源：http://kjk.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://upt.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://lqd.316326.xyz

JS:   process.argv.slice(2)
来源：http://dun.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://nbu.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://kms.zhoulong.xyz

Go:   os.Args[1:]
来源：http://ofu.jianghu66.top

Ruby: ARGV
来源：http://hqo.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://ohg.hysaishi.cn

[M02] 读取环境变量
来源：http://fdl.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://ytn.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ieh.fengsongda.top

JS:   process.env.HOME
来源：http://erb.9152youxi.cn

TS:   process.env.HOME
来源：http://nkz.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://qer.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lct.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://wef.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cqf.ivvv.top

[M03] 执行外部命令
来源：http://phj.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://acs.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hvx.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bat.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aby.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://txc.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pnr.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://aln.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://qcq.redwolf501.top

[M04] 获取当前工作目录
来源：http://kcv.guannengcc.top

Py:   os.getcwd()
来源：http://gov.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://bse.fanxiaobao.xyz

JS:   process.cwd()
来源：http://pal.wangdashe.top

TS:   process.cwd()
来源：http://ooa.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://yuc.jlsjyb.cn

Go:   os.Getwd()
来源：http://hxk.hfpthk.cn

Ruby: Dir.pwd
来源：http://ffv.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dvn.yonumen.top

[M05] 设置退出码
来源：http://unw.gzhubu.top

Py:   sys.exit(1)
来源：http://mzx.yueranfly.top

PHP:  exit(1);
来源：http://urj.316326.xyz

JS:   process.exit(1)
来源：http://unc.sweek.top

TS:   process.exit(1)
来源：http://btg.jqgfzy.top

Java: System.exit(1)
来源：http://gye.yueranfly.top

Go:   os.Exit(1)
来源：http://una.hywenlv.cn

Ruby: exit 1
来源：http://vwc.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://seb.bjfxy.top

[M06] 向标准错误输出
来源：http://blw.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://uem.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://ifr.jqgfzy.top

JS:   console.error("err")
来源：http://hqi.ydzc1.top

TS:   console.error("err")
来源：http://rbw.snrcjt.cn

Java: System.err.println("err")
来源：http://hoh.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nzj.fengsongda.top

Ruby: warn "err"
来源：http://yfz.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://adu.uphjek.com

[M07] 判断是否为主入口
来源：http://tdt.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://oet.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xzp.hnqzz.top

JS:   require.main === module
来源：http://agj.hesvh.cn

TS:   require.main === module
来源：http://nsd.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://zyj.tanke756.top

Go:   func main()
来源：http://yai.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ndw.yfazqb.com

C#:   static void Main(string[] args)
来源：http://jhb.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://yds.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://bln.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://jjs.xziqi.cn

JS:   process.platform;  process.version
来源：http://irk.zdqjudy.top

TS:   process.platform;  process.version
来源：http://plq.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ixv.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zsk.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dtp.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://eqi.quarkkingdee.top

================================================================================
来源：http://rgb.jinghuilouyu.cn

N. 数据结构与算法
来源：http://egu.cashguo.top

================================================================================
来源：http://mwq.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://dda.jinghuilouyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fco.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ufz.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zmx.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bin.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lpe.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://bbz.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fnq.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vdk.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://qch.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://rpw.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vyv.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://znp.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ogi.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://liq.tarul.cn

Go:   slices.Sort(arr)
来源：http://vmv.ppjwa.cn

Ruby: arr.sort
来源：http://nax.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://twi.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://msu.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bgq.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://wzk.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jsa.316326.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvp.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xof.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tqs.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gzd.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://qgs.daxiang520.top

[N04] 斐波那契数列
来源：http://rft.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ier.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pge.zhaomingkeji.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://riu.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rfd.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bbt.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jwn.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jei.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://csx.hcnkem.com

[N05] 最大公约数
来源：http://zlc.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ibc.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ydn.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aex.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lta.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dsu.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byl.xziqi.cn

Ruby: a.gcd(b)
来源：http://dky.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dty.jinyuanbaomall.cn

[N06] 判断回文字符串
来源：http://wyh.bjfxy.top

Py:   s == s[::-1]
来源：http://llo.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://mxz.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://hfs.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://abl.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nli.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://hwm.ydjk.org.cn

Ruby: s == s.reverse
来源：http://vii.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hqy.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://djd.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ins.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axc.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dqm.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://rpe.fehbvm.com

Java: // 手写 HashMap
来源：http://zko.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://gvj.ehwqpu.com

Ruby: // 手写 Hash
来源：http://jer.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ink.havefunace.top

[N08] 生成全排列
来源：http://fue.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://pfk.zycfv.cn

PHP:  // 手写递归交换
来源：http://nkx.9152youxi.cn

JS:   // 手写回溯递归
来源：http://hdx.haohaochexian.top

TS:   // 手写回溯递归
来源：http://cxg.yfazqb.com

Java: // 手写回溯递归
来源：http://xon.hcnkem.com

Go:   // 手写回溯递归
来源：http://rcj.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://ylm.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://mkf.smart0.xyz

[N09] 栈与队列
来源：http://wmd.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xtb.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zyz.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uko.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rjd.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://okt.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://att.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qky.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ket.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://vqg.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cfv.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uig.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eqj.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gfj.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://izy.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://zcg.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lul.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yrm.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://kmp.mhx1999.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fom.0kj1m.cn

PHP:  // 手写递归函数
来源：http://qje.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvv.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bkp.gzhubu.top

Java: // 手写递归
来源：http://nzd.hysaishi.cn

Go:   // 手写递归
来源：http://jnk.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lur.guowangkeji.top

C#:   // 手写递归
来源：http://kaq.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wgs.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ixq.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tct.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qxe.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygp.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sbr.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ifo.cdnleiting.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aty.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ore.jinyuanbaomall.cn


<!-- 参考信息 -->