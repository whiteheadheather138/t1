代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://afv.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nba.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gkt.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cew.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://thn.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ibo.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xnf.jinqigfzy.top

[K05] 深拷贝对象
来源：http://nfk.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://mqh.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://ehw.guannengcc.top

JS:   structuredClone(obj)
来源：http://zlg.daxiang520.top

TS:   structuredClone(obj)
来源：http://oll.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://izh.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yst.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://brr.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://its.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://gli.ivvv.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nkq.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://njd.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adf.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tcq.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zck.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufl.iojbl.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wjg.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tgp.redwolf501.top

[K07] 进制转换
来源：http://jla.jinqigufen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rgc.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mtc.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tcn.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lzu.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xev.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wbo.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qst.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://old.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://nln.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://ebj.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kpc.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://zdn.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://xxh.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cjc.yfazqb.com

Go:   encoding/gob
来源：http://lso.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://rsf.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xtu.shanyushiyangtech.top

================================================================================
来源：http://rxa.uphjek.com

L. 网络请求
来源：http://hye.fzhhl.top

================================================================================
来源：http://epy.andypj.xyz

[L01] 发送 GET 请求
来源：http://ajs.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://snj.sjlbkw.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kml.hongshengwenyu.top

JS:   await fetch(url)
来源：http://xxn.ybcxt.top

TS:   await fetch(url)
来源：http://zmw.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ngk.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://jcw.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bwa.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dlp.yangfankeji.com

[L02] 发送 POST JSON
来源：http://rkp.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://zvm.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gxm.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qwy.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgt.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ezs.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qfu.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wol.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kph.jqgfzy.top

[L03] 设置自定义请求头
来源：http://cck.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yqe.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xda.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flt.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dwe.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dgi.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cyq.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sjz.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pqu.fehbvm.com

[L04] 设置超时
来源：http://nar.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://pal.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://plp.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iaa.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://trg.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nnz.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwi.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jzn.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kfr.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://plz.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oyd.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jhi.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rvv.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kom.tarul.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rra.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ukc.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://org.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fvy.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://tta.zycfv.cn

Py:   resp.json()
来源：http://anm.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://avz.hnxiangtu.top

JS:   await resp.json()
来源：http://kpd.tianlin.xyz

TS:   await resp.json()
来源：http://trr.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://syl.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://top.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://qnf.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rxu.zdqjudy.top

[L07] 处理 HTTP 状态码
来源：http://fcw.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tlq.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svi.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://gup.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://mgc.havefunace.top

Java: resp.statusCode()
来源：http://hcg.zhijiandao.cn

Go:   resp.StatusCode
来源：http://wko.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://ylc.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://npp.52xcode.cn

[L08] 并发请求多个地址
来源：http://fdl.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://unu.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://uec.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sdh.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://htb.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mgx.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dyg.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ddg.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eve.jyoumei.cn

================================================================================
来源：http://hyb.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://bdp.dashuyun.cn

================================================================================
来源：http://coc.hnxiangtu.top

[M01] 读取命令行参数
来源：http://gho.yfazqb.com

Py:   sys.argv[1:]
来源：http://qgl.ivvv.top

PHP:  $argv;  $argc;
来源：http://gco.52xcode.cn

JS:   process.argv.slice(2)
来源：http://mzi.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://snu.wangdashe.top

Java: args 数组（main 方法参数）
来源：http://ydy.guowangkeji.top

Go:   os.Args[1:]
来源：http://yzs.jlsjyb.cn

Ruby: ARGV
来源：http://rmh.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://wsk.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://mtu.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://zgm.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qcd.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://ydp.bbcook.cn

TS:   process.env.HOME
来源：http://dhu.yonumen.top

Java: System.getenv("HOME")
来源：http://hoo.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gbq.pycfn.com

Ruby: ENV["HOME"]
来源：http://bxr.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xof.shuidangran.top

[M03] 执行外部命令
来源：http://jda.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uft.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gaa.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://whl.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rfh.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yeh.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://otb.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://joq.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://dmx.fengsongda.top

[M04] 获取当前工作目录
来源：http://xzz.tarul.cn

Py:   os.getcwd()
来源：http://ars.zdbjq.cn

PHP:  getcwd();
来源：http://qlj.fanxiaobao.xyz

JS:   process.cwd()
来源：http://vya.jqgfzy.top

TS:   process.cwd()
来源：http://dfa.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://stj.wangshuangyany.cn

Go:   os.Getwd()
来源：http://asl.wangdashe.top

Ruby: Dir.pwd
来源：http://pph.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://qyl.cashguo.top

[M05] 设置退出码
来源：http://tcm.andypj.xyz

Py:   sys.exit(1)
来源：http://jqo.bbcook.cn

PHP:  exit(1);
来源：http://axh.jqgufenzy.top

JS:   process.exit(1)
来源：http://fqr.guannengcc.top

TS:   process.exit(1)
来源：http://emk.bjfxy.top

Java: System.exit(1)
来源：http://mnh.c1oappe.top

Go:   os.Exit(1)
来源：http://zjt.fengsongda.top

Ruby: exit 1
来源：http://wee.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rgm.smart0.xyz

[M06] 向标准错误输出
来源：http://qnw.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://zbh.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gmi.zhengqikj.top

JS:   console.error("err")
来源：http://mwd.chenlongwang.top

TS:   console.error("err")
来源：http://rmf.c1oappe.top

Java: System.err.println("err")
来源：http://dxy.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kgo.vqdsnc.cn

Ruby: warn "err"
来源：http://xgp.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://xnv.haohaochexian.top

[M07] 判断是否为主入口
来源：http://hbj.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://fif.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ebb.cqqwz.cn

JS:   require.main === module
来源：http://qfo.quarkkingdee.top

TS:   require.main === module
来源：http://fev.smart0.xyz

Java: public static void main(String[] args)
来源：http://pzu.nanxuanxn.top

Go:   func main()
来源：http://opr.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cum.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://gkt.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://fbr.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://oye.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://cxc.yfazqb.com

JS:   process.platform;  process.version
来源：http://wdt.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://tce.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nhj.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsq.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hyf.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://juc.jqgufenzy.top

================================================================================
来源：http://yjf.uphjek.com

N. 数据结构与算法
来源：http://ljz.jlsjyb.cn

================================================================================
来源：http://aig.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://usq.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://mmm.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iso.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cmi.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zul.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://idl.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://okj.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wln.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pdo.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://hsj.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://dgj.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ncz.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ttl.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dac.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pvs.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://yuf.gogol.net.cn

Ruby: arr.sort
来源：http://uxa.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qve.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://wxp.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qri.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://erw.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vdg.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://buu.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gqp.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xzz.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hne.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jqc.hnqzz.top

[N04] 斐波那契数列
来源：http://pra.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ino.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eok.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygj.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tao.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gbr.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ssc.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kou.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://frv.quarkkingdee.top

[N05] 最大公约数
来源：http://ysf.nanxinkj.top

Py:   math.gcd(a, b)
来源：http://hmm.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cei.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iav.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pcx.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yde.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://plc.chenlongwang.top

Ruby: a.gcd(b)
来源：http://ean.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jim.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://rov.tian-w.cn

Py:   s == s[::-1]
来源：http://ywy.zycfv.cn

PHP:  $s === strrev($s);
来源：http://iwh.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://ypj.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://djf.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://faq.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://lxa.vqdsnc.cn

Ruby: s == s.reverse
来源：http://ehj.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nss.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://ejv.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fbo.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sdr.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://syh.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://ock.hcnkem.com

Java: // 手写 HashMap
来源：http://fdm.havefunace.top

Go:   // 手写 map[int]int
来源：http://ksz.gzhubu.top

Ruby: // 手写 Hash
来源：http://nlt.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://ooi.gzhubu.top

[N08] 生成全排列
来源：http://cfi.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://hfg.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://tqv.guannengcc.top

JS:   // 手写回溯递归
来源：http://vor.fzhhl.top

TS:   // 手写回溯递归
来源：http://yzb.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://lip.52xcode.cn

Go:   // 手写回溯递归
来源：http://opn.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://cuk.zhengqikj.top

C#:   // 手写回溯递归
来源：http://bbh.xinyue.icu

[N09] 栈与队列
来源：http://alj.jyoumei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kzw.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zio.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ovk.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gxc.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fuf.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pze.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tkw.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lee.ivvv.top

[N10] 链表节点定义
来源：http://ymz.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wgg.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ngb.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qzd.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qno.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://paw.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xbm.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://amr.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qee.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://eeo.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://azz.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ikc.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzr.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tly.daria6918.cn

Java: // 手写递归
来源：http://acp.ppjwa.cn

Go:   // 手写递归
来源：http://brm.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xxs.chenlongwang.top

C#:   // 手写递归
来源：http://jip.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sgr.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ypj.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gjd.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llv.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpk.pengpengdd.cyou


<!-- 参考信息 -->