代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jyx.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://snp.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqd.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kiy.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kir.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rbb.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wxd.jiagoushi.top

[K05] 深拷贝对象
来源：http://bes.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://luu.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://apy.yj20258.top

JS:   structuredClone(obj)
来源：http://xix.yvedp.cn

TS:   structuredClone(obj)
来源：http://eru.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://esb.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cyf.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rps.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fse.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://fyx.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yyg.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tbh.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcz.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jrf.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hya.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://cdg.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aht.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jdd.pengpengdd.cyou

[K07] 进制转换
来源：http://whe.epnwcf.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cpp.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xrl.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oif.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shs.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ktp.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fbl.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lrr.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rgn.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://hbl.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://uzm.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fui.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://njm.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://cld.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pyx.nanxinkj.top

Go:   encoding/gob
来源：http://cps.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://avk.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hjh.gotoacloud.top

================================================================================
来源：http://uma.yj202588.top

L. 网络请求
来源：http://uqz.jqgfzy.top

================================================================================
来源：http://rmm.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://fvg.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hjv.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xzg.hysaishi.cn

JS:   await fetch(url)
来源：http://jdi.birdmap.top

TS:   await fetch(url)
来源：http://aib.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zit.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://guj.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mzx.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rci.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://wdh.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://vlm.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://twv.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vls.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bnu.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zxj.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qzb.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hiu.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yhv.tian-w.cn

[L03] 设置自定义请求头
来源：http://iyl.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://afb.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qjn.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lcv.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gsq.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ell.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nqc.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cdl.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qyc.dashuyun.cn

[L04] 设置超时
来源：http://umt.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://dux.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aih.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rim.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztj.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zmd.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wgs.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fpr.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rou.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://hjr.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bky.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rrj.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dve.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ijp.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fst.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bki.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ysg.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzh.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://kad.shangyingyoupin.top

Py:   resp.json()
来源：http://myk.pycfn.com

PHP:  json_decode($body, true);
来源：http://inn.fktsv.cn

JS:   await resp.json()
来源：http://tyr.zdqjudy.top

TS:   await resp.json()
来源：http://fke.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nwj.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dky.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://cld.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ewn.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://tub.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ldw.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tml.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://ura.yj202588.top

TS:   resp.ok;  resp.status
来源：http://lio.wangdashe.top

Java: resp.statusCode()
来源：http://mix.jinqigfzy.top

Go:   resp.StatusCode
来源：http://qis.vehdjk.com

Ruby: resp.code.to_i
来源：http://hgj.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://jwf.cashguo.top

[L08] 并发请求多个地址
来源：http://tut.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tgx.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://kik.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jsp.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxa.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkv.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kef.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cxl.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qjw.andypj.xyz

================================================================================
来源：http://nbv.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://kip.chenjidiqi.icu

================================================================================
来源：http://ukg.chenlongwang.top

[M01] 读取命令行参数
来源：http://owg.xinyue.icu

Py:   sys.argv[1:]
来源：http://ljq.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://rup.fzhhl.top

JS:   process.argv.slice(2)
来源：http://kha.daria6918.cn

TS:   process.argv.slice(2)
来源：http://obu.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://bsm.jlsjyb.cn

Go:   os.Args[1:]
来源：http://kuj.xuetiantiany.cn

Ruby: ARGV
来源：http://glw.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://fyq.316326.xyz

[M02] 读取环境变量
来源：http://yzg.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://bno.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vax.tianlin.xyz

JS:   process.env.HOME
来源：http://vyp.sweek.top

TS:   process.env.HOME
来源：http://tce.hysaishi.cn

Java: System.getenv("HOME")
来源：http://nxi.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vzs.xylfe.cn

Ruby: ENV["HOME"]
来源：http://fqp.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xtj.gaohongyu789.top

[M03] 执行外部命令
来源：http://ljh.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uyt.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xhb.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zgn.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://npw.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mpu.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://sic.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fmi.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://isr.hesvh.cn

[M04] 获取当前工作目录
来源：http://rzg.havefunace.top

Py:   os.getcwd()
来源：http://ipt.hfpthk.cn

PHP:  getcwd();
来源：http://dwq.0kj1m.cn

JS:   process.cwd()
来源：http://lwc.vehdjk.com

TS:   process.cwd()
来源：http://mti.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://udk.yj20258888.top

Go:   os.Getwd()
来源：http://rxe.xinyue.icu

Ruby: Dir.pwd
来源：http://bgx.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://kgm.gaohongyu789.top

[M05] 设置退出码
来源：http://tjx.zhoulong.xyz

Py:   sys.exit(1)
来源：http://vqh.tian-w.cn

PHP:  exit(1);
来源：http://xmm.0kj1m.cn

JS:   process.exit(1)
来源：http://xum.hongshengwenyu.top

TS:   process.exit(1)
来源：http://qab.ppjwa.cn

Java: System.exit(1)
来源：http://dzs.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://bvw.cashguo.top

Ruby: exit 1
来源：http://ngi.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nol.cqqwz.cn

[M06] 向标准错误输出
来源：http://fpf.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://mvm.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wzt.tarul.cn

JS:   console.error("err")
来源：http://yzc.hesvh.cn

TS:   console.error("err")
来源：http://wgt.jiagoushi.top

Java: System.err.println("err")
来源：http://ckt.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zwf.jinqigfzy.top

Ruby: warn "err"
来源：http://gfn.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://nqp.yonumen.top

[M07] 判断是否为主入口
来源：http://fix.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://xba.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lmg.jinghuilouyu.cn

JS:   require.main === module
来源：http://dxt.jianghu66.top

TS:   require.main === module
来源：http://vpl.haohaochexian.top

Java: public static void main(String[] args)
来源：http://dql.zycfv.cn

Go:   func main()
来源：http://duz.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rts.yongpay.top

C#:   static void Main(string[] args)
来源：http://vmf.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://lug.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://wjg.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://zqy.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://dbo.nanxinkj.top

TS:   process.platform;  process.version
来源：http://akh.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://srz.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://swj.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iyd.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gen.dianchejie.cn

================================================================================
来源：http://nwi.ybcxt.top

N. 数据结构与算法
来源：http://fml.cucudq.cn

================================================================================
来源：http://hmh.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://ipl.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dkc.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rti.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qnc.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://stt.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://kof.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ezi.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://myj.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlf.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://cos.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://tbq.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eot.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vfq.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fpp.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qav.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://kvm.birdmap.top

Ruby: arr.sort
来源：http://dxd.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fot.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://bas.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bjg.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://cnm.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qop.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tsu.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uhb.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://djh.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ovw.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://bkt.xinyue.icu

[N04] 斐波那契数列
来源：http://lzd.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xix.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xum.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://huz.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gtw.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://alx.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gbx.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uoc.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xiy.yuanzhike.top

[N05] 最大公约数
来源：http://yex.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://vfn.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bcm.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://saq.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://toz.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://exa.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekw.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://ome.yj20258.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cqs.sxryk.cn

[N06] 判断回文字符串
来源：http://oof.daria6918.cn

Py:   s == s[::-1]
来源：http://tro.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://wyx.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://osz.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://tpm.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fds.316326.xyz

Go:   // 双指针从两端比较
来源：http://pso.kuanghao11.cn

Ruby: s == s.reverse
来源：http://efe.bjfxy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pez.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://pvk.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mrw.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ppe.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://urt.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://sxe.bjfxy.top

Java: // 手写 HashMap
来源：http://tsr.fzhhl.top

Go:   // 手写 map[int]int
来源：http://tgi.cheryme.top

Ruby: // 手写 Hash
来源：http://omg.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://lef.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://tcx.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://dti.hfpthk.cn

PHP:  // 手写递归交换
来源：http://bkc.havefunace.top

JS:   // 手写回溯递归
来源：http://gvh.iojbl.cn

TS:   // 手写回溯递归
来源：http://jbe.nanxuanxn.top

Java: // 手写回溯递归
来源：http://kig.jqgfzy.top

Go:   // 手写回溯递归
来源：http://etj.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://ejv.guowangkeji.top

C#:   // 手写回溯递归
来源：http://okb.c1oappe.top

[N09] 栈与队列
来源：http://mim.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mob.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tbx.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ars.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kbf.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xsl.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpw.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://apd.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hmk.yvedp.cn

[N10] 链表节点定义
来源：http://ypv.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://osw.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ezi.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tfn.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kun.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://rea.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://vpl.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zpo.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rfw.ybcxt.top

[N11] 二叉树中序遍历
来源：http://qqu.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xic.gotoacloud.top

PHP:  // 手写递归函数
来源：http://qrh.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayq.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://skg.yuanzhike.top

Java: // 手写递归
来源：http://nmc.uphjek.com

Go:   // 手写递归
来源：http://kda.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dnv.hammf.cn

C#:   // 手写递归
来源：http://oih.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://znf.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nni.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tlo.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrx.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://syy.fanxiaobao.xyz


<!-- 参考信息 -->