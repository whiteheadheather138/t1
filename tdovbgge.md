代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wxt.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lwf.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zoy.guowangkeji.top

[K05] 深拷贝对象
来源：http://fnl.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://soo.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://thn.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://nfq.tianlin.xyz

TS:   structuredClone(obj)
来源：http://jro.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://uho.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://atd.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nyc.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://njq.andypj.xyz

[K06] 解析 URL 查询串
来源：http://yug.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://msy.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dco.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yzi.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hpl.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hax.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://qcn.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xtx.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fjw.sweek.top

[K07] 进制转换
来源：http://kbl.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmu.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssl.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fos.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cnh.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tux.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://prg.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fze.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://akn.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://nqk.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://syt.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cif.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://mee.cashguo.top

TS:   v8.serialize(obj)        // Node
来源：http://bhv.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mcz.ydzc1.top

Go:   encoding/gob
来源：http://afk.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://psf.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pjk.chenzaomai.com

================================================================================
来源：http://cgu.zhixingplan.top

L. 网络请求
来源：http://kam.shuidangran.top

================================================================================
来源：http://pnr.tanke756.top

[L01] 发送 GET 请求
来源：http://bpp.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uqz.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iup.cheryme.top

JS:   await fetch(url)
来源：http://nvl.vehdjk.com

TS:   await fetch(url)
来源：http://xfj.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://von.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://twv.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iia.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://glu.dashuyun.cn

[L02] 发送 POST JSON
来源：http://wkj.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://uhg.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jyv.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fxx.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gft.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pas.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vbd.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sqx.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qnd.nwbrower.top

[L03] 设置自定义请求头
来源：http://wxu.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqh.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xur.nanxinkj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wav.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbl.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wni.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uib.bbcook.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbe.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pei.svipenyu.cn

[L04] 设置超时
来源：http://wfd.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://vav.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqi.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xbi.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sct.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ecr.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oac.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tuw.smart0.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gmk.sxryk.cn

[L05] 上传文件（multipart）
来源：http://shh.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hju.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wfx.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hlh.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ujp.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dqb.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wnq.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xtv.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aou.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://yjr.hcnkem.com

Py:   resp.json()
来源：http://tfp.yonumen.top

PHP:  json_decode($body, true);
来源：http://rfn.yongpay.top

JS:   await resp.json()
来源：http://kvz.nanxuanxn.top

TS:   await resp.json()
来源：http://cqx.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nya.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cmm.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://vmp.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ovp.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://nhs.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hoh.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://urm.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://irf.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://dpv.hysaishi.cn

Java: resp.statusCode()
来源：http://gpy.yvedp.cn

Go:   resp.StatusCode
来源：http://yps.yuxming.cn

Ruby: resp.code.to_i
来源：http://spc.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://jck.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://nhf.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mhq.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://nrg.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bgy.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hma.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fxr.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wja.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oox.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lpd.cqqwz.cn

================================================================================
来源：http://gqn.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://ykj.xuetiantiany.cn

================================================================================
来源：http://ads.xziqi.cn

[M01] 读取命令行参数
来源：http://kpl.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://nsb.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://vwe.tanke756.top

JS:   process.argv.slice(2)
来源：http://fzd.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://xle.hammf.cn

Java: args 数组（main 方法参数）
来源：http://qpc.yangfankeji.com

Go:   os.Args[1:]
来源：http://tlr.cqqwz.cn

Ruby: ARGV
来源：http://atq.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://tug.zhixingplan.top

[M02] 读取环境变量
来源：http://ndw.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://mwe.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xsf.bbcook.cn

JS:   process.env.HOME
来源：http://ptj.shangyingyoupin.top

TS:   process.env.HOME
来源：http://erj.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://efs.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vat.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://bkz.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://thr.jqgfzy.top

[M03] 执行外部命令
来源：http://lnp.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nbf.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vmp.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nkl.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iuv.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://plr.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://epw.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ncb.fktsv.cn

C#:   Process.Start("ls", "-l");
来源：http://jjx.daria6918.cn

[M04] 获取当前工作目录
来源：http://ehh.shangyingyoupin.top

Py:   os.getcwd()
来源：http://ota.52xcode.cn

PHP:  getcwd();
来源：http://vmm.bjfxy.top

JS:   process.cwd()
来源：http://cuj.gaohongyu789.top

TS:   process.cwd()
来源：http://tch.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://sil.xziqi.cn

Go:   os.Getwd()
来源：http://uvc.ppjwa.cn

Ruby: Dir.pwd
来源：http://unr.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://hpa.snrcjt.cn

[M05] 设置退出码
来源：http://siy.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://tps.feifeiyinyue.top

PHP:  exit(1);
来源：http://mpz.hammf.cn

JS:   process.exit(1)
来源：http://ypb.fehbvm.com

TS:   process.exit(1)
来源：http://rpy.tian-w.cn

Java: System.exit(1)
来源：http://iro.hcnkem.com

Go:   os.Exit(1)
来源：http://mgw.fzhhl.top

Ruby: exit 1
来源：http://msh.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vec.cashguo.top

[M06] 向标准错误输出
来源：http://lav.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://omz.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cwi.daxiang520.top

JS:   console.error("err")
来源：http://yey.ppjwa.cn

TS:   console.error("err")
来源：http://jrp.sjlbkw.cn

Java: System.err.println("err")
来源：http://cdy.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://brm.fzhhl.top

Ruby: warn "err"
来源：http://bsv.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://khk.aizwys.cn

[M07] 判断是否为主入口
来源：http://qyc.316326.xyz

Py:   if __name__ == "__main__":
来源：http://iar.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yii.ywan-chungtsiang.top

JS:   require.main === module
来源：http://guo.zhoulong.xyz

TS:   require.main === module
来源：http://uqn.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://gpe.xingfuxueyuan.xyz

Go:   func main()
来源：http://rkg.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvr.xylfe.cn

C#:   static void Main(string[] args)
来源：http://sqg.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://djf.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://hfx.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://xfx.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://nxj.fzhhl.top

TS:   process.platform;  process.version
来源：http://okt.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zyj.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://ccz.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://clw.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://aer.zhongyouzk.top

================================================================================
来源：http://kux.fzhhl.top

N. 数据结构与算法
来源：http://kkz.cdnleiting.top

================================================================================
来源：http://ehq.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://eee.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://lzw.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hya.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iin.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llw.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://gov.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://gzg.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://dyj.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://uvj.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://xie.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://bfs.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sxh.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ckk.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aik.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjy.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://cuk.snrcjt.cn

Ruby: arr.sort
来源：http://bxx.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jlc.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://xcn.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ogv.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://nkf.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rfu.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unx.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rtd.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://llm.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tww.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://qvo.hnqzz.top

[N04] 斐波那契数列
来源：http://ygv.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qzg.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hxo.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vns.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djm.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wcj.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ajx.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kqk.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rcw.tian-w.cn

[N05] 最大公约数
来源：http://sgm.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://ova.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kvz.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://don.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qab.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pkv.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bhr.svipenyu.cn

Ruby: a.gcd(b)
来源：http://ali.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bar.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://nth.dashuyun.cn

Py:   s == s[::-1]
来源：http://kfx.yuxming.cn

PHP:  $s === strrev($s);
来源：http://ziu.c1oappe.top

JS:   s === [...s].reverse().join("")
来源：http://jqp.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://rnt.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sbp.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://pry.pycfn.com

Ruby: s == s.reverse
来源：http://vky.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gbt.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://sjt.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jtx.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lmb.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lgc.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://foz.gzhubu.top

Java: // 手写 HashMap
来源：http://eda.wangdashe.top

Go:   // 手写 map[int]int
来源：http://svt.yj202588.top

Ruby: // 手写 Hash
来源：http://isc.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://ptc.sufxvd.cn

[N08] 生成全排列
来源：http://pzc.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://dcc.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://ygl.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://gkc.yj20258888.top

TS:   // 手写回溯递归
来源：http://kze.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://fgp.aibaodan.cn

Go:   // 手写回溯递归
来源：http://sag.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://xag.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://cka.guannengcc.top

[N09] 栈与队列
来源：http://uba.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tva.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vpt.hnxiangtu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkx.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oxt.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xcz.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://adz.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bse.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://keq.bbcook.cn

[N10] 链表节点定义
来源：http://vza.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qin.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nmx.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bja.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://slm.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://hty.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://hxq.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mlg.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fxc.bbcook.cn

[N11] 二叉树中序遍历
来源：http://jms.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sbv.wangdashe.top

PHP:  // 手写递归函数
来源：http://fzw.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://amf.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjs.xziqi.cn

Java: // 手写递归
来源：http://hco.meibo888.top

Go:   // 手写递归
来源：http://tfe.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://veo.hywenlv.cn

C#:   // 手写递归
来源：http://bhz.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://orf.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cny.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bzw.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwk.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://acx.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kft.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vwa.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nsr.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jmb.jqgufenzy.top


<!-- 参考信息 -->