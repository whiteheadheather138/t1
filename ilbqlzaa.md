代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fpy.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://quq.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://olk.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dha.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wvq.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xmd.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uim.yangfankeji.com

[K05] 深拷贝对象
来源：http://qzc.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://vrs.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://ssh.nwbrower.top

JS:   structuredClone(obj)
来源：http://zah.yfazqb.com

TS:   structuredClone(obj)
来源：http://hlt.zhijiandao.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nys.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dln.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://btx.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pxe.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://zmp.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xfb.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gon.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkr.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fho.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://put.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ghn.dashuyun.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bzo.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pet.fehbvm.com

[K07] 进制转换
来源：http://mhx.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qny.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://moy.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lhe.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://snt.jianghu66.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rrl.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rnf.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ovj.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oar.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://nra.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://vlp.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pfl.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jtt.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://cnh.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jvt.jqgfzy.top

Go:   encoding/gob
来源：http://shm.sweek.top

Ruby: Marshal.dump(obj)
来源：http://dhd.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://grf.zhiwuduotai.top

================================================================================
来源：http://stg.yfazqb.com

L. 网络请求
来源：http://ltn.yuxming.cn

================================================================================
来源：http://rhv.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://gdl.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fie.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gyf.kuanghao11.cn

JS:   await fetch(url)
来源：http://mom.svipenyu.cn

TS:   await fetch(url)
来源：http://lws.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lbx.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://qih.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://okb.smart0.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://seq.jianghu66.top

[L02] 发送 POST JSON
来源：http://cqh.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://shj.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jhi.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sxw.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnk.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ddo.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dpf.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lvc.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pte.zdqjudy.top

[L03] 设置自定义请求头
来源：http://puj.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uxd.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://agf.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyy.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osm.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jor.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cxg.vehdjk.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zlp.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vyv.guowangkeji.top

[L04] 设置超时
来源：http://xdw.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://pag.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bgz.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywx.zhixingplan.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myw.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://plk.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zlx.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://umj.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://skh.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://xng.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zvr.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hnf.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gfm.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ucn.yuanzhike.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bug.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pym.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uvx.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kus.yueranfly.top

[L06] 解析响应为 JSON
来源：http://lxe.fktsv.cn

Py:   resp.json()
来源：http://xiq.zycfv.cn

PHP:  json_decode($body, true);
来源：http://zwi.hnqzz.top

JS:   await resp.json()
来源：http://szf.meibo888.top

TS:   await resp.json()
来源：http://bfm.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yeh.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dgf.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://lzf.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yot.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://axj.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwd.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qmh.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://iyb.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://vll.yvedp.cn

Java: resp.statusCode()
来源：http://kcr.yonumen.top

Go:   resp.StatusCode
来源：http://zbk.hongshengwenyu.top

Ruby: resp.code.to_i
来源：http://xur.tarul.cn

C#:   (int)resp.StatusCode
来源：http://lqw.cheryme.top

[L08] 并发请求多个地址
来源：http://ygq.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://chb.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://rtx.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmg.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qhb.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hza.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dun.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ram.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zqo.zhijiandao.cn

================================================================================
来源：http://jrq.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://czv.zhongyouzk.top

================================================================================
来源：http://hgr.jqgufenzy.top

[M01] 读取命令行参数
来源：http://xca.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://elt.bjfxy.top

PHP:  $argv;  $argc;
来源：http://vxi.c1oappe.top

JS:   process.argv.slice(2)
来源：http://qct.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://pmk.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://cpf.9152youxi.cn

Go:   os.Args[1:]
来源：http://ubt.haohaochexian.top

Ruby: ARGV
来源：http://oix.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://eqw.tarul.cn

[M02] 读取环境变量
来源：http://bzi.yonumen.top

Py:   os.environ.get("HOME")
来源：http://rxr.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iuc.feifeiyinyue.top

JS:   process.env.HOME
来源：http://mrx.tarul.cn

TS:   process.env.HOME
来源：http://onq.c1oappe.top

Java: System.getenv("HOME")
来源：http://ezf.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vxo.c1oappe.top

Ruby: ENV["HOME"]
来源：http://bya.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rzn.xuetiantiany.cn

[M03] 执行外部命令
来源：http://tyq.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xfs.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gky.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zex.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cib.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cdu.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rkm.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://wrj.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://ici.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://wlm.zhoulong.xyz

Py:   os.getcwd()
来源：http://cqh.yuxming.cn

PHP:  getcwd();
来源：http://rhl.gzhubu.top

JS:   process.cwd()
来源：http://hid.hysaishi.cn

TS:   process.cwd()
来源：http://nno.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://jkt.svipenyu.cn

Go:   os.Getwd()
来源：http://cic.xuanzx.com

Ruby: Dir.pwd
来源：http://nuf.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://dkk.sjlbkw.cn

[M05] 设置退出码
来源：http://ilw.tianlin.xyz

Py:   sys.exit(1)
来源：http://jyj.ydjk.org.cn

PHP:  exit(1);
来源：http://auo.nwbrower.top

JS:   process.exit(1)
来源：http://zux.yangfankeji.com

TS:   process.exit(1)
来源：http://zqg.ppjwa.cn

Java: System.exit(1)
来源：http://gda.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://rlw.sysykeji.top

Ruby: exit 1
来源：http://lvi.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mzo.yuxming.cn

[M06] 向标准错误输出
来源：http://yab.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://fxj.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yyy.daxiang520.top

JS:   console.error("err")
来源：http://iap.cheryme.top

TS:   console.error("err")
来源：http://jwh.bbcook.cn

Java: System.err.println("err")
来源：http://wty.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uuv.cqqwz.cn

Ruby: warn "err"
来源：http://gnw.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://wwv.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://ijz.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://ekw.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fca.havefunace.top

JS:   require.main === module
来源：http://mvt.shuidangran.top

TS:   require.main === module
来源：http://qdc.guannengcc.top

Java: public static void main(String[] args)
来源：http://mlo.shzxlz.cn

Go:   func main()
来源：http://kqu.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://abu.gaohongyu789.top

C#:   static void Main(string[] args)
来源：http://zjp.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://wib.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://phf.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://eig.jiagoushi.top

JS:   process.platform;  process.version
来源：http://clu.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://oqc.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jvr.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fzu.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uiw.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yea.yj20258888.top

================================================================================
来源：http://zqc.bbcook.cn

N. 数据结构与算法
来源：http://mqr.hnqzz.top

================================================================================
来源：http://uei.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://nqi.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://itz.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hdm.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bkn.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azn.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kno.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://hdp.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://drq.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://imn.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://glk.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://ocr.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://odn.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jdz.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://dwu.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uft.tanke756.top

Go:   slices.Sort(arr)
来源：http://jzg.shanyushiyangtech.top

Ruby: arr.sort
来源：http://ffm.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zsu.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://hag.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gqa.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://vsk.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://edk.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wqr.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fgx.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzi.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xoi.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://pvv.c1oappe.top

[N04] 斐波那契数列
来源：http://aki.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://olv.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://brp.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ifq.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sqp.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xcp.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qpb.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rmi.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xox.gotoacloud.top

[N05] 最大公约数
来源：http://fbs.sxryk.cn

Py:   math.gcd(a, b)
来源：http://zdr.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xmo.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rjv.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pca.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://frm.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dum.316326.xyz

Ruby: a.gcd(b)
来源：http://jqg.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bnt.cucudq.cn

[N06] 判断回文字符串
来源：http://emc.smart0.xyz

Py:   s == s[::-1]
来源：http://juo.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://nox.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://qjs.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://xbz.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://twh.yonumen.top

Go:   // 双指针从两端比较
来源：http://kqs.quarkkingdee.top

Ruby: s == s.reverse
来源：http://gpe.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfv.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://dhj.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://odb.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlj.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mjb.chenzaomai.com

TS:   // 手写 Map<string, number>
来源：http://kfl.aibaodan.cn

Java: // 手写 HashMap
来源：http://exl.yueranfly.top

Go:   // 手写 map[int]int
来源：http://gcx.chenzaomai.com

Ruby: // 手写 Hash
来源：http://hus.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gwy.ppjwa.cn

[N08] 生成全排列
来源：http://zbd.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://qht.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://orm.52xcode.cn

JS:   // 手写回溯递归
来源：http://joa.uphjek.com

TS:   // 手写回溯递归
来源：http://yok.haohaochexian.top

Java: // 手写回溯递归
来源：http://ygt.fengsongda.top

Go:   // 手写回溯递归
来源：http://jto.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://aff.cqqwz.cn

C#:   // 手写回溯递归
来源：http://kcj.xylfe.cn

[N09] 栈与队列
来源：http://wwr.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lac.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://obl.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nlv.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqz.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://crt.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vvg.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fnd.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lai.dashuyun.cn

[N10] 链表节点定义
来源：http://cly.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dsb.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oox.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lam.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fho.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://pvz.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://srl.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://umj.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rwi.havefunace.top

[N11] 二叉树中序遍历
来源：http://cmy.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hzy.yangfankeji.com

PHP:  // 手写递归函数
来源：http://xuf.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txl.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gke.bjfxy.top

Java: // 手写递归
来源：http://yrv.xziqi.cn

Go:   // 手写递归
来源：http://qqy.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ypm.xuanzx.com

C#:   // 手写递归
来源：http://ibq.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bdl.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tqf.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fpf.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqx.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iht.fehbvm.com


<!-- 参考信息 -->