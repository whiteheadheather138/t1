代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wzh.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ouy.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vyo.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fnq.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iwu.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://rkp.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mtp.dianchejie.cn

[K05] 深拷贝对象
来源：http://afu.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://slh.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://dks.zycfv.cn

JS:   structuredClone(obj)
来源：http://vie.andypj.xyz

TS:   structuredClone(obj)
来源：http://bhi.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qyw.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pcq.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qwc.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ght.yongpay.top

[K06] 解析 URL 查询串
来源：http://fcv.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qms.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xkq.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pwf.hnqzz.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://znm.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kdl.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sck.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ugh.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vin.zhixingplan.top

[K07] 进制转换
来源：http://wyv.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yio.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lam.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tlg.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bcf.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pzo.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cyh.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mfz.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ouc.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://eij.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://lzr.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dpd.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://oef.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://vkw.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bdd.smart0.xyz

Go:   encoding/gob
来源：http://tiz.sweek.top

Ruby: Marshal.dump(obj)
来源：http://hyi.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hnk.hfpthk.cn

================================================================================
来源：http://rxm.gotoacloud.top

L. 网络请求
来源：http://wdg.hongshengwenyu.top

================================================================================
来源：http://jbw.hcnkem.com

[L01] 发送 GET 请求
来源：http://dxm.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qld.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pfk.tarul.cn

JS:   await fetch(url)
来源：http://lpn.gaohongyu789.top

TS:   await fetch(url)
来源：http://ffd.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dbn.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://jtz.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://occ.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dql.zdqjudy.top

[L02] 发送 POST JSON
来源：http://gfn.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yqu.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://chg.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsk.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bdo.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kxr.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cfc.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zso.gaohongyu789.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://amv.tian-w.cn

[L03] 设置自定义请求头
来源：http://qnb.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqo.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cnu.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bub.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyf.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ynt.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zii.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vgx.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wos.jianghu66.top

[L04] 设置超时
来源：http://qoi.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://dnl.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ddd.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fby.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kfx.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bcj.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fxu.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cvc.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aol.shuidangran.top

[L05] 上传文件（multipart）
来源：http://egl.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eqr.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvy.dianchejie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gjh.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dzc.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://som.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://htd.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://znj.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://top.wangdashe.top

[L06] 解析响应为 JSON
来源：http://hbm.chenlongwang.top

Py:   resp.json()
来源：http://wma.guannengcc.top

PHP:  json_decode($body, true);
来源：http://vpb.aizwys.cn

JS:   await resp.json()
来源：http://qlm.ybcxt.top

TS:   await resp.json()
来源：http://rrg.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bui.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ndv.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://uyi.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ehk.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://icv.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jsn.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vxk.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://tlc.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://ppo.jyoumei.cn

Java: resp.statusCode()
来源：http://tlt.jqgfzy.top

Go:   resp.StatusCode
来源：http://odh.tian-w.cn

Ruby: resp.code.to_i
来源：http://iyq.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://bhh.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://ard.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yvy.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://qyb.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kov.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eyg.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://stq.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xnl.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ekc.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yjp.sufxvd.cn

================================================================================
来源：http://ifc.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://qpj.fengsongda.top

================================================================================
来源：http://poa.yj202588.top

[M01] 读取命令行参数
来源：http://ruw.cdnleiting.top

Py:   sys.argv[1:]
来源：http://xhe.birdmap.top

PHP:  $argv;  $argc;
来源：http://grw.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://bpd.hammf.cn

TS:   process.argv.slice(2)
来源：http://kbk.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://hiw.zdbjq.cn

Go:   os.Args[1:]
来源：http://aoc.yangfankeji.com

Ruby: ARGV
来源：http://hld.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://ahm.0kj1m.cn

[M02] 读取环境变量
来源：http://zqz.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://vgp.smart0.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ooo.xuanzx.com

JS:   process.env.HOME
来源：http://rqz.nanxinkj.top

TS:   process.env.HOME
来源：http://aug.zdbjq.cn

Java: System.getenv("HOME")
来源：http://rjy.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oxg.jianghu66.top

Ruby: ENV["HOME"]
来源：http://wxo.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gwj.yuanzhike.top

[M03] 执行外部命令
来源：http://xnn.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ora.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fdx.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zdz.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bqs.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ygc.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lva.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://dxs.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://qgk.jiagoushi.top

[M04] 获取当前工作目录
来源：http://ylj.guannengcc.top

Py:   os.getcwd()
来源：http://xvm.sysykeji.top

PHP:  getcwd();
来源：http://pvr.c1oappe.top

JS:   process.cwd()
来源：http://aio.9152youxi.cn

TS:   process.cwd()
来源：http://ybm.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://bzc.ctjpmb.com

Go:   os.Getwd()
来源：http://vhg.zhijiandao.cn

Ruby: Dir.pwd
来源：http://fak.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ehi.hysaishi.cn

[M05] 设置退出码
来源：http://zpc.tianlin.xyz

Py:   sys.exit(1)
来源：http://aiz.pycfn.com

PHP:  exit(1);
来源：http://bun.shangyingyoupin.top

JS:   process.exit(1)
来源：http://bkn.jqgufenzy.top

TS:   process.exit(1)
来源：http://dtd.cucudq.cn

Java: System.exit(1)
来源：http://les.yanxiufei.cn

Go:   os.Exit(1)
来源：http://cva.cucudq.cn

Ruby: exit 1
来源：http://dik.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iix.zdqjudy.top

[M06] 向标准错误输出
来源：http://zwp.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://zkc.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://exh.ctjpmb.com

JS:   console.error("err")
来源：http://zhz.c1oappe.top

TS:   console.error("err")
来源：http://gfj.yuanzhike.top

Java: System.err.println("err")
来源：http://eiz.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uwz.jinqigfzy.top

Ruby: warn "err"
来源：http://gxl.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://azx.yj20258.top

[M07] 判断是否为主入口
来源：http://ygi.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://hxy.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jyo.shuidangran.top

JS:   require.main === module
来源：http://bre.shanyushiyangkeji.top

TS:   require.main === module
来源：http://cer.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://bms.hnqzz.top

Go:   func main()
来源：http://upa.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mjh.redwolf501.top

C#:   static void Main(string[] args)
来源：http://ebx.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://lfq.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://lel.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://ova.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://iig.yuxming.cn

TS:   process.platform;  process.version
来源：http://jlu.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cbr.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rfy.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ybb.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pfj.tarul.cn

================================================================================
来源：http://nzr.shuidangran.top

N. 数据结构与算法
来源：http://hoa.jyoumei.cn

================================================================================
来源：http://yno.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://wvn.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://phm.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eca.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkc.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zzz.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://wnb.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://xno.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://efl.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://cce.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://jlh.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://pfo.xylfe.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogs.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mhh.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dod.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kar.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://mih.redwolf501.top

Ruby: arr.sort
来源：http://cbi.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://akd.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://abl.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fbu.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://ipm.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lja.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nth.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rmt.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ntf.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fwt.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wlt.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://eet.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yyw.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tjf.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jxi.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkf.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xzr.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://esq.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://apx.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ril.kuanghao11.cn

[N05] 最大公约数
来源：http://bdg.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://bov.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://opl.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jus.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cuu.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwh.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vhl.yuxming.cn

Ruby: a.gcd(b)
来源：http://nwx.xziqi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gjx.aizwys.cn

[N06] 判断回文字符串
来源：http://tpe.jqgufenzy.top

Py:   s == s[::-1]
来源：http://vwd.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://iiz.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://ymj.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://mfk.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://krm.sweek.top

Go:   // 双指针从两端比较
来源：http://dsq.tianlin.xyz

Ruby: s == s.reverse
来源：http://lek.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vae.yj202588.top

[N07] 两数之和（返回下标）
来源：http://hjq.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezu.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hxk.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mmv.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://qlw.ivvv.top

Java: // 手写 HashMap
来源：http://ljn.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://owk.tian-w.cn

Ruby: // 手写 Hash
来源：http://sgu.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sfh.jqgfzy.top

[N08] 生成全排列
来源：http://zwn.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://nat.gzhubu.top

PHP:  // 手写递归交换
来源：http://cqh.316326.xyz

JS:   // 手写回溯递归
来源：http://iwj.zycfv.cn

TS:   // 手写回溯递归
来源：http://riz.iojbl.cn

Java: // 手写回溯递归
来源：http://egf.zhixingplan.top

Go:   // 手写回溯递归
来源：http://gwy.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://quk.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://nbu.yuxming.cn

[N09] 栈与队列
来源：http://hvg.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lew.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wjs.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bjn.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fge.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vps.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vsg.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jsr.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nxq.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://myu.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qae.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cib.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pkg.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lcz.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://ugz.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zvw.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://wpc.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rni.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://duc.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nie.cheryme.top

PHP:  // 手写递归函数
来源：http://erk.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fhg.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffs.zhaomingkeji.xyz

Java: // 手写递归
来源：http://azj.zdbjq.cn

Go:   // 手写递归
来源：http://qhq.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://reo.feifeiyinyue.top

C#:   // 手写递归
来源：http://ezn.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ufp.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bms.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sof.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gjo.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://plw.zhongyouzk.top


<!-- 参考信息 -->