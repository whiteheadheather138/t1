代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://zjo.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://soy.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://dpp.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ibw.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ctw.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tyy.9152youxi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goe.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qbh.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bvd.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vtr.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hmu.shuidangran.top

[K05] 深拷贝对象
来源：http://fjx.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://vcd.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://wzk.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://ggg.jiagoushi.top

TS:   structuredClone(obj)
来源：http://xbj.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cmi.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fps.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndw.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bvt.epnwcf.com

[K06] 解析 URL 查询串
来源：http://zba.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hky.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wmk.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vea.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbr.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qwd.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ufn.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zrf.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://isi.cheryme.top

[K07] 进制转换
来源：http://zhj.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wmz.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rne.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://isi.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmy.jqgufenzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ncc.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vil.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpf.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yfr.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://nuu.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://geh.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oni.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://fsi.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://hbe.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ftq.dashuyun.cn

Go:   encoding/gob
来源：http://btz.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://opg.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pdw.cheryme.top

================================================================================
来源：http://iht.aibaodan.cn

L. 网络请求
来源：http://qgb.shzxlz.cn

================================================================================
来源：http://kfz.hysaishi.cn

[L01] 发送 GET 请求
来源：http://gkl.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pzx.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uxx.quarkkingdee.top

JS:   await fetch(url)
来源：http://epr.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://uwz.shuidangran.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rab.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://sxl.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nyw.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ckx.chenlongwang.top

[L02] 发送 POST JSON
来源：http://szs.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bjm.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jbk.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ulq.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qcc.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ebz.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qaw.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kqp.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sie.jyoumei.cn

[L03] 设置自定义请求头
来源：http://wgf.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fwr.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cxd.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgb.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmz.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gzf.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dra.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pwq.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgm.jqgufenzy.top

[L04] 设置超时
来源：http://ftq.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://mbu.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aql.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxd.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://enp.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bar.zhongyouzk.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zou.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ybk.ydjk.org.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://opv.bjfxy.top

[L05] 上传文件（multipart）
来源：http://gax.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tnz.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iwi.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ttf.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://amx.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cwa.mhx1999.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hek.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vcl.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uci.yonumen.top

[L06] 解析响应为 JSON
来源：http://fyy.vehdjk.com

Py:   resp.json()
来源：http://lde.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://bvi.ctjpmb.com

JS:   await resp.json()
来源：http://pzx.jqgufenzy.top

TS:   await resp.json()
来源：http://ahc.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ziw.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qvv.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://hum.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vtr.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://bup.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://twg.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rai.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://qqr.c1oappe.top

TS:   resp.ok;  resp.status
来源：http://avj.zhijiandao.cn

Java: resp.statusCode()
来源：http://riv.ivvv.top

Go:   resp.StatusCode
来源：http://bug.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://pzm.xziqi.cn

C#:   (int)resp.StatusCode
来源：http://qis.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://zmb.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vyk.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://amt.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nhl.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://upv.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kzd.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rjr.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://azu.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ykq.fengsongda.top

================================================================================
来源：http://yzv.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://are.zycfv.cn

================================================================================
来源：http://ddf.gogol.net.cn

[M01] 读取命令行参数
来源：http://evs.bbcook.cn

Py:   sys.argv[1:]
来源：http://gxo.yvedp.cn

PHP:  $argv;  $argc;
来源：http://zvk.sweek.top

JS:   process.argv.slice(2)
来源：http://qnq.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://jil.tanke756.top

Java: args 数组（main 方法参数）
来源：http://kqh.tanke756.top

Go:   os.Args[1:]
来源：http://hmf.yj20258888.top

Ruby: ARGV
来源：http://ist.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://dep.hcnkem.com

[M02] 读取环境变量
来源：http://khp.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://wmb.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fhe.sxryk.cn

JS:   process.env.HOME
来源：http://tir.sysykeji.top

TS:   process.env.HOME
来源：http://wza.jqgfzy.top

Java: System.getenv("HOME")
来源：http://fpn.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://msh.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://xlx.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wuf.c1oappe.top

[M03] 执行外部命令
来源：http://uts.shanyushiyangtech.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ozn.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rcy.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lpu.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ekk.fzhhl.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uge.cheryme.top

Go:   exec.Command("ls", "-l").Output()
来源：http://suf.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://hxr.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://nie.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://pal.sweek.top

Py:   os.getcwd()
来源：http://fkw.yonumen.top

PHP:  getcwd();
来源：http://xlb.yanxiufei.cn

JS:   process.cwd()
来源：http://arn.gogol.net.cn

TS:   process.cwd()
来源：http://cay.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://uxd.meibo888.top

Go:   os.Getwd()
来源：http://nid.hcnkem.com

Ruby: Dir.pwd
来源：http://thn.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://bxe.guowangkeji.top

[M05] 设置退出码
来源：http://gns.havefunace.top

Py:   sys.exit(1)
来源：http://jcc.hongshengwenyu.top

PHP:  exit(1);
来源：http://amx.xziqi.cn

JS:   process.exit(1)
来源：http://azm.jqgfzy.top

TS:   process.exit(1)
来源：http://hjc.yfazqb.com

Java: System.exit(1)
来源：http://utm.tanke756.top

Go:   os.Exit(1)
来源：http://wow.jlsjyb.cn

Ruby: exit 1
来源：http://hgg.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yxw.svipenyu.cn

[M06] 向标准错误输出
来源：http://tla.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://rzh.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lpb.tarul.cn

JS:   console.error("err")
来源：http://uje.wangdashe.top

TS:   console.error("err")
来源：http://bhx.xuetiantiany.cn

Java: System.err.println("err")
来源：http://hdf.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qjg.gaohongyu789.top

Ruby: warn "err"
来源：http://ohu.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://fjy.mhx1999.top

[M07] 判断是否为主入口
来源：http://tuo.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://kmb.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnc.chenlongwang.top

JS:   require.main === module
来源：http://qcn.yj202588.top

TS:   require.main === module
来源：http://mfu.gogol.net.cn

Java: public static void main(String[] args)
来源：http://mqc.hywenlv.cn

Go:   func main()
来源：http://eyh.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mla.epnwcf.com

C#:   static void Main(string[] args)
来源：http://geh.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://sec.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://bxq.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://xdw.yfazqb.com

JS:   process.platform;  process.version
来源：http://eea.shzxlz.cn

TS:   process.platform;  process.version
来源：http://pzq.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qnr.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ixw.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bvc.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kyi.cheryme.top

================================================================================
来源：http://jrq.ybcxt.top

N. 数据结构与算法
来源：http://jfw.ybcxt.top

================================================================================
来源：http://awx.xingfuxueyuan.xyz

[N01] 二分查找（有序数组）
来源：http://ypr.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iof.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://svy.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dgn.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rmg.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://zpi.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://why.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://nmm.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nri.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://ddr.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://yfc.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cbv.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rba.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sxk.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ksq.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://tud.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://kna.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://upb.316326.xyz

[N03] 快速排序（分治示例）
来源：http://qsu.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bcd.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://fgr.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://csn.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddh.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aor.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bll.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lzb.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://fzv.hesvh.cn

[N04] 斐波那契数列
来源：http://dib.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hqu.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://djq.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rar.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybb.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://igm.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpk.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aqo.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lhg.haohaochexian.top

[N05] 最大公约数
来源：http://fjp.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://cpc.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zps.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxd.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npp.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yqb.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://srn.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://qup.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xen.jianghu66.top

[N06] 判断回文字符串
来源：http://rou.bbcook.cn

Py:   s == s[::-1]
来源：http://ihr.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://djl.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://dzj.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://wwe.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cko.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://uzn.ivvv.top

Ruby: s == s.reverse
来源：http://wjf.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://krh.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://glb.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://srn.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hye.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sbo.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://gfk.jyoumei.cn

Java: // 手写 HashMap
来源：http://xty.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://lqk.fehbvm.com

Ruby: // 手写 Hash
来源：http://npa.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://fjg.haohaochexian.top

[N08] 生成全排列
来源：http://vjm.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://sxc.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://vhl.nwbrower.top

JS:   // 手写回溯递归
来源：http://epg.aizwys.cn

TS:   // 手写回溯递归
来源：http://owg.sjlbkw.cn

Java: // 手写回溯递归
来源：http://wji.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://pdc.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://eqb.hcnkem.com

C#:   // 手写回溯递归
来源：http://rdv.hnqzz.top

[N09] 栈与队列
来源：http://gcl.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zjs.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wlg.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yfu.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pkx.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://akw.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://srf.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sfc.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aba.nanxinkj.top

[N10] 链表节点定义
来源：http://qno.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://krg.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qkx.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tvx.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hem.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://grf.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lvr.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zpm.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wao.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://cac.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xbq.gotoacloud.top

PHP:  // 手写递归函数
来源：http://iji.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://huv.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rgz.xuetiantiany.cn

Java: // 手写递归
来源：http://lig.aizwys.cn

Go:   // 手写递归
来源：http://hbf.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wdr.gaohongyu789.top

C#:   // 手写递归
来源：http://zeo.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gjq.fehbvm.com


<!-- 参考信息 -->