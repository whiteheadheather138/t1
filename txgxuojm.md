代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wxz.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://myr.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dqs.andypj.xyz

[K05] 深拷贝对象
来源：http://lgu.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://nqb.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://xkt.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://kij.ydzc1.top

TS:   structuredClone(obj)
来源：http://hmy.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://atc.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pvc.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hkv.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://utg.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://eaa.gzhubu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aqx.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fgp.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ivk.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://una.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xrq.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxe.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cxw.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iae.smart0.xyz

[K07] 进制转换
来源：http://aky.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tky.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://trb.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vse.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://adx.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://som.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://afl.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dxc.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://prk.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://sdd.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://ryj.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hws.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://wlz.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://kiy.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://stg.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://hma.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://uvv.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ift.yueranfly.top

================================================================================
来源：http://aug.fengsongda.top

L. 网络请求
来源：http://cre.quarkkingdee.top

================================================================================
来源：http://aes.smart0.xyz

[L01] 发送 GET 请求
来源：http://tfm.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kcd.zdbjq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cvw.fzhhl.top

JS:   await fetch(url)
来源：http://ibm.sjlbkw.cn

TS:   await fetch(url)
来源：http://fqa.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xjo.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://zmh.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ndb.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxd.shzxlz.cn

[L02] 发送 POST JSON
来源：http://opo.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cfu.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tdk.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://amd.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyo.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://czr.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ohr.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rgu.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jpn.zhengqikj.top

[L03] 设置自定义请求头
来源：http://inz.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aeb.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xwx.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ttd.jinghuilouyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pdo.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jre.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wcp.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wiz.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kkf.andypj.xyz

[L04] 设置超时
来源：http://xkc.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://ezu.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xsz.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tyz.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kme.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pxc.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xoq.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://muv.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jur.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://eaz.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ywf.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wav.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xly.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://axx.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iig.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lhr.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pzo.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sjq.meibo888.top

[L06] 解析响应为 JSON
来源：http://otd.hongshengwenyu.top

Py:   resp.json()
来源：http://taq.yfazqb.com

PHP:  json_decode($body, true);
来源：http://zdm.shuidangran.top

JS:   await resp.json()
来源：http://cxt.zhixingplan.top

TS:   await resp.json()
来源：http://dqa.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zkn.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bur.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://htx.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dbi.zhengqikj.top

[L07] 处理 HTTP 状态码
来源：http://nwv.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dpe.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gfy.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://yzr.shangyingyoupin.top

TS:   resp.ok;  resp.status
来源：http://jpi.0kj1m.cn

Java: resp.statusCode()
来源：http://wno.vehdjk.com

Go:   resp.StatusCode
来源：http://zrx.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://lox.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://pae.dianchejie.cn

[L08] 并发请求多个地址
来源：http://vyt.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jhx.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://yta.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yci.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkz.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xww.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://drv.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ban.jianghu66.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gkl.nanxuanxn.top

================================================================================
来源：http://bgk.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://kww.yfazqb.com

================================================================================
来源：http://esd.sjlbkw.cn

[M01] 读取命令行参数
来源：http://sgy.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://gfa.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://ocd.meibo888.top

JS:   process.argv.slice(2)
来源：http://bxb.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://vgo.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://dzm.fktsv.cn

Go:   os.Args[1:]
来源：http://ldg.jlsjyb.cn

Ruby: ARGV
来源：http://soc.hongshengwenyu.top

C#:   args 数组（Main 方法参数）
来源：http://oyc.yj20258888.top

[M02] 读取环境变量
来源：http://irz.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://soa.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kqt.yuxming.cn

JS:   process.env.HOME
来源：http://dhp.ctjpmb.com

TS:   process.env.HOME
来源：http://vkw.wangdashe.top

Java: System.getenv("HOME")
来源：http://wnp.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://apu.52xcode.cn

Ruby: ENV["HOME"]
来源：http://aji.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nek.hfpthk.cn

[M03] 执行外部命令
来源：http://qbb.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://srd.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nng.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://akq.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jvk.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cfh.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vmc.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://cmy.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://gan.yonumen.top

[M04] 获取当前工作目录
来源：http://mxu.sxryk.cn

Py:   os.getcwd()
来源：http://znz.jianghu66.top

PHP:  getcwd();
来源：http://xpa.hnxiangtu.top

JS:   process.cwd()
来源：http://ocy.zhoulong.xyz

TS:   process.cwd()
来源：http://tiv.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://rmr.tianlin.xyz

Go:   os.Getwd()
来源：http://wrb.xinyue.icu

Ruby: Dir.pwd
来源：http://usb.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://ait.xziqi.cn

[M05] 设置退出码
来源：http://jkh.316326.xyz

Py:   sys.exit(1)
来源：http://ygo.jqgfzy.top

PHP:  exit(1);
来源：http://mux.cashguo.top

JS:   process.exit(1)
来源：http://mfa.sjlbkw.cn

TS:   process.exit(1)
来源：http://bkt.ivvv.top

Java: System.exit(1)
来源：http://hbr.cqqwz.cn

Go:   os.Exit(1)
来源：http://pes.cheryme.top

Ruby: exit 1
来源：http://kut.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xhk.zdqjudy.top

[M06] 向标准错误输出
来源：http://zhi.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://esb.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://mfo.vqdsnc.cn

JS:   console.error("err")
来源：http://sex.jyoumei.cn

TS:   console.error("err")
来源：http://hsc.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://hnx.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mhw.ppjwa.cn

Ruby: warn "err"
来源：http://gkb.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://wvl.havefunace.top

[M07] 判断是否为主入口
来源：http://qql.chenjidiqi.icu

Py:   if __name__ == "__main__":
来源：http://lxa.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://clo.smart0.xyz

JS:   require.main === module
来源：http://esy.nanxuanxn.top

TS:   require.main === module
来源：http://plt.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://ick.chenzaomai.com

Go:   func main()
来源：http://gtt.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yzg.smart0.xyz

C#:   static void Main(string[] args)
来源：http://rtc.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://eic.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://ubh.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://noa.fktsv.cn

JS:   process.platform;  process.version
来源：http://fvh.epnwcf.com

TS:   process.platform;  process.version
来源：http://tzh.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pyg.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tbj.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://whz.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uht.ivvv.top

================================================================================
来源：http://ftd.sjlbkw.cn

N. 数据结构与算法
来源：http://ekc.ywan-chungtsiang.top

================================================================================
来源：http://mhr.yj20258.top

[N01] 二分查找（有序数组）
来源：http://zxr.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://ljn.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olm.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dqs.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwv.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oun.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://sta.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://muh.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://ojc.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://gny.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://yyj.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jai.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://apv.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kth.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qip.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://axb.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://uvf.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uuc.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://iuy.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gcp.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://qts.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://daz.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rcg.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://thq.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://guz.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qey.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://nrg.jinqigufen.top

[N04] 斐波那契数列
来源：http://wpl.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcv.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bbc.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pln.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://miu.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cwj.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vtd.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hba.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sxn.pycfn.com

[N05] 最大公约数
来源：http://vos.ivvv.top

Py:   math.gcd(a, b)
来源：http://utb.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yvq.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhl.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyn.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fwk.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ewg.tanke756.top

Ruby: a.gcd(b)
来源：http://erc.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tsk.andypj.xyz

[N06] 判断回文字符串
来源：http://dol.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://sty.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://iyf.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://iwi.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://uhk.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nar.cucudq.cn

Go:   // 双指针从两端比较
来源：http://ofk.jianghu66.top

Ruby: s == s.reverse
来源：http://gdl.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aoy.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://cyo.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xyw.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ipv.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sts.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://sux.guannengcc.top

Java: // 手写 HashMap
来源：http://icr.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://hdi.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://nbd.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://whb.cheryme.top

[N08] 生成全排列
来源：http://vju.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://rbd.tanke756.top

PHP:  // 手写递归交换
来源：http://dty.vehdjk.com

JS:   // 手写回溯递归
来源：http://vwi.jinqigufen.top

TS:   // 手写回溯递归
来源：http://lrj.sufxvd.cn

Java: // 手写回溯递归
来源：http://fgg.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://gbu.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://bvu.yongpay.top

C#:   // 手写回溯递归
来源：http://flg.fengsongda.top

[N09] 栈与队列
来源：http://enf.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://idk.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fvn.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gro.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qso.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oso.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ljl.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://atk.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kho.ydzc1.top

[N10] 链表节点定义
来源：http://khv.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iad.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://che.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bdo.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pqv.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://avw.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://yfg.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qbo.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xpc.wangdashe.top

[N11] 二叉树中序遍历
来源：http://jti.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://buk.svipenyu.cn

PHP:  // 手写递归函数
来源：http://tiw.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sup.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ryr.cqqwz.cn

Java: // 手写递归
来源：http://dxq.yangfankeji.com

Go:   // 手写递归
来源：http://wgp.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://srk.yvedp.cn

C#:   // 手写递归
来源：http://wat.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nea.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fhw.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fnh.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxy.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://con.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pmz.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lzd.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zdr.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dvb.316326.xyz


<!-- 参考信息 -->