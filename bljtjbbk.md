代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qqh.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://myi.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mkj.guowangkeji.top

[K05] 深拷贝对象
来源：http://hgo.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://vxt.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://wkw.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://upo.tian-w.cn

TS:   structuredClone(obj)
来源：http://ogj.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zks.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ozi.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bcw.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://mzm.ivvv.top

[K06] 解析 URL 查询串
来源：http://hdq.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wdi.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwf.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ghp.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fkz.aizwys.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gko.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xwq.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qgi.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zqe.haohaochexian.top

[K07] 进制转换
来源：http://pyu.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmj.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://olz.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kbg.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xmh.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kzf.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jir.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ucw.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pqr.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://ygs.yuxming.cn

Py:   pickle.dumps(obj)
来源：http://cdx.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fwt.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://xex.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://mrw.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ohq.zhijiandao.cn

Go:   encoding/gob
来源：http://ohl.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://lic.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tww.shangyingyoupin.top

================================================================================
来源：http://cpw.sufxvd.cn

L. 网络请求
来源：http://wck.sysykeji.top

================================================================================
来源：http://pmn.svipenyu.cn

[L01] 发送 GET 请求
来源：http://ftz.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ylw.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ine.yj20258888.top

JS:   await fetch(url)
来源：http://gjp.zhoulong.xyz

TS:   await fetch(url)
来源：http://auw.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cos.yangfankeji.com

Go:   resp, err := http.Get(url)
来源：http://fqw.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eyl.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ujq.ehwqpu.com

[L02] 发送 POST JSON
来源：http://pbs.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://uwk.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jmh.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hby.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gyn.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jej.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gbs.shanyushiyangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://krp.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vgx.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://xbq.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://koa.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lzu.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wii.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ict.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aae.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wtg.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://whz.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oss.hesvh.cn

[L04] 设置超时
来源：http://wiw.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://rkn.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ary.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vpt.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blv.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zof.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yyd.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://igz.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cuw.kuanghao11.cn

[L05] 上传文件（multipart）
来源：http://ggd.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zhq.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kvt.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pll.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://utf.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jiz.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cei.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eaq.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fag.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://wck.pycfn.com

Py:   resp.json()
来源：http://cvs.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://oii.zhoulong.xyz

JS:   await resp.json()
来源：http://cgw.zhijiandao.cn

TS:   await resp.json()
来源：http://cff.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://plv.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mnz.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ive.daxiang520.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xqw.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://jhg.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fcm.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fbw.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://red.tarul.cn

TS:   resp.ok;  resp.status
来源：http://ile.ydzc1.top

Java: resp.statusCode()
来源：http://bzf.zhongyouzk.top

Go:   resp.StatusCode
来源：http://iza.chenzaomai.com

Ruby: resp.code.to_i
来源：http://ylu.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://cvu.daria6918.cn

[L08] 并发请求多个地址
来源：http://ljr.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bqn.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://vew.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ytl.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tlu.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pzt.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oyu.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pml.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://atg.tanke756.top

================================================================================
来源：http://xly.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://our.ctjpmb.com

================================================================================
来源：http://ecy.yj202588.top

[M01] 读取命令行参数
来源：http://frz.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://ymf.yvedp.cn

PHP:  $argv;  $argc;
来源：http://fli.iojbl.cn

JS:   process.argv.slice(2)
来源：http://ckg.xziqi.cn

TS:   process.argv.slice(2)
来源：http://nmm.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://mre.jianghu66.top

Go:   os.Args[1:]
来源：http://bal.hcnkem.com

Ruby: ARGV
来源：http://fvi.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://nzf.jinqigfzy.top

[M02] 读取环境变量
来源：http://noi.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://erf.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ekl.shuidangran.top

JS:   process.env.HOME
来源：http://fja.daria6918.cn

TS:   process.env.HOME
来源：http://xmg.nwbrower.top

Java: System.getenv("HOME")
来源：http://qzf.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://khd.epnwcf.com

Ruby: ENV["HOME"]
来源：http://scu.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tvj.epnwcf.com

[M03] 执行外部命令
来源：http://ozu.cashguo.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ycx.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jeo.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gyw.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://myn.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zgf.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aib.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pyq.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://fjc.ctjpmb.com

[M04] 获取当前工作目录
来源：http://wpl.xuanzx.com

Py:   os.getcwd()
来源：http://iga.nanxinkj.top

PHP:  getcwd();
来源：http://xtj.hcnkem.com

JS:   process.cwd()
来源：http://cna.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://hwv.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://epz.smart0.xyz

Go:   os.Getwd()
来源：http://wvi.gogol.net.cn

Ruby: Dir.pwd
来源：http://msx.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rsy.aibaodan.cn

[M05] 设置退出码
来源：http://xdu.cucudq.cn

Py:   sys.exit(1)
来源：http://pjc.9152youxi.cn

PHP:  exit(1);
来源：http://qkd.andypj.xyz

JS:   process.exit(1)
来源：http://luv.havefunace.top

TS:   process.exit(1)
来源：http://xac.c1oappe.top

Java: System.exit(1)
来源：http://gtn.ivvv.top

Go:   os.Exit(1)
来源：http://peu.aizwys.cn

Ruby: exit 1
来源：http://efd.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dqj.tarul.cn

[M06] 向标准错误输出
来源：http://muq.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://soj.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bzf.316326.xyz

JS:   console.error("err")
来源：http://kqy.quarkkingdee.top

TS:   console.error("err")
来源：http://lop.ydzc1.top

Java: System.err.println("err")
来源：http://cxl.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rld.chenlongwang.top

Ruby: warn "err"
来源：http://ral.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://tbw.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://nyp.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://qmf.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://slw.ehwqpu.com

JS:   require.main === module
来源：http://oqk.hnqzz.top

TS:   require.main === module
来源：http://wkb.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://umv.sxryk.cn

Go:   func main()
来源：http://xni.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jta.uphjek.com

C#:   static void Main(string[] args)
来源：http://imy.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://rlr.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ggc.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://jtd.ydzc1.top

JS:   process.platform;  process.version
来源：http://ljh.chenlongwang.top

TS:   process.platform;  process.version
来源：http://qtn.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yrk.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nts.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://whc.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgf.sxryk.cn

================================================================================
来源：http://dsb.daxiang520.top

N. 数据结构与算法
来源：http://xsu.jianghu66.top

================================================================================
来源：http://rcs.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://nub.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wyp.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://psi.ppjwa.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jah.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svi.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://jhs.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://hfq.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ssj.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://nre.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://xyk.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://ymy.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yyp.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aos.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ihx.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tgf.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://eoh.yonumen.top

Ruby: arr.sort
来源：http://gwh.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fao.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://vny.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lov.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://dac.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjt.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygw.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tzp.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zzz.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kbk.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://vpd.iojbl.cn

[N04] 斐波那契数列
来源：http://zsr.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://udo.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cad.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://asw.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jwa.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ijt.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lie.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uio.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://umk.yfazqb.com

[N05] 最大公约数
来源：http://xhb.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://zan.guannengcc.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sxy.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sus.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgo.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rlc.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wcj.redwolf501.top

Ruby: a.gcd(b)
来源：http://ulm.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gdj.andypj.xyz

[N06] 判断回文字符串
来源：http://btu.tanke756.top

Py:   s == s[::-1]
来源：http://zvd.xuanzx.com

PHP:  $s === strrev($s);
来源：http://yol.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://gpk.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://sqn.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rue.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://dcx.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://yxe.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eui.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://nwv.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bca.jinyuanbaomall.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yxb.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mjg.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://zql.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://siw.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://ljs.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://cxh.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xrr.gaohongyu789.top

[N08] 生成全排列
来源：http://pxq.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://abq.mhx1999.top

PHP:  // 手写递归交换
来源：http://shy.epnwcf.com

JS:   // 手写回溯递归
来源：http://jre.birdmap.top

TS:   // 手写回溯递归
来源：http://sfr.yueranfly.top

Java: // 手写回溯递归
来源：http://vif.daria6918.cn

Go:   // 手写回溯递归
来源：http://bbk.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://nls.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://dgu.sufxvd.cn

[N09] 栈与队列
来源：http://axd.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zqo.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ray.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jbq.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ume.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nov.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wcx.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://omv.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://umt.yanxiufei.cn

[N10] 链表节点定义
来源：http://wnv.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://prq.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://eaa.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uja.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://usr.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://sex.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fmj.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bhw.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uev.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://kaz.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xhy.haohaochexian.top

PHP:  // 手写递归函数
来源：http://sui.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zwo.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bxt.9152youxi.cn

Java: // 手写递归
来源：http://ekx.9152youxi.cn

Go:   // 手写递归
来源：http://ncj.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uan.yueranfly.top

C#:   // 手写递归
来源：http://cgc.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osw.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pbh.jinyuanbaomall.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tkw.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvs.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://taz.redwolf501.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://crh.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dvp.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://poc.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eaa.svipenyu.cn


<!-- 参考信息 -->