代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oqp.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yum.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmh.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gjl.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vit.cqqwz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://brs.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://izg.zhoulong.xyz

[K05] 深拷贝对象
来源：http://grm.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://gap.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://ofp.yj20258.top

JS:   structuredClone(obj)
来源：http://ajy.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://heo.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://brp.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ltt.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dvn.vqdsnc.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ufd.wangdashe.top

[K06] 解析 URL 查询串
来源：http://mdd.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oge.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gag.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kkc.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://frj.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jlq.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xaa.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://idg.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rkg.ivvv.top

[K07] 进制转换
来源：http://qrd.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yhb.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rdu.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qni.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rnt.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xtd.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hyx.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pkb.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://adi.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://suy.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://qwr.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yxt.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://gjh.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://shr.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bwc.jinghuilouyu.cn

Go:   encoding/gob
来源：http://naz.tarul.cn

Ruby: Marshal.dump(obj)
来源：http://awp.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lft.c1oappe.top

================================================================================
来源：http://liq.yuxming.cn

L. 网络请求
来源：http://tji.snrcjt.cn

================================================================================
来源：http://mnv.ydzc1.top

[L01] 发送 GET 请求
来源：http://duz.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jed.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cjn.jianghu66.top

JS:   await fetch(url)
来源：http://pje.dashuyun.cn

TS:   await fetch(url)
来源：http://qef.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://esv.vehdjk.com

Go:   resp, err := http.Get(url)
来源：http://rwy.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bqe.jqgufenzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mqp.sufxvd.cn

[L02] 发送 POST JSON
来源：http://cll.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://buo.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hlh.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jya.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ybc.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jml.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dre.redwolf501.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tlx.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mfb.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://wib.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jtw.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://umh.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbp.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxv.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xnd.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ysb.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fle.hnqzz.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cgx.shuidangran.top

[L04] 设置超时
来源：http://fsv.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://gvi.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lmq.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bvd.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqm.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://twa.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://inu.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cte.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xby.epnwcf.com

[L05] 上传文件（multipart）
来源：http://gje.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bog.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fya.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nnu.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://taw.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://krc.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aeu.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://izd.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aev.pycfn.com

[L06] 解析响应为 JSON
来源：http://jpj.dashuyun.cn

Py:   resp.json()
来源：http://qhl.tanke756.top

PHP:  json_decode($body, true);
来源：http://wrq.meibo888.top

JS:   await resp.json()
来源：http://lkh.xinyue.icu

TS:   await resp.json()
来源：http://vaz.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qly.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yix.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://cxc.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://trz.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://cia.fengsongda.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ibp.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dmy.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://xcm.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://xan.yvedp.cn

Java: resp.statusCode()
来源：http://jsb.zhijiandao.cn

Go:   resp.StatusCode
来源：http://ufg.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://tkg.cheryme.top

C#:   (int)resp.StatusCode
来源：http://idq.0kj1m.cn

[L08] 并发请求多个地址
来源：http://dii.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ldf.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://sko.gaohongyu789.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fgb.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoj.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dow.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sko.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jcj.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cfa.guannengcc.top

================================================================================
来源：http://khf.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://eli.hesvh.cn

================================================================================
来源：http://pvp.tarul.cn

[M01] 读取命令行参数
来源：http://djk.cashguo.top

Py:   sys.argv[1:]
来源：http://xnq.sxryk.cn

PHP:  $argv;  $argc;
来源：http://qlt.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://doe.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://vnx.yonumen.top

Java: args 数组（main 方法参数）
来源：http://cix.zhengqikj.top

Go:   os.Args[1:]
来源：http://apz.dianchejie.cn

Ruby: ARGV
来源：http://jtg.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://xsu.yuanzhike.top

[M02] 读取环境变量
来源：http://tyn.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://pmj.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ynm.sufxvd.cn

JS:   process.env.HOME
来源：http://men.pengpengdd.cyou

TS:   process.env.HOME
来源：http://ykr.sufxvd.cn

Java: System.getenv("HOME")
来源：http://sxt.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://etz.cucudq.cn

Ruby: ENV["HOME"]
来源：http://dhe.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qzw.daria6918.cn

[M03] 执行外部命令
来源：http://dad.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://las.dianchejie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mxg.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bnh.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dcm.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lud.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kse.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xzl.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://vbo.cucudq.cn

[M04] 获取当前工作目录
来源：http://els.nwbrower.top

Py:   os.getcwd()
来源：http://pfm.nanxinkj.top

PHP:  getcwd();
来源：http://fij.jqgufenzy.top

JS:   process.cwd()
来源：http://gdh.guannengcc.top

TS:   process.cwd()
来源：http://cjl.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://dai.ybcxt.top

Go:   os.Getwd()
来源：http://xuc.hcnkem.com

Ruby: Dir.pwd
来源：http://ppv.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://udz.yj20258.top

[M05] 设置退出码
来源：http://cjj.ydjk.org.cn

Py:   sys.exit(1)
来源：http://yrr.yfazqb.com

PHP:  exit(1);
来源：http://auq.fzhhl.top

JS:   process.exit(1)
来源：http://edo.xinyue.icu

TS:   process.exit(1)
来源：http://tkc.jinqigufen.top

Java: System.exit(1)
来源：http://sut.birdmap.top

Go:   os.Exit(1)
来源：http://rop.sxryk.cn

Ruby: exit 1
来源：http://pqk.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://goz.svipenyu.cn

[M06] 向标准错误输出
来源：http://hrx.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://uog.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pfl.cheryme.top

JS:   console.error("err")
来源：http://hor.xinyue.icu

TS:   console.error("err")
来源：http://ycq.chenjidiqi.icu

Java: System.err.println("err")
来源：http://sry.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pri.fanxiaobao.xyz

Ruby: warn "err"
来源：http://vjy.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://gjg.xuanzx.com

[M07] 判断是否为主入口
来源：http://kwr.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://jaw.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dbf.zycfv.cn

JS:   require.main === module
来源：http://keq.xziqi.cn

TS:   require.main === module
来源：http://duw.hysaishi.cn

Java: public static void main(String[] args)
来源：http://tfx.jinqigufen.top

Go:   func main()
来源：http://dgx.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ykb.daxiang520.top

C#:   static void Main(string[] args)
来源：http://pfl.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://mpj.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://dch.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://xjq.52xcode.cn

JS:   process.platform;  process.version
来源：http://qfy.epnwcf.com

TS:   process.platform;  process.version
来源：http://pny.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nky.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ijg.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vof.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kbf.cashguo.top

================================================================================
来源：http://ckd.zdqjudy.top

N. 数据结构与算法
来源：http://fue.smart0.xyz

================================================================================
来源：http://cab.sweek.top

[N01] 二分查找（有序数组）
来源：http://zwc.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zjs.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jpi.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uio.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dzf.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://hvd.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://erd.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qpa.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ceu.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://zkl.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://fir.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://flc.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://gsh.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qmc.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mot.hnqzz.top

Go:   slices.Sort(arr)
来源：http://onk.fengsongda.top

Ruby: arr.sort
来源：http://zox.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eee.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://dte.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yrf.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://ssr.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lre.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipr.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wij.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zwo.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nvz.quarkkingdee.top

C#:   // 手写递归，或 Array.Sort
来源：http://jdj.aizwys.cn

[N04] 斐波那契数列
来源：http://vhd.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nsj.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aey.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gzz.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hlw.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://heq.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qqf.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bfu.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jiy.zhixingplan.top

[N05] 最大公约数
来源：http://tij.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://pqd.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xqw.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpf.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msm.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ocg.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pad.daxiang520.top

Ruby: a.gcd(b)
来源：http://cpt.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xan.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://par.jinqigfzy.top

Py:   s == s[::-1]
来源：http://vap.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://wkf.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://uvf.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://bnq.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dit.hnqzz.top

Go:   // 双指针从两端比较
来源：http://cxu.quarkkingdee.top

Ruby: s == s.reverse
来源：http://blp.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssb.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://elh.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lvo.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://acs.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vrf.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://ukv.guannengcc.top

Java: // 手写 HashMap
来源：http://otj.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://kdg.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://lhx.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://uco.shanyushiyangtech.top

[N08] 生成全排列
来源：http://cgo.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://mmk.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://pcy.zdbjq.cn

JS:   // 手写回溯递归
来源：http://yxn.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://kik.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://zsw.zycfv.cn

Go:   // 手写回溯递归
来源：http://pxa.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://yxm.mhx1999.top

C#:   // 手写回溯递归
来源：http://etp.xinyue.icu

[N09] 栈与队列
来源：http://lih.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkp.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ged.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cfy.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cwj.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pri.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fda.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xbs.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xgs.xinyue.icu

[N10] 链表节点定义
来源：http://sxd.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oib.jinqigufen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rlr.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nyp.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://maa.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://kwe.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dcy.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fop.pengpengdd.cyou

C#:   class Node { public int V; public Node? Next; }
来源：http://kyp.sxryk.cn

[N11] 二叉树中序遍历
来源：http://ysd.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hag.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://xdd.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://enp.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mng.c1oappe.top

Java: // 手写递归
来源：http://rnx.ehwqpu.com

Go:   // 手写递归
来源：http://bsb.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://crp.zycfv.cn

C#:   // 手写递归
来源：http://xrt.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xqf.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hgh.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kdq.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wqt.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://snc.wangshuangyany.cn


<!-- 参考信息 -->