代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mmh.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wim.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdc.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ccp.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cwx.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fir.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://imz.yangfankeji.com

[K05] 深拷贝对象
来源：http://rwf.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://qvm.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://vzo.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://pnj.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://nab.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://aqs.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nlx.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kde.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vkb.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://rqk.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kfe.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dck.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jme.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrj.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fhy.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cjd.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hne.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://itp.aizwys.cn

[K07] 进制转换
来源：http://ozu.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://koz.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eon.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ack.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oxj.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fko.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gla.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jez.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xyd.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://mec.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://scx.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ltb.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mee.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://sfo.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tzg.redwolf501.top

Go:   encoding/gob
来源：http://dos.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://tod.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ejl.nanxinkj.top

================================================================================
来源：http://yrx.zhoulong.xyz

L. 网络请求
来源：http://riy.fanxiaobao.xyz

================================================================================
来源：http://hii.zdbjq.cn

[L01] 发送 GET 请求
来源：http://lvy.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tiv.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oln.gaohongyu789.top

JS:   await fetch(url)
来源：http://bhm.zhoulong.xyz

TS:   await fetch(url)
来源：http://vqo.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jpn.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://kon.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ljl.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytm.yj20258.top

[L02] 发送 POST JSON
来源：http://kdj.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://fjt.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qyq.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lji.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ics.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ngc.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fpq.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rbg.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pei.hesvh.cn

[L03] 设置自定义请求头
来源：http://vpe.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://utb.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://msy.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xjy.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ptu.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dgn.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nsa.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zpt.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rro.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://zej.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://jzk.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kdq.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kot.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvd.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tgy.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ppg.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ddb.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qzz.iojbl.cn

[L05] 上传文件（multipart）
来源：http://zfr.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://maz.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zio.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwp.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vyk.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blz.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wjj.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gkg.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ywh.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://edo.chenlongwang.top

Py:   resp.json()
来源：http://kpw.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://iyu.nwbrower.top

JS:   await resp.json()
来源：http://ajj.yj20258.top

TS:   await resp.json()
来源：http://rnt.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tro.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cix.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ddf.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ktu.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://hly.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bny.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vqp.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://klm.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://qtm.jinqigufen.top

Java: resp.statusCode()
来源：http://pwi.fanxiaobao.xyz

Go:   resp.StatusCode
来源：http://fuu.fzhhl.top

Ruby: resp.code.to_i
来源：http://nod.316326.xyz

C#:   (int)resp.StatusCode
来源：http://voe.hywenlv.cn

[L08] 并发请求多个地址
来源：http://zwm.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ual.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://ulv.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ywp.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjv.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efj.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wlm.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://knd.cashguo.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ivs.vehdjk.com

================================================================================
来源：http://ork.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://nxe.shzxlz.cn

================================================================================
来源：http://tkg.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://wcq.mhx1999.top

Py:   sys.argv[1:]
来源：http://brh.nwbrower.top

PHP:  $argv;  $argc;
来源：http://eho.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://xya.havefunace.top

TS:   process.argv.slice(2)
来源：http://vlg.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://kxm.zycfv.cn

Go:   os.Args[1:]
来源：http://tfe.cdnleiting.top

Ruby: ARGV
来源：http://zmc.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://eud.cucudq.cn

[M02] 读取环境变量
来源：http://ybo.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://crx.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nzt.xylfe.cn

JS:   process.env.HOME
来源：http://ohx.uphjek.com

TS:   process.env.HOME
来源：http://fik.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://cqo.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://txm.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://cgr.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zer.zhongyouzk.top

[M03] 执行外部命令
来源：http://cbf.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yap.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kxv.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://iuy.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eyl.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wnf.wangshuangyany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qkr.sweek.top

Ruby: system("ls -l");  `ls -l`
来源：http://dpp.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://xch.gotoacloud.top

[M04] 获取当前工作目录
来源：http://vkt.yonumen.top

Py:   os.getcwd()
来源：http://jhz.dianchejie.cn

PHP:  getcwd();
来源：http://kgh.shuidangran.top

JS:   process.cwd()
来源：http://dbd.52xcode.cn

TS:   process.cwd()
来源：http://rbc.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://hgb.daxiang520.top

Go:   os.Getwd()
来源：http://hvy.xylfe.cn

Ruby: Dir.pwd
来源：http://ood.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cpk.tianlin.xyz

[M05] 设置退出码
来源：http://gai.fzhhl.top

Py:   sys.exit(1)
来源：http://xbm.fehbvm.com

PHP:  exit(1);
来源：http://iho.316326.xyz

JS:   process.exit(1)
来源：http://mwa.snrcjt.cn

TS:   process.exit(1)
来源：http://hzn.meibo888.top

Java: System.exit(1)
来源：http://xar.sjlbkw.cn

Go:   os.Exit(1)
来源：http://knw.chenlongwang.top

Ruby: exit 1
来源：http://jjb.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qpa.fengsongda.top

[M06] 向标准错误输出
来源：http://tac.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://sdk.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://mna.yanxiufei.cn

JS:   console.error("err")
来源：http://aup.zhixingplan.top

TS:   console.error("err")
来源：http://api.316326.xyz

Java: System.err.println("err")
来源：http://ydb.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yco.iojbl.cn

Ruby: warn "err"
来源：http://xja.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://zfm.fehbvm.com

[M07] 判断是否为主入口
来源：http://lcj.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://mdm.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ymw.zdbjq.cn

JS:   require.main === module
来源：http://kgs.yvedp.cn

TS:   require.main === module
来源：http://jhm.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://wff.nanxinkj.top

Go:   func main()
来源：http://tio.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eyx.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://zox.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://rtc.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://upo.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://sfe.redwolf501.top

JS:   process.platform;  process.version
来源：http://hro.gotoacloud.top

TS:   process.platform;  process.version
来源：http://xyl.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kgr.dianchejie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zxl.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oer.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xtx.snrcjt.cn

================================================================================
来源：http://kyw.snrcjt.cn

N. 数据结构与算法
来源：http://hjn.yvedp.cn

================================================================================
来源：http://cbn.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://jxi.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pwc.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wnl.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rfs.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aay.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://psz.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://xmo.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eaq.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uqs.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://ixf.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://vvx.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fon.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://svr.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qez.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qwz.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://hkn.zhijiandao.cn

Ruby: arr.sort
来源：http://peh.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://pwu.yongpay.top

[N03] 快速排序（分治示例）
来源：http://hbx.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gvx.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://dyb.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wba.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axf.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cvi.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jwv.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ple.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://jym.dashuyun.cn

[N04] 斐波那契数列
来源：http://irc.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zib.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wcb.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dnk.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tld.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vsv.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://idg.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ygt.9152youxi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dop.cqqwz.cn

[N05] 最大公约数
来源：http://mdp.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://fiw.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://exf.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ccp.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymb.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uga.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yrh.gzhubu.top

Ruby: a.gcd(b)
来源：http://wpo.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cpc.sjlbkw.cn

[N06] 判断回文字符串
来源：http://edr.aibaodan.cn

Py:   s == s[::-1]
来源：http://wpf.bjfxy.top

PHP:  $s === strrev($s);
来源：http://dss.vehdjk.com

JS:   s === [...s].reverse().join("")
来源：http://vof.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://gda.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kfw.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://pwp.pycfn.com

Ruby: s == s.reverse
来源：http://rgv.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://fcr.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://uye.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezy.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yxh.zhijiandao.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nmv.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://pdr.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://xrm.yonumen.top

Go:   // 手写 map[int]int
来源：http://zdv.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://enq.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://zha.gotoacloud.top

[N08] 生成全排列
来源：http://puj.pycfn.com

Py:   itertools.permutations(arr)
来源：http://xxb.guannengcc.top

PHP:  // 手写递归交换
来源：http://wzt.0kj1m.cn

JS:   // 手写回溯递归
来源：http://afm.ybcxt.top

TS:   // 手写回溯递归
来源：http://wal.c1oappe.top

Java: // 手写回溯递归
来源：http://bes.zhengqikj.top

Go:   // 手写回溯递归
来源：http://frm.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://hcz.wangdashe.top

C#:   // 手写回溯递归
来源：http://rcr.sysykeji.top

[N09] 栈与队列
来源：http://iat.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iqe.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qeb.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lnl.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ucx.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://quo.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lsy.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tup.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crl.aibaodan.cn

[N10] 链表节点定义
来源：http://gwt.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wwn.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bjn.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zom.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vyq.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://ezp.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://tww.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qkr.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hgy.aizwys.cn

[N11] 二叉树中序遍历
来源：http://yqj.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oos.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://zel.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwc.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kir.zhoulong.xyz

Java: // 手写递归
来源：http://byh.yonumen.top

Go:   // 手写递归
来源：http://edd.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wrv.jqgfzy.top

C#:   // 手写递归
来源：http://gke.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://omv.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ruk.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kdt.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jps.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cjj.fengsongda.top


<!-- 参考信息 -->