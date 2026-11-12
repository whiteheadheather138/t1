代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eeh.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oxk.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rpf.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lfo.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lia.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kxw.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vyo.tanke756.top

[K05] 深拷贝对象
来源：http://phl.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://wrd.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://ree.bbcook.cn

JS:   structuredClone(obj)
来源：http://ycw.cheryme.top

TS:   structuredClone(obj)
来源：http://tlk.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xaw.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cqo.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vie.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qol.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://pyr.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nif.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwz.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uxg.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://huh.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rwj.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hrp.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xbi.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://axu.ivvv.top

[K07] 进制转换
来源：http://xle.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fcl.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wbl.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lzx.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sij.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tzi.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ppj.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kmw.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cnk.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://wjb.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://dth.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tgy.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://upo.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://noc.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ycr.9152youxi.cn

Go:   encoding/gob
来源：http://pdi.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://nfi.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xek.cheryme.top

================================================================================
来源：http://mrm.meibo888.top

L. 网络请求
来源：http://vwb.ctjpmb.com

================================================================================
来源：http://ura.wangdashe.top

[L01] 发送 GET 请求
来源：http://cfx.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://num.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rje.cdnleiting.top

JS:   await fetch(url)
来源：http://xre.svipenyu.cn

TS:   await fetch(url)
来源：http://oqc.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ahv.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://bnr.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yej.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aom.xziqi.cn

[L02] 发送 POST JSON
来源：http://ueh.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://pvt.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://slf.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfv.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mxa.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wek.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eiy.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cxu.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://irx.xinyue.icu

[L03] 设置自定义请求头
来源：http://foi.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oah.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jmz.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpt.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ydy.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ocl.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ebk.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qzt.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tbj.sufxvd.cn

[L04] 设置超时
来源：http://onh.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://ifm.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xbs.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wgq.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ndp.yvedp.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://adp.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkg.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fba.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qox.tanke756.top

[L05] 上传文件（multipart）
来源：http://xuj.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pbr.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ori.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bln.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jsr.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qmt.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wis.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zad.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pti.yj202588.top

[L06] 解析响应为 JSON
来源：http://uzj.daxiang520.top

Py:   resp.json()
来源：http://lvv.ivvv.top

PHP:  json_decode($body, true);
来源：http://nxw.tian-w.cn

JS:   await resp.json()
来源：http://aoa.fktsv.cn

TS:   await resp.json()
来源：http://spg.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://axd.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nwz.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://ksr.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rav.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://skb.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dug.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yoc.yj20258.top

JS:   resp.ok;  resp.status
来源：http://yxw.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://jbj.yuxming.cn

Java: resp.statusCode()
来源：http://efs.wangshuangyany.cn

Go:   resp.StatusCode
来源：http://vpc.daxiang520.top

Ruby: resp.code.to_i
来源：http://zyb.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://xhh.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://vtw.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hjf.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://wfj.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://syu.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baj.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hoe.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hyr.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ess.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://swb.redwolf501.top

================================================================================
来源：http://axm.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://vjh.zhaomingkeji.xyz

================================================================================
来源：http://ghu.yongpay.top

[M01] 读取命令行参数
来源：http://ixp.52xcode.cn

Py:   sys.argv[1:]
来源：http://uky.bjfxy.top

PHP:  $argv;  $argc;
来源：http://hvp.pycfn.com

JS:   process.argv.slice(2)
来源：http://wxv.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://agb.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://abv.ivvv.top

Go:   os.Args[1:]
来源：http://wjo.redwolf501.top

Ruby: ARGV
来源：http://bdc.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://ysk.tarul.cn

[M02] 读取环境变量
来源：http://fmb.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://rhw.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dpc.svipenyu.cn

JS:   process.env.HOME
来源：http://gib.xziqi.cn

TS:   process.env.HOME
来源：http://pip.iojbl.cn

Java: System.getenv("HOME")
来源：http://slb.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zjj.bbcook.cn

Ruby: ENV["HOME"]
来源：http://nuh.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjk.yj20258888.top

[M03] 执行外部命令
来源：http://ypg.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://suk.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://avu.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jvq.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ouq.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nfw.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kwx.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://pmq.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://zfk.yvedp.cn

[M04] 获取当前工作目录
来源：http://nht.tarul.cn

Py:   os.getcwd()
来源：http://hvu.zhongyouzk.top

PHP:  getcwd();
来源：http://mmu.uphjek.com

JS:   process.cwd()
来源：http://ovh.fanxiaobao.xyz

TS:   process.cwd()
来源：http://tru.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://kwz.yonumen.top

Go:   os.Getwd()
来源：http://ree.xuanzx.com

Ruby: Dir.pwd
来源：http://dhp.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tnc.kuanghao11.cn

[M05] 设置退出码
来源：http://oku.yj20258888.top

Py:   sys.exit(1)
来源：http://lwf.yuanzhike.top

PHP:  exit(1);
来源：http://dkl.zhijiandao.cn

JS:   process.exit(1)
来源：http://smc.yuxming.cn

TS:   process.exit(1)
来源：http://zjm.chenjidiqi.icu

Java: System.exit(1)
来源：http://twz.fzhhl.top

Go:   os.Exit(1)
来源：http://yjy.hysaishi.cn

Ruby: exit 1
来源：http://xfe.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lfy.cashguo.top

[M06] 向标准错误输出
来源：http://gzf.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://ead.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mll.hnqzz.top

JS:   console.error("err")
来源：http://lkt.aizwys.cn

TS:   console.error("err")
来源：http://irk.fehbvm.com

Java: System.err.println("err")
来源：http://gik.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cds.jinqigufen.top

Ruby: warn "err"
来源：http://bvm.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://ibm.iojbl.cn

[M07] 判断是否为主入口
来源：http://wac.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://cok.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://knz.haohaochexian.top

JS:   require.main === module
来源：http://uro.yj202588.top

TS:   require.main === module
来源：http://tjf.vehdjk.com

Java: public static void main(String[] args)
来源：http://xyk.uphjek.com

Go:   func main()
来源：http://bhh.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ukj.sweek.top

C#:   static void Main(string[] args)
来源：http://uzd.pycfn.com

[M08] 获取系统与运行时信息
来源：http://ank.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://bab.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://dhm.0kj1m.cn

JS:   process.platform;  process.version
来源：http://kku.jinqigufen.top

TS:   process.platform;  process.version
来源：http://apk.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ttv.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dqj.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hpg.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oad.zdqjudy.top

================================================================================
来源：http://lsb.0kj1m.cn

N. 数据结构与算法
来源：http://zrx.0kj1m.cn

================================================================================
来源：http://mul.yongpay.top

[N01] 二分查找（有序数组）
来源：http://knt.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://jsv.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rnz.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://phx.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tip.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://goi.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://tze.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rvp.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hll.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://pul.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://xrn.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nng.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://elo.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://muq.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cnz.mhx1999.top

Go:   slices.Sort(arr)
来源：http://jan.52xcode.cn

Ruby: arr.sort
来源：http://zlx.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybd.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://qfn.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvq.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://qjs.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxg.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ryq.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwp.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fxh.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jkt.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://vua.gzhubu.top

[N04] 斐波那契数列
来源：http://vbk.nanxuanxn.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tua.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uku.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qkt.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qlk.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hgo.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jwf.ctjpmb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tik.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lgd.yangfankeji.com

[N05] 最大公约数
来源：http://ois.ydzc1.top

Py:   math.gcd(a, b)
来源：http://omh.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qpp.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ruy.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcv.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://umh.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jra.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://vbb.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ljk.meibo888.top

[N06] 判断回文字符串
来源：http://npg.zhengqikj.top

Py:   s == s[::-1]
来源：http://xfu.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://iez.jqgufenzy.top

JS:   s === [...s].reverse().join("")
来源：http://bgo.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://tnu.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lro.yongpay.top

Go:   // 双指针从两端比较
来源：http://gsw.tianlin.xyz

Ruby: s == s.reverse
来源：http://fxt.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://giq.0kj1m.cn

[N07] 两数之和（返回下标）
来源：http://usc.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jwi.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ito.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uqc.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://bfe.316326.xyz

Java: // 手写 HashMap
来源：http://tpw.meibo888.top

Go:   // 手写 map[int]int
来源：http://ejh.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://xcq.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://nbp.ydzc1.top

[N08] 生成全排列
来源：http://rxr.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://uqz.yuanzhike.top

PHP:  // 手写递归交换
来源：http://wrr.haohaochexian.top

JS:   // 手写回溯递归
来源：http://cmx.yangfankeji.com

TS:   // 手写回溯递归
来源：http://lms.zhijiandao.cn

Java: // 手写回溯递归
来源：http://uvc.xziqi.cn

Go:   // 手写回溯递归
来源：http://eoc.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://pts.dashuyun.cn

C#:   // 手写回溯递归
来源：http://ffu.hysaishi.cn

[N09] 栈与队列
来源：http://cjv.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lnk.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lwv.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://duu.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqm.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iic.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ums.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uxo.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pln.yvedp.cn

[N10] 链表节点定义
来源：http://gol.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nus.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rck.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://flp.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://apf.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://myd.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nub.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xdd.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mmt.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://gly.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fyb.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://dit.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nun.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hnx.sxryk.cn

Java: // 手写递归
来源：http://sed.tian-w.cn

Go:   // 手写递归
来源：http://pmv.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://onz.yanxiufei.cn

C#:   // 手写递归
来源：http://tfd.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rft.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hmf.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://shd.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rsn.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qui.jinqigufen.top


<!-- 参考信息 -->