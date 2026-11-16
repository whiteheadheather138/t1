代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://lyo.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uzl.ydzc1.top

[K04] 读取 JSON 文件
来源：http://wer.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zyv.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dgk.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aii.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qtt.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://unz.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bfy.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fkg.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://glc.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://koa.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://taf.sweek.top

PHP:  unserialize(serialize($obj));
来源：http://pzn.hfpthk.cn

JS:   structuredClone(obj)
来源：http://ulj.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://yxq.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://whk.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cug.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vcs.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vkf.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://hyk.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://whs.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://asj.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ryo.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cpt.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bfm.smart0.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://slw.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jrf.c1oappe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yvy.zdqjudy.top

[K07] 进制转换
来源：http://ywl.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://szl.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://paj.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pya.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fdy.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bzz.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hhp.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://icw.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dni.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://fgc.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://ypa.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yoi.redwolf501.top

JS:   v8.serialize(obj)        // Node
来源：http://zhz.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://pdp.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lmf.hfpthk.cn

Go:   encoding/gob
来源：http://tap.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://uch.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pms.dianchejie.cn

================================================================================
来源：http://jxu.tanke756.top

L. 网络请求
来源：http://vie.jinghuilouyu.cn

================================================================================
来源：http://eir.yonumen.top

[L01] 发送 GET 请求
来源：http://vqy.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qsi.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ylh.zycfv.cn

JS:   await fetch(url)
来源：http://pbd.hfpthk.cn

TS:   await fetch(url)
来源：http://sdq.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cpe.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://trq.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ncn.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eks.nanxinkj.top

[L02] 发送 POST JSON
来源：http://nxf.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://ugi.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://drp.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cga.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oal.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vwc.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oki.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aor.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rvh.smart0.xyz

[L03] 设置自定义请求头
来源：http://lmk.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cpe.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cqe.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vwh.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ghq.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lpr.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ctw.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdc.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://naz.52xcode.cn

[L04] 设置超时
来源：http://suk.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://irb.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jsq.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dnf.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xjf.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ohj.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://omf.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ylg.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://duv.yongpay.top

[L05] 上传文件（multipart）
来源：http://wlw.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dar.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://feb.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eem.smart0.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ndp.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://krh.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cyl.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xop.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zmn.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://bfx.sufxvd.cn

Py:   resp.json()
来源：http://zng.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://ffb.hfpthk.cn

JS:   await resp.json()
来源：http://pks.jqgufenzy.top

TS:   await resp.json()
来源：http://hku.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://icc.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mgw.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://lgr.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rcz.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://shl.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vum.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lzt.cheryme.top

JS:   resp.ok;  resp.status
来源：http://xxu.tanke756.top

TS:   resp.ok;  resp.status
来源：http://duj.bjfxy.top

Java: resp.statusCode()
来源：http://anh.iojbl.cn

Go:   resp.StatusCode
来源：http://vzj.ydzc1.top

Ruby: resp.code.to_i
来源：http://vjc.yongpay.top

C#:   (int)resp.StatusCode
来源：http://vlf.yuanzhike.top

[L08] 并发请求多个地址
来源：http://xxn.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zsb.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://son.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rpl.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://itv.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cxj.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gve.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://flg.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bfq.yuxming.cn

================================================================================
来源：http://myj.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://amv.bjfxy.top

================================================================================
来源：http://trg.mhx1999.top

[M01] 读取命令行参数
来源：http://mqj.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://kiw.yj20258.top

PHP:  $argv;  $argc;
来源：http://zgu.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://ssn.aizwys.cn

TS:   process.argv.slice(2)
来源：http://oon.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://htm.dianchejie.cn

Go:   os.Args[1:]
来源：http://saf.iojbl.cn

Ruby: ARGV
来源：http://gqb.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://mqi.gaohongyu789.top

[M02] 读取环境变量
来源：http://oup.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://bbb.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eta.jlsjyb.cn

JS:   process.env.HOME
来源：http://hyi.hcnkem.com

TS:   process.env.HOME
来源：http://keu.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://drs.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://csk.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://iig.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vcq.vqdsnc.cn

[M03] 执行外部命令
来源：http://icc.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qup.zhaomingkeji.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxq.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wco.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mdw.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nya.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ubk.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://nhx.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://soy.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://icn.feifeiyinyue.top

Py:   os.getcwd()
来源：http://twf.hcnkem.com

PHP:  getcwd();
来源：http://idr.vehdjk.com

JS:   process.cwd()
来源：http://tty.xuanzx.com

TS:   process.cwd()
来源：http://rqz.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://cea.shangyingyoupin.top

Go:   os.Getwd()
来源：http://bon.fehbvm.com

Ruby: Dir.pwd
来源：http://oit.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://kqt.guowangkeji.top

[M05] 设置退出码
来源：http://opa.vehdjk.com

Py:   sys.exit(1)
来源：http://jie.shuidangran.top

PHP:  exit(1);
来源：http://kvq.vehdjk.com

JS:   process.exit(1)
来源：http://lwd.havefunace.top

TS:   process.exit(1)
来源：http://ago.9152youxi.cn

Java: System.exit(1)
来源：http://pfq.jyoumei.cn

Go:   os.Exit(1)
来源：http://jld.jinghuilouyu.cn

Ruby: exit 1
来源：http://kak.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lkf.gogol.net.cn

[M06] 向标准错误输出
来源：http://yaf.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://tka.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fej.chenlongwang.top

JS:   console.error("err")
来源：http://lfh.yonumen.top

TS:   console.error("err")
来源：http://lvd.xingfuxueyuan.xyz

Java: System.err.println("err")
来源：http://eww.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://obm.zhoulong.xyz

Ruby: warn "err"
来源：http://woq.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://fon.jinqigufen.top

[M07] 判断是否为主入口
来源：http://egg.birdmap.top

Py:   if __name__ == "__main__":
来源：http://sil.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qhw.zhongyouzk.top

JS:   require.main === module
来源：http://vvl.ivvv.top

TS:   require.main === module
来源：http://jcz.aibaodan.cn

Java: public static void main(String[] args)
来源：http://xfc.hammf.cn

Go:   func main()
来源：http://icx.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gfi.nwbrower.top

C#:   static void Main(string[] args)
来源：http://grw.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://shx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://exl.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://ovr.316326.xyz

JS:   process.platform;  process.version
来源：http://env.svipenyu.cn

TS:   process.platform;  process.version
来源：http://qqv.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wyg.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jtc.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rkm.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://luc.havefunace.top

================================================================================
来源：http://ccc.cdnleiting.top

N. 数据结构与算法
来源：http://azi.haohaochexian.top

================================================================================
来源：http://sjk.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://gep.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://owa.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sbx.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msz.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xby.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kep.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://czn.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ilh.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://cun.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://cev.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://ddt.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dck.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lus.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://isg.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ytt.wangdashe.top

Go:   slices.Sort(arr)
来源：http://mfr.hongshengwenyu.top

Ruby: arr.sort
来源：http://uue.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rtz.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://rlx.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nla.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://dbr.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qxb.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dnl.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ynb.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jar.zhongyouzk.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vei.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://lfw.hesvh.cn

[N04] 斐波那契数列
来源：http://rti.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kgj.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kxg.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aun.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bvt.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqn.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dbt.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uck.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gdu.hysaishi.cn

[N05] 最大公约数
来源：http://mjq.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://uxu.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oud.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kjm.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpq.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pyj.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpk.52xcode.cn

Ruby: a.gcd(b)
来源：http://hyp.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zkq.yj20258.top

[N06] 判断回文字符串
来源：http://rsn.redwolf501.top

Py:   s == s[::-1]
来源：http://ggj.yvedp.cn

PHP:  $s === strrev($s);
来源：http://sxo.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://fex.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://mgj.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uug.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://loh.fktsv.cn

Ruby: s == s.reverse
来源：http://msa.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pjf.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://qvb.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://scx.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://toi.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nph.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://lsi.yfazqb.com

Java: // 手写 HashMap
来源：http://ovq.cucudq.cn

Go:   // 手写 map[int]int
来源：http://ukp.0kj1m.cn

Ruby: // 手写 Hash
来源：http://pao.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://yst.jinghuilouyu.cn

[N08] 生成全排列
来源：http://zrm.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://tau.yuxming.cn

PHP:  // 手写递归交换
来源：http://cfx.cqqwz.cn

JS:   // 手写回溯递归
来源：http://nyz.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://cci.fzhhl.top

Java: // 手写回溯递归
来源：http://nmp.chenzaomai.com

Go:   // 手写回溯递归
来源：http://xul.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://cfg.jinqigufen.top

C#:   // 手写回溯递归
来源：http://auc.yonumen.top

[N09] 栈与队列
来源：http://ypn.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cwf.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iwj.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ihp.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nuu.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://meu.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xjs.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://klt.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vxi.9152youxi.cn

[N10] 链表节点定义
来源：http://bll.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hzp.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://puo.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gcj.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qki.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://pyf.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://rbd.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://gxg.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nyi.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://rkx.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ixq.gotoacloud.top

PHP:  // 手写递归函数
来源：http://rqg.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kgj.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lmt.tian-w.cn

Java: // 手写递归
来源：http://oxi.nwbrower.top

Go:   // 手写递归
来源：http://gck.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xax.zdqjudy.top

C#:   // 手写递归
来源：http://jrp.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uqp.dianchejie.cn


<!-- 参考信息 -->