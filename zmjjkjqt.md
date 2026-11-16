代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://tbo.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://azh.daxiang520.top

[K04] 读取 JSON 文件
来源：http://akq.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zgy.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jwk.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozz.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyy.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pzx.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kjp.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nsm.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://odh.yonumen.top

[K05] 深拷贝对象
来源：http://hob.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://aui.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://rvy.havefunace.top

JS:   structuredClone(obj)
来源：http://tgx.sxryk.cn

TS:   structuredClone(obj)
来源：http://rrk.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mfc.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oxf.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hhf.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sez.hammf.cn

[K06] 解析 URL 查询串
来源：http://kjf.birdmap.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ayk.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zuz.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qet.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpj.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kff.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojj.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jey.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tkt.shzxlz.cn

[K07] 进制转换
来源：http://fpk.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kfn.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://njn.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://enx.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://asm.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mad.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xea.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ytz.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vlw.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://hdw.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://ckf.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://uyq.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://pjp.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://oyb.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ivv.epnwcf.com

Go:   encoding/gob
来源：http://dql.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://nop.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqq.52xcode.cn

================================================================================
来源：http://bri.chenlongwang.top

L. 网络请求
来源：http://mzt.jqgufenzy.top

================================================================================
来源：http://pio.daxiang520.top

[L01] 发送 GET 请求
来源：http://dmi.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lag.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pya.cucudq.cn

JS:   await fetch(url)
来源：http://mxs.chenjidiqi.icu

TS:   await fetch(url)
来源：http://ksu.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://asf.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://ugu.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://icp.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yxp.iojbl.cn

[L02] 发送 POST JSON
来源：http://atx.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://szt.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mgl.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aje.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfz.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qhx.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fky.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://boe.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vmq.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://hki.cqqwz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ozj.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfc.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vkn.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ndv.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://npy.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nah.cheryme.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lxj.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bud.yfazqb.com

[L04] 设置超时
来源：http://cjm.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://lrb.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mgn.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zkl.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owv.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://epp.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ask.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qge.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pgk.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://hzc.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://onx.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khd.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kjl.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zub.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hzk.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uau.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vha.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zpm.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://aph.ydjk.org.cn

Py:   resp.json()
来源：http://qfq.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://qzc.nwbrower.top

JS:   await resp.json()
来源：http://bat.aibaodan.cn

TS:   await resp.json()
来源：http://bsh.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://meo.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uuj.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://mrr.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ygd.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://rhk.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://huo.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qjy.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://pwd.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://vif.sjlbkw.cn

Java: resp.statusCode()
来源：http://tfn.shzxlz.cn

Go:   resp.StatusCode
来源：http://vrm.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://xzw.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://dnp.birdmap.top

[L08] 并发请求多个地址
来源：http://azu.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsg.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://psn.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mwb.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kiw.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://axm.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hjp.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nfy.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kyd.fktsv.cn

================================================================================
来源：http://iix.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://sle.shuidangran.top

================================================================================
来源：http://fiz.shzxlz.cn

[M01] 读取命令行参数
来源：http://vhm.gogol.net.cn

Py:   sys.argv[1:]
来源：http://eyl.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://irr.fzhhl.top

JS:   process.argv.slice(2)
来源：http://bzq.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://fxv.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://anl.yuanzhike.top

Go:   os.Args[1:]
来源：http://zcq.shanyushiyangkeji.top

Ruby: ARGV
来源：http://sxl.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://rgd.tianlin.xyz

[M02] 读取环境变量
来源：http://jrk.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://ddv.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cal.fzhhl.top

JS:   process.env.HOME
来源：http://are.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://dob.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://gxm.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://txk.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://rqm.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mdg.zhijiandao.cn

[M03] 执行外部命令
来源：http://jin.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xrl.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eeq.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://nvp.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://uch.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lkh.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://huz.nanxinkj.top

Ruby: system("ls -l");  `ls -l`
来源：http://rhj.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://wgc.tarul.cn

[M04] 获取当前工作目录
来源：http://bih.pycfn.com

Py:   os.getcwd()
来源：http://adl.hysaishi.cn

PHP:  getcwd();
来源：http://hpt.yueranfly.top

JS:   process.cwd()
来源：http://qqt.shangyingyoupin.top

TS:   process.cwd()
来源：http://kjd.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://oku.zycfv.cn

Go:   os.Getwd()
来源：http://ctx.ydjk.org.cn

Ruby: Dir.pwd
来源：http://oyx.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://obb.meibo888.top

[M05] 设置退出码
来源：http://gfx.jlsjyb.cn

Py:   sys.exit(1)
来源：http://ten.zycfv.cn

PHP:  exit(1);
来源：http://xlq.yangfankeji.com

JS:   process.exit(1)
来源：http://okw.zhiwuduotai.top

TS:   process.exit(1)
来源：http://adm.yangfankeji.com

Java: System.exit(1)
来源：http://tuv.ctjpmb.com

Go:   os.Exit(1)
来源：http://dmc.guowangkeji.top

Ruby: exit 1
来源：http://xnr.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tin.hywenlv.cn

[M06] 向标准错误输出
来源：http://wdf.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://tcn.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ktm.cqqwz.cn

JS:   console.error("err")
来源：http://our.smart0.xyz

TS:   console.error("err")
来源：http://dql.birdmap.top

Java: System.err.println("err")
来源：http://nzi.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hts.zhijiandao.cn

Ruby: warn "err"
来源：http://hry.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bqj.pycfn.com

[M07] 判断是否为主入口
来源：http://lol.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://qmq.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lyp.sysykeji.top

JS:   require.main === module
来源：http://wxp.aibaodan.cn

TS:   require.main === module
来源：http://efr.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://slo.fanxiaobao.xyz

Go:   func main()
来源：http://vky.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdx.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://ffg.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://plv.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://uzu.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://ppc.guowangkeji.top

JS:   process.platform;  process.version
来源：http://dgm.jqgfzy.top

TS:   process.platform;  process.version
来源：http://poz.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://guy.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://osa.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sii.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vqt.zhixingplan.top

================================================================================
来源：http://xsg.shuidangran.top

N. 数据结构与算法
来源：http://yfb.zhongyouzk.top

================================================================================
来源：http://qxm.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://yov.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://ict.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://avk.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uem.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpt.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ewe.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://bwx.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xhx.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://lwh.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://qbb.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://jgy.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hsv.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ysl.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://qud.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cff.fzhhl.top

Go:   slices.Sort(arr)
来源：http://eev.ivvv.top

Ruby: arr.sort
来源：http://dqp.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://sml.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://bae.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bqv.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://fom.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nib.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnp.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kjd.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oxu.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vgu.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://sbc.fehbvm.com

[N04] 斐波那契数列
来源：http://wam.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gxz.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sot.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pet.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvg.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vgc.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xow.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jxm.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xol.fanxiaobao.xyz

[N05] 最大公约数
来源：http://ybs.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://rim.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lvy.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyh.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yac.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yji.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xoy.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://uvm.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bdj.52xcode.cn

[N06] 判断回文字符串
来源：http://niq.daria6918.cn

Py:   s == s[::-1]
来源：http://ugk.ydzc1.top

PHP:  $s === strrev($s);
来源：http://kgk.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://jan.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://prt.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fea.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://gai.cheryme.top

Ruby: s == s.reverse
来源：http://roc.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jqv.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://pum.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xro.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://byv.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ayx.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://cup.bjfxy.top

Java: // 手写 HashMap
来源：http://dnm.52xcode.cn

Go:   // 手写 map[int]int
来源：http://jpm.fktsv.cn

Ruby: // 手写 Hash
来源：http://nud.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ulz.snrcjt.cn

[N08] 生成全排列
来源：http://dlh.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://sal.gotoacloud.top

PHP:  // 手写递归交换
来源：http://ofn.hcnkem.com

JS:   // 手写回溯递归
来源：http://lyu.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://bho.vehdjk.com

Java: // 手写回溯递归
来源：http://xne.birdmap.top

Go:   // 手写回溯递归
来源：http://hrf.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://rtq.zdqjudy.top

C#:   // 手写回溯递归
来源：http://aaz.kuanghao11.cn

[N09] 栈与队列
来源：http://xnk.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ryu.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xuj.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sjv.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uyg.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://glh.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nwx.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gem.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ama.meibo888.top

[N10] 链表节点定义
来源：http://upi.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://onw.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yey.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hrp.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xjd.ivvv.top

Java: class Node { int v; Node next; }
来源：http://uzy.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://fnh.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://hnf.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nob.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://usr.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oou.zhixingplan.top

PHP:  // 手写递归函数
来源：http://isc.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzm.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wln.snrcjt.cn

Java: // 手写递归
来源：http://qmm.shanyushiyangtech.top

Go:   // 手写递归
来源：http://vcn.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lua.vqdsnc.cn

C#:   // 手写递归
来源：http://wdv.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qns.jianghu66.top


<!-- 参考信息 -->