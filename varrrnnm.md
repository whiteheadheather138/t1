代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://uej.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ryd.zhengqikj.top

[K04] 读取 JSON 文件
来源：http://nxi.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wvl.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dud.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fwi.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://olg.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nze.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sva.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vrk.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://huk.sysykeji.top

[K05] 深拷贝对象
来源：http://nmm.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://fwv.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://oia.yj20258888.top

JS:   structuredClone(obj)
来源：http://rip.xinyue.icu

TS:   structuredClone(obj)
来源：http://jrv.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zpv.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bld.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://viy.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xpw.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://oiu.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aag.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xyz.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pfc.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzk.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lzd.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lza.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zet.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tgb.cheryme.top

[K07] 进制转换
来源：http://nbj.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ijk.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tvt.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qff.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oui.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fdj.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cul.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yhx.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vke.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://cva.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://ygw.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nhq.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://lcw.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://sql.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lgl.uphjek.com

Go:   encoding/gob
来源：http://ftp.zhongyouzk.top

Ruby: Marshal.dump(obj)
来源：http://qoi.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oce.hysaishi.cn

================================================================================
来源：http://cfk.ppjwa.cn

L. 网络请求
来源：http://mhp.wangshuangyany.cn

================================================================================
来源：http://mrv.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://sqx.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qzp.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rsa.xinyue.icu

JS:   await fetch(url)
来源：http://jsf.yfazqb.com

TS:   await fetch(url)
来源：http://nth.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dfd.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://bap.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://cru.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xrx.andypj.xyz

[L02] 发送 POST JSON
来源：http://xpw.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://pko.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://znk.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dog.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://shx.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://djj.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dbd.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rxh.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://brv.ctjpmb.com

[L03] 设置自定义请求头
来源：http://lku.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xcw.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xbv.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynr.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://umc.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hzm.tanke756.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://atd.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bqj.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zqh.jiagoushi.top

[L04] 设置超时
来源：http://jxl.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://waq.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hpz.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rxl.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tnq.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dqp.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nss.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ori.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rdn.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://lfp.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vca.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vhi.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fxt.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jio.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ydc.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cau.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oju.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rzg.tianlin.xyz

[L06] 解析响应为 JSON
来源：http://xql.yangfankeji.com

Py:   resp.json()
来源：http://eyr.fehbvm.com

PHP:  json_decode($body, true);
来源：http://xav.zhoulong.xyz

JS:   await resp.json()
来源：http://fvg.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://pir.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dzu.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvf.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://sfw.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://trg.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://akp.aizwys.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jqx.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://byr.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://dfc.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://dal.yangfankeji.com

Java: resp.statusCode()
来源：http://grp.52xcode.cn

Go:   resp.StatusCode
来源：http://lli.xinyue.icu

Ruby: resp.code.to_i
来源：http://kzn.cashguo.top

C#:   (int)resp.StatusCode
来源：http://anf.hesvh.cn

[L08] 并发请求多个地址
来源：http://phh.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yjq.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://vpt.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzu.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogu.mhx1999.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qwe.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://isf.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uic.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://buj.aibaodan.cn

================================================================================
来源：http://wyd.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://hqq.yanxiufei.cn

================================================================================
来源：http://rok.uphjek.com

[M01] 读取命令行参数
来源：http://fsm.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://mrh.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://oca.meibo888.top

JS:   process.argv.slice(2)
来源：http://xxy.c1oappe.top

TS:   process.argv.slice(2)
来源：http://wsv.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://teb.jinqigfzy.top

Go:   os.Args[1:]
来源：http://vnj.hysaishi.cn

Ruby: ARGV
来源：http://puf.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://yxd.yj20258888.top

[M02] 读取环境变量
来源：http://vla.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://wjr.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ute.nanxuanxn.top

JS:   process.env.HOME
来源：http://idm.hammf.cn

TS:   process.env.HOME
来源：http://eza.xziqi.cn

Java: System.getenv("HOME")
来源：http://luy.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gam.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://afo.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dnu.zhixingplan.top

[M03] 执行外部命令
来源：http://kbj.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nyl.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bte.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kub.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://xcf.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rol.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://why.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://dmf.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://rzv.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://hyg.snrcjt.cn

Py:   os.getcwd()
来源：http://xcg.jqgfzy.top

PHP:  getcwd();
来源：http://dgk.iojbl.cn

JS:   process.cwd()
来源：http://vlr.zhengqikj.top

TS:   process.cwd()
来源：http://mwj.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://zqt.yj20258.top

Go:   os.Getwd()
来源：http://glu.dashuyun.cn

Ruby: Dir.pwd
来源：http://vou.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://ryz.gotoacloud.top

[M05] 设置退出码
来源：http://qwu.tarul.cn

Py:   sys.exit(1)
来源：http://yly.yongpay.top

PHP:  exit(1);
来源：http://psf.fktsv.cn

JS:   process.exit(1)
来源：http://awf.jqgfzy.top

TS:   process.exit(1)
来源：http://krp.cheryme.top

Java: System.exit(1)
来源：http://cks.zhoulong.xyz

Go:   os.Exit(1)
来源：http://sly.cdnleiting.top

Ruby: exit 1
来源：http://jre.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ins.hnxiangtu.top

[M06] 向标准错误输出
来源：http://tnw.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://ijy.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xtt.yuxming.cn

JS:   console.error("err")
来源：http://nec.uphjek.com

TS:   console.error("err")
来源：http://hwn.jinqigufen.top

Java: System.err.println("err")
来源：http://vsb.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ytx.hfpthk.cn

Ruby: warn "err"
来源：http://vcs.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://ioq.chenlongwang.top

[M07] 判断是否为主入口
来源：http://mth.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://bca.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vhl.tianlin.xyz

JS:   require.main === module
来源：http://jlm.nanxuanxn.top

TS:   require.main === module
来源：http://iet.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://ltf.316326.xyz

Go:   func main()
来源：http://gqr.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://myv.aizwys.cn

C#:   static void Main(string[] args)
来源：http://iia.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://pan.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://yqn.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://teg.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://voe.52xcode.cn

TS:   process.platform;  process.version
来源：http://mtb.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mhx.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lvt.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gpz.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mgc.yongpay.top

================================================================================
来源：http://pxp.zycfv.cn

N. 数据结构与算法
来源：http://qpr.cheryme.top

================================================================================
来源：http://tjw.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://uil.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://trt.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kcu.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uye.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yeb.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://kej.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://thl.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://drg.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://vtu.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://dza.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://cio.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tji.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://epm.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xbq.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvz.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://cwf.gotoacloud.top

Ruby: arr.sort
来源：http://cqg.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://gar.havefunace.top

[N03] 快速排序（分治示例）
来源：http://dmx.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hds.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://ltr.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chu.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nhj.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hae.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cja.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://enw.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jii.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://ouc.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zyo.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ugv.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qep.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oox.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nii.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xdx.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cbf.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pfc.sysykeji.top

[N05] 最大公约数
来源：http://kmr.pycfn.com

Py:   math.gcd(a, b)
来源：http://sre.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nxr.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://opv.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbj.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jea.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wzq.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://bqy.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://spg.yfazqb.com

[N06] 判断回文字符串
来源：http://wjt.hnqzz.top

Py:   s == s[::-1]
来源：http://alu.andypj.xyz

PHP:  $s === strrev($s);
来源：http://cnj.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://nqi.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://tyj.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://occ.xylfe.cn

Go:   // 双指针从两端比较
来源：http://bgi.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://rzn.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ckv.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://iwe.guowangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fnm.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://swr.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sxr.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://khn.jlsjyb.cn

Java: // 手写 HashMap
来源：http://vyi.hammf.cn

Go:   // 手写 map[int]int
来源：http://oda.andypj.xyz

Ruby: // 手写 Hash
来源：http://ypl.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://axj.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://fqc.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://eti.yj202588.top

PHP:  // 手写递归交换
来源：http://gvz.tian-w.cn

JS:   // 手写回溯递归
来源：http://lnm.havefunace.top

TS:   // 手写回溯递归
来源：http://eqe.daria6918.cn

Java: // 手写回溯递归
来源：http://aph.fzhhl.top

Go:   // 手写回溯递归
来源：http://hhw.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://ldb.52xcode.cn

C#:   // 手写回溯递归
来源：http://hke.tianlin.xyz

[N09] 栈与队列
来源：http://abw.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gon.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://txr.epnwcf.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ixt.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kkh.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pit.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mbf.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rcw.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vkp.kuanghao11.cn

[N10] 链表节点定义
来源：http://pux.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tha.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://soo.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jfb.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yqe.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://rfp.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://hkp.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vtj.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://blp.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://kfa.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lwm.hywenlv.cn

PHP:  // 手写递归函数
来源：http://iwh.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzv.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ker.tianlin.xyz

Java: // 手写递归
来源：http://sow.hnxiangtu.top

Go:   // 手写递归
来源：http://yqo.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wmz.hesvh.cn

C#:   // 手写递归
来源：http://dyj.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://isq.hywenlv.cn


<!-- 参考信息 -->