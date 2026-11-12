代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rtv.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hbe.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://icx.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://utj.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fvr.yj20258888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vtz.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fer.nanxuanxn.top

[K05] 深拷贝对象
来源：http://lbd.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://bln.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://mkq.yongpay.top

JS:   structuredClone(obj)
来源：http://bql.c1oappe.top

TS:   structuredClone(obj)
来源：http://yis.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bwh.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ilp.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://woz.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vnd.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://ujk.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iro.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://puq.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ema.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ket.cashguo.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvh.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wjt.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwi.bbcook.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jmf.pycfn.com

[K07] 进制转换
来源：http://ipf.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yrv.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bqq.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cgs.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tso.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cqw.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hpd.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mik.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hff.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://mts.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://zmu.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://olm.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://uad.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://noz.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vrx.birdmap.top

Go:   encoding/gob
来源：http://wok.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://tfb.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tjj.ybcxt.top

================================================================================
来源：http://jbd.hysaishi.cn

L. 网络请求
来源：http://kfd.guowangkeji.top

================================================================================
来源：http://nep.xuanzx.com

[L01] 发送 GET 请求
来源：http://vqp.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wxy.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vex.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://pjl.jqgufenzy.top

TS:   await fetch(url)
来源：http://bhm.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qbf.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://pnm.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ben.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lrd.tian-w.cn

[L02] 发送 POST JSON
来源：http://den.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://wwq.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gtx.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kia.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahb.feifeiyinyue.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vqy.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lzb.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://trm.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ads.ybcxt.top

[L03] 设置自定义请求头
来源：http://cnh.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pik.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://egh.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://abi.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lmx.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nfz.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vqq.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oob.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uiv.chenjidiqi.icu

[L04] 设置超时
来源：http://rwz.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://xee.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://div.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fbx.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cyh.ybcxt.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ldw.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kim.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ynm.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qgz.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://gvt.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dbd.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hmw.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwt.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wby.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mnt.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vqm.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xdl.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uzg.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://wpv.redwolf501.top

Py:   resp.json()
来源：http://jpz.tarul.cn

PHP:  json_decode($body, true);
来源：http://xkl.fanxiaobao.xyz

JS:   await resp.json()
来源：http://kya.sxryk.cn

TS:   await resp.json()
来源：http://csk.yongpay.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jsv.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://goh.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://bui.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fek.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://azb.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pqq.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sxl.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://ddw.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://muo.redwolf501.top

Java: resp.statusCode()
来源：http://ixb.yonumen.top

Go:   resp.StatusCode
来源：http://ubz.chenzaomai.com

Ruby: resp.code.to_i
来源：http://mrl.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://mtm.316326.xyz

[L08] 并发请求多个地址
来源：http://pao.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://svb.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://oki.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ycu.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzx.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vda.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hre.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttb.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xdd.xuanzx.com

================================================================================
来源：http://xvb.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://npb.chenzaomai.com

================================================================================
来源：http://zua.ydzc1.top

[M01] 读取命令行参数
来源：http://kgs.pycfn.com

Py:   sys.argv[1:]
来源：http://stl.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://urj.jianghu66.top

JS:   process.argv.slice(2)
来源：http://oqc.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://kir.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://ahq.fehbvm.com

Go:   os.Args[1:]
来源：http://ofi.vehdjk.com

Ruby: ARGV
来源：http://fre.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://zpn.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://guv.havefunace.top

Py:   os.environ.get("HOME")
来源：http://bop.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sup.bjfxy.top

JS:   process.env.HOME
来源：http://iiy.gogol.net.cn

TS:   process.env.HOME
来源：http://jnk.52xcode.cn

Java: System.getenv("HOME")
来源：http://eos.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jna.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://nnd.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eoa.daria6918.cn

[M03] 执行外部命令
来源：http://zxq.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzc.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mwe.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jkj.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cud.fengsongda.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vgf.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cuj.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qhn.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://xfr.52xcode.cn

[M04] 获取当前工作目录
来源：http://abg.ppjwa.cn

Py:   os.getcwd()
来源：http://bka.hfpthk.cn

PHP:  getcwd();
来源：http://vjm.birdmap.top

JS:   process.cwd()
来源：http://azr.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://qkm.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://tvd.fengsongda.top

Go:   os.Getwd()
来源：http://ahd.aizwys.cn

Ruby: Dir.pwd
来源：http://nih.redwolf501.top

C#:   Directory.GetCurrentDirectory()
来源：http://wvh.sjlbkw.cn

[M05] 设置退出码
来源：http://sja.jianghu66.top

Py:   sys.exit(1)
来源：http://vng.dianchejie.cn

PHP:  exit(1);
来源：http://dpz.guowangkeji.top

JS:   process.exit(1)
来源：http://yll.xuetiantiany.cn

TS:   process.exit(1)
来源：http://bkm.yj202588.top

Java: System.exit(1)
来源：http://fnm.bjfxy.top

Go:   os.Exit(1)
来源：http://jke.jinghuilouyu.cn

Ruby: exit 1
来源：http://hrz.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hrh.aizwys.cn

[M06] 向标准错误输出
来源：http://mee.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://dup.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://nar.aizwys.cn

JS:   console.error("err")
来源：http://lza.yj20258888.top

TS:   console.error("err")
来源：http://uju.yueranfly.top

Java: System.err.println("err")
来源：http://mov.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hov.haohaochexian.top

Ruby: warn "err"
来源：http://ztd.jianghu66.top

C#:   Console.Error.WriteLine("err")
来源：http://qkw.smart0.xyz

[M07] 判断是否为主入口
来源：http://npo.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://bab.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://avi.guannengcc.top

JS:   require.main === module
来源：http://mrq.yfazqb.com

TS:   require.main === module
来源：http://ydj.cqqwz.cn

Java: public static void main(String[] args)
来源：http://qbz.fengsongda.top

Go:   func main()
来源：http://ngg.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://itf.vehdjk.com

C#:   static void Main(string[] args)
来源：http://exm.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://koo.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://cbd.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://xnj.mhx1999.top

JS:   process.platform;  process.version
来源：http://wxh.ivvv.top

TS:   process.platform;  process.version
来源：http://ijn.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yym.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xou.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://atu.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uqp.cucudq.cn

================================================================================
来源：http://eqc.iojbl.cn

N. 数据结构与算法
来源：http://eoc.cdnleiting.top

================================================================================
来源：http://uac.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://bzj.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ywl.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gjh.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpi.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qwr.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://iyk.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://yog.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ccj.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://liz.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://dxh.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://wuq.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://emq.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxa.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rpo.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjq.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://aoc.ctjpmb.com

Ruby: arr.sort
来源：http://rbc.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gsv.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://aah.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lcf.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://cdc.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fgb.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcp.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xkg.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kem.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tvu.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://mmo.andypj.xyz

[N04] 斐波那契数列
来源：http://acf.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wyk.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://exx.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tki.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmq.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rsc.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bca.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://msf.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tut.yj202588.top

[N05] 最大公约数
来源：http://gcz.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://ddp.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://spb.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlg.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bfc.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dql.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gdr.aizwys.cn

Ruby: a.gcd(b)
来源：http://xva.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zkv.9152youxi.cn

[N06] 判断回文字符串
来源：http://xfd.kuanghao11.cn

Py:   s == s[::-1]
来源：http://ouv.mhx1999.top

PHP:  $s === strrev($s);
来源：http://osv.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://spr.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://jqi.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yls.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://qjp.hysaishi.cn

Ruby: s == s.reverse
来源：http://gyz.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lpw.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://jrt.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ygr.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jph.daria6918.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uoi.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://qvd.zhongyouzk.top

Java: // 手写 HashMap
来源：http://pbc.c1oappe.top

Go:   // 手写 map[int]int
来源：http://iyh.svipenyu.cn

Ruby: // 手写 Hash
来源：http://jdc.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://fbq.epnwcf.com

[N08] 生成全排列
来源：http://ktm.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://zlo.pycfn.com

PHP:  // 手写递归交换
来源：http://whp.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://suc.zhengqikj.top

TS:   // 手写回溯递归
来源：http://aml.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://fyw.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://sld.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://imy.guannengcc.top

C#:   // 手写回溯递归
来源：http://mii.sxryk.cn

[N09] 栈与队列
来源：http://gdc.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gtt.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nal.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jtl.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqa.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://buu.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xog.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kgt.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qma.sjlbkw.cn

[N10] 链表节点定义
来源：http://mfr.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://izg.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://buv.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://omm.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zdn.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://enc.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://sly.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eue.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nqj.redwolf501.top

[N11] 二叉树中序遍历
来源：http://rtb.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gtx.svipenyu.cn

PHP:  // 手写递归函数
来源：http://qhm.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tne.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://evh.zycfv.cn

Java: // 手写递归
来源：http://tcj.ivvv.top

Go:   // 手写递归
来源：http://joc.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ltj.kuanghao11.cn

C#:   // 手写递归
来源：http://hfo.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ssp.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zaf.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vzz.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybn.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mss.fehbvm.com


<!-- 参考信息 -->